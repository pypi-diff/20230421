# Comparing `tmp/globalemu-1.5.1.tar.gz` & `tmp/globalemu-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalemu-1.5.1.tar", last modified: Sat Nov 13 09:35:16 2021, max compression
+gzip compressed data, was "globalemu-1.6.0.tar", last modified: Fri Apr 21 11:54:26 2023, max compression
```

## Comparing `globalemu-1.5.1.tar` & `globalemu-1.6.0.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxrwxr-x   0 harry     (1000) harry     (1000)        0 2021-11-13 09:35:16.733454 globalemu-1.5.1/
--rw-rw-r--   0 harry     (1000) harry     (1000)     1082 2021-08-26 16:38:43.000000 globalemu-1.5.1/LICENSE
--rw-rw-r--   0 harry     (1000) harry     (1000)       25 2021-08-26 16:38:43.000000 globalemu-1.5.1/MANIFEST.in
--rw-rw-r--   0 harry     (1000) harry     (1000)    10102 2021-11-13 09:35:16.733454 globalemu-1.5.1/PKG-INFO
--rw-rw-r--   0 harry     (1000) harry     (1000)     9357 2021-11-13 09:27:32.000000 globalemu-1.5.1/README.rst
-drwxrwxr-x   0 harry     (1000) harry     (1000)        0 2021-11-13 09:35:16.733454 globalemu-1.5.1/globalemu/
--rw-rw-r--   0 harry     (1000) harry     (1000)        0 2021-08-26 16:38:43.000000 globalemu-1.5.1/globalemu/__init__.py
--rw-rw-r--   0 harry     (1000) harry     (1000)     2331 2021-08-26 16:38:43.000000 globalemu-1.5.1/globalemu/cmSim.py
--rw-rw-r--   0 harry     (1000) harry     (1000)     1854 2021-08-26 16:38:43.000000 globalemu-1.5.1/globalemu/downloads.py
--rw-rw-r--   0 harry     (1000) harry     (1000)    10545 2021-08-26 16:38:43.000000 globalemu-1.5.1/globalemu/eval.py
--rw-rw-r--   0 harry     (1000) harry     (1000)     4689 2021-08-26 16:38:43.000000 globalemu-1.5.1/globalemu/gui_config.py
--rw-rw-r--   0 harry     (1000) harry     (1000)      957 2021-08-26 16:38:43.000000 globalemu-1.5.1/globalemu/losses.py
--rw-rw-r--   0 harry     (1000) harry     (1000)     1594 2021-08-26 16:38:43.000000 globalemu-1.5.1/globalemu/models.py
--rw-rw-r--   0 harry     (1000) harry     (1000)    14394 2021-11-13 09:27:03.000000 globalemu-1.5.1/globalemu/network.py
--rw-rw-r--   0 harry     (1000) harry     (1000)     8446 2021-08-26 16:38:43.000000 globalemu-1.5.1/globalemu/plotter.py
--rw-rw-r--   0 harry     (1000) harry     (1000)    10698 2021-08-26 16:38:43.000000 globalemu-1.5.1/globalemu/preprocess.py
--rw-rw-r--   0 harry     (1000) harry     (1000)     1626 2021-08-26 16:38:43.000000 globalemu-1.5.1/globalemu/resample.py
-drwxrwxr-x   0 harry     (1000) harry     (1000)        0 2021-11-13 09:35:16.733454 globalemu-1.5.1/globalemu.egg-info/
--rw-rw-r--   0 harry     (1000) harry     (1000)    10102 2021-11-13 09:35:16.000000 globalemu-1.5.1/globalemu.egg-info/PKG-INFO
--rw-rw-r--   0 harry     (1000) harry     (1000)      472 2021-11-13 09:35:16.000000 globalemu-1.5.1/globalemu.egg-info/SOURCES.txt
--rw-rw-r--   0 harry     (1000) harry     (1000)        1 2021-11-13 09:35:16.000000 globalemu-1.5.1/globalemu.egg-info/dependency_links.txt
--rw-rw-r--   0 harry     (1000) harry     (1000)       83 2021-11-13 09:35:16.000000 globalemu-1.5.1/globalemu.egg-info/requires.txt
--rw-rw-r--   0 harry     (1000) harry     (1000)       10 2021-11-13 09:35:16.000000 globalemu-1.5.1/globalemu.egg-info/top_level.txt
--rw-rw-r--   0 harry     (1000) harry     (1000)       42 2021-08-26 16:38:43.000000 globalemu-1.5.1/requirements.txt
-drwxrwxr-x   0 harry     (1000) harry     (1000)        0 2021-11-13 09:35:16.733454 globalemu-1.5.1/scripts/
--rw-rw-r--   0 harry     (1000) harry     (1000)     4699 2021-11-13 09:25:05.000000 globalemu-1.5.1/scripts/globalemu
--rw-rw-r--   0 harry     (1000) harry     (1000)       38 2021-11-13 09:35:16.733454 globalemu-1.5.1/setup.cfg
--rw-rw-r--   0 harry     (1000) harry     (1000)     1285 2021-11-13 09:27:28.000000 globalemu-1.5.1/setup.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-21 11:54:26.269770 globalemu-1.6.0/
+-rw-r--r--   0 harry      (501) staff       (20)     1082 2022-09-02 15:51:21.000000 globalemu-1.6.0/LICENSE
+-rw-r--r--   0 harry      (501) staff       (20)       25 2022-09-02 15:51:21.000000 globalemu-1.6.0/MANIFEST.in
+-rw-r--r--   0 harry      (501) staff       (20)    10082 2023-04-21 11:54:26.269607 globalemu-1.6.0/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)     9357 2023-04-21 11:53:48.000000 globalemu-1.6.0/README.rst
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-21 11:54:26.267839 globalemu-1.6.0/globalemu/
+-rw-r--r--   0 harry      (501) staff       (20)        0 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/__init__.py
+-rw-r--r--   0 harry      (501) staff       (20)     2331 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/cmSim.py
+-rw-r--r--   0 harry      (501) staff       (20)     1854 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/downloads.py
+-rw-r--r--   0 harry      (501) staff       (20)    10537 2023-04-21 11:53:48.000000 globalemu-1.6.0/globalemu/eval.py
+-rw-r--r--   0 harry      (501) staff       (20)     4689 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/gui_config.py
+-rw-r--r--   0 harry      (501) staff       (20)      957 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/losses.py
+-rw-r--r--   0 harry      (501) staff       (20)     1594 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/models.py
+-rw-r--r--   0 harry      (501) staff       (20)    14428 2023-04-21 11:53:48.000000 globalemu-1.6.0/globalemu/network.py
+-rw-r--r--   0 harry      (501) staff       (20)     8446 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/plotter.py
+-rw-r--r--   0 harry      (501) staff       (20)    12993 2023-04-21 11:53:48.000000 globalemu-1.6.0/globalemu/preprocess.py
+-rw-r--r--   0 harry      (501) staff       (20)     1626 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/resample.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-21 11:54:26.268452 globalemu-1.6.0/globalemu.egg-info/
+-rw-r--r--   0 harry      (501) staff       (20)    10082 2023-04-21 11:54:26.000000 globalemu-1.6.0/globalemu.egg-info/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)      628 2023-04-21 11:54:26.000000 globalemu-1.6.0/globalemu.egg-info/SOURCES.txt
+-rw-r--r--   0 harry      (501) staff       (20)        1 2023-04-21 11:54:26.000000 globalemu-1.6.0/globalemu.egg-info/dependency_links.txt
+-rw-r--r--   0 harry      (501) staff       (20)       83 2023-04-21 11:54:26.000000 globalemu-1.6.0/globalemu.egg-info/requires.txt
+-rw-r--r--   0 harry      (501) staff       (20)       10 2023-04-21 11:54:26.000000 globalemu-1.6.0/globalemu.egg-info/top_level.txt
+-rw-r--r--   0 harry      (501) staff       (20)       42 2023-04-21 08:08:31.000000 globalemu-1.6.0/requirements.txt
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-21 11:54:26.268569 globalemu-1.6.0/scripts/
+-rw-r--r--   0 harry      (501) staff       (20)     4699 2022-09-02 15:51:21.000000 globalemu-1.6.0/scripts/globalemu
+-rw-r--r--   0 harry      (501) staff       (20)       38 2023-04-21 11:54:26.269806 globalemu-1.6.0/setup.cfg
+-rw-r--r--   0 harry      (501) staff       (20)     1285 2023-04-21 11:53:48.000000 globalemu-1.6.0/setup.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-21 11:54:26.269449 globalemu-1.6.0/tests/
+-rw-r--r--   0 harry      (501) staff       (20)      408 2022-09-02 15:51:21.000000 globalemu-1.6.0/tests/test_cmsim.py
+-rw-r--r--   0 harry      (501) staff       (20)     1315 2023-04-21 11:53:48.000000 globalemu-1.6.0/tests/test_download.py
+-rw-r--r--   0 harry      (501) staff       (20)     2102 2023-04-21 10:57:50.000000 globalemu-1.6.0/tests/test_eval.py
+-rw-r--r--   0 harry      (501) staff       (20)     1863 2023-04-21 11:53:48.000000 globalemu-1.6.0/tests/test_gui_config.py
+-rw-r--r--   0 harry      (501) staff       (20)     2301 2023-04-21 11:53:48.000000 globalemu-1.6.0/tests/test_network.py
+-rw-r--r--   0 harry      (501) staff       (20)     2917 2023-04-21 11:53:48.000000 globalemu-1.6.0/tests/test_plotter.py
+-rw-r--r--   0 harry      (501) staff       (20)     2363 2023-04-21 11:53:48.000000 globalemu-1.6.0/tests/test_preprocess.py
```

### Comparing `globalemu-1.5.1/LICENSE` & `globalemu-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `globalemu-1.5.1/PKG-INFO` & `globalemu-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: globalemu
-Version: 1.5.1
+Version: 1.6.0
 Summary: globalemu: Robust and Fast Global 21-cm Signal Emulation
 Home-page: https://github.com/htjb/globalemu
 Author: Harry T. J. Bevins
 Author-email: htjb2@cam.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
@@ -24,15 +23,15 @@
 ========================================================
 
 Introduction
 ------------
 
 :globalemu: Robust Global 21-cm Signal Emulation
 :Author: Harry Thomas Jones Bevins
-:Version: 1.5.1
+:Version: 1.6.0
 :Homepage: https://github.com/htjb/globalemu
 :Documentation: https://globalemu.readthedocs.io/
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/htjb/globalemu/master?filepath=notebooks%2F
 .. image:: https://readthedocs.org/projects/globalemu/badge/?version=latest
  :target: https://globalemu.readthedocs.io/en/latest/?badge=latest
@@ -308,9 +307,7 @@
 ------------
 
 Contributions to ``globalemu`` are very much welcome and can be made via,
 
 - Opening an issue to report a bug/propose a new feature.
 - Making a pull request. Please consider opening an issue first to discuss
   any proposals and ensure the PR will be accepted.
-
-
```

### Comparing `globalemu-1.5.1/README.rst` & `globalemu-1.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ========================================================
 
 Introduction
 ------------
 
 :globalemu: Robust Global 21-cm Signal Emulation
 :Author: Harry Thomas Jones Bevins
-:Version: 1.5.1
+:Version: 1.6.0
 :Homepage: https://github.com/htjb/globalemu
 :Documentation: https://globalemu.readthedocs.io/
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/htjb/globalemu/master?filepath=notebooks%2F
 .. image:: https://readthedocs.org/projects/globalemu/badge/?version=latest
  :target: https://globalemu.readthedocs.io/en/latest/?badge=latest
```

### Comparing `globalemu-1.5.1/globalemu/cmSim.py` & `globalemu-1.6.0/globalemu/cmSim.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.5.1/globalemu/downloads.py` & `globalemu-1.6.0/globalemu/downloads.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.5.1/globalemu/eval.py` & `globalemu-1.6.0/globalemu/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,9 +242,9 @@
                 evaluation *= self.label_stds
 
         if self.preprocess_settings['AFB'] is True:
             evaluation += np.interp(self.z, self.original_z, self.AFB)
 
         if type(evaluation) is not np.ndarray:
             evaluation = np.array(evaluation)
-        
+
         return evaluation, self.z
```

### Comparing `globalemu-1.5.1/globalemu/gui_config.py` & `globalemu-1.6.0/globalemu/gui_config.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.5.1/globalemu/losses.py` & `globalemu-1.6.0/globalemu/losses.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.5.1/globalemu/models.py` & `globalemu-1.6.0/globalemu/models.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.5.1/globalemu/network.py` & `globalemu-1.6.0/globalemu/network.py`

 * *Files 16% similar despite different names*

```diff
@@ -70,26 +70,16 @@
             | This should be the same as the ``base_dir`` used when
                 preprocessing. It contains the data that the network will
                 work with and is the directory in which the trained model will
                 be saved in.
 
         early_stop: **Bool / default: False**
             | If ``early_stop`` is set too ``True`` then the network will stop
-                learning if the loss has not changed up to an accuracy given
-                by ``early_stop_lim`` within the last ten epochs.
-
-        early_stop_lim: **float / default: 1e-4**
-            | The precision with which to assess the change in loss over the
-                last ten epochs when ``early_stop=True``. The value of this
-                parameter is strongly dependent on the magnitude of the
-                evaluated loss at each epoch and the default may be to high or
-                too low for the desired outcome. For example if our loss value
-                is initially 0.01 and decreases with each epoch then a
-                ``epoch_stop_lim`` of 0.1 will cause training to stop after
-                10 epochs and give poor results.
+                learning if the loss has not changed within
+                the last twenty epochs.
 
         xHI: **Bool / default: False**
             | If True then ``globalemu`` will act as if it is training a
                 neutral fraction history emulator.
 
         output_activation: **string / default: 'linear'**
             | Determines the output activation function for the network.
@@ -149,15 +139,15 @@
     def __init__(self, **kwargs):
 
         for key, values in kwargs.items():
             if key not in set(
                     ['batch_size', 'activation', 'epochs',
                         'lr', 'dropout', 'input_shape',
                         'output_shape', 'layer_sizes', 'base_dir',
-                        'early_stop', 'early_stop_lim', 'xHI', 'resume',
+                        'early_stop', 'xHI', 'resume',
                         'random_seed', 'output_activation',
                         'loss_function']):
                 raise KeyError("Unexpected keyword argument in nn()")
 
         self.resume = kwargs.pop('resume', False)
         self.base_dir = kwargs.pop('base_dir', 'model_dir/')
         if type(self.base_dir) is not str:
@@ -180,15 +170,14 @@
         self.drop_val = kwargs.pop('dropout', 0)
         self.input_shape = kwargs.pop('input_shape', 8)
         self.output_shape = kwargs.pop('output_shape', 1)
         self.layer_sizes = kwargs.pop(
             'layer_sizes', [self.input_shape, self.input_shape])
         if type(self.layer_sizes) is not list:
             raise TypeError("'layer_sizes' must be a list.")
-        self.early_stop_lim = kwargs.pop('early_stop_lim', 1e-4)
         self.early_stop = kwargs.pop('early_stop', False)
         self.xHI = kwargs.pop('xHI', False)
         self.random_seed = kwargs.pop('random_seed', None)
 
         boolean_kwargs = [self.resume, self.early_stop, self.xHI]
         boolean_strings = ['resume', 'early_stop', 'xHI']
         for i in range(len(boolean_kwargs)):
@@ -199,17 +188,17 @@
                       self.output_shape]
         int_strings = ['batch_size', 'epochs', 'input_shape',
                        'output_shape']
         for i in range(len(int_kwargs)):
             if type(int_kwargs[i]) is not int:
                 raise TypeError("'" + int_strings[i] + "' must be a int.")
 
-        float_kwargs = [self.lr, self.early_stop_lim, self.drop_val,
+        float_kwargs = [self.lr, self.drop_val,
                         self.random_seed]
-        float_strings = ['lr', 'early_stop_lim', 'dropout', 'random_seed']
+        float_strings = ['lr', 'dropout', 'random_seed']
         for i in range(len(float_kwargs)):
             if float_kwargs[i] is not None:
                 if type(float_kwargs[i]) not in set([float, int]):
                     raise TypeError("'" + float_strings[i] +
                                     "' must be a float.")
 
         loss_function = kwargs.pop('loss_function', None)
@@ -234,14 +223,17 @@
         train_dataset = tf.data.experimental.make_csv_dataset(
             train_dataset_fp,
             self.batch_size,
             column_names=column_names,
             label_name=label_names,
             num_epochs=1)
 
+        test_data = np.loadtxt(self.base_dir + 'test_data.txt')
+        test_labels = np.loadtxt(self.base_dir + 'test_label.txt')
+
         def pack_features_vector(features, labels):
             return tf.stack(list(features.values()), axis=1), labels
 
         train_dataset = train_dataset.map(pack_features_vector)
 
         self.output_activation = kwargs.pop('output_activation', 'linear')
         if self.xHI is True:
@@ -272,16 +264,19 @@
                 loss_value, model.trainable_variables)
 
         optimizer = keras.optimizers.Adam(learning_rate=self.lr)
 
         if self.resume is True:
             train_loss_results = list(
                 np.loadtxt(self.base_dir + 'loss_history.txt'))
+            test_loss_results = list(
+                np.loadtxt(self.base_dir + 'test_loss_history.txt'))
         else:
             train_loss_results = []
+            test_loss_results = []
         train_rmse_results = []
         num_epochs = self.epochs
         for epoch in range(num_epochs):
             s = time.time()
             epoch_loss_avg = tf.keras.metrics.Mean()
             epoch_rmse_avg = tf.keras.metrics.Mean()
 
@@ -292,28 +287,39 @@
                 epoch_loss_avg.update_state(loss_values)
                 epoch_rmse_avg.update_state(rmse)
 
             train_loss_results.append(epoch_loss_avg.result())
             train_rmse_results.append(epoch_rmse_avg.result())
             e = time.time()
 
+            test_loss, _ = loss(model, test_data, test_labels, training=False)
+            test_loss_results.append(test_loss)
+
             print(
-                'Epoch: {:03d}, Loss: {:.5f}, RMSE: {:.5f}, Time: {:.3f}'
-                .format(
-                    epoch, epoch_loss_avg.result(),
-                    epoch_rmse_avg.result(), e-s))
-
-            if self.early_stop is True:
-                if len(train_loss_results) > 10:
-                    if np.isclose(
-                            train_loss_results[-10], train_loss_results[-1],
-                            self.early_stop_lim, self.early_stop_lim):
-                        print('Early Stop')
-                        model.save(self.base_dir + 'model.h5')
+                'Epoch: {:03d}, Loss: {:.5f}, Test Loss: {:.5f},'
+                .format(epoch, epoch_loss_avg.result(), test_loss_results[-1])
+                + 'RMSE: {:.5f}, Time: {:.3f}'
+                .format(epoch_rmse_avg.result(), e-s))
+
+            if self.early_stop:
+                if len(test_loss_results) > 20:
+                    delta = 2*np.abs(test_loss_results[-21] -
+                                     test_loss_results[-1]) / \
+                                     (test_loss_results[-21] +
+                                      test_loss_results[-1])
+
+                    if delta*100 < 1e-2:
+                        print('Early Stopped: {:.5f}'.format(delta.numpy()*100)
+                              + ' < 1e-2')
+                        print('Epochs used = ' + str(len(test_loss_results)))
                         break
+
             if (epoch + 1) % 10 == 0:
                 model.save(self.base_dir + 'model.h5')
                 np.savetxt(
                     self.base_dir + 'loss_history.txt', train_loss_results)
+                np.savetxt(
+                    self.base_dir + 'test_loss_history.txt', test_loss_results)
 
         model.save(self.base_dir + 'model.h5')
         np.savetxt(self.base_dir + 'loss_history.txt', train_loss_results)
+        np.savetxt(self.base_dir + 'test_loss_history.txt', test_loss_results)
```

### Comparing `globalemu-1.5.1/globalemu/plotter.py` & `globalemu-1.6.0/globalemu/plotter.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.5.1/globalemu/preprocess.py` & `globalemu-1.6.0/globalemu/preprocess.py`

 * *Files 15% similar despite different names*

```diff
@@ -93,18 +93,22 @@
                 raise KeyError("Unexpected keyword argument in process()")
 
         self.num = num
         if type(self.num) is not int:
             if self.num != 'full':
                 raise TypeError("'num' must be an integer or 'full'.")
 
-        self.z = z
-        if type(self.z) not in set([np.ndarray, list]):
+        if type(z) not in set([np.ndarray, list]):
             raise TypeError("'z' should be a numpy array or list.")
 
+        # Convert to numpy array, and cast to float to
+        # avoid NaN errors in AFB later
+        z = np.array(z, dtype=float)
+        self.z = z
+
         self.base_dir = kwargs.pop('base_dir', 'model_dir/')
         self.data_location = kwargs.pop('data_location', 'data/')
 
         file_kwargs = [self.base_dir, self.data_location]
         file_strings = ['base_dir', 'data_location']
         for i in range(len(file_kwargs)):
             if type(file_kwargs[i]) is not str:
@@ -142,31 +146,35 @@
 
         file = open(self.base_dir + "preprocess_settings.pkl", "wb")
         pickle.dump(self.preprocess_settings, file)
         file.close()
 
         np.savetxt(self.base_dir + 'z.txt', self.z)
 
-        full_train_data = pd.read_csv(
-            self.data_location + 'train_data.txt',
-            delim_whitespace=True, header=None).values
-        full_train_labels = pd.read_csv(
-            self.data_location + 'train_labels.txt',
-            delim_whitespace=True, header=None).values
+        def load_data(file):
+            return pd.read_csv(
+                self.data_location + file,
+                delim_whitespace=True, header=None).values
+
+        full_train_data = load_data('train_data.txt')
+        full_train_labels = load_data('train_labels.txt')
+        full_test_data = load_data('test_data.txt')
+        test_labels = load_data('test_labels.txt')
 
         if self.preprocess_settings['AFB'] is True:
             np.save(
                 self.base_dir + 'AFB_norm_factor.npy',
                 full_train_labels[0, -1]*1e-3)
             res = calc_signal(self.z, self.base_dir)
 
         if self.num == 'full':
             train_data = full_train_data.copy()
             if self.preprocess_settings['AFB'] is True:
                 train_labels = full_train_labels.copy() - res.deltaT
+                test_labels -= res.deltaT
             else:
                 train_labels = full_train_labels.copy()
         else:
             ind = []
             for i in range(len(full_train_labels)):
                 index = np.random.randint(0, len(full_train_labels))
                 if index not in set(ind):
@@ -182,76 +190,123 @@
                     if self.preprocess_settings['AFB'] is True:
                         train_labels.append(full_train_labels[i] - res.deltaT)
                     else:
                         train_labels.append(full_train_labels[i])
             train_data, train_labels = np.array(train_data), \
                 np.array(train_labels)
 
-        log_td = []
+        log_train_data = []
         for i in range(train_data.shape[1]):
             if i in set(self.logs):
                 for j in range(train_data.shape[0]):
                     if train_data[j, i] == 0:
                         train_data[j, i] = 1e-6
-                log_td.append(np.log10(train_data[:, i]))
+                log_train_data.append(np.log10(train_data[:, i]))
             else:
-                log_td.append(train_data[:, i])
-        train_data = np.array(log_td).T
+                log_train_data.append(train_data[:, i])
+        train_data = np.array(log_train_data).T
+
+        log_test_data = []
+        for i in range(full_test_data.shape[1]):
+            if i in set(self.logs):
+                for j in range(full_test_data.shape[0]):
+                    if full_test_data[j, i] == 0:
+                        full_test_data[j, i] = 1e-6
+                log_test_data.append(np.log10(full_test_data[:, i]))
+            else:
+                log_test_data.append(full_test_data[:, i])
+        test_data = np.array(log_test_data).T
 
         if self.preprocess_settings['resampling'] is True:
             sampling_call = sampling(
                 self.z, self.base_dir, train_labels)
             samples = sampling_call.samples
             cdf = sampling_call.cdf
 
             resampled_labels = []
             for i in range(len(train_labels)):
                 resampled_labels.append(
                     np.interp(samples, self.z, train_labels[i]))
             train_labels = np.array(resampled_labels)
 
             norm_s = np.interp(samples, self.z, cdf)
+
+            resampled_test_labels = []
+            for i in range(len(test_labels)):
+                resampled_test_labels.append(
+                    np.interp(samples, self.z, test_labels[i]))
+            test_labels = np.array(resampled_test_labels)
         else:
             norm_s = (self.z - self.z.min())/(self.z.max() - self.z.min())
 
-        data_mins = train_data.min(axis=0)
-        data_maxs = train_data.max(axis=0)
+        train_data_mins = train_data.min(axis=0)
+        train_data_maxs = train_data.max(axis=0)
+
+        test_data_mins = test_data.min(axis=0)
+        test_data_maxs = test_data.max(axis=0)
 
         norm_train_data = []
         for i in range(train_data.shape[1]):
             norm_train_data.append(
-                (train_data[:, i] - data_mins[i])/(data_maxs[i]-data_mins[i]))
+                                   (train_data[:, i] - train_data_mins[i]) /
+                                   (train_data_maxs[i] - train_data_mins[i]))
         norm_train_data = np.array(norm_train_data).T
 
+        norm_test_data = []
+        for i in range(test_data.shape[1]):
+            norm_test_data.append(
+                                  (test_data[:, i] - test_data_mins[i]) /
+                                  (test_data_maxs[i] - test_data_mins[i]))
+        norm_test_data = np.array(norm_test_data).T
+
         if self.preprocess_settings['std_division'] is True:
             labels_stds = train_labels.std()
             norm_train_labels = [
                 train_labels[i, :]/labels_stds
                 for i in range(train_labels.shape[0])]
             norm_train_labels = np.array(norm_train_labels)
 
             norm_train_labels = norm_train_labels.flatten()
             np.save(self.base_dir + 'labels_stds.npy', labels_stds)
+
+            test_labels_stds = test_labels.std()
+            norm_test_labels = [
+                test_labels[i, :]/test_labels_stds
+                for i in range(test_labels.shape[0])]
+            norm_test_labels = np.array(norm_test_labels)
+
+            norm_test_labels = norm_test_labels.flatten()
+
         else:
             norm_train_labels = train_labels.flatten()
+            norm_test_labels = test_labels.flatten()
 
         if self.num != 'full':
             np.savetxt(self.base_dir + 'indices.txt', ind)
-        np.savetxt(self.base_dir + 'data_mins.txt', data_mins)
-        np.savetxt(self.base_dir + 'data_maxs.txt', data_maxs)
+        np.savetxt(self.base_dir + 'data_mins.txt', train_data_mins)
+        np.savetxt(self.base_dir + 'data_maxs.txt', train_data_maxs)
 
         flattened_train_data = []
         for i in range(len(norm_train_data)):
             for j in range(len(norm_s)):
                 flattened_train_data.append(
                     np.hstack([norm_train_data[i, :], norm_s[j]]))
         flattened_train_data = np.array(flattened_train_data)
 
-        train_data, train_label = flattened_train_data, norm_train_labels
-        train_dataset = np.hstack([train_data, train_label[:, np.newaxis]])
+        flattened_test_data = []
+        for i in range(len(norm_test_data)):
+            for j in range(len(norm_s)):
+                flattened_test_data.append(
+                    np.hstack([norm_test_data[i, :], norm_s[j]]))
+        flattened_test_data = np.array(flattened_test_data)
+
+        train_dataset = np.hstack([flattened_train_data,
+                                   norm_train_labels[:, np.newaxis]])
 
         np.savetxt(
             self.base_dir + 'train_dataset.csv', train_dataset, delimiter=',')
-        np.savetxt(self.base_dir + 'train_data.txt', train_data)
-        np.savetxt(self.base_dir + 'train_label.txt', train_label)
+        np.savetxt(self.base_dir + 'train_data.txt', flattened_train_data)
+        np.savetxt(self.base_dir + 'train_label.txt', norm_train_labels)
+        np.savetxt(self.base_dir + 'test_data.txt', flattened_test_data)
+        np.savetxt(self.base_dir + 'test_label.txt', norm_test_labels)
 
         print('...preprocessing done.')
```

### Comparing `globalemu-1.5.1/globalemu/resample.py` & `globalemu-1.6.0/globalemu/resample.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.5.1/globalemu.egg-info/PKG-INFO` & `globalemu-1.6.0/globalemu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: globalemu
-Version: 1.5.1
+Version: 1.6.0
 Summary: globalemu: Robust and Fast Global 21-cm Signal Emulation
 Home-page: https://github.com/htjb/globalemu
 Author: Harry T. J. Bevins
 Author-email: htjb2@cam.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
@@ -24,15 +23,15 @@
 ========================================================
 
 Introduction
 ------------
 
 :globalemu: Robust Global 21-cm Signal Emulation
 :Author: Harry Thomas Jones Bevins
-:Version: 1.5.1
+:Version: 1.6.0
 :Homepage: https://github.com/htjb/globalemu
 :Documentation: https://globalemu.readthedocs.io/
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/htjb/globalemu/master?filepath=notebooks%2F
 .. image:: https://readthedocs.org/projects/globalemu/badge/?version=latest
  :target: https://globalemu.readthedocs.io/en/latest/?badge=latest
@@ -308,9 +307,7 @@
 ------------
 
 Contributions to ``globalemu`` are very much welcome and can be made via,
 
 - Opening an issue to report a bug/propose a new feature.
 - Making a pull request. Please consider opening an issue first to discuss
   any proposals and ensure the PR will be accepted.
-
-
```

### Comparing `globalemu-1.5.1/scripts/globalemu` & `globalemu-1.6.0/scripts/globalemu`

 * *Files identical despite different names*

### Comparing `globalemu-1.5.1/setup.py` & `globalemu-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         if short:
             return f.readlines()[1].strip()
         else:
             return f.read()
 
 setup(
     name='globalemu',
-    version='1.5.1',
+    version='1.6.0',
     description='globalemu: Robust and Fast Global 21-cm Signal Emulation',
     long_description=readme(),
     author='Harry T. J. Bevins',
     author_email='htjb2@cam.ac.uk',
     url='https://github.com/htjb/globalemu',
     packages=find_packages(),
     install_requires=open('requirements.txt').read().splitlines(),
```

