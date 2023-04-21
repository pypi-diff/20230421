# Comparing `tmp/pydvma-0.9.0.tar.gz` & `tmp/pydvma-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydvma-0.9.0.tar", last modified: Wed Apr 19 20:58:21 2023, max compression
+gzip compressed data, was "pydvma-0.9.1.tar", last modified: Fri Apr 21 09:25:59 2023, max compression
```

## Comparing `pydvma-0.9.0.tar` & `pydvma-0.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tore       (501) staff       (20)        0 2023-04-19 20:58:21.700582 pydvma-0.9.0/
--rw-r--r--   0 tore       (501) staff       (20)     1603 2022-01-23 21:29:32.000000 pydvma-0.9.0/LICENSE
--rw-r--r--   0 tore       (501) staff       (20)     3051 2023-04-19 20:58:21.700381 pydvma-0.9.0/PKG-INFO
--rw-r--r--   0 tore       (501) staff       (20)     2850 2023-04-18 16:49:03.000000 pydvma-0.9.0/README.md
-drwxr-xr-x   0 tore       (501) staff       (20)        0 2023-04-19 20:58:21.699289 pydvma-0.9.0/pydvma/
--rw-r--r--   0 tore       (501) staff       (20)     1149 2023-04-19 18:08:23.000000 pydvma-0.9.0/pydvma/__init__.py
--rw-r--r--   0 tore       (501) staff       (20)    10546 2023-04-19 17:23:28.000000 pydvma-0.9.0/pydvma/acquisition.py
--rw-r--r--   0 tore       (501) staff       (20)    15939 2023-04-19 17:23:29.000000 pydvma-0.9.0/pydvma/analysis.py
--rw-r--r--   0 tore       (501) staff       (20)    29939 2023-04-19 17:23:31.000000 pydvma-0.9.0/pydvma/datastructure.py
--rw-r--r--   0 tore       (501) staff       (20)    16198 2023-04-19 17:23:32.000000 pydvma-0.9.0/pydvma/file.py
--rw-r--r--   0 tore       (501) staff       (20)   123535 2023-04-19 18:11:37.000000 pydvma-0.9.0/pydvma/gui.py
--rw-r--r--   0 tore       (501) staff       (20)     2718 2023-04-13 15:37:51.000000 pydvma-0.9.0/pydvma/gui_tk.py
--rw-r--r--   0 tore       (501) staff       (20)   144611 2023-04-06 11:15:26.000000 pydvma-0.9.0/pydvma/icon.png
--rw-r--r--   0 tore       (501) staff       (20)    10266 2023-04-19 17:23:39.000000 pydvma-0.9.0/pydvma/modal.py
--rw-r--r--   0 tore       (501) staff       (20)     7853 2023-04-19 17:23:42.000000 pydvma-0.9.0/pydvma/options.py
--rw-r--r--   0 tore       (501) staff       (20)    14580 2023-04-19 18:02:41.000000 pydvma-0.9.0/pydvma/oscilloscope.py
--rw-r--r--   0 tore       (501) staff       (20)    27099 2023-04-19 17:23:46.000000 pydvma-0.9.0/pydvma/plotting.py
--rw-r--r--   0 tore       (501) staff       (20)    25560 2023-04-19 17:23:48.000000 pydvma-0.9.0/pydvma/streams.py
--rw-r--r--   0 tore       (501) staff       (20)     2778 2023-04-19 17:56:13.000000 pydvma-0.9.0/pydvma/testdata.py
-drwxr-xr-x   0 tore       (501) staff       (20)        0 2023-04-19 20:58:21.700151 pydvma-0.9.0/pydvma.egg-info/
--rw-r--r--   0 tore       (501) staff       (20)     3051 2023-04-19 20:58:21.000000 pydvma-0.9.0/pydvma.egg-info/PKG-INFO
--rw-r--r--   0 tore       (501) staff       (20)      434 2023-04-19 20:58:21.000000 pydvma-0.9.0/pydvma.egg-info/SOURCES.txt
--rw-r--r--   0 tore       (501) staff       (20)        1 2023-04-19 20:58:21.000000 pydvma-0.9.0/pydvma.egg-info/dependency_links.txt
--rw-r--r--   0 tore       (501) staff       (20)       63 2023-04-19 20:58:21.000000 pydvma-0.9.0/pydvma.egg-info/requires.txt
--rw-r--r--   0 tore       (501) staff       (20)        7 2023-04-19 20:58:21.000000 pydvma-0.9.0/pydvma.egg-info/top_level.txt
--rw-r--r--   0 tore       (501) staff       (20)       38 2023-04-19 20:58:21.700639 pydvma-0.9.0/setup.cfg
--rw-r--r--   0 tore       (501) staff       (20)      596 2023-04-18 16:42:23.000000 pydvma-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:25:59.648021 pydvma-0.9.1/
+-rw-rw-rw-   0        0        0     1634 2022-04-26 11:34:19.000000 pydvma-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     3150 2023-04-21 09:25:59.647501 pydvma-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2940 2023-04-19 10:31:43.000000 pydvma-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 09:25:59.633733 pydvma-0.9.1/pydvma/
+-rw-rw-rw-   0        0        0     1165 2023-04-20 11:25:15.000000 pydvma-0.9.1/pydvma/__init__.py
+-rw-rw-rw-   0        0        0    10825 2023-04-20 11:25:15.000000 pydvma-0.9.1/pydvma/acquisition.py
+-rw-rw-rw-   0        0        0    16393 2023-04-20 11:25:15.000000 pydvma-0.9.1/pydvma/analysis.py
+-rw-rw-rw-   0        0        0    30676 2023-04-21 09:25:02.000000 pydvma-0.9.1/pydvma/datastructure.py
+-rw-rw-rw-   0        0        0    16695 2023-04-19 14:11:21.000000 pydvma-0.9.1/pydvma/file.py
+-rw-rw-rw-   0        0        0   126389 2023-04-20 11:25:15.000000 pydvma-0.9.1/pydvma/gui.py
+-rw-rw-rw-   0        0        0     2815 2023-04-19 10:31:43.000000 pydvma-0.9.1/pydvma/gui_tk.py
+-rw-rw-rw-   0        0        0   144611 2023-04-19 10:31:43.000000 pydvma-0.9.1/pydvma/icon.png
+-rw-rw-rw-   0        0        0    10628 2023-04-20 11:25:15.000000 pydvma-0.9.1/pydvma/modal.py
+-rw-rw-rw-   0        0        0     8111 2023-04-21 09:24:50.000000 pydvma-0.9.1/pydvma/options.py
+-rw-rw-rw-   0        0        0    14944 2023-04-20 11:25:15.000000 pydvma-0.9.1/pydvma/oscilloscope.py
+-rw-rw-rw-   0        0        0    27763 2023-04-20 11:25:15.000000 pydvma-0.9.1/pydvma/plotting.py
+-rw-rw-rw-   0        0        0    26182 2023-04-20 11:25:15.000000 pydvma-0.9.1/pydvma/streams.py
+-rw-rw-rw-   0        0        0     2871 2023-04-20 11:25:15.000000 pydvma-0.9.1/pydvma/testdata.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:25:59.645074 pydvma-0.9.1/pydvma.egg-info/
+-rw-rw-rw-   0        0        0     3150 2023-04-21 09:25:59.000000 pydvma-0.9.1/pydvma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-21 09:25:59.000000 pydvma-0.9.1/pydvma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:25:59.000000 pydvma-0.9.1/pydvma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-21 09:25:59.000000 pydvma-0.9.1/pydvma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 09:25:59.000000 pydvma-0.9.1/pydvma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:25:59.648656 pydvma-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-04-21 09:25:11.000000 pydvma-0.9.1/setup.py
```

### Comparing `pydvma-0.9.0/LICENSE` & `pydvma-0.9.1/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-BSD 3-Clause License
-
-Copyright (c) 2020, Tore Butlin
-Contributors: Tore Butlin, Jim Woodhouse, Areeg Emarah, En Yi Tee, Theo Brown, Rick Lupton
-
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2020, Tore Butlin
+Contributors: Tore Butlin, Jim Woodhouse, Areeg Emarah, En Yi Tee, Theo Brown, Rick Lupton
+
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `pydvma-0.9.0/PKG-INFO` & `pydvma-0.9.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,90 @@
-Metadata-Version: 2.1
-Name: pydvma
-Version: 0.9.0
-Home-page: https://github.com/torebutlin/pydvma
-Author: Tore Butlin
-Author-email: tb267@cam.ac.uk
-License: BSD 3-Clause License
-License-File: LICENSE
-
-# pydvma
-
-A Python package for dynamics and vibration measurements and analysis.
-
-
-## About pydvma
-
-This is a modular library for data measurement and analysis in the context of dynamics and vibration, for use in student laboratory experiments as well as for research projects, developed at Cambridge University Engineering Department.
-
-A high-level interface allows straightforward application for common use-cases and a low-level interface provides more control when needed.
-
-The aim is for a library that is simple to use and simple to maintain. It is not a full-featured GUI, but when used in conjunction with Jupyter Notebooks it is intended to provide the best of both worlds: interactive tools for common tasks and a command line interface for customisation.
-
-
-## Getting started
-
-### Installation
-
-The logger is recommended for use with Python 3.10.
-
-```
-pip install pydvma
-```
-
-If you would like soundcard acquisition then also install sounddevice:
-```
-pip install sounddevice
-```
-
-Or clone this repository and install using:
-```
-python setup.py install
-```
-
-Alternatively you can use the environment yml file provided:
-```
-conda env -name logger create -f logger.yml
-conda activate logger
-```
-
-### Running the logger
-
-To get started, open the file:
-```
-pydvma_template.ipynb
-```
-
-or within a Jupyter Notebook or Python console:
-```python
-%gui qt
-import pydvma as dvma
-settings = dvma.MySettings()
-osc = dvma.Oscilloscope(settings)
-logger = dvma.Logger(settings)
-```
-
-## Roadmap
-
-At present the library has basic functionality for:
-
-- logging data using soundcards or National Instrument DAQs (requires NiDAQmx to be installed from NI, windows only)
-- logging with pre-trigger for impulse response measurements
-- logging with pc generated output (soundcard and NIDAQ)
-- computing frequency domain data
-- computing transfer function data
-- computing sonograms/spectrograms
-- basic modal analysis tools (mode-fitting)
-- saving and plotting data
-- export to Matlab
-- interactive tools for standard acquisition and analysis
-- oscilloscope view of input signals
-
-The plan is to include the following functionality:
-
-- wider support for import/export
-- more advanced modal analysis tools (e.g. global fitting)
-- extend the range of hardware that can be accessed from this library
-
-
-## Contributer guidelines
-
-Contributions to this project are welcomed, keeping in mind the project aims above:
-
-- If you find a bug, please report using GitHub's issue tracker
-
-- For bug-fixes and refinements: please feel free to clone the repository, make edits and create a pull request with a clear description of changes made.
-
-- If you would like to make a more significant contribution or change, then please be in contact to outline your suggestion.
-
-Please see the documentation for details of the code structure and templates for anticipated applications.
+# pydvma
+
+A Python package for dynamics and vibration measurements and analysis.
+
+
+## About pydvma
+
+This is a modular library for data measurement and analysis in the context of dynamics and vibration, for use in student laboratory experiments as well as for research projects, developed at Cambridge University Engineering Department.
+
+A high-level interface allows straightforward application for common use-cases and a low-level interface provides more control when needed.
+
+The aim is for a library that is simple to use and simple to maintain. It is not a full-featured GUI, but when used in conjunction with Jupyter Notebooks it is intended to provide the best of both worlds: interactive tools for common tasks and a command line interface for customisation.
+
+
+## Getting started
+
+### Installation
+
+The logger is recommended for use with Python 3.10.
+
+```
+pip install pydvma
+```
+
+If you would like soundcard acquisition then also install sounddevice:
+```
+pip install sounddevice
+```
+
+Or clone this repository and install using:
+```
+python setup.py install
+```
+
+Alternatively you can use the environment yml file provided:
+```
+conda env -name logger create -f logger.yml
+conda activate logger
+```
+
+### Running the logger
+
+To get started, open the file:
+```
+pydvma_template.ipynb
+```
+
+or within a Jupyter Notebook or Python console:
+```python
+%gui qt
+import pydvma as dvma
+settings = dvma.MySettings()
+osc = dvma.Oscilloscope(settings)
+logger = dvma.Logger(settings)
+```
+
+## Roadmap
+
+At present the library has basic functionality for:
+
+- logging data using soundcards or National Instrument DAQs (requires NiDAQmx to be installed from NI, windows only)
+- logging with pre-trigger for impulse response measurements
+- logging with pc generated output (soundcard and NIDAQ)
+- computing frequency domain data
+- computing transfer function data
+- computing sonograms/spectrograms
+- basic modal analysis tools (mode-fitting)
+- saving and plotting data
+- export to Matlab
+- interactive tools for standard acquisition and analysis
+- oscilloscope view of input signals
+
+The plan is to include the following functionality:
+
+- wider support for import/export
+- more advanced modal analysis tools (e.g. global fitting)
+- extend the range of hardware that can be accessed from this library
+
+
+## Contributer guidelines
+
+Contributions to this project are welcomed, keeping in mind the project aims above:
+
+- If you find a bug, please report using GitHub's issue tracker
+
+- For bug-fixes and refinements: please feel free to clone the repository, make edits and create a pull request with a clear description of changes made.
+
+- If you would like to make a more significant contribution or change, then please be in contact to outline your suggestion.
+
+Please see the documentation for details of the code structure and templates for anticipated applications.
```

### Comparing `pydvma-0.9.0/pydvma/__init__.py` & `pydvma-0.9.1/pydvma/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from .gui import Logger, Oscilloscope
-from .options import MySettings, set_plot_colours
-from .file import load_data, save_data, save_fig, export_to_matlab_jwlogger, export_to_matlab, export_to_csv
-# from .oscilloscope import Oscilloscope
-from .acquisition import log_data, log_data_with_output, output_signal, signal_generator, stream_snapshot
-from .datastructure import DataSet, TimeData, FreqData, CrossSpecData, TfData, SonoData, MetaData, ModalData, update_dataset
-from .testdata import create_test_impulse_data, create_test_impulse_ensemble, create_test_noise_data
-from .plotting import PlotData
-from .analysis import calculate_fft, calculate_cross_spectrum_matrix, calculate_cross_spectra_averaged, clean_impulse
-from .analysis import calculate_tf, calculate_tf_averaged, multiply_by_power_of_iw, best_match, calculate_sonogram
-from .streams import Recorder, Recorder_NI, start_stream, REC, setup_output_NI, setup_output_soundcard, list_available_devices, get_devices_NI, get_devices_soundcard
-from .modal import modal_fit_single_channel, modal_fit_all_channels
-# import faulthandler
-# faulthandler.enable()
-# from .gui_tk_test import Logger
-
+from .gui import Logger, Oscilloscope
+from .options import MySettings, set_plot_colours
+from .file import load_data, save_data, save_fig, export_to_matlab_jwlogger, export_to_matlab, export_to_csv
+# from .oscilloscope import Oscilloscope
+from .acquisition import log_data, log_data_with_output, output_signal, signal_generator, stream_snapshot
+from .datastructure import DataSet, TimeData, FreqData, CrossSpecData, TfData, SonoData, MetaData, ModalData, update_dataset
+from .testdata import create_test_impulse_data, create_test_impulse_ensemble, create_test_noise_data
+from .plotting import PlotData
+from .analysis import calculate_fft, calculate_cross_spectrum_matrix, calculate_cross_spectra_averaged, clean_impulse
+from .analysis import calculate_tf, calculate_tf_averaged, multiply_by_power_of_iw, best_match, calculate_sonogram
+from .streams import Recorder, Recorder_NI, start_stream, REC, setup_output_NI, setup_output_soundcard, list_available_devices, get_devices_NI, get_devices_soundcard
+from .modal import modal_fit_single_channel, modal_fit_all_channels
+# import faulthandler
+# faulthandler.enable()
+# from .gui_tk_test import Logger
+
```

### Comparing `pydvma-0.9.0/pydvma/acquisition.py` & `pydvma-0.9.1/pydvma/acquisition.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,280 +1,280 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Aug 27 17:08:42 2018
-
-@author: tb267
-"""
-
-from . import datastructure
-from . import streams
-
-import numpy as np
-import scipy.signal as signal
-import scipy.stats as stats
-import datetime
-import time
-
-MESSAGE = ''
-
-#%% Main data acquisition function
-def log_data(settings,test_name=None,rec=None, output=None):
-    '''
-    Logs data according to settings and returns DataSet class
-    '''
-    global MESSAGE
-    
-    if rec is None:
-        streams.start_stream(settings)
-        rec = streams.REC
-        
-    
-    streams.REC.trigger_detected = False
-    
-    # Stream is slightly longer than settings.stored_time, so need to add delay
-    # from initialisation to allow stream to fill up and prevent zeros at start
-    # of logged data.
-    time.sleep(2*settings.chunk_size/settings.fs)
-    t = datetime.datetime.now()
-    timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)
-    
-    if settings.pretrig_samples == None:
-
-        MESSAGE = 'Logging data for {} seconds.\n'.format(settings.stored_time)
-        print(MESSAGE)
-        
-        
-        # basic way to control logging time: won't be precise time from calling function
-        # also won't be exactly synced to output signal
-        if output is not None:
-            s = output_signal(settings,output)
-            # rec.write(output.astype('float32'))
-        
-        if (settings.device_driver == 'nidaq') or (output is None): # nidaq output is nonblocking, but soundcard is blocking
-            time.sleep(settings.stored_time)
-        
-            
-        # make copy of data
-        stored_time_data_copy = np.copy(streams.REC.stored_time_data)
-        number_samples = int(streams.REC.settings.stored_time * streams.REC.settings.fs)
-        
-        stored_time_data_copy = stored_time_data_copy[-number_samples:,:]
-        MESSAGE += 'Logging complete.\n'
-        print(MESSAGE)
-
-        if output is not None:
-            if settings.output_device_driver == 'soundcard':
-                s.stop()
-                s.close()
-            if settings.output_device_driver == 'nidaq':
-                s.WaitUntilTaskDone(settings.stored_time+5)
-                s.StopTask()
-        
-
-        
-    else:
-        streams.REC.__init__(settings) # zeros buffers so looks for trigger in fresh data
-        streams.REC.trigger_detected = False # somehow this can be true even after previous call
-        streams.REC.trigger_first_detected_message = True
-        
-        MESSAGE = 'Waiting for trigger on channel {}.\n'.format(settings.pretrig_channel)
-        print(MESSAGE)
-        
-        start_output_flag = True
-        t0 = time.time()
-        while (time.time()-t0 < settings.pretrig_timeout) and not streams.REC.trigger_detected:
-            if (output is not None) and (start_output_flag == True): # start output within loop, but only once!
-                time.sleep(1)
-                MESSAGE = 'Starting output signal.\n'
-                print(MESSAGE)
-                s = output_signal(settings,output)
-                # rec.write(output.astype('float32'))
-                start_output_flag = False
-
-            time.sleep(0.2)
-        if (time.time()-t0 > settings.pretrig_timeout):
-            MESSAGE = 'Trigger not detected within timeout of {} seconds.\n'.format(settings.pretrig_timeout)
-            print(MESSAGE)
-        
-        # make copy of data
-        stored_time_data_copy = np.copy(streams.REC.stored_time_data)
-        trigger_check = stored_time_data_copy[(settings.chunk_size):(2*settings.chunk_size),settings.pretrig_channel]
-        detected_sample = settings.chunk_size + np.where(np.abs(trigger_check) > settings.pretrig_threshold)[0][0]
-        number_samples = int(settings.stored_time * settings.fs)
-        start_index = detected_sample - settings.pretrig_samples
-        end_index   = start_index + number_samples
-        streams.REC.trigger_detected = False # don't start stream again until sorted out trigger detection
-        
-        stored_time_data_copy = stored_time_data_copy[start_index:end_index,:]
-        
-        MESSAGE = 'Logging complete.\n'
-        print(MESSAGE)
-
-        if output is not None:
-            if settings.output_device_driver == 'soundcard':
-                s.stop()
-                s.close()
-            if settings.output_device_driver == 'nidaq':
-                s.WaitUntilTaskDone(settings.stored_time+5)
-                s.StopTask()
-        
-    # make into dataset
-    fs = settings.fs
-    n_samp = len(stored_time_data_copy[:,0])
-    dt = 1/fs
-    t_samp = n_samp*dt
-    time_axis = np.linspace(0,(n_samp-1)/n_samp * settings.stored_time,n_samp)
-    
-    if (output is not None) and (settings.use_output_as_ch0 == True):
-        stored_output = np.zeros((n_samp,len(output[0,:])))
-        n_start = settings.pretrig_samples
-        if n_start is None:
-            n_start = 0
-        n_end = np.copy(n_samp)
-        if len(output[:,0]) >= (n_end-n_start):
-            stored_output[n_start:n_end,:] = output[:n_end-n_start,:]
-        elif len(output[:,0]) < (n_end-n_start):
-            stored_output[n_start:len(output[:,0])+n_start,:] = output[:,:]
-            
-        stored_time_data_copy = np.concatenate((stored_output,stored_time_data_copy),axis=1)
-    
-    timedata = datastructure.TimeData(time_axis,stored_time_data_copy,settings,timestamp=t,timestring=timestring,test_name=test_name)
-    
-    
-    dataset  = datastructure.DataSet()
-    dataset.add_to_dataset(timedata)
-    
-    # check for clipping
-    if np.any(np.abs(stored_time_data_copy) > 0.95):
-        MESSAGE += 'WARNING: Data may be clipped'
-        print(MESSAGE)
-    
-    
-    return dataset
-    
-
-
-def log_data_with_output(settings, output,test_name=None, rec=None):
-
-    
-    # call log_data function
-    dataset = log_data(settings, test_name, rec)
-    
-    # call output_signal function
-    output_signal(settings,output)
-    
-    return dataset
-    
-
-
-def output_signal(settings,output):
-    # setup NI / audio stream
-    if settings.output_device_driver == 'soundcard':
-        s = streams.setup_output_soundcard(settings)
-        data = output.astype('float32')
-        s.write(data)
-        return s
-        
-    elif settings.output_device_driver == 'nidaq':
-        sh = np.shape(output)
-        T = sh[0]/settings.fs
-        s = streams.setup_output_NI(settings,output)
-        s.StartTask()
-        return s
-    else:
-        print('device_driver not recognised')
-        return None
-        
-    # send to device
-
-
-def signal_generator(settings,sig='gaussian',T=1,amplitude=0.1,f=None,selected_channels='all'):
-    """
-    Creates a signal ready for output to a chosen device
-    """
-    global MESSAGE
-    if selected_channels == 'all':
-        selected_channels = np.arange(0,settings.output_channels)
-       
-    # initiate variables
-    t = np.arange(0,T,1/settings.output_fs)
-    N_per_channel = np.size(t)
-    y = np.zeros((N_per_channel,settings.output_channels))
-    win = np.ones((N_per_channel,1))
-    T_ramp = np.min([T/10,0.1])
-    N_ramp = int(T_ramp*settings.output_fs)
-    win[0:N_ramp,0] = 0.5*(1-np.cos(np.arange(0,N_ramp)/N_ramp*np.pi))
-    win[-N_ramp:,0] = 0.5*(1+np.cos(np.arange(0,N_ramp)/N_ramp*np.pi))
-    
-    limit = 1 # generate signals normalised with amplitudes 0-1
-    
-    # Create sig. Note 'sig' is choice of signal, while 'signal' is scipy.signal
-    if sig == 'gaussian':
-        y[:,selected_channels] = np.random.randn(N_per_channel,np.size(selected_channels))
-        
-        
-        
-#        if settings.output_device_driver == 'soundcard':
-#            limit = 1
-#        elif settings.output_device_driver == 'nidaq':
-#            limit = settings.VmaxNI
-             
-                
-        y[:,selected_channels] = stats.truncnorm.rvs(-limit/amplitude, limit/amplitude, loc=0,scale=amplitude, size=(N_per_channel,np.size(selected_channels)))
-        if f is not None:
-            b,a = signal.butter(3,f,btype='bandpass',fs=settings.output_fs)
-            y = signal.filtfilt(b,a,y,axis=0,padtype=None)
-            y = amplitude * y / np.sqrt(np.mean(y**2))
-            if np.max(np.abs(y)) > limit:
-                y = limit * y / np.max(np.abs(y))
-                MESSAGE = 'Actual rms output after scaling to avoid clipping is {0:1.3f}'.format(np.sqrt(np.mean(y**2)))
-            else:
-                MESSAGE = 'Actual rms output is {0:1.3f}'.format(np.sqrt(np.mean(y**2)))
-                
-            
-#            N_exceed_lim = np.sum(y>limit)+np.sum(y<-limit)
-#            fraction_clipped = N_exceed_lim/np.size(y)
-#            y[y>limit] = limit
-#            y[y<-limit] = -limit
-#            if fraction_clipped > 0:
-#                print('{} out of {} samples exceeded output voltage limit of device and have been clipped'.format(N_exceed_lim,np.size(y)))
-#            if fraction_clipped > 0.01:
-#                print('{0:1.1f} percent of samples exceed output voltage limit of device'.format(fraction_clipped*100))
-                
-    elif sig == 'uniform':
-        y[:,selected_channels] = np.random.uniform(low=-amplitude,high=amplitude,size=(N_per_channel,np.size(selected_channels)))
-        if f is not None:
-            b,a = signal.butter(3,f,btype='bandpass',fs=settings.output_fs)
-            y = signal.filtfilt(b,a,y,axis=0,padtype=None)
-            y = amplitude * y / np.sqrt(np.mean(y**2))
-    elif sig == 'sweep':
-        if f is None:
-            f = [0,settings.output_fs/2]
-        
-        for ch in selected_channels:
-            y[:,ch] = amplitude*signal.chirp(t,f[0],T,f[1])
-    else:
-        print('signal type must be one of {''gaussian'',''uniform'',''sweep''}')
-        y = np.zeros((N_per_channel,settings.output_channels))
-    
-    y = win * y
-    
-    # final correction to ensure all signals limited to 0-1
-    if np.max(np.abs(y)) > limit:
-        y = limit * y / np.max(np.abs(y))
-        MESSAGE = 'Actual rms output after scaling to avoid clipping is {0:1.3f}'.format(np.sqrt(np.mean(y**2)))
-        
-    return t,y
-
-
-def stream_snapshot(rec):
-    
-    time_data_copy = np.copy(streams.REC.osc_time_data)
-    time_axis_copy = np.copy(streams.REC.osc_time_axis)
-    
-    t = datetime.datetime.now()
-    timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)    
-
-    time_data = datastructure.TimeData(time_axis_copy,time_data_copy,streams.REC.settings,timestamp=t,timestring=timestring,test_name='stream_snapshot')
-    
-    
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Aug 27 17:08:42 2018
+
+@author: tb267
+"""
+
+from . import datastructure
+from . import streams
+
+import numpy as np
+import scipy.signal as signal
+import scipy.stats as stats
+import datetime
+import time
+
+MESSAGE = ''
+
+#%% Main data acquisition function
+def log_data(settings,test_name=None,rec=None, output=None):
+    '''
+    Logs data according to settings and returns DataSet class
+    '''
+    global MESSAGE
+    
+    if rec is None:
+        streams.start_stream(settings)
+        rec = streams.REC
+        
+    
+    streams.REC.trigger_detected = False
+    
+    # Stream is slightly longer than settings.stored_time, so need to add delay
+    # from initialisation to allow stream to fill up and prevent zeros at start
+    # of logged data.
+    time.sleep(2*settings.chunk_size/settings.fs)
+    t = datetime.datetime.now()
+    timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)
+    
+    if settings.pretrig_samples == None:
+
+        MESSAGE = 'Logging data for {} seconds.\n'.format(settings.stored_time)
+        print(MESSAGE)
+        
+        
+        # basic way to control logging time: won't be precise time from calling function
+        # also won't be exactly synced to output signal
+        if output is not None:
+            s = output_signal(settings,output)
+            # rec.write(output.astype('float32'))
+        
+        if (settings.device_driver == 'nidaq') or (output is None): # nidaq output is nonblocking, but soundcard is blocking
+            time.sleep(settings.stored_time)
+        
+            
+        # make copy of data
+        stored_time_data_copy = np.copy(streams.REC.stored_time_data)
+        number_samples = int(streams.REC.settings.stored_time * streams.REC.settings.fs)
+        
+        stored_time_data_copy = stored_time_data_copy[-number_samples:,:]
+        MESSAGE += 'Logging complete.\n'
+        print(MESSAGE)
+
+        if output is not None:
+            if settings.output_device_driver == 'soundcard':
+                s.stop()
+                s.close()
+            if settings.output_device_driver == 'nidaq':
+                s.WaitUntilTaskDone(settings.stored_time+5)
+                s.StopTask()
+        
+
+        
+    else:
+        streams.REC.__init__(settings) # zeros buffers so looks for trigger in fresh data
+        streams.REC.trigger_detected = False # somehow this can be true even after previous call
+        streams.REC.trigger_first_detected_message = True
+        
+        MESSAGE = 'Waiting for trigger on channel {}.\n'.format(settings.pretrig_channel)
+        print(MESSAGE)
+        
+        start_output_flag = True
+        t0 = time.time()
+        while (time.time()-t0 < settings.pretrig_timeout) and not streams.REC.trigger_detected:
+            if (output is not None) and (start_output_flag == True): # start output within loop, but only once!
+                time.sleep(1)
+                MESSAGE = 'Starting output signal.\n'
+                print(MESSAGE)
+                s = output_signal(settings,output)
+                # rec.write(output.astype('float32'))
+                start_output_flag = False
+
+            time.sleep(0.2)
+        if (time.time()-t0 > settings.pretrig_timeout):
+            MESSAGE = 'Trigger not detected within timeout of {} seconds.\n'.format(settings.pretrig_timeout)
+            print(MESSAGE)
+        
+        # make copy of data
+        stored_time_data_copy = np.copy(streams.REC.stored_time_data)
+        trigger_check = stored_time_data_copy[(settings.chunk_size):(2*settings.chunk_size),settings.pretrig_channel]
+        detected_sample = settings.chunk_size + np.where(np.abs(trigger_check) > settings.pretrig_threshold)[0][0]
+        number_samples = int(settings.stored_time * settings.fs)
+        start_index = detected_sample - settings.pretrig_samples
+        end_index   = start_index + number_samples
+        streams.REC.trigger_detected = False # don't start stream again until sorted out trigger detection
+        
+        stored_time_data_copy = stored_time_data_copy[start_index:end_index,:]
+        
+        MESSAGE = 'Logging complete.\n'
+        print(MESSAGE)
+
+        if output is not None:
+            if settings.output_device_driver == 'soundcard':
+                s.stop()
+                s.close()
+            if settings.output_device_driver == 'nidaq':
+                s.WaitUntilTaskDone(settings.stored_time+5)
+                s.StopTask()
+        
+    # make into dataset
+    fs = settings.fs
+    n_samp = len(stored_time_data_copy[:,0])
+    dt = 1/fs
+    t_samp = n_samp*dt
+    time_axis = np.linspace(0,(n_samp-1)/n_samp * settings.stored_time,n_samp)
+    
+    if (output is not None) and (settings.use_output_as_ch0 == True):
+        stored_output = np.zeros((n_samp,len(output[0,:])))
+        n_start = settings.pretrig_samples
+        if n_start is None:
+            n_start = 0
+        n_end = np.copy(n_samp)
+        if len(output[:,0]) >= (n_end-n_start):
+            stored_output[n_start:n_end,:] = output[:n_end-n_start,:]
+        elif len(output[:,0]) < (n_end-n_start):
+            stored_output[n_start:len(output[:,0])+n_start,:] = output[:,:]
+            
+        stored_time_data_copy = np.concatenate((stored_output,stored_time_data_copy),axis=1)
+    
+    timedata = datastructure.TimeData(time_axis,stored_time_data_copy,settings,timestamp=t,timestring=timestring,test_name=test_name)
+    
+    
+    dataset  = datastructure.DataSet()
+    dataset.add_to_dataset(timedata)
+    
+    # check for clipping
+    if np.any(np.abs(stored_time_data_copy) > 0.95):
+        MESSAGE += 'WARNING: Data may be clipped'
+        print(MESSAGE)
+    
+    
+    return dataset
+    
+
+
+def log_data_with_output(settings, output,test_name=None, rec=None):
+
+    
+    # call log_data function
+    dataset = log_data(settings, test_name, rec)
+    
+    # call output_signal function
+    output_signal(settings,output)
+    
+    return dataset
+    
+
+
+def output_signal(settings,output):
+    # setup NI / audio stream
+    if settings.output_device_driver == 'soundcard':
+        s = streams.setup_output_soundcard(settings)
+        data = output.astype('float32')
+        s.write(data)
+        return s
+        
+    elif settings.output_device_driver == 'nidaq':
+        sh = np.shape(output)
+        T = sh[0]/settings.fs
+        s = streams.setup_output_NI(settings,output)
+        s.StartTask()
+        return s
+    else:
+        print('device_driver not recognised')
+        return None
+        
+    # send to device
+
+
+def signal_generator(settings,sig='gaussian',T=1,amplitude=0.1,f=None,selected_channels='all'):
+    """
+    Creates a signal ready for output to a chosen device
+    """
+    global MESSAGE
+    if selected_channels == 'all':
+        selected_channels = np.arange(0,settings.output_channels)
+       
+    # initiate variables
+    t = np.arange(0,T,1/settings.output_fs)
+    N_per_channel = np.size(t)
+    y = np.zeros((N_per_channel,settings.output_channels))
+    win = np.ones((N_per_channel,1))
+    T_ramp = np.min([T/10,0.1])
+    N_ramp = int(T_ramp*settings.output_fs)
+    win[0:N_ramp,0] = 0.5*(1-np.cos(np.arange(0,N_ramp)/N_ramp*np.pi))
+    win[-N_ramp:,0] = 0.5*(1+np.cos(np.arange(0,N_ramp)/N_ramp*np.pi))
+    
+    limit = 1 # generate signals normalised with amplitudes 0-1
+    
+    # Create sig. Note 'sig' is choice of signal, while 'signal' is scipy.signal
+    if sig == 'gaussian':
+        y[:,selected_channels] = np.random.randn(N_per_channel,np.size(selected_channels))
+        
+        
+        
+#        if settings.output_device_driver == 'soundcard':
+#            limit = 1
+#        elif settings.output_device_driver == 'nidaq':
+#            limit = settings.VmaxNI
+             
+                
+        y[:,selected_channels] = stats.truncnorm.rvs(-limit/amplitude, limit/amplitude, loc=0,scale=amplitude, size=(N_per_channel,np.size(selected_channels)))
+        if f is not None:
+            b,a = signal.butter(3,f,btype='bandpass',fs=settings.output_fs)
+            y = signal.filtfilt(b,a,y,axis=0,padtype=None)
+            y = amplitude * y / np.sqrt(np.mean(y**2))
+            if np.max(np.abs(y)) > limit:
+                y = limit * y / np.max(np.abs(y))
+                MESSAGE = 'Actual rms output after scaling to avoid clipping is {0:1.3f}'.format(np.sqrt(np.mean(y**2)))
+            else:
+                MESSAGE = 'Actual rms output is {0:1.3f}'.format(np.sqrt(np.mean(y**2)))
+                
+            
+#            N_exceed_lim = np.sum(y>limit)+np.sum(y<-limit)
+#            fraction_clipped = N_exceed_lim/np.size(y)
+#            y[y>limit] = limit
+#            y[y<-limit] = -limit
+#            if fraction_clipped > 0:
+#                print('{} out of {} samples exceeded output voltage limit of device and have been clipped'.format(N_exceed_lim,np.size(y)))
+#            if fraction_clipped > 0.01:
+#                print('{0:1.1f} percent of samples exceed output voltage limit of device'.format(fraction_clipped*100))
+                
+    elif sig == 'uniform':
+        y[:,selected_channels] = np.random.uniform(low=-amplitude,high=amplitude,size=(N_per_channel,np.size(selected_channels)))
+        if f is not None:
+            b,a = signal.butter(3,f,btype='bandpass',fs=settings.output_fs)
+            y = signal.filtfilt(b,a,y,axis=0,padtype=None)
+            y = amplitude * y / np.sqrt(np.mean(y**2))
+    elif sig == 'sweep':
+        if f is None:
+            f = [0,settings.output_fs/2]
+        
+        for ch in selected_channels:
+            y[:,ch] = amplitude*signal.chirp(t,f[0],T,f[1])
+    else:
+        print('signal type must be one of {''gaussian'',''uniform'',''sweep''}')
+        y = np.zeros((N_per_channel,settings.output_channels))
+    
+    y = win * y
+    
+    # final correction to ensure all signals limited to 0-1
+    if np.max(np.abs(y)) > limit:
+        y = limit * y / np.max(np.abs(y))
+        MESSAGE = 'Actual rms output after scaling to avoid clipping is {0:1.3f}'.format(np.sqrt(np.mean(y**2)))
+        
+    return t,y
+
+
+def stream_snapshot(rec):
+    
+    time_data_copy = np.copy(streams.REC.osc_time_data)
+    time_axis_copy = np.copy(streams.REC.osc_time_axis)
+    
+    t = datetime.datetime.now()
+    timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)    
+
+    time_data = datastructure.TimeData(time_axis_copy,time_data_copy,streams.REC.settings,timestamp=t,timestring=timestring,test_name='stream_snapshot')
+    
+    
     return time_data
```

### Comparing `pydvma-0.9.0/pydvma/analysis.py` & `pydvma-0.9.1/pydvma/analysis.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,455 +1,455 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Sun Sep  2 20:16:26 2018
-
-@author: tb267
-"""
-
-from . import datastructure
-
-import numpy as np
-from scipy import signal
-import copy
-
-MESSAGE = ''
-
-
-def calculate_fft(time_data,time_range=None,window=None):
-    '''
-    Args:
-        time_data (<TimeData> object): time series data
-        time_range: 2x1 numpy array to specify data segment to use
-        window (bool): apply blackman filter to data before fft or not
-    '''
-    
-    if time_data.__class__.__name__ != 'TimeData':
-        raise Exception('Input data needs to be single <TimeData> object')
-    
-
-    if time_range == None:
-        ### use all data
-        time_range_copy = time_data.time_axis[[0,-1]]
-        
-    elif time_range.__class__.__name__ == 'PlotData':
-        time_range_copy=time_range.ax.get_xbound()
-        
-    settings = copy.copy(time_data.settings)
-    settings.window = window
-    settings.time_range = time_range_copy
-
-    s1 = time_data.time_axis >= time_range_copy[0]
-    s2 = time_data.time_axis <= time_range_copy[1]
-    selection = s1 & s2
-    data_selected = time_data.time_data[selection,:]
-    N = len(data_selected[:,0])
-    
-    if window is None:
-        w = signal.windows.get_window('boxcar',N)
-    else:
-        w = signal.windows.get_window(window,N)
-        
-    # Broadcast the window across potentially multiple channels
-    data_selected = w[:, None] * data_selected
-        
-    fdata = np.fft.rfft(data_selected,axis=0)
-    faxis = np.fft.rfftfreq(N,1/time_data.settings.fs)
-    
-    freq_data = datastructure.FreqData(faxis,fdata,settings,id_link=time_data.unique_id,test_name=time_data.test_name)
-    
-    return freq_data
-
-def multiply_by_power_of_iw(data,power,channel_list):
-    
-    if data.__class__.__name__ == 'TfData':
-        iw = 1j*2*np.pi * data.freq_axis[:,None]
-        if power<0:
-            iw[0]=np.inf
-        data.tf_data[:,channel_list] = (iw**power) * data.tf_data[:,channel_list]
-        # keep track of multiplication powers
-        if hasattr(data,'iw_power_counter'):
-            data.iw_power_counter[channel_list] += power
-        else:
-            data.iw_power_counter = np.zeros(len(data.tf_data[0,:]))
-            data.iw_power_counter[channel_list] = power
-            
-    elif data.__class__.__name__ == 'FreqData':
-        iw = 1j*2*np.pi * data.freq_axis[:,None]
-        if power<0:
-            iw[0]=np.inf
-        data.freq_data[:,channel_list] = (iw**power) * data.freq_data[:,channel_list]
-        if hasattr(data,'iw_power_counter'):
-            data.iw_power_counter[channel_list] += power
-        else:
-            data.iw_power_counter = np.zeros(len(data.freq_data[0,:]))
-            data.iw_power_counter[channel_list] = power
-    else:
-        print('Expecting input argument of type <FreqData> or <TfData>')
-
-            
-    return data
-
-
-
-
-def best_match(tf_data_list,freq_range=None,set_ref=0,ch_ref=0):
-    '''
-    Args:
-        tf_data (<TfData> object): transfer function data
-        freq_range: 2x1 numpy array to specify data segment to use
-    '''
-    
-    if tf_data_list.__class__.__name__ != 'TfDataList':
-        raise ValueError('Input data needs to be single <TfData> object')
-    
-
-    if freq_range == None:
-        ### use all data
-        freq_range_copy = tf_data_list[set_ref].freq_axis[[0,-1]]
-        
-    elif freq_range.__class__.__name__ == 'PlotData':
-        freq_range_copy=freq_range.tfax.get_xbound()
-        
-    else:
-        freq_range_copy = freq_range
-        
-    
-    settings = copy.copy(tf_data_list[0].settings)
-    settings.freq_range = freq_range_copy
-
-    
-    n_set = len(tf_data_list)
-    
-    s1 = tf_data_list[set_ref].freq_axis >= freq_range_copy[0]
-    s2 = tf_data_list[set_ref].freq_axis <= freq_range_copy[1]
-    selection_ref = s1 & s2
-    # choose 0-1 scale to make dimensions of data compatible
-    f_ref = tf_data_list[set_ref].freq_axis[selection_ref]
-        
-    factors = []
-    for ns in range(n_set):
-        f=[]
-        n_chan = len(tf_data_list[ns].tf_data[0,:])
-        s1 = tf_data_list[ns].freq_axis >= freq_range_copy[0]
-        s2 = tf_data_list[ns].freq_axis <= freq_range_copy[1]
-        selection = s1 & s2
-        f_sel = tf_data_list[ns].freq_axis[selection]
-        N_ref = len(f_ref)
-        N_sel = len(f_sel)
-        f_newref = np.linspace(freq_range[0],freq_range[1],np.max([N_ref,N_sel]))
-        
-        for nc in range(n_chan):
-            # could make more efficient by doing all channels at once
-            x = tf_data_list[ns].freq_axis
-            y = tf_data_list[ns].tf_data[:,nc]
-            a = np.interp(f_newref,x,y)
-            a2d = a.reshape(np.size(a),1)
-            
-            x = tf_data_list[set_ref].freq_axis
-            y = tf_data_list[set_ref].tf_data[:,ch_ref]
-            b = np.interp(f_newref,x,y)
-            b2d = b.reshape(np.size(b),1)
-            
-            # use least squares only to get sign of factor
-            # get scale factor just by matching rms values
-            LS = np.linalg.lstsq(a2d.real, b2d.real, rcond=None)
-            sign = np.sign(LS[0][0])
-            f += [sign*np.sqrt(np.mean(np.abs(b)**2)) / np.sqrt(np.mean(np.abs(a)**2))]
-            
-            
-        f = np.array(f)
-        factors.append(f)
-    
-    return factors
-
-
-
-def calculate_cross_spectrum_matrix(time_data, time_range=None, window=None, N_frames=1, overlap=0.5):
-    '''
-    Args:
-        time_data (<TimeData> object): time series data
-        time_range: 2x1 numpy array to specify data segment to use
-        window (None or str): apply filter to data before fft or not
-        N_frames (int): number of frames to average over
-        overlap (between 0,1): frame overlap fraction
-    '''
-    # TODO iterate over list of timedata... but need new dataset type?
-    
-    if window==None:
-        window='boxcar'
-        
-    if time_data.__class__.__name__ != 'TimeData':
-        raise Exception('Input data needs to be single <TimeData> object')
-
-    if time_range == None:
-        ### use all data
-        time_range = time_data.time_axis[[0,-1]]
-        
-    elif time_range.__class__.__name__ == 'PlotData':
-        time_range=time_range.ax.get_xbound()
-        
-    settings = copy.copy(time_data.settings)
-    settings.window = window
-    settings.time_range = time_range
-    settings.N_frames = N_frames
-    settings.overlap = overlap
-
-    ## Select data range to use
-    s1 = time_data.time_axis >= time_range[0]
-    s2 = time_data.time_axis <= time_range[1]
-    selection = s1 & s2
-    data_selected = time_data.time_data[selection,:]
-    #time_selected = timedata.time_axis[selection]
-    
-    N_samples = len(data_selected[:,0])
-    nperseg = int(np.ceil(N_samples / (N_frames+1) / (1-overlap)))
-    freqlength = len(np.fft.rfftfreq(nperseg))
-    
-
-    noverlap = np.ceil(overlap*nperseg)
-    
-    N_chans = len(time_data.time_data[0,:])
-    Pxy = np.zeros([N_chans,N_chans,freqlength],dtype=complex)
-    Cxy = np.zeros([N_chans,N_chans,freqlength])
-    for nx in np.arange(N_chans):
-        for ny in np.arange(N_chans):
-            if nx > ny:
-                Pxy[nx,ny,:] = np.conjugate(Pxy[ny,nx,:])
-                Cxy[nx,ny,:] = Cxy[ny,nx,:]
-            else:
-                x = data_selected[:,nx]
-                y = data_selected[:,ny]
-                f,P = signal.csd(x,y,settings.fs,window=window, nperseg=nperseg, noverlap=noverlap,scaling='spectrum')
-                f,C = signal.coherence(x,y,settings.fs,window=window, nperseg=nperseg, noverlap=noverlap)
-                Pxy[nx,ny,:] = P
-                Cxy[nx,ny,:] = C
-            
-    cross_spec_data = datastructure.CrossSpecData(f,Pxy,Cxy,settings,id_link=time_data.unique_id,test_name=time_data.test_name)
-    
-    return cross_spec_data
-
-
-def calculate_cross_spectra_averaged(time_data_list, time_range=None, window=None):
-    '''
-    Calculates cross spectra averaged across ensemble of time_data_list. Note that 
-    this expects a <TimeDataList> of <TimeData> objects.
-    
-    Takes each time series as an independent measurement.
-    
-    Intended for averaged transfer functions from separate measurements, e.g. impulse hammer tests.
-    
-    Does not average data across sub-frames.    
-    
-    Args:
-        time_data_list (<TimeDataList> object): a list of time series data
-        time_range: 2x1 numpy array to specify data segment to use
-        window (None or str): type of window to use, default is None.
-    '''
-    
-    if time_data_list.__class__.__name__ != 'TimeDataList':
-        raise Exception('Input argument must be <TimeDataList> object.')
-
-    id_link_list = []
-    for td in time_data_list:
-        id_link_list += [td.unique_id]
-    
-    settings = copy.copy(time_data_list[0].settings)
-    settings.window = window
-    settings.time_range = time_range
-
-    
-    N_ensemble = len(time_data_list)
-    Pxy_av = 0
-    for td in time_data_list:
-        cross_spec_data = calculate_cross_spectrum_matrix(td, time_range=time_range, window=window, N_frames=1)
-        Pxy_av += cross_spec_data.Pxy / N_ensemble
-    
-    ch_all = np.arange(time_data_list[0].settings.channels)
-    Cxy = np.zeros([len(ch_all),len(ch_all),len(Pxy_av[0,0,:])])
-    for ch_in in ch_all:
-        for ch_out in ch_all:
-            Cxy[ch_in,ch_out,:] = np.abs(Pxy_av[ch_in,ch_out,:])**2 / (np.abs(Pxy_av[ch_in,ch_in,:]) * np.abs(Pxy_av[ch_out,ch_out,:]))
-    
-    
-    cross_spec_data_av = datastructure.CrossSpecData(cross_spec_data.freq_axis,Pxy_av,Cxy,settings,id_link=id_link_list,test_name=time_data_list[0].test_name)
-
-    return cross_spec_data_av
-
-
-def calculate_tf(time_data, ch_in=0, time_range=None, window=None, N_frames=1, overlap=0.5):
-    '''
-    Args:
-        time_data (<TimeData> object): time series data
-        ch_in (int): index of input channel
-        time_range: 2x1 numpy array to specify data segment to use
-        window (None or str): apply filter to data before fft or not
-        N_frames (int): number of frames to average over
-        overlap (between 0,1): frame overlap fraction
-    '''
-    if time_data.__class__.__name__ != 'TimeData':
-        raise Exception('Input data needs to be single <TimeData> object')
-
-
-    settings = copy.copy(time_data.settings)
-    settings.window = window
-    settings.time_range = time_range
-    
-    ## compute cross spectra
-    cross_spec_data = calculate_cross_spectrum_matrix(time_data, time_range=time_range, window=window, N_frames=N_frames, overlap=overlap)
-    f = cross_spec_data.freq_axis
-    Pxy = cross_spec_data.Pxy
-    Cxy = cross_spec_data.Cxy
-    ## identify transfer functions and corresponding coherence
-    
-    ch_all = np.arange(len(time_data.time_data[0,:]))
-    ch_out_set = np.setxor1d(ch_all,ch_in)
-    
-    tf_data = np.zeros([len(f),len(ch_out_set)],dtype=complex)
-    tf_coherence = np.zeros([len(f),len(ch_out_set)])
-    ch_count = -1
-    for ch_out in ch_out_set:
-        ch_count += 1
-        tf_data[:,ch_count] = Pxy[ch_in,ch_out,:] / Pxy[ch_in,ch_in,:]
-        tf_coherence[:,ch_count] = Cxy[ch_out,ch_in,:]
-        
-    settings.ch_in = ch_in
-    settings.ch_out_set = ch_out_set
-    
-    tfdata = datastructure.TfData(f,tf_data,tf_coherence,settings,id_link=time_data.unique_id,test_name=time_data.test_name)
-    
-    return tfdata
-    
-
-def calculate_tf_averaged(time_data_list, ch_in=0, time_range=None, window=None):
-    '''
-    Calculates transfer function averaged across ensemble of timedata. Note that 
-    this expects a Python list of timedata objects.
-    
-    Takes each time series as an independent measurement.
-    
-    Intended for averaged transfer functions from separate measurements, e.g. impulse hammer tests.
-    
-    Does not average data across sub-frames.    
-    
-    Args:
-        time_data_list (<TimeDataList> object): a list of time series data
-        ch_in (int): index of input channel
-        time_range: 2x1 numpy array to specify data segment to use
-        window (None or str): type of window to use, default is None.
-    '''
-    
-    if time_data_list.__class__.__name__ != 'TimeDataList':
-        raise Exception('Input argument must be <TimeDataList> object.')
-
-
-    id_link_list = []
-    for td in time_data_list:
-        id_link_list += [td.unique_id]
-        
-    N_ensemble = len(time_data_list)
-    Pxy_av = 0
-    count = -1
-    for td in time_data_list:
-        count += 1
-        ch_all = np.arange(len(td.time_data[0,:]))
-        ch_out_set = np.setxor1d(ch_all,ch_in)
-        cross_spec_data = calculate_cross_spectrum_matrix(td, time_range=time_range, window=window, N_frames=1)
-        f = cross_spec_data.freq_axis
-        Pxy = cross_spec_data.Pxy
-        Pxy_av += Pxy / N_ensemble
-    
-    tf_data = np.zeros([len(f),len(ch_out_set)],dtype=complex)
-    tf_coherence = np.zeros([len(f),len(ch_out_set)])    
-    ch_count = -1
-    for ch_out in ch_out_set:
-        ch_count += 1
-        tf_data[:,ch_count] = Pxy_av[ch_out,ch_in,:] / Pxy_av[ch_in,ch_in,:]
-        tf_coherence[:,ch_count] = np.abs(Pxy_av[ch_in,ch_out,:])**2 / (np.abs(Pxy_av[ch_in,ch_in,:]) * np.abs(Pxy_av[ch_out,ch_out,:]))
-
-    settings = copy.copy(td.settings)
-    settings.window = window
-    settings.time_range = time_range
-    settings.ch_in = ch_in
-    settings.ch_out_set = ch_out_set
-    
-    
-    tfdata = datastructure.TfData(f,tf_data,tf_coherence,settings,id_link=id_link_list,test_name=time_data_list[0].test_name)
-    
-    return tfdata
-
-
-#%% CLEAN IMPULSE
-def clean_impulse(time_data, ch_impulse=0):
-    '''
-    Sets all data outside of impulse to zero.
-    
-    Pulse width is estimated by assuming half cosine impulse, using width of half peak amplitude.
-    
-    Data before peak is unchanged. Data after estimated end of impulse is ramped to zero using half cosine pulse of width 10x estimated pulse width.
-    '''
-    global MESSAGE
-    if not hasattr(time_data,'impulse_cleaned'):
-        time_data.impulse_cleaned = False
-    
-    if time_data.impulse_cleaned == False:    
-        y = copy.deepcopy(time_data.time_data[:,ch_impulse])
-        yi_max = np.argmax(np.abs(y))
-        y_max = np.max(np.abs(y))
-        yi_out = np.where(np.abs(y)<y_max/2)[0]
-        yi_out1 = yi_out[yi_out < yi_max]
-        yi_out2 = yi_out[yi_out > yi_max]
-        y1 = yi_out1[-1]
-        y2 = yi_out2[0]
-        
-        
-        N = y2-y1
-        b = int(3*N/2) #half cosine estimate
-        end = int(yi_max + b/2)
-        b = 10*b # less agressive roll off
-        #print(time_data.settings.fs/b)
-    
-        ramp = np.hanning(2*b+1)    
-        win = np.ones(len(y))
-        win[end:end+b+1] = ramp[b:2*b+1]
-        win[end+b:] = 0
-        
-        y2 = win * y
-        
-        td = copy.deepcopy(time_data)
-        td.time_data[:,ch_impulse] = y2
-        td.impulse_cleaned = True
-        
-        yd = y2-y
-        if np.max(np.abs(yd)) > 0.1*np.max(np.abs(y)):
-            MESSAGE = 'Cleaned impulse data contained significant signal content.\n'
-            MESSAGE += 'Check for possible multiple impacts, or correct channel using ch_impulse.'
-        else:
-            MESSAGE = 'Impulse data cleaned.'
-        print(MESSAGE)
-        
-        return td
-    
-    else:
-        MESSAGE ='Impulse data already cleaned. No change made.'
-        print(MESSAGE)
-        return time_data
-
-    
-    
-#%% SONOGRAM    
-def calculate_sonogram(time_data, nperseg=None):
-    
-    y = np.copy(time_data.time_data) # handles all channels simultaneously
-    if nperseg == None:
-        nperseg = int(len(time_data.time_axis)/50) #roughly 50 fft's per time-series not counting overlap
-    f,t,S = signal.spectrogram(y,fs=time_data.settings.fs,window='hann',nperseg=nperseg,noverlap=nperseg//4,axis=0,mode='complex')
-    
-    # put channel axis at end
-    S_all_chans = np.swapaxes(S,1,2)
-    
-    sono_data = datastructure.SonoData(t,f,S_all_chans,time_data.settings,id_link=time_data.id_link,test_name=time_data.test_name)
-    
-    return sono_data
-
-#%% CWT
-#def calculate_cwt(time_data):
+# -*- coding: utf-8 -*-
+"""
+Created on Sun Sep  2 20:16:26 2018
+
+@author: tb267
+"""
+
+from . import datastructure
+
+import numpy as np
+from scipy import signal
+import copy
+
+MESSAGE = ''
+
+
+def calculate_fft(time_data,time_range=None,window=None):
+    '''
+    Args:
+        time_data (<TimeData> object): time series data
+        time_range: 2x1 numpy array to specify data segment to use
+        window (bool): apply blackman filter to data before fft or not
+    '''
+    
+    if time_data.__class__.__name__ != 'TimeData':
+        raise Exception('Input data needs to be single <TimeData> object')
+    
+
+    if time_range == None:
+        ### use all data
+        time_range_copy = time_data.time_axis[[0,-1]]
+        
+    elif time_range.__class__.__name__ == 'PlotData':
+        time_range_copy=time_range.ax.get_xbound()
+        
+    settings = copy.copy(time_data.settings)
+    settings.window = window
+    settings.time_range = time_range_copy
+
+    s1 = time_data.time_axis >= time_range_copy[0]
+    s2 = time_data.time_axis <= time_range_copy[1]
+    selection = s1 & s2
+    data_selected = time_data.time_data[selection,:]
+    N = len(data_selected[:,0])
+    
+    if window is None:
+        w = signal.windows.get_window('boxcar',N)
+    else:
+        w = signal.windows.get_window(window,N)
+        
+    # Broadcast the window across potentially multiple channels
+    data_selected = w[:, None] * data_selected
+        
+    fdata = np.fft.rfft(data_selected,axis=0)
+    faxis = np.fft.rfftfreq(N,1/time_data.settings.fs)
+    
+    freq_data = datastructure.FreqData(faxis,fdata,settings,id_link=time_data.unique_id,test_name=time_data.test_name)
+    
+    return freq_data
+
+def multiply_by_power_of_iw(data,power,channel_list):
+    
+    if data.__class__.__name__ == 'TfData':
+        iw = 1j*2*np.pi * data.freq_axis[:,None]
+        if power<0:
+            iw[0]=np.inf
+        data.tf_data[:,channel_list] = (iw**power) * data.tf_data[:,channel_list]
+        # keep track of multiplication powers
+        if hasattr(data,'iw_power_counter'):
+            data.iw_power_counter[channel_list] += power
+        else:
+            data.iw_power_counter = np.zeros(len(data.tf_data[0,:]))
+            data.iw_power_counter[channel_list] = power
+            
+    elif data.__class__.__name__ == 'FreqData':
+        iw = 1j*2*np.pi * data.freq_axis[:,None]
+        if power<0:
+            iw[0]=np.inf
+        data.freq_data[:,channel_list] = (iw**power) * data.freq_data[:,channel_list]
+        if hasattr(data,'iw_power_counter'):
+            data.iw_power_counter[channel_list] += power
+        else:
+            data.iw_power_counter = np.zeros(len(data.freq_data[0,:]))
+            data.iw_power_counter[channel_list] = power
+    else:
+        print('Expecting input argument of type <FreqData> or <TfData>')
+
+            
+    return data
+
+
+
+
+def best_match(tf_data_list,freq_range=None,set_ref=0,ch_ref=0):
+    '''
+    Args:
+        tf_data (<TfData> object): transfer function data
+        freq_range: 2x1 numpy array to specify data segment to use
+    '''
+    
+    if tf_data_list.__class__.__name__ != 'TfDataList':
+        raise ValueError('Input data needs to be single <TfData> object')
+    
+
+    if freq_range == None:
+        ### use all data
+        freq_range_copy = tf_data_list[set_ref].freq_axis[[0,-1]]
+        
+    elif freq_range.__class__.__name__ == 'PlotData':
+        freq_range_copy=freq_range.tfax.get_xbound()
+        
+    else:
+        freq_range_copy = freq_range
+        
+    
+    settings = copy.copy(tf_data_list[0].settings)
+    settings.freq_range = freq_range_copy
+
+    
+    n_set = len(tf_data_list)
+    
+    s1 = tf_data_list[set_ref].freq_axis >= freq_range_copy[0]
+    s2 = tf_data_list[set_ref].freq_axis <= freq_range_copy[1]
+    selection_ref = s1 & s2
+    # choose 0-1 scale to make dimensions of data compatible
+    f_ref = tf_data_list[set_ref].freq_axis[selection_ref]
+        
+    factors = []
+    for ns in range(n_set):
+        f=[]
+        n_chan = len(tf_data_list[ns].tf_data[0,:])
+        s1 = tf_data_list[ns].freq_axis >= freq_range_copy[0]
+        s2 = tf_data_list[ns].freq_axis <= freq_range_copy[1]
+        selection = s1 & s2
+        f_sel = tf_data_list[ns].freq_axis[selection]
+        N_ref = len(f_ref)
+        N_sel = len(f_sel)
+        f_newref = np.linspace(freq_range[0],freq_range[1],np.max([N_ref,N_sel]))
+        
+        for nc in range(n_chan):
+            # could make more efficient by doing all channels at once
+            x = tf_data_list[ns].freq_axis
+            y = tf_data_list[ns].tf_data[:,nc]
+            a = np.interp(f_newref,x,y)
+            a2d = a.reshape(np.size(a),1)
+            
+            x = tf_data_list[set_ref].freq_axis
+            y = tf_data_list[set_ref].tf_data[:,ch_ref]
+            b = np.interp(f_newref,x,y)
+            b2d = b.reshape(np.size(b),1)
+            
+            # use least squares only to get sign of factor
+            # get scale factor just by matching rms values
+            LS = np.linalg.lstsq(a2d.real, b2d.real, rcond=None)
+            sign = np.sign(LS[0][0])
+            f += [sign*np.sqrt(np.mean(np.abs(b)**2)) / np.sqrt(np.mean(np.abs(a)**2))]
+            
+            
+        f = np.array(f)
+        factors.append(f)
+    
+    return factors
+
+
+
+def calculate_cross_spectrum_matrix(time_data, time_range=None, window=None, N_frames=1, overlap=0.5):
+    '''
+    Args:
+        time_data (<TimeData> object): time series data
+        time_range: 2x1 numpy array to specify data segment to use
+        window (None or str): apply filter to data before fft or not
+        N_frames (int): number of frames to average over
+        overlap (between 0,1): frame overlap fraction
+    '''
+    # TODO iterate over list of timedata... but need new dataset type?
+    
+    if window==None:
+        window='boxcar'
+        
+    if time_data.__class__.__name__ != 'TimeData':
+        raise Exception('Input data needs to be single <TimeData> object')
+
+    if time_range == None:
+        ### use all data
+        time_range = time_data.time_axis[[0,-1]]
+        
+    elif time_range.__class__.__name__ == 'PlotData':
+        time_range=time_range.ax.get_xbound()
+        
+    settings = copy.copy(time_data.settings)
+    settings.window = window
+    settings.time_range = time_range
+    settings.N_frames = N_frames
+    settings.overlap = overlap
+
+    ## Select data range to use
+    s1 = time_data.time_axis >= time_range[0]
+    s2 = time_data.time_axis <= time_range[1]
+    selection = s1 & s2
+    data_selected = time_data.time_data[selection,:]
+    #time_selected = timedata.time_axis[selection]
+    
+    N_samples = len(data_selected[:,0])
+    nperseg = int(np.ceil(N_samples / (N_frames+1) / (1-overlap)))
+    freqlength = len(np.fft.rfftfreq(nperseg))
+    
+
+    noverlap = np.ceil(overlap*nperseg)
+    
+    N_chans = len(time_data.time_data[0,:])
+    Pxy = np.zeros([N_chans,N_chans,freqlength],dtype=complex)
+    Cxy = np.zeros([N_chans,N_chans,freqlength])
+    for nx in np.arange(N_chans):
+        for ny in np.arange(N_chans):
+            if nx > ny:
+                Pxy[nx,ny,:] = np.conjugate(Pxy[ny,nx,:])
+                Cxy[nx,ny,:] = Cxy[ny,nx,:]
+            else:
+                x = data_selected[:,nx]
+                y = data_selected[:,ny]
+                f,P = signal.csd(x,y,settings.fs,window=window, nperseg=nperseg, noverlap=noverlap,scaling='spectrum')
+                f,C = signal.coherence(x,y,settings.fs,window=window, nperseg=nperseg, noverlap=noverlap)
+                Pxy[nx,ny,:] = P
+                Cxy[nx,ny,:] = C
+            
+    cross_spec_data = datastructure.CrossSpecData(f,Pxy,Cxy,settings,id_link=time_data.unique_id,test_name=time_data.test_name)
+    
+    return cross_spec_data
+
+
+def calculate_cross_spectra_averaged(time_data_list, time_range=None, window=None):
+    '''
+    Calculates cross spectra averaged across ensemble of time_data_list. Note that 
+    this expects a <TimeDataList> of <TimeData> objects.
+    
+    Takes each time series as an independent measurement.
+    
+    Intended for averaged transfer functions from separate measurements, e.g. impulse hammer tests.
+    
+    Does not average data across sub-frames.    
+    
+    Args:
+        time_data_list (<TimeDataList> object): a list of time series data
+        time_range: 2x1 numpy array to specify data segment to use
+        window (None or str): type of window to use, default is None.
+    '''
+    
+    if time_data_list.__class__.__name__ != 'TimeDataList':
+        raise Exception('Input argument must be <TimeDataList> object.')
+
+    id_link_list = []
+    for td in time_data_list:
+        id_link_list += [td.unique_id]
+    
+    settings = copy.copy(time_data_list[0].settings)
+    settings.window = window
+    settings.time_range = time_range
+
+    
+    N_ensemble = len(time_data_list)
+    Pxy_av = 0
+    for td in time_data_list:
+        cross_spec_data = calculate_cross_spectrum_matrix(td, time_range=time_range, window=window, N_frames=1)
+        Pxy_av += cross_spec_data.Pxy / N_ensemble
+    
+    ch_all = np.arange(time_data_list[0].settings.channels)
+    Cxy = np.zeros([len(ch_all),len(ch_all),len(Pxy_av[0,0,:])])
+    for ch_in in ch_all:
+        for ch_out in ch_all:
+            Cxy[ch_in,ch_out,:] = np.abs(Pxy_av[ch_in,ch_out,:])**2 / (np.abs(Pxy_av[ch_in,ch_in,:]) * np.abs(Pxy_av[ch_out,ch_out,:]))
+    
+    
+    cross_spec_data_av = datastructure.CrossSpecData(cross_spec_data.freq_axis,Pxy_av,Cxy,settings,id_link=id_link_list,test_name=time_data_list[0].test_name)
+
+    return cross_spec_data_av
+
+
+def calculate_tf(time_data, ch_in=0, time_range=None, window=None, N_frames=1, overlap=0.5):
+    '''
+    Args:
+        time_data (<TimeData> object): time series data
+        ch_in (int): index of input channel
+        time_range: 2x1 numpy array to specify data segment to use
+        window (None or str): apply filter to data before fft or not
+        N_frames (int): number of frames to average over
+        overlap (between 0,1): frame overlap fraction
+    '''
+    if time_data.__class__.__name__ != 'TimeData':
+        raise Exception('Input data needs to be single <TimeData> object')
+
+
+    settings = copy.copy(time_data.settings)
+    settings.window = window
+    settings.time_range = time_range
+    
+    ## compute cross spectra
+    cross_spec_data = calculate_cross_spectrum_matrix(time_data, time_range=time_range, window=window, N_frames=N_frames, overlap=overlap)
+    f = cross_spec_data.freq_axis
+    Pxy = cross_spec_data.Pxy
+    Cxy = cross_spec_data.Cxy
+    ## identify transfer functions and corresponding coherence
+    
+    ch_all = np.arange(len(time_data.time_data[0,:]))
+    ch_out_set = np.setxor1d(ch_all,ch_in)
+    
+    tf_data = np.zeros([len(f),len(ch_out_set)],dtype=complex)
+    tf_coherence = np.zeros([len(f),len(ch_out_set)])
+    ch_count = -1
+    for ch_out in ch_out_set:
+        ch_count += 1
+        tf_data[:,ch_count] = Pxy[ch_in,ch_out,:] / Pxy[ch_in,ch_in,:]
+        tf_coherence[:,ch_count] = Cxy[ch_out,ch_in,:]
+        
+    settings.ch_in = ch_in
+    settings.ch_out_set = ch_out_set
+    
+    tfdata = datastructure.TfData(f,tf_data,tf_coherence,settings,id_link=time_data.unique_id,test_name=time_data.test_name)
+    
+    return tfdata
+    
+
+def calculate_tf_averaged(time_data_list, ch_in=0, time_range=None, window=None):
+    '''
+    Calculates transfer function averaged across ensemble of timedata. Note that 
+    this expects a Python list of timedata objects.
+    
+    Takes each time series as an independent measurement.
+    
+    Intended for averaged transfer functions from separate measurements, e.g. impulse hammer tests.
+    
+    Does not average data across sub-frames.    
+    
+    Args:
+        time_data_list (<TimeDataList> object): a list of time series data
+        ch_in (int): index of input channel
+        time_range: 2x1 numpy array to specify data segment to use
+        window (None or str): type of window to use, default is None.
+    '''
+    
+    if time_data_list.__class__.__name__ != 'TimeDataList':
+        raise Exception('Input argument must be <TimeDataList> object.')
+
+
+    id_link_list = []
+    for td in time_data_list:
+        id_link_list += [td.unique_id]
+        
+    N_ensemble = len(time_data_list)
+    Pxy_av = 0
+    count = -1
+    for td in time_data_list:
+        count += 1
+        ch_all = np.arange(len(td.time_data[0,:]))
+        ch_out_set = np.setxor1d(ch_all,ch_in)
+        cross_spec_data = calculate_cross_spectrum_matrix(td, time_range=time_range, window=window, N_frames=1)
+        f = cross_spec_data.freq_axis
+        Pxy = cross_spec_data.Pxy
+        Pxy_av += Pxy / N_ensemble
+    
+    tf_data = np.zeros([len(f),len(ch_out_set)],dtype=complex)
+    tf_coherence = np.zeros([len(f),len(ch_out_set)])    
+    ch_count = -1
+    for ch_out in ch_out_set:
+        ch_count += 1
+        tf_data[:,ch_count] = Pxy_av[ch_out,ch_in,:] / Pxy_av[ch_in,ch_in,:]
+        tf_coherence[:,ch_count] = np.abs(Pxy_av[ch_in,ch_out,:])**2 / (np.abs(Pxy_av[ch_in,ch_in,:]) * np.abs(Pxy_av[ch_out,ch_out,:]))
+
+    settings = copy.copy(td.settings)
+    settings.window = window
+    settings.time_range = time_range
+    settings.ch_in = ch_in
+    settings.ch_out_set = ch_out_set
+    
+    
+    tfdata = datastructure.TfData(f,tf_data,tf_coherence,settings,id_link=id_link_list,test_name=time_data_list[0].test_name)
+    
+    return tfdata
+
+
+#%% CLEAN IMPULSE
+def clean_impulse(time_data, ch_impulse=0):
+    '''
+    Sets all data outside of impulse to zero.
+    
+    Pulse width is estimated by assuming half cosine impulse, using width of half peak amplitude.
+    
+    Data before peak is unchanged. Data after estimated end of impulse is ramped to zero using half cosine pulse of width 10x estimated pulse width.
+    '''
+    global MESSAGE
+    if not hasattr(time_data,'impulse_cleaned'):
+        time_data.impulse_cleaned = False
+    
+    if time_data.impulse_cleaned == False:    
+        y = copy.deepcopy(time_data.time_data[:,ch_impulse])
+        yi_max = np.argmax(np.abs(y))
+        y_max = np.max(np.abs(y))
+        yi_out = np.where(np.abs(y)<y_max/2)[0]
+        yi_out1 = yi_out[yi_out < yi_max]
+        yi_out2 = yi_out[yi_out > yi_max]
+        y1 = yi_out1[-1]
+        y2 = yi_out2[0]
+        
+        
+        N = y2-y1
+        b = int(3*N/2) #half cosine estimate
+        end = int(yi_max + b/2)
+        b = 10*b # less agressive roll off
+        #print(time_data.settings.fs/b)
+    
+        ramp = np.hanning(2*b+1)    
+        win = np.ones(len(y))
+        win[end:end+b+1] = ramp[b:2*b+1]
+        win[end+b:] = 0
+        
+        y2 = win * y
+        
+        td = copy.deepcopy(time_data)
+        td.time_data[:,ch_impulse] = y2
+        td.impulse_cleaned = True
+        
+        yd = y2-y
+        if np.max(np.abs(yd)) > 0.1*np.max(np.abs(y)):
+            MESSAGE = 'Cleaned impulse data contained significant signal content.\n'
+            MESSAGE += 'Check for possible multiple impacts, or correct channel using ch_impulse.'
+        else:
+            MESSAGE = 'Impulse data cleaned.'
+        print(MESSAGE)
+        
+        return td
+    
+    else:
+        MESSAGE ='Impulse data already cleaned. No change made.'
+        print(MESSAGE)
+        return time_data
+
+    
+    
+#%% SONOGRAM    
+def calculate_sonogram(time_data, nperseg=None):
+    
+    y = np.copy(time_data.time_data) # handles all channels simultaneously
+    if nperseg == None:
+        nperseg = int(len(time_data.time_axis)/50) #roughly 50 fft's per time-series not counting overlap
+    f,t,S = signal.spectrogram(y,fs=time_data.settings.fs,window='hann',nperseg=nperseg,noverlap=nperseg//4,axis=0,mode='complex')
+    
+    # put channel axis at end
+    S_all_chans = np.swapaxes(S,1,2)
+    
+    sono_data = datastructure.SonoData(t,f,S_all_chans,time_data.settings,id_link=time_data.id_link,test_name=time_data.test_name)
+    
+    return sono_data
+
+#%% CWT
+#def calculate_cwt(time_data):
 #    return None
```

### Comparing `pydvma-0.9.0/pydvma/file.py` & `pydvma-0.9.1/pydvma/file.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,498 +1,498 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Aug 27 14:32:35 2018
-
-@author: tb267
-"""
-
-import os.path
-import numpy as np
-import scipy.io as io
-import pyqtgraph as pg
-from qtpy import QtWidgets
-from qtpy.QtWidgets import QFileDialog
-
-
-
-def load_data(parent=None, filename=None):
-    '''
-    Loads dataset from filename, or displays a dialog if no argument provided.
-    '''
-    if filename is None:
-        # wid = QtWidgets.QWidget()
-        filename, _ = QFileDialog.getOpenFileName(parent, 'Open data file', '', '*.npy')
-        
-        # file_dialog = QFileDialog(parent, 'Open data file', '', '*.npy')
-        # file_dialog.setFileMode(QFileDialog.FileMode.ExistingFile)
-        # file_dialog.exec()
-        # filename = file_dialog.selectedFiles()
-
-        if not filename:
-            return None
-
-    d = np.load(filename,allow_pickle=True,fix_imports=True)
-    dataset = d[0]
-    return dataset
-
-
-def save_data(dataset, parent=None, filename=None, overwrite_without_prompt=False):
-    '''
-    Saves dataset class to file 'filename.npy', or provides dialog if no
-    filename provided.
-
-    Args:
-       dataset: An object of the class dataSet
-       filename: string [optional]
-       overwrite_without_prompt: bool
-
-    '''
-
-    # put data into numpy array
-    d = np.array([dataset])
-
-    # If filename not specified, provide dialog
-    if filename is None:
-        filename, _ = QFileDialog.getSaveFileName(parent, 'Save dataset', '', '*.npy')
-        if not filename:
-            # No filename chosen, give up on saving
-            print('Save cancelled')
-            return None
-
-
-    # If it exists, check if we should overwrite it (unless
-    # overwrite_without_prompt is True)
-    elif os.path.isfile(filename) and not overwrite_without_prompt:
-        answer = input('File %r already exists. Overwrite? [y/n]: ' % filename)
-        if answer != 'y':
-            print('Save cancelled')
-            return None
-        print('Will overwrite existing file')
-        
-    # Make sure it ends with .npy
-    if not filename.endswith('.npy'):
-        filename += '.npy'
-        
-    # Actually save!
-    np.save(filename, d)
-    print("Data saved as %s" % filename)
-
-    return filename
-
-
-
-def save_fig(plot, parent=None, figsize=None, filename=None, overwrite_without_prompt=False):
-    '''
-    Saves figure to file 'filename.png' and 'filename.pdf', or provides dialog if no
-    filename provided.
-
-    Args:
-       fig: A matplotlib fig object
-       filename: string [optional]
-       overwrite_without_prompt: boo
-    '''
-    if plot.__class__.__name__ == 'PlotData':
-        fig = plot.fig
-    elif plot.__class__.__name__ == 'Figure':
-        fig = plot
-
-    # If filename not specified, provide dialog
-    if filename is None:
-        filename, _ = QFileDialog.getSaveFileName(parent, 'Save figure', '')
-        if not filename:
-            # No filename chosen, give up on saving
-            print('Save cancelled')
-            return None
-
-
-    # If it exists, check if we should overwrite it (unless
-    # overwrite_without_prompt is True)
-    elif os.path.isfile(filename) and not overwrite_without_prompt:
-        answer = input('File %r already exists. Overwrite? [y/n]: ' % filename)
-        if answer != 'y':
-            print('Save cancelled')
-            return None
-        print('Will overwrite existing file')
-
-    # Set figsize...
-    original_size = fig.get_size_inches()
-    if figsize is not None:
-        fig.set_size_inches(figsize,forward=False)
-        
-    # Make sure it ends with .png then .pdf
-    filename = os.path.splitext(filename)[0]
-    if not filename.endswith('.png'):
-        filename += '.png'
-    fig.savefig(filename, dpi=300)
-    print("Figure saved as %s" % filename)
-    
-    filename = os.path.splitext(filename)[0]
-    if not filename.endswith('.pdf'):
-        filename += '.pdf'
-    fig.savefig(filename, dpi=300)
-    print("Figure saved as %s" % filename)
-
-    # return to original size
-    fig.set_size_inches(original_size,forward=False)
-    
-    
-    return filename
-
-
-
-#%% EXPORT TO MATLAB
-def export_to_matlab(dataset, parent=None, filename=None, overwrite_without_prompt=False):
-    '''
-    Exports dataset class to file 'filename.mat', or provides dialog if no
-    filename provided.
-    
-    Saved file can be loaded directly in Matlab as set of arrays.
-
-    Args:
-       dataset: An object of the class dataSet
-       filename: string [optional]
-       overwrite_without_prompt: bool
-
-    '''
-    
-    # convert data into dictionary ready for Matlab
-    data_matlab = dict()
-    
-    #%% TIME
-    if len(dataset.time_data_list) > 0:
-        T=0
-        fs=0
-        n_time=0
-        for time_data in dataset.time_data_list:
-            N = len(time_data.time_axis)
-            T = np.max([time_data.time_axis[-1]*N/(N-1),T])
-            fs = np.max([1/np.mean(np.diff(time_data.time_axis)),fs])
-            n_time += time_data.settings.channels
-        
-        t=np.arange(0,T,1/fs)
-        time_data_all = np.zeros((len(t),n_time))
-        counter = -1
-        for time_data in dataset.time_data_list:
-            for i in range(time_data.settings.channels):
-                counter += 1
-                time_data_all[:,counter] = np.interp(t,time_data.time_axis,time_data.time_data[:,i],right=0)
-                
-        data_matlab['time_axis_all'] = np.transpose(np.atleast_2d(t))
-        data_matlab['time_data_all'] = time_data_all
-
-    
-
-
-    #%% FFT - doesn't export coherence
-    if len(dataset.freq_data_list) > 0:
-        df=np.inf
-        fmax=0
-        n_tf=0
-        for freq_data in dataset.freq_data_list:
-            df_check = np.mean(np.diff(freq_data.freq_axis))
-            df = np.min([df,df_check])
-            fmax = np.max([freq_data.freq_axis[-1],fmax])
-            tf_shape = np.shape(freq_data.freq_data)
-            n_tf += tf_shape[1]
-        
-        f=np.arange(0,fmax+df,df)
-        npts = 2*(len(f)-1)
-        fs_tf = 2*f[-1]
-        freq_data_all = np.zeros((len(f),n_tf),dtype=complex)
-        counter = -1
-        for freq_data in dataset.freq_data_list:
-            freq_shape = np.shape(freq_data.freq_data)
-            for i in range(freq_shape[1]):
-                counter += 1
-                freq_data_all[:,counter] = np.interp(f,freq_data.freq_axis,freq_data.freq_data[:,i],right=0)
-        
-        data_matlab['freq_axis_all'] = np.transpose(np.atleast_2d(f))
-        data_matlab['freq_data_all'] = freq_data_all
-        
- 
-
-
-    #%% Transfer Function - doesn't export coherence
-    if len(dataset.tf_data_list) > 0:
-        df=np.inf
-        fmax=0
-        n_tf=0
-        for tf_data in dataset.tf_data_list:
-            df_check = np.mean(np.diff(tf_data.freq_axis))
-            df = np.min([df,df_check])
-            fmax = np.max([tf_data.freq_axis[-1],fmax])
-            tf_shape = np.shape(tf_data.tf_data)
-            n_tf += tf_shape[1]
-        
-        f=np.arange(0,fmax+df,df)
-        npts = 2*(len(f)-1)
-        fs_tf = 2*f[-1]
-        tf_data_all = np.zeros((len(f),n_tf),dtype=complex)
-        counter = -1
-        for tf_data in dataset.tf_data_list:
-            tf_shape = np.shape(tf_data.tf_data)
-            for i in range(tf_shape[1]):
-                counter += 1
-                tf_data_all[:,counter] = np.interp(f,tf_data.freq_axis,tf_data.tf_data[:,i],right=0)
-        
-        data_matlab['tf_axis_all'] = np.transpose(np.atleast_2d(f))
-        data_matlab['tf_data_all'] = tf_data_all
-        
-
-    
-
-
-    #%% SAVE
-
-    # If filename not specified, provide dialog
-    if filename is None:
-        filename, _ = QFileDialog.getSaveFileName(parent, 'Save dataset', '', '*.mat')
-        if not filename:
-            # No filename chosen, give up on saving
-            print('Save cancelled')
-            return None
-
-
-    # If it exists, check if we should overwrite it (unless
-    # overwrite_without_prompt is True)
-    elif os.path.isfile(filename) and not overwrite_without_prompt:
-        answer = input('File %r already exists. Overwrite? [y/n]: ' % filename)
-        if answer != 'y':
-            print('Save cancelled')
-            return None
-        print('Will overwrite existing file')
-        
-    # Make sure it ends with .npy
-    if not filename.endswith('.mat'):
-        filename += '.mat'
-        
-    # Actually save!
-    io.savemat(filename,data_matlab)
-    print("Data saved as %s" % filename)
-
-    return filename
-
-
-
-#%% EXPORT TO MATLAB JWLOGGER
-def export_to_matlab_jwlogger(dataset, parent=None, filename=None, overwrite_without_prompt=False):
-    '''
-    Exports dataset class to file 'filename.mat', or provides dialog if no
-    filename provided.
-    
-    Saved file is compatible with Jim Woodhouse logger file format.
-
-    Args:
-       dataset: An object of the class dataSet
-       filename: string [optional]
-       overwrite_without_prompt: bool
-
-    '''
-
-    # convert data into dictionary ready for Matlab
-    data_jwlogger = dict()
-    
-    #%% TIME
-    if len(dataset.time_data_list) > 0:
-        T=0
-        fs=0
-        n_time=0
-        for time_data in dataset.time_data_list:
-            N = len(time_data.time_axis)
-            T = np.max([time_data.time_axis[-1]*N/(N-1),T])
-            fs = np.max([1/np.mean(np.diff(time_data.time_axis)),fs])
-            n_time += time_data.settings.channels
-        
-        t=np.arange(0,T,1/fs)
-        time_data_all = np.zeros((len(t),n_time))
-        counter = -1
-        for time_data in dataset.time_data_list:
-            for i in range(time_data.settings.channels):
-                counter += 1
-                time_data_all[:,counter] = np.interp(t,time_data.time_axis,time_data.time_data[:,i],right=0)
-                
-        data_jwlogger['buflen'] = float(np.size(t))
-        data_jwlogger['indata'] = time_data_all
-        data_jwlogger['tsmax'] = float(t[-1])
-    else:
-        n_time = 0
-        time_data_all = 0
-    
-    
-    #%% FFT: get's overwritten by TF if exists
-    if len(dataset.freq_data_list) > 0:
-        df=np.inf
-        fmax=0
-        n_freq=0
-        for freq_data in dataset.freq_data_list:
-            df_check = np.mean(np.diff(freq_data.freq_axis))
-            df = np.min([df,df_check])
-            fmax = np.max([freq_data.freq_axis[-1],fmax])
-            freq_shape = np.shape(freq_data.freq_data)
-            n_freq += freq_shape[1]
-        
-        f=np.arange(0,fmax+df,df)
-        npts = 2*(len(f)-1)
-        fs_freq = 2*f[-1]
-        freq_data_all = np.zeros((len(f),n_freq),dtype=complex)
-        counter = -1
-        for freq_data in dataset.freq_data_list:
-            freq_shape = np.shape(freq_data.freq_data)
-            for i in range(freq_shape[1]):
-                counter += 1
-                freq_data_all[:,counter] = np.interp(f,freq_data.freq_axis,freq_data.freq_data[:,i],right=1)
-                freq_data_all[0,counter] = freq_data_all[1,counter] # to match equivalent tweak in JW Logger for handling DC singularities
-                zero_test = freq_data_all[:,counter] == 0
-                freq_data_all[zero_test,counter] = np.min(np.abs(freq_data_all[:,counter])) # handle zeros
-        
-        # convert
-        data_jwlogger['freq'] = float(fs_freq)
-        data_jwlogger['npts'] = float(npts)
-        data_jwlogger['yspec'] = freq_data_all
-    else:
-        n_freq = 0
-        freq_data_all = 0
-    
-    
-    #%% Transfer Function - doesn't export coherence
-    if len(dataset.tf_data_list) > 0:
-        df=np.inf
-        fmax=0
-        n_tf=0
-        for tf_data in dataset.tf_data_list:
-            df_check = np.mean(np.diff(tf_data.freq_axis))
-            df = np.min([df,df_check])
-            fmax = np.max([tf_data.freq_axis[-1],fmax])
-            tf_shape = np.shape(tf_data.tf_data)
-            n_tf += tf_shape[1]
-        
-        f=np.arange(0,fmax+df,df)
-        npts = 2*(len(f)-1)
-        fs_tf = 2*f[-1]
-        tf_data_all = np.zeros((len(f),n_tf),dtype=complex)
-        counter = -1
-        for tf_data in dataset.tf_data_list:
-            tf_shape = np.shape(tf_data.tf_data)
-            for i in range(tf_shape[1]):
-                counter += 1
-                tf_data_all[:,counter] = np.interp(f,tf_data.freq_axis,tf_data.tf_data[:,i],right=1)
-                tf_data_all[0,counter] = tf_data_all[1,counter] # to match equivalent tweak in JW Logger for handling DC singularities
-                zero_test = freq_data_all[:,counter] == 0
-                tf_data_all[zero_test,counter] = np.min(np.abs(tf_data_all[:,counter])) # handle zeros
-        
-        # convert
-        data_jwlogger['freq'] = float(fs_tf)
-        data_jwlogger['npts'] = float(npts)
-        data_jwlogger['yspec'] = tf_data_all
-    else:
-        n_tf = 0
-        tf_data_all = 0
-    
-    #%% Convert
-    
-    if (n_freq > 0) & (n_tf > 0):
-        # if both FFT and TF data present then TF overwrites
-        N = n_tf
-    else:
-        # if only one of FFT or TF, or neither, then keep non-zero one, or neither
-        N = np.max([n_tf,n_freq])
-    
-    data_jwlogger['dt2'] = np.array([n_time,N,0],dtype=float)
-    data_jwlogger['dtype'] = np.array([n_time,N,0],dtype=float)
-    
-
-    # SAVE
-
-    # If filename not specified, provide dialog
-    if filename is None:
-        filename, _ = QFileDialog.getSaveFileName(parent, 'Save dataset', '', '*.mat')
-        if not filename:
-            # No filename chosen, give up on saving
-            print('Save cancelled')
-            return None
-
-
-    # If it exists, check if we should overwrite it (unless
-    # overwrite_without_prompt is True)
-    elif os.path.isfile(filename) and not overwrite_without_prompt:
-        answer = input('File %r already exists. Overwrite? [y/n]: ' % filename)
-        if answer != 'y':
-            print('Save cancelled')
-            return None
-        print('Will overwrite existing file')
-        
-    # Make sure it ends with .npy
-    if not filename.endswith('.mat'):
-        filename += '.mat'
-        
-    # Actually save!
-    io.savemat(filename,data_jwlogger)
-    print("Data saved as %s" % filename)
-
-    return filename
-
-
-def export_to_csv(data_list, parent=None, filename=None, overwrite_without_prompt=False):
-    '''
-    Exports data to file 'filename.csv', or provides dialog if no
-    filename provided.
-    
-    Saved file is *.csv
-
-    Args:
-       data_list: An object of the class TimeDataList, FreqDataList, or TfDataList
-       filename: string [optional]
-       overwrite_without_prompt: bool
-    '''
-    
-    data_list_type = data_list.__class__.__name__
-    
-    if data_list_type == 'TimeDataList':
-        darray = np.transpose(np.atleast_2d(data_list[0].time_axis))
-        for time_data in data_list:
-            darray = np.append(darray,time_data.time_data,axis=1)
-        
-            
-            
-    elif data_list_type == 'FreqDataList':
-        darray = np.transpose(np.atleast_2d(data_list[0].freq_axis))
-        for freq_data in data_list:
-            darray = np.append(darray,freq_data.freq_data,axis=1)
-        
-    elif data_list_type == 'TfDataList':
-        darray = np.transpose(np.atleast_2d(data_list[0].freq_axis))
-        for tf_data in data_list:
-            darray = np.append(darray,tf_data.tf_data,axis=1)
-        
-    else:
-        print('Expecting input to be one of TimeDataList, FreqDataList, or TfDataList')
-        return None
-    
-    # SAVE
-
-    # If filename not specified, provide dialog
-    if filename is None:
-        filename, _ = QFileDialog.getSaveFileName(parent, 'Save dataset', '', '*.csv')
-        if not filename:
-            # No filename chosen, give up on saving
-            print('Save cancelled')
-            return None
-
-
-    # If it exists, check if we should overwrite it (unless
-    # overwrite_without_prompt is True)
-    elif os.path.isfile(filename) and not overwrite_without_prompt:
-        answer = input('File %r already exists. Overwrite? [y/n]: ' % filename)
-        if answer != 'y':
-            print('Save cancelled')
-            return None
-        print('Will overwrite existing file')
-        
-    # Make sure it ends with .csv
-    if not filename.endswith('.csv'):
-        filename += '.csv'
-        
-    # Actually save!
-    np.savetxt(filename, darray, delimiter=",")
-    print("Data saved as %s" % filename)
-
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Aug 27 14:32:35 2018
+
+@author: tb267
+"""
+
+import os.path
+import numpy as np
+import scipy.io as io
+import pyqtgraph as pg
+from qtpy import QtWidgets
+from qtpy.QtWidgets import QFileDialog
+
+
+
+def load_data(parent=None, filename=None):
+    '''
+    Loads dataset from filename, or displays a dialog if no argument provided.
+    '''
+    if filename is None:
+        # wid = QtWidgets.QWidget()
+        filename, _ = QFileDialog.getOpenFileName(parent, 'Open data file', '', '*.npy')
+        
+        # file_dialog = QFileDialog(parent, 'Open data file', '', '*.npy')
+        # file_dialog.setFileMode(QFileDialog.FileMode.ExistingFile)
+        # file_dialog.exec()
+        # filename = file_dialog.selectedFiles()
+
+        if not filename:
+            return None
+
+    d = np.load(filename,allow_pickle=True,fix_imports=True)
+    dataset = d[0]
+    return dataset
+
+
+def save_data(dataset, parent=None, filename=None, overwrite_without_prompt=False):
+    '''
+    Saves dataset class to file 'filename.npy', or provides dialog if no
+    filename provided.
+
+    Args:
+       dataset: An object of the class dataSet
+       filename: string [optional]
+       overwrite_without_prompt: bool
+
+    '''
+
+    # put data into numpy array
+    d = np.array([dataset])
+
+    # If filename not specified, provide dialog
+    if filename is None:
+        filename, _ = QFileDialog.getSaveFileName(parent, 'Save dataset', '', '*.npy')
+        if not filename:
+            # No filename chosen, give up on saving
+            print('Save cancelled')
+            return None
+
+
+    # If it exists, check if we should overwrite it (unless
+    # overwrite_without_prompt is True)
+    elif os.path.isfile(filename) and not overwrite_without_prompt:
+        answer = input('File %r already exists. Overwrite? [y/n]: ' % filename)
+        if answer != 'y':
+            print('Save cancelled')
+            return None
+        print('Will overwrite existing file')
+        
+    # Make sure it ends with .npy
+    if not filename.endswith('.npy'):
+        filename += '.npy'
+        
+    # Actually save!
+    np.save(filename, d)
+    print("Data saved as %s" % filename)
+
+    return filename
+
+
+
+def save_fig(plot, parent=None, figsize=None, filename=None, overwrite_without_prompt=False):
+    '''
+    Saves figure to file 'filename.png' and 'filename.pdf', or provides dialog if no
+    filename provided.
+
+    Args:
+       fig: A matplotlib fig object
+       filename: string [optional]
+       overwrite_without_prompt: boo
+    '''
+    if plot.__class__.__name__ == 'PlotData':
+        fig = plot.fig
+    elif plot.__class__.__name__ == 'Figure':
+        fig = plot
+
+    # If filename not specified, provide dialog
+    if filename is None:
+        filename, _ = QFileDialog.getSaveFileName(parent, 'Save figure', '')
+        if not filename:
+            # No filename chosen, give up on saving
+            print('Save cancelled')
+            return None
+
+
+    # If it exists, check if we should overwrite it (unless
+    # overwrite_without_prompt is True)
+    elif os.path.isfile(filename) and not overwrite_without_prompt:
+        answer = input('File %r already exists. Overwrite? [y/n]: ' % filename)
+        if answer != 'y':
+            print('Save cancelled')
+            return None
+        print('Will overwrite existing file')
+
+    # Set figsize...
+    original_size = fig.get_size_inches()
+    if figsize is not None:
+        fig.set_size_inches(figsize,forward=False)
+        
+    # Make sure it ends with .png then .pdf
+    filename = os.path.splitext(filename)[0]
+    if not filename.endswith('.png'):
+        filename += '.png'
+    fig.savefig(filename, dpi=300)
+    print("Figure saved as %s" % filename)
+    
+    filename = os.path.splitext(filename)[0]
+    if not filename.endswith('.pdf'):
+        filename += '.pdf'
+    fig.savefig(filename, dpi=300)
+    print("Figure saved as %s" % filename)
+
+    # return to original size
+    fig.set_size_inches(original_size,forward=False)
+    
+    
+    return filename
+
+
+
+#%% EXPORT TO MATLAB
+def export_to_matlab(dataset, parent=None, filename=None, overwrite_without_prompt=False):
+    '''
+    Exports dataset class to file 'filename.mat', or provides dialog if no
+    filename provided.
+    
+    Saved file can be loaded directly in Matlab as set of arrays.
+
+    Args:
+       dataset: An object of the class dataSet
+       filename: string [optional]
+       overwrite_without_prompt: bool
+
+    '''
+    
+    # convert data into dictionary ready for Matlab
+    data_matlab = dict()
+    
+    #%% TIME
+    if len(dataset.time_data_list) > 0:
+        T=0
+        fs=0
+        n_time=0
+        for time_data in dataset.time_data_list:
+            N = len(time_data.time_axis)
+            T = np.max([time_data.time_axis[-1]*N/(N-1),T])
+            fs = np.max([1/np.mean(np.diff(time_data.time_axis)),fs])
+            n_time += time_data.settings.channels
+        
+        t=np.arange(0,T,1/fs)
+        time_data_all = np.zeros((len(t),n_time))
+        counter = -1
+        for time_data in dataset.time_data_list:
+            for i in range(time_data.settings.channels):
+                counter += 1
+                time_data_all[:,counter] = np.interp(t,time_data.time_axis,time_data.time_data[:,i],right=0)
+                
+        data_matlab['time_axis_all'] = np.transpose(np.atleast_2d(t))
+        data_matlab['time_data_all'] = time_data_all
+
+    
+
+
+    #%% FFT - doesn't export coherence
+    if len(dataset.freq_data_list) > 0:
+        df=np.inf
+        fmax=0
+        n_tf=0
+        for freq_data in dataset.freq_data_list:
+            df_check = np.mean(np.diff(freq_data.freq_axis))
+            df = np.min([df,df_check])
+            fmax = np.max([freq_data.freq_axis[-1],fmax])
+            tf_shape = np.shape(freq_data.freq_data)
+            n_tf += tf_shape[1]
+        
+        f=np.arange(0,fmax+df,df)
+        npts = 2*(len(f)-1)
+        fs_tf = 2*f[-1]
+        freq_data_all = np.zeros((len(f),n_tf),dtype=complex)
+        counter = -1
+        for freq_data in dataset.freq_data_list:
+            freq_shape = np.shape(freq_data.freq_data)
+            for i in range(freq_shape[1]):
+                counter += 1
+                freq_data_all[:,counter] = np.interp(f,freq_data.freq_axis,freq_data.freq_data[:,i],right=0)
+        
+        data_matlab['freq_axis_all'] = np.transpose(np.atleast_2d(f))
+        data_matlab['freq_data_all'] = freq_data_all
+        
+ 
+
+
+    #%% Transfer Function - doesn't export coherence
+    if len(dataset.tf_data_list) > 0:
+        df=np.inf
+        fmax=0
+        n_tf=0
+        for tf_data in dataset.tf_data_list:
+            df_check = np.mean(np.diff(tf_data.freq_axis))
+            df = np.min([df,df_check])
+            fmax = np.max([tf_data.freq_axis[-1],fmax])
+            tf_shape = np.shape(tf_data.tf_data)
+            n_tf += tf_shape[1]
+        
+        f=np.arange(0,fmax+df,df)
+        npts = 2*(len(f)-1)
+        fs_tf = 2*f[-1]
+        tf_data_all = np.zeros((len(f),n_tf),dtype=complex)
+        counter = -1
+        for tf_data in dataset.tf_data_list:
+            tf_shape = np.shape(tf_data.tf_data)
+            for i in range(tf_shape[1]):
+                counter += 1
+                tf_data_all[:,counter] = np.interp(f,tf_data.freq_axis,tf_data.tf_data[:,i],right=0)
+        
+        data_matlab['tf_axis_all'] = np.transpose(np.atleast_2d(f))
+        data_matlab['tf_data_all'] = tf_data_all
+        
+
+    
+
+
+    #%% SAVE
+
+    # If filename not specified, provide dialog
+    if filename is None:
+        filename, _ = QFileDialog.getSaveFileName(parent, 'Save dataset', '', '*.mat')
+        if not filename:
+            # No filename chosen, give up on saving
+            print('Save cancelled')
+            return None
+
+
+    # If it exists, check if we should overwrite it (unless
+    # overwrite_without_prompt is True)
+    elif os.path.isfile(filename) and not overwrite_without_prompt:
+        answer = input('File %r already exists. Overwrite? [y/n]: ' % filename)
+        if answer != 'y':
+            print('Save cancelled')
+            return None
+        print('Will overwrite existing file')
+        
+    # Make sure it ends with .npy
+    if not filename.endswith('.mat'):
+        filename += '.mat'
+        
+    # Actually save!
+    io.savemat(filename,data_matlab)
+    print("Data saved as %s" % filename)
+
+    return filename
+
+
+
+#%% EXPORT TO MATLAB JWLOGGER
+def export_to_matlab_jwlogger(dataset, parent=None, filename=None, overwrite_without_prompt=False):
+    '''
+    Exports dataset class to file 'filename.mat', or provides dialog if no
+    filename provided.
+    
+    Saved file is compatible with Jim Woodhouse logger file format.
+
+    Args:
+       dataset: An object of the class dataSet
+       filename: string [optional]
+       overwrite_without_prompt: bool
+
+    '''
+
+    # convert data into dictionary ready for Matlab
+    data_jwlogger = dict()
+    
+    #%% TIME
+    if len(dataset.time_data_list) > 0:
+        T=0
+        fs=0
+        n_time=0
+        for time_data in dataset.time_data_list:
+            N = len(time_data.time_axis)
+            T = np.max([time_data.time_axis[-1]*N/(N-1),T])
+            fs = np.max([1/np.mean(np.diff(time_data.time_axis)),fs])
+            n_time += time_data.settings.channels
+        
+        t=np.arange(0,T,1/fs)
+        time_data_all = np.zeros((len(t),n_time))
+        counter = -1
+        for time_data in dataset.time_data_list:
+            for i in range(time_data.settings.channels):
+                counter += 1
+                time_data_all[:,counter] = np.interp(t,time_data.time_axis,time_data.time_data[:,i],right=0)
+                
+        data_jwlogger['buflen'] = float(np.size(t))
+        data_jwlogger['indata'] = time_data_all
+        data_jwlogger['tsmax'] = float(t[-1])
+    else:
+        n_time = 0
+        time_data_all = 0
+    
+    
+    #%% FFT: get's overwritten by TF if exists
+    if len(dataset.freq_data_list) > 0:
+        df=np.inf
+        fmax=0
+        n_freq=0
+        for freq_data in dataset.freq_data_list:
+            df_check = np.mean(np.diff(freq_data.freq_axis))
+            df = np.min([df,df_check])
+            fmax = np.max([freq_data.freq_axis[-1],fmax])
+            freq_shape = np.shape(freq_data.freq_data)
+            n_freq += freq_shape[1]
+        
+        f=np.arange(0,fmax+df,df)
+        npts = 2*(len(f)-1)
+        fs_freq = 2*f[-1]
+        freq_data_all = np.zeros((len(f),n_freq),dtype=complex)
+        counter = -1
+        for freq_data in dataset.freq_data_list:
+            freq_shape = np.shape(freq_data.freq_data)
+            for i in range(freq_shape[1]):
+                counter += 1
+                freq_data_all[:,counter] = np.interp(f,freq_data.freq_axis,freq_data.freq_data[:,i],right=1)
+                freq_data_all[0,counter] = freq_data_all[1,counter] # to match equivalent tweak in JW Logger for handling DC singularities
+                zero_test = freq_data_all[:,counter] == 0
+                freq_data_all[zero_test,counter] = np.min(np.abs(freq_data_all[:,counter])) # handle zeros
+        
+        # convert
+        data_jwlogger['freq'] = float(fs_freq)
+        data_jwlogger['npts'] = float(npts)
+        data_jwlogger['yspec'] = freq_data_all
+    else:
+        n_freq = 0
+        freq_data_all = 0
+    
+    
+    #%% Transfer Function - doesn't export coherence
+    if len(dataset.tf_data_list) > 0:
+        df=np.inf
+        fmax=0
+        n_tf=0
+        for tf_data in dataset.tf_data_list:
+            df_check = np.mean(np.diff(tf_data.freq_axis))
+            df = np.min([df,df_check])
+            fmax = np.max([tf_data.freq_axis[-1],fmax])
+            tf_shape = np.shape(tf_data.tf_data)
+            n_tf += tf_shape[1]
+        
+        f=np.arange(0,fmax+df,df)
+        npts = 2*(len(f)-1)
+        fs_tf = 2*f[-1]
+        tf_data_all = np.zeros((len(f),n_tf),dtype=complex)
+        counter = -1
+        for tf_data in dataset.tf_data_list:
+            tf_shape = np.shape(tf_data.tf_data)
+            for i in range(tf_shape[1]):
+                counter += 1
+                tf_data_all[:,counter] = np.interp(f,tf_data.freq_axis,tf_data.tf_data[:,i],right=1)
+                tf_data_all[0,counter] = tf_data_all[1,counter] # to match equivalent tweak in JW Logger for handling DC singularities
+                zero_test = freq_data_all[:,counter] == 0
+                tf_data_all[zero_test,counter] = np.min(np.abs(tf_data_all[:,counter])) # handle zeros
+        
+        # convert
+        data_jwlogger['freq'] = float(fs_tf)
+        data_jwlogger['npts'] = float(npts)
+        data_jwlogger['yspec'] = tf_data_all
+    else:
+        n_tf = 0
+        tf_data_all = 0
+    
+    #%% Convert
+    
+    if (n_freq > 0) & (n_tf > 0):
+        # if both FFT and TF data present then TF overwrites
+        N = n_tf
+    else:
+        # if only one of FFT or TF, or neither, then keep non-zero one, or neither
+        N = np.max([n_tf,n_freq])
+    
+    data_jwlogger['dt2'] = np.array([n_time,N,0],dtype=float)
+    data_jwlogger['dtype'] = np.array([n_time,N,0],dtype=float)
+    
+
+    # SAVE
+
+    # If filename not specified, provide dialog
+    if filename is None:
+        filename, _ = QFileDialog.getSaveFileName(parent, 'Save dataset', '', '*.mat')
+        if not filename:
+            # No filename chosen, give up on saving
+            print('Save cancelled')
+            return None
+
+
+    # If it exists, check if we should overwrite it (unless
+    # overwrite_without_prompt is True)
+    elif os.path.isfile(filename) and not overwrite_without_prompt:
+        answer = input('File %r already exists. Overwrite? [y/n]: ' % filename)
+        if answer != 'y':
+            print('Save cancelled')
+            return None
+        print('Will overwrite existing file')
+        
+    # Make sure it ends with .npy
+    if not filename.endswith('.mat'):
+        filename += '.mat'
+        
+    # Actually save!
+    io.savemat(filename,data_jwlogger)
+    print("Data saved as %s" % filename)
+
+    return filename
+
+
+def export_to_csv(data_list, parent=None, filename=None, overwrite_without_prompt=False):
+    '''
+    Exports data to file 'filename.csv', or provides dialog if no
+    filename provided.
+    
+    Saved file is *.csv
+
+    Args:
+       data_list: An object of the class TimeDataList, FreqDataList, or TfDataList
+       filename: string [optional]
+       overwrite_without_prompt: bool
+    '''
+    
+    data_list_type = data_list.__class__.__name__
+    
+    if data_list_type == 'TimeDataList':
+        darray = np.transpose(np.atleast_2d(data_list[0].time_axis))
+        for time_data in data_list:
+            darray = np.append(darray,time_data.time_data,axis=1)
+        
+            
+            
+    elif data_list_type == 'FreqDataList':
+        darray = np.transpose(np.atleast_2d(data_list[0].freq_axis))
+        for freq_data in data_list:
+            darray = np.append(darray,freq_data.freq_data,axis=1)
+        
+    elif data_list_type == 'TfDataList':
+        darray = np.transpose(np.atleast_2d(data_list[0].freq_axis))
+        for tf_data in data_list:
+            darray = np.append(darray,tf_data.tf_data,axis=1)
+        
+    else:
+        print('Expecting input to be one of TimeDataList, FreqDataList, or TfDataList')
+        return None
+    
+    # SAVE
+
+    # If filename not specified, provide dialog
+    if filename is None:
+        filename, _ = QFileDialog.getSaveFileName(parent, 'Save dataset', '', '*.csv')
+        if not filename:
+            # No filename chosen, give up on saving
+            print('Save cancelled')
+            return None
+
+
+    # If it exists, check if we should overwrite it (unless
+    # overwrite_without_prompt is True)
+    elif os.path.isfile(filename) and not overwrite_without_prompt:
+        answer = input('File %r already exists. Overwrite? [y/n]: ' % filename)
+        if answer != 'y':
+            print('Save cancelled')
+            return None
+        print('Will overwrite existing file')
+        
+    # Make sure it ends with .csv
+    if not filename.endswith('.csv'):
+        filename += '.csv'
+        
+    # Actually save!
+    np.savetxt(filename, darray, delimiter=",")
+    print("Data saved as %s" % filename)
+
     return filename
```

### Comparing `pydvma-0.9.0/pydvma/gui.py` & `pydvma-0.9.1/pydvma/gui.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,2854 +1,2854 @@
-from qtpy.QtWidgets import QMainWindow, QApplication, QWidget, QPushButton, QMessageBox, QTabWidget, QFormLayout, QToolBar, QLineEdit, QLabel, QComboBox, QSlider, QSizePolicy, QVBoxLayout, QHBoxLayout, QGridLayout, QGroupBox, QFrame, QStyleFactory, QSplitter, QFrame, QFormLayout
-from qtpy.QtCore import Qt, QThread, Signal, QTimer, QObject
-from qtpy.QtGui import QPalette, QDoubleValidator, QIntValidator, QFontMetrics
-from qtpy import QtGui
-from qtpy.QtWidgets import QToolTip, QFileDialog
-from qtpy import QtCore
-
-import pyqtgraph as pg
-
-import copy
-from matplotlib.backends.backend_qt5agg import FigureCanvas, NavigationToolbar2QT as NavigationToolbar
-from matplotlib.figure import Figure
-from matplotlib.ticker import AutoLocator
-import numpy as np
-import datetime
-
-
-
-
-#import logging
-#logging.basicConfig(filename='example.log',level=logging.DEBUG)
-#%%
-
-from . import plotting
-from . import datastructure
-from . import acquisition
-from . import analysis
-from . import streams
-from . import file
-from . import modal
-from . import options
-from . import oscilloscope
-import time
-import sys, os
-
-
-#%%
-class BlueButton(QPushButton):
-    def __init__(self,text):
-        super().__init__(text)
-        self.setStyleSheet("background-color: hsv(240, 170, 255)")
-        self.setText(text) 
-
-class GreenButton(QPushButton):
-    def __init__(self,text):
-        super().__init__(text)
-        self.setStyleSheet("background-color: hsv(120, 170, 255);")
-        self.setText(text)
-
-class RedButton(QPushButton):
-    def __init__(self,text):
-        super().__init__(text)
-        self.setStyleSheet("background-color: hsv(0, 170, 255)")
-        self.setText(text)
-        
-class OrangeButton(QPushButton):
-    def __init__(self,text):
-        super().__init__(text)
-        self.setStyleSheet("background-color: hsv(30, 170,255)")
-        self.setText(text)
-
-class QHLine(QFrame):
-    def __init__(self):
-        super(QHLine, self).__init__()
-        self.setFrameShape(QFrame.HLine)
-        self.setFrameShadow(QFrame.Sunken)
-        
-class newComboBox(QComboBox):
-    def __init__(self,items_list):
-        super().__init__()
-        self.setStyleSheet('selection-background-color: hsv(240, 170, 255)')
-        self.addItems(items_list)
-        
-class boldLabel(QLabel):
-    def __init__(self,text):
-        super().__init__(text)
-        self.setStyleSheet('font: bold')
-        
-        
-class LogDataThread(QThread):
-    
-    s = Signal(datastructure.DataSet)
-
-    def __init__(self,settings,test_name,rec,output):
-        super().__init__()
-        
-        self.settings = settings
-        self.test_name = test_name
-        self.rec = rec
-        self.output = output
-        
-    def __del__(self):
-        self.wait()
-    
-    def run(self):
-        self.d = acquisition.log_data(self.settings,test_name=self.test_name, rec=self.rec, output=self.output)
-        self.s.emit(self.d)
-        
-        
-        
-class PreviewWindow():
-    def __init__(self,title='Time Data'):
-        self.preview_window = QWidget()
-        self.preview_window.setStyleSheet("background-color: white")
-        self.preview_window.setWindowTitle('Output Signal Preview')
-        self.preview_window.setWindowIcon(QtGui.QIcon('pydvma/icon.png'))
-
-        self.fig = Figure(figsize=(9, 5),dpi=100)
-        self.canvas = FigureCanvas(self.fig)
-        self.toolbar = NavigationToolbar(self.canvas,None)
-        self.toolbar.setOrientation(Qt.Orientation.Horizontal)
-        self.p = plotting.PlotData(canvas=self.canvas,fig=self.fig)
-        
-        self.label_figure = boldLabel(title)
-        self.label_figure.setMaximumHeight(20)
-        self.label_figure.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        
-        # widgets to layout
-        self.layout_figure = QVBoxLayout()
-        self.layout_figure.addWidget(self.label_figure)
-        self.layout_figure.addWidget(self.canvas)
-        self.layout_figure.addWidget(self.toolbar)
-        
-        self.preview_window.setLayout(self.layout_figure)
-        
-        self.preview_window.showMinimized()
-        time.sleep(0.6)
-        self.preview_window.show()
-        self.preview_window.showNormal()
-        self.preview_window.raise_()
-        
-app = QApplication(sys.argv)
-app.setStyle(QStyleFactory.create('Fusion'))
-app.setWindowIcon(QtGui.QIcon('pydvma/icon.png'))
-
-class Logger():
-        
-    def __init__(self,settings=None,test_name=None,default_window=None):
-        
-        # Initialise variables
-        global MESSAGE
-        if default_window is None:
-            default_window = 'None'
-        self.settings = settings
-        self.test_name = test_name
-        self.dataset = datastructure.DataSet()
-        
-        self.default_window = default_window
-        self.current_view = 'Time'    
-        self.N_frames = 1
-        self.overlap = 0.5
-        self.iw_fft_power = 0
-        self.iw_tf_power = 0
-        self.legend_loc = 'lower right'
-        self.show_coherence = True
-        self.show_data = True
-        self.coherence_plot_type = 'linear'
-        self.xlinlog = 'linear'
-        self.plot_type = None
-        self.freq_range = [0,np.inf]
-        self.auto_xy = 'xy'
-        self.sets = 'all'
-        self.channels = 'all'
-        self.last_action = None
-        self.iw_power = 0
-        self.selected_channels = []
-        self.flag_scaling = False
-        self.message_time = 0
-        self.flag_log_and_replace = False
-        self.flag_output = False
-        self.message_timer = QTimer() # purely for pretrig live messages
-        self.stream_check_timer = QTimer() # for levels messages
-        self.levels_timer = QTimer() # for levels messages
-        self.message = ''
-        self.t0_clipped = 0
-        self.fn_in_range = np.array([])
-        
-        # SETUP GUI
-        # self.app = app
-        # self.app.setStyle(QStyleFactory.create('Fusion'))
-        self.window = QWidget()
-        self.window.setStyleSheet("background-color: white")
-        self.window.setWindowTitle('Logger')
-        self.window.setWindowIcon(QtGui.QIcon('pydvma/icon.png'))
-        # self.window.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
-        
-        # initiate all interface tool frames
-        self.setup_frame_tools()
-        self.setup_frame_input()
-        self.setup_frame_figure()
-        self.setup_frame_save()
-        self.setup_frame_axes()
-        
-        # arrange frames and create window
-        self.setup_layout_main()
-        self.window.showNormal()
-        # time.sleep(0.6)
-        self.window.show()
-        self.window.raise_()
-        # self.window.showNormal()
-        
-        
-        # start stream if already passed settings
-        self.start_stream()
-        self.message_timer.timeout.connect(self.show_message_timer) # connect after stream started
-        self.stream_check_timer.start(1000)
-        self.stream_check_timer.timeout.connect(self.check_stream) # connect after stream started
-        self.levels_timer.timeout.connect(self.show_levels) # connect after stream started
-        
-        app.exec()
-
-        
-    def setup_layout_main(self):
-
-        # organise frames
-        self.splitter_mid = QSplitter(Qt.Orientation.Vertical)
-        self.splitter_mid.addWidget(self.frame_input)
-        self.splitter_mid.addWidget(self.frame_figure)
-        self.splitter_mid.addWidget(self.frame_save)
-        
-        self.splitter_all = QSplitter(Qt.Orientation.Horizontal)
-        self.splitter_all.addWidget(self.frame_axes)
-        self.splitter_all.addWidget(self.splitter_mid)
-        self.splitter_all.addWidget(self.frame_tools)
-        
-        # frames to main layout
-        self.layout_main = QGridLayout()
-        self.layout_main.addWidget(self.splitter_all)
-        
-        # main layout to window
-        self.window.setLayout(self.layout_main)
-        
-
-    def setup_frame_figure(self):
-        # content
-        
-        self.fig = Figure(figsize=(9, 7),dpi=100)
-        self.canvas = FigureCanvas(self.fig)
-        self.toolbar = NavigationToolbar(self.canvas,None)
-        
-        # disable some buttons
-        for ch in self.toolbar.children():
-            try:
-                if ch.iconText() in ['Home','Subplots','Save','Customize']:
-                    ch.setVisible(False)
-            except:
-                pass
-        
-        self.toolbar.setOrientation(Qt.Orientation.Horizontal)
-        self.p = plotting.PlotData(canvas=self.canvas,fig=self.fig)
-        self.p.ax.callbacks.connect('xlim_changed', self.update_axes_values)
-        self.p.ax.callbacks.connect('ylim_changed', self.update_axes_values)
-        self.p.ax.callbacks.connect('xlim_changed', self.update_modal_message)
-        self.p.ax2.callbacks.connect('ylim_changed', self.update_co_axes_values)
-        self.fig.canvas.mpl_connect('pick_event', self.update_selected_channels)
-        
-        self.label_figure = boldLabel('Time Data')
-        self.label_figure.setMaximumHeight(20)
-        self.label_figure.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        
-        # widgets to layout
-        self.layout_figure = QGridLayout()
-        self.layout_figure.addWidget(self.label_figure,0,0,1,3)
-        self.layout_figure.addWidget(self.canvas,1,0,1,3)
-        self.layout_figure.addWidget(self.toolbar,2,1,1,1)
-        self.layout_figure.addWidget(QLabel('Back/Forward/Pan/Zoom:'),2,0,1,1)
-#        self.layout_figure.addWidget(QLabel('(box-zoom right-click will zoom out)'),2,2,1,1)
-        
-        # layout to frame
-        self.frame_figure = QFrame()
-        self.frame_figure.setFrameShape(QFrame.Shape.StyledPanel)
-        self.frame_figure.setLayout(self.layout_figure)
-        
-    def setup_frame_input(self):
-        
-        self.setup_frame_message()
-        
-        # content
-        self.button_osc = QPushButton('')
-        self.button_osc.setIcon(QtGui.QIcon('pydvma/icon.png'))
-        self.button_log_data = GreenButton('Log Data')
-        self.button_del_data = OrangeButton('Delete Last')
-        self.button_res_data = RedButton('Delete All')
-        self.button_load_data = BlueButton('Load Data')
-                
-        self.button_osc.clicked.connect(self.button_clicked_osc)
-        self.button_log_data.clicked.connect(self.button_clicked_log_data)
-        self.button_del_data.clicked.connect(self.delete_last_data)
-        self.button_res_data.clicked.connect(self.reset_data)
-        self.button_load_data.clicked.connect(self.load_data)
-        
-        # widgets to layout
-        self.layout_input = QGridLayout()
-        self.layout_input.addWidget(self.button_osc,0,0,1,1)
-        self.layout_input.addWidget(self.button_log_data,0,1,1,4)
-        self.layout_input.addWidget(self.button_del_data,0,5,1,4)
-        self.layout_input.addWidget(self.button_res_data,0,9,1,4)
-        self.layout_input.addWidget(self.button_load_data,0,13,1,4)
-        self.layout_input.addWidget(self.frame_message,1,0,1,17)
-        self.layout_input.setAlignment(Qt.AlignmentFlag.AlignTop)
-        
-        # layout to frame
-        self.frame_input = QFrame()
-        self.frame_input.setFrameShape(QFrame.Shape.StyledPanel)
-        self.frame_input.setLayout(self.layout_input)
-        
-        
-    def setup_frame_message(self):
-        self.label_message = QLabel()
-        self.button_message = GreenButton('OK')
-        self.button_cancel = OrangeButton('Cancel')
-        self.button_undo = RedButton('Undo')
-        
-        # function connections
-        self.button_message.clicked.connect(self.hide_message)
-        self.button_cancel.clicked.connect(self.cancel_logging)
-        self.button_undo.clicked.connect(self.undo_last_action)
-        
-        self.layout_message = QGridLayout()
-        
-        self.layout_message.addWidget(self.label_message,0,0,1,3)
-        self.layout_message.addWidget(self.button_message,0,3,1,1)
-        self.layout_message.addWidget(self.button_cancel,0,3,1,1)
-        self.layout_message.addWidget(self.button_undo,1,3,1,1)
-        self.layout_message.setAlignment(Qt.AlignmentFlag.AlignTop)
-        
-        self.frame_message = QFrame()
-        self.frame_message.setLayout(self.layout_message)
-        self.hide_message()
-        
-        
-    def setup_frame_save(self):
-        # design items
-#        self.label_save = QLabel('Quick save:')
-        self.buttons_save = [GreenButton(i) for i in ['Save Dataset','Save Figure']]
-        self.buttons_save[0].clicked.connect(self.save_data)
-        self.buttons_save[1].clicked.connect(self.save_fig)
-        
-        # widgets to layout
-        self.layout_save = QHBoxLayout()
-        for n in range(len(self.buttons_save)):
-            self.layout_save.addWidget(self.buttons_save[n])
-            
-        # layout to frame
-        self.frame_save = QFrame()
-        self.frame_save.setFrameShape(QFrame.Shape.StyledPanel)
-        self.frame_save.setLayout(self.layout_save)
-        
-    
-    def setup_frame_axes(self):
-        
-        self.setup_frame_plot_details()
-        
-        self.input_list_figures = newComboBox(['Time Data','FFT Data','TF Data','Sono Data'])
-        self.input_list_figures.currentIndexChanged.connect(self.select_view)
-        
-        self.button_x = GreenButton('Auto X')
-        self.button_y = GreenButton('Auto Y')
-        
-        self.button_x.clicked.connect(self.auto_x)
-        self.button_y.clicked.connect(self.auto_y)
-        
-        self.label_axes = [QLabel(i) for i in ['xmin:','xmax:','ymin:','ymax:']]
-        self.input_axes = [QLineEdit() for i in range(4)]
-        self.input_axes[0].setValidator(QDoubleValidator(float(0),float(np.inf),5)) 
-        self.input_axes[0].editingFinished.connect(self.xmin)
-        self.input_axes[1].setValidator(QDoubleValidator(float(0),float(np.inf),5)) 
-        self.input_axes[1].editingFinished.connect(self.xmax)
-        self.input_axes[2].setValidator(QDoubleValidator(float(-np.inf),float(np.inf),5)) 
-        self.input_axes[2].editingFinished.connect(self.ymin)
-        self.input_axes[3].setValidator(QDoubleValidator(float(-np.inf),float(np.inf),5)) 
-        self.input_axes[3].editingFinished.connect(self.ymax)
-        
-        self.button_select_all_data = GreenButton('All')
-        self.button_select_no_data = GreenButton('None')
-        self.button_select_all_data.clicked.connect(self.select_all_data)
-        self.button_select_no_data.clicked.connect(self.select_no_data)
-        
-        self.button_select_next = GreenButton('>')
-        self.button_select_prev = GreenButton('<')
-        self.button_select_next.clicked.connect(self.next_chans)
-        self.button_select_prev.clicked.connect(self.prev_chans)
-        width = self.button_select_next.fontMetrics().boundingRect('>').width()*4
-        self.button_select_next.setMaximumWidth(width)
-        self.button_select_prev.setMaximumWidth(width)
-        
-        self.button_select_set_only = BlueButton('Show Set Only')
-        self.button_select_set_only.clicked.connect(self.show_set_only)
-        self.button_select_chan_only = BlueButton('Show Chan Only')
-        self.button_select_chan_only.clicked.connect(self.show_chan_only)
-        
-        self.input_select_set_only = QLineEdit('0')
-        self.input_select_set_only.setValidator(QIntValidator(0,1000))
-        self.input_select_chan_only = QLineEdit('0')
-        self.input_select_chan_only.setValidator(QIntValidator(0,1000))
-        
-        self.legend_buttons = [BlueButton(i) for i in ['left','on/off','right']]
-        self.legend_buttons[0].clicked.connect(self.legend_left)
-        self.legend_buttons[1].clicked.connect(self.legend_onoff)
-        self.legend_buttons[2].clicked.connect(self.legend_right)
-        
-        
-        # widgets to layout
-        self.layout_axes = QGridLayout()
-        self.layout_axes.setAlignment(Qt.AlignmentFlag.AlignTop)
-
-
-        # Figure selection
-        row_start = 0
-        self.layout_axes.addWidget(boldLabel('Figure selection:'),row_start+0,0,1,6)
-        self.layout_axes.addWidget(self.input_list_figures,row_start+1,0,1,6)
-        
-        # Axes control
-        row_start = 3
-        self.layout_axes.addWidget(QLabel(),row_start,0,1,6)
-        self.layout_axes.addWidget(boldLabel('Axes control:'),row_start+1,0,1,6)
-        self.layout_axes.addWidget(self.button_x,row_start+2,0,1,3)
-        self.layout_axes.addWidget(self.button_y,row_start+2,3,1,3)
-        
-        for n in range(len(self.label_axes)):
-            self.label_axes[n].setAlignment(Qt.AlignmentFlag.AlignRight)
-            self.layout_axes.addWidget(self.label_axes[n],row_start+n+4,0,1,2)
-            self.layout_axes.addWidget(self.input_axes[n],row_start+n+4,2,1,4)
-            
-        # Line Selection
-        row_start = 11
-        self.layout_axes.addWidget(QLabel(),row_start,0,1,6)
-        self.layout_axes.addWidget(boldLabel('Line Selection:'),row_start+1,0,1,6)
-        self.layout_axes.addWidget(self.button_select_all_data,row_start+2,0,1,2)
-        self.layout_axes.addWidget(self.button_select_no_data,row_start+2,2,1,2)
-        self.layout_axes.addWidget(self.button_select_prev,row_start+2,4,1,1)
-        self.layout_axes.addWidget(self.button_select_next,row_start+2,5,1,1)
-        self.layout_axes.addWidget(self.button_select_set_only,row_start+3,0,1,3)
-        self.layout_axes.addWidget(self.input_select_set_only,row_start+3,3,1,3)
-        self.layout_axes.addWidget(self.button_select_chan_only,row_start+4,0,1,3)
-        self.layout_axes.addWidget(self.input_select_chan_only,row_start+4,3,1,3)
-        
-        
-        # Legend control
-        row_start = 17
-        self.layout_axes.addWidget(QLabel(),row_start,0,1,6)
-        self.layout_axes.addWidget(boldLabel('Legend control:'),row_start+1,0,1,6)
-        for n in range(len(self.legend_buttons)):
-            self.layout_axes.addWidget(self.legend_buttons[n],row_start+2,2*n,1,2)
-        
-        
-        # Plot-specific tools
-        row_start = 20
-        self.layout_axes.addWidget(self.frame_plot_details,row_start,0,1,6)
-        self.frame_plot_details.setVisible(False)
-        
-        # layout to frame
-        self.frame_axes = QFrame()
-        self.frame_axes.setFrameShape(QFrame.Shape.StyledPanel)
-        self.frame_axes.setLayout(self.layout_axes)
-       
-    def setup_frame_plot_details(self):
-        #items
-        self.items_list_plot_type = ['Amplitude (dB)','Amplitude (linear)', 'Real Part', 'Imag Part', 'Nyquist', 'Phase']
-        self.input_list_plot_type = newComboBox(self.items_list_plot_type)
-        self.button_xlinlog = BlueButton('X Lin/Log')
-        self.button_data_toggle = BlueButton('Data on/off')
-        self.button_coherence_toggle = BlueButton('Coherence on/off')
-        
-        
-        self.label_co_freq_min = QLabel('co. min:')
-        self.label_co_freq_max = QLabel('co. max:')
-        self.input_co_min = QLineEdit('0')
-        self.input_co_min.setValidator(QDoubleValidator(float(-np.inf),float(np.inf),5))
-        self.input_co_max = QLineEdit('1')
-        self.input_co_max.setValidator(QDoubleValidator(float(-np.inf),float(np.inf),5))
-        
-        # freq range for Nyquist
-        self.input_freq_min = QLineEdit()
-        self.input_freq_min.setValidator(QDoubleValidator(float(0),float(np.inf),5))
-        self.input_freq_min.editingFinished.connect(self.freq_min)
-        self.input_freq_max = QLineEdit()
-        self.input_freq_max.setValidator(QDoubleValidator(float(0),float(np.inf),5))
-        self.input_freq_max.editingFinished.connect(self.freq_max)
-        
-        #self.button_modal_fit_toggle = BlueButton('Modal Fit on/off')
-        
-#        self.input_list_plot_type.currentIndexChanged.connect(self.select_view)
-        self.input_list_plot_type.activated.connect(self.select_view) # TRY THIS SO ONLY CALLED WITH MANUAL SELECTION NOT WITHIN SELECT_VIEW
-        self.input_co_min.editingFinished.connect(self.co_min)
-        self.input_co_max.editingFinished.connect(self.co_max)
-        self.button_data_toggle.clicked.connect(self.data_toggle)
-        self.button_coherence_toggle.clicked.connect(self.coherence_toggle)
-        self.button_xlinlog.clicked.connect(self.select_xlinlog)
-        #layout
-        self.layout_plot_details = QGridLayout()
-        self.layout_plot_details.addWidget(QLabel(),0,0,1,1)
-        self.layout_plot_details.addWidget(boldLabel('Plot type:'),1,0,1,2)
-        self.layout_plot_details.addWidget(self.input_list_plot_type,2,0,1,2)
-        self.layout_plot_details.addWidget(self.button_xlinlog,3,0,1,2)
-        self.layout_plot_details.addWidget(self.button_data_toggle,4,0,1,1)
-        self.layout_plot_details.addWidget(self.button_coherence_toggle,4,1,1,1)
-        self.layout_plot_details.addWidget(self.label_co_freq_min,5,0,1,1)
-        self.layout_plot_details.addWidget(self.input_co_min,5,1,1,1)
-        self.layout_plot_details.addWidget(self.input_freq_min,5,1,1,1)
-        self.layout_plot_details.addWidget(self.label_co_freq_max,6,0,1,1)
-        self.layout_plot_details.addWidget(self.input_co_max,6,1,1,1)
-        self.layout_plot_details.addWidget(self.input_freq_max,6,1,1,1)
-        #self.layout_plot_details.addWidget(self.button_modal_fit_toggle,7,0,1,2)        
-        
-        #only show these for Nyquist plots
-        self.input_freq_min.setVisible(False)
-        self.input_freq_max.setVisible(False)
-        
-        #frame
-        self.frame_plot_details = QFrame()
-        self.frame_plot_details.setLayout(self.layout_plot_details)
-    
-    
-    def setup_frame_tools(self):
-        
-        # initiate all tools frames
-        self.setup_frame_tools_selection()
-        self.setup_frame_tools_time_domain()
-        self.setup_frame_tools_fft()
-        self.setup_frame_tools_tf()
-        self.setup_frame_tools_scaling()
-        self.setup_frame_tools_mode_fitting()
-        self.setup_frame_tools_settings()
-        self.setup_frame_tools_generate_output()
-        self.setup_frame_tools_edit_dataset()
-        self.setup_frame_tools_sonogram()
-        self.setup_frame_tools_save_export()
-        
-        # widgets to layout
-        self.layout_tools = QVBoxLayout()
-        self.layout_tools.addWidget(self.frame_tools_selection)
-        self.layout_tools.addWidget(self.frame_tools_time_domain)
-        self.layout_tools.addWidget(self.frame_tools_fft)
-        self.layout_tools.addWidget(self.frame_tools_tf)
-        self.layout_tools.addWidget(self.frame_tools_scaling)
-        self.layout_tools.addWidget(self.frame_tools_mode_fitting)
-        self.layout_tools.addWidget(self.frame_tools_settings)
-        self.layout_tools.addWidget(self.frame_tools_generate_output)
-        self.layout_tools.addWidget(self.frame_tools_edit_dataset)
-        self.layout_tools.addWidget(self.frame_tools_sonogram)
-        self.layout_tools.addWidget(self.frame_tools_save_export)
-        
-        self.layout_tools.setAlignment(Qt.AlignmentFlag.AlignTop)
-        
-        # layout to frame
-        self.frame_tools = QFrame()
-        self.frame_tools.setFrameShape(QFrame.Shape.StyledPanel)
-        self.frame_tools.setLayout(self.layout_tools)
-        
-        # widgets to layout according to selection
-        self.input_list_tools.setCurrentText('Standard Tools')
-        self.select_tool()
-        
-        
-        
-        
-    def setup_frame_tools_selection(self):
-        
-        self.input_list_tools = newComboBox(['Standard Tools','Logger Settings','Generate Output','Pre-process','FFT','Transfer Function','Calibration / Scaling','Sonogram','Mode Fitting','Edit Dataset','Save / Export'])
-        self.input_list_tools.setCurrentIndex(0)
-        self.input_list_tools.currentIndexChanged.connect(self.select_tool)
-        
-        self.layout_tools_selection = QGridLayout()
-        self.layout_tools_selection.addWidget(boldLabel('Tool selection:'),0,0,1,3)
-        self.layout_tools_selection.addWidget(self.input_list_tools,1,0,1,3)
-        
-        self.frame_tools_selection = QFrame()
-        self.frame_tools_selection.setLayout(self.layout_tools_selection)
-        
-
-
-    def setup_frame_tools_time_domain(self):
-        
-        self.button_clean_impulse = BlueButton('Clean Impulse')
-        self.button_clean_impulse.clicked.connect(self.clean_impulse)
-        
-        self.input_impulse_channel = QLineEdit('0')
-        self.input_impulse_channel.setValidator(QIntValidator(0,1000))
-        self.layout_tools_time_domain = QGridLayout()
-        self.layout_tools_time_domain.addWidget(boldLabel('Pre-process:'),0,0,1,3)
-        self.layout_tools_time_domain.addWidget(QLabel('Impulse channel:'),1,0,1,1)
-        self.layout_tools_time_domain.addWidget(self.input_impulse_channel,1,1,1,2)
-        self.layout_tools_time_domain.addWidget(self.button_clean_impulse,2,0,1,3)
-        
-        self.frame_tools_time_domain = QFrame()
-        self.frame_tools_time_domain.setLayout(self.layout_tools_time_domain)
-
-
-    def setup_frame_tools_fft(self):
-        
-        self.input_list_window_fft = newComboBox(['None','hann'])
-        self.input_list_window_fft.setCurrentText(self.default_window)
-        self.button_FFT = BlueButton('Calc FFT')
-        self.button_FFT.clicked.connect(self.calc_fft)
-        
-        self.layout_tools_fft = QGridLayout()
-        self.layout_tools_fft.addWidget(boldLabel('FFT:'),0,0,1,3)
-        self.layout_tools_fft.addWidget(QLabel('window:'),1,0,1,1)
-        self.layout_tools_fft.addWidget(self.input_list_window_fft,1,1,1,2)
-        self.layout_tools_fft.addWidget(self.button_FFT,2,0,1,3)
-        
-        self.frame_tools_fft = QFrame()
-        self.frame_tools_fft.setLayout(self.layout_tools_fft)
-
-    def setup_frame_tools_tf(self):
-        self.input_list_window_tf = newComboBox(['None','hann'])
-        self.input_list_window_tf.setCurrentText(self.default_window)
-        self.input_list_average_TF = newComboBox(['None','within each set','across sets'])
-        self.input_list_average_TF.setCurrentText(self.default_window)
-        self.button_TF = BlueButton('Calc TF')
-        self.button_TF.clicked.connect(self.calc_tf)
-        self.input_list_average_TF.currentIndexChanged.connect(self.select_averaging_type)
-        self.label_Nframes = QLabel('N frames:')
-        self.input_Nframes = QLineEdit()
-        self.input_Nframes.setValidator(QIntValidator(1,1000))
-        self.input_Nframes.setText('1')
-        self.input_Nframes.editingFinished.connect(self.refresh_Nframes_slider)
-        self.input_Nframes.editingFinished.connect(self.calc_tf)
-        
-        self.slider_Nframes = QSlider(Qt.Orientation.Horizontal)
-        self.slider_Nframes.setMinimum(1)
-        self.slider_Nframes.setMaximum(30)
-        self.slider_Nframes.valueChanged.connect(self.refresh_Nframes_text)
-        self.slider_Nframes.valueChanged.connect(self.calc_tf)
-        
-        self.label_Nframes_time = QLabel('')
-        
-        self.button_TFav = BlueButton('Calc TF average')
-        self.button_TFav.clicked.connect(self.calc_tf_av)
-        
-        
-        self.layout_tools_tf = QGridLayout()
-        self.layout_tools_tf.addWidget(boldLabel('Transfer Function:'),0,0,1,3)
-        self.layout_tools_tf.addWidget(QLabel('window:'),1,0,1,1)
-        self.layout_tools_tf.addWidget(self.input_list_window_tf,1,1,1,2)
-        self.layout_tools_tf.addWidget(QLabel('average:'),2,0,1,1)
-        self.layout_tools_tf.addWidget(self.input_list_average_TF,2,1,1,2)
-        self.layout_tools_tf.addWidget(self.label_Nframes,3,0,1,1)
-        self.layout_tools_tf.addWidget(self.input_Nframes,3,1,1,2)
-        self.layout_tools_tf.addWidget(self.slider_Nframes,4,0,1,3)
-        self.layout_tools_tf.addWidget(self.label_Nframes_time,5,0,1,3)
-        self.layout_tools_tf.addWidget(self.button_TF,6,0,1,3)
-        self.layout_tools_tf.addWidget(self.button_TFav,6,0,1,3)
-        
-        # initiate view
-        self.input_list_average_TF.setCurrentIndex(0)
-        self.input_Nframes.setText('1')
-        self.slider_Nframes.setValue(1)
-        self.label_Nframes.setVisible(False)
-        self.input_Nframes.setVisible(False)
-        self.slider_Nframes.setVisible(False)
-        self.label_Nframes_time.setVisible(False)
-        self.button_TFav.setVisible(False)
-        self.button_TF.setVisible(True)
-        
-        
-        self.frame_tools_tf = QFrame()
-        self.frame_tools_tf.setLayout(self.layout_tools_tf)
-        
-        
-    def setup_frame_tools_scaling(self):
-        self.input_iw_power = QLineEdit('0')
-        self.input_iw_power.setValidator(QIntValidator(0,2))
-        
-        self.button_xiw = BlueButton('x (iw)')
-        self.button_diw = BlueButton('x 1/(iw)')
-        self.button_xiw.clicked.connect(self.xiw)
-        self.button_diw.clicked.connect(self.diw)
-        
-        self.input_refset = QLineEdit('0')
-        self.input_refset.setValidator(QIntValidator(0,1000))
-        self.input_refchan = QLineEdit('0')
-        self.input_refchan.setValidator(QIntValidator(0,1000))
-
-        self.button_best_match = BlueButton('Best Match (to ref)')
-        self.button_best_match.clicked.connect(self.best_match)
-        self.button_undo_scaling = RedButton('Undo All Scaling')
-        self.button_undo_scaling.clicked.connect(self.undo_scaling)        
-        
-        self.layout_tools_scaling = QGridLayout()
-        self.layout_tools_scaling.addWidget(boldLabel('Calibration / Scaling:'),0,0,1,4)
-        self.layout_tools_scaling.addWidget(self.button_xiw,1,0,1,2)
-        self.layout_tools_scaling.addWidget(self.button_diw,1,2,1,2)
-        
-        self.layout_tools_scaling.addWidget(QLabel('Ref set / chan:'),2,0,1,2)
-        self.layout_tools_scaling.addWidget(self.input_refset,2,2,1,1)
-        self.layout_tools_scaling.addWidget(self.input_refchan,2,3,1,1)
-        
-        self.layout_tools_scaling.addWidget(self.button_best_match,3,0,1,4)
-        self.layout_tools_scaling.addWidget(self.button_undo_scaling,4,0,1,4)
-        
-        self.frame_tools_scaling = QFrame()
-        self.frame_tools_scaling.setLayout(self.layout_tools_scaling)
-        
-    def setup_frame_tools_mode_fitting(self):
-        self.input_freq_min2 = QLineEdit()
-        self.input_freq_min2.setValidator(QDoubleValidator(float(0),float(np.inf),5))
-        self.input_freq_min2.editingFinished.connect(self.freq_min2)
-        self.input_freq_max2 = QLineEdit()
-        self.input_freq_max2.setValidator(QDoubleValidator(float(0),float(np.inf),5))
-        self.input_freq_max2.editingFinished.connect(self.freq_max2)
-        
-        self.input_list_tf_type = newComboBox(['Acceleration','Velocity','Displacement'])
-        
-        self.button_fit_mode = GreenButton('Fit')
-        self.button_fit_mode.clicked.connect(self.fit_mode)
-        self.button_reject_mode = RedButton('Reject')
-        self.button_reject_mode.clicked.connect(self.reject_mode)
-        self.button_view_mode_summary = BlueButton('Summary')
-        self.button_view_mode_summary.clicked.connect(self.view_mode_summary)
-        self.button_view_modal_reconstruction = BlueButton('Reconstruction')
-        self.button_view_modal_reconstruction.clicked.connect(self.view_modal_reconstruction)
-        
-        self.layout_tools_mode_fitting = QGridLayout()
-        self.layout_tools_mode_fitting.addWidget(boldLabel('Mode Fitting:'),0,0,1,4)
-        self.layout_tools_mode_fitting.addWidget(QLabel('TF type:'),1,0,1,1)
-        self.layout_tools_mode_fitting.addWidget(self.input_list_tf_type,1,1,1,3)
-        
-        self.layout_tools_mode_fitting.addWidget(QLabel('Zoom to view a single peak:'),2,0,1,4)
-        self.layout_tools_mode_fitting.addWidget(QLabel('fmin:'),3,0,1,1)
-        self.layout_tools_mode_fitting.addWidget(self.input_freq_min2,3,1,1,3)
-        self.layout_tools_mode_fitting.addWidget(QLabel('fmax:'),4,0,1,1)
-        self.layout_tools_mode_fitting.addWidget(self.input_freq_max2,4,1,1,3)
-        self.layout_tools_mode_fitting.addWidget(self.button_fit_mode,5,0,1,2)
-        self.layout_tools_mode_fitting.addWidget(self.button_reject_mode,5,2,1,2)
-        self.layout_tools_mode_fitting.addWidget(self.button_view_mode_summary,6,0,1,4)
-        self.layout_tools_mode_fitting.addWidget(self.button_view_modal_reconstruction,7,0,1,4)
-        
-        self.frame_tools_mode_fitting = QFrame()
-        self.frame_tools_mode_fitting.setLayout(self.layout_tools_mode_fitting)
-        
-    def setup_frame_tools_settings(self):
-        
-        if self.settings is None:
-            self.settings = options.MySettings()
-            
-            
-        self.button_apply_settings = GreenButton('Apply Settings')
-        self.button_apply_settings.clicked.connect(self.apply_settings)
-        
-        self.button_show_available_devices = BlueButton('Show Available Devices')
-        self.button_show_available_devices.clicked.connect(self.show_available_devices)
-        
-        self.settings_dict = self.settings.__dict__
-        self.labels_settings = list(self.settings_dict.keys())
-        self.values_settings = list(self.settings_dict.values())
-        
-        self.input_settings = dict()
-        for (label,value) in self.settings_dict.items():
-            self.input_settings[label] = QLineEdit(str(value))
-        
-            
-        
-        NI = streams.get_devices_NI()
-        SC = streams.get_devices_soundcard()
-        
-        if NI == (None,None):
-            self.input_list_devices = []
-        else:
-            self.input_list_devices = ['nidaq']
-        if SC != None:
-            self.input_list_devices += ['soundcard']
-        
-        self.input_test_name = QLineEdit()
-        self.input_test_name.editingFinished.connect(self.refresh_test_name)
-        
-        self.layout_tools_settings = QFormLayout()
-        
-        self.layout_tools_settings.addWidget(boldLabel('Input Settings:'))
-        self.layout_tools_settings.addRow(QLabel('Test Name:'),self.input_test_name)
-        for n_row in range(9):
-            self.layout_tools_settings.addRow(QLabel(self.labels_settings[n_row]),self.input_settings[self.labels_settings[n_row]])
-        self.layout_tools_settings.addWidget(boldLabel('Output Settings:'))
-        for n_row in range(9,14):
-            self.layout_tools_settings.addRow(QLabel(self.labels_settings[n_row]),self.input_settings[self.labels_settings[n_row]])
-        
-        self.layout_tools_settings.addWidget(self.button_show_available_devices)
-        self.layout_tools_settings.addWidget(self.button_apply_settings)
-        self.frame_tools_settings = QFrame()
-        self.frame_tools_settings.setLayout(self.layout_tools_settings)
-        
-    def setup_frame_tools_generate_output(self):
-        self.list_output_options = ['None','sweep','gaussian','uniform']
-        self.input_output_options = newComboBox(self.list_output_options)
-        self.input_output_options.currentTextChanged.connect(self.update_output)
-        
-        self.input_output_amp = QLineEdit('0')
-        v = QDoubleValidator(0.0,1.0,5)
-        v.setNotation(QDoubleValidator.Notation.StandardNotation)
-        self.input_output_amp.setValidator(v)
-        
-        self.input_output_f1 = QLineEdit('0')
-        self.input_output_f1.setValidator(QDoubleValidator(0.0,float(np.inf),5))
-        
-        self.input_output_f2 = QLineEdit('0')
-        self.input_output_f2.setValidator(QDoubleValidator(0.0,float(np.inf),5))
-        
-        self.input_output_duration = QLineEdit(str(self.settings.stored_time))
-        self.input_output_duration.setValidator(QDoubleValidator(0.0,float(np.inf),5))
-        
-        self.button_output_preview = BlueButton('Preview Output')
-        self.button_output_preview.clicked.connect(self.preview_output)
-        
-        self.button_start_output = BlueButton('Start Output')
-        self.button_start_output.clicked.connect(self.start_output)
-        
-        self.button_log_with_output = GreenButton('Log with Output')
-        self.button_log_with_output.clicked.connect(self.button_clicked_log_data)
-        
-        
-        self.input_test_name2 = QLineEdit()
-        self.input_test_name2.editingFinished.connect(self.refresh_test_name2)
-        
-        self.layout_tools_generate_output = QFormLayout()
-        
-        self.layout_tools_generate_output.addRow(boldLabel('Generate Outputs:'))
-        self.layout_tools_generate_output.addRow(QLabel('Test Name:'),self.input_test_name2)
-        self.layout_tools_generate_output.addRow(QLabel('Type:'),self.input_output_options)
-        self.layout_tools_generate_output.addRow(QLabel('Amplitude (0-1):'),self.input_output_amp)
-        self.layout_tools_generate_output.addRow(QLabel('f1 (Hz):'),self.input_output_f1)
-        self.layout_tools_generate_output.addRow(QLabel('f2 (Hz):'),self.input_output_f2)
-        self.layout_tools_generate_output.addRow(QLabel('Duration (s):'),self.input_output_duration)
-        self.layout_tools_generate_output.addRow(self.button_output_preview)
-        self.layout_tools_generate_output.addRow(self.button_start_output)
-        self.layout_tools_generate_output.addRow(self.button_log_with_output)
-        
-        self.frame_tools_generate_output = QFrame()
-        self.frame_tools_generate_output.setLayout(self.layout_tools_generate_output)
-        
-    
-    def setup_frame_tools_edit_dataset(self):
-        self.list_data_type = ['Time Data','FFT Data','TF Data','Modal Data','Sono Data']
-        
-        self.input_list_data_type = newComboBox(self.list_data_type)
-        self.input_list_data_type.setCurrentText('Time Data')
-        self.input_list_data_type.currentIndexChanged.connect(self.update_selected_set)
-        
-        self.button_delete_data_type = RedButton('Delete all data of this type')
-        self.button_delete_data_type.clicked.connect(self.delete_data_type)
-        
-        self.button_delete_data_set = OrangeButton('Delete Selected Set')
-        self.button_delete_data_set.clicked.connect(self.delete_data_set)
-        
-        self.input_selected_set = QLineEdit()
-        self.input_selected_set.setValidator(QIntValidator(0,1000))
-
-        self.button_log_replace = GreenButton('Log && Replace Selected Set')
-        self.button_log_replace.clicked.connect(self.log_and_replace)
-        
-        text = self.dataset.__repr__()
-        self.label_data_summary = QLabel(text)
-        
-        self.layout_tools_edit_dataset = QGridLayout()
-        self.layout_tools_edit_dataset.addWidget(boldLabel('Dataset Summary'),0,0,1,4)
-        self.layout_tools_edit_dataset.addWidget(self.label_data_summary,1,0,1,4)
-        self.layout_tools_edit_dataset.addWidget(boldLabel('Edit Dataset'),2,0,1,4)
-        self.layout_tools_edit_dataset.addWidget(QLabel('Selected Type:'),3,0,1,2)
-        self.layout_tools_edit_dataset.addWidget(self.input_list_data_type,3,2,1,2)
-        self.layout_tools_edit_dataset.addWidget(self.button_delete_data_type,4,0,1,4)
-        self.layout_tools_edit_dataset.addWidget(QLabel('Selected Set:'),5,0,1,2)
-        self.layout_tools_edit_dataset.addWidget(self.input_selected_set,5,2,1,2)
-        self.layout_tools_edit_dataset.addWidget(self.button_delete_data_set,6,0,1,4)
-        self.layout_tools_edit_dataset.addWidget(self.button_log_replace,7,0,1,4)
-        
-        self.frame_tools_edit_dataset = QFrame()
-        self.frame_tools_edit_dataset.setLayout(self.layout_tools_edit_dataset)
-        
-    def setup_frame_tools_sonogram(self):
-        self.input_sono_N_frames = QLineEdit('50')
-        self.input_sono_N_frames.setValidator(QIntValidator(10,10000))
-        self.input_sono_N_frames.editingFinished.connect(self.refresh_sono_N_frames_slider)
-        self.input_sono_N_frames.editingFinished.connect(self.calc_sono)
-        
-        self.slider_sono_N_frames = QSlider(Qt.Orientation.Horizontal)
-        self.slider_sono_N_frames.setMinimum(10)
-        self.slider_sono_N_frames.setMaximum(500)
-        self.slider_sono_N_frames.setValue(50)
-        self.slider_sono_N_frames.valueChanged.connect(self.refresh_sono_N_frames_text)
-        self.slider_sono_N_frames.valueChanged.connect(self.calc_sono)
-        
-        self.input_sono_n_set = QLineEdit('0')
-        self.input_sono_n_set.setValidator(QIntValidator(0,1000))
-        self.input_sono_n_set.editingFinished.connect(self.calc_sono)
-        self.input_sono_n_chan = QLineEdit('0')
-        self.input_sono_n_chan.setValidator(QIntValidator(0,1000))
-        self.input_sono_n_chan.editingFinished.connect(self.calc_sono)
-        
-        self.input_db_range = QLineEdit('60')
-        self.input_db_range.setValidator(QIntValidator(1,200))
-        self.input_db_range.editingFinished.connect(self.calc_sono)
-        
-        self.sono_info = QLabel('')
-        
-        
-        self.button_calc_sono = BlueButton('Calc Sonogram')
-        self.button_calc_sono.clicked.connect(self.calc_sono)
-        
-        self.layout_tools_sonogram = QGridLayout()
-        self.layout_tools_sonogram.addWidget(boldLabel('Calculate Sonogram:'),0,0,1,4)
-        self.layout_tools_sonogram.addWidget(QLabel('N frames:'),1,0,1,2)
-        self.layout_tools_sonogram.addWidget(self.input_sono_N_frames,1,2,1,2)
-        self.layout_tools_sonogram.addWidget(self.slider_sono_N_frames,2,0,1,4)
-        self.layout_tools_sonogram.addWidget(self.sono_info,3,0,1,4)
-        self.layout_tools_sonogram.addWidget(QLabel('Dynamic Range (dB):'),4,0,1,2)
-        self.layout_tools_sonogram.addWidget(self.input_db_range,4,2,1,2)
-        self.layout_tools_sonogram.addWidget(QLabel('Set / Chan:'),5,0,1,2)
-        self.layout_tools_sonogram.addWidget(self.input_sono_n_set,5,2,1,1)
-        self.layout_tools_sonogram.addWidget(self.input_sono_n_chan,5,3,1,1)
-        self.layout_tools_sonogram.addWidget(self.button_calc_sono,6,0,1,4)
-        
-        self.frame_tools_sonogram = QFrame()
-        self.frame_tools_sonogram.setLayout(self.layout_tools_sonogram)
-        
-    def setup_frame_tools_save_export(self):
-        #self.button_import_matlab_jwlogger = BlueButton('Import from JW Logger')
-        #self.button_import_matlab_jwlogger.clicked.connect(self.import_jwlogger)
-        
-        self.button_export_matlab_jwlogger = BlueButton('Export to JW Logger')
-        self.button_export_matlab_jwlogger.clicked.connect(self.export_jwlogger)
-        
-        self.button_export_matlab = BlueButton('Export to Matlab')
-        self.button_export_matlab.clicked.connect(self.export_matlab)
-        
-        self.button_export_csv = BlueButton('Export to CSV')
-        self.button_export_csv.clicked.connect(self.export_csv)
-        
-        
-        self.layout_tools_save_export = QVBoxLayout()
-        #self.layout_tools_save_export.addWidget(self.button_import_matlab_jwlogger)
-        self.layout_tools_save_export.addWidget(self.button_export_matlab_jwlogger)
-        self.layout_tools_save_export.addWidget(self.button_export_matlab)
-        self.layout_tools_save_export.addWidget(self.button_export_csv)
-        
-        self.frame_tools_save_export = QFrame()
-        self.frame_tools_save_export.setLayout(self.layout_tools_save_export)
-        
-        
-    def update_frame_tools(self):
-        self.frame_tools.setLayout(self.layout_tools)
-
-
-    #%% INTERACTION FUNCTIONS
-    
-    def show(self):
-        # allow logger to be opened again after closing
-        # self.window.showMinimized()
-        self.window.show()
-        self.window.showNormal()
-        self.window.raise_()
-        
-        app.exec()
-        
-        
-    def close(self):
-        # allow logger to be closed programmatically
-        self.window.close()
-    
-    def start_stream(self):
-        if self.settings != None:
-            try:
-                streams.start_stream(self.settings)
-                self.rec = streams.REC
-            except:
-                self.rec = None
-                message = 'Data stream can\'t be initialised.\n'
-                message += 'Possible reasons: sounddevice or PyDAQmx not installed, or acquisition hardware not connected.\n' 
-                message += 'Please note that it won\'t be possible to log data.'
-                self.show_message(message)
-                
-        else:
-            message = 'To enable data acquisition, please use \'Logger Settings\' tool.'
-            self.show_message(message)
-#            self.input_list_tools.setCurrentIndex(1)
-            self.select_view()
-
-    def show_message(self,message,b='ok'):
-        # if multiple messages from different functions, then join them up
-        time_since_last = time.time()-self.message_time
-        if (time_since_last < 0.5) and (message not in self.message):# and (self.message not in message):
-            self.message += message # join messages if not duplicating
-        else:
-            self.message = message
-        self.message_time = time.time()
-        
-#        if (message not in self.message) and (self.message not in message):
-#            self.message += message # join messages if not duplicating
-#        else:
-#            self.message = message
-        if message != '':
-            self.label_message.setText(self.message)
-            if b == 'ok':
-                self.button_message.setVisible(True)
-                self.button_cancel.setVisible(False)
-                self.button_undo.setVisible(False)
-            elif b == 'cancel':
-                self.button_message.setVisible(False)
-                self.button_cancel.setVisible(True)
-                self.button_undo.setVisible(False)
-            elif b == 'undo':
-                self.button_message.setVisible(True)
-                self.button_cancel.setVisible(False)
-                self.button_undo.setVisible(True)
-                
-            self.frame_message.setVisible(True)
-        
-        
-    def hide_message(self):
-        self.label_message.setText('')
-        self.message = ''
-        modal.MESSAGE = ''
-        self.frame_message.setVisible(False)
-      
-    def show_message_timer(self):
-        message = acquisition.MESSAGE
-#        message += self.rec.MESSAGE
-        self.show_message(message,b='cancel')
-    
-    def check_stream(self):
-        if streams.REC is None:
-            self.levels_timer.stop()
-            self.window.setWindowTitle('Logger')
-        else:
-            self.levels_timer.start()
-    
-    def show_levels(self):
-        if streams.REC is not None:
-            max_levels = np.max(np.abs(self.rec.osc_time_data),axis=0)
-            ch_max = np.argmax(max_levels)
-            max_levels_all = max_levels[ch_max]
-            W = 20
-            N = int(np.round(max_levels_all*W))
-            display_text = N*'-' + '>|' + (W-N)*'-' + '] in ch ' + str(ch_max)
-            if max_levels_all > 0.99:
-                display_text += ' *** WARNING CLIPPED ***'
-                self.t0_clipped = time.time()
-            elif (max_levels_all < 0.99) and ((time.time()-self.t0_clipped) < 1):
-                display_text += ' *** WARNING CLIPPED ***'
-            
-                
-            self.window.setWindowTitle('Logger | Max Level: [' + display_text)
-        
-    
-    def button_clicked_osc(self):
-        # launch oscilloscope
-        self.osc = Oscilloscope(self.settings)
-
-
-    def button_clicked_log_data(self):
-        # delegate messages to acquisition global MESSAGE, and streams rec.MESSAGE
-        # this lets messages be seen from within logging thread, with live updates
-        self.message_timer.start(300) 
-        
-        # start stream
-        if self.rec is None:
-            self.start_stream()
-            
-        # generate output if specified
-        self.create_output_signal()
-        if self.output_time_data is not None:
-            y = self.output_time_data.time_data
-            # warn if amplitude set too high
-            if np.any(np.abs(y)>1):
-                message = 'Output amplitude too high: must be less than 1.\n'
-                self.show_message(message)
-                return None
-        else:
-            y = None
-
-        
-        
-        # reset trigger
-        self.rec.trigger_detected = False # but need to do this again inside acquisition
-        self.button_log_data.setStyleSheet("background-color: white")
-        
-#        # show message re trigger
-#        if self.settings.pretrig_samples is None:
-#            message = 'Logging data for {} seconds'.format(self.settings.stored_time)
-#        else:
-            #message = 'Logging data for {} seconds, with trigger.\n'.format(self.settings.stored_time)
-            
-            
-        
-        
-#        # show message re output
-#        if y is not None:
-#            message += '\n\nOutput signal starting.'
-#            self.show_message(message) # this one 
-        
-        
-        self.thread = LogDataThread(self.settings,test_name=self.test_name, rec=self.rec, output=y)
-        #self.thread.setPriority(QThread.TimeCriticalPriority)
-#        self.show_message(message,'cancel')
-        
-        self.thread.start()
-        self.thread.s.connect(self.add_logged_data)
-        
-        
-    def add_logged_data(self,d):
-        
-        if self.flag_log_and_replace == False:
-            self.dataset.add_to_dataset(d.time_data_list)
-            N = len(self.dataset.time_data_list)
-            self.sets = [N-1]
-            # this doesn't make it through from acquisition.MESSAGE because polling stops first
-            message = 'Logging complete.\n'
-            if np.any(np.abs(d.time_data_list[0].time_data) > 0.95):
-                message += '\nWARNING: Data may be clipped.\n'
-            self.show_message(message)
-#            message = ''
-#            self.hide_message()
-        else:
-            self.dataset.replace_data_item(d.time_data_list[0],self.selected_set)
-            self.sets = [self.selected_set]
-            self.last_action = 'data replaced'
-            # this doesn't make it through from acquisition.MESSAGE because polling stops first
-            message = 'Logged data replaced set {}.\n'.format(self.selected_set)
-            if np.any(np.abs(d.time_data_list[0].time_data) > 0.95):
-                message += '\nWARNING: Data may be clipped.\n'
-            self.show_message(message,b='undo')
-            self.flag_log_and_replace = False
-
-        
-        # update figure then update selection
-        self.channels = 'all'
-        self.switch_view('Time Data') # need to switch to time and update plot so that get_selected_chans picks up new data
-        
-        # only show most recently logged data
-        selection = self.p.get_selected_channels()
-        for ns in range(len(selection)):
-            for nc in range(len(selection[ns])):
-                if ns in self.sets:
-                    selection[ns][nc] = True
-                else:
-                    selection[ns][nc] = False
-        self.selected_channels = selection
-        
-        # update with final selection and make -1 to 1, change button back to green
-        self.auto_xy = 'x'
-        self.update_figure()
-        self.p.ax.set_ylim([-1,1])
-        self.button_log_data.setStyleSheet('background-color: hsv(120, 170, 255)')
-        self.message_timer.stop()
-        
-        
-    def cancel_logging(self):
-        self.thread.terminate() # stop thread
-        streams.start_stream(self.settings) # reset stream
-        self.rec = streams.REC # reset stream
-        self.show_message('Logging cancelled')
-        self.button_log_data.setStyleSheet('background-color: hsv(120, 170, 255)')
-        self.message_timer.stop() # stop acquisition messages
-        self.selected_channels = self.p.get_selected_channels()
-
-    def delete_last_data(self):
-        self.dataset_backup = copy.deepcopy(self.dataset)
-        self.dataset.remove_last_data_item('TimeData')
-        self.dataset.freq_data_list = datastructure.FreqDataList()
-        self.dataset.tf_data_list = datastructure.TfDataList()
-        N = len(self.dataset.time_data_list)
-        self.sets = [N-1]
-        self.channels = 'all'
-        
-        # only show most recently logged data
-        if N > 0:
-            selection = self.p.get_selected_channels()
-            for ns in range(len(selection)):
-                for nc in range(len(selection[ns])):
-                    if ns in self.sets:
-                        selection[ns][nc] = True
-                    else:
-                        selection[ns][nc] = False
-            self.selected_channels = selection
-        
-        self.auto_xy = 'x'
-        self.update_figure()
-        self.p.ax.set_ylim([-1,1])
-#        self.auto_xy = ''
-#        self.p.update(self.dataset.time_data_list,sets=[N-1],channels='all', auto_xy=self.auto_xy)
-#        update(self,data_list,sets='all',channels='all',xlinlog='linear',show_coherence=True,plot_type=None,coherence_plot_type='linear',freq_range=None, auto_xy='xyc'):
-        self.switch_view('Time Data')
-        self.last_action = 'delete data'
-        message = 'Last logged time data deleted.\n'
-        message += 'FFT and TF data also deleted.\n'
-        message += 'For more data editing options select ''Edit Dataset'' tool.'
-        self.show_message(message,b='undo')
-#        self.selected_channels = self.p.get_selected_channels()
-#        self.update_selected_set()
-        
-    def reset_data(self):
-        self.dataset_backup = copy.deepcopy(self.dataset)
-        self.dataset = datastructure.DataSet()
-        N = len(self.dataset.time_data_list)
-        self.p.update(self.dataset.time_data_list,sets=[N-1],channels='all')
-        self.switch_view('Time Data')
-        self.last_action = 'delete data'
-        message = 'All data deleted.\n'
-        message += 'For more data editing options select ''Edit Dataset'' tool.'
-        self.show_message(message,b='undo')
-#        self.selected_channels = self.p.get_selected_channels()
-#        self.update_selected_set()
-
-    
-    def load_data(self):
-        
-        d = file.load_data(parent=self.window)
-        
-        if d is not None:
-            d = datastructure.update_dataset(d) # updates data saved using previous logger versions
-            self.dataset.add_to_dataset(d.time_data_list)
-            self.dataset.add_to_dataset(d.freq_data_list)
-            self.dataset.add_to_dataset(d.tf_data_list)
-            self.dataset.add_to_dataset(d.cross_spec_data_list)
-            self.dataset.add_to_dataset(d.sono_data_list)
-            self.dataset.add_to_dataset(d.meta_data_list)
-            self.dataset.add_to_dataset(d.modal_data_list)
-            
-        else:
-            message = 'No data loaded'
-            self.show_message(message)
-            return None
-    
-        
-        no_data = True
-        self.auto_xy = 'xyc'
-        if len(d.time_data_list) != 0:
-            self.input_list_figures.setCurrentText('Time Data')
-            self.select_view()
-#            self.hide_message()
-            no_data = False
-        if len(d.freq_data_list) != 0:
-            self.input_list_figures.setCurrentText('FFT Data')
-            self.select_view()
-#            self.hide_message()
-            no_data = False
-        if len(d.tf_data_list) != 0:
-            self.input_list_figures.setCurrentText('TF Data')
-            self.select_view()
-#            self.hide_message()
-            no_data = False
-        if no_data == True:
-            message = 'No data to view'
-            self.show_message(message)
-        self.input_list_data_type.setCurrentText(self.selected_view)
-        self.select_all_data()
-        self.selected_channels = self.p.get_selected_channels()
-#        self.update_selected_set()
-        
-        
-        
-            
-    def save_data(self):
-        filename = self.dataset.save_data()
-        if filename is not None:
-            message = 'Saved dataset:\n\n'
-            message += self.dataset.__repr__()
-            message += '\n\n'
-            message += 'to file '
-            message += filename
-        else:
-            message = 'Save dataset cancelled'
-        self.show_message(message)
-            
-    def save_fig(self):
-        if self.plot_type == 'Nyquist':
-            filename = file.save_fig(self.p,figsize=(9,9))
-        else:
-            filename = file.save_fig(self.p,figsize=(9,5))
-        if filename is not None:
-            message = 'Saved current figure to file:\n'
-            message += filename
-        else:
-            message = 'Save figure cancelled'
-        self.canvas.draw()
-        self.show_message(message)
-
-    def xmin(self):
-        xmin = float(self.input_axes[0].text())
-        xlim = self.p.ax.get_xlim()
-        self.p.ax.set_xlim([xmin,xlim[1]])
-        if ((self.current_view == 'TF Data') or (self.current_view == 'FFT Data')) and (self.plot_type != 'Nyquist'):
-            self.freq_range = list(self.p.ax.get_xlim())
-        self.canvas.draw()
-        
-    def xmax(self):
-        xmax = float(self.input_axes[1].text())
-        xlim = self.p.ax.get_xlim()
-        self.p.ax.set_xlim([xlim[0],xmax])
-        if ((self.current_view == 'TF Data') or (self.current_view == 'FFT Data')) and (self.plot_type != 'Nyquist'):
-            self.freq_range = list(self.p.ax.get_xlim())
-        self.canvas.draw()
-        
-    def ymin(self):
-        ymin = float(self.input_axes[2].text())
-        ylim = self.p.ax.get_ylim()
-        self.p.ax.set_ylim([ymin,ylim[1]])
-        self.canvas.draw()
-        
-    def ymax(self):
-        ymax = float(self.input_axes[3].text())
-        ylim = self.p.ax.get_ylim()
-        self.p.ax.set_ylim([ylim[0],ymax])
-        self.canvas.draw()
-        
-    def auto_x(self):
-#        self.auto_xy = 'x'
-#        self.update_figure()
-        self.p.auto_x()
-        
-    def auto_y(self):
-#        self.auto_xy = 'yc'
-#        self.update_figure()
-        self.p.auto_y()
-        
-    def update_axes_values(self,axes):
-#        self.selected_channels = self.p.get_selected_channels()
-        
-        xlim = self.p.ax.get_xlim()
-        ylim = self.p.ax.get_ylim()
-        self.input_axes[0].setText('{:0.5g}'.format(xlim[0]))
-        self.input_axes[1].setText('{:0.5g}'.format(xlim[1]))
-        self.input_axes[2].setText('{:0.5g}'.format(ylim[0]))
-        self.input_axes[3].setText('{:0.5g}'.format(ylim[1]))
-        if ((self.current_view == 'TF Data') or (self.current_view == 'FFT Data')) and (self.plot_type != 'Nyquist'):
-            self.freq_range = list(xlim)
-            self.input_freq_min2.setText('{:0.5g}'.format(xlim[0]))
-            self.input_freq_max2.setText('{:0.5g}'.format(xlim[1]))
-        
-                
-    def update_modal_message(self,axes):
-        # only connected to x-axis
-        if (self.current_view == 'TF Data') and (len(self.dataset.modal_data_list) > 0) and (self.selected_tool == 'Mode Fitting') and (modal.MESSAGE == ''):
-            # Show message to highlight modal fit, to allow removing or replacing a given fit
-            fn_all = self.dataset.modal_data_list[0].M[:,0]
-            self.fn_in_range = fn_all[(fn_all > self.freq_range[0]) & (fn_all < self.freq_range[1])]
-            if len(self.fn_in_range) > 1:
-                message = 'A total of {} modes have been fitted within this frequency range so far:\n\n'.format(len(self.fn_in_range))
-                message += 'Fitted mode frequencies = {} (Hz)\n\n'.format(np.array2string(self.fn_in_range,precision=2))
-                message += 'To delete all of these modal fits, press ''Reject Mode''.'
-                self.show_message(message)
-            elif len(self.fn_in_range) == 1:
-                message = 'One mode has been fitted within this frequency range:\n\n'
-                message += 'Fitted mode frequency = {} Hz\n\n'.format(np.array2string(self.fn_in_range,precision=2))
-                message += 'To replace this mode fit with a new fit, press ''Fit Mode''.\n'
-                message += 'To delete this mode fit, press ''Reject Mode''.'
-                self.show_message(message)
-            else:
-                self.hide_message()
-        
-    def legend_left(self):
-        self.legend_loc = 'lower left'
-        self.p.update_legend(self.legend_loc)
-        self.canvas.draw()
-        
-    def legend_right(self):
-        self.legend_loc = 'lower right'
-        self.p.update_legend(self.legend_loc)
-        self.canvas.draw()
-            
-    def legend_onoff(self):
-        self.selected_channels = self.p.get_selected_channels()
-        visibility = self.p.ax.get_legend().get_visible()
-        self.p.ax.get_legend().set_visible(not visibility)
-        self.canvas.draw()
-        
-        
-    def update_figure(self):
-        # get current status of axes for case auto_xy=''
-        xlim = self.p.ax.get_xlim()
-        ylim = self.p.ax.get_ylim()
-            
-        try:
-            # sometimes starting point with no legend object
-            visibility = self.p.ax.get_legend().get_visible()
-        except:
-            pass
-        # updates the currently viewed plot
-        if self.current_view == 'Time Data':
-            data_list = self.dataset.time_data_list
-        elif self.current_view == 'FFT Data':
-            data_list = self.dataset.freq_data_list
-        elif self.current_view == 'TF Data':
-            data_list = self.dataset.tf_data_list
-        elif self.current_view == 'Sono Data':
-            data_list = self.dataset.sono_data_list
-            
-        if self.current_view == 'Sono Data':
-            if self.current_view_changed == True:
-                auto_xy = 'xy'
-            else:
-                auto_xy=''
-                
-            n_set = int(self.input_sono_n_set.text())
-            n_chan = int(self.input_sono_n_chan.text())
-            db_range = int(self.input_db_range.text())
-            self.p.update_sonogram(self.dataset.sono_data_list, n_set, n_chan, db_range=db_range,auto_xy=auto_xy)
-            self.label_figure.setText(self.selected_view + ': Set {}, Channel {}'.format(n_set,n_chan))
-        else:
-            self.p.update(data_list, sets=self.sets, channels=self.channels, xlinlog=self.xlinlog,show_coherence=self.show_coherence,plot_type=self.plot_type,coherence_plot_type=self.coherence_plot_type,freq_range=self.freq_range,auto_xy=self.auto_xy)
-            self.label_figure.setText(self.selected_view)
-        if self.current_view_changed == False:
-            try:
-                # not robust as not consistent in keeping up to date
-                # if only one data set then make sure it's visible
-                if len(data_list) == 1:
-                    selection = self.p.get_selected_channels()
-                    for nc in range(len(selection[0])):
-                        selection[0][nc] = True
-                    self.selected_channels = selection
-                # otherwise just inherit prev data selection
-                self.p.set_selected_channels(self.selected_channels)
-                self.p.ax.get_legend().set_visible(visibility)
-                self.fig.canvas.draw()
-            except:
-                # get selected_channels back into sync
-                pass# not sure helping. self.selected_channels = self.p.get_selected_channels()
-        if self.auto_xy=='':
-            # handle this case manually
-            self.p.ax.set_xlim(xlim)
-            self.p.ax.set_ylim(ylim)
-            self.p.fig.canvas.draw()
-
-        self.selected_channels = self.p.get_selected_channels()
-                   
-    def update_selected_channels(self,_):
-        # keeps selected_channels in sync with legend picking
-        self.selected_channels = self.p.get_selected_channels()
-        
-    def select_all_data(self):
-        if len(self.p.ax.lines) > 0:
-            for line in self.p.ax.lines:
-                line.set_alpha(plotting.LINE_ALPHA)
-            for line in self.p.legend.get_lines():
-                line.set_alpha(plotting.LINE_ALPHA)
-            self.canvas.draw()
-        else:
-            message = 'No data to show.\n'
-            self.show_message(message)
-        self.selected_channels = self.p.get_selected_channels()
-        
-        
-        
-    def select_no_data(self):
-        if len(self.p.ax.lines) > 0:
-            for line in self.p.ax.lines:
-                line.set_alpha(1-plotting.LINE_ALPHA)
-            for line in self.p.legend.get_lines():
-                line.set_alpha(1-plotting.LINE_ALPHA)
-            self.canvas.draw()
-        else:
-            message = 'No data to hide.\n'
-            self.show_message(message)
-        self.selected_channels = self.p.get_selected_channels()
-            
-    def show_set_only(self):
-        n_set = int(self.input_select_set_only.text())
-        selection = self.p.get_selected_channels()
-        for ns in range(len(selection)):
-            for nc in range(len(selection[ns])):
-                if ns == n_set:
-                    selection[ns][nc] = True
-                else:
-                    selection[ns][nc] = False
-        self.p.set_selected_channels(selection)
-        self.selected_channels = selection
-        
-    def show_chan_only(self):
-        n_chan = int(self.input_select_chan_only.text())
-        selection = self.p.get_selected_channels()
-        for ns in range(len(selection)):
-            for nc in range(len(selection[ns])):
-                if nc == n_chan:
-                    selection[ns][nc] = True
-                else:
-                    selection[ns][nc] = False
-        self.p.set_selected_channels(selection)
-        self.selected_channels = selection
-        
-    def next_chans(self):
-        try:
-            # sometimes starting point with no legend object
-            visibility = self.p.ax.get_legend().get_visible()
-        except:
-            pass
-        
-        selection = self.p.get_selected_channels()
-        prev_line = bool(selection[-1][-1])
-        for ns in range(len(selection)):
-            for nc in range(len(selection[ns])):
-                this_line = bool(selection[ns][nc])
-                selection[ns][nc] = bool(prev_line)
-                prev_line = bool(this_line)
-        
-        self.p.set_selected_channels(selection)
-        self.selected_channels = selection
-        try:
-            self.p.ax.get_legend().set_visible(visibility)
-            self.fig.canvas.draw()
-        except:
-            pass
-        
-    def prev_chans(self):
-        try:
-            # sometimes starting point with no legend object
-            visibility = self.p.ax.get_legend().get_visible()
-        except:
-            pass
-        selection = self.p.get_selected_channels()
-        prev_line = bool(selection[0][0])
-        for ns in reversed(range(len(selection))):
-            for nc in reversed(range(len(selection[ns]))):
-                this_line = bool(selection[ns][nc])
-                selection[ns][nc] = bool(prev_line)
-                prev_line = bool(this_line)
-        
-        self.p.set_selected_channels(selection) 
-        self.selected_channels = selection
-        try:
-            self.p.ax.get_legend().set_visible(visibility)
-            self.fig.canvas.draw()
-        except:
-            pass
-
-           
-        
-    def co_min(self):
-        co_min = float(self.input_co_min.text())
-        ylim = self.p.ax2.get_ylim()
-        self.p.ax2.set_ylim([co_min,ylim[1]])
-        self.canvas.draw()
-    
-    def co_max(self):
-        co_max = float(self.input_co_max.text())
-        ylim = self.p.ax2.get_ylim()
-        self.p.ax2.set_ylim([ylim[0],co_max])
-        self.canvas.draw()
-        
-    def freq_min(self):
-        self.freq_range[0] = float(self.input_freq_min.text())
-        self.input_freq_min2.setText(str(self.freq_range[0]))
-        self.update_figure()
-#        self.p.update(self.dataset.tf_data_list, xlinlog=self.xlinlog, show_coherence=self.show_coherence,plot_type=self.plot_type,coherence_plot_type=self.coherence_plot_type,freq_range=self.freq_range,auto_xy=self.auto_xy)
-        
-    def freq_max(self):
-        self.freq_range[1] = float(self.input_freq_max.text())
-        self.input_freq_max2.setText(str(self.freq_range[1]))
-        self.update_figure()
-#        self.p.update(self.dataset.tf_data_list, xlinlog=self.xlinlog, show_coherence=self.show_coherence,plot_type=self.plot_type,coherence_plot_type=self.coherence_plot_type,freq_range=self.freq_range,auto_xy=self.auto_xy)
-        
-    def update_co_axes_values(self,axes):
-        ylim = self.p.ax2.get_ylim()
-        self.input_co_min.setText('{:0.5g}'.format(ylim[0]))
-        self.input_co_max.setText('{:0.5g}'.format(ylim[1]))
-        
-    def data_toggle(self):
-        self.show_data = not self.show_data
-        self.select_view()
-        for line in self.p.ax.lines:
-            line.set_visible(self.show_data)
-        if self.show_data == False:
-            self.p.ax.set_ylabel('')
-            self.p.ax.set_yticks([])
-        else:
-            self.p.ax.yaxis.set_major_locator(AutoLocator())
-            
-        self.canvas.draw()
-
-    def coherence_toggle(self):
-        self.show_coherence = not self.show_coherence
-        self.select_view()
-                
-        
-    def select_xlinlog(self):
-        if self.xlinlog == 'linear':
-            self.xlinlog = 'log' # or symlog
-        else:
-            self.xlinlog = 'linear'
-        
-        self.update_figure()
-    
-    def switch_view(self,new_view_text):
-        index = self.input_list_figures.findText(new_view_text, Qt.MatchFlag.MatchFixedString)
-        if self.input_list_figures.itemText(index) == 'Time Data':
-            N = len(self.dataset.time_data_list)
-        elif self.input_list_figures.itemText(index) == 'FFT Data':
-            N = len(self.dataset.freq_data_list)
-        elif self.input_list_figures.itemText(index) == 'TF Data':
-            N = len(self.dataset.tf_data_list)
-        elif self.input_list_figures.itemText(index) == 'Sono Data':
-            N = len(self.dataset.sono_data_list)
-        if N > 0:
-            self.input_list_figures.setCurrentIndex(index)
-            self.input_list_data_type.setCurrentText(self.input_list_figures.currentText())
-            
-        self.select_view()
-        
-    def select_view(self):
-        # handles logic of what to show in gui depending on selected view options
-        ci = self.input_list_figures.currentIndex()
-        self.selected_view = self.input_list_figures.itemText(ci)
-        
-        if self.current_view == self.selected_view:
-            self.current_view = np.copy(self.selected_view)
-            self.current_view_changed = False
-            self.plot_type_before = np.copy(self.plot_type)
-            self.plot_type = self.items_list_plot_type[self.input_list_plot_type.currentIndex()]
-            self.switch_to_nyquist = (self.plot_type == 'Nyquist') and ('Nyquist' != self.plot_type_before)
-            self.switch_from_nyquist = (self.plot_type_before == 'Nyquist') and ('Nyquist' != self.plot_type)
-#            self.selected_channels = self.p.get_selected_channels()
-        else:
-            self.current_view_changed = True
-        
-        # Time Data
-        if self.selected_view == 'Time Data':
-            ### set to time gui
-            N = len(self.dataset.time_data_list)
-            # check if any data present to display
-            if N != 0:
-                # no plot details needed for time display
-                self.hide_plot_details()
-                # reset data/coherence plot properties if changed view back to time
-                if self.current_view_changed:
-                    self.current_view = self.selected_view
-                    self.show_data = True
-                    self.show_coherence = True # won't plot but reests for other selections
-                    self.xlinlog = 'linear'
-                    self.auto_xy = 'xyc'
-                    self.plot_type = 'Amplitude (dB)'# - can trigger this to be called again
-                    self.input_list_plot_type.setCurrentText(self.plot_type)
-                else:
-                    self.auto_xy = ''
-                    
-                # plot
-                self.update_figure()
-                
-            # show message if no data
-            else:
-                message = 'No time data to display.\n'
-                self.show_message(message)
-                
-        # FFT Data
-        elif self.selected_view == 'FFT Data':
-            N = len(self.dataset.freq_data_list)
-            # check if freq data exists
-            if N != 0:
-                # if main view changed reset plot properties
-                if self.current_view_changed:
-                    self.current_view = self.selected_view
-                    self.show_data = True
-                    self.show_coherence = True # won't plot but reests for other selections
-                    self.auto_xy = 'xyc'
-                    self.plot_type = 'Amplitude (dB)'
-                    self.input_list_plot_type.setCurrentText(self.plot_type)
-                    
-                
-                # if staying as FFT plot but changing to nyquist then switch to FFT Nyquist toolset
-                elif self.switch_to_nyquist == True:
-                    # get properties before switch so can go back to this view
-                    self.freq_range = list(self.p.ax.get_xlim()) #force to list instead of tuple
-                    self.show_coherence_before = self.show_coherence
-                    self.show_coherence = False
-                    self.xlinlog_before = self.xlinlog
-                    # linear x axis for nyquist
-                    self.xlinlog = 'linear'
-                    # update freq range text
-                    self.input_freq_min.setText('{:5f}'.format(self.freq_range[0]))
-                    self.input_freq_max.setText('{:5f}'.format(self.freq_range[1]))
-                    self.auto_xy = 'xy'
-                    
-                    
-                # if moving from nyquist back, reset properties to previous
-                elif self.switch_from_nyquist == True:
-                    self.show_coherence = self.show_coherence_before
-                    self.xlinlog = self.xlinlog_before
-                    # freq range already set above as must have moved to nyquist first
-                    self.auto_xy = 'fy'
-                    
-                else:
-                    # update freq range if switching plot other than to/from nyquist
-                    self.freq_range = list(self.p.ax.get_xlim()) # force to list instead of tuple
-                    self.auto_xy = 'fy'
-                    
-                    
-                # always reset figure heading
-                self.label_figure.setText(self.selected_view)
-                                
-                # set gui to correct toolset
-                if self.plot_type == 'Nyquist':
-                    #self.auto_xy = 'xy'
-                    self.show_plot_details_with_nqyuist()
-                else:
-                    self.show_plot_details_basic()
-                    
-                self.update_figure()
-
-                
-            # show message if no data to plot
-            else:
-                message = 'No FFT data to display.\n'
-                self.show_message(message)
-        
-        # TF Data
-        elif self.selected_view == 'TF Data':
-            N = len(self.dataset.tf_data_list)
-            # check if data to plot
-            if N != 0:
-                # if main view changed reset plot properties
-                if self.current_view_changed:
-                    self.current_view = self.selected_view
-                    self.show_data = True
-                    self.show_coherence = True 
-                    self.auto_xy = 'xyc'
-                    self.plot_type = 'Amplitude (dB)'
-                    self.input_list_plot_type.setCurrentText(self.plot_type)
-                
-                # if staying as TF plot but changing to nyquist then switch to TF Nyquist toolset
-                elif self.switch_to_nyquist == True:
-                    # get properties before switch so can go back to this view
-                    self.freq_range = list(self.p.ax.get_xlim()) #force to list instead of tuple
-                    self.show_coherence_before = self.show_coherence
-                    self.show_coherence = False
-                    self.xlinlog_before = self.xlinlog
-                    # linear x axis for nyquist
-                    self.xlinlog = 'linear'
-                    # update freq range text
-                    self.input_freq_min.setText('{:0.5g}'.format(self.freq_range[0]))
-                    self.input_freq_max.setText('{:0.5g}'.format(self.freq_range[1]))
-                    self.auto_xy = 'xy'
-                
-                # if moving from nyquist back, reset properties to previous
-                elif self.switch_from_nyquist == True:
-                    self.show_coherence = self.show_coherence_before
-                    self.xlinlog = self.xlinlog_before
-                    self.auto_xy = 'fy'
-                    # freq range already set above as must have moved to nyquist first
-            
-                else:
-                    # update freq range if switching plot other than to/from nyquist
-                    self.freq_range = list(self.p.ax.get_xlim()) # force to list instead of tuple
-                    self.auto_xy = 'fy'
-
-                # plot now then auto-x/y according to nyquist or not
-                self.update_figure()
-
-                    
-                # set gui to correct toolset
-                self.label_figure.setText(self.selected_view)
-                if self.plot_type == 'Nyquist':
-                    self.show_plot_details_with_nqyuist()
-                else:
-                    self.show_plot_details_with_coherence()
-                    
-            # show message if no data
-            else:
-                message = 'No transfer function data to display.\n'
-                self.show_message(message)
-            
-        elif self.selected_view == 'Sono Data':
-             ### set to time gui
-            N = len(self.dataset.sono_data_list)
-            # check if any data present to display
-            if N != 0:
-                # no plot details needed for sonogram display
-                self.hide_plot_details()
-                # reset data/coherence plot properties if changed view back to time
-                if self.current_view_changed:
-                    self.current_view = self.selected_view
-                    self.show_data = True
-                    self.show_coherence = True # won't plot but reests for other selections
-                    self.xlinlog = 'linear'
-                    self.auto_xy = 'xyc'
-                    self.plot_type = 'Amplitude (dB)'
-                    self.input_list_plot_type.setCurrentText(self.plot_type)
-                else:
-                    self.auto_xy = ''
-                    
-                # plot
-                self.update_figure()
-                
-            # show message if no data
-            else:
-                message = 'No sonogram data to display.\n'
-                self.show_message(message)
-            
-            
-        
-    def hide_plot_details(self):
-        self.frame_plot_details.setVisible(False)
-        
-    def show_plot_details_with_coherence(self):
-        # Put Falses before Trues
-        self.input_freq_min.setVisible(False)
-        self.input_freq_max.setVisible(False)        
-
-        self.button_xlinlog.setVisible(True)
-        self.button_data_toggle.setVisible(True)
-        self.button_coherence_toggle.setVisible(True)
-        self.label_co_freq_min.setVisible(True)
-        self.label_co_freq_max.setVisible(True)
-        self.label_co_freq_min.setText('co. min:')
-        self.label_co_freq_max.setText('co. max:')
-        
-        self.input_co_min.setVisible(True)
-        self.input_co_max.setVisible(True)
-        
-        self.frame_plot_details.setVisible(True)
-        
-        
-    def show_plot_details_with_nqyuist(self):
-        # Put Falses before Trues
-        self.button_xlinlog.setVisible(False)
-        self.button_data_toggle.setVisible(False)
-        self.button_coherence_toggle.setVisible(False)
-        self.input_co_min.setVisible(False)
-        self.input_co_max.setVisible(False)
-        
-        self.label_co_freq_min.setVisible(True)
-        self.label_co_freq_max.setVisible(True)
-        self.label_co_freq_min.setText('freq. min:')
-        self.label_co_freq_max.setText('freq. max:')
-        
-        self.input_freq_min.setVisible(True)
-        self.input_freq_max.setVisible(True)
-
-        self.frame_plot_details.setVisible(True)
-        
-        
-    def show_plot_details_basic(self):
-        # put Falses before Trues
-        self.button_data_toggle.setVisible(False)
-        self.button_coherence_toggle.setVisible(False)
-        self.label_co_freq_min.setVisible(False)
-        self.label_co_freq_max.setVisible(False)
-        
-        self.input_co_min.setVisible(False)
-        self.input_co_max.setVisible(False)
-        self.input_freq_min.setVisible(False)
-        self.input_freq_max.setVisible(False)
-        
-        self.button_xlinlog.setVisible(True)
-        self.frame_plot_details.setVisible(True)
-        
-    def hide_all_tools(self):
-        self.frame_tools_time_domain.setVisible(False)
-        self.frame_tools_fft.setVisible(False)
-        self.frame_tools_tf.setVisible(False)
-        self.frame_tools_scaling.setVisible(False)
-        self.frame_tools_mode_fitting.setVisible(False)
-        self.frame_tools_settings.setVisible(False)
-        self.frame_tools_generate_output.setVisible(False)
-        self.frame_tools_edit_dataset.setVisible(False)
-        self.frame_tools_sonogram.setVisible(False)
-        self.frame_tools_save_export.setVisible(False)
-        
-    def select_tool(self):
-        self.selected_tool = self.input_list_tools.currentText()
-        if self.selected_tool == 'Standard Tools':
-            self.hide_all_tools()
-            self.frame_tools_time_domain.setVisible(True)
-            self.frame_tools_fft.setVisible(True)
-            self.frame_tools_tf.setVisible(True)
-            self.frame_tools_scaling.setVisible(True)
-            
-            
-        elif self.selected_tool == 'Logger Settings':
-            self.hide_all_tools()
-            self.frame_tools_settings.setVisible(True)
-            
-        elif self.selected_tool == 'Generate Output':
-            self.hide_all_tools()
-            self.frame_tools_generate_output.setVisible(True)
-            
-        elif self.selected_tool == 'Pre-process':
-            self.hide_all_tools()
-            self.frame_tools_time_domain.setVisible(True)
-            
-        elif self.selected_tool == 'FFT':
-            self.hide_all_tools()
-            self.frame_tools_fft.setVisible(True)
-            
-        elif self.selected_tool == 'Transfer Function':
-            self.hide_all_tools()
-            self.frame_tools_tf.setVisible(True)
-            
-        elif self.selected_tool == 'Calibration / Scaling':
-            self.hide_all_tools()
-            self.frame_tools_scaling.setVisible(True)
-            
-        elif self.selected_tool == 'Sonogram':
-            self.hide_all_tools()
-            self.frame_tools_sonogram.setVisible(True)
-            
-        elif self.selected_tool == 'Mode Fitting':
-            self.hide_all_tools()
-            self.frame_tools_mode_fitting.setVisible(True)
-            
-        elif self.selected_tool == 'Edit Dataset':
-            self.hide_all_tools()
-            self.auto_xy = ''
-            self.update_selected_set()
-            self.frame_tools_edit_dataset.setVisible(True)
-
-            
-        elif self.selected_tool == 'Save / Export':
-            self.hide_all_tools()
-            self.frame_tools_save_export.setVisible(True)
-            
-    def apply_settings(self):
-        settings_dict = dict()
-        for n_row in range(14):
-            label = self.labels_settings[n_row]
-            text = self.input_settings[label].text()
-            settings_dict[label] = text
-        self.settings_dict = settings_dict
-        self.settings = options.MySettings(**settings_dict)
-        self.test_name = self.input_test_name.text()
-        if self.test_name == '':
-            self.test_name = None
-        self.start_stream()
-            
-    
-    def show_available_devices(self):
-        message = streams.list_available_devices()
-        self.show_message(message)
-
-    def update_selected_set(self):
-        # this function is related to edit_dataset tool, not selecting channels
-        data_type = self.input_list_data_type.currentText()
-        if data_type == 'Time Data':
-            self.data_list = self.dataset.time_data_list
-            self.switch_view(data_type)
-        elif data_type == 'FFT Data':
-            self.data_list = self.dataset.freq_data_list
-            self.switch_view(data_type)
-        elif data_type == 'TF Data':
-            self.data_list = self.dataset.tf_data_list
-            self.switch_view(data_type)
-        elif data_type == 'Modal Data':
-            self.data_list = self.dataset.modal_data_list
-        elif data_type == 'Sono Data':
-            self.data_list = self.dataset.sono_data_list
-        else:
-            self.data_list = []
-        
-        self.update_data_summary()
-        
-    def update_data_summary(self):
-        # also keeps validator up to date
-        N = len(self.data_list)
-        self.input_selected_set.setValidator(QIntValidator(0,N-1))
-        text = self.dataset.__repr__()
-        self.label_data_summary.setText(text)
-
-    def delete_data_type(self):
-        self.auto_xy = ''
-        self.update_selected_set()
-        if len(self.data_list) != 0:
-            self.dataset_backup = copy.deepcopy(self.dataset)
-            self.data_type = self.data_list[0].__class__.__name__
-            self.dataset.remove_data_item_by_index(self.data_type,np.arange(len(self.data_list)))
-            self.last_action = 'delete data'
-            message = 'All {} items deleted.\n\n'.format(self.data_type)
-            self.show_message(message, b='undo')
-        else:
-            message = 'No {} to delete.'.format(self.data_typye)
-            self.show_message(message)
-        self.update_selected_set()
-            
-    
-    def delete_data_set(self):
-        self.auto_xy = ''
-        self.selected_set = int(self.input_selected_set.text())
-        if len(self.data_list) != 0:
-            self.dataset_backup = copy.deepcopy(self.dataset)
-            self.data_type = self.data_list[0].__class__.__name__
-            self.dataset.remove_data_item_by_index(self.data_type,self.selected_set)
-            self.last_action = 'delete data'
-            message = 'Set {} of type {} deleted.'.format(self.selected_set,self.data_type)
-            self.show_message(message, b='undo')
-        else:
-            message = 'No {} to delete.'.format(self.data_typye)
-            self.show_message(message)
-        self.update_selected_set()
-    
-    def log_and_replace(self):
-        self.auto_xy = ''
-        self.dataset_backup = copy.deepcopy(self.dataset)
-        self.selected_set = int(self.input_selected_set.text())
-        self.flag_log_and_replace = True
-        self.button_clicked_log_data()
-        
-#        ### DUPLICATES button_clicked_log_data FUNCTION SO THAT MESSAGE APPEARS ###
-#        if self.rec is None:
-#            self.start_stream()
-#        self.rec.trigger_detected = False
-#        self.button_log_data.setStyleSheet("background-color: white")
-#        if self.settings.pretrig_samples is None:
-#            message = 'Logging data for {} seconds'.format(self.settings.stored_time)
-#        else:
-#            message = 'Logging data for {} seconds, with trigger'.format(self.settings.stored_time)
-#        self.thread = LogDataThread(self.settings,test_name=self.test_name, rec=self.rec)
-#        self.show_message(message,'cancel')
-#        self.thread.start()
-#        self.thread.s.connect(self.add_logged_data)
-        ###########################################################################
-    
-    def update_output(self):
-        sig = self.input_output_options.currentText()
-        if sig == 'None':
-            self.flag_output = False
-        else:
-            self.flag_output = True
-            
-    def create_output_signal(self):
-        sig = self.input_output_options.currentText()
-        T = float(self.input_output_duration.text())
-        amp = float(self.input_output_amp.text())
-        f1 = float(self.input_output_f1.text())
-        f2 = float(self.input_output_f2.text())
-        f_max = np.max([f1,f2])
-        fs_min = np.min([self.settings.fs,self.settings.output_fs])
-            
-        if sig != 'None':
-            if f_max > fs_min/2:
-                message = 'Highest output frequency {} Hz exceeds input or output sampling frequency {} Hz.'.format(f_max,fs_min)
-                self.show_message(message)
-                td = None
-            else:
-                t,y = acquisition.signal_generator(self.settings,sig=sig,T=T,amplitude=amp,f=[f1,f2],selected_channels='all')
-                td = datastructure.TimeData(t,y,self.settings,test_name='output_signal')
-                message = acquisition.MESSAGE
-                self.show_message(message)
-        else:
-            td = None
-#            message = 'Output signal turned off.'
-#            self.show_message(message)         
-        self.output_time_data = td
-            
-    def preview_output(self):
-        self.create_output_signal()
-        if self.output_time_data != None:
-            d = datastructure.DataSet(self.output_time_data)
-            d.calculate_fft_set()
-            self.preview_window = PreviewWindow(title='Time Data')
-            self.preview_window.p.update(d.time_data_list,auto_xy='xy')
-            self.preview_window2 = PreviewWindow(title='FFT Data')
-            self.preview_window2.p.update(d.freq_data_list, xlinlog='log',auto_xy='xy')
-    
-    def start_output(self):
-        self.create_output_signal()
-        if self.output_time_data != None:
-            s = acquisition.output_signal(self.settings,self.output_time_data.time_data)
-        else:
-            message = 'No output data to generate.'
-            self.show_message(message)
-            
-
-    #%% DATA PROCESSING
-    def clean_impulse(self):
-        try:
-            ch_impulse = int(self.input_impulse_channel.text())
-            
-            dataset_new = self.dataset.clean_impulse(ch_impulse=ch_impulse)
-            
-            if 'data already cleaned' not in analysis.MESSAGE:
-                # only make backup if first time cleaned, otherwise backup no longer contains original data
-                # not watertight logic if cleaned some but not all channels before
-                # needs updating
-                self.dataset_backup = self.dataset
-            self.dataset = dataset_new
-            self.show_message(analysis.MESSAGE,b='undo')
-            self.last_action = 'clean_impulse'
-            self.auto_xy = ''
-            selection = self.p.get_selected_channels()
-            self.update_figure()
-            self.p.set_selected_channels(selection)
-        except:
-            analysis.MESSAGE = 'Clean impulse not successful, no change made.\n'
-            analysis.MESSAGE += 'Check if ch_{} exists for each set of data.'.format(ch_impulse)
-            self.show_message(analysis.MESSAGE,b='ok')
-            
-            
-    def undo_last_action(self):
-        if self.last_action == 'clean_impulse':
-            self.dataset = self.dataset_backup
-            self.update_figure()
-        if self.last_action == 'scaling':
-            self.dataset = self.dataset_backup
-            self.update_figure()
-        if self.last_action == 'delete modes':
-            self.dataset = self.dataset_backup
-            self.selected_channels = self.selected_channels_backup
-            self.update_figure()
-            message = 'Deleted mode fits restored.'
-            self.show_message(message)
-        if self.last_action == 'delete data':
-            self.dataset = self.dataset_backup
-            self.update_figure()
-            message = 'Deleted data restored.'
-            self.show_message(message)
-        if self.last_action == 'data replaced':
-            self.dataset = self.dataset_backup
-            self.update_figure()
-            message = 'Replaced data restored.'
-            self.show_message(message)
-            
-    def calc_fft(self):
-        if len(self.dataset.time_data_list) == 0:
-            message = 'No time data to calculate transfer function.'
-            self.show_message(message)
-        
-        else:
-            window = self.input_list_window_fft.currentText()
-            if window == 'None':
-                window = None
-            
-            self.dataset.calculate_fft_set(window=window)
-            self.switch_view('FFT Data')
-            
-    def select_averaging_type(self):
-        self.averaging_method = self.input_list_average_TF.currentText()
-        if self.averaging_method == 'None':
-            self.input_Nframes.setText('1')
-            self.slider_Nframes.setValue(1)
-            self.label_Nframes.setVisible(False)
-            self.input_Nframes.setVisible(False)
-            self.slider_Nframes.setVisible(False)
-            self.label_Nframes_time.setVisible(False)
-            self.button_TFav.setVisible(False)
-            self.button_TF.setVisible(True)
-            
-        elif self.averaging_method == 'within each set':
-            self.button_TFav.setVisible(False)
-            self.button_TF.setVisible(True)
-            self.label_Nframes.setVisible(True)
-            self.input_Nframes.setVisible(True)
-            self.label_Nframes_time.setVisible(True)
-            self.slider_Nframes.setVisible(True)
-            
-        elif self.averaging_method == 'across sets':
-            self.button_TF.setVisible(False)
-            self.label_Nframes.setVisible(False)
-            self.input_Nframes.setVisible(False)
-            self.slider_Nframes.setVisible(False)
-            self.label_Nframes_time.setVisible(False)
-            self.button_TFav.setVisible(True)
-            
-    def refresh_Nframes_text(self):
-        self.N_frames = self.slider_Nframes.value()
-        self.input_Nframes.setText(str(self.N_frames))
-        if len(self.dataset.time_data_list)>0:
-            stored_time = self.dataset.time_data_list[0].settings.stored_time
-            text = "Frame length = {:.2f} seconds.".format(stored_time/(self.N_frames-self.overlap*self.N_frames+self.overlap))
-        else:   
-            text = 'No time data'
-        self.label_Nframes_time.setText(text)
-        
-        
-    def refresh_Nframes_slider(self):
-        self.N_frames = int(self.input_Nframes.text())
-        # allows setting text to higher than max slider
-        try:
-            self.slider_Nframes.setValue(self.N_frames)
-        except:
-            pass
-        if len(self.dataset.time_data_list)>0:
-            stored_time = self.dataset.time_data_list[0].settings.stored_time
-            text = "Frame length = {:.2f} seconds.".format(stored_time/(self.N_frames-self.overlap*self.N_frames+self.overlap))
-        else:   
-            text = 'No time data'
-        self.label_Nframes_time.setText(text)
-        
-        
-    def refresh_test_name(self):
-        # keep both places for entering test_name up to date
-        self.input_test_name2.setText(self.input_test_name.text())
-        self.test_name = self.input_test_name.text()
-        
-    def refresh_test_name2(self):
-        # keep both places for entering test_name up to date
-        self.input_test_name.setText(self.input_test_name2.text())
-        self.test_name = self.input_test_name2.text()
-        
-    def calc_tf(self):
-        if len(self.dataset.time_data_list) == 0:
-            message = 'No time data to calculate transfer function.'
-            self.show_message(message)
-        
-        else:
-            self.N_frames = int(self.input_Nframes.text())
-            window = self.input_list_window_tf.currentText()
-            if window == 'None':
-                window = None
-
-            self.dataset.calculate_tf_set(window=window,N_frames=self.N_frames,overlap=self.overlap)
-            if self.current_view != 'TF Data':
-                self.switch_view('TF Data')
-            else:
-                self.auto_xy = ''
-                self.update_figure()
-            
-    
-    def calc_tf_av(self,b):
-        if len(self.dataset.time_data_list) == 0:
-            message = 'No data to calculate FFT.'
-            self.show_message(message)
-        
-        else:
-            window = self.input_list_window_tf.currentText()
-            if window == 'None':
-                window = None
-        
-            self.dataset.calculate_tf_averaged(window=window)
-            
-            if self.current_view != 'TF Data':
-                self.switch_view('TF Data')
-            else:
-                self.auto_xy = ''
-                self.update_figure()
-        
-    def xiw(self):
-        power = 1
-        self.xiwp(power)
-        
-    def diw(self):
-        power = -1
-        self.xiwp(power)
-
-
-        
-    def xiwp(self,power):
-        if self.flag_scaling == False:
-            # create backup before any changes made - used to reset
-            self.dataset_backup = copy.deepcopy(self.dataset)
-                
-        if self.current_view == 'FFT Data':
-            data_list = self.dataset.freq_data_list
-        elif self.current_view == 'TF Data':
-            data_list = self.dataset.tf_data_list
-        else:
-            message = 'First select ''FFT Data'' or ''TF Data''.'
-            self.show_message(message)
-            return None
-        
-        if len(data_list) > 0:            
-            s = self.p.get_selected_channels()
-            if self.selected_channels != s:
-                # reset gui's iw_power record if changed selection
-                self.iw_fft_power = 0
-                self.selected_channels = s
-                
-            
-            for ns in range(len(s)):
-                newdata = analysis.multiply_by_power_of_iw(data_list[ns],power=power,channel_list=s[ns])
-                data_list[ns] = newdata
-                self.flag_scaling = True
-                
-            if data_list.__class__.__name__ == 'FreqData':
-                self.dataset.freq_data_list = data_list
-            elif data_list.__class__.__name__ == 'TfData':
-                self.dataset.tf_data_list = data_list
-            
-            
-            if self.plot_type == 'Nyquist':
-                self.auto_xy = 'xy'
-            else:
-                self.auto_xy = 'fy'
-            
-            self.update_figure()
-            self.p.set_selected_channels(s)
-            
-            self.iw_fft_power += power # local counter for currently selected channels
-            self.last_action = 'scaling'
-            message = 'Selected FFT data multiplied by (iw)**{}\n'.format(self.iw_fft_power)
-            message += '(note that power counter resets when selection changes)'
-            self.show_message(message)
-        else:
-            message = 'First calculate FFT or TF of data.'
-            self.show_message(message)
-        
-    def undo_scaling(self):
-        if self.last_action == 'scaling':
-            self.undo_last_action()
-            self.flag_scaling = False
-            message = 'Scaling removed.'
-        else:
-            message = 'Can''t undo: scaling not last action carried out.'
-        
-        self.show_message(message)
-        
-        
-    def best_match(self):
-        if self.flag_scaling == False:
-            # provide backup for undo
-            self.dataset_backup = copy.deepcopy(self.dataset)
-            self.flag_scaling = True
-            
-        self.refset  = int(self.input_refset.text())
-        self.refchan = int(self.input_refchan.text())
-        if self.current_view == 'TF Data':
-            current_calibration_factors = self.dataset.tf_data_list.get_calibration_factors()
-            reference = current_calibration_factors[self.refset][self.refchan]
-            factors = analysis.best_match(self.dataset.tf_data_list,freq_range=self.freq_range,set_ref=self.refset,ch_ref=self.refchan)
-            factors = [reference*x for x in factors]
-            self.dataset.tf_data_list.set_calibration_factors_all(factors)
-            self.auto_xy = ''
-            self.update_figure()
-            with np.printoptions(precision=3, suppress=False):
-                message = 'Scale factors:\n'
-                n_set = -1
-                self.factors = factors
-                for fs in factors:
-                    n_set += 1
-#                    message += 'Set {:>10:d}: factors = {:.5g}\n'.format(n_set,np.squeeze(fs))
-#                    [[fill]align][sign][#][0][minimumwidth][.precision][type]
-                    message += '{:<3} {:>4} {:<12} {}\n'.format('Set',n_set,': factors =',np.squeeze(fs))
-                self.show_message(message)
-            
-            self.last_action = 'scaling'
-            
-        else:
-            message = 'First select ''TF Data'' or ''Calc TF''.\n'
-            self.show_message(message)
-        
-    def fit_mode(self):
-        if self.current_view == 'TF Data':
-            if self.input_list_tf_type.currentText() == 'Acceleration':
-                self.measurement_type = 'acc'
-            elif self.input_list_tf_type.currentText() == 'Velocity':
-                self.measurement_type = 'vel'
-            elif self.input_list_tf_type.currentText() == 'Displacement':
-                self.measurement_type = 'dsp'
-            
-            m = modal.modal_fit_all_channels(self.dataset.tf_data_list,freq_range=self.freq_range, measurement_type=self.measurement_type)
-            self.last_mode_fit = m
-            self.show_message(modal.MESSAGE)
-            if len(self.dataset.modal_data_list) == 0:
-                self.dataset.modal_data_list = [m]
-            elif len(self.fn_in_range) > 1:
-                message = 'Several mode fits already in this range.\n\n'
-                message += 'Fitted mode frequencies = {} (Hz)\n\n'.format(np.array2string(self.fn_in_range,precision=2))
-                message += 'To delete them, press ''Reject''.'
-                message += 'To replace a single fit, zoom into a single peak first.'
-                self.show_message(message)
-                return None
-            elif len(self.fn_in_range) == 1:
-                # find which mode and replace it
-                fn_all = self.dataset.modal_data_list[0].M[:,0]
-                mode_number = np.where((fn_all > self.freq_range[0]) & (fn_all < self.freq_range[1]))[0]
-                self.dataset.modal_data_list[0].delete_mode(mode_number)
-                self.dataset.modal_data_list[0].add_mode(m.M[0,:]) # only one mode in 'm'
-            else:
-                self.dataset.modal_data_list[0].add_mode(m.M[0,:]) # only one mode in 'm'
-            
-            # local reconstruction
-            s1 = self.p.get_selected_channels() # keep selection after auto-range
-            
-            f = np.linspace(self.freq_range[0],self.freq_range[1],3000)
-            tf_data = modal.reconstruct_transfer_function(m,f,self.measurement_type)
-            tf_data.flag_modal_TF = True
-            self.dataset.tf_data_list.add_modal_reconstruction(tf_data,mode='replace')
-            
-            if self.plot_type == 'Nyquist':
-                self.auto_xy = 'xy'
-            else:
-                self.auto_xy = 'fy'
-                
-            self.update_figure()
-            s2 = self.p.get_selected_channels()
-            # retain selection for fitted selection
-            # assumes each set is a single Transfer Function
-            # might break down if data organised differently
-            for i in range(len(s2[-1])):
-                #s2[i] = s1[i]
-                s2[-1][i] = s2[i][0]
-            if len(s1) != len(s2):
-                s1 += [[]]
-                
-            self.p.set_selected_channels(s2) # keep selection after auto-range
-            self.selected_channels = s2.copy()
-            self.update_figure() # run a second time so autoscaling picks up new lines
-            fn_all = self.dataset.modal_data_list[0].M[:,0]
-            self.fn_in_range = m.fn
-            ### allow time for plots and axes to update before clearing modal.MESSAGE
-            #time.sleep(1)
-            #modal.MESSAGE = '' # this is a condition for update_axes_values to let modal messages appear
-        else:
-            message = 'First select ''TF Data''.'
-            self.show_message(message)
-            
-    
-    def freq_min2(self):
-        self.freq_range[0] = float(self.input_freq_min2.text())
-        self.input_freq_min.setText(str(self.freq_range[0]))
-        self.freq_min()
-    
-    def freq_max2(self):
-        self.freq_range[1] = float(self.input_freq_max2.text())
-        self.input_freq_max.setText(str(self.freq_range[1]))
-        self.freq_max
-        
-    def accept_mode(self):
-        self.dataset.modal_data_list
-        self.view_modal_reconstruction()
-        
-    
-    def reject_mode(self):
-        # reject mode fits currently in view
-        if len(self.fn_in_range) >= 1:
-            self.last_action = 'delete modes'
-            self.dataset_backup = copy.deepcopy(self.dataset)
-            self.selected_channels_backup = self.p.get_selected_channels()
-            # find which mode and replace it
-            fn_all = self.dataset.modal_data_list[0].M[:,0]
-            mode_number = np.where((fn_all > self.freq_range[0]) & (fn_all < self.freq_range[1]))[0]
-            self.dataset.modal_data_list[0].delete_mode(mode_number)
-            if self.dataset.tf_data_list[-1].flag_modal_TF == True:
-                self.dataset.remove_last_data_item('TfData')
-                self.selected_channels.pop(-1) # updates selected channels
-                self.auto_xy = ''
-                self.update_figure()
-            message = 'Mode fits deleted.'
-            self.show_message(message,b='undo')
-        
-    def view_mode_summary(self):
-        message = 'Modes fitted:\n\n'
-        message += 'fn = {} (Hz)\n\n'.format(np.array2string(self.dataset.modal_data_list[0].fn,precision=2))
-        message += 'zn = {}\n'.format(np.array2string(self.dataset.modal_data_list[0].zn,precision=5))
-        message += 'Qn = 1/(2 zn) = {}'.format(np.array2string(1/2/self.dataset.modal_data_list[0].zn,precision=1))
-        self.show_message(message)
-    
-    def view_modal_reconstruction(self):
-        # Global reconstruction
-        s = self.p.get_selected_channels() # keep selection after auto-range
-        
-        f = self.dataset.tf_data_list[0].freq_axis
-        m = self.dataset.modal_data_list[0]
-        tf_data = modal.reconstruct_transfer_function_global(m,f,self.measurement_type)
-        tf_data.flag_modal_TF = True
-        self.dataset.tf_data_list.add_modal_reconstruction(tf_data,mode='replace')
-        
-        self.auto_xy = 'xy'
-        self.update_figure()
-        s2 = self.p.get_selected_channels()
-        for i in range(len(s2[-1])):
-            s2[-1][i] = True
-        if len(s) != len(s2):
-            s += [[]]
-        s[-1] = s2[-1]
-        self.p.set_selected_channels(s) # keep selection after auto-range
-        self.fn_in_range = m.fn
-        
-    def refresh_sono_N_frames_slider(self):
-        self.slider_sono_N_frames.setValue(int(self.input_sono_N_frames.text()))
-    
-    def refresh_sono_N_frames_text(self):
-        self.input_sono_N_frames.setText(str(self.slider_sono_N_frames.value()))
-    
-    def calc_sono(self):
-        if len(self.dataset.time_data_list) == 0:
-            message = 'No time data to calculate transfer function.'
-            self.show_message(message)
-        else:
-            self.N_frames_sono = int(self.input_sono_N_frames.text())
-            n_set = int(self.input_sono_n_set.text())
-            n_chan = int(self.input_sono_n_chan.text())
-#            db_range = int(self.input_db_range.text())
-            NT = len(self.dataset.time_data_list[n_set].time_data[:,n_chan])
-            f = 1/4 # match overlap in sonogram
-            self.nperseg = int(NT // (self.N_frames_sono * (1-f) + f)) # 1/8 is default overlap for spectrogram
-            self.dataset.calculate_sono_set(nperseg=self.nperseg)
-            
-            # calc sonogram info
-            npfft,npt = np.shape(self.dataset.sono_data_list[n_set].sono_data[:,:,n_chan])
-            text = 'FFT length: {}\n'.format(self.nperseg)
-            text += 'Freq resolution: {:5g} (Hz)\n'.format(np.diff(self.dataset.sono_data_list[n_set].freq_axis[[0,1]])[0])
-            
-            self.sono_info.setText(text)
-            if self.current_view != 'Sono Data':
-                self.switch_view('Sono Data')
-            self.update_figure()
-            
-    def import_jwlogger(self):
-        pass
-    
-    def export_jwlogger(self):
-        # export data to data structure compatible with JW Logger
-        file.export_to_matlab_jwlogger(self.dataset)        
-        
-    def export_matlab(self):
-        # export data to data structure compatible with Matlab
-        file.export_to_matlab(self.dataset)
-    
-    def export_csv(self):
-        # export data displayed to CSV
-        if  self.current_view == 'Time Data':
-            file.export_to_csv(self.dataset.time_data_list)
-        elif  self.current_view == 'FFT Data':
-            file.export_to_csv(self.dataset.freq_data_list)
-        elif  self.current_view == 'TF Data':
-            file.export_to_csv(self.dataset.tf_data_list)
-        else:
-            self.show_message('Can only export Time, FFT or TF Data')
-        
-#sys._excepthook = sys.excepthook 
-#def exception_hook(exctype, value, traceback):
-#    print(exctype, value, traceback)
-#    sys._excepthook(exctype, value, traceback) 
-#    sys.exit(1) 
-#sys.excepthook = exception_hook 
-
-
-
-class Oscilloscope():
-    def __init__(self, settings):
-        '''Creates an Oscilloscope
-        Args:
-            settings: An object of the class MySettings
-        '''
-
-        self.settings = settings
-        
-        streams.start_stream(settings)
-        self.rec = streams.REC
-        
-
-        self.timer = QtCore.QTimer()
-        self.create_figure()
-
-        self.win.sigKeyPress.connect(self.keyPressed)
-        self.win.sigClose.connect(self.on_close)
-
-        # Start the update timer
-        self.timer.timeout.connect(self.update) # update figure and buffer
-        self.timer.start(60)
-
-        if app.applicationState() != Qt.ApplicationActive:
-            app.exec()  
-
-    def create_figure(self):
-        '''
-        Creates a figure which is an object of the class KeyPressWindow.
-
-        '''
-        pg.setConfigOption('background', 'w')
-        self.win = KeyPressWindow()
-        self.win.setWindowIcon(QtGui.QIcon('icon.png'))
-#        window_geometry = self.win.geometry()
-        self.win.setGeometry(100,100,800,600)
-        self.win.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
-        
-        # This ensures the window appears at front.
-        # self.win.showMinimized()
-        
-
-        self.win.setWindowTitle("Oscilloscope ('s': save new, 'space': autosave, 'p': pause, 'a': always top, 'y': autoscale)")
-        # time.sleep(0.6)
-        self.win.show()
-        self.win.showNormal()
-        self.win.raise_()
-
-        self.view_time = self.settings.init_view_time
-        self.view_freq = self.settings.init_view_freq
-        self.view_levels = self.settings.init_view_levels
-
-        self.toggle_view()
-        
-        self.auto_scale = False
-
-        self.data_saved_counter = 0 #  to indicate not yet saved file
-
-    def on_close(self, evt):
-        self.timer.stop()
-        # self.rec.end_stream()
-
-    def toggle_view(self):
-        '''
-        Switches between views, triggered by keypress
-        '''
-        self.win.clear()
-
-        if self.view_time:
-            self.time_plot()
-
-        if self.view_freq:
-            self.freq_plot()
-
-        if self.view_levels:
-            self.levels_plot()
-
-    def time_plot(self):
-        # create a plot for the time domain
-        self.view_time = True
-        self.win.nextRow()
-        self.osc_time_line = self.win.addPlot(title="Time Domain (toggle with 'T')")
-
-        if self.settings.channels == 1:
-            self.auto_scale = True
-            self.osc_time_line.enableAutoRange()
-        else:
-            # Stack the channels -- channel 0 is centred on 0, channel 1
-            # centred on 1 etc.
-            self.auto_scale = False
-            self.osc_time_line.setYRange(-1,self.settings.channels)
-
-        self.osc_time_line.setXRange(self.rec.osc_time_axis[0],
-                                     self.rec.osc_time_axis[-1])
-        self.osc_time_line.showGrid(True, True)
-        self.osc_time_line.addLegend()
-        self.osc_time_line.setLabel('left', 'Normalised Amplitude')
-        self.osc_time_line.setLabel('bottom', 'Time (s)')
-
-        self.ax_time = self.osc_time_line.getAxis('left')
-        self.ax_time.setTickSpacing(1, 1)
-
-        self.osc_time_lineset = {}
-        for i in range(self.settings.channels):
-            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:])
-            self.osc_time_lineset[i] = self.osc_time_line.plot(
-                pen=pen_, name='Channel %d' % i)
-
-#        self.win.FillBetweenItem(curve1=osc_time_lineset[0], curve2=osc_time_lineset[1])
-
-    def freq_plot(self):
-        # create a plot for the frequency domain
-        self.view_freq = True
-        self.win.nextRow()
-        self.osc_freq_line = self.win.addPlot(
-            title="Frequency Domain (toggle with 'F')")
-        self.osc_freq_line.enableAutoRange()
-        self.osc_freq_line.setXRange(self.rec.osc_freq_axis[0],
-                                     self.rec.osc_freq_axis[-1])
-        self.osc_freq_line.showGrid(True, True)
-        self.osc_freq_line.addLegend()
-        self.osc_freq_line.setLabel('left', 'Power Spectrum (dB)')
-        self.osc_freq_line.setLabel('bottom', 'Frequency (Hz)')
-
-        self.osc_freq_lineset = {}
-        for i in range(self.settings.channels):
-            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:])
-            self.osc_freq_lineset[i] = self.osc_freq_line.plot(
-                pen=pen_, name='Channel %d' % i)
-
-    def levels_plot(self):
-        # create a plot for the frequency domain
-        self.view_levels = True
-        self.win.nextRow()
-        self.osc_levels_line = self.win.addPlot(title="Channel Levels (toggle with 'L')")
-        self.osc_levels_line.setYRange(0, 1)
-        self.osc_levels_line.setXRange(-0.5, self.settings.channels - 0.5)
-        self.osc_levels_line.showGrid(False, True)
-        self.osc_levels_line.setLabel('left', 'Normalised Amplitude')
-        self.osc_levels_line.setLabel('bottom', 'Channel Index')
-
-        self.ax_levels = self.osc_levels_line.getAxis('bottom')
-        self.ax_levels.setTickSpacing(1, 1)
-#        ax.showLabel(show=True)
-#        self.osc_levels_line.setTicks(np.arange(self.settings.channels))
-        self.osc_levels_lineset={}
-        for i in range(self.settings.channels):
-            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
-            pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
-            self.osc_levels_lineset[i]=self.osc_levels_line.plot(pen=pen_, name='vertical')
-            self.osc_levels_lineset[self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_, name='top')
-            self.osc_levels_lineset[2*self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_peak, name='peak hold')
-#            self.osc_levels_lineset[3]=self.osc_levels_line.plot(pen=pen_, name='Channel')
-
-        self.osc_levels_peak_hold = np.zeros(self.settings.channels)
-        self.time_last_changed = np.zeros(self.settings.channels)
-
-    def update(self):
-        '''
-        Updates plots with incoming data from __call__.
-        Called with a 0s interval by QTimer.
-
-        '''
-        time_data_snapshot = np.copy(self.rec.osc_time_data)
-        if self.view_levels == True:
-            self.osc_levels_rms = np.sqrt(np.mean(time_data_snapshot**2,axis=0))
-            self.osc_levels_max = np.max(np.abs(time_data_snapshot),axis=0)
-            changed_indices = self.osc_levels_peak_hold < self.osc_levels_max
-            self.time_last_changed[changed_indices] = time.time()
-            self.osc_levels_peak_hold = np.maximum(self.osc_levels_peak_hold,self.osc_levels_max)
-            self.osc_levels_peak_hold[time.time()-self.time_last_changed>2] = 0
-
-        for i in range(self.settings.channels):
-            offset = i
-            if self.view_time == True:
-                if (self.auto_scale is True) and (self.settings.channels==1):
-                    shift = 0
-                    scale_factor = 1
-                    self.osc_time_line.enableAutoRange()
-                elif (self.auto_scale is True) and (self.settings.channels!=1):
-                    shift = np.mean(time_data_snapshot[:,i])
-                    scale_factor = np.max(np.abs(time_data_snapshot[:,i]-shift))*2
-                    self.osc_time_line.setYRange(-1,self.settings.channels)
-                else:
-                    shift = 0
-                    scale_factor = 1
-                    self.osc_time_line.setYRange(-1,self.settings.channels)
-                    
-                self.osc_time_lineset[i].setData(self.rec.osc_time_axis, (time_data_snapshot[:,i]-shift)/scale_factor + offset)
-
-            if self.view_freq == True:
-                # calculate the FFT
-                self.rec.osc_time_data_windowed[:,i] = time_data_snapshot[:,i] * np.blackman(np.shape(time_data_snapshot)[0])
-                fd = np.abs(np.fft.rfft(self.rec.osc_time_data_windowed[:,i]))/len(self.rec.osc_time_data_windowed[:,i])
-                fd[fd==0] = np.min(fd+1e-16) # to avoid log10(0) warnings
-                self.rec.osc_freq_data[:,i] = 20 * np.log10(fd)
-                self.osc_freq_lineset[i].setData(self.rec.osc_freq_axis,self.rec.osc_freq_data[:,i])
-
-            if self.view_levels == True:
-                self.osc_levels_lineset[i].setData([i,i],[0,self.osc_levels_max[i]])
-                self.osc_levels_lineset[self.settings.channels+i].setData([i-0.3,i+0.3],self.osc_levels_max[i]*np.ones(2))
-
-                if self.osc_levels_peak_hold[i] > 0.98:
-                    pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=10)
-                else:
-                    pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
-#                self.osc_levels_lineset[2*self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_peak, name='peak hold')
-                self.osc_levels_lineset[2*self.settings.channels+i].setData([i-0.3,i+0.3],self.osc_levels_peak_hold[i]*np.ones(2),pen=pen_peak)
-#                self.osc_levels_lineset[3].setData(np.arange(2),np.ones(2))
-
-
-
-    #KeyPressed function within osciolloscpe since can only take one argument
-    def keyPressed(self, evt):
-        '''
-        Upon a Space Bar press, makes a copy of data from the past stored_time seconds,plots it in Bokeh and gives the user an option to save it.
-        '''
-
-        if evt.key() == QtCore.Qt.Key_T:
-
-            if self.view_freq != False or self.view_levels != False:
-#                print('toggled time domain view')
-                self.view_time = not self.view_time
-                self.toggle_view()
-#            else:
-#                print('toggling all views off is prevented')
-
-        if evt.key() == QtCore.Qt.Key_F:
-
-            if self.view_time != False or self.view_levels != False:
-#                print('toggled frequency domain view')
-                self.view_freq = not self.view_freq
-                self.toggle_view()
-#            else:
-#                print('toggling all views off is prevented')
-
-        if evt.key() == QtCore.Qt.Key_L:
-            if self.view_time != False or self.view_freq != False:
-#                print('toggled levels view')
-                self.view_levels = not self.view_levels
-                self.toggle_view()
-#            else:
-#                print('toggling all views off is prevented')
-        
-        if evt.key() == QtCore.Qt.Key_P:
-            if self.timer.isActive():
-                self.timer.stop()
-            else:
-                self.timer.start()
-                
-        if evt.key() == QtCore.Qt.Key_A:
-            self.win.setWindowFlags(self.win.windowFlags() ^ QtCore.Qt.WindowStaysOnTopHint)       
-            self.win.show()
-                
-            
-        if evt.key() == QtCore.Qt.Key_Y:
-            self.auto_scale = not self.auto_scale 
-                
-        if evt.key() == QtCore.Qt.Key_Space or evt.key() == QtCore.Qt.Key_S:
-
-            stored_time_data_copy=np.copy(self.rec.stored_time_data)
-            t = datetime.datetime.now()
-            timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)
-#            print("key press trigger: saving data to file in working directory")
-
-            ### make into dataset
-            
-            fs=self.settings.fs
-            n_samp=len(stored_time_data_copy[:,0])
-            dt=1/fs
-            t_axis= np.arange(n_samp)*dt
-
-            
-            timedata = datastructure.TimeData(t_axis,stored_time_data_copy,self.settings,timestamp=t,timestring=timestring,test_name='Test_{}'.format(self.data_saved_counter))
-            
-            dataset = datastructure.DataSet()
-            dataset.add_to_dataset(timedata)
-            
-            
-            if evt.key() == QtCore.Qt.Key_S:
-                self.data_saved_counter = 1
-                self.last_filename = file.save_data(dataset,self.win)
-            
-#            # this version saves all data as new timedata objects within one file
-#            if evt.key() == QtCore.Qt.Key_Space:
-#                if self.data_saved_counter == 0:
-#                    self.last_filename = file.save_data(dataset)
-#                    if self.last_filename == '':
-#                        self.data_saved_counter = 0
-#                    else:
-#                        self.data_saved_counter += 1
-#                
-#                else:
-#                    d = file.load_data(self.last_filename)
-#                    d.add_to_dataset(timedata)
-#                    file.save_data(d,self.last_filename,overwrite_without_prompt=True)
-#                    self.data_saved_counter += 1
-            
-            # this version saves each new dataset to new file
-            if evt.key() == QtCore.Qt.Key_Space:
-                if self.data_saved_counter == 0:
-                    self.last_filename = file.save_data(dataset,self.win)
-                    if self.last_filename == '':
-                        self.data_saved_counter = 0
-                    else:
-                        self.data_saved_counter += 1
-                
-                else:
-                    d = datastructure.DataSet()
-                    d.add_to_dataset(timedata)
-                    filename = self.last_filename.replace('.npy','_'+str(self.data_saved_counter)+'.npy')
-                    file.save_data(d,self.win, filename,overwrite_without_prompt=True)
-                    self.data_saved_counter += 1
-
-class KeyPressWindow(pg.GraphicsLayoutWidget):
-    '''
-    A subclass of pyQtGraph GraphicsWindow that emits a signal when a key is pressed.
-
-    '''
-    sigKeyPress = Signal(object)
-    sigClose = Signal(object)
-
-    def __init__(self, *args, **kwargs):
-        '''
-        Re-implmented from parent.
-        '''
-        super().__init__(*args, **kwargs)
-
-    def keyPressEvent(self, evt):
-        '''
-        Emits a signal upon a key press
-        '''
-        self.scene().keyPressEvent(evt)
-        self.sigKeyPress.emit(evt)
-
-    def closeEvent(self, evt):
-        '''
-        Emits a signal when the window is closed.
-        '''
-        self.sigClose.emit(evt)
-        self.close()
+from qtpy.QtWidgets import QMainWindow, QApplication, QWidget, QPushButton, QMessageBox, QTabWidget, QFormLayout, QToolBar, QLineEdit, QLabel, QComboBox, QSlider, QSizePolicy, QVBoxLayout, QHBoxLayout, QGridLayout, QGroupBox, QFrame, QStyleFactory, QSplitter, QFrame, QFormLayout
+from qtpy.QtCore import Qt, QThread, Signal, QTimer, QObject
+from qtpy.QtGui import QPalette, QDoubleValidator, QIntValidator, QFontMetrics
+from qtpy import QtGui
+from qtpy.QtWidgets import QToolTip, QFileDialog
+from qtpy import QtCore
+
+import pyqtgraph as pg
+
+import copy
+from matplotlib.backends.backend_qt5agg import FigureCanvas, NavigationToolbar2QT as NavigationToolbar
+from matplotlib.figure import Figure
+from matplotlib.ticker import AutoLocator
+import numpy as np
+import datetime
+
+
+
+
+#import logging
+#logging.basicConfig(filename='example.log',level=logging.DEBUG)
+#%%
+
+from . import plotting
+from . import datastructure
+from . import acquisition
+from . import analysis
+from . import streams
+from . import file
+from . import modal
+from . import options
+from . import oscilloscope
+import time
+import sys, os
+
+
+#%%
+class BlueButton(QPushButton):
+    def __init__(self,text):
+        super().__init__(text)
+        self.setStyleSheet("background-color: hsv(240, 170, 255)")
+        self.setText(text) 
+
+class GreenButton(QPushButton):
+    def __init__(self,text):
+        super().__init__(text)
+        self.setStyleSheet("background-color: hsv(120, 170, 255);")
+        self.setText(text)
+
+class RedButton(QPushButton):
+    def __init__(self,text):
+        super().__init__(text)
+        self.setStyleSheet("background-color: hsv(0, 170, 255)")
+        self.setText(text)
+        
+class OrangeButton(QPushButton):
+    def __init__(self,text):
+        super().__init__(text)
+        self.setStyleSheet("background-color: hsv(30, 170,255)")
+        self.setText(text)
+
+class QHLine(QFrame):
+    def __init__(self):
+        super(QHLine, self).__init__()
+        self.setFrameShape(QFrame.HLine)
+        self.setFrameShadow(QFrame.Sunken)
+        
+class newComboBox(QComboBox):
+    def __init__(self,items_list):
+        super().__init__()
+        self.setStyleSheet('selection-background-color: hsv(240, 170, 255)')
+        self.addItems(items_list)
+        
+class boldLabel(QLabel):
+    def __init__(self,text):
+        super().__init__(text)
+        self.setStyleSheet('font: bold')
+        
+        
+class LogDataThread(QThread):
+    
+    s = Signal(datastructure.DataSet)
+
+    def __init__(self,settings,test_name,rec,output):
+        super().__init__()
+        
+        self.settings = settings
+        self.test_name = test_name
+        self.rec = rec
+        self.output = output
+        
+    def __del__(self):
+        self.wait()
+    
+    def run(self):
+        self.d = acquisition.log_data(self.settings,test_name=self.test_name, rec=self.rec, output=self.output)
+        self.s.emit(self.d)
+        
+        
+        
+class PreviewWindow():
+    def __init__(self,title='Time Data'):
+        self.preview_window = QWidget()
+        self.preview_window.setStyleSheet("background-color: white")
+        self.preview_window.setWindowTitle('Output Signal Preview')
+        self.preview_window.setWindowIcon(QtGui.QIcon('pydvma/icon.png'))
+
+        self.fig = Figure(figsize=(9, 5),dpi=100)
+        self.canvas = FigureCanvas(self.fig)
+        self.toolbar = NavigationToolbar(self.canvas,None)
+        self.toolbar.setOrientation(Qt.Orientation.Horizontal)
+        self.p = plotting.PlotData(canvas=self.canvas,fig=self.fig)
+        
+        self.label_figure = boldLabel(title)
+        self.label_figure.setMaximumHeight(20)
+        self.label_figure.setAlignment(Qt.AlignmentFlag.AlignCenter)
+        
+        # widgets to layout
+        self.layout_figure = QVBoxLayout()
+        self.layout_figure.addWidget(self.label_figure)
+        self.layout_figure.addWidget(self.canvas)
+        self.layout_figure.addWidget(self.toolbar)
+        
+        self.preview_window.setLayout(self.layout_figure)
+        
+        self.preview_window.showMinimized()
+        time.sleep(0.6)
+        self.preview_window.show()
+        self.preview_window.showNormal()
+        self.preview_window.raise_()
+        
+app = QApplication(sys.argv)
+app.setStyle(QStyleFactory.create('Fusion'))
+app.setWindowIcon(QtGui.QIcon('pydvma/icon.png'))
+
+class Logger():
+        
+    def __init__(self,settings=None,test_name=None,default_window=None):
+        
+        # Initialise variables
+        global MESSAGE
+        if default_window is None:
+            default_window = 'None'
+        self.settings = settings
+        self.test_name = test_name
+        self.dataset = datastructure.DataSet()
+        
+        self.default_window = default_window
+        self.current_view = 'Time'    
+        self.N_frames = 1
+        self.overlap = 0.5
+        self.iw_fft_power = 0
+        self.iw_tf_power = 0
+        self.legend_loc = 'lower right'
+        self.show_coherence = True
+        self.show_data = True
+        self.coherence_plot_type = 'linear'
+        self.xlinlog = 'linear'
+        self.plot_type = None
+        self.freq_range = [0,np.inf]
+        self.auto_xy = 'xy'
+        self.sets = 'all'
+        self.channels = 'all'
+        self.last_action = None
+        self.iw_power = 0
+        self.selected_channels = []
+        self.flag_scaling = False
+        self.message_time = 0
+        self.flag_log_and_replace = False
+        self.flag_output = False
+        self.message_timer = QTimer() # purely for pretrig live messages
+        self.stream_check_timer = QTimer() # for levels messages
+        self.levels_timer = QTimer() # for levels messages
+        self.message = ''
+        self.t0_clipped = 0
+        self.fn_in_range = np.array([])
+        
+        # SETUP GUI
+        # self.app = app
+        # self.app.setStyle(QStyleFactory.create('Fusion'))
+        self.window = QWidget()
+        self.window.setStyleSheet("background-color: white")
+        self.window.setWindowTitle('Logger')
+        self.window.setWindowIcon(QtGui.QIcon('pydvma/icon.png'))
+        # self.window.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
+        
+        # initiate all interface tool frames
+        self.setup_frame_tools()
+        self.setup_frame_input()
+        self.setup_frame_figure()
+        self.setup_frame_save()
+        self.setup_frame_axes()
+        
+        # arrange frames and create window
+        self.setup_layout_main()
+        self.window.showNormal()
+        # time.sleep(0.6)
+        self.window.show()
+        self.window.raise_()
+        # self.window.showNormal()
+        
+        
+        # start stream if already passed settings
+        self.start_stream()
+        self.message_timer.timeout.connect(self.show_message_timer) # connect after stream started
+        self.stream_check_timer.start(1000)
+        self.stream_check_timer.timeout.connect(self.check_stream) # connect after stream started
+        self.levels_timer.timeout.connect(self.show_levels) # connect after stream started
+        
+        app.exec()
+
+        
+    def setup_layout_main(self):
+
+        # organise frames
+        self.splitter_mid = QSplitter(Qt.Orientation.Vertical)
+        self.splitter_mid.addWidget(self.frame_input)
+        self.splitter_mid.addWidget(self.frame_figure)
+        self.splitter_mid.addWidget(self.frame_save)
+        
+        self.splitter_all = QSplitter(Qt.Orientation.Horizontal)
+        self.splitter_all.addWidget(self.frame_axes)
+        self.splitter_all.addWidget(self.splitter_mid)
+        self.splitter_all.addWidget(self.frame_tools)
+        
+        # frames to main layout
+        self.layout_main = QGridLayout()
+        self.layout_main.addWidget(self.splitter_all)
+        
+        # main layout to window
+        self.window.setLayout(self.layout_main)
+        
+
+    def setup_frame_figure(self):
+        # content
+        
+        self.fig = Figure(figsize=(9, 7),dpi=100)
+        self.canvas = FigureCanvas(self.fig)
+        self.toolbar = NavigationToolbar(self.canvas,None)
+        
+        # disable some buttons
+        for ch in self.toolbar.children():
+            try:
+                if ch.iconText() in ['Home','Subplots','Save','Customize']:
+                    ch.setVisible(False)
+            except:
+                pass
+        
+        self.toolbar.setOrientation(Qt.Orientation.Horizontal)
+        self.p = plotting.PlotData(canvas=self.canvas,fig=self.fig)
+        self.p.ax.callbacks.connect('xlim_changed', self.update_axes_values)
+        self.p.ax.callbacks.connect('ylim_changed', self.update_axes_values)
+        self.p.ax.callbacks.connect('xlim_changed', self.update_modal_message)
+        self.p.ax2.callbacks.connect('ylim_changed', self.update_co_axes_values)
+        self.fig.canvas.mpl_connect('pick_event', self.update_selected_channels)
+        
+        self.label_figure = boldLabel('Time Data')
+        self.label_figure.setMaximumHeight(20)
+        self.label_figure.setAlignment(Qt.AlignmentFlag.AlignCenter)
+        
+        # widgets to layout
+        self.layout_figure = QGridLayout()
+        self.layout_figure.addWidget(self.label_figure,0,0,1,3)
+        self.layout_figure.addWidget(self.canvas,1,0,1,3)
+        self.layout_figure.addWidget(self.toolbar,2,1,1,1)
+        self.layout_figure.addWidget(QLabel('Back/Forward/Pan/Zoom:'),2,0,1,1)
+#        self.layout_figure.addWidget(QLabel('(box-zoom right-click will zoom out)'),2,2,1,1)
+        
+        # layout to frame
+        self.frame_figure = QFrame()
+        self.frame_figure.setFrameShape(QFrame.Shape.StyledPanel)
+        self.frame_figure.setLayout(self.layout_figure)
+        
+    def setup_frame_input(self):
+        
+        self.setup_frame_message()
+        
+        # content
+        self.button_osc = QPushButton('')
+        self.button_osc.setIcon(QtGui.QIcon('pydvma/icon.png'))
+        self.button_log_data = GreenButton('Log Data')
+        self.button_del_data = OrangeButton('Delete Last')
+        self.button_res_data = RedButton('Delete All')
+        self.button_load_data = BlueButton('Load Data')
+                
+        self.button_osc.clicked.connect(self.button_clicked_osc)
+        self.button_log_data.clicked.connect(self.button_clicked_log_data)
+        self.button_del_data.clicked.connect(self.delete_last_data)
+        self.button_res_data.clicked.connect(self.reset_data)
+        self.button_load_data.clicked.connect(self.load_data)
+        
+        # widgets to layout
+        self.layout_input = QGridLayout()
+        self.layout_input.addWidget(self.button_osc,0,0,1,1)
+        self.layout_input.addWidget(self.button_log_data,0,1,1,4)
+        self.layout_input.addWidget(self.button_del_data,0,5,1,4)
+        self.layout_input.addWidget(self.button_res_data,0,9,1,4)
+        self.layout_input.addWidget(self.button_load_data,0,13,1,4)
+        self.layout_input.addWidget(self.frame_message,1,0,1,17)
+        self.layout_input.setAlignment(Qt.AlignmentFlag.AlignTop)
+        
+        # layout to frame
+        self.frame_input = QFrame()
+        self.frame_input.setFrameShape(QFrame.Shape.StyledPanel)
+        self.frame_input.setLayout(self.layout_input)
+        
+        
+    def setup_frame_message(self):
+        self.label_message = QLabel()
+        self.button_message = GreenButton('OK')
+        self.button_cancel = OrangeButton('Cancel')
+        self.button_undo = RedButton('Undo')
+        
+        # function connections
+        self.button_message.clicked.connect(self.hide_message)
+        self.button_cancel.clicked.connect(self.cancel_logging)
+        self.button_undo.clicked.connect(self.undo_last_action)
+        
+        self.layout_message = QGridLayout()
+        
+        self.layout_message.addWidget(self.label_message,0,0,1,3)
+        self.layout_message.addWidget(self.button_message,0,3,1,1)
+        self.layout_message.addWidget(self.button_cancel,0,3,1,1)
+        self.layout_message.addWidget(self.button_undo,1,3,1,1)
+        self.layout_message.setAlignment(Qt.AlignmentFlag.AlignTop)
+        
+        self.frame_message = QFrame()
+        self.frame_message.setLayout(self.layout_message)
+        self.hide_message()
+        
+        
+    def setup_frame_save(self):
+        # design items
+#        self.label_save = QLabel('Quick save:')
+        self.buttons_save = [GreenButton(i) for i in ['Save Dataset','Save Figure']]
+        self.buttons_save[0].clicked.connect(self.save_data)
+        self.buttons_save[1].clicked.connect(self.save_fig)
+        
+        # widgets to layout
+        self.layout_save = QHBoxLayout()
+        for n in range(len(self.buttons_save)):
+            self.layout_save.addWidget(self.buttons_save[n])
+            
+        # layout to frame
+        self.frame_save = QFrame()
+        self.frame_save.setFrameShape(QFrame.Shape.StyledPanel)
+        self.frame_save.setLayout(self.layout_save)
+        
+    
+    def setup_frame_axes(self):
+        
+        self.setup_frame_plot_details()
+        
+        self.input_list_figures = newComboBox(['Time Data','FFT Data','TF Data','Sono Data'])
+        self.input_list_figures.currentIndexChanged.connect(self.select_view)
+        
+        self.button_x = GreenButton('Auto X')
+        self.button_y = GreenButton('Auto Y')
+        
+        self.button_x.clicked.connect(self.auto_x)
+        self.button_y.clicked.connect(self.auto_y)
+        
+        self.label_axes = [QLabel(i) for i in ['xmin:','xmax:','ymin:','ymax:']]
+        self.input_axes = [QLineEdit() for i in range(4)]
+        self.input_axes[0].setValidator(QDoubleValidator(float(0),float(np.inf),5)) 
+        self.input_axes[0].editingFinished.connect(self.xmin)
+        self.input_axes[1].setValidator(QDoubleValidator(float(0),float(np.inf),5)) 
+        self.input_axes[1].editingFinished.connect(self.xmax)
+        self.input_axes[2].setValidator(QDoubleValidator(float(-np.inf),float(np.inf),5)) 
+        self.input_axes[2].editingFinished.connect(self.ymin)
+        self.input_axes[3].setValidator(QDoubleValidator(float(-np.inf),float(np.inf),5)) 
+        self.input_axes[3].editingFinished.connect(self.ymax)
+        
+        self.button_select_all_data = GreenButton('All')
+        self.button_select_no_data = GreenButton('None')
+        self.button_select_all_data.clicked.connect(self.select_all_data)
+        self.button_select_no_data.clicked.connect(self.select_no_data)
+        
+        self.button_select_next = GreenButton('>')
+        self.button_select_prev = GreenButton('<')
+        self.button_select_next.clicked.connect(self.next_chans)
+        self.button_select_prev.clicked.connect(self.prev_chans)
+        width = self.button_select_next.fontMetrics().boundingRect('>').width()*4
+        self.button_select_next.setMaximumWidth(width)
+        self.button_select_prev.setMaximumWidth(width)
+        
+        self.button_select_set_only = BlueButton('Show Set Only')
+        self.button_select_set_only.clicked.connect(self.show_set_only)
+        self.button_select_chan_only = BlueButton('Show Chan Only')
+        self.button_select_chan_only.clicked.connect(self.show_chan_only)
+        
+        self.input_select_set_only = QLineEdit('0')
+        self.input_select_set_only.setValidator(QIntValidator(0,1000))
+        self.input_select_chan_only = QLineEdit('0')
+        self.input_select_chan_only.setValidator(QIntValidator(0,1000))
+        
+        self.legend_buttons = [BlueButton(i) for i in ['left','on/off','right']]
+        self.legend_buttons[0].clicked.connect(self.legend_left)
+        self.legend_buttons[1].clicked.connect(self.legend_onoff)
+        self.legend_buttons[2].clicked.connect(self.legend_right)
+        
+        
+        # widgets to layout
+        self.layout_axes = QGridLayout()
+        self.layout_axes.setAlignment(Qt.AlignmentFlag.AlignTop)
+
+
+        # Figure selection
+        row_start = 0
+        self.layout_axes.addWidget(boldLabel('Figure selection:'),row_start+0,0,1,6)
+        self.layout_axes.addWidget(self.input_list_figures,row_start+1,0,1,6)
+        
+        # Axes control
+        row_start = 3
+        self.layout_axes.addWidget(QLabel(),row_start,0,1,6)
+        self.layout_axes.addWidget(boldLabel('Axes control:'),row_start+1,0,1,6)
+        self.layout_axes.addWidget(self.button_x,row_start+2,0,1,3)
+        self.layout_axes.addWidget(self.button_y,row_start+2,3,1,3)
+        
+        for n in range(len(self.label_axes)):
+            self.label_axes[n].setAlignment(Qt.AlignmentFlag.AlignRight)
+            self.layout_axes.addWidget(self.label_axes[n],row_start+n+4,0,1,2)
+            self.layout_axes.addWidget(self.input_axes[n],row_start+n+4,2,1,4)
+            
+        # Line Selection
+        row_start = 11
+        self.layout_axes.addWidget(QLabel(),row_start,0,1,6)
+        self.layout_axes.addWidget(boldLabel('Line Selection:'),row_start+1,0,1,6)
+        self.layout_axes.addWidget(self.button_select_all_data,row_start+2,0,1,2)
+        self.layout_axes.addWidget(self.button_select_no_data,row_start+2,2,1,2)
+        self.layout_axes.addWidget(self.button_select_prev,row_start+2,4,1,1)
+        self.layout_axes.addWidget(self.button_select_next,row_start+2,5,1,1)
+        self.layout_axes.addWidget(self.button_select_set_only,row_start+3,0,1,3)
+        self.layout_axes.addWidget(self.input_select_set_only,row_start+3,3,1,3)
+        self.layout_axes.addWidget(self.button_select_chan_only,row_start+4,0,1,3)
+        self.layout_axes.addWidget(self.input_select_chan_only,row_start+4,3,1,3)
+        
+        
+        # Legend control
+        row_start = 17
+        self.layout_axes.addWidget(QLabel(),row_start,0,1,6)
+        self.layout_axes.addWidget(boldLabel('Legend control:'),row_start+1,0,1,6)
+        for n in range(len(self.legend_buttons)):
+            self.layout_axes.addWidget(self.legend_buttons[n],row_start+2,2*n,1,2)
+        
+        
+        # Plot-specific tools
+        row_start = 20
+        self.layout_axes.addWidget(self.frame_plot_details,row_start,0,1,6)
+        self.frame_plot_details.setVisible(False)
+        
+        # layout to frame
+        self.frame_axes = QFrame()
+        self.frame_axes.setFrameShape(QFrame.Shape.StyledPanel)
+        self.frame_axes.setLayout(self.layout_axes)
+       
+    def setup_frame_plot_details(self):
+        #items
+        self.items_list_plot_type = ['Amplitude (dB)','Amplitude (linear)', 'Real Part', 'Imag Part', 'Nyquist', 'Phase']
+        self.input_list_plot_type = newComboBox(self.items_list_plot_type)
+        self.button_xlinlog = BlueButton('X Lin/Log')
+        self.button_data_toggle = BlueButton('Data on/off')
+        self.button_coherence_toggle = BlueButton('Coherence on/off')
+        
+        
+        self.label_co_freq_min = QLabel('co. min:')
+        self.label_co_freq_max = QLabel('co. max:')
+        self.input_co_min = QLineEdit('0')
+        self.input_co_min.setValidator(QDoubleValidator(float(-np.inf),float(np.inf),5))
+        self.input_co_max = QLineEdit('1')
+        self.input_co_max.setValidator(QDoubleValidator(float(-np.inf),float(np.inf),5))
+        
+        # freq range for Nyquist
+        self.input_freq_min = QLineEdit()
+        self.input_freq_min.setValidator(QDoubleValidator(float(0),float(np.inf),5))
+        self.input_freq_min.editingFinished.connect(self.freq_min)
+        self.input_freq_max = QLineEdit()
+        self.input_freq_max.setValidator(QDoubleValidator(float(0),float(np.inf),5))
+        self.input_freq_max.editingFinished.connect(self.freq_max)
+        
+        #self.button_modal_fit_toggle = BlueButton('Modal Fit on/off')
+        
+#        self.input_list_plot_type.currentIndexChanged.connect(self.select_view)
+        self.input_list_plot_type.activated.connect(self.select_view) # TRY THIS SO ONLY CALLED WITH MANUAL SELECTION NOT WITHIN SELECT_VIEW
+        self.input_co_min.editingFinished.connect(self.co_min)
+        self.input_co_max.editingFinished.connect(self.co_max)
+        self.button_data_toggle.clicked.connect(self.data_toggle)
+        self.button_coherence_toggle.clicked.connect(self.coherence_toggle)
+        self.button_xlinlog.clicked.connect(self.select_xlinlog)
+        #layout
+        self.layout_plot_details = QGridLayout()
+        self.layout_plot_details.addWidget(QLabel(),0,0,1,1)
+        self.layout_plot_details.addWidget(boldLabel('Plot type:'),1,0,1,2)
+        self.layout_plot_details.addWidget(self.input_list_plot_type,2,0,1,2)
+        self.layout_plot_details.addWidget(self.button_xlinlog,3,0,1,2)
+        self.layout_plot_details.addWidget(self.button_data_toggle,4,0,1,1)
+        self.layout_plot_details.addWidget(self.button_coherence_toggle,4,1,1,1)
+        self.layout_plot_details.addWidget(self.label_co_freq_min,5,0,1,1)
+        self.layout_plot_details.addWidget(self.input_co_min,5,1,1,1)
+        self.layout_plot_details.addWidget(self.input_freq_min,5,1,1,1)
+        self.layout_plot_details.addWidget(self.label_co_freq_max,6,0,1,1)
+        self.layout_plot_details.addWidget(self.input_co_max,6,1,1,1)
+        self.layout_plot_details.addWidget(self.input_freq_max,6,1,1,1)
+        #self.layout_plot_details.addWidget(self.button_modal_fit_toggle,7,0,1,2)        
+        
+        #only show these for Nyquist plots
+        self.input_freq_min.setVisible(False)
+        self.input_freq_max.setVisible(False)
+        
+        #frame
+        self.frame_plot_details = QFrame()
+        self.frame_plot_details.setLayout(self.layout_plot_details)
+    
+    
+    def setup_frame_tools(self):
+        
+        # initiate all tools frames
+        self.setup_frame_tools_selection()
+        self.setup_frame_tools_time_domain()
+        self.setup_frame_tools_fft()
+        self.setup_frame_tools_tf()
+        self.setup_frame_tools_scaling()
+        self.setup_frame_tools_mode_fitting()
+        self.setup_frame_tools_settings()
+        self.setup_frame_tools_generate_output()
+        self.setup_frame_tools_edit_dataset()
+        self.setup_frame_tools_sonogram()
+        self.setup_frame_tools_save_export()
+        
+        # widgets to layout
+        self.layout_tools = QVBoxLayout()
+        self.layout_tools.addWidget(self.frame_tools_selection)
+        self.layout_tools.addWidget(self.frame_tools_time_domain)
+        self.layout_tools.addWidget(self.frame_tools_fft)
+        self.layout_tools.addWidget(self.frame_tools_tf)
+        self.layout_tools.addWidget(self.frame_tools_scaling)
+        self.layout_tools.addWidget(self.frame_tools_mode_fitting)
+        self.layout_tools.addWidget(self.frame_tools_settings)
+        self.layout_tools.addWidget(self.frame_tools_generate_output)
+        self.layout_tools.addWidget(self.frame_tools_edit_dataset)
+        self.layout_tools.addWidget(self.frame_tools_sonogram)
+        self.layout_tools.addWidget(self.frame_tools_save_export)
+        
+        self.layout_tools.setAlignment(Qt.AlignmentFlag.AlignTop)
+        
+        # layout to frame
+        self.frame_tools = QFrame()
+        self.frame_tools.setFrameShape(QFrame.Shape.StyledPanel)
+        self.frame_tools.setLayout(self.layout_tools)
+        
+        # widgets to layout according to selection
+        self.input_list_tools.setCurrentText('Standard Tools')
+        self.select_tool()
+        
+        
+        
+        
+    def setup_frame_tools_selection(self):
+        
+        self.input_list_tools = newComboBox(['Standard Tools','Logger Settings','Generate Output','Pre-process','FFT','Transfer Function','Calibration / Scaling','Sonogram','Mode Fitting','Edit Dataset','Save / Export'])
+        self.input_list_tools.setCurrentIndex(0)
+        self.input_list_tools.currentIndexChanged.connect(self.select_tool)
+        
+        self.layout_tools_selection = QGridLayout()
+        self.layout_tools_selection.addWidget(boldLabel('Tool selection:'),0,0,1,3)
+        self.layout_tools_selection.addWidget(self.input_list_tools,1,0,1,3)
+        
+        self.frame_tools_selection = QFrame()
+        self.frame_tools_selection.setLayout(self.layout_tools_selection)
+        
+
+
+    def setup_frame_tools_time_domain(self):
+        
+        self.button_clean_impulse = BlueButton('Clean Impulse')
+        self.button_clean_impulse.clicked.connect(self.clean_impulse)
+        
+        self.input_impulse_channel = QLineEdit('0')
+        self.input_impulse_channel.setValidator(QIntValidator(0,1000))
+        self.layout_tools_time_domain = QGridLayout()
+        self.layout_tools_time_domain.addWidget(boldLabel('Pre-process:'),0,0,1,3)
+        self.layout_tools_time_domain.addWidget(QLabel('Impulse channel:'),1,0,1,1)
+        self.layout_tools_time_domain.addWidget(self.input_impulse_channel,1,1,1,2)
+        self.layout_tools_time_domain.addWidget(self.button_clean_impulse,2,0,1,3)
+        
+        self.frame_tools_time_domain = QFrame()
+        self.frame_tools_time_domain.setLayout(self.layout_tools_time_domain)
+
+
+    def setup_frame_tools_fft(self):
+        
+        self.input_list_window_fft = newComboBox(['None','hann'])
+        self.input_list_window_fft.setCurrentText(self.default_window)
+        self.button_FFT = BlueButton('Calc FFT')
+        self.button_FFT.clicked.connect(self.calc_fft)
+        
+        self.layout_tools_fft = QGridLayout()
+        self.layout_tools_fft.addWidget(boldLabel('FFT:'),0,0,1,3)
+        self.layout_tools_fft.addWidget(QLabel('window:'),1,0,1,1)
+        self.layout_tools_fft.addWidget(self.input_list_window_fft,1,1,1,2)
+        self.layout_tools_fft.addWidget(self.button_FFT,2,0,1,3)
+        
+        self.frame_tools_fft = QFrame()
+        self.frame_tools_fft.setLayout(self.layout_tools_fft)
+
+    def setup_frame_tools_tf(self):
+        self.input_list_window_tf = newComboBox(['None','hann'])
+        self.input_list_window_tf.setCurrentText(self.default_window)
+        self.input_list_average_TF = newComboBox(['None','within each set','across sets'])
+        self.input_list_average_TF.setCurrentText(self.default_window)
+        self.button_TF = BlueButton('Calc TF')
+        self.button_TF.clicked.connect(self.calc_tf)
+        self.input_list_average_TF.currentIndexChanged.connect(self.select_averaging_type)
+        self.label_Nframes = QLabel('N frames:')
+        self.input_Nframes = QLineEdit()
+        self.input_Nframes.setValidator(QIntValidator(1,1000))
+        self.input_Nframes.setText('1')
+        self.input_Nframes.editingFinished.connect(self.refresh_Nframes_slider)
+        self.input_Nframes.editingFinished.connect(self.calc_tf)
+        
+        self.slider_Nframes = QSlider(Qt.Orientation.Horizontal)
+        self.slider_Nframes.setMinimum(1)
+        self.slider_Nframes.setMaximum(30)
+        self.slider_Nframes.valueChanged.connect(self.refresh_Nframes_text)
+        self.slider_Nframes.valueChanged.connect(self.calc_tf)
+        
+        self.label_Nframes_time = QLabel('')
+        
+        self.button_TFav = BlueButton('Calc TF average')
+        self.button_TFav.clicked.connect(self.calc_tf_av)
+        
+        
+        self.layout_tools_tf = QGridLayout()
+        self.layout_tools_tf.addWidget(boldLabel('Transfer Function:'),0,0,1,3)
+        self.layout_tools_tf.addWidget(QLabel('window:'),1,0,1,1)
+        self.layout_tools_tf.addWidget(self.input_list_window_tf,1,1,1,2)
+        self.layout_tools_tf.addWidget(QLabel('average:'),2,0,1,1)
+        self.layout_tools_tf.addWidget(self.input_list_average_TF,2,1,1,2)
+        self.layout_tools_tf.addWidget(self.label_Nframes,3,0,1,1)
+        self.layout_tools_tf.addWidget(self.input_Nframes,3,1,1,2)
+        self.layout_tools_tf.addWidget(self.slider_Nframes,4,0,1,3)
+        self.layout_tools_tf.addWidget(self.label_Nframes_time,5,0,1,3)
+        self.layout_tools_tf.addWidget(self.button_TF,6,0,1,3)
+        self.layout_tools_tf.addWidget(self.button_TFav,6,0,1,3)
+        
+        # initiate view
+        self.input_list_average_TF.setCurrentIndex(0)
+        self.input_Nframes.setText('1')
+        self.slider_Nframes.setValue(1)
+        self.label_Nframes.setVisible(False)
+        self.input_Nframes.setVisible(False)
+        self.slider_Nframes.setVisible(False)
+        self.label_Nframes_time.setVisible(False)
+        self.button_TFav.setVisible(False)
+        self.button_TF.setVisible(True)
+        
+        
+        self.frame_tools_tf = QFrame()
+        self.frame_tools_tf.setLayout(self.layout_tools_tf)
+        
+        
+    def setup_frame_tools_scaling(self):
+        self.input_iw_power = QLineEdit('0')
+        self.input_iw_power.setValidator(QIntValidator(0,2))
+        
+        self.button_xiw = BlueButton('x (iw)')
+        self.button_diw = BlueButton('x 1/(iw)')
+        self.button_xiw.clicked.connect(self.xiw)
+        self.button_diw.clicked.connect(self.diw)
+        
+        self.input_refset = QLineEdit('0')
+        self.input_refset.setValidator(QIntValidator(0,1000))
+        self.input_refchan = QLineEdit('0')
+        self.input_refchan.setValidator(QIntValidator(0,1000))
+
+        self.button_best_match = BlueButton('Best Match (to ref)')
+        self.button_best_match.clicked.connect(self.best_match)
+        self.button_undo_scaling = RedButton('Undo All Scaling')
+        self.button_undo_scaling.clicked.connect(self.undo_scaling)        
+        
+        self.layout_tools_scaling = QGridLayout()
+        self.layout_tools_scaling.addWidget(boldLabel('Calibration / Scaling:'),0,0,1,4)
+        self.layout_tools_scaling.addWidget(self.button_xiw,1,0,1,2)
+        self.layout_tools_scaling.addWidget(self.button_diw,1,2,1,2)
+        
+        self.layout_tools_scaling.addWidget(QLabel('Ref set / chan:'),2,0,1,2)
+        self.layout_tools_scaling.addWidget(self.input_refset,2,2,1,1)
+        self.layout_tools_scaling.addWidget(self.input_refchan,2,3,1,1)
+        
+        self.layout_tools_scaling.addWidget(self.button_best_match,3,0,1,4)
+        self.layout_tools_scaling.addWidget(self.button_undo_scaling,4,0,1,4)
+        
+        self.frame_tools_scaling = QFrame()
+        self.frame_tools_scaling.setLayout(self.layout_tools_scaling)
+        
+    def setup_frame_tools_mode_fitting(self):
+        self.input_freq_min2 = QLineEdit()
+        self.input_freq_min2.setValidator(QDoubleValidator(float(0),float(np.inf),5))
+        self.input_freq_min2.editingFinished.connect(self.freq_min2)
+        self.input_freq_max2 = QLineEdit()
+        self.input_freq_max2.setValidator(QDoubleValidator(float(0),float(np.inf),5))
+        self.input_freq_max2.editingFinished.connect(self.freq_max2)
+        
+        self.input_list_tf_type = newComboBox(['Acceleration','Velocity','Displacement'])
+        
+        self.button_fit_mode = GreenButton('Fit')
+        self.button_fit_mode.clicked.connect(self.fit_mode)
+        self.button_reject_mode = RedButton('Reject')
+        self.button_reject_mode.clicked.connect(self.reject_mode)
+        self.button_view_mode_summary = BlueButton('Summary')
+        self.button_view_mode_summary.clicked.connect(self.view_mode_summary)
+        self.button_view_modal_reconstruction = BlueButton('Reconstruction')
+        self.button_view_modal_reconstruction.clicked.connect(self.view_modal_reconstruction)
+        
+        self.layout_tools_mode_fitting = QGridLayout()
+        self.layout_tools_mode_fitting.addWidget(boldLabel('Mode Fitting:'),0,0,1,4)
+        self.layout_tools_mode_fitting.addWidget(QLabel('TF type:'),1,0,1,1)
+        self.layout_tools_mode_fitting.addWidget(self.input_list_tf_type,1,1,1,3)
+        
+        self.layout_tools_mode_fitting.addWidget(QLabel('Zoom to view a single peak:'),2,0,1,4)
+        self.layout_tools_mode_fitting.addWidget(QLabel('fmin:'),3,0,1,1)
+        self.layout_tools_mode_fitting.addWidget(self.input_freq_min2,3,1,1,3)
+        self.layout_tools_mode_fitting.addWidget(QLabel('fmax:'),4,0,1,1)
+        self.layout_tools_mode_fitting.addWidget(self.input_freq_max2,4,1,1,3)
+        self.layout_tools_mode_fitting.addWidget(self.button_fit_mode,5,0,1,2)
+        self.layout_tools_mode_fitting.addWidget(self.button_reject_mode,5,2,1,2)
+        self.layout_tools_mode_fitting.addWidget(self.button_view_mode_summary,6,0,1,4)
+        self.layout_tools_mode_fitting.addWidget(self.button_view_modal_reconstruction,7,0,1,4)
+        
+        self.frame_tools_mode_fitting = QFrame()
+        self.frame_tools_mode_fitting.setLayout(self.layout_tools_mode_fitting)
+        
+    def setup_frame_tools_settings(self):
+        
+        if self.settings is None:
+            self.settings = options.MySettings()
+            
+            
+        self.button_apply_settings = GreenButton('Apply Settings')
+        self.button_apply_settings.clicked.connect(self.apply_settings)
+        
+        self.button_show_available_devices = BlueButton('Show Available Devices')
+        self.button_show_available_devices.clicked.connect(self.show_available_devices)
+        
+        self.settings_dict = self.settings.__dict__
+        self.labels_settings = list(self.settings_dict.keys())
+        self.values_settings = list(self.settings_dict.values())
+        
+        self.input_settings = dict()
+        for (label,value) in self.settings_dict.items():
+            self.input_settings[label] = QLineEdit(str(value))
+        
+            
+        
+        NI = streams.get_devices_NI()
+        SC = streams.get_devices_soundcard()
+        
+        if NI == (None,None):
+            self.input_list_devices = []
+        else:
+            self.input_list_devices = ['nidaq']
+        if SC != None:
+            self.input_list_devices += ['soundcard']
+        
+        self.input_test_name = QLineEdit()
+        self.input_test_name.editingFinished.connect(self.refresh_test_name)
+        
+        self.layout_tools_settings = QFormLayout()
+        
+        self.layout_tools_settings.addWidget(boldLabel('Input Settings:'))
+        self.layout_tools_settings.addRow(QLabel('Test Name:'),self.input_test_name)
+        for n_row in range(9):
+            self.layout_tools_settings.addRow(QLabel(self.labels_settings[n_row]),self.input_settings[self.labels_settings[n_row]])
+        self.layout_tools_settings.addWidget(boldLabel('Output Settings:'))
+        for n_row in range(9,14):
+            self.layout_tools_settings.addRow(QLabel(self.labels_settings[n_row]),self.input_settings[self.labels_settings[n_row]])
+        
+        self.layout_tools_settings.addWidget(self.button_show_available_devices)
+        self.layout_tools_settings.addWidget(self.button_apply_settings)
+        self.frame_tools_settings = QFrame()
+        self.frame_tools_settings.setLayout(self.layout_tools_settings)
+        
+    def setup_frame_tools_generate_output(self):
+        self.list_output_options = ['None','sweep','gaussian','uniform']
+        self.input_output_options = newComboBox(self.list_output_options)
+        self.input_output_options.currentTextChanged.connect(self.update_output)
+        
+        self.input_output_amp = QLineEdit('0')
+        v = QDoubleValidator(0.0,1.0,5)
+        v.setNotation(QDoubleValidator.Notation.StandardNotation)
+        self.input_output_amp.setValidator(v)
+        
+        self.input_output_f1 = QLineEdit('0')
+        self.input_output_f1.setValidator(QDoubleValidator(0.0,float(np.inf),5))
+        
+        self.input_output_f2 = QLineEdit('0')
+        self.input_output_f2.setValidator(QDoubleValidator(0.0,float(np.inf),5))
+        
+        self.input_output_duration = QLineEdit(str(self.settings.stored_time))
+        self.input_output_duration.setValidator(QDoubleValidator(0.0,float(np.inf),5))
+        
+        self.button_output_preview = BlueButton('Preview Output')
+        self.button_output_preview.clicked.connect(self.preview_output)
+        
+        self.button_start_output = BlueButton('Start Output')
+        self.button_start_output.clicked.connect(self.start_output)
+        
+        self.button_log_with_output = GreenButton('Log with Output')
+        self.button_log_with_output.clicked.connect(self.button_clicked_log_data)
+        
+        
+        self.input_test_name2 = QLineEdit()
+        self.input_test_name2.editingFinished.connect(self.refresh_test_name2)
+        
+        self.layout_tools_generate_output = QFormLayout()
+        
+        self.layout_tools_generate_output.addRow(boldLabel('Generate Outputs:'))
+        self.layout_tools_generate_output.addRow(QLabel('Test Name:'),self.input_test_name2)
+        self.layout_tools_generate_output.addRow(QLabel('Type:'),self.input_output_options)
+        self.layout_tools_generate_output.addRow(QLabel('Amplitude (0-1):'),self.input_output_amp)
+        self.layout_tools_generate_output.addRow(QLabel('f1 (Hz):'),self.input_output_f1)
+        self.layout_tools_generate_output.addRow(QLabel('f2 (Hz):'),self.input_output_f2)
+        self.layout_tools_generate_output.addRow(QLabel('Duration (s):'),self.input_output_duration)
+        self.layout_tools_generate_output.addRow(self.button_output_preview)
+        self.layout_tools_generate_output.addRow(self.button_start_output)
+        self.layout_tools_generate_output.addRow(self.button_log_with_output)
+        
+        self.frame_tools_generate_output = QFrame()
+        self.frame_tools_generate_output.setLayout(self.layout_tools_generate_output)
+        
+    
+    def setup_frame_tools_edit_dataset(self):
+        self.list_data_type = ['Time Data','FFT Data','TF Data','Modal Data','Sono Data']
+        
+        self.input_list_data_type = newComboBox(self.list_data_type)
+        self.input_list_data_type.setCurrentText('Time Data')
+        self.input_list_data_type.currentIndexChanged.connect(self.update_selected_set)
+        
+        self.button_delete_data_type = RedButton('Delete all data of this type')
+        self.button_delete_data_type.clicked.connect(self.delete_data_type)
+        
+        self.button_delete_data_set = OrangeButton('Delete Selected Set')
+        self.button_delete_data_set.clicked.connect(self.delete_data_set)
+        
+        self.input_selected_set = QLineEdit()
+        self.input_selected_set.setValidator(QIntValidator(0,1000))
+
+        self.button_log_replace = GreenButton('Log && Replace Selected Set')
+        self.button_log_replace.clicked.connect(self.log_and_replace)
+        
+        text = self.dataset.__repr__()
+        self.label_data_summary = QLabel(text)
+        
+        self.layout_tools_edit_dataset = QGridLayout()
+        self.layout_tools_edit_dataset.addWidget(boldLabel('Dataset Summary'),0,0,1,4)
+        self.layout_tools_edit_dataset.addWidget(self.label_data_summary,1,0,1,4)
+        self.layout_tools_edit_dataset.addWidget(boldLabel('Edit Dataset'),2,0,1,4)
+        self.layout_tools_edit_dataset.addWidget(QLabel('Selected Type:'),3,0,1,2)
+        self.layout_tools_edit_dataset.addWidget(self.input_list_data_type,3,2,1,2)
+        self.layout_tools_edit_dataset.addWidget(self.button_delete_data_type,4,0,1,4)
+        self.layout_tools_edit_dataset.addWidget(QLabel('Selected Set:'),5,0,1,2)
+        self.layout_tools_edit_dataset.addWidget(self.input_selected_set,5,2,1,2)
+        self.layout_tools_edit_dataset.addWidget(self.button_delete_data_set,6,0,1,4)
+        self.layout_tools_edit_dataset.addWidget(self.button_log_replace,7,0,1,4)
+        
+        self.frame_tools_edit_dataset = QFrame()
+        self.frame_tools_edit_dataset.setLayout(self.layout_tools_edit_dataset)
+        
+    def setup_frame_tools_sonogram(self):
+        self.input_sono_N_frames = QLineEdit('50')
+        self.input_sono_N_frames.setValidator(QIntValidator(10,10000))
+        self.input_sono_N_frames.editingFinished.connect(self.refresh_sono_N_frames_slider)
+        self.input_sono_N_frames.editingFinished.connect(self.calc_sono)
+        
+        self.slider_sono_N_frames = QSlider(Qt.Orientation.Horizontal)
+        self.slider_sono_N_frames.setMinimum(10)
+        self.slider_sono_N_frames.setMaximum(500)
+        self.slider_sono_N_frames.setValue(50)
+        self.slider_sono_N_frames.valueChanged.connect(self.refresh_sono_N_frames_text)
+        self.slider_sono_N_frames.valueChanged.connect(self.calc_sono)
+        
+        self.input_sono_n_set = QLineEdit('0')
+        self.input_sono_n_set.setValidator(QIntValidator(0,1000))
+        self.input_sono_n_set.editingFinished.connect(self.calc_sono)
+        self.input_sono_n_chan = QLineEdit('0')
+        self.input_sono_n_chan.setValidator(QIntValidator(0,1000))
+        self.input_sono_n_chan.editingFinished.connect(self.calc_sono)
+        
+        self.input_db_range = QLineEdit('60')
+        self.input_db_range.setValidator(QIntValidator(1,200))
+        self.input_db_range.editingFinished.connect(self.calc_sono)
+        
+        self.sono_info = QLabel('')
+        
+        
+        self.button_calc_sono = BlueButton('Calc Sonogram')
+        self.button_calc_sono.clicked.connect(self.calc_sono)
+        
+        self.layout_tools_sonogram = QGridLayout()
+        self.layout_tools_sonogram.addWidget(boldLabel('Calculate Sonogram:'),0,0,1,4)
+        self.layout_tools_sonogram.addWidget(QLabel('N frames:'),1,0,1,2)
+        self.layout_tools_sonogram.addWidget(self.input_sono_N_frames,1,2,1,2)
+        self.layout_tools_sonogram.addWidget(self.slider_sono_N_frames,2,0,1,4)
+        self.layout_tools_sonogram.addWidget(self.sono_info,3,0,1,4)
+        self.layout_tools_sonogram.addWidget(QLabel('Dynamic Range (dB):'),4,0,1,2)
+        self.layout_tools_sonogram.addWidget(self.input_db_range,4,2,1,2)
+        self.layout_tools_sonogram.addWidget(QLabel('Set / Chan:'),5,0,1,2)
+        self.layout_tools_sonogram.addWidget(self.input_sono_n_set,5,2,1,1)
+        self.layout_tools_sonogram.addWidget(self.input_sono_n_chan,5,3,1,1)
+        self.layout_tools_sonogram.addWidget(self.button_calc_sono,6,0,1,4)
+        
+        self.frame_tools_sonogram = QFrame()
+        self.frame_tools_sonogram.setLayout(self.layout_tools_sonogram)
+        
+    def setup_frame_tools_save_export(self):
+        #self.button_import_matlab_jwlogger = BlueButton('Import from JW Logger')
+        #self.button_import_matlab_jwlogger.clicked.connect(self.import_jwlogger)
+        
+        self.button_export_matlab_jwlogger = BlueButton('Export to JW Logger')
+        self.button_export_matlab_jwlogger.clicked.connect(self.export_jwlogger)
+        
+        self.button_export_matlab = BlueButton('Export to Matlab')
+        self.button_export_matlab.clicked.connect(self.export_matlab)
+        
+        self.button_export_csv = BlueButton('Export to CSV')
+        self.button_export_csv.clicked.connect(self.export_csv)
+        
+        
+        self.layout_tools_save_export = QVBoxLayout()
+        #self.layout_tools_save_export.addWidget(self.button_import_matlab_jwlogger)
+        self.layout_tools_save_export.addWidget(self.button_export_matlab_jwlogger)
+        self.layout_tools_save_export.addWidget(self.button_export_matlab)
+        self.layout_tools_save_export.addWidget(self.button_export_csv)
+        
+        self.frame_tools_save_export = QFrame()
+        self.frame_tools_save_export.setLayout(self.layout_tools_save_export)
+        
+        
+    def update_frame_tools(self):
+        self.frame_tools.setLayout(self.layout_tools)
+
+
+    #%% INTERACTION FUNCTIONS
+    
+    def show(self):
+        # allow logger to be opened again after closing
+        # self.window.showMinimized()
+        self.window.show()
+        self.window.showNormal()
+        self.window.raise_()
+        
+        app.exec()
+        
+        
+    def close(self):
+        # allow logger to be closed programmatically
+        self.window.close()
+    
+    def start_stream(self):
+        if self.settings != None:
+            try:
+                streams.start_stream(self.settings)
+                self.rec = streams.REC
+            except:
+                self.rec = None
+                message = 'Data stream can\'t be initialised.\n'
+                message += 'Possible reasons: sounddevice or PyDAQmx not installed, or acquisition hardware not connected.\n' 
+                message += 'Please note that it won\'t be possible to log data.'
+                self.show_message(message)
+                
+        else:
+            message = 'To enable data acquisition, please use \'Logger Settings\' tool.'
+            self.show_message(message)
+#            self.input_list_tools.setCurrentIndex(1)
+            self.select_view()
+
+    def show_message(self,message,b='ok'):
+        # if multiple messages from different functions, then join them up
+        time_since_last = time.time()-self.message_time
+        if (time_since_last < 0.5) and (message not in self.message):# and (self.message not in message):
+            self.message += message # join messages if not duplicating
+        else:
+            self.message = message
+        self.message_time = time.time()
+        
+#        if (message not in self.message) and (self.message not in message):
+#            self.message += message # join messages if not duplicating
+#        else:
+#            self.message = message
+        if message != '':
+            self.label_message.setText(self.message)
+            if b == 'ok':
+                self.button_message.setVisible(True)
+                self.button_cancel.setVisible(False)
+                self.button_undo.setVisible(False)
+            elif b == 'cancel':
+                self.button_message.setVisible(False)
+                self.button_cancel.setVisible(True)
+                self.button_undo.setVisible(False)
+            elif b == 'undo':
+                self.button_message.setVisible(True)
+                self.button_cancel.setVisible(False)
+                self.button_undo.setVisible(True)
+                
+            self.frame_message.setVisible(True)
+        
+        
+    def hide_message(self):
+        self.label_message.setText('')
+        self.message = ''
+        modal.MESSAGE = ''
+        self.frame_message.setVisible(False)
+      
+    def show_message_timer(self):
+        message = acquisition.MESSAGE
+#        message += self.rec.MESSAGE
+        self.show_message(message,b='cancel')
+    
+    def check_stream(self):
+        if streams.REC is None:
+            self.levels_timer.stop()
+            self.window.setWindowTitle('Logger')
+        else:
+            self.levels_timer.start()
+    
+    def show_levels(self):
+        if streams.REC is not None:
+            max_levels = np.max(np.abs(self.rec.osc_time_data),axis=0)
+            ch_max = np.argmax(max_levels)
+            max_levels_all = max_levels[ch_max]
+            W = 20
+            N = int(np.round(max_levels_all*W))
+            display_text = N*'-' + '>|' + (W-N)*'-' + '] in ch ' + str(ch_max)
+            if max_levels_all > 0.99:
+                display_text += ' *** WARNING CLIPPED ***'
+                self.t0_clipped = time.time()
+            elif (max_levels_all < 0.99) and ((time.time()-self.t0_clipped) < 1):
+                display_text += ' *** WARNING CLIPPED ***'
+            
+                
+            self.window.setWindowTitle('Logger | Max Level: [' + display_text)
+        
+    
+    def button_clicked_osc(self):
+        # launch oscilloscope
+        self.osc = Oscilloscope(self.settings)
+
+
+    def button_clicked_log_data(self):
+        # delegate messages to acquisition global MESSAGE, and streams rec.MESSAGE
+        # this lets messages be seen from within logging thread, with live updates
+        self.message_timer.start(300) 
+        
+        # start stream
+        if self.rec is None:
+            self.start_stream()
+            
+        # generate output if specified
+        self.create_output_signal()
+        if self.output_time_data is not None:
+            y = self.output_time_data.time_data
+            # warn if amplitude set too high
+            if np.any(np.abs(y)>1):
+                message = 'Output amplitude too high: must be less than 1.\n'
+                self.show_message(message)
+                return None
+        else:
+            y = None
+
+        
+        
+        # reset trigger
+        self.rec.trigger_detected = False # but need to do this again inside acquisition
+        self.button_log_data.setStyleSheet("background-color: white")
+        
+#        # show message re trigger
+#        if self.settings.pretrig_samples is None:
+#            message = 'Logging data for {} seconds'.format(self.settings.stored_time)
+#        else:
+            #message = 'Logging data for {} seconds, with trigger.\n'.format(self.settings.stored_time)
+            
+            
+        
+        
+#        # show message re output
+#        if y is not None:
+#            message += '\n\nOutput signal starting.'
+#            self.show_message(message) # this one 
+        
+        
+        self.thread = LogDataThread(self.settings,test_name=self.test_name, rec=self.rec, output=y)
+        #self.thread.setPriority(QThread.TimeCriticalPriority)
+#        self.show_message(message,'cancel')
+        
+        self.thread.start()
+        self.thread.s.connect(self.add_logged_data)
+        
+        
+    def add_logged_data(self,d):
+        
+        if self.flag_log_and_replace == False:
+            self.dataset.add_to_dataset(d.time_data_list)
+            N = len(self.dataset.time_data_list)
+            self.sets = [N-1]
+            # this doesn't make it through from acquisition.MESSAGE because polling stops first
+            message = 'Logging complete.\n'
+            if np.any(np.abs(d.time_data_list[0].time_data) > 0.95):
+                message += '\nWARNING: Data may be clipped.\n'
+            self.show_message(message)
+#            message = ''
+#            self.hide_message()
+        else:
+            self.dataset.replace_data_item(d.time_data_list[0],self.selected_set)
+            self.sets = [self.selected_set]
+            self.last_action = 'data replaced'
+            # this doesn't make it through from acquisition.MESSAGE because polling stops first
+            message = 'Logged data replaced set {}.\n'.format(self.selected_set)
+            if np.any(np.abs(d.time_data_list[0].time_data) > 0.95):
+                message += '\nWARNING: Data may be clipped.\n'
+            self.show_message(message,b='undo')
+            self.flag_log_and_replace = False
+
+        
+        # update figure then update selection
+        self.channels = 'all'
+        self.switch_view('Time Data') # need to switch to time and update plot so that get_selected_chans picks up new data
+        
+        # only show most recently logged data
+        selection = self.p.get_selected_channels()
+        for ns in range(len(selection)):
+            for nc in range(len(selection[ns])):
+                if ns in self.sets:
+                    selection[ns][nc] = True
+                else:
+                    selection[ns][nc] = False
+        self.selected_channels = selection
+        
+        # update with final selection and make -1 to 1, change button back to green
+        self.auto_xy = 'x'
+        self.update_figure()
+        self.p.ax.set_ylim([-1,1])
+        self.button_log_data.setStyleSheet('background-color: hsv(120, 170, 255)')
+        self.message_timer.stop()
+        
+        
+    def cancel_logging(self):
+        self.thread.terminate() # stop thread
+        streams.start_stream(self.settings) # reset stream
+        self.rec = streams.REC # reset stream
+        self.show_message('Logging cancelled')
+        self.button_log_data.setStyleSheet('background-color: hsv(120, 170, 255)')
+        self.message_timer.stop() # stop acquisition messages
+        self.selected_channels = self.p.get_selected_channels()
+
+    def delete_last_data(self):
+        self.dataset_backup = copy.deepcopy(self.dataset)
+        self.dataset.remove_last_data_item('TimeData')
+        self.dataset.freq_data_list = datastructure.FreqDataList()
+        self.dataset.tf_data_list = datastructure.TfDataList()
+        N = len(self.dataset.time_data_list)
+        self.sets = [N-1]
+        self.channels = 'all'
+        
+        # only show most recently logged data
+        if N > 0:
+            selection = self.p.get_selected_channels()
+            for ns in range(len(selection)):
+                for nc in range(len(selection[ns])):
+                    if ns in self.sets:
+                        selection[ns][nc] = True
+                    else:
+                        selection[ns][nc] = False
+            self.selected_channels = selection
+        
+        self.auto_xy = 'x'
+        self.update_figure()
+        self.p.ax.set_ylim([-1,1])
+#        self.auto_xy = ''
+#        self.p.update(self.dataset.time_data_list,sets=[N-1],channels='all', auto_xy=self.auto_xy)
+#        update(self,data_list,sets='all',channels='all',xlinlog='linear',show_coherence=True,plot_type=None,coherence_plot_type='linear',freq_range=None, auto_xy='xyc'):
+        self.switch_view('Time Data')
+        self.last_action = 'delete data'
+        message = 'Last logged time data deleted.\n'
+        message += 'FFT and TF data also deleted.\n'
+        message += 'For more data editing options select ''Edit Dataset'' tool.'
+        self.show_message(message,b='undo')
+#        self.selected_channels = self.p.get_selected_channels()
+#        self.update_selected_set()
+        
+    def reset_data(self):
+        self.dataset_backup = copy.deepcopy(self.dataset)
+        self.dataset = datastructure.DataSet()
+        N = len(self.dataset.time_data_list)
+        self.p.update(self.dataset.time_data_list,sets=[N-1],channels='all')
+        self.switch_view('Time Data')
+        self.last_action = 'delete data'
+        message = 'All data deleted.\n'
+        message += 'For more data editing options select ''Edit Dataset'' tool.'
+        self.show_message(message,b='undo')
+#        self.selected_channels = self.p.get_selected_channels()
+#        self.update_selected_set()
+
+    
+    def load_data(self):
+        
+        d = file.load_data(parent=self.window)
+        
+        if d is not None:
+            d = datastructure.update_dataset(d) # updates data saved using previous logger versions
+            self.dataset.add_to_dataset(d.time_data_list)
+            self.dataset.add_to_dataset(d.freq_data_list)
+            self.dataset.add_to_dataset(d.tf_data_list)
+            self.dataset.add_to_dataset(d.cross_spec_data_list)
+            self.dataset.add_to_dataset(d.sono_data_list)
+            self.dataset.add_to_dataset(d.meta_data_list)
+            self.dataset.add_to_dataset(d.modal_data_list)
+            
+        else:
+            message = 'No data loaded'
+            self.show_message(message)
+            return None
+    
+        
+        no_data = True
+        self.auto_xy = 'xyc'
+        if len(d.time_data_list) != 0:
+            self.input_list_figures.setCurrentText('Time Data')
+            self.select_view()
+#            self.hide_message()
+            no_data = False
+        if len(d.freq_data_list) != 0:
+            self.input_list_figures.setCurrentText('FFT Data')
+            self.select_view()
+#            self.hide_message()
+            no_data = False
+        if len(d.tf_data_list) != 0:
+            self.input_list_figures.setCurrentText('TF Data')
+            self.select_view()
+#            self.hide_message()
+            no_data = False
+        if no_data == True:
+            message = 'No data to view'
+            self.show_message(message)
+        self.input_list_data_type.setCurrentText(self.selected_view)
+        self.select_all_data()
+        self.selected_channels = self.p.get_selected_channels()
+#        self.update_selected_set()
+        
+        
+        
+            
+    def save_data(self):
+        filename = self.dataset.save_data()
+        if filename is not None:
+            message = 'Saved dataset:\n\n'
+            message += self.dataset.__repr__()
+            message += '\n\n'
+            message += 'to file '
+            message += filename
+        else:
+            message = 'Save dataset cancelled'
+        self.show_message(message)
+            
+    def save_fig(self):
+        if self.plot_type == 'Nyquist':
+            filename = file.save_fig(self.p,figsize=(9,9))
+        else:
+            filename = file.save_fig(self.p,figsize=(9,5))
+        if filename is not None:
+            message = 'Saved current figure to file:\n'
+            message += filename
+        else:
+            message = 'Save figure cancelled'
+        self.canvas.draw()
+        self.show_message(message)
+
+    def xmin(self):
+        xmin = float(self.input_axes[0].text())
+        xlim = self.p.ax.get_xlim()
+        self.p.ax.set_xlim([xmin,xlim[1]])
+        if ((self.current_view == 'TF Data') or (self.current_view == 'FFT Data')) and (self.plot_type != 'Nyquist'):
+            self.freq_range = list(self.p.ax.get_xlim())
+        self.canvas.draw()
+        
+    def xmax(self):
+        xmax = float(self.input_axes[1].text())
+        xlim = self.p.ax.get_xlim()
+        self.p.ax.set_xlim([xlim[0],xmax])
+        if ((self.current_view == 'TF Data') or (self.current_view == 'FFT Data')) and (self.plot_type != 'Nyquist'):
+            self.freq_range = list(self.p.ax.get_xlim())
+        self.canvas.draw()
+        
+    def ymin(self):
+        ymin = float(self.input_axes[2].text())
+        ylim = self.p.ax.get_ylim()
+        self.p.ax.set_ylim([ymin,ylim[1]])
+        self.canvas.draw()
+        
+    def ymax(self):
+        ymax = float(self.input_axes[3].text())
+        ylim = self.p.ax.get_ylim()
+        self.p.ax.set_ylim([ylim[0],ymax])
+        self.canvas.draw()
+        
+    def auto_x(self):
+#        self.auto_xy = 'x'
+#        self.update_figure()
+        self.p.auto_x()
+        
+    def auto_y(self):
+#        self.auto_xy = 'yc'
+#        self.update_figure()
+        self.p.auto_y()
+        
+    def update_axes_values(self,axes):
+#        self.selected_channels = self.p.get_selected_channels()
+        
+        xlim = self.p.ax.get_xlim()
+        ylim = self.p.ax.get_ylim()
+        self.input_axes[0].setText('{:0.5g}'.format(xlim[0]))
+        self.input_axes[1].setText('{:0.5g}'.format(xlim[1]))
+        self.input_axes[2].setText('{:0.5g}'.format(ylim[0]))
+        self.input_axes[3].setText('{:0.5g}'.format(ylim[1]))
+        if ((self.current_view == 'TF Data') or (self.current_view == 'FFT Data')) and (self.plot_type != 'Nyquist'):
+            self.freq_range = list(xlim)
+            self.input_freq_min2.setText('{:0.5g}'.format(xlim[0]))
+            self.input_freq_max2.setText('{:0.5g}'.format(xlim[1]))
+        
+                
+    def update_modal_message(self,axes):
+        # only connected to x-axis
+        if (self.current_view == 'TF Data') and (len(self.dataset.modal_data_list) > 0) and (self.selected_tool == 'Mode Fitting') and (modal.MESSAGE == ''):
+            # Show message to highlight modal fit, to allow removing or replacing a given fit
+            fn_all = self.dataset.modal_data_list[0].M[:,0]
+            self.fn_in_range = fn_all[(fn_all > self.freq_range[0]) & (fn_all < self.freq_range[1])]
+            if len(self.fn_in_range) > 1:
+                message = 'A total of {} modes have been fitted within this frequency range so far:\n\n'.format(len(self.fn_in_range))
+                message += 'Fitted mode frequencies = {} (Hz)\n\n'.format(np.array2string(self.fn_in_range,precision=2))
+                message += 'To delete all of these modal fits, press ''Reject Mode''.'
+                self.show_message(message)
+            elif len(self.fn_in_range) == 1:
+                message = 'One mode has been fitted within this frequency range:\n\n'
+                message += 'Fitted mode frequency = {} Hz\n\n'.format(np.array2string(self.fn_in_range,precision=2))
+                message += 'To replace this mode fit with a new fit, press ''Fit Mode''.\n'
+                message += 'To delete this mode fit, press ''Reject Mode''.'
+                self.show_message(message)
+            else:
+                self.hide_message()
+        
+    def legend_left(self):
+        self.legend_loc = 'lower left'
+        self.p.update_legend(self.legend_loc)
+        self.canvas.draw()
+        
+    def legend_right(self):
+        self.legend_loc = 'lower right'
+        self.p.update_legend(self.legend_loc)
+        self.canvas.draw()
+            
+    def legend_onoff(self):
+        self.selected_channels = self.p.get_selected_channels()
+        visibility = self.p.ax.get_legend().get_visible()
+        self.p.ax.get_legend().set_visible(not visibility)
+        self.canvas.draw()
+        
+        
+    def update_figure(self):
+        # get current status of axes for case auto_xy=''
+        xlim = self.p.ax.get_xlim()
+        ylim = self.p.ax.get_ylim()
+            
+        try:
+            # sometimes starting point with no legend object
+            visibility = self.p.ax.get_legend().get_visible()
+        except:
+            pass
+        # updates the currently viewed plot
+        if self.current_view == 'Time Data':
+            data_list = self.dataset.time_data_list
+        elif self.current_view == 'FFT Data':
+            data_list = self.dataset.freq_data_list
+        elif self.current_view == 'TF Data':
+            data_list = self.dataset.tf_data_list
+        elif self.current_view == 'Sono Data':
+            data_list = self.dataset.sono_data_list
+            
+        if self.current_view == 'Sono Data':
+            if self.current_view_changed == True:
+                auto_xy = 'xy'
+            else:
+                auto_xy=''
+                
+            n_set = int(self.input_sono_n_set.text())
+            n_chan = int(self.input_sono_n_chan.text())
+            db_range = int(self.input_db_range.text())
+            self.p.update_sonogram(self.dataset.sono_data_list, n_set, n_chan, db_range=db_range,auto_xy=auto_xy)
+            self.label_figure.setText(self.selected_view + ': Set {}, Channel {}'.format(n_set,n_chan))
+        else:
+            self.p.update(data_list, sets=self.sets, channels=self.channels, xlinlog=self.xlinlog,show_coherence=self.show_coherence,plot_type=self.plot_type,coherence_plot_type=self.coherence_plot_type,freq_range=self.freq_range,auto_xy=self.auto_xy)
+            self.label_figure.setText(self.selected_view)
+        if self.current_view_changed == False:
+            try:
+                # not robust as not consistent in keeping up to date
+                # if only one data set then make sure it's visible
+                if len(data_list) == 1:
+                    selection = self.p.get_selected_channels()
+                    for nc in range(len(selection[0])):
+                        selection[0][nc] = True
+                    self.selected_channels = selection
+                # otherwise just inherit prev data selection
+                self.p.set_selected_channels(self.selected_channels)
+                self.p.ax.get_legend().set_visible(visibility)
+                self.fig.canvas.draw()
+            except:
+                # get selected_channels back into sync
+                pass# not sure helping. self.selected_channels = self.p.get_selected_channels()
+        if self.auto_xy=='':
+            # handle this case manually
+            self.p.ax.set_xlim(xlim)
+            self.p.ax.set_ylim(ylim)
+            self.p.fig.canvas.draw()
+
+        self.selected_channels = self.p.get_selected_channels()
+                   
+    def update_selected_channels(self,_):
+        # keeps selected_channels in sync with legend picking
+        self.selected_channels = self.p.get_selected_channels()
+        
+    def select_all_data(self):
+        if len(self.p.ax.lines) > 0:
+            for line in self.p.ax.lines:
+                line.set_alpha(plotting.LINE_ALPHA)
+            for line in self.p.legend.get_lines():
+                line.set_alpha(plotting.LINE_ALPHA)
+            self.canvas.draw()
+        else:
+            message = 'No data to show.\n'
+            self.show_message(message)
+        self.selected_channels = self.p.get_selected_channels()
+        
+        
+        
+    def select_no_data(self):
+        if len(self.p.ax.lines) > 0:
+            for line in self.p.ax.lines:
+                line.set_alpha(1-plotting.LINE_ALPHA)
+            for line in self.p.legend.get_lines():
+                line.set_alpha(1-plotting.LINE_ALPHA)
+            self.canvas.draw()
+        else:
+            message = 'No data to hide.\n'
+            self.show_message(message)
+        self.selected_channels = self.p.get_selected_channels()
+            
+    def show_set_only(self):
+        n_set = int(self.input_select_set_only.text())
+        selection = self.p.get_selected_channels()
+        for ns in range(len(selection)):
+            for nc in range(len(selection[ns])):
+                if ns == n_set:
+                    selection[ns][nc] = True
+                else:
+                    selection[ns][nc] = False
+        self.p.set_selected_channels(selection)
+        self.selected_channels = selection
+        
+    def show_chan_only(self):
+        n_chan = int(self.input_select_chan_only.text())
+        selection = self.p.get_selected_channels()
+        for ns in range(len(selection)):
+            for nc in range(len(selection[ns])):
+                if nc == n_chan:
+                    selection[ns][nc] = True
+                else:
+                    selection[ns][nc] = False
+        self.p.set_selected_channels(selection)
+        self.selected_channels = selection
+        
+    def next_chans(self):
+        try:
+            # sometimes starting point with no legend object
+            visibility = self.p.ax.get_legend().get_visible()
+        except:
+            pass
+        
+        selection = self.p.get_selected_channels()
+        prev_line = bool(selection[-1][-1])
+        for ns in range(len(selection)):
+            for nc in range(len(selection[ns])):
+                this_line = bool(selection[ns][nc])
+                selection[ns][nc] = bool(prev_line)
+                prev_line = bool(this_line)
+        
+        self.p.set_selected_channels(selection)
+        self.selected_channels = selection
+        try:
+            self.p.ax.get_legend().set_visible(visibility)
+            self.fig.canvas.draw()
+        except:
+            pass
+        
+    def prev_chans(self):
+        try:
+            # sometimes starting point with no legend object
+            visibility = self.p.ax.get_legend().get_visible()
+        except:
+            pass
+        selection = self.p.get_selected_channels()
+        prev_line = bool(selection[0][0])
+        for ns in reversed(range(len(selection))):
+            for nc in reversed(range(len(selection[ns]))):
+                this_line = bool(selection[ns][nc])
+                selection[ns][nc] = bool(prev_line)
+                prev_line = bool(this_line)
+        
+        self.p.set_selected_channels(selection) 
+        self.selected_channels = selection
+        try:
+            self.p.ax.get_legend().set_visible(visibility)
+            self.fig.canvas.draw()
+        except:
+            pass
+
+           
+        
+    def co_min(self):
+        co_min = float(self.input_co_min.text())
+        ylim = self.p.ax2.get_ylim()
+        self.p.ax2.set_ylim([co_min,ylim[1]])
+        self.canvas.draw()
+    
+    def co_max(self):
+        co_max = float(self.input_co_max.text())
+        ylim = self.p.ax2.get_ylim()
+        self.p.ax2.set_ylim([ylim[0],co_max])
+        self.canvas.draw()
+        
+    def freq_min(self):
+        self.freq_range[0] = float(self.input_freq_min.text())
+        self.input_freq_min2.setText(str(self.freq_range[0]))
+        self.update_figure()
+#        self.p.update(self.dataset.tf_data_list, xlinlog=self.xlinlog, show_coherence=self.show_coherence,plot_type=self.plot_type,coherence_plot_type=self.coherence_plot_type,freq_range=self.freq_range,auto_xy=self.auto_xy)
+        
+    def freq_max(self):
+        self.freq_range[1] = float(self.input_freq_max.text())
+        self.input_freq_max2.setText(str(self.freq_range[1]))
+        self.update_figure()
+#        self.p.update(self.dataset.tf_data_list, xlinlog=self.xlinlog, show_coherence=self.show_coherence,plot_type=self.plot_type,coherence_plot_type=self.coherence_plot_type,freq_range=self.freq_range,auto_xy=self.auto_xy)
+        
+    def update_co_axes_values(self,axes):
+        ylim = self.p.ax2.get_ylim()
+        self.input_co_min.setText('{:0.5g}'.format(ylim[0]))
+        self.input_co_max.setText('{:0.5g}'.format(ylim[1]))
+        
+    def data_toggle(self):
+        self.show_data = not self.show_data
+        self.select_view()
+        for line in self.p.ax.lines:
+            line.set_visible(self.show_data)
+        if self.show_data == False:
+            self.p.ax.set_ylabel('')
+            self.p.ax.set_yticks([])
+        else:
+            self.p.ax.yaxis.set_major_locator(AutoLocator())
+            
+        self.canvas.draw()
+
+    def coherence_toggle(self):
+        self.show_coherence = not self.show_coherence
+        self.select_view()
+                
+        
+    def select_xlinlog(self):
+        if self.xlinlog == 'linear':
+            self.xlinlog = 'log' # or symlog
+        else:
+            self.xlinlog = 'linear'
+        
+        self.update_figure()
+    
+    def switch_view(self,new_view_text):
+        index = self.input_list_figures.findText(new_view_text, Qt.MatchFlag.MatchFixedString)
+        if self.input_list_figures.itemText(index) == 'Time Data':
+            N = len(self.dataset.time_data_list)
+        elif self.input_list_figures.itemText(index) == 'FFT Data':
+            N = len(self.dataset.freq_data_list)
+        elif self.input_list_figures.itemText(index) == 'TF Data':
+            N = len(self.dataset.tf_data_list)
+        elif self.input_list_figures.itemText(index) == 'Sono Data':
+            N = len(self.dataset.sono_data_list)
+        if N > 0:
+            self.input_list_figures.setCurrentIndex(index)
+            self.input_list_data_type.setCurrentText(self.input_list_figures.currentText())
+            
+        self.select_view()
+        
+    def select_view(self):
+        # handles logic of what to show in gui depending on selected view options
+        ci = self.input_list_figures.currentIndex()
+        self.selected_view = self.input_list_figures.itemText(ci)
+        
+        if self.current_view == self.selected_view:
+            self.current_view = np.copy(self.selected_view)
+            self.current_view_changed = False
+            self.plot_type_before = np.copy(self.plot_type)
+            self.plot_type = self.items_list_plot_type[self.input_list_plot_type.currentIndex()]
+            self.switch_to_nyquist = (self.plot_type == 'Nyquist') and ('Nyquist' != self.plot_type_before)
+            self.switch_from_nyquist = (self.plot_type_before == 'Nyquist') and ('Nyquist' != self.plot_type)
+#            self.selected_channels = self.p.get_selected_channels()
+        else:
+            self.current_view_changed = True
+        
+        # Time Data
+        if self.selected_view == 'Time Data':
+            ### set to time gui
+            N = len(self.dataset.time_data_list)
+            # check if any data present to display
+            if N != 0:
+                # no plot details needed for time display
+                self.hide_plot_details()
+                # reset data/coherence plot properties if changed view back to time
+                if self.current_view_changed:
+                    self.current_view = self.selected_view
+                    self.show_data = True
+                    self.show_coherence = True # won't plot but reests for other selections
+                    self.xlinlog = 'linear'
+                    self.auto_xy = 'xyc'
+                    self.plot_type = 'Amplitude (dB)'# - can trigger this to be called again
+                    self.input_list_plot_type.setCurrentText(self.plot_type)
+                else:
+                    self.auto_xy = ''
+                    
+                # plot
+                self.update_figure()
+                
+            # show message if no data
+            else:
+                message = 'No time data to display.\n'
+                self.show_message(message)
+                
+        # FFT Data
+        elif self.selected_view == 'FFT Data':
+            N = len(self.dataset.freq_data_list)
+            # check if freq data exists
+            if N != 0:
+                # if main view changed reset plot properties
+                if self.current_view_changed:
+                    self.current_view = self.selected_view
+                    self.show_data = True
+                    self.show_coherence = True # won't plot but reests for other selections
+                    self.auto_xy = 'xyc'
+                    self.plot_type = 'Amplitude (dB)'
+                    self.input_list_plot_type.setCurrentText(self.plot_type)
+                    
+                
+                # if staying as FFT plot but changing to nyquist then switch to FFT Nyquist toolset
+                elif self.switch_to_nyquist == True:
+                    # get properties before switch so can go back to this view
+                    self.freq_range = list(self.p.ax.get_xlim()) #force to list instead of tuple
+                    self.show_coherence_before = self.show_coherence
+                    self.show_coherence = False
+                    self.xlinlog_before = self.xlinlog
+                    # linear x axis for nyquist
+                    self.xlinlog = 'linear'
+                    # update freq range text
+                    self.input_freq_min.setText('{:5f}'.format(self.freq_range[0]))
+                    self.input_freq_max.setText('{:5f}'.format(self.freq_range[1]))
+                    self.auto_xy = 'xy'
+                    
+                    
+                # if moving from nyquist back, reset properties to previous
+                elif self.switch_from_nyquist == True:
+                    self.show_coherence = self.show_coherence_before
+                    self.xlinlog = self.xlinlog_before
+                    # freq range already set above as must have moved to nyquist first
+                    self.auto_xy = 'fy'
+                    
+                else:
+                    # update freq range if switching plot other than to/from nyquist
+                    self.freq_range = list(self.p.ax.get_xlim()) # force to list instead of tuple
+                    self.auto_xy = 'fy'
+                    
+                    
+                # always reset figure heading
+                self.label_figure.setText(self.selected_view)
+                                
+                # set gui to correct toolset
+                if self.plot_type == 'Nyquist':
+                    #self.auto_xy = 'xy'
+                    self.show_plot_details_with_nqyuist()
+                else:
+                    self.show_plot_details_basic()
+                    
+                self.update_figure()
+
+                
+            # show message if no data to plot
+            else:
+                message = 'No FFT data to display.\n'
+                self.show_message(message)
+        
+        # TF Data
+        elif self.selected_view == 'TF Data':
+            N = len(self.dataset.tf_data_list)
+            # check if data to plot
+            if N != 0:
+                # if main view changed reset plot properties
+                if self.current_view_changed:
+                    self.current_view = self.selected_view
+                    self.show_data = True
+                    self.show_coherence = True 
+                    self.auto_xy = 'xyc'
+                    self.plot_type = 'Amplitude (dB)'
+                    self.input_list_plot_type.setCurrentText(self.plot_type)
+                
+                # if staying as TF plot but changing to nyquist then switch to TF Nyquist toolset
+                elif self.switch_to_nyquist == True:
+                    # get properties before switch so can go back to this view
+                    self.freq_range = list(self.p.ax.get_xlim()) #force to list instead of tuple
+                    self.show_coherence_before = self.show_coherence
+                    self.show_coherence = False
+                    self.xlinlog_before = self.xlinlog
+                    # linear x axis for nyquist
+                    self.xlinlog = 'linear'
+                    # update freq range text
+                    self.input_freq_min.setText('{:0.5g}'.format(self.freq_range[0]))
+                    self.input_freq_max.setText('{:0.5g}'.format(self.freq_range[1]))
+                    self.auto_xy = 'xy'
+                
+                # if moving from nyquist back, reset properties to previous
+                elif self.switch_from_nyquist == True:
+                    self.show_coherence = self.show_coherence_before
+                    self.xlinlog = self.xlinlog_before
+                    self.auto_xy = 'fy'
+                    # freq range already set above as must have moved to nyquist first
+            
+                else:
+                    # update freq range if switching plot other than to/from nyquist
+                    self.freq_range = list(self.p.ax.get_xlim()) # force to list instead of tuple
+                    self.auto_xy = 'fy'
+
+                # plot now then auto-x/y according to nyquist or not
+                self.update_figure()
+
+                    
+                # set gui to correct toolset
+                self.label_figure.setText(self.selected_view)
+                if self.plot_type == 'Nyquist':
+                    self.show_plot_details_with_nqyuist()
+                else:
+                    self.show_plot_details_with_coherence()
+                    
+            # show message if no data
+            else:
+                message = 'No transfer function data to display.\n'
+                self.show_message(message)
+            
+        elif self.selected_view == 'Sono Data':
+             ### set to time gui
+            N = len(self.dataset.sono_data_list)
+            # check if any data present to display
+            if N != 0:
+                # no plot details needed for sonogram display
+                self.hide_plot_details()
+                # reset data/coherence plot properties if changed view back to time
+                if self.current_view_changed:
+                    self.current_view = self.selected_view
+                    self.show_data = True
+                    self.show_coherence = True # won't plot but reests for other selections
+                    self.xlinlog = 'linear'
+                    self.auto_xy = 'xyc'
+                    self.plot_type = 'Amplitude (dB)'
+                    self.input_list_plot_type.setCurrentText(self.plot_type)
+                else:
+                    self.auto_xy = ''
+                    
+                # plot
+                self.update_figure()
+                
+            # show message if no data
+            else:
+                message = 'No sonogram data to display.\n'
+                self.show_message(message)
+            
+            
+        
+    def hide_plot_details(self):
+        self.frame_plot_details.setVisible(False)
+        
+    def show_plot_details_with_coherence(self):
+        # Put Falses before Trues
+        self.input_freq_min.setVisible(False)
+        self.input_freq_max.setVisible(False)        
+
+        self.button_xlinlog.setVisible(True)
+        self.button_data_toggle.setVisible(True)
+        self.button_coherence_toggle.setVisible(True)
+        self.label_co_freq_min.setVisible(True)
+        self.label_co_freq_max.setVisible(True)
+        self.label_co_freq_min.setText('co. min:')
+        self.label_co_freq_max.setText('co. max:')
+        
+        self.input_co_min.setVisible(True)
+        self.input_co_max.setVisible(True)
+        
+        self.frame_plot_details.setVisible(True)
+        
+        
+    def show_plot_details_with_nqyuist(self):
+        # Put Falses before Trues
+        self.button_xlinlog.setVisible(False)
+        self.button_data_toggle.setVisible(False)
+        self.button_coherence_toggle.setVisible(False)
+        self.input_co_min.setVisible(False)
+        self.input_co_max.setVisible(False)
+        
+        self.label_co_freq_min.setVisible(True)
+        self.label_co_freq_max.setVisible(True)
+        self.label_co_freq_min.setText('freq. min:')
+        self.label_co_freq_max.setText('freq. max:')
+        
+        self.input_freq_min.setVisible(True)
+        self.input_freq_max.setVisible(True)
+
+        self.frame_plot_details.setVisible(True)
+        
+        
+    def show_plot_details_basic(self):
+        # put Falses before Trues
+        self.button_data_toggle.setVisible(False)
+        self.button_coherence_toggle.setVisible(False)
+        self.label_co_freq_min.setVisible(False)
+        self.label_co_freq_max.setVisible(False)
+        
+        self.input_co_min.setVisible(False)
+        self.input_co_max.setVisible(False)
+        self.input_freq_min.setVisible(False)
+        self.input_freq_max.setVisible(False)
+        
+        self.button_xlinlog.setVisible(True)
+        self.frame_plot_details.setVisible(True)
+        
+    def hide_all_tools(self):
+        self.frame_tools_time_domain.setVisible(False)
+        self.frame_tools_fft.setVisible(False)
+        self.frame_tools_tf.setVisible(False)
+        self.frame_tools_scaling.setVisible(False)
+        self.frame_tools_mode_fitting.setVisible(False)
+        self.frame_tools_settings.setVisible(False)
+        self.frame_tools_generate_output.setVisible(False)
+        self.frame_tools_edit_dataset.setVisible(False)
+        self.frame_tools_sonogram.setVisible(False)
+        self.frame_tools_save_export.setVisible(False)
+        
+    def select_tool(self):
+        self.selected_tool = self.input_list_tools.currentText()
+        if self.selected_tool == 'Standard Tools':
+            self.hide_all_tools()
+            self.frame_tools_time_domain.setVisible(True)
+            self.frame_tools_fft.setVisible(True)
+            self.frame_tools_tf.setVisible(True)
+            self.frame_tools_scaling.setVisible(True)
+            
+            
+        elif self.selected_tool == 'Logger Settings':
+            self.hide_all_tools()
+            self.frame_tools_settings.setVisible(True)
+            
+        elif self.selected_tool == 'Generate Output':
+            self.hide_all_tools()
+            self.frame_tools_generate_output.setVisible(True)
+            
+        elif self.selected_tool == 'Pre-process':
+            self.hide_all_tools()
+            self.frame_tools_time_domain.setVisible(True)
+            
+        elif self.selected_tool == 'FFT':
+            self.hide_all_tools()
+            self.frame_tools_fft.setVisible(True)
+            
+        elif self.selected_tool == 'Transfer Function':
+            self.hide_all_tools()
+            self.frame_tools_tf.setVisible(True)
+            
+        elif self.selected_tool == 'Calibration / Scaling':
+            self.hide_all_tools()
+            self.frame_tools_scaling.setVisible(True)
+            
+        elif self.selected_tool == 'Sonogram':
+            self.hide_all_tools()
+            self.frame_tools_sonogram.setVisible(True)
+            
+        elif self.selected_tool == 'Mode Fitting':
+            self.hide_all_tools()
+            self.frame_tools_mode_fitting.setVisible(True)
+            
+        elif self.selected_tool == 'Edit Dataset':
+            self.hide_all_tools()
+            self.auto_xy = ''
+            self.update_selected_set()
+            self.frame_tools_edit_dataset.setVisible(True)
+
+            
+        elif self.selected_tool == 'Save / Export':
+            self.hide_all_tools()
+            self.frame_tools_save_export.setVisible(True)
+            
+    def apply_settings(self):
+        settings_dict = dict()
+        for n_row in range(14):
+            label = self.labels_settings[n_row]
+            text = self.input_settings[label].text()
+            settings_dict[label] = text
+        self.settings_dict = settings_dict
+        self.settings = options.MySettings(**settings_dict)
+        self.test_name = self.input_test_name.text()
+        if self.test_name == '':
+            self.test_name = None
+        self.start_stream()
+            
+    
+    def show_available_devices(self):
+        message = streams.list_available_devices()
+        self.show_message(message)
+
+    def update_selected_set(self):
+        # this function is related to edit_dataset tool, not selecting channels
+        data_type = self.input_list_data_type.currentText()
+        if data_type == 'Time Data':
+            self.data_list = self.dataset.time_data_list
+            self.switch_view(data_type)
+        elif data_type == 'FFT Data':
+            self.data_list = self.dataset.freq_data_list
+            self.switch_view(data_type)
+        elif data_type == 'TF Data':
+            self.data_list = self.dataset.tf_data_list
+            self.switch_view(data_type)
+        elif data_type == 'Modal Data':
+            self.data_list = self.dataset.modal_data_list
+        elif data_type == 'Sono Data':
+            self.data_list = self.dataset.sono_data_list
+        else:
+            self.data_list = []
+        
+        self.update_data_summary()
+        
+    def update_data_summary(self):
+        # also keeps validator up to date
+        N = len(self.data_list)
+        self.input_selected_set.setValidator(QIntValidator(0,N-1))
+        text = self.dataset.__repr__()
+        self.label_data_summary.setText(text)
+
+    def delete_data_type(self):
+        self.auto_xy = ''
+        self.update_selected_set()
+        if len(self.data_list) != 0:
+            self.dataset_backup = copy.deepcopy(self.dataset)
+            self.data_type = self.data_list[0].__class__.__name__
+            self.dataset.remove_data_item_by_index(self.data_type,np.arange(len(self.data_list)))
+            self.last_action = 'delete data'
+            message = 'All {} items deleted.\n\n'.format(self.data_type)
+            self.show_message(message, b='undo')
+        else:
+            message = 'No {} to delete.'.format(self.data_typye)
+            self.show_message(message)
+        self.update_selected_set()
+            
+    
+    def delete_data_set(self):
+        self.auto_xy = ''
+        self.selected_set = int(self.input_selected_set.text())
+        if len(self.data_list) != 0:
+            self.dataset_backup = copy.deepcopy(self.dataset)
+            self.data_type = self.data_list[0].__class__.__name__
+            self.dataset.remove_data_item_by_index(self.data_type,self.selected_set)
+            self.last_action = 'delete data'
+            message = 'Set {} of type {} deleted.'.format(self.selected_set,self.data_type)
+            self.show_message(message, b='undo')
+        else:
+            message = 'No {} to delete.'.format(self.data_typye)
+            self.show_message(message)
+        self.update_selected_set()
+    
+    def log_and_replace(self):
+        self.auto_xy = ''
+        self.dataset_backup = copy.deepcopy(self.dataset)
+        self.selected_set = int(self.input_selected_set.text())
+        self.flag_log_and_replace = True
+        self.button_clicked_log_data()
+        
+#        ### DUPLICATES button_clicked_log_data FUNCTION SO THAT MESSAGE APPEARS ###
+#        if self.rec is None:
+#            self.start_stream()
+#        self.rec.trigger_detected = False
+#        self.button_log_data.setStyleSheet("background-color: white")
+#        if self.settings.pretrig_samples is None:
+#            message = 'Logging data for {} seconds'.format(self.settings.stored_time)
+#        else:
+#            message = 'Logging data for {} seconds, with trigger'.format(self.settings.stored_time)
+#        self.thread = LogDataThread(self.settings,test_name=self.test_name, rec=self.rec)
+#        self.show_message(message,'cancel')
+#        self.thread.start()
+#        self.thread.s.connect(self.add_logged_data)
+        ###########################################################################
+    
+    def update_output(self):
+        sig = self.input_output_options.currentText()
+        if sig == 'None':
+            self.flag_output = False
+        else:
+            self.flag_output = True
+            
+    def create_output_signal(self):
+        sig = self.input_output_options.currentText()
+        T = float(self.input_output_duration.text())
+        amp = float(self.input_output_amp.text())
+        f1 = float(self.input_output_f1.text())
+        f2 = float(self.input_output_f2.text())
+        f_max = np.max([f1,f2])
+        fs_min = np.min([self.settings.fs,self.settings.output_fs])
+            
+        if sig != 'None':
+            if f_max > fs_min/2:
+                message = 'Highest output frequency {} Hz exceeds input or output sampling frequency {} Hz.'.format(f_max,fs_min)
+                self.show_message(message)
+                td = None
+            else:
+                t,y = acquisition.signal_generator(self.settings,sig=sig,T=T,amplitude=amp,f=[f1,f2],selected_channels='all')
+                td = datastructure.TimeData(t,y,self.settings,test_name='output_signal')
+                message = acquisition.MESSAGE
+                self.show_message(message)
+        else:
+            td = None
+#            message = 'Output signal turned off.'
+#            self.show_message(message)         
+        self.output_time_data = td
+            
+    def preview_output(self):
+        self.create_output_signal()
+        if self.output_time_data != None:
+            d = datastructure.DataSet(self.output_time_data)
+            d.calculate_fft_set()
+            self.preview_window = PreviewWindow(title='Time Data')
+            self.preview_window.p.update(d.time_data_list,auto_xy='xy')
+            self.preview_window2 = PreviewWindow(title='FFT Data')
+            self.preview_window2.p.update(d.freq_data_list, xlinlog='log',auto_xy='xy')
+    
+    def start_output(self):
+        self.create_output_signal()
+        if self.output_time_data != None:
+            s = acquisition.output_signal(self.settings,self.output_time_data.time_data)
+        else:
+            message = 'No output data to generate.'
+            self.show_message(message)
+            
+
+    #%% DATA PROCESSING
+    def clean_impulse(self):
+        try:
+            ch_impulse = int(self.input_impulse_channel.text())
+            
+            dataset_new = self.dataset.clean_impulse(ch_impulse=ch_impulse)
+            
+            if 'data already cleaned' not in analysis.MESSAGE:
+                # only make backup if first time cleaned, otherwise backup no longer contains original data
+                # not watertight logic if cleaned some but not all channels before
+                # needs updating
+                self.dataset_backup = self.dataset
+            self.dataset = dataset_new
+            self.show_message(analysis.MESSAGE,b='undo')
+            self.last_action = 'clean_impulse'
+            self.auto_xy = ''
+            selection = self.p.get_selected_channels()
+            self.update_figure()
+            self.p.set_selected_channels(selection)
+        except:
+            analysis.MESSAGE = 'Clean impulse not successful, no change made.\n'
+            analysis.MESSAGE += 'Check if ch_{} exists for each set of data.'.format(ch_impulse)
+            self.show_message(analysis.MESSAGE,b='ok')
+            
+            
+    def undo_last_action(self):
+        if self.last_action == 'clean_impulse':
+            self.dataset = self.dataset_backup
+            self.update_figure()
+        if self.last_action == 'scaling':
+            self.dataset = self.dataset_backup
+            self.update_figure()
+        if self.last_action == 'delete modes':
+            self.dataset = self.dataset_backup
+            self.selected_channels = self.selected_channels_backup
+            self.update_figure()
+            message = 'Deleted mode fits restored.'
+            self.show_message(message)
+        if self.last_action == 'delete data':
+            self.dataset = self.dataset_backup
+            self.update_figure()
+            message = 'Deleted data restored.'
+            self.show_message(message)
+        if self.last_action == 'data replaced':
+            self.dataset = self.dataset_backup
+            self.update_figure()
+            message = 'Replaced data restored.'
+            self.show_message(message)
+            
+    def calc_fft(self):
+        if len(self.dataset.time_data_list) == 0:
+            message = 'No time data to calculate transfer function.'
+            self.show_message(message)
+        
+        else:
+            window = self.input_list_window_fft.currentText()
+            if window == 'None':
+                window = None
+            
+            self.dataset.calculate_fft_set(window=window)
+            self.switch_view('FFT Data')
+            
+    def select_averaging_type(self):
+        self.averaging_method = self.input_list_average_TF.currentText()
+        if self.averaging_method == 'None':
+            self.input_Nframes.setText('1')
+            self.slider_Nframes.setValue(1)
+            self.label_Nframes.setVisible(False)
+            self.input_Nframes.setVisible(False)
+            self.slider_Nframes.setVisible(False)
+            self.label_Nframes_time.setVisible(False)
+            self.button_TFav.setVisible(False)
+            self.button_TF.setVisible(True)
+            
+        elif self.averaging_method == 'within each set':
+            self.button_TFav.setVisible(False)
+            self.button_TF.setVisible(True)
+            self.label_Nframes.setVisible(True)
+            self.input_Nframes.setVisible(True)
+            self.label_Nframes_time.setVisible(True)
+            self.slider_Nframes.setVisible(True)
+            
+        elif self.averaging_method == 'across sets':
+            self.button_TF.setVisible(False)
+            self.label_Nframes.setVisible(False)
+            self.input_Nframes.setVisible(False)
+            self.slider_Nframes.setVisible(False)
+            self.label_Nframes_time.setVisible(False)
+            self.button_TFav.setVisible(True)
+            
+    def refresh_Nframes_text(self):
+        self.N_frames = self.slider_Nframes.value()
+        self.input_Nframes.setText(str(self.N_frames))
+        if len(self.dataset.time_data_list)>0:
+            stored_time = self.dataset.time_data_list[0].settings.stored_time
+            text = "Frame length = {:.2f} seconds.".format(stored_time/(self.N_frames-self.overlap*self.N_frames+self.overlap))
+        else:   
+            text = 'No time data'
+        self.label_Nframes_time.setText(text)
+        
+        
+    def refresh_Nframes_slider(self):
+        self.N_frames = int(self.input_Nframes.text())
+        # allows setting text to higher than max slider
+        try:
+            self.slider_Nframes.setValue(self.N_frames)
+        except:
+            pass
+        if len(self.dataset.time_data_list)>0:
+            stored_time = self.dataset.time_data_list[0].settings.stored_time
+            text = "Frame length = {:.2f} seconds.".format(stored_time/(self.N_frames-self.overlap*self.N_frames+self.overlap))
+        else:   
+            text = 'No time data'
+        self.label_Nframes_time.setText(text)
+        
+        
+    def refresh_test_name(self):
+        # keep both places for entering test_name up to date
+        self.input_test_name2.setText(self.input_test_name.text())
+        self.test_name = self.input_test_name.text()
+        
+    def refresh_test_name2(self):
+        # keep both places for entering test_name up to date
+        self.input_test_name.setText(self.input_test_name2.text())
+        self.test_name = self.input_test_name2.text()
+        
+    def calc_tf(self):
+        if len(self.dataset.time_data_list) == 0:
+            message = 'No time data to calculate transfer function.'
+            self.show_message(message)
+        
+        else:
+            self.N_frames = int(self.input_Nframes.text())
+            window = self.input_list_window_tf.currentText()
+            if window == 'None':
+                window = None
+
+            self.dataset.calculate_tf_set(window=window,N_frames=self.N_frames,overlap=self.overlap)
+            if self.current_view != 'TF Data':
+                self.switch_view('TF Data')
+            else:
+                self.auto_xy = ''
+                self.update_figure()
+            
+    
+    def calc_tf_av(self,b):
+        if len(self.dataset.time_data_list) == 0:
+            message = 'No data to calculate FFT.'
+            self.show_message(message)
+        
+        else:
+            window = self.input_list_window_tf.currentText()
+            if window == 'None':
+                window = None
+        
+            self.dataset.calculate_tf_averaged(window=window)
+            
+            if self.current_view != 'TF Data':
+                self.switch_view('TF Data')
+            else:
+                self.auto_xy = ''
+                self.update_figure()
+        
+    def xiw(self):
+        power = 1
+        self.xiwp(power)
+        
+    def diw(self):
+        power = -1
+        self.xiwp(power)
+
+
+        
+    def xiwp(self,power):
+        if self.flag_scaling == False:
+            # create backup before any changes made - used to reset
+            self.dataset_backup = copy.deepcopy(self.dataset)
+                
+        if self.current_view == 'FFT Data':
+            data_list = self.dataset.freq_data_list
+        elif self.current_view == 'TF Data':
+            data_list = self.dataset.tf_data_list
+        else:
+            message = 'First select ''FFT Data'' or ''TF Data''.'
+            self.show_message(message)
+            return None
+        
+        if len(data_list) > 0:            
+            s = self.p.get_selected_channels()
+            if self.selected_channels != s:
+                # reset gui's iw_power record if changed selection
+                self.iw_fft_power = 0
+                self.selected_channels = s
+                
+            
+            for ns in range(len(s)):
+                newdata = analysis.multiply_by_power_of_iw(data_list[ns],power=power,channel_list=s[ns])
+                data_list[ns] = newdata
+                self.flag_scaling = True
+                
+            if data_list.__class__.__name__ == 'FreqData':
+                self.dataset.freq_data_list = data_list
+            elif data_list.__class__.__name__ == 'TfData':
+                self.dataset.tf_data_list = data_list
+            
+            
+            if self.plot_type == 'Nyquist':
+                self.auto_xy = 'xy'
+            else:
+                self.auto_xy = 'fy'
+            
+            self.update_figure()
+            self.p.set_selected_channels(s)
+            
+            self.iw_fft_power += power # local counter for currently selected channels
+            self.last_action = 'scaling'
+            message = 'Selected FFT data multiplied by (iw)**{}\n'.format(self.iw_fft_power)
+            message += '(note that power counter resets when selection changes)'
+            self.show_message(message)
+        else:
+            message = 'First calculate FFT or TF of data.'
+            self.show_message(message)
+        
+    def undo_scaling(self):
+        if self.last_action == 'scaling':
+            self.undo_last_action()
+            self.flag_scaling = False
+            message = 'Scaling removed.'
+        else:
+            message = 'Can''t undo: scaling not last action carried out.'
+        
+        self.show_message(message)
+        
+        
+    def best_match(self):
+        if self.flag_scaling == False:
+            # provide backup for undo
+            self.dataset_backup = copy.deepcopy(self.dataset)
+            self.flag_scaling = True
+            
+        self.refset  = int(self.input_refset.text())
+        self.refchan = int(self.input_refchan.text())
+        if self.current_view == 'TF Data':
+            current_calibration_factors = self.dataset.tf_data_list.get_calibration_factors()
+            reference = current_calibration_factors[self.refset][self.refchan]
+            factors = analysis.best_match(self.dataset.tf_data_list,freq_range=self.freq_range,set_ref=self.refset,ch_ref=self.refchan)
+            factors = [reference*x for x in factors]
+            self.dataset.tf_data_list.set_calibration_factors_all(factors)
+            self.auto_xy = ''
+            self.update_figure()
+            with np.printoptions(precision=3, suppress=False):
+                message = 'Scale factors:\n'
+                n_set = -1
+                self.factors = factors
+                for fs in factors:
+                    n_set += 1
+#                    message += 'Set {:>10:d}: factors = {:.5g}\n'.format(n_set,np.squeeze(fs))
+#                    [[fill]align][sign][#][0][minimumwidth][.precision][type]
+                    message += '{:<3} {:>4} {:<12} {}\n'.format('Set',n_set,': factors =',np.squeeze(fs))
+                self.show_message(message)
+            
+            self.last_action = 'scaling'
+            
+        else:
+            message = 'First select ''TF Data'' or ''Calc TF''.\n'
+            self.show_message(message)
+        
+    def fit_mode(self):
+        if self.current_view == 'TF Data':
+            if self.input_list_tf_type.currentText() == 'Acceleration':
+                self.measurement_type = 'acc'
+            elif self.input_list_tf_type.currentText() == 'Velocity':
+                self.measurement_type = 'vel'
+            elif self.input_list_tf_type.currentText() == 'Displacement':
+                self.measurement_type = 'dsp'
+            
+            m = modal.modal_fit_all_channels(self.dataset.tf_data_list,freq_range=self.freq_range, measurement_type=self.measurement_type)
+            self.last_mode_fit = m
+            self.show_message(modal.MESSAGE)
+            if len(self.dataset.modal_data_list) == 0:
+                self.dataset.modal_data_list = [m]
+            elif len(self.fn_in_range) > 1:
+                message = 'Several mode fits already in this range.\n\n'
+                message += 'Fitted mode frequencies = {} (Hz)\n\n'.format(np.array2string(self.fn_in_range,precision=2))
+                message += 'To delete them, press ''Reject''.'
+                message += 'To replace a single fit, zoom into a single peak first.'
+                self.show_message(message)
+                return None
+            elif len(self.fn_in_range) == 1:
+                # find which mode and replace it
+                fn_all = self.dataset.modal_data_list[0].M[:,0]
+                mode_number = np.where((fn_all > self.freq_range[0]) & (fn_all < self.freq_range[1]))[0]
+                self.dataset.modal_data_list[0].delete_mode(mode_number)
+                self.dataset.modal_data_list[0].add_mode(m.M[0,:]) # only one mode in 'm'
+            else:
+                self.dataset.modal_data_list[0].add_mode(m.M[0,:]) # only one mode in 'm'
+            
+            # local reconstruction
+            s1 = self.p.get_selected_channels() # keep selection after auto-range
+            
+            f = np.linspace(self.freq_range[0],self.freq_range[1],3000)
+            tf_data = modal.reconstruct_transfer_function(m,f,self.measurement_type)
+            tf_data.flag_modal_TF = True
+            self.dataset.tf_data_list.add_modal_reconstruction(tf_data,mode='replace')
+            
+            if self.plot_type == 'Nyquist':
+                self.auto_xy = 'xy'
+            else:
+                self.auto_xy = 'fy'
+                
+            self.update_figure()
+            s2 = self.p.get_selected_channels()
+            # retain selection for fitted selection
+            # assumes each set is a single Transfer Function
+            # might break down if data organised differently
+            for i in range(len(s2[-1])):
+                #s2[i] = s1[i]
+                s2[-1][i] = s2[i][0]
+            if len(s1) != len(s2):
+                s1 += [[]]
+                
+            self.p.set_selected_channels(s2) # keep selection after auto-range
+            self.selected_channels = s2.copy()
+            self.update_figure() # run a second time so autoscaling picks up new lines
+            fn_all = self.dataset.modal_data_list[0].M[:,0]
+            self.fn_in_range = m.fn
+            ### allow time for plots and axes to update before clearing modal.MESSAGE
+            #time.sleep(1)
+            #modal.MESSAGE = '' # this is a condition for update_axes_values to let modal messages appear
+        else:
+            message = 'First select ''TF Data''.'
+            self.show_message(message)
+            
+    
+    def freq_min2(self):
+        self.freq_range[0] = float(self.input_freq_min2.text())
+        self.input_freq_min.setText(str(self.freq_range[0]))
+        self.freq_min()
+    
+    def freq_max2(self):
+        self.freq_range[1] = float(self.input_freq_max2.text())
+        self.input_freq_max.setText(str(self.freq_range[1]))
+        self.freq_max
+        
+    def accept_mode(self):
+        self.dataset.modal_data_list
+        self.view_modal_reconstruction()
+        
+    
+    def reject_mode(self):
+        # reject mode fits currently in view
+        if len(self.fn_in_range) >= 1:
+            self.last_action = 'delete modes'
+            self.dataset_backup = copy.deepcopy(self.dataset)
+            self.selected_channels_backup = self.p.get_selected_channels()
+            # find which mode and replace it
+            fn_all = self.dataset.modal_data_list[0].M[:,0]
+            mode_number = np.where((fn_all > self.freq_range[0]) & (fn_all < self.freq_range[1]))[0]
+            self.dataset.modal_data_list[0].delete_mode(mode_number)
+            if self.dataset.tf_data_list[-1].flag_modal_TF == True:
+                self.dataset.remove_last_data_item('TfData')
+                self.selected_channels.pop(-1) # updates selected channels
+                self.auto_xy = ''
+                self.update_figure()
+            message = 'Mode fits deleted.'
+            self.show_message(message,b='undo')
+        
+    def view_mode_summary(self):
+        message = 'Modes fitted:\n\n'
+        message += 'fn = {} (Hz)\n\n'.format(np.array2string(self.dataset.modal_data_list[0].fn,precision=2))
+        message += 'zn = {}\n'.format(np.array2string(self.dataset.modal_data_list[0].zn,precision=5))
+        message += 'Qn = 1/(2 zn) = {}'.format(np.array2string(1/2/self.dataset.modal_data_list[0].zn,precision=1))
+        self.show_message(message)
+    
+    def view_modal_reconstruction(self):
+        # Global reconstruction
+        s = self.p.get_selected_channels() # keep selection after auto-range
+        
+        f = self.dataset.tf_data_list[0].freq_axis
+        m = self.dataset.modal_data_list[0]
+        tf_data = modal.reconstruct_transfer_function_global(m,f,self.measurement_type)
+        tf_data.flag_modal_TF = True
+        self.dataset.tf_data_list.add_modal_reconstruction(tf_data,mode='replace')
+        
+        self.auto_xy = 'xy'
+        self.update_figure()
+        s2 = self.p.get_selected_channels()
+        for i in range(len(s2[-1])):
+            s2[-1][i] = True
+        if len(s) != len(s2):
+            s += [[]]
+        s[-1] = s2[-1]
+        self.p.set_selected_channels(s) # keep selection after auto-range
+        self.fn_in_range = m.fn
+        
+    def refresh_sono_N_frames_slider(self):
+        self.slider_sono_N_frames.setValue(int(self.input_sono_N_frames.text()))
+    
+    def refresh_sono_N_frames_text(self):
+        self.input_sono_N_frames.setText(str(self.slider_sono_N_frames.value()))
+    
+    def calc_sono(self):
+        if len(self.dataset.time_data_list) == 0:
+            message = 'No time data to calculate transfer function.'
+            self.show_message(message)
+        else:
+            self.N_frames_sono = int(self.input_sono_N_frames.text())
+            n_set = int(self.input_sono_n_set.text())
+            n_chan = int(self.input_sono_n_chan.text())
+#            db_range = int(self.input_db_range.text())
+            NT = len(self.dataset.time_data_list[n_set].time_data[:,n_chan])
+            f = 1/4 # match overlap in sonogram
+            self.nperseg = int(NT // (self.N_frames_sono * (1-f) + f)) # 1/8 is default overlap for spectrogram
+            self.dataset.calculate_sono_set(nperseg=self.nperseg)
+            
+            # calc sonogram info
+            npfft,npt = np.shape(self.dataset.sono_data_list[n_set].sono_data[:,:,n_chan])
+            text = 'FFT length: {}\n'.format(self.nperseg)
+            text += 'Freq resolution: {:5g} (Hz)\n'.format(np.diff(self.dataset.sono_data_list[n_set].freq_axis[[0,1]])[0])
+            
+            self.sono_info.setText(text)
+            if self.current_view != 'Sono Data':
+                self.switch_view('Sono Data')
+            self.update_figure()
+            
+    def import_jwlogger(self):
+        pass
+    
+    def export_jwlogger(self):
+        # export data to data structure compatible with JW Logger
+        file.export_to_matlab_jwlogger(self.dataset)        
+        
+    def export_matlab(self):
+        # export data to data structure compatible with Matlab
+        file.export_to_matlab(self.dataset)
+    
+    def export_csv(self):
+        # export data displayed to CSV
+        if  self.current_view == 'Time Data':
+            file.export_to_csv(self.dataset.time_data_list)
+        elif  self.current_view == 'FFT Data':
+            file.export_to_csv(self.dataset.freq_data_list)
+        elif  self.current_view == 'TF Data':
+            file.export_to_csv(self.dataset.tf_data_list)
+        else:
+            self.show_message('Can only export Time, FFT or TF Data')
+        
+#sys._excepthook = sys.excepthook 
+#def exception_hook(exctype, value, traceback):
+#    print(exctype, value, traceback)
+#    sys._excepthook(exctype, value, traceback) 
+#    sys.exit(1) 
+#sys.excepthook = exception_hook 
+
+
+
+class Oscilloscope():
+    def __init__(self, settings):
+        '''Creates an Oscilloscope
+        Args:
+            settings: An object of the class MySettings
+        '''
+
+        self.settings = settings
+        
+        streams.start_stream(settings)
+        self.rec = streams.REC
+        
+
+        self.timer = QtCore.QTimer()
+        self.create_figure()
+
+        self.win.sigKeyPress.connect(self.keyPressed)
+        self.win.sigClose.connect(self.on_close)
+
+        # Start the update timer
+        self.timer.timeout.connect(self.update) # update figure and buffer
+        self.timer.start(60)
+
+        if app.applicationState() != Qt.ApplicationActive:
+            app.exec()  
+
+    def create_figure(self):
+        '''
+        Creates a figure which is an object of the class KeyPressWindow.
+
+        '''
+        pg.setConfigOption('background', 'w')
+        self.win = KeyPressWindow()
+        self.win.setWindowIcon(QtGui.QIcon('icon.png'))
+#        window_geometry = self.win.geometry()
+        self.win.setGeometry(100,100,800,600)
+        self.win.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
+        
+        # This ensures the window appears at front.
+        # self.win.showMinimized()
+        
+
+        self.win.setWindowTitle("Oscilloscope ('s': save new, 'space': autosave, 'p': pause, 'a': always top, 'y': autoscale)")
+        # time.sleep(0.6)
+        self.win.show()
+        self.win.showNormal()
+        self.win.raise_()
+
+        self.view_time = self.settings.init_view_time
+        self.view_freq = self.settings.init_view_freq
+        self.view_levels = self.settings.init_view_levels
+
+        self.toggle_view()
+        
+        self.auto_scale = False
+
+        self.data_saved_counter = 0 #  to indicate not yet saved file
+
+    def on_close(self, evt):
+        self.timer.stop()
+        # self.rec.end_stream()
+
+    def toggle_view(self):
+        '''
+        Switches between views, triggered by keypress
+        '''
+        self.win.clear()
+
+        if self.view_time:
+            self.time_plot()
+
+        if self.view_freq:
+            self.freq_plot()
+
+        if self.view_levels:
+            self.levels_plot()
+
+    def time_plot(self):
+        # create a plot for the time domain
+        self.view_time = True
+        self.win.nextRow()
+        self.osc_time_line = self.win.addPlot(title="Time Domain (toggle with 'T')")
+
+        if self.settings.channels == 1:
+            self.auto_scale = True
+            self.osc_time_line.enableAutoRange()
+        else:
+            # Stack the channels -- channel 0 is centred on 0, channel 1
+            # centred on 1 etc.
+            self.auto_scale = False
+            self.osc_time_line.setYRange(-1,self.settings.channels)
+
+        self.osc_time_line.setXRange(self.rec.osc_time_axis[0],
+                                     self.rec.osc_time_axis[-1])
+        self.osc_time_line.showGrid(True, True)
+        self.osc_time_line.addLegend()
+        self.osc_time_line.setLabel('left', 'Normalised Amplitude')
+        self.osc_time_line.setLabel('bottom', 'Time (s)')
+
+        self.ax_time = self.osc_time_line.getAxis('left')
+        self.ax_time.setTickSpacing(1, 1)
+
+        self.osc_time_lineset = {}
+        for i in range(self.settings.channels):
+            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:])
+            self.osc_time_lineset[i] = self.osc_time_line.plot(
+                pen=pen_, name='Channel %d' % i)
+
+#        self.win.FillBetweenItem(curve1=osc_time_lineset[0], curve2=osc_time_lineset[1])
+
+    def freq_plot(self):
+        # create a plot for the frequency domain
+        self.view_freq = True
+        self.win.nextRow()
+        self.osc_freq_line = self.win.addPlot(
+            title="Frequency Domain (toggle with 'F')")
+        self.osc_freq_line.enableAutoRange()
+        self.osc_freq_line.setXRange(self.rec.osc_freq_axis[0],
+                                     self.rec.osc_freq_axis[-1])
+        self.osc_freq_line.showGrid(True, True)
+        self.osc_freq_line.addLegend()
+        self.osc_freq_line.setLabel('left', 'Power Spectrum (dB)')
+        self.osc_freq_line.setLabel('bottom', 'Frequency (Hz)')
+
+        self.osc_freq_lineset = {}
+        for i in range(self.settings.channels):
+            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:])
+            self.osc_freq_lineset[i] = self.osc_freq_line.plot(
+                pen=pen_, name='Channel %d' % i)
+
+    def levels_plot(self):
+        # create a plot for the frequency domain
+        self.view_levels = True
+        self.win.nextRow()
+        self.osc_levels_line = self.win.addPlot(title="Channel Levels (toggle with 'L')")
+        self.osc_levels_line.setYRange(0, 1)
+        self.osc_levels_line.setXRange(-0.5, self.settings.channels - 0.5)
+        self.osc_levels_line.showGrid(False, True)
+        self.osc_levels_line.setLabel('left', 'Normalised Amplitude')
+        self.osc_levels_line.setLabel('bottom', 'Channel Index')
+
+        self.ax_levels = self.osc_levels_line.getAxis('bottom')
+        self.ax_levels.setTickSpacing(1, 1)
+#        ax.showLabel(show=True)
+#        self.osc_levels_line.setTicks(np.arange(self.settings.channels))
+        self.osc_levels_lineset={}
+        for i in range(self.settings.channels):
+            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
+            pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
+            self.osc_levels_lineset[i]=self.osc_levels_line.plot(pen=pen_, name='vertical')
+            self.osc_levels_lineset[self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_, name='top')
+            self.osc_levels_lineset[2*self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_peak, name='peak hold')
+#            self.osc_levels_lineset[3]=self.osc_levels_line.plot(pen=pen_, name='Channel')
+
+        self.osc_levels_peak_hold = np.zeros(self.settings.channels)
+        self.time_last_changed = np.zeros(self.settings.channels)
+
+    def update(self):
+        '''
+        Updates plots with incoming data from __call__.
+        Called with a 0s interval by QTimer.
+
+        '''
+        time_data_snapshot = np.copy(self.rec.osc_time_data)
+        if self.view_levels == True:
+            self.osc_levels_rms = np.sqrt(np.mean(time_data_snapshot**2,axis=0))
+            self.osc_levels_max = np.max(np.abs(time_data_snapshot),axis=0)
+            changed_indices = self.osc_levels_peak_hold < self.osc_levels_max
+            self.time_last_changed[changed_indices] = time.time()
+            self.osc_levels_peak_hold = np.maximum(self.osc_levels_peak_hold,self.osc_levels_max)
+            self.osc_levels_peak_hold[time.time()-self.time_last_changed>2] = 0
+
+        for i in range(self.settings.channels):
+            offset = i
+            if self.view_time == True:
+                if (self.auto_scale is True) and (self.settings.channels==1):
+                    shift = 0
+                    scale_factor = 1
+                    self.osc_time_line.enableAutoRange()
+                elif (self.auto_scale is True) and (self.settings.channels!=1):
+                    shift = np.mean(time_data_snapshot[:,i])
+                    scale_factor = np.max(np.abs(time_data_snapshot[:,i]-shift))*2
+                    self.osc_time_line.setYRange(-1,self.settings.channels)
+                else:
+                    shift = 0
+                    scale_factor = 1
+                    self.osc_time_line.setYRange(-1,self.settings.channels)
+                    
+                self.osc_time_lineset[i].setData(self.rec.osc_time_axis, (time_data_snapshot[:,i]-shift)/scale_factor + offset)
+
+            if self.view_freq == True:
+                # calculate the FFT
+                self.rec.osc_time_data_windowed[:,i] = time_data_snapshot[:,i] * np.blackman(np.shape(time_data_snapshot)[0])
+                fd = np.abs(np.fft.rfft(self.rec.osc_time_data_windowed[:,i]))/len(self.rec.osc_time_data_windowed[:,i])
+                fd[fd==0] = np.min(fd+1e-16) # to avoid log10(0) warnings
+                self.rec.osc_freq_data[:,i] = 20 * np.log10(fd)
+                self.osc_freq_lineset[i].setData(self.rec.osc_freq_axis,self.rec.osc_freq_data[:,i])
+
+            if self.view_levels == True:
+                self.osc_levels_lineset[i].setData([i,i],[0,self.osc_levels_max[i]])
+                self.osc_levels_lineset[self.settings.channels+i].setData([i-0.3,i+0.3],self.osc_levels_max[i]*np.ones(2))
+
+                if self.osc_levels_peak_hold[i] > 0.98:
+                    pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=10)
+                else:
+                    pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
+#                self.osc_levels_lineset[2*self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_peak, name='peak hold')
+                self.osc_levels_lineset[2*self.settings.channels+i].setData([i-0.3,i+0.3],self.osc_levels_peak_hold[i]*np.ones(2),pen=pen_peak)
+#                self.osc_levels_lineset[3].setData(np.arange(2),np.ones(2))
+
+
+
+    #KeyPressed function within osciolloscpe since can only take one argument
+    def keyPressed(self, evt):
+        '''
+        Upon a Space Bar press, makes a copy of data from the past stored_time seconds,plots it in Bokeh and gives the user an option to save it.
+        '''
+
+        if evt.key() == QtCore.Qt.Key_T:
+
+            if self.view_freq != False or self.view_levels != False:
+#                print('toggled time domain view')
+                self.view_time = not self.view_time
+                self.toggle_view()
+#            else:
+#                print('toggling all views off is prevented')
+
+        if evt.key() == QtCore.Qt.Key_F:
+
+            if self.view_time != False or self.view_levels != False:
+#                print('toggled frequency domain view')
+                self.view_freq = not self.view_freq
+                self.toggle_view()
+#            else:
+#                print('toggling all views off is prevented')
+
+        if evt.key() == QtCore.Qt.Key_L:
+            if self.view_time != False or self.view_freq != False:
+#                print('toggled levels view')
+                self.view_levels = not self.view_levels
+                self.toggle_view()
+#            else:
+#                print('toggling all views off is prevented')
+        
+        if evt.key() == QtCore.Qt.Key_P:
+            if self.timer.isActive():
+                self.timer.stop()
+            else:
+                self.timer.start()
+                
+        if evt.key() == QtCore.Qt.Key_A:
+            self.win.setWindowFlags(self.win.windowFlags() ^ QtCore.Qt.WindowStaysOnTopHint)       
+            self.win.show()
+                
+            
+        if evt.key() == QtCore.Qt.Key_Y:
+            self.auto_scale = not self.auto_scale 
+                
+        if evt.key() == QtCore.Qt.Key_Space or evt.key() == QtCore.Qt.Key_S:
+
+            stored_time_data_copy=np.copy(self.rec.stored_time_data)
+            t = datetime.datetime.now()
+            timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)
+#            print("key press trigger: saving data to file in working directory")
+
+            ### make into dataset
+            
+            fs=self.settings.fs
+            n_samp=len(stored_time_data_copy[:,0])
+            dt=1/fs
+            t_axis= np.arange(n_samp)*dt
+
+            
+            timedata = datastructure.TimeData(t_axis,stored_time_data_copy,self.settings,timestamp=t,timestring=timestring,test_name='Test_{}'.format(self.data_saved_counter))
+            
+            dataset = datastructure.DataSet()
+            dataset.add_to_dataset(timedata)
+            
+            
+            if evt.key() == QtCore.Qt.Key_S:
+                self.data_saved_counter = 1
+                self.last_filename = file.save_data(dataset,self.win)
+            
+#            # this version saves all data as new timedata objects within one file
+#            if evt.key() == QtCore.Qt.Key_Space:
+#                if self.data_saved_counter == 0:
+#                    self.last_filename = file.save_data(dataset)
+#                    if self.last_filename == '':
+#                        self.data_saved_counter = 0
+#                    else:
+#                        self.data_saved_counter += 1
+#                
+#                else:
+#                    d = file.load_data(self.last_filename)
+#                    d.add_to_dataset(timedata)
+#                    file.save_data(d,self.last_filename,overwrite_without_prompt=True)
+#                    self.data_saved_counter += 1
+            
+            # this version saves each new dataset to new file
+            if evt.key() == QtCore.Qt.Key_Space:
+                if self.data_saved_counter == 0:
+                    self.last_filename = file.save_data(dataset,self.win)
+                    if self.last_filename == '':
+                        self.data_saved_counter = 0
+                    else:
+                        self.data_saved_counter += 1
+                
+                else:
+                    d = datastructure.DataSet()
+                    d.add_to_dataset(timedata)
+                    filename = self.last_filename.replace('.npy','_'+str(self.data_saved_counter)+'.npy')
+                    file.save_data(d,self.win, filename,overwrite_without_prompt=True)
+                    self.data_saved_counter += 1
+
+class KeyPressWindow(pg.GraphicsLayoutWidget):
+    '''
+    A subclass of pyQtGraph GraphicsWindow that emits a signal when a key is pressed.
+
+    '''
+    sigKeyPress = Signal(object)
+    sigClose = Signal(object)
+
+    def __init__(self, *args, **kwargs):
+        '''
+        Re-implmented from parent.
+        '''
+        super().__init__(*args, **kwargs)
+
+    def keyPressEvent(self, evt):
+        '''
+        Emits a signal upon a key press
+        '''
+        self.scene().keyPressEvent(evt)
+        self.sigKeyPress.emit(evt)
+
+    def closeEvent(self, evt):
+        '''
+        Emits a signal when the window is closed.
+        '''
+        self.sigClose.emit(evt)
+        self.close()
```

### Comparing `pydvma-0.9.0/pydvma/gui_tk.py` & `pydvma-0.9.1/pydvma/gui_tk.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-# tkinter import common modules
-import tkinter as tk
-from tkinter import ttk
-from tkinter import messagebox
-
-# tkinter matplotlib backend
-from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
-from matplotlib.figure import Figure
-from matplotlib.ticker import AutoLocator
-
-import copy
-import numpy as np
-import threading
-
-
-
-
-# #import logging
-# #logging.basicConfig(filename='example.log',level=logging.DEBUG)
-# #%%
-
-# from . import plotting
-# from . import datastructure
-# from . import acquisition
-# from . import analysis
-# from . import streams
-# from . import file
-# from . import modal
-# from . import options
-import time
-import sys, os
-
-#%%
-import tkinter as tk
-from tkinter import ttk
-import matplotlib.pyplot as plt
-from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
-
-class Logger(tk.Tk):
-    def __init__(self):
-        super().__init__()
-
-        # Set up the main window
-        self.title("Logger")
-        self.geometry("800x600")
-        self.iconphoto(True, tk.PhotoImage(file='./icon.png'))
-        
-        # Create grid of frames
-        self.frame_main = ttk.Frame(self)
-        self.frame_main.grid(column=0, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
-        
-
-        # Create left frame
-        self.left_frame = ttk.Frame(self.frame_main)
-        self.left_frame.grid(column=0, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
-        
-        # Create right frame
-        self.right_frame = ttk.Frame(self.frame_main)
-        self.right_frame.grid(column=2, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
-        
-        
-        # Create middle frame
-        self.middle_frame = ttk.Frame(self.frame_main)
-        self.middle_frame.grid(column=1, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
-        
-        
-        # Create top middle frame
-        self.top_middle_frame = ttk.Frame(self.middle_frame)
-        self.top_middle_frame.grid(column=0, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
-        
-        # Create centre middle frame
-        self.centre_middle_frame = ttk.Frame(self.middle_frame)
-        self.centre_middle_frame.grid(column=0, row=1, sticky=(tk.N, tk.W, tk.E, tk.S))
-        
-        
-        # Create bottom middle frame
-        self.bottom_middle_frame = ttk.Frame(self.middle_frame)
-        self.bottom_middle_frame.grid(column=0, row=1, sticky=(tk.N, tk.W, tk.E, tk.S))
-        
-        
-
-        self.setup_left_frame()
-        self.mainloop()
-
-    def setup_left_frame(self):
-        # add buttons
-        self.button_start = ttk.Button(self.left_frame, text="Start")
-        self.button_start.grid(column=0, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
-        
-        
-    
-    def show(self):
-        self.mainloop()
-        self.lift()
-
-
-# %%
+# tkinter import common modules
+import tkinter as tk
+from tkinter import ttk
+from tkinter import messagebox
+
+# tkinter matplotlib backend
+from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
+from matplotlib.figure import Figure
+from matplotlib.ticker import AutoLocator
+
+import copy
+import numpy as np
+import threading
+
+
+
+
+# #import logging
+# #logging.basicConfig(filename='example.log',level=logging.DEBUG)
+# #%%
+
+# from . import plotting
+# from . import datastructure
+# from . import acquisition
+# from . import analysis
+# from . import streams
+# from . import file
+# from . import modal
+# from . import options
+import time
+import sys, os
+
+#%%
+import tkinter as tk
+from tkinter import ttk
+import matplotlib.pyplot as plt
+from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
+
+class Logger(tk.Tk):
+    def __init__(self):
+        super().__init__()
+
+        # Set up the main window
+        self.title("Logger")
+        self.geometry("800x600")
+        self.iconphoto(True, tk.PhotoImage(file='./icon.png'))
+        
+        # Create grid of frames
+        self.frame_main = ttk.Frame(self)
+        self.frame_main.grid(column=0, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
+        
+
+        # Create left frame
+        self.left_frame = ttk.Frame(self.frame_main)
+        self.left_frame.grid(column=0, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
+        
+        # Create right frame
+        self.right_frame = ttk.Frame(self.frame_main)
+        self.right_frame.grid(column=2, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
+        
+        
+        # Create middle frame
+        self.middle_frame = ttk.Frame(self.frame_main)
+        self.middle_frame.grid(column=1, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
+        
+        
+        # Create top middle frame
+        self.top_middle_frame = ttk.Frame(self.middle_frame)
+        self.top_middle_frame.grid(column=0, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
+        
+        # Create centre middle frame
+        self.centre_middle_frame = ttk.Frame(self.middle_frame)
+        self.centre_middle_frame.grid(column=0, row=1, sticky=(tk.N, tk.W, tk.E, tk.S))
+        
+        
+        # Create bottom middle frame
+        self.bottom_middle_frame = ttk.Frame(self.middle_frame)
+        self.bottom_middle_frame.grid(column=0, row=1, sticky=(tk.N, tk.W, tk.E, tk.S))
+        
+        
+
+        self.setup_left_frame()
+        self.mainloop()
+
+    def setup_left_frame(self):
+        # add buttons
+        self.button_start = ttk.Button(self.left_frame, text="Start")
+        self.button_start.grid(column=0, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
+        
+        
+    
+    def show(self):
+        self.mainloop()
+        self.lift()
+
+
+# %%
```

### Comparing `pydvma-0.9.0/pydvma/icon.png` & `pydvma-0.9.1/pydvma/icon.png`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.0/pydvma/modal.py` & `pydvma-0.9.1/pydvma/modal.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,363 +1,363 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Aug 19 17:29:30 2019
-
-@author: tb267
-"""
-
-
-from . import datastructure
-from . import options
-
-import numpy as np
-from scipy import signal
-from scipy import optimize
-import copy
-
-MESSAGE = ''
-
-#%% single peak fit
-
-def f_3dB(f,G0):
-    
-    ff = np.linspace(f[0],f[-1],np.max([len(f),1000]))
-    GG = np.interp(ff,f,np.squeeze(G0))
-    
-    f=ff
-    G0=GG
-    
-    
-    fn0i = np.argmax(np.abs(G0))
-    fn0 = f[fn0i]
-    
-    halfpower = np.max(np.abs(G0)) / np.sqrt(2)
-    
-    xi = np.where(np.squeeze(np.abs(G0)) > halfpower)[0]
-
-    
-    f1 = f[xi[0]]
-    f2 = f[xi[-1]]
-
-    
-    df = f2-f1
-    zn0 = df/2/fn0
-    
-    return fn0,zn0
-
-
-
-def modal_fit_single_channel(tf_data,freq_range=None,channel=0,measurement_type='acc'):
-    '''
-    Fit modal parameters for a single mode to data within specified freq_range
-    '''
-    
-    if freq_range == None:
-        freq_range = tf_data.freq_axis[[0,-1]]
-    
-    
-    f = tf_data.freq_axis
-    selected_range = np.where((f > freq_range[0]) & (f < freq_range[1]))
-    
-    f = f[selected_range]
-    
-    #NEED GOOD INITIAL GUESS!
-    G0 = tf_data.tf_data[selected_range,channel]
-    
-    fn0,zn0 = f_3dB(f,G0)
-    
-    
-    
-    an0 = np.max(np.abs(G0))*(2*np.pi*fn0)**2 * 2*zn0
-    pn0 = 0
-    Rk0 = np.max(np.abs(G0))/1e3
-    Rm0 = np.max(np.abs(G0))*((2*np.pi*fn0)**2)/1e3
-    
-    
-    #x0 = np.array([fn0,zn0,an0,pn0,Rk0,Rm0])
-    x0 = np.concatenate(([fn0],[zn0],an0,pn0,Rk0,Rm0))
-    
-    bounds = ([freq_range[0],0,-np.inf,-np.pi/2,0,0],[freq_range[1],1,np.inf,np.pi/2,np.inf,np.inf])
-#    bounds = ((-np.inf,np.inf),(freq_range[0],freq_range[1]),(0,np.inf),(-np.pi/2,np.pi/2),(-np.inf,np.inf),(-np.inf,np.inf))
-    
-    r = optimize.least_squares(f_residual,x0, bounds=bounds, max_nfev=1000, args=(f,G0,measurement_type))
-#    r = optimize.minimize(f_residual,x0, bounds=bounds, method='SLSQP', args=(f,G0,measurement_type))
-    print('')
-    print('fn={:.4g} (Hz), zn={:.4g}, an={:.4g}, phase={:.4g} (deg)'.format(r.x[0],r.x[1],r.x[2],r.x[3]*180/np.pi))
-    print('')
-    if (np.abs(r.x[3])*180/np.pi > 60):
-        print('Phase is significant, check ''measurement_type'' setting is correct')
-    return r
-    
-    
-
-def f_TF(x,f,measurement_type):
-
-    fn = x[0]
-    zn = x[1]
-    an = x[2]
-    pn = x[3]
-#    R  = x[4] + 1j*x[5]
-    R1 = x[4]
-    R2 = x[5]
-    
-    wn = 2*np.pi*fn
-    w = 2*np.pi*f
-    
-    
-    if measurement_type == 'acc':
-        p = 2
-    elif measurement_type == 'vel':
-        p = 1
-    elif measurement_type == 'dsp':
-        p = 0
-    
-    G = an*np.exp(1j*pn)/(wn**2 + 2j*wn*zn*w - w**2) + R1 - R2/(w**2)
-    G = G*((1j*w)**p)
-    
-    return G
-
-
-
-def f_residual(x,f,G0,measurement_type):
-    
-    G0 = np.squeeze(G0)
-    G = f_TF(x,f,measurement_type)
-        
-    e = (G-G0)
-    #e = np.abs(e)
-    e = np.concatenate((np.real(e),np.imag(e)))
-    
-    
-    return e
-
-
-
-#%%
-def f_TF_all_channels(x,f,measurement_type):
-
-    N_tfs = int((len(x)-2)/4)
-    
-    fn = x[0]
-    zn = x[1]
-    an = x[2:2+N_tfs].reshape(1,N_tfs)
-    pn = x[2+N_tfs:2+2*N_tfs].reshape(1,N_tfs)
-#    R  = x[4] + 1j*x[5]
-    R1 = x[2+2*N_tfs:2+3*N_tfs].reshape(1,N_tfs)
-    R2 = x[2+3*N_tfs:2+4*N_tfs].reshape(1,N_tfs)
-    
-    wn = 2*np.pi*fn
-    w = 2*np.pi*f
-    w = w.reshape(len(w),1)
-    
-    
-    if measurement_type == 'acc':
-        p = 2
-    elif measurement_type == 'vel':
-        p = 1
-    elif measurement_type == 'dsp':
-        p = 0
-
-    if w[0]==0:
-        # avoid singularity at w=0
-        w[0] = w[1]
-    G = an*np.exp(1j*pn)/(wn**2 + 2j*wn*zn*w - w**2) + R1 - R2/(w**2)
-    G = G*((1j*w)**p)
-    
-    return G
-
-
-def f_residual_all_channels(x,f,G0,measurement_type):
-    
-    G = f_TF_all_channels(x,f,measurement_type)
-        
-    e = (G-G0)
-    #e = np.abs(e)
-    e = np.concatenate((np.real(e),np.imag(e)))
-    e = e.reshape(np.size(e))
-    
-    return e
-
-#%% MULTI-CHANNEL MODAL FIT
-def modal_fit_all_channels(tf_data_list,freq_range=None,measurement_type='acc'):
-    '''
-    Fit modal parameters for a single mode to data within specified freq_range.
-    
-    Assumes all tf_data in tf_data_list have same frequency axes
-    '''
-    global MESSAGE
-    
-    if measurement_type == 'acc':
-        p = 2
-    elif measurement_type == 'vel':
-        p = 1
-    elif measurement_type == 'dsp':
-        p = 0
-    
-    # Find out how many TFs in dataset
-    N_tfs = 0
-    for tf_data in tf_data_list:
-        if tf_data.flag_modal_TF == False:
-            N_tfs += len(tf_data.tf_data[0,:])
-    
-    if freq_range == None:
-        freq_range = tf_data.freq_axis[[0,-1]]
-    
-    # get selected frequency axis
-    f = tf_data_list[0].freq_axis
-    selected_range = np.where((f > freq_range[0]) & (f < freq_range[1]))
-    
-    f = f[selected_range]
-    
-    # compile transfer functions into single array, and get initial guesses
-    G0 = np.zeros((len(f),N_tfs),dtype=complex)
-    fn0 = np.zeros(N_tfs)
-    zn0 = np.zeros(N_tfs)
-    counter = -1
-    for tf_data in tf_data_list:
-        if tf_data.flag_modal_TF == False:
-            for n_chan in range(len(tf_data.tf_data[0,:])):
-                counter += 1
-                G0[:,counter] = tf_data.tf_data[selected_range,n_chan] * tf_data.channel_cal_factors[n_chan]
-                fn0[counter],zn0[counter] = f_3dB(f,G0[:,counter])
-            
-
-    # initial global guess for fn0,zn0 discarding any outliers
-    fn0 = np.median(fn0)
-    zn0 = np.median(zn0)
-    fn0i = np.argmin(np.abs(f - fn0))
-    
-    
-    # initial guesses for each channel
-    an0 = np.zeros(N_tfs)
-    pn0 = np.zeros(N_tfs)
-    Rk0 = np.zeros(N_tfs)
-    Rm0 = np.zeros(N_tfs)
-    id_link = []
-    counter = -1
-    for tf_data in tf_data_list:
-        if tf_data.flag_modal_TF == False:
-            id_link += [tf_data.id_link]
-            for n_chan in range(len(tf_data.tf_data[0,:])):
-                counter += 1
-                an0[counter] = np.max(np.abs(G0[:,counter]))*(2*np.pi*fn0)**(2-p) * 2*zn0
-    #            an0[counter] = an0[counter] * np.sign(np.real(G0[fn0i,counter] / ((2j*np.pi*fn0)**p)))
-                an0[counter] = an0[counter] * np.sign(-np.imag(G0[fn0i,counter] / ((1j)**p)))
-                
-                pn0[counter] = 0
-                Rk0[counter] = np.max(np.abs(G0[:,counter]))/1e6
-                Rm0[counter] = np.max(np.abs(G0[:,counter]))*((2*np.pi*fn0)**2)/1e6
-    
-    x0 = np.concatenate(([fn0],[zn0],an0,pn0,Rk0,Rm0))
-    
-    
-    # bounds
-    B_fn = freq_range
-    B_zn = [0,1]
-    B_an = np.zeros((N_tfs,2))
-    B_an[:,0] = -np.inf
-    B_an[:,1] =  np.inf
-    B_pn = np.zeros((N_tfs,2))
-    B_pn[:,0] = -np.pi/2
-    B_pn[:,1] =  np.pi/2
-    B_rk = np.zeros((N_tfs,2))
-    B_rk[:,0] = 0
-    B_rk[:,1] = np.inf
-    B_rm = np.copy(B_rk)
-    
-    lower_bounds = np.concatenate(([B_fn[0]],[B_zn[0]],B_an[:,0],B_pn[:,0],B_rk[:,0],B_rm[:,0]))
-    upper_bounds = np.concatenate(([B_fn[1]],[B_zn[1]],B_an[:,1],B_pn[:,1],B_rk[:,1],B_rm[:,1]))
-    
-    bounds = (lower_bounds,upper_bounds)
-    
-    r = optimize.least_squares(f_residual_all_channels,x0, bounds=bounds, max_nfev=1000, args=(f,G0,measurement_type))
-    
-    settings = tf_data_list[0].settings
-    test_name = tf_data_list[0].test_name
-    m = datastructure.ModalData(r.x, settings=settings, id_link=id_link, test_name=test_name)
-
-    fn,zn,an,pn,rk,rm = unpack(r.x)
-
-#    with np.printoptions(precision=3, suppress=True):
-    MESSAGE = 'fn={:.2f} (Hz), zn={:.3g}, Qn = 1/(2 zn) = {:.1f}\n\n'.format(fn,zn,1/2/zn)
-    MESSAGE += 'an={}\n\n'.format(np.array2string(an,precision=3))
-    MESSAGE += 'pn={} deg\n\n'.format(np.array2string(pn*180/np.pi,precision=2))
-    print(MESSAGE)
-    if np.any(np.abs(pn)*180/np.pi > 60):
-        MESSAGE += '\nPhase is significant, check ''TF type'' setting is correct.\n'
-        print(MESSAGE)
-        
-    # Check quality of fit
-    e = f_residual_all_channels(r.x,f,G0,measurement_type)
-    G0rms = np.mean(np.abs(G0)**2)
-    erms = np.mean(np.abs(e)**2)
-    e_rel = erms/G0rms
-    if e_rel > 0.1:
-        MESSAGE += '\nPoor quality fit: try adjusting frequency range.\n'
-        print(MESSAGE)
-
-    return m
-    
-#%%% Reconstruction
-def unpack(x):
-    # unpacks modal parameters into set of variables
-    N_tfs = int((len(x)-2)/4)
-    
-    fn = x[0]
-    zn = x[1]
-    an = x[2:2+N_tfs]
-    pn = x[2+N_tfs:2+2*N_tfs]
-    rk = x[2+2*N_tfs:2+3*N_tfs]
-    rm = x[2+3*N_tfs:2+4*N_tfs]
-    
-    return fn,zn,an,pn,rk,rm
-
-def unpack_matrix(X):
-    # unpacks modal parameters into set of variables
-    N_tfs = int((len(X[0,:])-2)/4)
-
-    fn = X[:,0]
-    zn = X[:,1]
-    an = X[:,2:2+N_tfs]
-    pn = X[:,2+N_tfs:2+2*N_tfs]
-    rk = X[:,2+2*N_tfs:2+3*N_tfs]
-    rm = X[:,2+3*N_tfs:2+4*N_tfs]
-
-    return fn,zn,an,pn,rk,rm
-    
-def pack(fn,zn,an,pn,rk,rm):
-    # packs modal parameters into single variable for optimisation
-    x = np.concatenate(([fn],[zn],an,pn,rk,rm))
-    return x
-    
-
-def reconstruct_transfer_function(modal_data,f,measurement_type='acc'):
-    '''
-    Reconstructs transfer functions from modal_data and returns TfData object
-    '''
-    G = 0
-    for n_row in range(len(modal_data.M[:,0])):
-        xn = modal_data.M[n_row,:]
-        G += f_TF_all_channels(xn,f,measurement_type=measurement_type)
-    
-    settings = modal_data.settings
-    settings.channels = modal_data.channels
-    tf_data = datastructure.TfData(f,G,None,settings,units=modal_data.units,channel_cal_factors=None,id_link=modal_data.id_link,test_name=modal_data.test_name)
-    tf_data.flag_modal_TF = True
-    return tf_data
-
-def reconstruct_transfer_function_global(modal_data,f,measurement_type='acc'):
-    '''
-    Reconstructs transfer functions from modal_data and returns TfData object
-    '''
-    G = 0
-    N_tfs = int((len(modal_data.M[0,:])-2)/4)
-    for n_row in range(len(modal_data.M[:,0])):
-        xn = modal_data.M[n_row,:]
-        xn[2+2*N_tfs:] = 0 #don't want local residual fits for global fits - i.e. rk and rm
-        G += f_TF_all_channels(xn,f,measurement_type=measurement_type)
-    
-    settings = modal_data.settings
-    settings.channels = modal_data.channels
-    tf_data = datastructure.TfData(f,G,None,settings,units=modal_data.units,channel_cal_factors=None,id_link=modal_data.id_link,test_name=modal_data.test_name)
-    tf_data.flag_modal_TF = True
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Aug 19 17:29:30 2019
+
+@author: tb267
+"""
+
+
+from . import datastructure
+from . import options
+
+import numpy as np
+from scipy import signal
+from scipy import optimize
+import copy
+
+MESSAGE = ''
+
+#%% single peak fit
+
+def f_3dB(f,G0):
+    
+    ff = np.linspace(f[0],f[-1],np.max([len(f),1000]))
+    GG = np.interp(ff,f,np.squeeze(G0))
+    
+    f=ff
+    G0=GG
+    
+    
+    fn0i = np.argmax(np.abs(G0))
+    fn0 = f[fn0i]
+    
+    halfpower = np.max(np.abs(G0)) / np.sqrt(2)
+    
+    xi = np.where(np.squeeze(np.abs(G0)) > halfpower)[0]
+
+    
+    f1 = f[xi[0]]
+    f2 = f[xi[-1]]
+
+    
+    df = f2-f1
+    zn0 = df/2/fn0
+    
+    return fn0,zn0
+
+
+
+def modal_fit_single_channel(tf_data,freq_range=None,channel=0,measurement_type='acc'):
+    '''
+    Fit modal parameters for a single mode to data within specified freq_range
+    '''
+    
+    if freq_range == None:
+        freq_range = tf_data.freq_axis[[0,-1]]
+    
+    
+    f = tf_data.freq_axis
+    selected_range = np.where((f > freq_range[0]) & (f < freq_range[1]))
+    
+    f = f[selected_range]
+    
+    #NEED GOOD INITIAL GUESS!
+    G0 = tf_data.tf_data[selected_range,channel]
+    
+    fn0,zn0 = f_3dB(f,G0)
+    
+    
+    
+    an0 = np.max(np.abs(G0))*(2*np.pi*fn0)**2 * 2*zn0
+    pn0 = 0
+    Rk0 = np.max(np.abs(G0))/1e3
+    Rm0 = np.max(np.abs(G0))*((2*np.pi*fn0)**2)/1e3
+    
+    
+    #x0 = np.array([fn0,zn0,an0,pn0,Rk0,Rm0])
+    x0 = np.concatenate(([fn0],[zn0],an0,pn0,Rk0,Rm0))
+    
+    bounds = ([freq_range[0],0,-np.inf,-np.pi/2,0,0],[freq_range[1],1,np.inf,np.pi/2,np.inf,np.inf])
+#    bounds = ((-np.inf,np.inf),(freq_range[0],freq_range[1]),(0,np.inf),(-np.pi/2,np.pi/2),(-np.inf,np.inf),(-np.inf,np.inf))
+    
+    r = optimize.least_squares(f_residual,x0, bounds=bounds, max_nfev=1000, args=(f,G0,measurement_type))
+#    r = optimize.minimize(f_residual,x0, bounds=bounds, method='SLSQP', args=(f,G0,measurement_type))
+    print('')
+    print('fn={:.4g} (Hz), zn={:.4g}, an={:.4g}, phase={:.4g} (deg)'.format(r.x[0],r.x[1],r.x[2],r.x[3]*180/np.pi))
+    print('')
+    if (np.abs(r.x[3])*180/np.pi > 60):
+        print('Phase is significant, check ''measurement_type'' setting is correct')
+    return r
+    
+    
+
+def f_TF(x,f,measurement_type):
+
+    fn = x[0]
+    zn = x[1]
+    an = x[2]
+    pn = x[3]
+#    R  = x[4] + 1j*x[5]
+    R1 = x[4]
+    R2 = x[5]
+    
+    wn = 2*np.pi*fn
+    w = 2*np.pi*f
+    
+    
+    if measurement_type == 'acc':
+        p = 2
+    elif measurement_type == 'vel':
+        p = 1
+    elif measurement_type == 'dsp':
+        p = 0
+    
+    G = an*np.exp(1j*pn)/(wn**2 + 2j*wn*zn*w - w**2) + R1 - R2/(w**2)
+    G = G*((1j*w)**p)
+    
+    return G
+
+
+
+def f_residual(x,f,G0,measurement_type):
+    
+    G0 = np.squeeze(G0)
+    G = f_TF(x,f,measurement_type)
+        
+    e = (G-G0)
+    #e = np.abs(e)
+    e = np.concatenate((np.real(e),np.imag(e)))
+    
+    
+    return e
+
+
+
+#%%
+def f_TF_all_channels(x,f,measurement_type):
+
+    N_tfs = int((len(x)-2)/4)
+    
+    fn = x[0]
+    zn = x[1]
+    an = x[2:2+N_tfs].reshape(1,N_tfs)
+    pn = x[2+N_tfs:2+2*N_tfs].reshape(1,N_tfs)
+#    R  = x[4] + 1j*x[5]
+    R1 = x[2+2*N_tfs:2+3*N_tfs].reshape(1,N_tfs)
+    R2 = x[2+3*N_tfs:2+4*N_tfs].reshape(1,N_tfs)
+    
+    wn = 2*np.pi*fn
+    w = 2*np.pi*f
+    w = w.reshape(len(w),1)
+    
+    
+    if measurement_type == 'acc':
+        p = 2
+    elif measurement_type == 'vel':
+        p = 1
+    elif measurement_type == 'dsp':
+        p = 0
+
+    if w[0]==0:
+        # avoid singularity at w=0
+        w[0] = w[1]
+    G = an*np.exp(1j*pn)/(wn**2 + 2j*wn*zn*w - w**2) + R1 - R2/(w**2)
+    G = G*((1j*w)**p)
+    
+    return G
+
+
+def f_residual_all_channels(x,f,G0,measurement_type):
+    
+    G = f_TF_all_channels(x,f,measurement_type)
+        
+    e = (G-G0)
+    #e = np.abs(e)
+    e = np.concatenate((np.real(e),np.imag(e)))
+    e = e.reshape(np.size(e))
+    
+    return e
+
+#%% MULTI-CHANNEL MODAL FIT
+def modal_fit_all_channels(tf_data_list,freq_range=None,measurement_type='acc'):
+    '''
+    Fit modal parameters for a single mode to data within specified freq_range.
+    
+    Assumes all tf_data in tf_data_list have same frequency axes
+    '''
+    global MESSAGE
+    
+    if measurement_type == 'acc':
+        p = 2
+    elif measurement_type == 'vel':
+        p = 1
+    elif measurement_type == 'dsp':
+        p = 0
+    
+    # Find out how many TFs in dataset
+    N_tfs = 0
+    for tf_data in tf_data_list:
+        if tf_data.flag_modal_TF == False:
+            N_tfs += len(tf_data.tf_data[0,:])
+    
+    if freq_range == None:
+        freq_range = tf_data.freq_axis[[0,-1]]
+    
+    # get selected frequency axis
+    f = tf_data_list[0].freq_axis
+    selected_range = np.where((f > freq_range[0]) & (f < freq_range[1]))
+    
+    f = f[selected_range]
+    
+    # compile transfer functions into single array, and get initial guesses
+    G0 = np.zeros((len(f),N_tfs),dtype=complex)
+    fn0 = np.zeros(N_tfs)
+    zn0 = np.zeros(N_tfs)
+    counter = -1
+    for tf_data in tf_data_list:
+        if tf_data.flag_modal_TF == False:
+            for n_chan in range(len(tf_data.tf_data[0,:])):
+                counter += 1
+                G0[:,counter] = tf_data.tf_data[selected_range,n_chan] * tf_data.channel_cal_factors[n_chan]
+                fn0[counter],zn0[counter] = f_3dB(f,G0[:,counter])
+            
+
+    # initial global guess for fn0,zn0 discarding any outliers
+    fn0 = np.median(fn0)
+    zn0 = np.median(zn0)
+    fn0i = np.argmin(np.abs(f - fn0))
+    
+    
+    # initial guesses for each channel
+    an0 = np.zeros(N_tfs)
+    pn0 = np.zeros(N_tfs)
+    Rk0 = np.zeros(N_tfs)
+    Rm0 = np.zeros(N_tfs)
+    id_link = []
+    counter = -1
+    for tf_data in tf_data_list:
+        if tf_data.flag_modal_TF == False:
+            id_link += [tf_data.id_link]
+            for n_chan in range(len(tf_data.tf_data[0,:])):
+                counter += 1
+                an0[counter] = np.max(np.abs(G0[:,counter]))*(2*np.pi*fn0)**(2-p) * 2*zn0
+    #            an0[counter] = an0[counter] * np.sign(np.real(G0[fn0i,counter] / ((2j*np.pi*fn0)**p)))
+                an0[counter] = an0[counter] * np.sign(-np.imag(G0[fn0i,counter] / ((1j)**p)))
+                
+                pn0[counter] = 0
+                Rk0[counter] = np.max(np.abs(G0[:,counter]))/1e6
+                Rm0[counter] = np.max(np.abs(G0[:,counter]))*((2*np.pi*fn0)**2)/1e6
+    
+    x0 = np.concatenate(([fn0],[zn0],an0,pn0,Rk0,Rm0))
+    
+    
+    # bounds
+    B_fn = freq_range
+    B_zn = [0,1]
+    B_an = np.zeros((N_tfs,2))
+    B_an[:,0] = -np.inf
+    B_an[:,1] =  np.inf
+    B_pn = np.zeros((N_tfs,2))
+    B_pn[:,0] = -np.pi/2
+    B_pn[:,1] =  np.pi/2
+    B_rk = np.zeros((N_tfs,2))
+    B_rk[:,0] = 0
+    B_rk[:,1] = np.inf
+    B_rm = np.copy(B_rk)
+    
+    lower_bounds = np.concatenate(([B_fn[0]],[B_zn[0]],B_an[:,0],B_pn[:,0],B_rk[:,0],B_rm[:,0]))
+    upper_bounds = np.concatenate(([B_fn[1]],[B_zn[1]],B_an[:,1],B_pn[:,1],B_rk[:,1],B_rm[:,1]))
+    
+    bounds = (lower_bounds,upper_bounds)
+    
+    r = optimize.least_squares(f_residual_all_channels,x0, bounds=bounds, max_nfev=1000, args=(f,G0,measurement_type))
+    
+    settings = tf_data_list[0].settings
+    test_name = tf_data_list[0].test_name
+    m = datastructure.ModalData(r.x, settings=settings, id_link=id_link, test_name=test_name)
+
+    fn,zn,an,pn,rk,rm = unpack(r.x)
+
+#    with np.printoptions(precision=3, suppress=True):
+    MESSAGE = 'fn={:.2f} (Hz), zn={:.3g}, Qn = 1/(2 zn) = {:.1f}\n\n'.format(fn,zn,1/2/zn)
+    MESSAGE += 'an={}\n\n'.format(np.array2string(an,precision=3))
+    MESSAGE += 'pn={} deg\n\n'.format(np.array2string(pn*180/np.pi,precision=2))
+    print(MESSAGE)
+    if np.any(np.abs(pn)*180/np.pi > 60):
+        MESSAGE += '\nPhase is significant, check ''TF type'' setting is correct.\n'
+        print(MESSAGE)
+        
+    # Check quality of fit
+    e = f_residual_all_channels(r.x,f,G0,measurement_type)
+    G0rms = np.mean(np.abs(G0)**2)
+    erms = np.mean(np.abs(e)**2)
+    e_rel = erms/G0rms
+    if e_rel > 0.1:
+        MESSAGE += '\nPoor quality fit: try adjusting frequency range.\n'
+        print(MESSAGE)
+
+    return m
+    
+#%%% Reconstruction
+def unpack(x):
+    # unpacks modal parameters into set of variables
+    N_tfs = int((len(x)-2)/4)
+    
+    fn = x[0]
+    zn = x[1]
+    an = x[2:2+N_tfs]
+    pn = x[2+N_tfs:2+2*N_tfs]
+    rk = x[2+2*N_tfs:2+3*N_tfs]
+    rm = x[2+3*N_tfs:2+4*N_tfs]
+    
+    return fn,zn,an,pn,rk,rm
+
+def unpack_matrix(X):
+    # unpacks modal parameters into set of variables
+    N_tfs = int((len(X[0,:])-2)/4)
+
+    fn = X[:,0]
+    zn = X[:,1]
+    an = X[:,2:2+N_tfs]
+    pn = X[:,2+N_tfs:2+2*N_tfs]
+    rk = X[:,2+2*N_tfs:2+3*N_tfs]
+    rm = X[:,2+3*N_tfs:2+4*N_tfs]
+
+    return fn,zn,an,pn,rk,rm
+    
+def pack(fn,zn,an,pn,rk,rm):
+    # packs modal parameters into single variable for optimisation
+    x = np.concatenate(([fn],[zn],an,pn,rk,rm))
+    return x
+    
+
+def reconstruct_transfer_function(modal_data,f,measurement_type='acc'):
+    '''
+    Reconstructs transfer functions from modal_data and returns TfData object
+    '''
+    G = 0
+    for n_row in range(len(modal_data.M[:,0])):
+        xn = modal_data.M[n_row,:]
+        G += f_TF_all_channels(xn,f,measurement_type=measurement_type)
+    
+    settings = modal_data.settings
+    settings.channels = modal_data.channels
+    tf_data = datastructure.TfData(f,G,None,settings,units=modal_data.units,channel_cal_factors=None,id_link=modal_data.id_link,test_name=modal_data.test_name)
+    tf_data.flag_modal_TF = True
+    return tf_data
+
+def reconstruct_transfer_function_global(modal_data,f,measurement_type='acc'):
+    '''
+    Reconstructs transfer functions from modal_data and returns TfData object
+    '''
+    G = 0
+    N_tfs = int((len(modal_data.M[0,:])-2)/4)
+    for n_row in range(len(modal_data.M[:,0])):
+        xn = modal_data.M[n_row,:]
+        xn[2+2*N_tfs:] = 0 #don't want local residual fits for global fits - i.e. rk and rm
+        G += f_TF_all_channels(xn,f,measurement_type=measurement_type)
+    
+    settings = modal_data.settings
+    settings.channels = modal_data.channels
+    tf_data = datastructure.TfData(f,G,None,settings,units=modal_data.units,channel_cal_factors=None,id_link=modal_data.id_link,test_name=modal_data.test_name)
+    tf_data.flag_modal_TF = True
     return tf_data
```

### Comparing `pydvma-0.9.0/pydvma/options.py` & `pydvma-0.9.1/pydvma/options.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Aug 27 13:28:39 2018
-
-@author: tb267
-"""
-
-from . import streams
-
-import numpy as np
-
-import pyqtgraph as pg
-import matplotlib.pyplot as plt
-import seaborn as sns
-
-# try:
-#     import pyaudio
-# except ImportError:
-#     pyaudio = None
-# except NotImplementedError:
-#     pyaudio = None
-
-
-try:
-    import sounddevice as sd
-except ImportError:
-    sd = None
-except NotImplementedError:
-    sd = None
-
-class MySettings(object):
-    '''
-    A class that stores the acquisition settings.
-    
-    Attributes:
-    --------------       
-    channels: int
-        Number of Channels
-    fs: int
-        Sampling Frequency
-    nbits: int
-        Number of bits - either 8, 16, 24 or 32
-    chunk_size: int
-        Number of samples obtained from each channel in one chunk
-    num_chunks: int
-        Number of chunks to store in circular buffer
-    view_time: float
-        If specified, overrides num_chunks to display view_time in seconds for oscilloscope
-    stored_time: float
-        Length of the pre-trigger when the space button is hit, in seconds
-    device_index: int
-        device index, will prompt if not specified
-    init_view_time: bool
-        flag for time domain view in oscilloscope
-    init_view_freq: bool
-        flag for frequency domain view in oscilloscope
-    init_view_levels: bool
-        flag for channel levels view in oscilloscope
-    '''
-        
-    def __init__(self, *, 
-                 channels=2, 
-                 fs=44100, 
-                 nbits=16, 
-                 chunk_size=100, 
-                 num_chunks=6,
-                 viewed_time=0.3,
-                 stored_time=2,
-                 pretrig_samples=None,
-                 pretrig_threshold=0.05,
-                 pretrig_channel=0,
-                 pretrig_timeout=20,
-                 device_driver='soundcard',
-                 device_index=None,
-                 VmaxNI=5,
-                 NI_mode='DAQmx_Val_RSE',
-                 init_view_time=True,
-                 init_view_freq=True,
-                 init_view_levels=True,
-                 output_device_driver=None,
-                 output_device_index=None,
-                 output_channels=None,
-                 output_fs=None,
-                 use_output_as_ch0=False):
-        
-        #INPUT SETTINGS
-        self.fs=int(fs)
-        self.channels=int(channels)
-        self.stored_time=float(stored_time)
-        
-        if pretrig_samples is not None:
-            self.pretrig_samples=int(pretrig_samples)
-        else:
-            self.pretrig_samples=None
-        
-        self.pretrig_threshold=float(pretrig_threshold)
-        self.pretrig_channel=int(pretrig_channel)
-        self.pretrig_timeout=float(pretrig_timeout)
-        
-        self.device_driver=device_driver
-        self.device_index=device_index
-        
-        
-        
-        #OUTPUT SETTINGS
-        if (output_fs is None) or (output_fs == 'None'):
-            self.output_fs = int(self.fs)
-        else:
-            self.output_fs = int(output_fs)
-            
-        if (output_channels is None) or (output_channels == 'None'):
-            self.output_channels = int(1)
-        else:
-            self.output_channels = int(output_channels)
-            
-        # if output device driver not specified then use same as input device
-        if (output_device_driver == None) or (output_device_driver == 'None'):
-            output_device_driver = device_driver
-
-        self.output_device_driver = output_device_driver
-            
-        if (device_driver == 'soundcard') and ((device_index == None) or (device_index == 'None')):
-            try:
-                # try to find default input soundcard device
-                self.device_index = sd.default.device[0]
-            except:
-                # if info not available, select index 1
-                self.device_index = 1
-        elif (device_driver == 'nidaq') and ((device_index == None) or (device_index == 'None')):
-            self.device_index = 0
-        else:
-            self.device_index = int(device_index)
-
-       
-                
-        # set output device index to defaults if not specified
-        if (output_device_driver == 'soundcard') and ((output_device_index == None) or  (output_device_index == 'None')):
-            try:
-                # try to find default output soundcard device
-                self.output_device_index = sd.default.device[1]
-            except:
-                # try to guess sensible default output soundcard by string matching device names
-                devices = streams.get_devices_soundcard()
-                if devices != None:
-                    output_devices = np.where(['output' in names for names in devices])
-                    self.output_device_index = output_devices[0][0]
-                else:
-                    self.output_device_index = 1
-        elif (output_device_driver == 'nidaq') and ((output_device_index == None) or (output_device_index == 'None')):
-            self.output_device_index = 0
-        else:
-            self.output_device_index = int(output_device_index)
-        
-        self.use_output_as_ch0 = bool(use_output_as_ch0)
-
-        
-        # ADVANCED SETTINGS
-        self.VmaxNI=float(VmaxNI)
-        self.NI_mode=NI_mode
-        self.chunk_size=int(chunk_size)
-        self.num_chunks=int(num_chunks)
-        self.viewed_time=float(viewed_time)
-        self.nbits=int(nbits)
-        self.init_view_time=bool(init_view_time)
-        self.init_view_freq=bool(init_view_freq)
-        self.init_view_levels=bool(init_view_levels)
-
-        ### derived settings
-        if (viewed_time != None) and (viewed_time != 'None'):
-            self.viewed_time = float(viewed_time)
-            self.num_chunks = int(np.ceil(self.viewed_time*self.fs/self.chunk_size))
-        else:
-            self.viewed_time = None
-        
-        if self.chunk_size < 10:
-            self.chunk_size = int(10)
-            print('Resetting ''chunk_size'' to minimum value of 10')
-            
-        try:    
-            self.format = eval('int'+str(self.nbits))
-        except:
-            pass
-        
-        self.device_name = None # until initialise stream
-        
-        if (pretrig_samples == None) or (pretrig_samples == 'None'):
-            self.pretrig_samples = None
-        else:
-            self.pretrig_samples = int(pretrig_samples)
-            if self.pretrig_samples > self.chunk_size:
-                raise Exception('pretrig_samples must be less than or equal to chunk_size (chunk_size={}).'.format(self.chunk_size))
-        
-            
-        
-    
-    def __repr__(self):
-        template = "{:>24}: {}" # column widths: 8, 10, 15, 7, 10
-        #print template.format("CLASSID", "DEPT", "COURSE NUMBER", "AREA", "TITLE") # header
-        settings_dict = self.__dict__
-        text = '\n<MySettings class>\n\n'
-        for attr in settings_dict: 
-            text += template.format(attr,settings_dict[attr])
-            text += '\n'
-        
-        return text
-
-        
-        
-def set_plot_colours(channels):
-    '''
-    Returns a list of RGB colours depending on the number of channels required.
-    '''
-    #TODO: Accessible colours
-    if channels <= 1:
-        cmap = plt.get_cmap('tab10')
-#        cmap = sns.color_palette('paired')
-        c_list = np.array((np.array(cmap.colors) * 255),dtype=int)
-    else:
-#        cmap = plt.get_cmap('plasma')
-#        v = np.linspace(0,1,channels)
-#        c_list = np.array(cmap(v) * 255,dtype=int)
-        cmap = sns.hls_palette(channels, l=.3, s=1)
-        c_list = np.array(np.array(cmap) * 255,dtype=int)
-    
-#    val = [0.0,0.5,1.0]
-#    colour = np.array([[255,0,0,255],[0,255,0,255],[0,0,255,255]], dtype = np.ubyte)
-#    plot_colourmap =  pg.ColorMap(val,colour)
-#    c_list = plot_colourmap.getLookupTable(nPts =channels,alpha=True)
-    return c_list 
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Aug 27 13:28:39 2018
+
+@author: tb267
+"""
+
+from . import streams
+
+import numpy as np
+
+import pyqtgraph as pg
+import matplotlib.pyplot as plt
+import seaborn as sns
+
+# try:
+#     import pyaudio
+# except ImportError:
+#     pyaudio = None
+# except NotImplementedError:
+#     pyaudio = None
+
+
+try:
+    import sounddevice as sd
+except ImportError:
+    sd = None
+except NotImplementedError:
+    sd = None
+
+class MySettings(object):
+    '''
+    A class that stores the acquisition settings.
+    
+    Attributes:
+    --------------       
+    channels: int
+        Number of Channels
+    fs: int
+        Sampling Frequency
+    nbits: int
+        Number of bits - either 8, 16, 24 or 32
+    chunk_size: int
+        Number of samples obtained from each channel in one chunk
+    num_chunks: int
+        Number of chunks to store in circular buffer
+    view_time: float
+        If specified, overrides num_chunks to display view_time in seconds for oscilloscope
+    stored_time: float
+        Length of the pre-trigger when the space button is hit, in seconds
+    device_index: int
+        device index, will prompt if not specified
+    init_view_time: bool
+        flag for time domain view in oscilloscope
+    init_view_freq: bool
+        flag for frequency domain view in oscilloscope
+    init_view_levels: bool
+        flag for channel levels view in oscilloscope
+    '''
+        
+    def __init__(self, *, 
+                 channels=2, 
+                 fs=44100, 
+                 nbits=16, 
+                 chunk_size=100, 
+                 num_chunks=6,
+                 viewed_time=0.3,
+                 stored_time=2,
+                 pretrig_samples=None,
+                 pretrig_threshold=0.05,
+                 pretrig_channel=0,
+                 pretrig_timeout=20,
+                 device_driver='soundcard',
+                 device_index=None,
+                 VmaxNI=5,
+                 NI_mode='DAQmx_Val_RSE',
+                 init_view_time=True,
+                 init_view_freq=True,
+                 init_view_levels=True,
+                 output_device_driver=None,
+                 output_device_index=None,
+                 output_channels=None,
+                 output_fs=None,
+                 use_output_as_ch0=False):
+        
+        #INPUT SETTINGS
+        self.fs=int(fs)
+        self.channels=int(channels)
+        self.stored_time=float(stored_time)
+        
+        if (pretrig_samples is None) or (pretrig_samples == 'None'):
+            self.pretrig_samples=None
+        else:
+            self.pretrig_samples=int(pretrig_samples)
+        
+        self.pretrig_threshold=float(pretrig_threshold)
+        self.pretrig_channel=int(pretrig_channel)
+        self.pretrig_timeout=float(pretrig_timeout)
+        
+        self.device_driver=device_driver
+        self.device_index=device_index
+        
+        
+        
+        #OUTPUT SETTINGS
+        if (output_fs is None) or (output_fs == 'None'):
+            self.output_fs = int(self.fs)
+        else:
+            self.output_fs = int(output_fs)
+            
+        if (output_channels is None) or (output_channels == 'None'):
+            self.output_channels = int(1)
+        else:
+            self.output_channels = int(output_channels)
+            
+        # if output device driver not specified then use same as input device
+        if (output_device_driver == None) or (output_device_driver == 'None'):
+            output_device_driver = device_driver
+
+        self.output_device_driver = output_device_driver
+            
+        if (device_driver == 'soundcard') and ((device_index == None) or (device_index == 'None')):
+            try:
+                # try to find default input soundcard device
+                self.device_index = sd.default.device[0]
+            except:
+                # if info not available, select index 1
+                self.device_index = 1
+        elif (device_driver == 'nidaq') and ((device_index == None) or (device_index == 'None')):
+            self.device_index = 0
+        else:
+            self.device_index = int(device_index)
+
+       
+                
+        # set output device index to defaults if not specified
+        if (output_device_driver == 'soundcard') and ((output_device_index == None) or  (output_device_index == 'None')):
+            try:
+                # try to find default output soundcard device
+                self.output_device_index = sd.default.device[1]
+            except:
+                # try to guess sensible default output soundcard by string matching device names
+                devices = streams.get_devices_soundcard()
+                if devices != None:
+                    output_devices = np.where(['output' in names for names in devices])
+                    self.output_device_index = output_devices[0][0]
+                else:
+                    self.output_device_index = 1
+        elif (output_device_driver == 'nidaq') and ((output_device_index == None) or (output_device_index == 'None')):
+            self.output_device_index = 0
+        else:
+            self.output_device_index = int(output_device_index)
+        
+        self.use_output_as_ch0 = bool(use_output_as_ch0)
+
+        
+        # ADVANCED SETTINGS
+        self.VmaxNI=float(VmaxNI)
+        self.NI_mode=NI_mode
+        self.chunk_size=int(chunk_size)
+        self.num_chunks=int(num_chunks)
+        self.viewed_time=float(viewed_time)
+        self.nbits=int(nbits)
+        self.init_view_time=bool(init_view_time)
+        self.init_view_freq=bool(init_view_freq)
+        self.init_view_levels=bool(init_view_levels)
+
+        ### derived settings
+        if (viewed_time != None) and (viewed_time != 'None'):
+            self.viewed_time = float(viewed_time)
+            self.num_chunks = int(np.ceil(self.viewed_time*self.fs/self.chunk_size))
+        else:
+            self.viewed_time = None
+        
+        if self.chunk_size < 10:
+            self.chunk_size = int(10)
+            print('Resetting ''chunk_size'' to minimum value of 10')
+            
+        try:    
+            self.format = eval('int'+str(self.nbits))
+        except:
+            pass
+        
+        self.device_name = None # until initialise stream
+        
+        if (pretrig_samples == None) or (pretrig_samples == 'None'):
+            self.pretrig_samples = None
+        else:
+            self.pretrig_samples = int(pretrig_samples)
+            if self.pretrig_samples > self.chunk_size:
+                raise Exception('pretrig_samples must be less than or equal to chunk_size (chunk_size={}).'.format(self.chunk_size))
+        
+            
+        
+    
+    def __repr__(self):
+        template = "{:>24}: {}" # column widths: 8, 10, 15, 7, 10
+        #print template.format("CLASSID", "DEPT", "COURSE NUMBER", "AREA", "TITLE") # header
+        settings_dict = self.__dict__
+        text = '\n<MySettings class>\n\n'
+        for attr in settings_dict: 
+            text += template.format(attr,settings_dict[attr])
+            text += '\n'
+        
+        return text
+
+        
+        
+def set_plot_colours(channels):
+    '''
+    Returns a list of RGB colours depending on the number of channels required.
+    '''
+    #TODO: Accessible colours
+    if channels <= 1:
+        cmap = plt.get_cmap('tab10')
+#        cmap = sns.color_palette('paired')
+        c_list = np.array((np.array(cmap.colors) * 255),dtype=int)
+    else:
+#        cmap = plt.get_cmap('plasma')
+#        v = np.linspace(0,1,channels)
+#        c_list = np.array(cmap(v) * 255,dtype=int)
+        cmap = sns.hls_palette(channels, l=.3, s=1)
+        c_list = np.array(np.array(cmap) * 255,dtype=int)
+    
+#    val = [0.0,0.5,1.0]
+#    colour = np.array([[255,0,0,255],[0,255,0,255],[0,0,255,255]], dtype = np.ubyte)
+#    plot_colourmap =  pg.ColorMap(val,colour)
+#    c_list = plot_colourmap.getLookupTable(nPts =channels,alpha=True)
+    return c_list
```

### Comparing `pydvma-0.9.0/pydvma/oscilloscope.py` & `pydvma-0.9.1/pydvma/oscilloscope.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Aug  3 11:27:29 2018
-
-@authors: ae407, tb267
-"""      
-import sys
-
-from . import options
-from . import file
-from . import datastructure
-from . import streams
-# from .gui import app
-
-import numpy as np
-import pyqtgraph as pg
-from qtpy import QtGui, QtCore
-from qtpy.QtCore import QObject, Signal, Qt
-
-import time
-import datetime
-
-
-class Oscilloscope():
-    def __init__(self, settings):
-        '''Creates an Oscilloscope
-        Args:
-            settings: An object of the class MySettings
-        '''
-
-        self.settings = settings
-        
-        streams.start_stream(settings)
-        self.rec = streams.REC
-        
-
-        self.timer = QtCore.QTimer()
-        self.create_figure()
-
-        self.win.sigKeyPress.connect(self.keyPressed)
-        self.win.sigClose.connect(self.on_close)
-
-        # Start the update timer
-        self.timer.timeout.connect(self.update) # update figure and buffer
-        self.timer.start(60)
-
-        if app.applicationState() != Qt.ApplicationActive:
-            app.exec()  
-
-    def create_figure(self):
-        '''
-        Creates a figure which is an object of the class KeyPressWindow.
-
-        '''
-        pg.setConfigOption('background', 'w')
-        self.win = KeyPressWindow()
-        self.win.setWindowIcon(QtGui.QIcon('icon.png'))
-#        window_geometry = self.win.geometry()
-        self.win.setGeometry(100,100,800,600)
-        self.win.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
-        
-        # This ensures the window appears at front.
-        self.win.showMinimized()
-        
-
-        self.win.setWindowTitle("Oscilloscope ('s': save new, 'space': autosave, 'p': pause, 'a': always top, 'y': autoscale)")
-        # time.sleep(0.6)
-        self.win.show()
-        self.win.showNormal()
-        self.win.raise_()
-
-        self.view_time = self.settings.init_view_time
-        self.view_freq = self.settings.init_view_freq
-        self.view_levels = self.settings.init_view_levels
-
-        self.toggle_view()
-        
-        self.auto_scale = False
-
-        self.data_saved_counter = 0 #  to indicate not yet saved file
-
-    def on_close(self, evt):
-        self.timer.stop()
-        # self.rec.end_stream()
-
-    def toggle_view(self):
-        '''
-        Switches between views, triggered by keypress
-        '''
-        self.win.clear()
-
-        if self.view_time:
-            self.time_plot()
-
-        if self.view_freq:
-            self.freq_plot()
-
-        if self.view_levels:
-            self.levels_plot()
-
-    def time_plot(self):
-        # create a plot for the time domain
-        self.view_time = True
-        self.win.nextRow()
-        self.osc_time_line = self.win.addPlot(title="Time Domain (toggle with 'T')")
-
-        if self.settings.channels == 1:
-            self.auto_scale = True
-            self.osc_time_line.enableAutoRange()
-        else:
-            # Stack the channels -- channel 0 is centred on 0, channel 1
-            # centred on 1 etc.
-            self.auto_scale = False
-            self.osc_time_line.setYRange(-1,self.settings.channels)
-
-        self.osc_time_line.setXRange(self.rec.osc_time_axis[0],
-                                     self.rec.osc_time_axis[-1])
-        self.osc_time_line.showGrid(True, True)
-        self.osc_time_line.addLegend()
-        self.osc_time_line.setLabel('left', 'Normalised Amplitude')
-        self.osc_time_line.setLabel('bottom', 'Time (s)')
-
-        self.ax_time = self.osc_time_line.getAxis('left')
-        self.ax_time.setTickSpacing(1, 1)
-
-        self.osc_time_lineset = {}
-        for i in range(self.settings.channels):
-            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:])
-            self.osc_time_lineset[i] = self.osc_time_line.plot(
-                pen=pen_, name='Channel %d' % i)
-
-#        self.win.FillBetweenItem(curve1=osc_time_lineset[0], curve2=osc_time_lineset[1])
-
-    def freq_plot(self):
-        # create a plot for the frequency domain
-        self.view_freq = True
-        self.win.nextRow()
-        self.osc_freq_line = self.win.addPlot(
-            title="Frequency Domain (toggle with 'F')")
-        self.osc_freq_line.enableAutoRange()
-        self.osc_freq_line.setXRange(self.rec.osc_freq_axis[0],
-                                     self.rec.osc_freq_axis[-1])
-        self.osc_freq_line.showGrid(True, True)
-        self.osc_freq_line.addLegend()
-        self.osc_freq_line.setLabel('left', 'Power Spectrum (dB)')
-        self.osc_freq_line.setLabel('bottom', 'Frequency (Hz)')
-
-        self.osc_freq_lineset = {}
-        for i in range(self.settings.channels):
-            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:])
-            self.osc_freq_lineset[i] = self.osc_freq_line.plot(
-                pen=pen_, name='Channel %d' % i)
-
-    def levels_plot(self):
-        # create a plot for the frequency domain
-        self.view_levels = True
-        self.win.nextRow()
-        self.osc_levels_line = self.win.addPlot(title="Channel Levels (toggle with 'L')")
-        self.osc_levels_line.setYRange(0, 1)
-        self.osc_levels_line.setXRange(-0.5, self.settings.channels - 0.5)
-        self.osc_levels_line.showGrid(False, True)
-        self.osc_levels_line.setLabel('left', 'Normalised Amplitude')
-        self.osc_levels_line.setLabel('bottom', 'Channel Index')
-
-        self.ax_levels = self.osc_levels_line.getAxis('bottom')
-        self.ax_levels.setTickSpacing(1, 1)
-#        ax.showLabel(show=True)
-#        self.osc_levels_line.setTicks(np.arange(self.settings.channels))
-        self.osc_levels_lineset={}
-        for i in range(self.settings.channels):
-            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
-            pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
-            self.osc_levels_lineset[i]=self.osc_levels_line.plot(pen=pen_, name='vertical')
-            self.osc_levels_lineset[self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_, name='top')
-            self.osc_levels_lineset[2*self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_peak, name='peak hold')
-#            self.osc_levels_lineset[3]=self.osc_levels_line.plot(pen=pen_, name='Channel')
-
-        self.osc_levels_peak_hold = np.zeros(self.settings.channels)
-        self.time_last_changed = np.zeros(self.settings.channels)
-
-    def update(self):
-        '''
-        Updates plots with incoming data from __call__.
-        Called with a 0s interval by QTimer.
-
-        '''
-        time_data_snapshot = np.copy(self.rec.osc_time_data)
-        if self.view_levels == True:
-            self.osc_levels_rms = np.sqrt(np.mean(time_data_snapshot**2,axis=0))
-            self.osc_levels_max = np.max(np.abs(time_data_snapshot),axis=0)
-            changed_indices = self.osc_levels_peak_hold < self.osc_levels_max
-            self.time_last_changed[changed_indices] = time.time()
-            self.osc_levels_peak_hold = np.maximum(self.osc_levels_peak_hold,self.osc_levels_max)
-            self.osc_levels_peak_hold[time.time()-self.time_last_changed>2] = 0
-
-        for i in range(self.settings.channels):
-            offset = i
-            if self.view_time == True:
-                if (self.auto_scale is True) and (self.settings.channels==1):
-                    shift = 0
-                    scale_factor = 1
-                    self.osc_time_line.enableAutoRange()
-                elif (self.auto_scale is True) and (self.settings.channels!=1):
-                    shift = np.mean(time_data_snapshot[:,i])
-                    scale_factor = np.max(np.abs(time_data_snapshot[:,i]-shift))*2
-                    self.osc_time_line.setYRange(-1,self.settings.channels)
-                else:
-                    shift = 0
-                    scale_factor = 1
-                    self.osc_time_line.setYRange(-1,self.settings.channels)
-                    
-                self.osc_time_lineset[i].setData(self.rec.osc_time_axis, (time_data_snapshot[:,i]-shift)/scale_factor + offset)
-
-            if self.view_freq == True:
-                # calculate the FFT
-                self.rec.osc_time_data_windowed[:,i] = time_data_snapshot[:,i] * np.blackman(np.shape(time_data_snapshot)[0])
-                fd = np.abs(np.fft.rfft(self.rec.osc_time_data_windowed[:,i]))/len(self.rec.osc_time_data_windowed[:,i])
-                fd[fd==0] = np.min(fd+1e-16) # to avoid log10(0) warnings
-                self.rec.osc_freq_data[:,i] = 20 * np.log10(fd)
-                self.osc_freq_lineset[i].setData(self.rec.osc_freq_axis,self.rec.osc_freq_data[:,i])
-
-            if self.view_levels == True:
-                self.osc_levels_lineset[i].setData([i,i],[0,self.osc_levels_max[i]])
-                self.osc_levels_lineset[self.settings.channels+i].setData([i-0.3,i+0.3],self.osc_levels_max[i]*np.ones(2))
-
-                if self.osc_levels_peak_hold[i] > 0.98:
-                    pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=10)
-                else:
-                    pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
-#                self.osc_levels_lineset[2*self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_peak, name='peak hold')
-                self.osc_levels_lineset[2*self.settings.channels+i].setData([i-0.3,i+0.3],self.osc_levels_peak_hold[i]*np.ones(2),pen=pen_peak)
-#                self.osc_levels_lineset[3].setData(np.arange(2),np.ones(2))
-
-
-
-    #KeyPressed function within osciolloscpe since can only take one argument
-    def keyPressed(self, evt):
-        '''
-        Upon a Space Bar press, makes a copy of data from the past stored_time seconds,plots it in Bokeh and gives the user an option to save it.
-        '''
-
-        if evt.key() == QtCore.Qt.Key_T:
-
-            if self.view_freq != False or self.view_levels != False:
-#                print('toggled time domain view')
-                self.view_time = not self.view_time
-                self.toggle_view()
-#            else:
-#                print('toggling all views off is prevented')
-
-        if evt.key() == QtCore.Qt.Key_F:
-
-            if self.view_time != False or self.view_levels != False:
-#                print('toggled frequency domain view')
-                self.view_freq = not self.view_freq
-                self.toggle_view()
-#            else:
-#                print('toggling all views off is prevented')
-
-        if evt.key() == QtCore.Qt.Key_L:
-            if self.view_time != False or self.view_freq != False:
-#                print('toggled levels view')
-                self.view_levels = not self.view_levels
-                self.toggle_view()
-#            else:
-#                print('toggling all views off is prevented')
-        
-        if evt.key() == QtCore.Qt.Key_P:
-            if self.timer.isActive():
-                self.timer.stop()
-            else:
-                self.timer.start()
-                
-        if evt.key() == QtCore.Qt.Key_A:
-            self.win.setWindowFlags(self.win.windowFlags() ^ QtCore.Qt.WindowStaysOnTopHint)       
-            self.win.show()
-                
-            
-        if evt.key() == QtCore.Qt.Key_Y:
-            self.auto_scale = not self.auto_scale 
-                
-        if evt.key() == QtCore.Qt.Key_Space or evt.key() == QtCore.Qt.Key_S:
-
-            stored_time_data_copy=np.copy(self.rec.stored_time_data)
-            t = datetime.datetime.now()
-            timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)
-#            print("key press trigger: saving data to file in working directory")
-
-            ### make into dataset
-            
-            fs=self.settings.fs
-            n_samp=len(stored_time_data_copy[:,0])
-            dt=1/fs
-            t_axis= np.arange(n_samp)*dt
-
-            
-            timedata = datastructure.TimeData(t_axis,stored_time_data_copy,self.settings,timestamp=t,timestring=timestring,test_name='Test_{}'.format(self.data_saved_counter))
-            
-            dataset = datastructure.DataSet()
-            dataset.add_to_dataset(timedata)
-            
-            
-            if evt.key() == QtCore.Qt.Key_S:
-                self.data_saved_counter = 1
-                self.last_filename = file.save_data(dataset,self.win)
-            
-#            # this version saves all data as new timedata objects within one file
-#            if evt.key() == QtCore.Qt.Key_Space:
-#                if self.data_saved_counter == 0:
-#                    self.last_filename = file.save_data(dataset)
-#                    if self.last_filename == '':
-#                        self.data_saved_counter = 0
-#                    else:
-#                        self.data_saved_counter += 1
-#                
-#                else:
-#                    d = file.load_data(self.last_filename)
-#                    d.add_to_dataset(timedata)
-#                    file.save_data(d,self.last_filename,overwrite_without_prompt=True)
-#                    self.data_saved_counter += 1
-            
-            # this version saves each new dataset to new file
-            if evt.key() == QtCore.Qt.Key_Space:
-                if self.data_saved_counter == 0:
-                    self.last_filename = file.save_data(dataset,self.win)
-                    if self.last_filename == '':
-                        self.data_saved_counter = 0
-                    else:
-                        self.data_saved_counter += 1
-                
-                else:
-                    d = datastructure.DataSet()
-                    d.add_to_dataset(timedata)
-                    filename = self.last_filename.replace('.npy','_'+str(self.data_saved_counter)+'.npy')
-                    file.save_data(d,self.win, filename,overwrite_without_prompt=True)
-                    self.data_saved_counter += 1
-
-class KeyPressWindow(pg.GraphicsLayoutWidget):
-    '''
-    A subclass of pyQtGraph GraphicsWindow that emits a signal when a key is pressed.
-
-    '''
-    sigKeyPress = Signal(object)
-    sigClose = Signal(object)
-
-    def __init__(self, *args, **kwargs):
-        '''
-        Re-implmented from parent.
-        '''
-        super().__init__(*args, **kwargs)
-
-    def keyPressEvent(self, evt):
-        '''
-        Emits a signal upon a key press
-        '''
-        self.scene().keyPressEvent(evt)
-        self.sigKeyPress.emit(evt)
-
-    def closeEvent(self, evt):
-        '''
-        Emits a signal when the window is closed.
-        '''
-        self.sigClose.emit(evt)
-        self.close()
+# -*- coding: utf-8 -*-
+"""
+Created on Fri Aug  3 11:27:29 2018
+
+@authors: ae407, tb267
+"""      
+import sys
+
+from . import options
+from . import file
+from . import datastructure
+from . import streams
+# from .gui import app
+
+import numpy as np
+import pyqtgraph as pg
+from qtpy import QtGui, QtCore
+from qtpy.QtCore import QObject, Signal, Qt
+
+import time
+import datetime
+
+
+class Oscilloscope():
+    def __init__(self, settings):
+        '''Creates an Oscilloscope
+        Args:
+            settings: An object of the class MySettings
+        '''
+
+        self.settings = settings
+        
+        streams.start_stream(settings)
+        self.rec = streams.REC
+        
+
+        self.timer = QtCore.QTimer()
+        self.create_figure()
+
+        self.win.sigKeyPress.connect(self.keyPressed)
+        self.win.sigClose.connect(self.on_close)
+
+        # Start the update timer
+        self.timer.timeout.connect(self.update) # update figure and buffer
+        self.timer.start(60)
+
+        if app.applicationState() != Qt.ApplicationActive:
+            app.exec()  
+
+    def create_figure(self):
+        '''
+        Creates a figure which is an object of the class KeyPressWindow.
+
+        '''
+        pg.setConfigOption('background', 'w')
+        self.win = KeyPressWindow()
+        self.win.setWindowIcon(QtGui.QIcon('icon.png'))
+#        window_geometry = self.win.geometry()
+        self.win.setGeometry(100,100,800,600)
+        self.win.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
+        
+        # This ensures the window appears at front.
+        self.win.showMinimized()
+        
+
+        self.win.setWindowTitle("Oscilloscope ('s': save new, 'space': autosave, 'p': pause, 'a': always top, 'y': autoscale)")
+        # time.sleep(0.6)
+        self.win.show()
+        self.win.showNormal()
+        self.win.raise_()
+
+        self.view_time = self.settings.init_view_time
+        self.view_freq = self.settings.init_view_freq
+        self.view_levels = self.settings.init_view_levels
+
+        self.toggle_view()
+        
+        self.auto_scale = False
+
+        self.data_saved_counter = 0 #  to indicate not yet saved file
+
+    def on_close(self, evt):
+        self.timer.stop()
+        # self.rec.end_stream()
+
+    def toggle_view(self):
+        '''
+        Switches between views, triggered by keypress
+        '''
+        self.win.clear()
+
+        if self.view_time:
+            self.time_plot()
+
+        if self.view_freq:
+            self.freq_plot()
+
+        if self.view_levels:
+            self.levels_plot()
+
+    def time_plot(self):
+        # create a plot for the time domain
+        self.view_time = True
+        self.win.nextRow()
+        self.osc_time_line = self.win.addPlot(title="Time Domain (toggle with 'T')")
+
+        if self.settings.channels == 1:
+            self.auto_scale = True
+            self.osc_time_line.enableAutoRange()
+        else:
+            # Stack the channels -- channel 0 is centred on 0, channel 1
+            # centred on 1 etc.
+            self.auto_scale = False
+            self.osc_time_line.setYRange(-1,self.settings.channels)
+
+        self.osc_time_line.setXRange(self.rec.osc_time_axis[0],
+                                     self.rec.osc_time_axis[-1])
+        self.osc_time_line.showGrid(True, True)
+        self.osc_time_line.addLegend()
+        self.osc_time_line.setLabel('left', 'Normalised Amplitude')
+        self.osc_time_line.setLabel('bottom', 'Time (s)')
+
+        self.ax_time = self.osc_time_line.getAxis('left')
+        self.ax_time.setTickSpacing(1, 1)
+
+        self.osc_time_lineset = {}
+        for i in range(self.settings.channels):
+            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:])
+            self.osc_time_lineset[i] = self.osc_time_line.plot(
+                pen=pen_, name='Channel %d' % i)
+
+#        self.win.FillBetweenItem(curve1=osc_time_lineset[0], curve2=osc_time_lineset[1])
+
+    def freq_plot(self):
+        # create a plot for the frequency domain
+        self.view_freq = True
+        self.win.nextRow()
+        self.osc_freq_line = self.win.addPlot(
+            title="Frequency Domain (toggle with 'F')")
+        self.osc_freq_line.enableAutoRange()
+        self.osc_freq_line.setXRange(self.rec.osc_freq_axis[0],
+                                     self.rec.osc_freq_axis[-1])
+        self.osc_freq_line.showGrid(True, True)
+        self.osc_freq_line.addLegend()
+        self.osc_freq_line.setLabel('left', 'Power Spectrum (dB)')
+        self.osc_freq_line.setLabel('bottom', 'Frequency (Hz)')
+
+        self.osc_freq_lineset = {}
+        for i in range(self.settings.channels):
+            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:])
+            self.osc_freq_lineset[i] = self.osc_freq_line.plot(
+                pen=pen_, name='Channel %d' % i)
+
+    def levels_plot(self):
+        # create a plot for the frequency domain
+        self.view_levels = True
+        self.win.nextRow()
+        self.osc_levels_line = self.win.addPlot(title="Channel Levels (toggle with 'L')")
+        self.osc_levels_line.setYRange(0, 1)
+        self.osc_levels_line.setXRange(-0.5, self.settings.channels - 0.5)
+        self.osc_levels_line.showGrid(False, True)
+        self.osc_levels_line.setLabel('left', 'Normalised Amplitude')
+        self.osc_levels_line.setLabel('bottom', 'Channel Index')
+
+        self.ax_levels = self.osc_levels_line.getAxis('bottom')
+        self.ax_levels.setTickSpacing(1, 1)
+#        ax.showLabel(show=True)
+#        self.osc_levels_line.setTicks(np.arange(self.settings.channels))
+        self.osc_levels_lineset={}
+        for i in range(self.settings.channels):
+            pen_ = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
+            pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
+            self.osc_levels_lineset[i]=self.osc_levels_line.plot(pen=pen_, name='vertical')
+            self.osc_levels_lineset[self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_, name='top')
+            self.osc_levels_lineset[2*self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_peak, name='peak hold')
+#            self.osc_levels_lineset[3]=self.osc_levels_line.plot(pen=pen_, name='Channel')
+
+        self.osc_levels_peak_hold = np.zeros(self.settings.channels)
+        self.time_last_changed = np.zeros(self.settings.channels)
+
+    def update(self):
+        '''
+        Updates plots with incoming data from __call__.
+        Called with a 0s interval by QTimer.
+
+        '''
+        time_data_snapshot = np.copy(self.rec.osc_time_data)
+        if self.view_levels == True:
+            self.osc_levels_rms = np.sqrt(np.mean(time_data_snapshot**2,axis=0))
+            self.osc_levels_max = np.max(np.abs(time_data_snapshot),axis=0)
+            changed_indices = self.osc_levels_peak_hold < self.osc_levels_max
+            self.time_last_changed[changed_indices] = time.time()
+            self.osc_levels_peak_hold = np.maximum(self.osc_levels_peak_hold,self.osc_levels_max)
+            self.osc_levels_peak_hold[time.time()-self.time_last_changed>2] = 0
+
+        for i in range(self.settings.channels):
+            offset = i
+            if self.view_time == True:
+                if (self.auto_scale is True) and (self.settings.channels==1):
+                    shift = 0
+                    scale_factor = 1
+                    self.osc_time_line.enableAutoRange()
+                elif (self.auto_scale is True) and (self.settings.channels!=1):
+                    shift = np.mean(time_data_snapshot[:,i])
+                    scale_factor = np.max(np.abs(time_data_snapshot[:,i]-shift))*2
+                    self.osc_time_line.setYRange(-1,self.settings.channels)
+                else:
+                    shift = 0
+                    scale_factor = 1
+                    self.osc_time_line.setYRange(-1,self.settings.channels)
+                    
+                self.osc_time_lineset[i].setData(self.rec.osc_time_axis, (time_data_snapshot[:,i]-shift)/scale_factor + offset)
+
+            if self.view_freq == True:
+                # calculate the FFT
+                self.rec.osc_time_data_windowed[:,i] = time_data_snapshot[:,i] * np.blackman(np.shape(time_data_snapshot)[0])
+                fd = np.abs(np.fft.rfft(self.rec.osc_time_data_windowed[:,i]))/len(self.rec.osc_time_data_windowed[:,i])
+                fd[fd==0] = np.min(fd+1e-16) # to avoid log10(0) warnings
+                self.rec.osc_freq_data[:,i] = 20 * np.log10(fd)
+                self.osc_freq_lineset[i].setData(self.rec.osc_freq_axis,self.rec.osc_freq_data[:,i])
+
+            if self.view_levels == True:
+                self.osc_levels_lineset[i].setData([i,i],[0,self.osc_levels_max[i]])
+                self.osc_levels_lineset[self.settings.channels+i].setData([i-0.3,i+0.3],self.osc_levels_max[i]*np.ones(2))
+
+                if self.osc_levels_peak_hold[i] > 0.98:
+                    pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=10)
+                else:
+                    pen_peak = pg.mkPen(color=options.set_plot_colours(self.settings.channels)[i,:],width=3)
+#                self.osc_levels_lineset[2*self.settings.channels+i]=self.osc_levels_line.plot(pen=pen_peak, name='peak hold')
+                self.osc_levels_lineset[2*self.settings.channels+i].setData([i-0.3,i+0.3],self.osc_levels_peak_hold[i]*np.ones(2),pen=pen_peak)
+#                self.osc_levels_lineset[3].setData(np.arange(2),np.ones(2))
+
+
+
+    #KeyPressed function within osciolloscpe since can only take one argument
+    def keyPressed(self, evt):
+        '''
+        Upon a Space Bar press, makes a copy of data from the past stored_time seconds,plots it in Bokeh and gives the user an option to save it.
+        '''
+
+        if evt.key() == QtCore.Qt.Key_T:
+
+            if self.view_freq != False or self.view_levels != False:
+#                print('toggled time domain view')
+                self.view_time = not self.view_time
+                self.toggle_view()
+#            else:
+#                print('toggling all views off is prevented')
+
+        if evt.key() == QtCore.Qt.Key_F:
+
+            if self.view_time != False or self.view_levels != False:
+#                print('toggled frequency domain view')
+                self.view_freq = not self.view_freq
+                self.toggle_view()
+#            else:
+#                print('toggling all views off is prevented')
+
+        if evt.key() == QtCore.Qt.Key_L:
+            if self.view_time != False or self.view_freq != False:
+#                print('toggled levels view')
+                self.view_levels = not self.view_levels
+                self.toggle_view()
+#            else:
+#                print('toggling all views off is prevented')
+        
+        if evt.key() == QtCore.Qt.Key_P:
+            if self.timer.isActive():
+                self.timer.stop()
+            else:
+                self.timer.start()
+                
+        if evt.key() == QtCore.Qt.Key_A:
+            self.win.setWindowFlags(self.win.windowFlags() ^ QtCore.Qt.WindowStaysOnTopHint)       
+            self.win.show()
+                
+            
+        if evt.key() == QtCore.Qt.Key_Y:
+            self.auto_scale = not self.auto_scale 
+                
+        if evt.key() == QtCore.Qt.Key_Space or evt.key() == QtCore.Qt.Key_S:
+
+            stored_time_data_copy=np.copy(self.rec.stored_time_data)
+            t = datetime.datetime.now()
+            timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)
+#            print("key press trigger: saving data to file in working directory")
+
+            ### make into dataset
+            
+            fs=self.settings.fs
+            n_samp=len(stored_time_data_copy[:,0])
+            dt=1/fs
+            t_axis= np.arange(n_samp)*dt
+
+            
+            timedata = datastructure.TimeData(t_axis,stored_time_data_copy,self.settings,timestamp=t,timestring=timestring,test_name='Test_{}'.format(self.data_saved_counter))
+            
+            dataset = datastructure.DataSet()
+            dataset.add_to_dataset(timedata)
+            
+            
+            if evt.key() == QtCore.Qt.Key_S:
+                self.data_saved_counter = 1
+                self.last_filename = file.save_data(dataset,self.win)
+            
+#            # this version saves all data as new timedata objects within one file
+#            if evt.key() == QtCore.Qt.Key_Space:
+#                if self.data_saved_counter == 0:
+#                    self.last_filename = file.save_data(dataset)
+#                    if self.last_filename == '':
+#                        self.data_saved_counter = 0
+#                    else:
+#                        self.data_saved_counter += 1
+#                
+#                else:
+#                    d = file.load_data(self.last_filename)
+#                    d.add_to_dataset(timedata)
+#                    file.save_data(d,self.last_filename,overwrite_without_prompt=True)
+#                    self.data_saved_counter += 1
+            
+            # this version saves each new dataset to new file
+            if evt.key() == QtCore.Qt.Key_Space:
+                if self.data_saved_counter == 0:
+                    self.last_filename = file.save_data(dataset,self.win)
+                    if self.last_filename == '':
+                        self.data_saved_counter = 0
+                    else:
+                        self.data_saved_counter += 1
+                
+                else:
+                    d = datastructure.DataSet()
+                    d.add_to_dataset(timedata)
+                    filename = self.last_filename.replace('.npy','_'+str(self.data_saved_counter)+'.npy')
+                    file.save_data(d,self.win, filename,overwrite_without_prompt=True)
+                    self.data_saved_counter += 1
+
+class KeyPressWindow(pg.GraphicsLayoutWidget):
+    '''
+    A subclass of pyQtGraph GraphicsWindow that emits a signal when a key is pressed.
+
+    '''
+    sigKeyPress = Signal(object)
+    sigClose = Signal(object)
+
+    def __init__(self, *args, **kwargs):
+        '''
+        Re-implmented from parent.
+        '''
+        super().__init__(*args, **kwargs)
+
+    def keyPressEvent(self, evt):
+        '''
+        Emits a signal upon a key press
+        '''
+        self.scene().keyPressEvent(evt)
+        self.sigKeyPress.emit(evt)
+
+    def closeEvent(self, evt):
+        '''
+        Emits a signal when the window is closed.
+        '''
+        self.sigClose.emit(evt)
+        self.close()
```

### Comparing `pydvma-0.9.0/pydvma/plotting.py` & `pydvma-0.9.1/pydvma/plotting.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,664 +1,664 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Aug 28 19:04:14 2018
-
-@author: tb267
-"""
-
-
-
-from . import options
-from . import datastructure
-from . import gui
-
-import numpy as np
-import matplotlib
-import matplotlib.pyplot as plt
-matplotlib.rcParams.update({'font.size': 10,'font.family':'serif'})
-from matplotlib.ticker import AutoLocator
-
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
-from matplotlib.figure import Figure
-from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
-
-from qtpy.QtWidgets import QWidget, QLabel, QVBoxLayout
-from qtpy.QtCore import Qt
-from qtpy import QtGui
-
-
-import time
-
-LINE_ALPHA = 0.9
-
-class PlotSonoData():
-    def __init__(self,figsize=(9,5),canvas=None,fig=None):
-        if canvas==None:
-            self.fig, self.ax = plt.subplots(1,1,figsize=figsize,dpi=100)#,constrained_layout=True)
-        else:
-            self.fig = fig
-            self.canvas = canvas
-            self.ax = self.canvas.figure.subplots()
-        
-        self.ax.grid(False)
-        self.fig.canvas.draw()
-        
-    def update(self,sono_data_list,n_set=0,n_chan=0):
-        
-        f = sono_data_list[n_set].freq_axis
-        t = sono_data_list[n_set].time_axis
-        S = sono_data_list[n_set].sono_data[:,:,n_chan]
-        self.ax.pcolor(t,f,20*np.log10(np.abs(S)))
-        self.ax.set_xlabel('Time (s)')
-        self.ax.set_ylabel('Frequency (Hz)')
-    
-
-class PlotData():
-    def __init__(self,window_title=None,sets='all',channels='all',figsize=(9,5),canvas=None,fig=None):
-        if canvas==None:
-            # self.fig = Figure(figsize=(9, 7),dpi=100)
-            # self.canvas = FigureCanvas(self.fig)
-            # self.toolbar = NavigationToolbar(self.canvas,None)
-            self.fig, self.ax = plt.subplots(1,1,figsize=figsize,dpi=100)
-            self.fig.show()
-            
-            # self.plot_window = QWidget()
-            # self.plot_window.setStyleSheet("background-color: white")
-            # self.plot_window.setWindowTitle('Figure')
-            # self.plot_window.setWindowIcon(QtGui.QIcon('pydvma/icon.png'))
-            
-            # self.fig = Figure(figsize=(9, 5),dpi=100)
-            # self.canvas = FigureCanvas(self.fig)
-            # self.toolbar = NavigationToolbar(self.canvas,None)
-            # self.toolbar.setOrientation(Qt.Orientation.Horizontal)
-            # self.ax = self.canvas.figure.subplots()
-            
-            # if window_title is not None:
-            #     self.label_figure = QLabel(window_title)
-            # else:
-            #     self.label_figure = QLabel('')
-
-            # self.label_figure.setMaximumHeight(20)
-            # self.label_figure.setAlignment(Qt.AlignmentFlag.AlignCenter)
-            
-            # # widgets to layout
-            # self.layout_figure = QVBoxLayout()
-            # self.layout_figure.addWidget(self.label_figure)
-            # self.layout_figure.addWidget(self.canvas)
-            # self.layout_figure.addWidget(self.toolbar)
-            
-            # self.plot_window.setLayout(self.layout_figure)
-            
-            
-            # # self.plot_window.showMinimized()
-            # # time.sleep(0.6)
-            # self.plot_window.show()
-            # self.plot_window.showNormal()
-            # self.plot_window.raise_()
-            # if gui.app.applicationState() == Qt.ApplicationState.ApplicationInactive:
-            #     gui.app.exec()
-            # self.gui.app.exec()
-        else:
-            self.fig = fig
-            self.canvas = canvas
-            self.ax = self.canvas.figure.subplots()
-
-        #ax2 is for coherence
-        self.ax2 = self.ax.twinx()
-        self.ax2.set_visible(False)
-        self.ax.set_zorder(self.ax2.get_zorder()+1)
-        self.ax.patch.set_visible(False)
-        
-#        #ax3 is for sonograms: 
-#        self.ax2 = self.ax.twinx()
-#        self.ax2.set_visible(False)
-#        self.ax.set_zorder(self.ax2.get_zorder()+1)
-#        self.ax.patch.set_visible(False)
-
-        [line.remove() for line in self.ax.lines]
-        [line.remove() for line in self.ax2.lines]
-        self.line_listbyset = []
-        self.line2_listbyset = []
-        self.pcolor_sono = None
-        self.visibility = True
-        
-        self.ax.grid(True,alpha=0.2)
-        self.fig.canvas.mpl_connect('pick_event', self.channel_select)
-        self.fig.canvas.draw()
-        
-    def update(self,data_list,sets='all',channels='all',xlinlog='linear',show_coherence=True,plot_type=None,coherence_plot_type='linear',freq_range=None, auto_xy='xyc'):
-        global LINE_ALPHA
-        
-        # when switching back from sonogram, remove all pcolormesh parts of plot
-        for ch in self.ax.get_children():
-                if ch.__class__.__name__ == 'QuadMesh':
-                    ch.remove()
-                    self.visibility = True # turn legend back on
-        
-        
-        self.ax.grid(True,alpha=0.2)
-        self.data_list = data_list
-        self.plot_type = plot_type
-        self.freq_range = freq_range
-        self.xlinlog = xlinlog
-        
-        if data_list.__class__.__name__ == 'TimeDataList':
-            self.ax2.set_visible(False)
-            self.ax.set_xlabel('Time (s)')
-            self.ax.set_ylabel('Amplitude')
-            self.ax.axis('auto')
-        elif data_list.__class__.__name__ == 'FreqDataList':
-            self.ax2.set_visible(False)
-            if (plot_type == 'Amplitude (dB)') or (plot_type == None):
-                self.ax.set_xlabel('Frequency (Hz)')
-                self.ax.set_ylabel('Amplitude (dB)')
-                self.ax.axis('auto')
-            elif plot_type == 'Amplitude (linear)':
-                self.ax.set_xlabel('Frequency (Hz)')
-                self.ax.set_ylabel('Amplitude')
-                self.ax.axis('auto')
-            elif plot_type == 'Real Part':
-                self.ax.set_xlabel('Frequency (Hz)')
-                self.ax.set_ylabel('Real Part')
-                self.ax.axis('auto')
-            elif plot_type == 'Imag Part':
-                self.ax.set_xlabel('Frequency (Hz)')
-                self.ax.set_ylabel('Imag Part')
-                self.ax.axis('auto')
-            elif plot_type == 'Nyquist':
-                self.ax.set_xlabel('Real Part')
-                self.ax.set_ylabel('Imag Part')
-                self.ax.set_aspect('equal','datalim')
-            elif plot_type == 'Phase':
-                self.ax.set_xlabel('Frequency (Hz)')
-                self.ax.set_ylabel('Phase (deg)')
-                self.ax.axis('auto')
-                
-            self.ax.set_xscale(xlinlog)
-            if 'log' in xlinlog:
-                self.ax.grid(visible=True, which='minor',axis='x',alpha=0.2)
-            else:
-                self.ax.grid(visible=False)
-            
-        elif data_list.__class__.__name__ == 'TfDataList':
-            if (plot_type == 'Amplitude (dB)') or (plot_type == None):
-                self.ax.set_xlabel('Frequency (Hz)')
-                self.ax.set_ylabel('Amplitude (dB)')
-                self.ax.axis('auto')
-            elif plot_type == 'Amplitude (linear)':
-                self.ax.set_xlabel('Frequency (Hz)')
-                self.ax.set_ylabel('Amplitude')
-                self.ax.axis('auto')
-            elif plot_type == 'Real Part':
-                self.ax.set_xlabel('Frequency (Hz)')
-                self.ax.set_ylabel('Real Part')
-                self.ax.axis('auto')
-            elif plot_type == 'Imag Part':
-                self.ax.set_xlabel('Frequency (Hz)')
-                self.ax.set_ylabel('Imag Part')
-                self.ax.axis('auto')
-            elif plot_type == 'Nyquist':
-                self.ax.set_xlabel('Real Part')
-                self.ax.set_ylabel('Imag Part')
-                self.ax.set_aspect('equal','datalim')
-            elif plot_type == 'Phase':
-                self.ax.set_xlabel('Frequency (Hz)')
-                self.ax.set_ylabel('Phase (deg)')
-                self.ax.axis('auto')
-            
-            
-            self.ax.set_xscale(xlinlog)
-            if 'log' in xlinlog:
-                self.ax.grid(visible=True, which='minor',axis='x',alpha=0.2)
-            else:
-                self.ax.grid(visible=False)
-            
-            # setup twin axis
-            # don't plot coherence if no data, or if all coherence is one
-            flag_coherence = []
-            for n_set in range(len(data_list)):
-                if data_list[n_set].tf_coherence is None:
-                    flag_coherence += [True]
-                else:
-                    tfc = data_list[n_set].tf_coherence
-                    i = np.isnan(tfc)
-                    tfc[i] = 1
-                    diff_to_one = np.abs(tfc - 1)
-                    flag_coherence += [np.all(diff_to_one<1e-10)]
-            if np.all(flag_coherence):
-                show_coherence = False
-            
-            if show_coherence == True:
-                self.ax2.set_ylabel('Coherence')
-                self.ax2.set_visible(True)
-            else:
-                self.ax2.set_visible(False)
-    
-        # sonogram plot completely different, use separate function
-        
-        N_sets = len(data_list)
-
-        # pre-count how many channels total
-        ch_counter = 0
-        for n_set in range(N_sets):
-            if data_list.__class__.__name__ == 'TimeDataList':
-                ch_counter += len(data_list[n_set].time_data[0,:])
-            elif data_list.__class__.__name__ == 'FreqDataList':
-                ch_counter += len(data_list[n_set].freq_data[0,:])
-            elif data_list.__class__.__name__ == 'TfDataList':
-                ch_counter += len(data_list[n_set].tf_data[0,:])
-
-        self.ch_total = ch_counter
-        if self.ch_total <= 12:
-            LINE_ALPHA = 0.9
-        else:
-            # option to make lines fainter when more lines... needs some tweaking to make feel right
-            LINE_ALPHA = 1-1/self.ch_total # make deselected lines fainter if more channels
-        
-        [line.remove() for line in self.ax.lines]
-        [line.remove() for line in self.ax2.lines]
-        self.line_listbyset = []
-        self.line2_listbyset = []
-        
-        if sets == 'all':
-            sets = range(N_sets)
-        count = -1
-        for n_set in range(len(data_list)):
-            self.line_listbyset.append([])
-            self.line2_listbyset.append([])
-            
-            if data_list.__class__.__name__ == 'TfDataList':
-                N_chans = len(data_list[n_set].tf_data[0,:])
-            elif data_list.__class__.__name__ == 'FreqDataList':
-                N_chans = len(data_list[n_set].freq_data[0,:])
-            elif data_list.__class__.__name__ == 'TimeDataList':
-                N_chans = len(data_list[n_set].time_data[0,:])
-                
-            if channels == 'all':
-                channels = range(N_chans)
-
-            
-
-            for n_chan in range(N_chans):
-                count += 1
-                if (n_set not in sets) or (n_chan not in channels):
-                    alpha = 1-LINE_ALPHA
-                else:
-                    alpha = LINE_ALPHA
-                
-                if data_list.__class__.__name__ == 'TimeDataList':
-                    x = data_list[n_set].time_axis
-                    y = data_list[n_set].time_data[:,n_chan] * data_list[n_set].channel_cal_factors[n_chan]
-        
-                elif data_list.__class__.__name__ == 'FreqDataList':
-                    x = data_list[n_set].freq_axis
-                    ylin = data_list[n_set].freq_data[:,n_chan] * data_list[n_set].channel_cal_factors[n_chan]
-                    
-                    
-                    if (plot_type == 'Amplitude (dB)') or (plot_type == None):
-                        # handle log(0) manually to avoid warnings
-                        y = np.zeros(np.shape(ylin))
-                        izero = ylin==0
-                        y[~izero] = 20*np.log10(np.abs(ylin[~izero]))
-                        y[izero] = -np.inf
-                    elif plot_type == 'Amplitude (linear)':
-                        y = np.abs(ylin)
-                    elif plot_type == 'Real Part':
-                        y = np.real(ylin)
-                    elif plot_type == 'Imag Part':
-                        y = np.imag(ylin)
-                    elif plot_type == 'Nyquist':
-                        if freq_range == None:
-                            freq_range = [-1,np.inf]
-                        selected_data = np.where((x>freq_range[0]) * (x<freq_range[1]))[0]
-                        x = np.real(ylin[selected_data])
-                        y = np.imag(ylin[selected_data])
-                        
-                    elif plot_type == 'Phase':
-                        y = np.angle(ylin,deg=True)
-                        
-                    
-                elif data_list.__class__.__name__ == 'TfDataList':
-                    x = data_list[n_set].freq_axis
-                    ylin = data_list[n_set].tf_data[:,n_chan] * data_list[n_set].channel_cal_factors[n_chan]
-                    if (plot_type == 'Amplitude (dB)') or (plot_type == None):
-                        # handle log(0) manually to avoid warnings
-                        y = np.zeros(np.shape(ylin))
-                        izero = ylin==0
-                        y[~izero] = 20*np.log10(np.abs(ylin[~izero]))
-                        y[izero] = -np.inf
-                        
-                    elif plot_type == 'Amplitude (linear)':
-                        y = np.abs(ylin)
-                    elif plot_type == 'Real Part':
-                        y = np.real(ylin)
-                    elif plot_type == 'Imag Part':
-                        y = np.imag(ylin)
-                    elif plot_type == 'Nyquist':
-                        if freq_range == None:
-                            freq_range = [-1,np.inf]
-                        selected_data = np.where((x>freq_range[0]) * (x<freq_range[1]))[0]
-                        x = np.real(ylin[selected_data])
-                        y = np.imag(ylin[selected_data])
-                    elif plot_type == 'Phase':
-                        y = np.angle(ylin,deg=True)
-                    if data_list[n_set].tf_coherence is not None:
-                        # handle log(0) manually to avoid warnings
-                        yclin = data_list[n_set].tf_coherence[:,n_chan]
-                        if coherence_plot_type == 'linear':
-                            yc = yclin
-                        elif coherence_plot_type == 'log':
-                            yc = np.zeros(np.shape(yclin))
-                            izero = yclin==0
-                            yc[~izero] = 20*np.log10(np.abs(yclin[~izero]))
-                            yc[izero] = -np.inf
-                            yc = 20*np.log10(np.abs(yclin))
-                    else:
-                        yc = np.ones(np.shape(data_list[n_set].tf_data))
-                        
-                        
-                color = options.set_plot_colours(ch_counter)[count,:]/255
-                
-                if type(data_list[n_set].test_name) is str:
-                    test_name = data_list[n_set].test_name
-                else:
-                    test_name = ''
-                    
-                if test_name != '':
-                    test_name = test_name + ': '
-                    
-                if self.ch_total < 10:
-                    label = '{}set_{}, ch_{}'.format(test_name,n_set,n_chan)
-                else:
-                    label = 'set{},ch{}'.format(n_set,n_chan)
-                    
-                if data_list.__class__.__name__ == 'TfDataList':
-                    if data_list[n_set].flag_modal_TF == True:
-                        label = 'fit{}'.format(n_chan)
-                        
-                self.line_listbyset[n_set] += self.ax.plot(x,y,'-',linewidth=1,color = color,label=label,alpha=alpha)
-                
-                if data_list.__class__.__name__ == 'TfDataList':
-                    if show_coherence == True:
-                        self.line2_listbyset[n_set] += self.ax2.plot(x,yc,':',linewidth=1,color = color,label=label+' (coherence)',alpha=alpha)
-                        self.ax2.set_visible(True)
-                    else:
-                        self.ax2.set_visible(False)
-        
-        self.fig.tight_layout()
-        self.fig.canvas.draw()
-        self.update_legend()
-        if 'x' in auto_xy:
-            self.auto_x()
-        if 'f' in auto_xy: # use freq_range for x axis
-            if ('log' in xlinlog) and freq_range[0]==0:
-                self.lines = self.ax.get_lines()
-                xminlog = np.inf
-                for line in self.lines:
-                    if line.get_alpha() > 0.5:
-                        data = line.get_data()
-                        xxlog = data[0][1] # first nonzero freq axis
-                        xminlog = min([xminlog,xxlog])
-                        freq_range[0] = xminlog
-                self.ax.set_xlim(freq_range)
-            else:
-                self.ax.set_xlim(freq_range)
-            self.fig.canvas.draw()
-            self.auto_y()
-        if 'y' in auto_xy:
-            self.auto_y()
-        if 'c' in auto_xy: # auto coherence y
-            self.ax2.set_ylim([0,1])
-            
-#        self.ax.xaxis.set_major_locator(AutoLocator())
-#        self.ax.yaxis.set_major_locator(AutoLocator())
-        self.fig.canvas.draw()
-        
-        
-        
-    def update_legend(self,loc='lower right',draggable=False):
-        
-        if len(self.data_list) != 0:
-            if self.ax.get_legend() is None:
-                self.visibility = True
-                
-            if self.ch_total >= 10:
-                # make legend more compact
-                col_sizes = np.arange(10,7,-1)
-                rem = np.remainder(self.ch_total,col_sizes)
-                if any(rem==0):
-                    remi = np.where(rem==0)[0]
-                    remi = remi[0]
-                    ncol = int(self.ch_total / col_sizes[remi])
-                else:
-                    remi = np.argmax(rem)
-                    ncol = int(np.ceil(self.ch_total/ col_sizes[remi]))
-            else:
-                ncol = 1
-                
-            self.legend = self.ax.legend(loc=loc, ncol=ncol)
-#            self.ax.legend()
-            self.legend.set_draggable(draggable,use_blit=True)#(True),update='bbox',use_blit=True
-            self.lines = self.ax.get_lines()
-            self.lines2 = self.ax2.get_lines()
-            self.lined = dict()
-            self.lined2 = dict()
-
-            # make dictionary of legend lines for selection    
-            for legline, origline in zip(self.legend.get_lines(), self.lines):
-                legline.set_picker(True)  # argument tolerance
-                legline.set_pickradius(10)  # argument tolerance
-                self.lined[legline] = origline
-                legline.set_alpha(origline.get_alpha())
-
-            # make dictionary of coherence lines to select with legend - only for TF Data
-            if len(self.ax2.lines) > 0:
-                for legline, origline2 in zip(self.legend.get_lines(), self.lines2):
-                    self.lined2[legline] = origline2 
-                    origline2.set_alpha(legline.get_alpha())
-                    
-            self.ax.get_legend().set_visible(self.visibility)
-        else:
-            self.legend = self.ax.get_legend()
-            if self.legend is not None:
-                self.legend.remove()
-            self.fig.canvas.draw()
-    
-    
-    def auto_x(self):
-        if self.data_list.__class__.__name__ == 'SonoDataList':
-            xlim = self.data_list[self.n_set].time_axis[[0,-1]]
-            self.ax.set_xlim(xlim)
-        else:
-            self.lines = self.ax.get_lines()
-            xmin = np.inf
-            xminlog = np.inf
-            xmax = -np.inf
-            ymin = np.inf # for Nyquist to stop cropping
-            ymax = -np.inf
-            for line in self.lines:
-                if line.get_alpha() > 0.5:
-                    data = line.get_data()
-                    try:
-                        # handle when some lines are out of view
-                        xx = min(data[0])
-                        xmin = min([xx,xmin])
-                        
-                        xxlog = data[0][1] # first nonzero freq axis
-                        xminlog = min([xminlog,xxlog])
-                        
-                        xx = max(data[0])
-                        xmax = max([xx,xmax])
-                        if self.plot_type == 'Nyquist':
-                            yy = min(data[1])
-                            ymin = min([yy,ymin])
-                            yy = max(data[1])
-                            ymax = max([yy,ymax])
-                    except:
-                        pass
-            try:
-                if 'log' in self.xlinlog:
-                    self.ax.set_xlim([xminlog,xmax])
-                else:
-                    if self.plot_type == 'Nyquist':
-                        # equal axis means need x range needs to stay greater than y range
-                        yrange = ymax-ymin
-                        # get bounding box bb to know current aspect ratio ar
-                        bb=self.ax.get_window_extent().transformed(self.fig.dpi_scale_trans.inverted())
-                        ar = bb.width / bb.height
-                        if (xmax-xmin) < (ar*yrange):
-                            xmid = (xmin+xmax)/2
-                            xmax = xmid + ar*yrange/2
-                            xmin = xmid - ar*yrange/2
-                        
-                    self.ax.set_xlim([xmin,xmax])
-                    
-            except:
-                pass
-        self.fig.canvas.draw()
-        
-        
-    def auto_y(self):
-        if self.data_list.__class__.__name__ == 'SonoDataList':
-            ylim = self.data_list[self.n_set].freq_axis[[0,-1]]
-            self.ax.set_ylim(ylim)
-        else:
-            self.lines = self.ax.get_lines()
-            if (self.data_list.__class__.__name__ == 'TfData') and (self.plot_type != 'Nyquist'):
-                # at the moment this doesn't get called
-                # it should be TfDataList in condition
-                # and it should be == nyquist not !=
-                # but plot behaviour correct as it stands and probably just need this setting to xlim always
-                xview = self.freq_range
-            else:
-                xview = self.ax.get_xlim()
-            ymin = np.inf
-            ymax = -np.inf
-            c=-1
-            for line in self.lines:
-                c+=1
-                data = line.get_data() 
-                x = data[0]
-                selection = (xview[0] < x) & (x < xview[1])
-                if line.get_alpha() > 0.5:
-                    try:
-                        # handle case when some lines out of view
-                        yy = min(data[1][selection])
-                        ymin = min([yy,ymin])
-                        yy = max(data[1][selection])
-                        ymax = max([yy,ymax])
-                    except:
-                        pass
-            try:
-                self.ax.set_ylim([ymin,ymax])
-            except:
-                pass
-        if self.data_list.__class__.__name__ == 'TfDataList':
-            # reset coherence to 0-1
-            self.ax2.set_ylim([0,1])
-            
-        self.fig.canvas.draw()
-        
-    def channel_select(self,event):
-        selected_line = event.artist
-        
-        a = selected_line.get_alpha()
-        # This function is called when legend dragged, and a is None
-        # So only want to change line opacity when line actually selected.
-        if a is not None:
-            # change opacity of both legend line and actual line
-            a = 1-a
-            origline = self.lined[selected_line]
-            
-
-            selected_line.set_alpha(a)
-            origline.set_alpha(a)
-            
-            # change z order to bring selected line to foreground
-            for line in self.ax.lines:
-                line.set_zorder(0)
-            if a > 0.5:
-                origline.set_zorder(1)
-            else:
-                origline.set_zorder(0)
-                
-            # also select matching coherence lines
-            if len(self.ax2.lines) > 0:
-                origline2 = self.lined2[selected_line]
-                origline2.set_alpha(a)
-                for line2 in self.ax2.lines:
-                    line2.set_zorder(0)
-                if a > 0.5:
-                    origline2.set_zorder(1)
-                else:
-                    origline2.set_zorder(0)
-            self.fig.canvas.draw()
-    
-    def get_selected_channels(self):
-        # find the sets and channels higlighted in figure
-        
-        n_sets = len(self.line_listbyset)
-        selected_data = []
-        
-        for ns in range(n_sets):
-            selected_data += [[]]
-            for line in self.line_listbyset[ns]:
-                selected_data[ns] += [line.get_alpha() > 0.5] # skip coherence lines
-            
-        return selected_data
-    
-    def set_selected_channels(self,s):
-        global LINE_ALPHA
-        # relies on all sets of data with same number of channels. Need to make more general.
-        for n_set in range(len(s)):
-            for n_chan in range(len(s[n_set])):
-                if s[n_set][n_chan] == True:
-                    self.line_listbyset[n_set][n_chan].set_alpha(LINE_ALPHA)
-                else:
-                    self.line_listbyset[n_set][n_chan].set_alpha(1-LINE_ALPHA)
-        # make legend line alphas match actual lines, but keep visibility as before
-        self.update_legend()
-        self.fig.canvas.draw()
-        
-    def update_sonogram(self,sono_data_list,n_set,n_chan,db_range=60,auto_xy='xy'):
-        self.data_list = sono_data_list # makes auto_x/y work!
-        
-        for ch in self.ax.get_children():
-                if ch.__class__.__name__ == 'QuadMesh':
-                    ch.remove()
-        
-        self.n_set = n_set
-        self.n_chan = n_chan
-        self.ax2.set_visible(False)
-        self.ax.set_xlabel('Time (s)')
-        self.ax.set_ylabel('Frequency (Hz)')
-        self.ax.grid(False)
-        if self.ax.get_legend() is not None:
-            self.ax.get_legend().set_visible(False)
-        
-        [line.remove() for line in self.ax.lines]
-        [line.remove() for line in self.ax2.lines]
-        self.line_listbyset = []
-        self.line2_listbyset = []
-        
-        f = sono_data_list[n_set].freq_axis
-        t = sono_data_list[n_set].time_axis
-        S = sono_data_list[n_set].sono_data[:,:,n_chan]
-        S[S==0] = 1e-16 # avoid log10(0) warnings
-        SdB = 20*np.log10(np.abs(S))
-        vmax = SdB.max()
-        vmin = np.max([SdB.min(),vmax-db_range])
-        self.pcolor_sono = self.ax.pcolormesh(t,f,SdB,shading='gouraud',cmap='Blues',vmax=vmax,vmin=vmin,rasterized=True)
-        if 'x' in auto_xy:
-            self.auto_x()
-        if 'y' in auto_xy:
-            self.auto_y()
-
-#        self.fig.colorbar(ax=self.ax)
-        self.fig.canvas.draw()
-        
-        
-    
-    
-    
-
-
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Aug 28 19:04:14 2018
+
+@author: tb267
+"""
+
+
+
+from . import options
+from . import datastructure
+from . import gui
+
+import numpy as np
+import matplotlib
+import matplotlib.pyplot as plt
+matplotlib.rcParams.update({'font.size': 10,'font.family':'serif'})
+from matplotlib.ticker import AutoLocator
+
+from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+from matplotlib.figure import Figure
+from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
+
+from qtpy.QtWidgets import QWidget, QLabel, QVBoxLayout
+from qtpy.QtCore import Qt
+from qtpy import QtGui
+
+
+import time
+
+LINE_ALPHA = 0.9
+
+class PlotSonoData():
+    def __init__(self,figsize=(9,5),canvas=None,fig=None):
+        if canvas==None:
+            self.fig, self.ax = plt.subplots(1,1,figsize=figsize,dpi=100)#,constrained_layout=True)
+        else:
+            self.fig = fig
+            self.canvas = canvas
+            self.ax = self.canvas.figure.subplots()
+        
+        self.ax.grid(False)
+        self.fig.canvas.draw()
+        
+    def update(self,sono_data_list,n_set=0,n_chan=0):
+        
+        f = sono_data_list[n_set].freq_axis
+        t = sono_data_list[n_set].time_axis
+        S = sono_data_list[n_set].sono_data[:,:,n_chan]
+        self.ax.pcolor(t,f,20*np.log10(np.abs(S)))
+        self.ax.set_xlabel('Time (s)')
+        self.ax.set_ylabel('Frequency (Hz)')
+    
+
+class PlotData():
+    def __init__(self,window_title=None,sets='all',channels='all',figsize=(9,5),canvas=None,fig=None):
+        if canvas==None:
+            # self.fig = Figure(figsize=(9, 7),dpi=100)
+            # self.canvas = FigureCanvas(self.fig)
+            # self.toolbar = NavigationToolbar(self.canvas,None)
+            self.fig, self.ax = plt.subplots(1,1,figsize=figsize,dpi=100)
+            self.fig.show()
+            
+            # self.plot_window = QWidget()
+            # self.plot_window.setStyleSheet("background-color: white")
+            # self.plot_window.setWindowTitle('Figure')
+            # self.plot_window.setWindowIcon(QtGui.QIcon('pydvma/icon.png'))
+            
+            # self.fig = Figure(figsize=(9, 5),dpi=100)
+            # self.canvas = FigureCanvas(self.fig)
+            # self.toolbar = NavigationToolbar(self.canvas,None)
+            # self.toolbar.setOrientation(Qt.Orientation.Horizontal)
+            # self.ax = self.canvas.figure.subplots()
+            
+            # if window_title is not None:
+            #     self.label_figure = QLabel(window_title)
+            # else:
+            #     self.label_figure = QLabel('')
+
+            # self.label_figure.setMaximumHeight(20)
+            # self.label_figure.setAlignment(Qt.AlignmentFlag.AlignCenter)
+            
+            # # widgets to layout
+            # self.layout_figure = QVBoxLayout()
+            # self.layout_figure.addWidget(self.label_figure)
+            # self.layout_figure.addWidget(self.canvas)
+            # self.layout_figure.addWidget(self.toolbar)
+            
+            # self.plot_window.setLayout(self.layout_figure)
+            
+            
+            # # self.plot_window.showMinimized()
+            # # time.sleep(0.6)
+            # self.plot_window.show()
+            # self.plot_window.showNormal()
+            # self.plot_window.raise_()
+            # if gui.app.applicationState() == Qt.ApplicationState.ApplicationInactive:
+            #     gui.app.exec()
+            # self.gui.app.exec()
+        else:
+            self.fig = fig
+            self.canvas = canvas
+            self.ax = self.canvas.figure.subplots()
+
+        #ax2 is for coherence
+        self.ax2 = self.ax.twinx()
+        self.ax2.set_visible(False)
+        self.ax.set_zorder(self.ax2.get_zorder()+1)
+        self.ax.patch.set_visible(False)
+        
+#        #ax3 is for sonograms: 
+#        self.ax2 = self.ax.twinx()
+#        self.ax2.set_visible(False)
+#        self.ax.set_zorder(self.ax2.get_zorder()+1)
+#        self.ax.patch.set_visible(False)
+
+        [line.remove() for line in self.ax.lines]
+        [line.remove() for line in self.ax2.lines]
+        self.line_listbyset = []
+        self.line2_listbyset = []
+        self.pcolor_sono = None
+        self.visibility = True
+        
+        self.ax.grid(True,alpha=0.2)
+        self.fig.canvas.mpl_connect('pick_event', self.channel_select)
+        self.fig.canvas.draw()
+        
+    def update(self,data_list,sets='all',channels='all',xlinlog='linear',show_coherence=True,plot_type=None,coherence_plot_type='linear',freq_range=None, auto_xy='xyc'):
+        global LINE_ALPHA
+        
+        # when switching back from sonogram, remove all pcolormesh parts of plot
+        for ch in self.ax.get_children():
+                if ch.__class__.__name__ == 'QuadMesh':
+                    ch.remove()
+                    self.visibility = True # turn legend back on
+        
+        
+        self.ax.grid(True,alpha=0.2)
+        self.data_list = data_list
+        self.plot_type = plot_type
+        self.freq_range = freq_range
+        self.xlinlog = xlinlog
+        
+        if data_list.__class__.__name__ == 'TimeDataList':
+            self.ax2.set_visible(False)
+            self.ax.set_xlabel('Time (s)')
+            self.ax.set_ylabel('Amplitude')
+            self.ax.axis('auto')
+        elif data_list.__class__.__name__ == 'FreqDataList':
+            self.ax2.set_visible(False)
+            if (plot_type == 'Amplitude (dB)') or (plot_type == None):
+                self.ax.set_xlabel('Frequency (Hz)')
+                self.ax.set_ylabel('Amplitude (dB)')
+                self.ax.axis('auto')
+            elif plot_type == 'Amplitude (linear)':
+                self.ax.set_xlabel('Frequency (Hz)')
+                self.ax.set_ylabel('Amplitude')
+                self.ax.axis('auto')
+            elif plot_type == 'Real Part':
+                self.ax.set_xlabel('Frequency (Hz)')
+                self.ax.set_ylabel('Real Part')
+                self.ax.axis('auto')
+            elif plot_type == 'Imag Part':
+                self.ax.set_xlabel('Frequency (Hz)')
+                self.ax.set_ylabel('Imag Part')
+                self.ax.axis('auto')
+            elif plot_type == 'Nyquist':
+                self.ax.set_xlabel('Real Part')
+                self.ax.set_ylabel('Imag Part')
+                self.ax.set_aspect('equal','datalim')
+            elif plot_type == 'Phase':
+                self.ax.set_xlabel('Frequency (Hz)')
+                self.ax.set_ylabel('Phase (deg)')
+                self.ax.axis('auto')
+                
+            self.ax.set_xscale(xlinlog)
+            if 'log' in xlinlog:
+                self.ax.grid(visible=True, which='minor',axis='x',alpha=0.2)
+            else:
+                self.ax.grid(visible=False)
+            
+        elif data_list.__class__.__name__ == 'TfDataList':
+            if (plot_type == 'Amplitude (dB)') or (plot_type == None):
+                self.ax.set_xlabel('Frequency (Hz)')
+                self.ax.set_ylabel('Amplitude (dB)')
+                self.ax.axis('auto')
+            elif plot_type == 'Amplitude (linear)':
+                self.ax.set_xlabel('Frequency (Hz)')
+                self.ax.set_ylabel('Amplitude')
+                self.ax.axis('auto')
+            elif plot_type == 'Real Part':
+                self.ax.set_xlabel('Frequency (Hz)')
+                self.ax.set_ylabel('Real Part')
+                self.ax.axis('auto')
+            elif plot_type == 'Imag Part':
+                self.ax.set_xlabel('Frequency (Hz)')
+                self.ax.set_ylabel('Imag Part')
+                self.ax.axis('auto')
+            elif plot_type == 'Nyquist':
+                self.ax.set_xlabel('Real Part')
+                self.ax.set_ylabel('Imag Part')
+                self.ax.set_aspect('equal','datalim')
+            elif plot_type == 'Phase':
+                self.ax.set_xlabel('Frequency (Hz)')
+                self.ax.set_ylabel('Phase (deg)')
+                self.ax.axis('auto')
+            
+            
+            self.ax.set_xscale(xlinlog)
+            if 'log' in xlinlog:
+                self.ax.grid(visible=True, which='minor',axis='x',alpha=0.2)
+            else:
+                self.ax.grid(visible=False)
+            
+            # setup twin axis
+            # don't plot coherence if no data, or if all coherence is one
+            flag_coherence = []
+            for n_set in range(len(data_list)):
+                if data_list[n_set].tf_coherence is None:
+                    flag_coherence += [True]
+                else:
+                    tfc = data_list[n_set].tf_coherence
+                    i = np.isnan(tfc)
+                    tfc[i] = 1
+                    diff_to_one = np.abs(tfc - 1)
+                    flag_coherence += [np.all(diff_to_one<1e-10)]
+            if np.all(flag_coherence):
+                show_coherence = False
+            
+            if show_coherence == True:
+                self.ax2.set_ylabel('Coherence')
+                self.ax2.set_visible(True)
+            else:
+                self.ax2.set_visible(False)
+    
+        # sonogram plot completely different, use separate function
+        
+        N_sets = len(data_list)
+
+        # pre-count how many channels total
+        ch_counter = 0
+        for n_set in range(N_sets):
+            if data_list.__class__.__name__ == 'TimeDataList':
+                ch_counter += len(data_list[n_set].time_data[0,:])
+            elif data_list.__class__.__name__ == 'FreqDataList':
+                ch_counter += len(data_list[n_set].freq_data[0,:])
+            elif data_list.__class__.__name__ == 'TfDataList':
+                ch_counter += len(data_list[n_set].tf_data[0,:])
+
+        self.ch_total = ch_counter
+        if self.ch_total <= 12:
+            LINE_ALPHA = 0.9
+        else:
+            # option to make lines fainter when more lines... needs some tweaking to make feel right
+            LINE_ALPHA = 1-1/self.ch_total # make deselected lines fainter if more channels
+        
+        [line.remove() for line in self.ax.lines]
+        [line.remove() for line in self.ax2.lines]
+        self.line_listbyset = []
+        self.line2_listbyset = []
+        
+        if sets == 'all':
+            sets = range(N_sets)
+        count = -1
+        for n_set in range(len(data_list)):
+            self.line_listbyset.append([])
+            self.line2_listbyset.append([])
+            
+            if data_list.__class__.__name__ == 'TfDataList':
+                N_chans = len(data_list[n_set].tf_data[0,:])
+            elif data_list.__class__.__name__ == 'FreqDataList':
+                N_chans = len(data_list[n_set].freq_data[0,:])
+            elif data_list.__class__.__name__ == 'TimeDataList':
+                N_chans = len(data_list[n_set].time_data[0,:])
+                
+            if channels == 'all':
+                channels = range(N_chans)
+
+            
+
+            for n_chan in range(N_chans):
+                count += 1
+                if (n_set not in sets) or (n_chan not in channels):
+                    alpha = 1-LINE_ALPHA
+                else:
+                    alpha = LINE_ALPHA
+                
+                if data_list.__class__.__name__ == 'TimeDataList':
+                    x = data_list[n_set].time_axis
+                    y = data_list[n_set].time_data[:,n_chan] * data_list[n_set].channel_cal_factors[n_chan]
+        
+                elif data_list.__class__.__name__ == 'FreqDataList':
+                    x = data_list[n_set].freq_axis
+                    ylin = data_list[n_set].freq_data[:,n_chan] * data_list[n_set].channel_cal_factors[n_chan]
+                    
+                    
+                    if (plot_type == 'Amplitude (dB)') or (plot_type == None):
+                        # handle log(0) manually to avoid warnings
+                        y = np.zeros(np.shape(ylin))
+                        izero = ylin==0
+                        y[~izero] = 20*np.log10(np.abs(ylin[~izero]))
+                        y[izero] = -np.inf
+                    elif plot_type == 'Amplitude (linear)':
+                        y = np.abs(ylin)
+                    elif plot_type == 'Real Part':
+                        y = np.real(ylin)
+                    elif plot_type == 'Imag Part':
+                        y = np.imag(ylin)
+                    elif plot_type == 'Nyquist':
+                        if freq_range == None:
+                            freq_range = [-1,np.inf]
+                        selected_data = np.where((x>freq_range[0]) * (x<freq_range[1]))[0]
+                        x = np.real(ylin[selected_data])
+                        y = np.imag(ylin[selected_data])
+                        
+                    elif plot_type == 'Phase':
+                        y = np.angle(ylin,deg=True)
+                        
+                    
+                elif data_list.__class__.__name__ == 'TfDataList':
+                    x = data_list[n_set].freq_axis
+                    ylin = data_list[n_set].tf_data[:,n_chan] * data_list[n_set].channel_cal_factors[n_chan]
+                    if (plot_type == 'Amplitude (dB)') or (plot_type == None):
+                        # handle log(0) manually to avoid warnings
+                        y = np.zeros(np.shape(ylin))
+                        izero = ylin==0
+                        y[~izero] = 20*np.log10(np.abs(ylin[~izero]))
+                        y[izero] = -np.inf
+                        
+                    elif plot_type == 'Amplitude (linear)':
+                        y = np.abs(ylin)
+                    elif plot_type == 'Real Part':
+                        y = np.real(ylin)
+                    elif plot_type == 'Imag Part':
+                        y = np.imag(ylin)
+                    elif plot_type == 'Nyquist':
+                        if freq_range == None:
+                            freq_range = [-1,np.inf]
+                        selected_data = np.where((x>freq_range[0]) * (x<freq_range[1]))[0]
+                        x = np.real(ylin[selected_data])
+                        y = np.imag(ylin[selected_data])
+                    elif plot_type == 'Phase':
+                        y = np.angle(ylin,deg=True)
+                    if data_list[n_set].tf_coherence is not None:
+                        # handle log(0) manually to avoid warnings
+                        yclin = data_list[n_set].tf_coherence[:,n_chan]
+                        if coherence_plot_type == 'linear':
+                            yc = yclin
+                        elif coherence_plot_type == 'log':
+                            yc = np.zeros(np.shape(yclin))
+                            izero = yclin==0
+                            yc[~izero] = 20*np.log10(np.abs(yclin[~izero]))
+                            yc[izero] = -np.inf
+                            yc = 20*np.log10(np.abs(yclin))
+                    else:
+                        yc = np.ones(np.shape(data_list[n_set].tf_data))
+                        
+                        
+                color = options.set_plot_colours(ch_counter)[count,:]/255
+                
+                if type(data_list[n_set].test_name) is str:
+                    test_name = data_list[n_set].test_name
+                else:
+                    test_name = ''
+                    
+                if test_name != '':
+                    test_name = test_name + ': '
+                    
+                if self.ch_total < 10:
+                    label = '{}set_{}, ch_{}'.format(test_name,n_set,n_chan)
+                else:
+                    label = 'set{},ch{}'.format(n_set,n_chan)
+                    
+                if data_list.__class__.__name__ == 'TfDataList':
+                    if data_list[n_set].flag_modal_TF == True:
+                        label = 'fit{}'.format(n_chan)
+                        
+                self.line_listbyset[n_set] += self.ax.plot(x,y,'-',linewidth=1,color = color,label=label,alpha=alpha)
+                
+                if data_list.__class__.__name__ == 'TfDataList':
+                    if show_coherence == True:
+                        self.line2_listbyset[n_set] += self.ax2.plot(x,yc,':',linewidth=1,color = color,label=label+' (coherence)',alpha=alpha)
+                        self.ax2.set_visible(True)
+                    else:
+                        self.ax2.set_visible(False)
+        
+        self.fig.tight_layout()
+        self.fig.canvas.draw()
+        self.update_legend()
+        if 'x' in auto_xy:
+            self.auto_x()
+        if 'f' in auto_xy: # use freq_range for x axis
+            if ('log' in xlinlog) and freq_range[0]==0:
+                self.lines = self.ax.get_lines()
+                xminlog = np.inf
+                for line in self.lines:
+                    if line.get_alpha() > 0.5:
+                        data = line.get_data()
+                        xxlog = data[0][1] # first nonzero freq axis
+                        xminlog = min([xminlog,xxlog])
+                        freq_range[0] = xminlog
+                self.ax.set_xlim(freq_range)
+            else:
+                self.ax.set_xlim(freq_range)
+            self.fig.canvas.draw()
+            self.auto_y()
+        if 'y' in auto_xy:
+            self.auto_y()
+        if 'c' in auto_xy: # auto coherence y
+            self.ax2.set_ylim([0,1])
+            
+#        self.ax.xaxis.set_major_locator(AutoLocator())
+#        self.ax.yaxis.set_major_locator(AutoLocator())
+        self.fig.canvas.draw()
+        
+        
+        
+    def update_legend(self,loc='lower right',draggable=False):
+        
+        if len(self.data_list) != 0:
+            if self.ax.get_legend() is None:
+                self.visibility = True
+                
+            if self.ch_total >= 10:
+                # make legend more compact
+                col_sizes = np.arange(10,7,-1)
+                rem = np.remainder(self.ch_total,col_sizes)
+                if any(rem==0):
+                    remi = np.where(rem==0)[0]
+                    remi = remi[0]
+                    ncol = int(self.ch_total / col_sizes[remi])
+                else:
+                    remi = np.argmax(rem)
+                    ncol = int(np.ceil(self.ch_total/ col_sizes[remi]))
+            else:
+                ncol = 1
+                
+            self.legend = self.ax.legend(loc=loc, ncol=ncol)
+#            self.ax.legend()
+            self.legend.set_draggable(draggable,use_blit=True)#(True),update='bbox',use_blit=True
+            self.lines = self.ax.get_lines()
+            self.lines2 = self.ax2.get_lines()
+            self.lined = dict()
+            self.lined2 = dict()
+
+            # make dictionary of legend lines for selection    
+            for legline, origline in zip(self.legend.get_lines(), self.lines):
+                legline.set_picker(True)  # argument tolerance
+                legline.set_pickradius(10)  # argument tolerance
+                self.lined[legline] = origline
+                legline.set_alpha(origline.get_alpha())
+
+            # make dictionary of coherence lines to select with legend - only for TF Data
+            if len(self.ax2.lines) > 0:
+                for legline, origline2 in zip(self.legend.get_lines(), self.lines2):
+                    self.lined2[legline] = origline2 
+                    origline2.set_alpha(legline.get_alpha())
+                    
+            self.ax.get_legend().set_visible(self.visibility)
+        else:
+            self.legend = self.ax.get_legend()
+            if self.legend is not None:
+                self.legend.remove()
+            self.fig.canvas.draw()
+    
+    
+    def auto_x(self):
+        if self.data_list.__class__.__name__ == 'SonoDataList':
+            xlim = self.data_list[self.n_set].time_axis[[0,-1]]
+            self.ax.set_xlim(xlim)
+        else:
+            self.lines = self.ax.get_lines()
+            xmin = np.inf
+            xminlog = np.inf
+            xmax = -np.inf
+            ymin = np.inf # for Nyquist to stop cropping
+            ymax = -np.inf
+            for line in self.lines:
+                if line.get_alpha() > 0.5:
+                    data = line.get_data()
+                    try:
+                        # handle when some lines are out of view
+                        xx = min(data[0])
+                        xmin = min([xx,xmin])
+                        
+                        xxlog = data[0][1] # first nonzero freq axis
+                        xminlog = min([xminlog,xxlog])
+                        
+                        xx = max(data[0])
+                        xmax = max([xx,xmax])
+                        if self.plot_type == 'Nyquist':
+                            yy = min(data[1])
+                            ymin = min([yy,ymin])
+                            yy = max(data[1])
+                            ymax = max([yy,ymax])
+                    except:
+                        pass
+            try:
+                if 'log' in self.xlinlog:
+                    self.ax.set_xlim([xminlog,xmax])
+                else:
+                    if self.plot_type == 'Nyquist':
+                        # equal axis means need x range needs to stay greater than y range
+                        yrange = ymax-ymin
+                        # get bounding box bb to know current aspect ratio ar
+                        bb=self.ax.get_window_extent().transformed(self.fig.dpi_scale_trans.inverted())
+                        ar = bb.width / bb.height
+                        if (xmax-xmin) < (ar*yrange):
+                            xmid = (xmin+xmax)/2
+                            xmax = xmid + ar*yrange/2
+                            xmin = xmid - ar*yrange/2
+                        
+                    self.ax.set_xlim([xmin,xmax])
+                    
+            except:
+                pass
+        self.fig.canvas.draw()
+        
+        
+    def auto_y(self):
+        if self.data_list.__class__.__name__ == 'SonoDataList':
+            ylim = self.data_list[self.n_set].freq_axis[[0,-1]]
+            self.ax.set_ylim(ylim)
+        else:
+            self.lines = self.ax.get_lines()
+            if (self.data_list.__class__.__name__ == 'TfData') and (self.plot_type != 'Nyquist'):
+                # at the moment this doesn't get called
+                # it should be TfDataList in condition
+                # and it should be == nyquist not !=
+                # but plot behaviour correct as it stands and probably just need this setting to xlim always
+                xview = self.freq_range
+            else:
+                xview = self.ax.get_xlim()
+            ymin = np.inf
+            ymax = -np.inf
+            c=-1
+            for line in self.lines:
+                c+=1
+                data = line.get_data() 
+                x = data[0]
+                selection = (xview[0] < x) & (x < xview[1])
+                if line.get_alpha() > 0.5:
+                    try:
+                        # handle case when some lines out of view
+                        yy = min(data[1][selection])
+                        ymin = min([yy,ymin])
+                        yy = max(data[1][selection])
+                        ymax = max([yy,ymax])
+                    except:
+                        pass
+            try:
+                self.ax.set_ylim([ymin,ymax])
+            except:
+                pass
+        if self.data_list.__class__.__name__ == 'TfDataList':
+            # reset coherence to 0-1
+            self.ax2.set_ylim([0,1])
+            
+        self.fig.canvas.draw()
+        
+    def channel_select(self,event):
+        selected_line = event.artist
+        
+        a = selected_line.get_alpha()
+        # This function is called when legend dragged, and a is None
+        # So only want to change line opacity when line actually selected.
+        if a is not None:
+            # change opacity of both legend line and actual line
+            a = 1-a
+            origline = self.lined[selected_line]
+            
+
+            selected_line.set_alpha(a)
+            origline.set_alpha(a)
+            
+            # change z order to bring selected line to foreground
+            for line in self.ax.lines:
+                line.set_zorder(0)
+            if a > 0.5:
+                origline.set_zorder(1)
+            else:
+                origline.set_zorder(0)
+                
+            # also select matching coherence lines
+            if len(self.ax2.lines) > 0:
+                origline2 = self.lined2[selected_line]
+                origline2.set_alpha(a)
+                for line2 in self.ax2.lines:
+                    line2.set_zorder(0)
+                if a > 0.5:
+                    origline2.set_zorder(1)
+                else:
+                    origline2.set_zorder(0)
+            self.fig.canvas.draw()
+    
+    def get_selected_channels(self):
+        # find the sets and channels higlighted in figure
+        
+        n_sets = len(self.line_listbyset)
+        selected_data = []
+        
+        for ns in range(n_sets):
+            selected_data += [[]]
+            for line in self.line_listbyset[ns]:
+                selected_data[ns] += [line.get_alpha() > 0.5] # skip coherence lines
+            
+        return selected_data
+    
+    def set_selected_channels(self,s):
+        global LINE_ALPHA
+        # relies on all sets of data with same number of channels. Need to make more general.
+        for n_set in range(len(s)):
+            for n_chan in range(len(s[n_set])):
+                if s[n_set][n_chan] == True:
+                    self.line_listbyset[n_set][n_chan].set_alpha(LINE_ALPHA)
+                else:
+                    self.line_listbyset[n_set][n_chan].set_alpha(1-LINE_ALPHA)
+        # make legend line alphas match actual lines, but keep visibility as before
+        self.update_legend()
+        self.fig.canvas.draw()
+        
+    def update_sonogram(self,sono_data_list,n_set,n_chan,db_range=60,auto_xy='xy'):
+        self.data_list = sono_data_list # makes auto_x/y work!
+        
+        for ch in self.ax.get_children():
+                if ch.__class__.__name__ == 'QuadMesh':
+                    ch.remove()
+        
+        self.n_set = n_set
+        self.n_chan = n_chan
+        self.ax2.set_visible(False)
+        self.ax.set_xlabel('Time (s)')
+        self.ax.set_ylabel('Frequency (Hz)')
+        self.ax.grid(False)
+        if self.ax.get_legend() is not None:
+            self.ax.get_legend().set_visible(False)
+        
+        [line.remove() for line in self.ax.lines]
+        [line.remove() for line in self.ax2.lines]
+        self.line_listbyset = []
+        self.line2_listbyset = []
+        
+        f = sono_data_list[n_set].freq_axis
+        t = sono_data_list[n_set].time_axis
+        S = sono_data_list[n_set].sono_data[:,:,n_chan]
+        S[S==0] = 1e-16 # avoid log10(0) warnings
+        SdB = 20*np.log10(np.abs(S))
+        vmax = SdB.max()
+        vmin = np.max([SdB.min(),vmax-db_range])
+        self.pcolor_sono = self.ax.pcolormesh(t,f,SdB,shading='gouraud',cmap='Blues',vmax=vmax,vmin=vmin,rasterized=True)
+        if 'x' in auto_xy:
+            self.auto_x()
+        if 'y' in auto_xy:
+            self.auto_y()
+
+#        self.fig.colorbar(ax=self.ax)
+        self.fig.canvas.draw()
+        
+        
+    
+    
+    
+
+
```

### Comparing `pydvma-0.9.0/pydvma/testdata.py` & `pydvma-0.9.1/pydvma/testdata.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Aug 27 17:08:42 2018
-
-@author: tb267
-"""
-
-from . import options
-from . import datastructure
-
-import numpy as np
-import datetime
-
-
-    
-
-#%% Create test data
-def create_test_impulse_data(noise_level=0):
-    '''
-    Creates example time domain data simulating impulse hammer test
-    '''
-    settings = options.MySettings(fs=10000)
-    N = int(1e4)
-    time_axis = np.arange(N)/settings.fs
-    
-    time_data = np.zeros([N,2])
-    pulse_width = 0.002
-    N_pulse = int(np.ceil(pulse_width*settings.fs))
-    n = np.arange(N_pulse)
-    pulse = 0.5*(1-np.cos(2*np.pi*n/N_pulse))
-    time_data[n,0] = pulse
-    
-    test_freq = 100
-    test_time_const = 0.1
-    y = np.exp(-time_axis/test_time_const) * np.sin(2*np.pi*test_freq*time_axis)
-    
-    y += noise_level*2*(np.random.rand(len(y)) - 0.5)
-    
-    time_data[:,1] = y
-    
-    t = datetime.datetime.now()
-    timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)
-    
-    timedata = datastructure.TimeData(time_axis,time_data,settings,timestamp=t, timestring=timestring, units=['N','m/s'], channel_cal_factors=[1,1], test_name='Synthesised data')
-    #metadata = MetaData(, tf_cal_factors=1)
-    
-    dataset = datastructure.DataSet()
-    dataset.add_to_dataset(timedata)
-    
-    return dataset
-
-def create_test_impulse_ensemble(N_ensemble=5, noise_level=0.1):
-    '''
-    Creates ensemble of example time domain data simulating impulse hammer tests
-    '''
-    dataset = datastructure.DataSet()
-    for n in range(N_ensemble):
-        d = create_test_impulse_data(noise_level=noise_level)
-        dataset.add_to_dataset(d.time_data_list)
-    
-    return dataset
-
-
-def create_test_noise_data(added_noise_level=0.1):
-    '''
-    Creates example time domain data simulating noise input test
-    '''
-    settings = options.MySettings(fs=10000)
-    N = int(10*1e4)
-    time_axis = np.arange(N)/settings.fs
-    
-    time_data = np.zeros([N,2])
-    x = np.random.rand(N) - 0.5
-    test_freq = 100
-    test_time_const = 0.1
-    g = np.exp(-time_axis/test_time_const) * np.sin(2*np.pi*test_freq*time_axis)
-    y = np.convolve(x,g)
-    y = y[0:len(x)]
-    
-    added_noise = added_noise_level*2*(np.random.rand(N)-0.5)
-    time_data[:,0] = x
-    time_data[:,1] = y + added_noise
-    
-    t = datetime.datetime.now()
-    timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)
-    
-    timedata = datastructure.TimeData(time_axis,time_data,settings,timestamp=t, timestring=timestring, units=['N','m/s'], channel_cal_factors=[1,1], test_name='Synthesised data')
-    
-    dataset = datastructure.DataSet()
-    dataset.add_to_dataset(timedata)
-    
-    return dataset
-    
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Aug 27 17:08:42 2018
+
+@author: tb267
+"""
+
+from . import options
+from . import datastructure
+
+import numpy as np
+import datetime
+
+
+    
+
+#%% Create test data
+def create_test_impulse_data(noise_level=0):
+    '''
+    Creates example time domain data simulating impulse hammer test
+    '''
+    settings = options.MySettings(fs=10000)
+    N = int(1e4)
+    time_axis = np.arange(N)/settings.fs
+    
+    time_data = np.zeros([N,2])
+    pulse_width = 0.002
+    N_pulse = int(np.ceil(pulse_width*settings.fs))
+    n = np.arange(N_pulse)
+    pulse = 0.5*(1-np.cos(2*np.pi*n/N_pulse))
+    time_data[n,0] = pulse
+    
+    test_freq = 100
+    test_time_const = 0.1
+    y = np.exp(-time_axis/test_time_const) * np.sin(2*np.pi*test_freq*time_axis)
+    
+    y += noise_level*2*(np.random.rand(len(y)) - 0.5)
+    
+    time_data[:,1] = y
+    
+    t = datetime.datetime.now()
+    timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)
+    
+    timedata = datastructure.TimeData(time_axis,time_data,settings,timestamp=t, timestring=timestring, units=['N','m/s'], channel_cal_factors=[1,1], test_name='Synthesised data')
+    #metadata = MetaData(, tf_cal_factors=1)
+    
+    dataset = datastructure.DataSet()
+    dataset.add_to_dataset(timedata)
+    
+    return dataset
+
+def create_test_impulse_ensemble(N_ensemble=5, noise_level=0.1):
+    '''
+    Creates ensemble of example time domain data simulating impulse hammer tests
+    '''
+    dataset = datastructure.DataSet()
+    for n in range(N_ensemble):
+        d = create_test_impulse_data(noise_level=noise_level)
+        dataset.add_to_dataset(d.time_data_list)
+    
+    return dataset
+
+
+def create_test_noise_data(added_noise_level=0.1):
+    '''
+    Creates example time domain data simulating noise input test
+    '''
+    settings = options.MySettings(fs=10000)
+    N = int(10*1e4)
+    time_axis = np.arange(N)/settings.fs
+    
+    time_data = np.zeros([N,2])
+    x = np.random.rand(N) - 0.5
+    test_freq = 100
+    test_time_const = 0.1
+    g = np.exp(-time_axis/test_time_const) * np.sin(2*np.pi*test_freq*time_axis)
+    y = np.convolve(x,g)
+    y = y[0:len(x)]
+    
+    added_noise = added_noise_level*2*(np.random.rand(N)-0.5)
+    time_data[:,0] = x
+    time_data[:,1] = y + added_noise
+    
+    t = datetime.datetime.now()
+    timestring = '_'+str(t.year)+'_'+str(t.month)+'_'+str(t.day)+'_at_'+str(t.hour)+'_'+str(t.minute)+'_'+str(t.second)
+    
+    timedata = datastructure.TimeData(time_axis,time_data,settings,timestamp=t, timestring=timestring, units=['N','m/s'], channel_cal_factors=[1,1], test_name='Synthesised data')
+    
+    dataset = datastructure.DataSet()
+    dataset.add_to_dataset(timedata)
+    
+    return dataset
+
```

