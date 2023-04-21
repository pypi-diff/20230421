# Comparing `tmp/banditcoot-0.1.3.tar.gz` & `tmp/banditcoot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banditcoot-0.1.3.tar", max compression
+gzip compressed data, was "banditcoot-0.1.4.tar", max compression
```

## Comparing `banditcoot-0.1.3.tar` & `banditcoot-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      703 2023-02-23 16:53:00.767023 banditcoot-0.1.3/README.md
--rw-r--r--   0        0        0      438 2023-03-01 22:44:46.581835 banditcoot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-15 20:48:37.853671 banditcoot-0.1.3/src/banditcoot/__init__.py
--rw-r--r--   0        0        0      211 2023-02-22 22:49:31.214728 banditcoot-0.1.3/src/banditcoot/algorithms/__init__.py
--rw-r--r--   0        0        0     2626 2023-03-01 22:40:11.657588 banditcoot-0.1.3/src/banditcoot/algorithms/_epsilon_greedy.py
--rw-r--r--   0        0        0     1834 2023-02-17 01:02:09.767228 banditcoot-0.1.3/src/banditcoot/algorithms/_softmax.py
--rw-r--r--   0        0        0       68 2023-02-15 01:21:28.635213 banditcoot-0.1.3/src/banditcoot/arms/__init__.py
--rw-r--r--   0        0        0      174 2023-02-15 01:21:50.132096 banditcoot-0.1.3/src/banditcoot/arms/_bernoulli.py
--rw-r--r--   0        0        0       82 2023-02-23 16:59:26.691116 banditcoot-0.1.3/src/banditcoot/utility/__init__.py
--rw-r--r--   0        0        0     1513 2023-02-23 17:06:14.467565 banditcoot-0.1.3/src/banditcoot/utility/_batch_monte_carlo_test.py
--rw-r--r--   0        0        0     1508 2023-02-23 17:06:16.205271 banditcoot-0.1.3/src/banditcoot/utility/_monte_carlo_test.py
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 banditcoot-0.1.3/setup.py
--rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 banditcoot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      703 2023-02-24 03:42:56.784428 banditcoot-0.1.4/README.md
+-rw-r--r--   0        0        0      438 2023-04-21 02:28:59.745629 banditcoot-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-24 03:42:56.785625 banditcoot-0.1.4/src/banditcoot/__init__.py
+-rw-r--r--   0        0        0      211 2023-02-24 03:42:56.785792 banditcoot-0.1.4/src/banditcoot/algorithms/__init__.py
+-rw-r--r--   0        0        0     2744 2023-04-21 02:27:45.151164 banditcoot-0.1.4/src/banditcoot/algorithms/_epsilon_greedy.py
+-rw-r--r--   0        0        0     1834 2023-02-24 03:42:56.786032 banditcoot-0.1.4/src/banditcoot/algorithms/_softmax.py
+-rw-r--r--   0        0        0       68 2023-02-24 03:42:56.786183 banditcoot-0.1.4/src/banditcoot/arms/__init__.py
+-rw-r--r--   0        0        0      174 2023-02-24 03:42:56.786284 banditcoot-0.1.4/src/banditcoot/arms/_bernoulli.py
+-rw-r--r--   0        0        0       82 2023-02-24 03:42:56.786425 banditcoot-0.1.4/src/banditcoot/utility/__init__.py
+-rw-r--r--   0        0        0     1513 2023-02-24 03:42:56.786532 banditcoot-0.1.4/src/banditcoot/utility/_batch_monte_carlo_test.py
+-rw-r--r--   0        0        0     1508 2023-02-24 03:42:56.786644 banditcoot-0.1.4/src/banditcoot/utility/_monte_carlo_test.py
+-rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 banditcoot-0.1.4/setup.py
+-rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 banditcoot-0.1.4/PKG-INFO
```

### Comparing `banditcoot-0.1.3/README.md` & `banditcoot-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.3/src/banditcoot/algorithms/_epsilon_greedy.py` & `banditcoot-0.1.4/src/banditcoot/algorithms/_epsilon_greedy.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,20 +22,19 @@
         Number of arms
     rewards: array
         Average units of reward observed for each successful arm pull
     conv_rates: array
         Success rates for each arm
     counts: array
         number of times each arm has been pulled
-    values: array
-        average number of successes observed for each arm (i.e. conversion rate)
 
     Attributes
     ----------
-
+    values: array
+        average number of successes observed for each arm (i.e. conversion rate)
     """
     def __init__(self, epsilon, n_arms, rewards, conv_rates=None, counts=None):
         self.epsilon    = epsilon
         self.rewards    = rewards
         self.conv_rates = [0 for i in range(n_arms)] if conv_rates is None else conv_rates
         self.counts     = [0 for i in range(n_arms)] if counts is None else counts
         self.values     = [i*j for i,j in zip(conv_rates,rewards)]
@@ -57,17 +56,19 @@
         # calculate new average reward for chosen arm
         n = self.counts[chosen_arm]
         prev_value = self.values[chosen_arm]
         new_value = ((n - 1) / float(n)) * prev_value + (1 / float(n)) * success_flag * self.rewards[chosen_arm]
         self.values[chosen_arm] = new_value
         return
     
-    def batch_update(self, chosen_arm, num_times_chosen, num_successes):
+    def batch_update(self, chosen_arm, num_times_chosen, num_successes, new_rewards=None):
         # increments counts for chosen arm
         self.counts[chosen_arm] = self.counts[chosen_arm] + num_times_chosen
+        # update rewards
+        self.rewards = self.rewards if new_rewards is None else new_rewards
         # calculate new average reward for chosen arm
         n = self.counts[chosen_arm]
         prev_value = self.values[chosen_arm]
         new_value = ((n - num_times_chosen) / float(n)) * prev_value + (num_successes / float(n)) * self.rewards[chosen_arm]
         self.values[chosen_arm] = new_value
         return
```

### Comparing `banditcoot-0.1.3/src/banditcoot/algorithms/_softmax.py` & `banditcoot-0.1.4/src/banditcoot/algorithms/_softmax.py`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.3/src/banditcoot/utility/_batch_monte_carlo_test.py` & `banditcoot-0.1.4/src/banditcoot/utility/_batch_monte_carlo_test.py`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.3/src/banditcoot/utility/_monte_carlo_test.py` & `banditcoot-0.1.4/src/banditcoot/utility/_monte_carlo_test.py`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.3/setup.py` & `banditcoot-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.5.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'banditcoot',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Python module for developing and testing multi-armed bandits',
     'long_description': 'Banditcoot\n====================\n\n<img align="left" width="75" src="https://github.com/dan-kwon/banditcoot/blob/master/resources/Banditcoot.png"/> \n\n**banditcoot** is a Python module is intended for my own personal use when developing and testing multi-armed bandit algorithms. Forked from the accompanying [code repository](https://github.com/johnmyleswhite/BanditsBook) for [Bandit Algorithms for Website Optimization](https://www.oreilly.com/library/view/bandit-algorithms-for/9781449341565/).\n\n*Any use of this code is at your own risk.*\n</br>\n\n## Installation\n--------------------\nRecommended method of installation is to use pip \n```\npip install banditcoot\n```\n\n\n## Quickstart\n--------------------\n',
     'author': 'dan-kwon',
     'author_email': 'danielkwon02@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `banditcoot-0.1.3/PKG-INFO` & `banditcoot-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banditcoot
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python module for developing and testing multi-armed bandits
 License: MIT
 Author: dan-kwon
 Author-email: danielkwon02@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

