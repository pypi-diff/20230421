# Comparing `tmp/nunchaku-0.8.0.tar.gz` & `tmp/nunchaku-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nunchaku-0.8.0.tar", max compression
+gzip compressed data, was "nunchaku-0.9.0.tar", max compression
```

## Comparing `nunchaku-0.8.0.tar` & `nunchaku-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-02-27 18:23:46.573059 nunchaku-0.8.0/nunchaku/__init__.py
--rw-r--r--   0        0        0     2177 2023-02-27 18:23:46.573059 nunchaku-0.8.0/nunchaku/_example_data.py
--rw-r--r--   0        0        0     4321 2023-02-27 18:23:46.576393 nunchaku-0.8.0/nunchaku/_models.py
--rw-r--r--   0        0        0    10721 2023-02-27 18:23:46.576393 nunchaku-0.8.0/nunchaku/gibbs_sampler.py
--rw-r--r--   0        0        0    22244 2023-02-27 18:23:46.576393 nunchaku-0.8.0/nunchaku/nunchaku.py
--rw-r--r--   0        0        0     1055 2023-02-27 18:28:02.523077 nunchaku-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1384 2023-02-27 18:23:46.579726 nunchaku-0.8.0/readme.md
--rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 nunchaku-0.8.0/setup.py
--rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 nunchaku-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-27 18:23:46.573059 nunchaku-0.9.0/nunchaku/__init__.py
+-rw-r--r--   0        0        0     2177 2023-02-27 18:23:46.573059 nunchaku-0.9.0/nunchaku/_example_data.py
+-rw-r--r--   0        0        0     2001 2023-04-10 17:29:58.943666 nunchaku-0.9.0/nunchaku/_models.py
+-rw-r--r--   0        0        0    10865 2023-04-10 17:29:58.943666 nunchaku-0.9.0/nunchaku/gibbs_sampler.py
+-rw-r--r--   0        0        0    35860 2023-04-10 17:29:58.947000 nunchaku-0.9.0/nunchaku/nunchaku.py
+-rw-r--r--   0        0        0     1077 2023-04-10 17:29:58.947000 nunchaku-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1475 2023-04-10 17:29:58.947000 nunchaku-0.9.0/readme.md
+-rw-r--r--   0        0        0     2275 1970-01-01 00:00:00.000000 nunchaku-0.9.0/setup.py
+-rw-r--r--   0        0        0     2579 1970-01-01 00:00:00.000000 nunchaku-0.9.0/PKG-INFO
```

### Comparing `nunchaku-0.8.0/nunchaku/_example_data.py` & `nunchaku-0.9.0/nunchaku/_example_data.py`

 * *Files identical despite different names*

### Comparing `nunchaku-0.8.0/nunchaku/gibbs_sampler.py` & `nunchaku-0.9.0/nunchaku/gibbs_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-class gibbs_sampler:
-    def __init__(self):
-        pass
+import numpy as np
+import matplotlib.pyplot as plt
+from logging import warning
+
+class GibbsSampler:
+    def __init__(self, nc):
+        self.nc = nc
 
-    def gibbs_sampler(
+    def sample(
         self,
         num_regions=3,
         initial_points="default",
         num_steps=20000,
         random_attempts=10,
         random_steps=2000,
         return_samples=False,
@@ -63,24 +67,24 @@
             if the initial guess input by user is not valid
 
         """
         # handle user input
         if initial_points is None:
             pass
         elif initial_points == "default":
-            initial_start_points = np.arange(num_regions, dtype=int) * self.minlen
-            initial_end_points = initial_start_points + self.minlen - 1
+            initial_start_points = np.arange(num_regions, dtype=int) * self.nc.minlen
+            initial_end_points = initial_start_points + self.nc.minlen - 1
             initial_points = list(
                 np.stack([initial_start_points, initial_end_points]).flatten(order="F")
             )
         elif initial_points == "reverse":
-            initial_start_points = np.arange(num_regions, dtype=int) * self.minlen
-            initial_end_points = initial_start_points + self.minlen - 1
+            initial_start_points = np.arange(num_regions, dtype=int) * self.nc.minlen
+            initial_end_points = initial_start_points + self.nc.minlen - 1
             initial_points = sorted(
-                len(self.x)
+                len(self.nc.x)
                 - np.stack([initial_start_points, initial_end_points]).flatten(
                     order="F"
                 )
                 - 1
             )
         elif len(initial_points) == num_regions * 2:
             initial_points = [int(x) for x in initial_points]
@@ -116,15 +120,15 @@
             plt.figure()
             plt.hist(evi_for_plot)
             plt.ylabel("counts")
             plt.xlabel("log evidence")
             plt.show()
         if plot_traces:
             self.plot_gibbs_traces(samples_max, show=True)
-        if check and self.logpmc:
+        if check and self.nc.logpmc:
             self._gibbs_checker(boundaries_max, check)
         if not return_samples:
             return boundaries_max
         else:
             return boundaries_max, samples_max
 
 
@@ -153,16 +157,16 @@
 
 
     ### Internal functions for gibbs sampling
     ###
 
     def _get_argmax_for_two(self):
         """find argmax of posterior for two linear regions."""
-        res = self.evidence.copy()
-        start, end, minlen = (self.start, self.end, self.minlen)
+        res = self.nc.evidence.copy()
+        start, end, minlen = (self.nc.start, self.nc.end, self.nc.minlen)
         results = np.empty(res.shape)
         results.fill(-np.inf)
         for st in range(start, end - minlen + 1):
             for ed in range(st + minlen, end + 1):
                 res_temp = res.copy()
                 res_temp[:ed, st:] = -np.inf
                 results[st, ed - 1] = np.nanmax(res_temp)
@@ -183,17 +187,17 @@
                     x_pre = list(samples[i - 1, j + 1 :])
                 samples[i, j] = self._conditional_sampler(x_post, x_pre)
         return samples
 
     def _conditional_sampler(self, x_post, x_pre):
         """construct the conditional distribution for the Gibbs sampler."""
         all_matrix, minlen, datalen = (
-            self.evidence,
-            self.minlen,
-            len(self.x),
+            self.nc.evidence,
+            self.nc.minlen,
+            len(self.nc.x),
         )
         # find x_j
         index = len(x_post)
         if index == 0:
             x_post = [-1]
         if len(x_pre) == 0:
             x_pre = [datalen]
@@ -216,24 +220,24 @@
         # normalise to one
         conditional = conditional / np.sum(conditional)
         # generate a sample
         return int(np.random.choice(np.arange(xmin, xmax + 1), p=conditional))
 
     def _gibbs_generate_initial_guess(self, number):
         """generate a random initial guess for the Gibbs sampler."""
-        mu, N = (self.minlen, len(self.x))
+        mu, N = (self.nc.minlen, len(self.nc.x))
         res = [-1]
         for j in range(number, 0, -1):
             res.append(np.random.choice(range(res[-1] + 1, N - j * mu + 1)))
             res.append(np.random.choice(range(res[-1] + mu - 1, N - (j - 1) * mu)))
         return res[1:]
 
     def _gibbs_get_evidence(self, boundaries):
         """return the evidence of regions within the boundaries."""
-        all_matrix = self.evidence
+        all_matrix = self.nc.evidence
         evi = 0
         coo = boundaries.copy()
         coo = coo[::-1]
         while len(coo) > 0:
             start = coo.pop()
             end = coo.pop()
             evi += all_matrix[start, end]
@@ -248,30 +252,30 @@
         for j in range(len(boundaries) - 1):
             boundaries_temp = boundaries.copy()
             del boundaries_temp[j : j + 2]
             evi = self._gibbs_get_evidence(boundaries_temp)
             if evi > evi_max:
                 evi_max = evi
                 boundaries_max = boundaries_temp
-        evi_short = evi_max + self._mc_logprior(len(boundaries_max))
-        evi_long = evi0 + self.logpmc + self._mc_logprior(len(boundaries))
+        evi_short = evi_max + self.nc._mc_logprior(len(boundaries_max))
+        evi_long = evi0 + self.nc.logpmc + self.nc._mc_logprior(len(boundaries))
         log10_bayes_factor = (evi_long - evi_short) / np.log(10)
         if log10_bayes_factor < check:
             warning(
                 f""" The bayes factor may favour smaller number of regions: {boundaries_max};
                 log10 bayes factor ({num_regions} regions over {num_regions - 1}): {log10_bayes_factor}.
                 or the Gibbs sampler is trapped by a local maximum or does not converge."""
             )
         else:
             print(f"Model check passed: log10 bayes factor {log10_bayes_factor}.")
         return None
 
     def _mc_judge(self, boundaries):
         """judge whether the given boundaries are valid."""
-        minlen = self.minlen
+        minlen = self.nc.minlen
         coo = boundaries.copy()
         coo = coo[::-1]
         while len(coo) > 0:
             start = coo.pop()
             end = coo.pop()
             if end - start < minlen - 1:
                 return False
```

### Comparing `nunchaku-0.8.0/nunchaku/nunchaku.py` & `nunchaku-0.9.0/nunchaku/nunchaku.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,238 +1,289 @@
-from ._models import mc, mc_t, mc_entropy
+from ._models import mc, mc_t
 import numpy as np
-from scipy.optimize import minimize
 from scipy.stats import linregress
 import matplotlib.pyplot as plt
 from logging import warning
 from ._example_data import return_data
 import pandas as pd
+from itertools import product
+from tqdm.auto import tqdm
+from scipy.special import loggamma
+from scipy.integrate import quad
 
 
 class Nunchaku:
     """Find how many linear regions a dataset should be divide into,
     and find the start and end of each linear region.
 
     Parameters
     ----------
     X : list of floats or 1-D numpy array
-        the x vector of data.
+        the x vector of data, sorted ascendingly.
     Y : array-like
         the y vector or matrix of data, each row being one replicate of
         measurement.
-    prior : list of length 2 or 4
+    err : list of floats or 1-D numpy array, optional
+        the error of the input data.
+    yrange : list of length 2, optional
+        the min and max of y allowed by the instrument's readout.
+    prior : list of length 2 or 4, optional
         the prior range of the slope (and the intercept when length is 4).
-    std : list of floats or 1-D numpy array, optional # error?
-        the standard deviation of the input data.
-    start : int, default 0
-        the min index of x that a valid region allows.
-    end : int, optional
-        the max index of x that a valid region allows (inclusive).
-    estimate_std : bool, optional
-        if True, estimate std from data; default True when Y has >= 3
+        This argument will overwrite `yrange`.
+    estimate_err : bool, optional
+        if True, estimate error from data; default True when Y has >= 3
         replicates.
     minlen : int, default 3
         the minimal length of a valid region (must be >= 3).
-    attempt : int, default 20
-        the max number of attempts to run the BFGS minimize routine when the std
-        is neither provided nor estimated.
 
     Raises
     ------
     ValueError
-        when Y has multiple replicates and std is provided.
+        when Y has multiple replicates and err is provided.
+
+    ValueError
+        when the length of `prior` is not 2 or 4, if provided.
 
     Examples
     --------
     >>> from nunchaku.nunchaku import nunchaku, get_example_data
     >>> x, y = get_example_data()
     >>> nc = nunchaku(x, y, prior=[-5,5]) # load data and set prior of slope
-    >>> # compare models with one, two or three linear regions
-    >>> num_regions, evidences = nc.get_number([1,2,3])
+    >>> # compare models with 1, 2, 3 and 4 linear regions
+    >>> num_regions, evidences = nc.get_number(max_num=4)
     >>> # get the mean and standard deviation of the boundary points
-    >>> bds, bds_std = nc.get_iboundaries(num_regions)
-    >>> info_df = nc.get_info()
+    >>> bds, bds_err = nc.get_iboundaries(num_regions)
+    >>> # get the information of all regions
+    >>> info_df = nc.get_info(bds)
+    >>> # plot the data and the regions
     >>> nc.plot(info_df)
 
     """
 
     def __init__(
         self,
         X,
         Y,
-        prior,
-        std=None,
-        start=0,
-        end=None,
-        estimate_std="default",
+        err=None,
+        yrange=None,
+        prior=None,
+        estimate_err="default",
         minlen=3,
-        attempt=20,
     ):
         # Load settings
         self.X = np.asarray(X)
         self.Y = np.asarray(Y)
-        if isinstance(std, (list, np.ndarray)):
-            self.std = np.asarray(std)
-        else:
-            self.std = None
-        self.start = start
-        if end:
-            self.end = end
+        if isinstance(err, (list, np.ndarray)):
+            self.err = np.asarray(err)
         else:
-            self.end = self.X.shape[0]
+            self.err = None
+        self.start = 0
+        self.end = self.X.shape[0]
         if minlen >= 3:
             self.minlen = minlen
         else:
             warning("Nunchaku: minlen must be >= 3. Reset to 3.")
             self.minlen = 3
-        self.attempt = attempt
-        # handle estimate_std
-        if estimate_std == "default":
-            # if Y has 3 replicates and std is none
-            if (self.Y.ndim > 1) and (self.Y.shape[0] >= 3) and (self.std is None):
-                estimate_std = True
-            else:
-                estimate_std = False
-        # if std is provided, do not estimate_std (overwrite user's setting)
-        if self.std is not None:
-            estimate_std = False
-        # if std is not provided but Y is 1-D, impossible to estimate_std
+        # handle estimate_err
+        if estimate_err == "default":
+            # if Y has 3 replicates and err is none
+            if (self.Y.ndim > 1) and (self.Y.shape[0] >= 3) and (self.err is None):
+                estimate_err = True
+            else:
+                estimate_err = False
+        # if err is provided, do not estimate_err (overwrite user's setting)
+        if self.err is not None:
+            estimate_err = False
+        # if err is not provided but Y is 1-D, impossible to estimate_err
         elif self.Y.ndim == 1:
-            estimate_std = False
-        # if std is provided but Y is 2-D, throw error
-        if self.std is not None and self.Y.ndim > 1:
-            raise ValueError("When std is provided, Y should be 1-D.")
-        # now estimate std
-        self.estimate_std = estimate_std
-        if estimate_std:
+            estimate_err = False
+        # if err is provided but Y is 2-D, throw error
+        if self.err is not None and self.Y.ndim > 1:
+            raise ValueError("When err is provided, Y should be 1-D.")
+        # now estimate err
+        self.estimate_err = estimate_err
+        if estimate_err:
             # x, y, instead of X, Y, are what the methods actually use
             self.x = self.X
             self.y = self.Y.mean(axis=0)
-            # OK to write std because estimate_std is True only when std is None
-            self.std = self.Y.std(axis=0)
+            # OK to write err because estimate_err is True only when err is None
+            self.err = self.Y.std(axis=0)
         else:
             self.x = self.X
             self.y = self.Y
-        # handle estimated std=0 when replicates have the same value by chance
-        if self.std is not None:
-            self.std[self.std == 0] = self.std[self.std > 0].mean()
+            if self.Y.ndim == 1:
+                self.nreplicates = 1
+            else:
+                self.nreplicates = self.Y.shape[0]
+        # handle estimated err=0 when replicates have the same value by chance
+        if self.err is not None:
+            self.err[self.err == 0] = self.err[self.err > 0].mean()
         # prior
         if prior:
             if len(prior) == 2:
-                prior.append(-self.x[-1] * prior[1])
-                prior.append(-self.x[-1] * prior[0])
+                prior.append(min(-self.x[-1] * prior[1], self.x[0] * prior[0]))
+                prior.append(max(-self.x[-1] * prior[0], self.x[0] * prior[1]))
             elif len(prior) != 4:
                 raise ValueError(f"len(prior) should be 2 or 4, not {prior}.")
             self.prior = prior
-            self.logpmc = -np.log((prior[1] - prior[0]) * (prior[3] - prior[2]))
         else:
-            self.logpmc = None
+            if yrange:
+                m_max = (yrange[1] - yrange[0]) / np.min(np.diff(self.x))
+            else:
+                warning(
+                    """Nunchaku: neither the prior of slope and intercept nor the range of y is given.
+                Using the min and max of y as the range of y to estimate of prior.
+                """
+                )
+                m_max = (np.max(self.y) - np.min(self.y)) / np.min(np.diff(self.x))
+            c_max = max(m_max * self.x[-1], m_max * self.x[0])
+            prior = [-m_max, m_max, -c_max, c_max]
+            self.prior = prior
+        self.logpmc = -np.log((prior[1] - prior[0]) * (prior[3] - prior[2]))
         # results
-        self.evidence = self._cal_evidence()
+        if self.err is not None:
+            self.evidence = self._cal_evidence()
+        else:
+            self.U, self.D, self.L = self._cal_evidence()
+        self.logZ = dict()
+        self.large = False
 
     def _cal_evidence(self):
         """Calculate evidence for each possible region between start and end."""
-        X, Y, std, start, end, minlen = (
+        X, Y, err, start, end, minlen = (
             self.x,
             self.y,
-            self.std,
+            self.err,
             self.start,
             self.end,
             self.minlen,
         )
         # Matrix to record results
-        results = np.ones((len(X), len(X))) * np.nan
-        results.fill(np.nan)
-        if self.std is None:
-            init_guess = self._get_init_guess()
-            funcs = mc_t()
-        else:
-            logL = mc()
         # calculate evidence
-        if self.std is None:
-            warning("Nunchaku: Std is not estimated or provided. It could be slow.")
-            for st in range(start, end - minlen + 1):
+        if self.err is None:
+            results_U = np.ones((len(X), len(X)), dtype=np.longdouble) * np.nan
+            results_D = np.ones((len(X), len(X)), dtype=np.longdouble) * np.nan
+            results_L = np.ones((len(X), len(X)), dtype=np.longdouble) * np.nan
+            U, D = mc_t()
+            for st in tqdm(
+                range(start, end - minlen + 1), desc="getting evidence matrix"
+            ):
                 for ed in range(st + minlen, end + 1):  # confirm?
                     # Run calculation and update init_guess
-                    init_guess, evi = self._cal_evidence_unknown_s(
-                        st, ed, init_guess, funcs
-                    )
-                    if evi is None:
-                        continue
-                    else:
-                        results[st, ed - 1] = evi
+                    evi_u = self._cal_evidence_unknown_err(st, ed, U)
+                    results_U[st, ed - 1] = evi_u
+                    evi_d = self._cal_evidence_unknown_err(st, ed, D)
+                    results_D[st, ed - 1] = evi_d
+                    results_L[st, ed - 1] = (ed - st) * self.nreplicates
+            return results_U, results_D, results_L
         else:
+            results = np.ones((len(X), len(X))) * np.nan
+            logL = mc()
             for st in range(start, end - minlen + 1):
                 for ed in range(st + minlen, end + 1):  # confirm?
-                    evi = logL(X[st:ed], Y[st:ed], std[st:ed], ed - st)
+                    evi = logL(X[st:ed], Y[st:ed], err[st:ed], ed - st)
                     # unknown bug in either builtin sum or numpy sum
                     if evi > 9e8:
                         evi = -np.inf
                     results[st, ed - 1] = evi  # must be (end - 1)?
-        # Normalise to start:end
-        # self.norm_factor = results[start, end - 1]
-        # results = results - results[start, end - 1]
-        return results
+            return results
 
-    def get_number(self, num_regions):
+    def get_number(self, max_num):
         """Get the most likely number of linear regions.
 
         Parameters
         ----------
-        num_regions : list of int
-            number of linear regions
+        max_num : list of int
+            maximum number of linear regions
+
+        Raises
+        ------
+        OverflowError
+            when numerical integration yields infinity.
 
         """
-        res = self.evidence.copy()
-        res = res.astype(np.longdouble)
-        # normalise to avoid overflow
-        log_norm_factor = np.nanmax(res)
-        res = np.exp(res - np.nanmax(res))
-        res[np.isnan(res)] = 0
         evi = []
-        for M in num_regions:
-            with np.errstate(divide="ignore", invalid="ignore"):
-                evi_M = (
-                    np.log(self._findZ(res, M))
-                    + self._mc_logprior(M)
-                    + self.logpmc * M
-                    + log_norm_factor * M
-                ) / np.log(10)
-            evi.append(evi_M)
+        if self.err is not None:
+            res = self.evidence.copy()
+            res = res.astype(np.longdouble)
+            # normalise to avoid overflow
+            log_norm_factor = np.nanmax(res)
+            res = np.exp(res - np.nanmax(res))
+            res[np.isnan(res)] = 0
+            for M in range(1, max_num + 1):
+                with np.errstate(divide="ignore", invalid="ignore"):
+                    evi_M = (
+                        np.log(self._findZ(res, M))
+                        + self._mc_logprior(M)
+                        + self.logpmc * M
+                        + log_norm_factor * M
+                    ) / np.log(10)
+                evi.append(evi_M)
+        else:
+            for M in tqdm(range(1, max_num + 1), desc="getting model evidence"):
+                with np.errstate(divide="ignore", invalid="ignore"):
+                    if M > 3:
+                        logZ = self._findZ_unknown_err_numerical(M)
+                        self.logZ[M] = logZ  # store Z for finding iboundaries
+                        log_evi = logZ + (
+                            -len(self.x) * self.nreplicates / 2 + M
+                        ) * np.log(2 * np.pi)
+                    else:  # use analytical sum where possible
+                        logZ = self._findZ_unknown_err_analytical(M)
+                        self.logZ[M] = logZ
+                        log_evi = (
+                            logZ
+                            + loggamma((len(self.x) * self.nreplicates - 1) / 2 - M)
+                            + (-len(self.x) * self.nreplicates / 2 + M)
+                            * np.log(2 * np.pi)
+                        )
+                    evi_M = (
+                        +log_evi + self._mc_logprior(M) + self.logpmc * M
+                    ) / np.log(10)
+                evi.append(evi_M)
+            # check
+            if len(evi) > 3:
+                if not (np.any(np.isfinite(np.array(evi[3:])))):
+                    warning(f"Nunchaku: the evidence may be numerically too small.")
+            elif not np.any(np.isfinite(np.array(evi))):
+                warning(f"Nunchaku: the evidence may be numerically too small.")
         ind = np.nanargmax(evi)
-        best_num_regions = num_regions[ind]
+        best_num_regions = ind + 1
+        # check
+        if best_num_regions == max_num:
+            warning(
+                "Nunchaku: the best number of regions equals the largest candidate."
+            )
         return best_num_regions, evi
 
     def get_info(self, boundaries):
         """Return a Pandas dataframe that describes the regions within given internal boundaries,
         i.e. excluding the first (0) and last (`len(x)`) indices of the data.
 
         Parameters
         ----------
         boundaries : list of int
             a list of indices of boundary points
 
         """
-        all_matrix, x, y = (self.evidence, self.x, self.y)
+        # quick check to make sure boundaries are sensible
+        x, y = (self.x, self.y)
         keys = [
             "start",
             "end",
-            "evidence",
             "slope",
             "intercept",
             "rsquare",
             "x range",
             "y range",
-            "entropy",
         ]
         d = {k: [] for k in keys}
         d["start"] = [0] + list(map(lambda x: x + 1, boundaries))
         d["end"] = boundaries + [len(self.x) - 1]
         for st, ed in zip(d["start"], d["end"]):
-            d["evidence"].append(all_matrix[st, ed])
             if y.ndim > 1:
                 # flatten for regression
                 x_flat = np.append([], [x[st : ed + 1]] * y.shape[0])
                 y_flat = y[:, st : ed + 1].flatten(order="C")
                 y_mn = y[:, st : ed + 1].mean(axis=0)
             else:
                 x_flat = x[st : ed + 1]
@@ -240,129 +291,222 @@
                 y_mn = y[st : ed + 1]
             d["x range"].append((x_flat[0], x_flat[-1]))
             d["y range"].append((y_mn[0], y_mn[-1]))
             lin_res = linregress(x_flat, y_flat)
             d["slope"].append(lin_res.slope)
             d["intercept"].append(lin_res.intercept)
             d["rsquare"].append(lin_res.rvalue**2)
-            if self.std is not None:
-                d["entropy"].append(self._get_entropy(st, ed))  # no need to ed+1
-            else:
-                d["entropy"].append(np.nan)
         return pd.DataFrame(d)
 
-    def get_iboundaries(self, num_regions, round=True):
+    def get_iboundaries(self, num_regions, round=True, bd_err=True):
         """Return the mean and standard deviation of the internal boundary indices,
         i.e. excluding the first (0) and last (`len(x)`) indices of the data.
 
         Parameters
         ----------
         num_regions : int
             number of linear regions
-        round : bool
+        round : bool, default True
             whether to round the returned mean to integer
+        bd_err : bool, default True
+            whether to estimate the error of the boundary positions. If False,
+            it takes shorter to get the internal boundaries.
+
+        Raises
+        ------
+        OverflowError
+            when numerical integration yields infinity.
 
         """
-        res = self.evidence.copy()
-        res = res.astype(np.longdouble)
-        # normalise to avod overflow
-        # log_norm_factor = np.nanmax(res)
-        res = np.exp(res - np.nanmax(res))
-        res[np.isnan(res)] = 0
-        Z = self._findZ(res, num_regions)
         boundaries = []
-        boundaries_std = []
-        for j in range(1, num_regions):
-            coo = self._find_moment(res, num_regions, j) / Z
-            boundaries.append(coo)
-            coo2 = self._find_moment(res, num_regions, j, moment=2) / Z
-            boundaries_std.append(np.sqrt(coo2 - coo**2))
+        boundaries_err = []
+        if self.err is not None:
+            res = self.evidence.copy()
+            res = res.astype(np.longdouble)
+            # normalise to avod overflow
+            # log_norm_factor = np.nanmax(res)
+            res = np.exp(res - np.nanmax(res))
+            res[np.isnan(res)] = 0
+            Z = self._findZ(res, num_regions)
+            for j in range(1, num_regions):
+                coo = self._find_moment(res, num_regions, j) / Z
+                boundaries.append(coo)
+                coo2 = self._find_moment(res, num_regions, j, moment=2) / Z
+                boundaries_err.append(np.sqrt(coo2 - coo**2))
+        else:
+            if num_regions > 3:
+                for j in tqdm(
+                    range(1, num_regions),
+                    desc="getting internal boundaries",
+                ):
+                    coo = np.exp(
+                        self._find_moment_unknown_err_numerical(num_regions, j)
+                        - self.logZ[num_regions],
+                        dtype=np.longdouble,
+                    )
+                    # quick check
+                    if coo >= self.minlen and coo < len(self.x):
+                        pass
+                    else:
+                        warning(
+                            "Nunchaku: numerical integration is probably inaccurate."
+                        )
+                    boundaries.append(coo)
+                    if bd_err:
+                        coo2 = np.exp(
+                            self._find_moment_unknown_err_numerical(
+                                num_regions, j, moment=2
+                            )
+                            - self.logZ[num_regions],
+                            dtype=np.longdouble,
+                        )
+                        boundaries_err.append(np.sqrt(coo2 - coo**2))
+            else:
+                for j in tqdm(
+                    range(1, num_regions),
+                    desc="getting internal boundaries",
+                ):
+                    coo = np.exp(
+                        self._find_moment_unknown_err_analytical(num_regions, j)
+                        - self.logZ[num_regions],
+                        dtype=np.longdouble,
+                    )
+                    boundaries.append(coo)
+                    if bd_err:
+                        coo2 = np.exp(
+                            self._find_moment_unknown_err_analytical(
+                                num_regions, j, moment=2
+                            )
+                            - self.logZ[num_regions],
+                            dtype=np.longdouble,
+                        )
+                        boundaries_err.append(np.sqrt(coo2 - coo**2))
+
         if round:
-            return list(np.array(boundaries).astype(int)), boundaries_std
+            return list(np.array(boundaries).astype(int)), boundaries_err
         else:
-            return boundaries, boundaries_std
+            return boundaries, boundaries_err
 
     def plot(
         self,
         info_df=None,
         show=False,
         figsize=(6, 5),
-        std_width=1,
+        err_width=1,
         s=10,
         color="red",
         alpha=0.5,
+        hlmax={"rsquare": ("orange", "s")},
+        hlmin=None,
         **kwargs,
     ):
         """Plot the raw data and the boundary points.
 
         Parameters
         ----------
         info_df : pandas dataframe, default None
             the pandas dataframe returned by `get_info()`; if None, only the data is shown.
-        show : bool
+        show : bool, default False
             if True, call `plt.show()`
-        figsize : tuple
+        figsize : tuple, default (6, 5)
             size of figure passed to `plt.subplots()`
-        std_width : float
-            the width of the error bar is this parameter times std times 2 (both
+        err_width : float, default 1
+            the width of the error bar is this parameter times err times 2 (both
             sides)
-        s : float
+        s : float, default 10
             size of the boundary points as passed into `plt.scatter()`
-        color : str
+        color : str, default "red"
             color of the boundary points as passed into `plt.scatter()`
-        alpha : float
+        alpha : float, default 0.5
             transparency of the boundary points as passed into `plt.scatter()`
+        hlmax : dict, default {"rsquare": ("orange", "s")}
+            highlighting the segment with max quantity (e.g. rsquare).
+            The key is the column name in `info_df` and the value is a tuple: (color, marker).
+        hlmin : dict, optional
+            highlighting the segment with min quantity (e.g. rsquare).
+            The key is the column name in `info_df` and the value is a tuple: (color, marker).
         **kwargs : keyword arguments
             as passed into `plt.plot()`
 
-        Examples
-        --------
-        `plot()` returns both the figure and axes, enabling users to customise them
-
-        >>> from nunchaku.nunchaku import nunchaku
-        >>> nc = nunchaku(x, y)
-        >>> bds, _ = nc.get_iboundaries(3)
-        >>> info_df = nc.get_info(bds)
-        >>> fig, ax = nc.plot(info_df)
-
         """
 
         if self.y.ndim > 1:
             y = self.y.mean(axis=0)
-            std = None
+            err = None
         else:
             y = self.y
-            std = self.std
+            err = self.err
         fig, ax = plt.subplots(figsize=figsize)
         ax.plot(self.x, y, color="blue")
-        if std is not None:
+        if err is not None:
             ax.fill_between(
                 self.x,
-                y - std_width * std,
-                y + std_width * std,
+                y - err_width * err,
+                y + err_width * err,
                 alpha=0.1,
                 color="blue",
             )
+
         if info_df is not None:
+            # handle how to highlight segments
+            if hlmax is not None:
+                idx_ignore_max = [info_df[k].idxmax() for k in hlmax.keys()]
+                idx_color_max = [v[0] for v in hlmax.values()]
+                idx_marker_max = [v[1] for v in hlmax.values()]
+            else:
+                idx_ignore_max = []
+                idx_color_max = []
+                idx_marker_max = []
+
+            if hlmin is not None:
+                idx_ignore_min = [info_df[k].idxmin() for k in hlmin.keys()]
+                idx_color_min = [v[0] for v in hlmin.values()]
+                idx_marker_min = [v[1] for v in hlmin.values()]
+            else:
+                idx_ignore_min = []
+                idx_color_min = []
+                idx_marker_min = []
+
+            idx_ignore = idx_ignore_max + idx_ignore_min
+            idx_color = idx_color_max + idx_color_min
+            idx_marker = idx_marker_max + idx_marker_min
+
             for j in range(info_df.shape[0]):
-                bd_start = info_df.loc[j, "start"]
-                bd_end = info_df.loc[j, "end"]
-                slope = info_df.loc[j, "slope"]
-                intercept = info_df.loc[j, "intercept"]
-                y_start = slope * self.x[bd_start] + intercept
-                y_end = slope * self.x[bd_end] + intercept
-                ax.plot(
-                    [self.x[bd_start], self.x[bd_end]],
-                    [y_start, y_end],
-                    color=color,
-                    alpha=alpha,
-                    marker="o",
-                    markersize=s,
-                    **kwargs,
-                )
+                if j not in idx_ignore:
+                    bd_start = info_df.loc[j, "start"]
+                    bd_end = info_df.loc[j, "end"]
+                    slope = info_df.loc[j, "slope"]
+                    intercept = info_df.loc[j, "intercept"]
+                    y_start = slope * self.x[bd_start] + intercept
+                    y_end = slope * self.x[bd_end] + intercept
+                    ax.plot(
+                        [self.x[bd_start], self.x[bd_end]],
+                        [y_start, y_end],
+                        color=color,
+                        alpha=alpha,
+                        marker="o",
+                        markersize=s,
+                        **kwargs,
+                    )
+        for idx, cl, mk in zip(idx_ignore, idx_color, idx_marker):
+            bd_start = info_df.loc[idx, "start"]
+            bd_end = info_df.loc[idx, "end"]
+            slope = info_df.loc[idx, "slope"]
+            intercept = info_df.loc[idx, "intercept"]
+            y_start = slope * self.x[bd_start] + intercept
+            y_end = slope * self.x[bd_end] + intercept
+            ax.plot(
+                [self.x[bd_start], self.x[bd_end]],
+                [y_start, y_end],
+                color=cl,
+                alpha=alpha,
+                marker=mk,
+                markersize=s,
+                **kwargs,
+            )
         ax.set_xlabel("x")
         ax.set_ylabel("y")
         if show:
             plt.show()
         return fig, ax
 
     def plot_matrix(self, show=False, figsize=(6, 5), **kwargs):
@@ -386,15 +530,20 @@
 
         >>> from nunchaku.nunchaku import nunchaku
         >>> nc = nunchaku(x, y)
         >>> fig, ax = nc.plot_matrix()
         >>> ax.set_ylim(200,)
 
         """
-        res = self.evidence
+        if self.err is not None:
+            res = self.evidence
+        else:
+            raise NotImplementedError(
+                "This method is only available if error is estimated or provided."
+            )
         fig = plt.figure(constrained_layout=True, figsize=figsize)
         # create three axes
         gs = fig.add_gridspec(
             2,
             2,
             width_ratios=(4, 1),
             height_ratios=(1, 4),
@@ -416,129 +565,45 @@
         ax_mgy.plot(mgy, range(len(mgy)))
         ax_mgy.yaxis.set_tick_params(labelleft=False)
         axes = [ax, ax_mgx, ax_mgy]
         if show:
             plt.show()
         return fig, axes
 
-    ### Internal functions for single region
-    ###
+    ### Internal functions
 
-    def _find_from_unknown_s(self):
-        """calculate the evidence when the std is unknown.
-
-        Raises
-        ------
-        ValueError
-            when the length of longest region is smaller than the minlen.
-
-        """
-
-        res = []
-        start, end, minlen = (
-            self.start,
-            self.end,
-            self.minlen,
-        )
-        funcs = mc_t()
-        if end - start <= minlen:
-            raise ValueError(f"(end - start) must be no less than {minlen}.")
-        # Initial guess with linear regression
-        init_guess = self._get_init_guess()
-        # Go through N's
-        for n in range(minlen, end + 1 - start):
-            # Run calculation and update init_guess
-            init_guess, evi = self._cal_evidence_unknown_s(
-                start, start + n, init_guess, funcs
-            )
-            if evi is None:
-                break
-            else:
-                res.append(evi)
-        return res
-
-    def _get_init_guess(self):
-        """get initial guess by regressing over the whole x and y"""
-        X, Y = self.x, self.y
-        if Y.ndim > 1:
-            # take the first rep as first guess
-            lin_res = linregress(X, Y[0, :])
-        else:
-            lin_res = linregress(X, Y)
-        init_guess = (lin_res.slope, lin_res.intercept)
-        return init_guess
-
-    def _cal_evidence_unknown_s(self, start, end, init_guess, funcs):
-        """calculate evidence without std
+    def _cal_evidence_unknown_err(self, start, end, func):
+        """calculate evidence without err
 
         Parameters
         ----------
         start : init
             start of region
         end : int
-            end of region (inclusive)
-        init_guess : tuple
-            initial guess for scipy.optimize.minimize
-        funcs : tuple of functions
-            tuple of -logL, hessian and jacobian.
+            end of region (exclusive)
 
         """
-        X, Y, attempt = (
-            self.x,
-            self.y,
-            self.attempt,
-        )
-        neglogL, hess, jac = funcs
+        X, Y = (self.x, self.y)
         # flatten multiple reps
         if Y.ndim > 1:
             X_flat = np.append([], [X[start:end]] * Y.shape[0])  # flatten X
             Y_flat = Y[:, start:end].flatten(order="C")
             n_flat = len(X[start:end]) * Y.shape[0]
         else:
             X_flat = X[start:end]
             Y_flat = Y[start:end]
             n_flat = len(X[start:end])
-        # run multiple attempts in case optimisation fails
-        for k in range(attempt):
-            # Guess m and c
-            th00 = np.random.normal(init_guess[0], 2 * np.abs(init_guess[0]))
-            th01 = np.random.normal(init_guess[1], 2 * np.abs(init_guess[1]))
-            th0 = (th00, th01)
-            # Find optimum
-            with np.errstate(invalid="raise", divide="raise"):
-                try:
-                    th_opt = minimize(
-                        neglogL,
-                        th0,
-                        (X_flat, Y_flat, n_flat),
-                        method="BFGS",
-                        jac=jac,
-                    )
-                except FloatingPointError:
-                    continue
-            if th_opt.success:
-                init_guess = th_opt.x  # Update guess
-                hess_opt = hess(th_opt.x, X_flat, Y_flat, n_flat)
-                maxL = -th_opt.fun
-                det = np.linalg.det(hess_opt / (2 * np.pi))
-                if det > 0:
-                    invdetsqrt = -np.log(det) / 2
-                    return (init_guess, maxL + invdetsqrt)
-                else:
-                    continue
-        else:
-            # After running all attempts, still not return, then None
-            return (None, None)
-
-    ### Internal functions for model comparison and exact posterior
-    ###
+        return func(X_flat, Y_flat, n_flat)
 
     def _mc_logprior(self, num_regions):
         """return the log value of the uniform prior given number of boundary points"""
-        res = self.evidence.copy()
+        if self.err is not None:
+            res = self.evidence.copy()
+        else:
+            res = self.D.copy()
         res[~np.isnan(res)] = 1
         res[np.isnan(res)] = 0
         return -np.log(self._findZ(res, num_regions))
 
     def _findZ(self, exp_res, number, vec=None):
         """finding the normalising factor of the posterior"""
         datalen = len(self.x)
@@ -593,25 +658,252 @@
                     return self._find_moment(exp_res, number - 1, k, moment, f_M)
                 else:
                     for n in range(datalen):
                         f_M.append(np.matmul(exp_res[n, :], vec.T)[0])
                     f_M = np.array([f_M[1:] + [0]])
                     return self._find_moment(exp_res, number - 1, k, moment, f_M)
 
-    ### getting entropy
-    ###
-    def _get_entropy(self, start, end):
-        # end is inclusive
-        x = self.x[start : end + 1]
-        y = self.y[start : end + 1]
-        std = self.std[start : end + 1]
-        N = len(x)
-        logevi = self.evidence[start, end]
-        func = mc_entropy()
-        return func(x, y, std, N, logevi)
+    def _findZ_unknown_err_analytical(self, number):
+        """finding the normalisation factor when sigma is unknown.
+
+        The 2pi term and the gamma term are handled in get_number().
+        """
+        exp_u = self._matrix_fill(self.U)
+        exp_d = self._matrix_fill(self.D)
+        N = len(self.x)
+        M = number
+        minlen = self.minlen
+        # upper limits of (number - 1) iboundries
+        u_limits = [N - k * minlen for k in range(number - 1, 0, -1)]
+        l_limits = minlen - 1
+        # list of possible values of each iboundary (end point)
+        ib_ranges = [range(l_limits, u) for u in u_limits]
+        all_combs = product(*ib_ranges)
+        len_all_combs = np.prod(np.array(u_limits) - l_limits)
+        # calculate sum
+        evi = 0
+        # for ibs in tqdm(all_combs, total=len_all_combs):
+        for ibs in all_combs:
+            # including start and end
+            begs_minus_1 = [-1] + list(ibs)
+            ends = list(ibs) + [N - 1]
+            d_i = np.array(
+                [exp_d[b + 1, e] for b, e in zip(begs_minus_1, ends)],
+                dtype=np.longdouble,
+            )
+            D = np.prod(d_i)
+            u_i = np.array(
+                [exp_u[b + 1, e] for b, e in zip(begs_minus_1, ends)],
+                dtype=np.longdouble,
+            )
+            U = np.sum(u_i)
+            # some constants like 2pi and gamma are handled in get_numbers()
+            evi += D * U ** (M - (N * self.nreplicates - 1) / 2) / 2
+        return np.log(evi, dtype=np.longdouble)
+
+    @staticmethod
+    def _matrix_fill(matrix):
+        """copy the result matrix and replace nans with zeros."""
+        res = matrix.copy()
+        res = res.astype(np.longdouble)
+        # normalise to avoid overflow
+        res[np.isnan(res)] = 0
+        return res
+
+    def _exp_res_sigma(self, sigma):
+        """
+        when sigma is unknown and numerical integration is necessary,
+        use this function to generate a matrix as a function of sigma,
+        from which we get P(D|segment, sigma) for each possible segment.
+
+        the 2pi term is left out for get_number() to handle.
+        """
+        return (
+            np.exp(
+                -(self.U) / sigma**2
+                + (2 - self.L) * np.log(sigma, dtype=np.longdouble),
+                # + (1 - self.L / 2) * np.log(2 * np.pi, dtype=np.longdouble),
+                dtype=np.longdouble,
+            )
+            * self.D
+        )
+
+    def _findZ_sigma(self, sigma, number, exp_res=None, vec=None):
+        """finding the normalising factor of the posterior as a function of sigma when sigma is unknown."""
+        if exp_res is None:
+            exp_res = self._matrix_fill(self._exp_res_sigma(sigma))
+        datalen = len(self.x)
+        if vec is None:
+            if number == 1:
+                return exp_res[0, -1]
+            else:
+                f_M = list(exp_res[:, datalen - 1])
+                f_M = np.array([f_M[1:] + [0]])
+                return self._findZ_sigma(sigma, number - 1, exp_res, f_M)
+        else:
+            if number == 1:
+                return np.matmul(exp_res[0, :], vec.T)[0]
+            else:
+                f_M = []
+                for n in range(datalen):
+                    f_M.append(np.matmul(exp_res[n, :], vec.T)[0])
+                f_M = np.array([f_M[1:] + [0]])
+                return self._findZ_sigma(sigma, number - 1, exp_res, f_M)
+
+    def _find_moment_sigma(self, sigma, number, k, moment=1, exp_res=None, vec=None):
+        """finding the moments of the posterior as a function of sigma when sigma is unknown."""
+        if exp_res is None:
+            exp_res = self._matrix_fill(self._exp_res_sigma(sigma))
+        datalen = len(self.x)
+        if vec is None:
+            if number == 1:
+                return None
+            else:  # k < number when vec is None
+                f_M = list(exp_res[:, datalen - 1])
+                f_M = np.array([f_M[1:] + [0]])
+                return self._find_moment_sigma(
+                    sigma, number - 1, k, moment, exp_res, f_M
+                )
+        else:
+            if number == 1:
+                if k == number:
+                    return np.matmul(
+                        exp_res[0, :],
+                        vec.T * np.arange(datalen).reshape(datalen, 1) ** moment,
+                    )[0]
+                else:
+                    return np.matmul(exp_res[0, :], vec.T)[0]
+            else:
+                f_M = []
+                if k == number:
+                    for n in range(datalen):
+                        f_M.append(
+                            np.matmul(
+                                exp_res[n, :],
+                                vec.T
+                                * np.arange(datalen).reshape(datalen, 1) ** moment,
+                            )[0]
+                        )
+                    f_M = np.array([f_M[1:] + [0]])
+                    return self._find_moment_sigma(
+                        sigma, number - 1, k, moment, exp_res, f_M
+                    )
+                else:
+                    for n in range(datalen):
+                        f_M.append(np.matmul(exp_res[n, :], vec.T)[0])
+                    f_M = np.array([f_M[1:] + [0]])
+                    return self._find_moment_sigma(
+                        sigma, number - 1, k, moment, exp_res, f_M
+                    )
+
+    def _find_moment_unknown_err_analytical(self, number, k, moment=1):
+        """finding the moments analytically when sigma is unknown.
+
+        the 2pi term and the gamma term are ignored:
+        that's ok because the Z have the same terms ignored.
+        """
+        exp_u = self._matrix_fill(self.U)
+        exp_d = self._matrix_fill(self.D)
+        N = len(self.x)
+        M = number
+        minlen = self.minlen
+        # upper limits of (number - 1) iboundries
+        u_limits = [N - j * minlen for j in range(number - 1, 0, -1)]
+        l_limits = minlen - 1
+        # list of possible values of each iboundary (end point)
+        ib_ranges = [range(l_limits, u) for u in u_limits]
+        all_combs = product(*ib_ranges)
+        # calculate sum
+        evi = 0
+        # for ibs in tqdm(all_combs, total=len_all_combs):
+        for ibs in all_combs:
+            # including start and end
+            begs_minus_1 = [-1] + list(ibs)
+            ends = list(ibs) + [N - 1]
+            d_i = np.array(
+                [exp_d[b + 1, e] for b, e in zip(begs_minus_1, ends)],
+                dtype=np.longdouble,
+            )
+            D = np.prod(d_i)
+            u_i = np.array(
+                [exp_u[b + 1, e] for b, e in zip(begs_minus_1, ends)],
+                dtype=np.longdouble,
+            )
+            U = np.sum(u_i)
+            evi += (
+                D
+                * U ** (M - (N * self.nreplicates - 1) / 2)
+                / 2
+                # * gamma((N - 1) / 2 - M)
+                * ibs[k - 1] ** moment
+            )
+        return np.log(evi, dtype=np.longdouble)
+
+    def _findZ_unknown_err_numerical(self, number):
+        """finding the normalisation factor numerically when sigma is unknown."""
+        if self.large is False:
+            res = quad(
+                self._findZ_sigma, 0, np.inf, args=(number,), epsabs=0.0, epsrel=1e-10
+            )[0]
+        if (self.large is True) or (
+            not np.isfinite(res)
+        ):  # when large, scale integrand
+            integrand = lambda sigma, M: self._findZ_sigma(sigma, M) / 1e300
+            res = quad(integrand, 0, np.inf, args=(number,), epsabs=0.0, epsrel=1e-10)[
+                0
+            ]
+            if not np.isfinite(res):  # if still infinite
+                raise OverflowError(
+                    "Integral is too large when finding model evidence."
+                )
+            self.large = True
+            return np.log(res, dtype=np.longdouble) + np.log(1e300, dtype=np.longdouble)
+        elif res == 0.0:  # if small
+            integrand = lambda sigma, M: self._findZ_sigma(sigma, M) * 1e300
+            res = quad(integrand, 0, np.inf, args=(number,), epsabs=0.0, epsrel=1e-10)[
+                0
+            ]
+            return np.log(res, dtype=np.longdouble) - np.log(1e300, dtype=np.longdouble)
+        return np.log(res, dtype=np.longdouble)
+
+    def _find_moment_unknown_err_numerical(self, number, k, moment=1):
+        """finding the moments numerically when sigma is unknown."""
+        if self.large is False:
+            res = quad(
+                self._find_moment_sigma,
+                0,
+                np.inf,
+                args=(number, k, moment),
+                epsabs=0.0,
+                epsrel=1e-10,
+            )[0]
+        if (self.large is True) or (
+            not np.isfinite(res)
+        ):  # when large, scale integrand
+            integrand = (
+                lambda sigma, M, K, mom: self._find_moment_sigma(sigma, M, K, mom)
+                / 1e300
+            )
+            res = quad(
+                integrand, 0, np.inf, args=(number, k, moment), epsabs=0.0, epsrel=1e-10
+            )[0]
+            if not np.isfinite(res):  # if still infinite
+                raise OverflowError("Integral is too large when finding boundaries.")
+            self.large = True
+            return np.log(res, dtype=np.longdouble) + np.log(1e300, dtype=np.longdouble)
+        elif res == 0.0:  # if small
+            integrand = (
+                lambda sigma, M, K, mom: self._find_moment_sigma(sigma, M, K, mom)
+                * 1e300
+            )
+            res = quad(
+                integrand, 0, np.inf, args=(number, k, moment), epsabs=0.0, epsrel=1e-10
+            )[0]
+            return np.log(res, dtype=np.longdouble) - np.log(1e300, dtype=np.longdouble)
+        return np.log(res, dtype=np.longdouble)
 
 
 def get_example_data(plot=False):
     """Return example data, with x being cell number and y being three replicates of OD measurement.
 
     Parameters
     ----------
@@ -626,9 +918,9 @@
     x, y = return_data()
     if plot:
         fig, ax = plt.subplots()
         for j in range(y.shape[0]):
             ax.scatter(x, y[j, :], alpha=0.7, color="b")
         ax.set_xlabel("cell number")
         ax.set_ylabel("optical density (OD)")
-        plt.plot()
+        plt.show()
     return x, y
```

### Comparing `nunchaku-0.8.0/pyproject.toml` & `nunchaku-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nunchaku"
-version = "0.8.0"
-description = "To find the linear segment of a curve or dataset."
+version = "0.9.0"
+description = "Dividing data into linear regions."
 authors = ["Yu Huo <yu.huo@ed.ac.uk>"]
 
 license = "MIT"
 readme = "readme.md"
 homepage = "https://nunchaku.readthedocs.io"
 repository = "https://git.ecdf.ed.ac.uk/s1856140/nunchaku"
 documentation = "https://nunchaku.readthedocs.io"
@@ -22,22 +22,24 @@
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 sympy = "^1.9"
 numpy = "^1.20.3"
 scipy = "^1.7.3"
 matplotlib = "^3.5.0"
 pandas = "^1.4"
+tqdm = "^4.65.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 jupyter = "^1.0.0"
 flake8 = "^4.0.1"
 pyright = "^1.1.258"
 Sphinx = "^6.1"
 seaborn = "^0.12.2"
+coverage = "^7.2.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nunchaku-0.8.0/readme.md` & `nunchaku-0.9.0/readme.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,32 +7,34 @@
 
 ## Installation
 For users, type in terminal
 ```
 > pip install nunchaku
 ```
 
-For developers, create a virtual environment and then type 
+For developers, create a virtual environment and then install with Poetry: 
 ```
 > git clone https://git.ecdf.ed.ac.uk/s1856140/nunchaku.git
 > cd nunchaku 
 > poetry install --with dev 
 ```
 
 ## Quickstart
 Data `x` is a list or a 1D Numpy array, sorted ascendingly; the data `y` is a list or a Numpy array, with each row being one replicate of measurement.
 ```
 >>> from nunchaku.nunchaku import nunchaku, get_example_data
 >>> x, y = get_example_data()
 >>> nc = nunchaku(x, y, prior=[-5,5]) # load data and set prior of slope
->>> # compare models with one, two or three linear regions
->>> num_regions, evidences = nc.get_number([1,2,3])
+>>> # compare models with 1, 2, 3 and 4 linear regions
+>>> num_regions, evidences = nc.get_number(max_num=4)
 >>> # get the mean and standard deviation of the boundary points
 >>> bds, bds_std = nc.get_iboundaries(num_regions)
+>>> # get the information of all regions
 >>> info_df = nc.get_info(bds)
+>>> # plot the data and the regions
 >>> nc.plot(info_df)
 ```
 
 ## Documentation
 Detailed documentation is available on [Readthedocs](https://nunchaku.readthedocs.io/en/latest/).
 
 ## Citation
```

### Comparing `nunchaku-0.8.0/setup.py` & `nunchaku-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.5.0,<4.0.0',
  'numpy>=1.20.3,<2.0.0',
  'pandas>=1.4,<2.0',
  'scipy>=1.7.3,<2.0.0',
- 'sympy>=1.9,<2.0']
+ 'sympy>=1.9,<2.0',
+ 'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'nunchaku',
-    'version': '0.8.0',
-    'description': 'To find the linear segment of a curve or dataset.',
-    'long_description': '# nunchaku: Dividing data into linear regions\n\n`nunchaku` is a Python module for dividing data into linear regions.\nIt answers two questions:\n1. how many linear regions best fit the data without overfitting (by Bayesian model comparison);\n2. given the number of linear regions, where the boundaries between them are (by finding the posterior of the boundaries).\n\n## Installation\nFor users, type in terminal\n```\n> pip install nunchaku\n```\n\nFor developers, create a virtual environment and then type \n```\n> git clone https://git.ecdf.ed.ac.uk/s1856140/nunchaku.git\n> cd nunchaku \n> poetry install --with dev \n```\n\n## Quickstart\nData `x` is a list or a 1D Numpy array, sorted ascendingly; the data `y` is a list or a Numpy array, with each row being one replicate of measurement.\n```\n>>> from nunchaku.nunchaku import nunchaku, get_example_data\n>>> x, y = get_example_data()\n>>> nc = nunchaku(x, y, prior=[-5,5]) # load data and set prior of slope\n>>> # compare models with one, two or three linear regions\n>>> num_regions, evidences = nc.get_number([1,2,3])\n>>> # get the mean and standard deviation of the boundary points\n>>> bds, bds_std = nc.get_iboundaries(num_regions)\n>>> info_df = nc.get_info(bds)\n>>> nc.plot(info_df)\n```\n\n## Documentation\nDetailed documentation is available on [Readthedocs](https://nunchaku.readthedocs.io/en/latest/).\n\n## Citation\nA preprint is coming soon.\n',
+    'version': '0.9.0',
+    'description': 'Dividing data into linear regions.',
+    'long_description': '# nunchaku: Dividing data into linear regions\n\n`nunchaku` is a Python module for dividing data into linear regions.\nIt answers two questions:\n1. how many linear regions best fit the data without overfitting (by Bayesian model comparison);\n2. given the number of linear regions, where the boundaries between them are (by finding the posterior of the boundaries).\n\n## Installation\nFor users, type in terminal\n```\n> pip install nunchaku\n```\n\nFor developers, create a virtual environment and then install with Poetry: \n```\n> git clone https://git.ecdf.ed.ac.uk/s1856140/nunchaku.git\n> cd nunchaku \n> poetry install --with dev \n```\n\n## Quickstart\nData `x` is a list or a 1D Numpy array, sorted ascendingly; the data `y` is a list or a Numpy array, with each row being one replicate of measurement.\n```\n>>> from nunchaku.nunchaku import nunchaku, get_example_data\n>>> x, y = get_example_data()\n>>> nc = nunchaku(x, y, prior=[-5,5]) # load data and set prior of slope\n>>> # compare models with 1, 2, 3 and 4 linear regions\n>>> num_regions, evidences = nc.get_number(max_num=4)\n>>> # get the mean and standard deviation of the boundary points\n>>> bds, bds_std = nc.get_iboundaries(num_regions)\n>>> # get the information of all regions\n>>> info_df = nc.get_info(bds)\n>>> # plot the data and the regions\n>>> nc.plot(info_df)\n```\n\n## Documentation\nDetailed documentation is available on [Readthedocs](https://nunchaku.readthedocs.io/en/latest/).\n\n## Citation\nA preprint is coming soon.\n',
     'author': 'Yu Huo',
     'author_email': 'yu.huo@ed.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://nunchaku.readthedocs.io',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `nunchaku-0.8.0/PKG-INFO` & `nunchaku-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nunchaku
-Version: 0.8.0
-Summary: To find the linear segment of a curve or dataset.
+Version: 0.9.0
+Summary: Dividing data into linear regions.
 Home-page: https://nunchaku.readthedocs.io
 License: MIT
 Keywords: linear segment,systems biology,bioinformatics,plate readers
 Author: Yu Huo
 Author-email: yu.huo@ed.ac.uk
 Requires-Python: >=3.8,<3.11
 Classifier: Intended Audience :: Science/Research
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: matplotlib (>=3.5.0,<4.0.0)
 Requires-Dist: numpy (>=1.20.3,<2.0.0)
 Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: scipy (>=1.7.3,<2.0.0)
 Requires-Dist: sympy (>=1.9,<2.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Documentation, https://nunchaku.readthedocs.io
 Project-URL: Repository, https://git.ecdf.ed.ac.uk/s1856140/nunchaku
 Description-Content-Type: text/markdown
 
 # nunchaku: Dividing data into linear regions
 
 `nunchaku` is a Python module for dividing data into linear regions.
@@ -34,32 +35,34 @@
 
 ## Installation
 For users, type in terminal
 ```
 > pip install nunchaku
 ```
 
-For developers, create a virtual environment and then type 
+For developers, create a virtual environment and then install with Poetry: 
 ```
 > git clone https://git.ecdf.ed.ac.uk/s1856140/nunchaku.git
 > cd nunchaku 
 > poetry install --with dev 
 ```
 
 ## Quickstart
 Data `x` is a list or a 1D Numpy array, sorted ascendingly; the data `y` is a list or a Numpy array, with each row being one replicate of measurement.
 ```
 >>> from nunchaku.nunchaku import nunchaku, get_example_data
 >>> x, y = get_example_data()
 >>> nc = nunchaku(x, y, prior=[-5,5]) # load data and set prior of slope
->>> # compare models with one, two or three linear regions
->>> num_regions, evidences = nc.get_number([1,2,3])
+>>> # compare models with 1, 2, 3 and 4 linear regions
+>>> num_regions, evidences = nc.get_number(max_num=4)
 >>> # get the mean and standard deviation of the boundary points
 >>> bds, bds_std = nc.get_iboundaries(num_regions)
+>>> # get the information of all regions
 >>> info_df = nc.get_info(bds)
+>>> # plot the data and the regions
 >>> nc.plot(info_df)
 ```
 
 ## Documentation
 Detailed documentation is available on [Readthedocs](https://nunchaku.readthedocs.io/en/latest/).
 
 ## Citation
```

