# Comparing `tmp/searchlogit-0.3.6.tar.gz` & `tmp/searchlogit-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchlogit-0.3.6.tar", last modified: Thu Apr 20 06:13:38 2023, max compression
+gzip compressed data, was "searchlogit-0.3.7.tar", last modified: Fri Apr 21 05:01:11 2023, max compression
```

## Comparing `searchlogit-0.3.6.tar` & `searchlogit-0.3.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:38.650545 searchlogit-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 06:13:28.000000 searchlogit-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-20 06:13:38.650545 searchlogit-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-20 06:13:28.000000 searchlogit-0.3.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:38.650545 searchlogit-0.3.6/searchlogit/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/_choice_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/boxcox_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    50811 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/latent_class_mixed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/mixed_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)   169496 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:38.650545 searchlogit-0.3.6/searchlogit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 06:13:38.650545 searchlogit-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-20 06:13:29.000000 searchlogit-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:38.650545 searchlogit-0.3.6/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test__choice_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test__device.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test_latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test_mixed_logit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test_multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:01:11.583451 searchlogit-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 05:01:02.000000 searchlogit-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-21 05:01:11.583451 searchlogit-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-21 05:01:02.000000 searchlogit-0.3.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:01:11.583451 searchlogit-0.3.7/searchlogit/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/_choice_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/boxcox_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50811 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/latent_class_mixed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/mixed_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169595 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:01:11.583451 searchlogit-0.3.7/searchlogit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 05:01:11.583451 searchlogit-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-21 05:01:02.000000 searchlogit-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:01:11.583451 searchlogit-0.3.7/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test__choice_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test__device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test_latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test_mixed_logit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test_multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test_search.py
```

### Comparing `searchlogit-0.3.6/LICENSE` & `searchlogit-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/PKG-INFO` & `searchlogit-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.6
+Version: 0.3.7
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.6/README.rst` & `searchlogit-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/searchlogit/_choice_model.py` & `searchlogit-0.3.7/searchlogit/_choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/searchlogit/_device.py` & `searchlogit-0.3.7/searchlogit/_device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/searchlogit/boxcox_functions.py` & `searchlogit-0.3.7/searchlogit/boxcox_functions.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/searchlogit/latent_class_mixed_model.py` & `searchlogit-0.3.7/searchlogit/latent_class_mixed_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/searchlogit/latent_class_model.py` & `searchlogit-0.3.7/searchlogit/latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/searchlogit/mixed_logit.py` & `searchlogit-0.3.7/searchlogit/mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/searchlogit/multinomial_logit.py` & `searchlogit-0.3.7/searchlogit/multinomial_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/searchlogit/search.py` & `searchlogit-0.3.7/searchlogit/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -952,15 +952,19 @@
                           init_coeff=def_vals, gtol=self.gtol,
                           weights=self.test_weight_var,
                           base_alt=self.base_alt, random_state=seed,
                           save_fitted_params=False  # speed-up computation
                           )
                 # Calculating MAE
                 # Choice frequecy obtained from estimated model applied on testing sample
-                predicted_probabilities_val = model.pred_prob * 100
+                if dev.using_gpu:
+                    pred_prob = dev.to_cpu(model.pred_prob)
+                else:
+                    pred_prob = model.pred_prob
+                predicted_probabilities_val = pred_prob * 100
                 obs_freq = model.obs_prob * 100
 
                 MAE = round((1/len(self.choice_set))*(np.sum(abs(predicted_probabilities_val -
                                                         obs_freq))), 2)
                 logger.info(f"MAE: {MAE}")
                 logger.info(f"Out of sample log-likelihood: {model.loglikelihood}")
                 if self.multi_objective_variable == "MAE":
@@ -1187,15 +1191,14 @@
 
         model = LatentClassMixedModel()
         if self.num_classes is None:
             optimal_num, model = model.fit(X,
                                            y,
                                            varnames=all_vars,
                                            alts=self.alt_var,
-                                           isvars=is_vars,
                                            ids=self.choice_id,
                                            panels=self.ind_id,
                                            randvars=rand_vars,
                                            n_draws=self.n_draws,
                                            correlation=corvars,
                                            transformation="boxcox",
                                            transvars=bcvars,
```

### Comparing `searchlogit-0.3.6/searchlogit.egg-info/PKG-INFO` & `searchlogit-0.3.7/searchlogit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.6
+Version: 0.3.7
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.6/searchlogit.egg-info/SOURCES.txt` & `searchlogit-0.3.7/searchlogit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/setup.py` & `searchlogit-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 
 with codecs.open("README.rst", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='searchlogit',
-                 version='0.3.6',
+                 version='0.3.7',
                  description='Extensions for a Python package for \
                               GPU-accelerated estimation of mixed logit models.',
                  long_description=long_description,
                  long_description_content_type="text/x-rst",
                  url='https://github.com/RyanJafefKelly/searchlogit',
                  author='Ryan Kelly, Prithvi Beeramoole and Alexander Paz',
                  author_email='ryan@kiiii.com',
```

### Comparing `searchlogit-0.3.6/tests/test__choice_model.py` & `searchlogit-0.3.7/tests/test__choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/tests/test__device.py` & `searchlogit-0.3.7/tests/test__device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/tests/test_latent_class_model.py` & `searchlogit-0.3.7/tests/test_latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/tests/test_mixed_logit.py` & `searchlogit-0.3.7/tests/test_mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.6/tests/test_multinomial_logit.py` & `searchlogit-0.3.7/tests/test_multinomial_logit.py`

 * *Files identical despite different names*

