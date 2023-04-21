# Comparing `tmp/plastic_balanced_network-0.0.3.tar.gz` & `tmp/plastic_balanced_network-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plastic_balanced_network-0.0.3.tar", last modified: Fri Mar 31 23:33:47 2023, max compression
+gzip compressed data, was "plastic_balanced_network-0.1.0.tar", last modified: Fri Apr 21 03:22:49 2023, max compression
```

## Comparing `plastic_balanced_network-0.0.3.tar` & `plastic_balanced_network-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-03-31 23:33:47.176419 plastic_balanced_network-0.0.3/
--rw-r--r--   0 alan       (501) staff       (20)     1080 2023-03-27 20:20:02.000000 plastic_balanced_network-0.0.3/LICENSE.txt
--rw-r--r--   0 alan       (501) staff       (20)     3049 2023-03-31 23:33:47.175990 plastic_balanced_network-0.0.3/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)     2121 2023-03-31 23:32:55.000000 plastic_balanced_network-0.0.3/README.md
--rw-r--r--   0 alan       (501) staff       (20)       38 2023-03-31 23:33:47.176595 plastic_balanced_network-0.0.3/setup.cfg
--rw-r--r--   0 alan       (501) staff       (20)     2163 2023-03-31 01:11:15.000000 plastic_balanced_network-0.0.3/setup.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-03-31 23:33:47.168980 plastic_balanced_network-0.0.3/src/
--rw-r--r--   0 alan       (501) staff       (20)    16875 2023-03-31 01:11:15.000000 plastic_balanced_network-0.0.3/src/pbn_simulation.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-03-31 23:33:47.170658 plastic_balanced_network-0.0.3/src/plastic_balanced_network/
--rw-r--r--   0 alan       (501) staff       (20)        0 2023-03-24 21:48:44.000000 plastic_balanced_network-0.0.3/src/plastic_balanced_network/__init__.py
--rw-r--r--   0 alan       (501) staff       (20)    45517 2023-03-31 23:27:08.000000 plastic_balanced_network-0.0.3/src/plastic_balanced_network/helpers.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-03-31 23:33:47.174094 plastic_balanced_network-0.0.3/src/plastic_balanced_network.egg-info/
--rw-r--r--   0 alan       (501) staff       (20)     3049 2023-03-31 23:33:47.000000 plastic_balanced_network-0.0.3/src/plastic_balanced_network.egg-info/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)      431 2023-03-31 23:33:47.000000 plastic_balanced_network-0.0.3/src/plastic_balanced_network.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (501) staff       (20)        1 2023-03-31 23:33:47.000000 plastic_balanced_network-0.0.3/src/plastic_balanced_network.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (501) staff       (20)      473 2023-03-31 23:33:47.000000 plastic_balanced_network-0.0.3/src/plastic_balanced_network.egg-info/requires.txt
--rw-r--r--   0 alan       (501) staff       (20)       40 2023-03-31 23:33:47.000000 plastic_balanced_network-0.0.3/src/plastic_balanced_network.egg-info/top_level.txt
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-03-31 23:33:47.174613 plastic_balanced_network-0.0.3/tests/
--rw-r--r--   0 alan       (501) staff       (20)    69893 2023-03-31 01:11:15.000000 plastic_balanced_network-0.0.3/tests/test_plastic_balanced_network.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-04-21 03:22:49.892877 plastic_balanced_network-0.1.0/
+-rw-r--r--   0 alan       (501) staff       (20)     1080 2023-04-21 03:08:55.000000 plastic_balanced_network-0.1.0/LICENSE.txt
+-rw-r--r--   0 alan       (501) staff       (20)     4943 2023-04-21 03:22:49.892555 plastic_balanced_network-0.1.0/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)     4015 2023-04-21 03:08:55.000000 plastic_balanced_network-0.1.0/README.md
+-rw-r--r--   0 alan       (501) staff       (20)      328 2023-04-21 03:03:07.000000 plastic_balanced_network-0.1.0/pyproject.toml
+-rw-r--r--   0 alan       (501) staff       (20)       38 2023-04-21 03:22:49.892998 plastic_balanced_network-0.1.0/setup.cfg
+-rw-r--r--   0 alan       (501) staff       (20)     2163 2023-04-21 03:08:56.000000 plastic_balanced_network-0.1.0/setup.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-04-21 03:22:49.886273 plastic_balanced_network-0.1.0/src/
+-rw-r--r--   0 alan       (501) staff       (20)    12196 2023-04-21 03:08:56.000000 plastic_balanced_network-0.1.0/src/pbn_simulation.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-04-21 03:22:49.887280 plastic_balanced_network-0.1.0/src/plastic_balanced_network/
+-rw-r--r--   0 alan       (501) staff       (20)        0 2023-04-21 03:08:56.000000 plastic_balanced_network-0.1.0/src/plastic_balanced_network/__init__.py
+-rw-r--r--   0 alan       (501) staff       (20)    54035 2023-04-21 03:08:56.000000 plastic_balanced_network-0.1.0/src/plastic_balanced_network/helpers.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-04-21 03:22:49.889891 plastic_balanced_network-0.1.0/src/plastic_balanced_network.egg-info/
+-rw-r--r--   0 alan       (501) staff       (20)     4943 2023-04-21 03:22:49.000000 plastic_balanced_network-0.1.0/src/plastic_balanced_network.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)      446 2023-04-21 03:22:49.000000 plastic_balanced_network-0.1.0/src/plastic_balanced_network.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (501) staff       (20)        1 2023-04-21 03:22:49.000000 plastic_balanced_network-0.1.0/src/plastic_balanced_network.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (501) staff       (20)      437 2023-04-21 03:22:49.000000 plastic_balanced_network-0.1.0/src/plastic_balanced_network.egg-info/requires.txt
+-rw-r--r--   0 alan       (501) staff       (20)       40 2023-04-21 03:22:49.000000 plastic_balanced_network-0.1.0/src/plastic_balanced_network.egg-info/top_level.txt
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-04-21 03:22:49.890299 plastic_balanced_network-0.1.0/tests/
+-rw-r--r--   0 alan       (501) staff       (20)    68808 2023-04-21 03:20:17.000000 plastic_balanced_network-0.1.0/tests/test_plastic_balanced_network.py
```

### Comparing `plastic_balanced_network-0.0.3/LICENSE.txt` & `plastic_balanced_network-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plastic_balanced_network-0.0.3/setup.py` & `plastic_balanced_network-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ####### Metadata ########
 NAME = "plastic_balanced_network"
 DESCRIPTION = "Plastic Balanced Network Package (Akil et al., 2021)"
 LDESCRIPTION = open('README.md').read()
 # URL = text/markdown
 MAINTAINER = "Alan Akil"
 EMAIL = "alan.akil@yahoo.com"
-REQUIRES_PYTHON = ">=3.7,<3.10"
+REQUIRES_PYTHON = ">3.7,<=3.10"
 PACKAGES = find_packages(where = "src", exclude=("tests",))
 
 ROOT_DIR = Path(__file__).parent
 
 PACKAGE_DIR = os.path.join(ROOT_DIR, "src", NAME)
 about = {}
 with open(os.path.join(PACKAGE_DIR, "VERSION")) as f:
```

### Comparing `plastic_balanced_network-0.0.3/src/pbn_simulation.py` & `plastic_balanced_network-0.1.0/src/pbn_simulation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 """
-This code is a sample simulation of a plastic balanced network as defined in Akil et al, 2021. 
+This code is a sample simulation of a plastic balanced network as defined in Akil et al, 2021.
 The purpose of this code is to demonstrate how the `plastic_balanced_network` package can be used.
 
-We allow for a great deal of flexibility constructing the simulation/s. 
-One may easily change the following parameters: 
+We allow for a great deal of flexibility constructing the simulation/s.
+One may easily change the following parameters:
 (1) Total number of neurons.
 (2) Fraction of E-I neurons.
 (3) Probability of connection.
 (4) Synaptic strengths.
 (5) Total time of simulation.
 (6) Input rate and correlations.
 (7) Extra injected current.
 (8) EIF neuron parameters.
 (9) Plasticity parameters on any connection type.
 
-Output data is saved in the `data/processed` folder. 
+Output data is saved in the `data/processed` folder.
 Logs are saved in `logs` folder.
 Please refer to the README.md for detailed instructions on how to run this code.
 """
 __author__ = "Alan Akil (alan.akil@yahoo.com)"
-__date__ = "MARCH 2023"
+__date__ = "APRIL 2023"
 
-#%%
+# %%
 # Load python packages.
 import numpy as np
-import random2
 import matplotlib.pyplot as plt
 import seaborn as sns
 import time
 import logging
 from datetime import datetime as dtm
-import datetime as dt
 import os
 from pathlib import Path
 
-from plastic_balanced_network.helpers import plasticNeuralNetwork
+from plastic_balanced_network.helpers import (
+    PlasticNeuralNetwork,
+    compute_firing_rate,
+    spike_count_cov,
+    cov2corr,
+    average_cov_corr_over_subpops,
+)
 
-#%%
+# %%
 # Construct a str containing the datetime when the simulation is run.
 todaysdate = dtm.today()
 datetime_format = "%Y%b%d-%H%M"
 datadatetime = todaysdate.strftime(datetime_format).upper()
 
 # Define paths: project root, data directory, and logs directory.
 PROJECTROOT = Path(__file__).parent.parent
 DATA_DIR = os.path.join(PROJECTROOT, "data", "processed")
 LOG_DIR = os.path.join(PROJECTROOT, "logs")
 os.makedirs(DATA_DIR, exist_ok=True)
 os.makedirs(LOG_DIR, exist_ok=True)
 DATA_FILE_PATH = f"{DATA_DIR}/pbn_data_{datadatetime}.npz"
 
-#%%
+# %%
 # Set up logging.
-log_format = (
-    "%(asctime)s - %(levelname)-8s - %(name)s - %(funcName)s:%(lineno)d - %(message)s"
-)
+log_format = "%(asctime)s - %(levelname)-8s - %(name)s - %(funcName)s:%(lineno)d - %(message)s"
 # Use loglevel to filter out undesired logs.
 loglevel = "INFO"
 loglevel = str(loglevel).replace('"', "")
 levels = {
     "CRITICAL": logging.CRITICAL,
     "ERROR": logging.ERROR,
     "WARN": logging.WARN,
@@ -78,146 +80,64 @@
 )
 
 logging.info(f"Project root: {PROJECTROOT}.")
 logging.info(f"Data directory: {DATA_DIR}.")
 logging.info(f"Logs directory: {LOG_DIR}.")
 
 
-#%%
+# %%
 # Define all input variables for the network simulation.
 logging.info("Define input variables for plastic balanced network simulation.")
 
 # Total number of neurons.
 N = int(5000)
-# Fraction of excitatory neurons.
-frac_exc = 0.8
-# Extra fraction of neurons (external).
-frac_ext = 0.2
-
-# Define individual connection probabilities.
-p_ee = 0.1
-p_ei = 0.1
-p_ie = 0.1
-p_ii = 0.1
-p_ex = 0.1
-p_ix = 0.1
-# Recurrent net connection probabilities.
-P = np.array([[p_ee, p_ei], [p_ie, p_ii]])
-# Ffwd connection probs.
-Px = np.array([[p_ex], [p_ix]])
-
-# Mean connection strengths between each cell type pair.
-jee = 25
-jei = -150
-jie = 112.5
-jii = -250
-jex = 180
-jix = 135
-Jm = np.array([[jee, jei], [jie, jii]]) / np.sqrt(N)
-Jxm = np.array([[jex], [jix]]) / np.sqrt(N)
-
 # Total time (in ms) for simulation.
 T = 5000
 
-# Step size for discretization.
-dt = 0.1
-
 # FFwd spike train rate (in kHz).
 rx = 10 / 1000
 # Correlation of ffwd spike trains.
 cx = 0.1
-# Timescale of correlation in ms. Jitter spike trains in external layer by taujitter.
-taujitter = 5
-
-# Extra stimulus: Istim is a Total_time-dependent stimulus
-# it is delivered to all neurons with weights given by Jstim.
-# Specifically, the stimulus to neuron j at Total_time index i is:
-# Istim(i)*Jstim(j)
-jestim = 0
-jistim = 0
-
-# Synaptic timescales in ms.
-taux = 10
-taue = 8
-taui = 4
-
-# Neuron parameters.
-Cm = 1
-gL = 1 / 15
-EL = -72
-Vth = -50
-Vre = -75
-DeltaT = 1
-VT = -55
-
-# Plasticity parameters.
-tauSTDP = 200  # ms
 
 # EE hebb
-Jmax_ee = 30 / np.sqrt(N)
 eta_ee_hebb = 0 / 10**3  # Learning rate, if zero then no plasticity.
-
 # EE kohonen
-beta = 2 / np.sqrt(N)
 eta_ee_koh = 0 / 10**2  # Learning rate, if zero then no plasticity.
-
+beta = 2
 # IE hebb
-Jmax_ie_hebb = 125 / np.sqrt(N)
 eta_ie_hebb = 0 / 10**3  # Learning rate, if zero then no plasticity.
-
 # IE homeostatic
-Jnorm_ie = 200 / np.sqrt(N)
-eta_ie_homeo = 0 / 10**3 / Jnorm_ie  # Learning rate, if zero then no plasticity.
+eta_ie_homeo = 0 / 10**3  # Learning rate, if zero then no plasticity.
 rho_ie = 0.020  # Target rate 20Hz
-alpha_ie = 2 * rho_ie * tauSTDP
-
 # EI homeostatic
-Jnorm_ei = -200 / np.sqrt(N)
-eta_ei = 0.015 / 10**3 / Jnorm_ei  # Learning rate, if zero then no plasticity.
+eta_ei = 0.015 / 10**3  # Learning rate, if zero then no plasticity.
 rho_ei = 0.010  # Target rate 10Hz
-alpha_ei = 2 * rho_ei * tauSTDP
-
 # II homeostatic
-Jnorm_ii = -300 / np.sqrt(N)
-eta_ii = 0.015 / 10**3 / Jnorm_ii  # Learning rate, if zero then no plasticity.
+eta_ii = 0.015 / 10**3  # Learning rate, if zero then no plasticity.
 rho_ii = 0.020  # Target rate 20Hz
-alpha_ii = 2 * rho_ii * tauSTDP
-
-# Number of neurons to record from each population.
-numrecord = int(100)  
-# Number of time bins to average over when recording currents and voltages.
-nBinsRecord = 10
-# Number of synapses to be sampled per cell type pair that is plastic.
-nJrecord0 = 1000
 
 # Set the random seed.
 np.random.seed(31415)
 
-#%%
+# %%
 # Define the model.
-pnn = plasticNeuralNetwork(
+pnn = PlasticNeuralNetwork(
     N,
-    frac_exc,
-    frac_ext,
     T,
-    dt,
-    jestim,
-    jistim,
-    nBinsRecord,
 )
 
-#%%
+# %%
 # Initialize the connectivity.
-pnn.connectivity(Jm, Jxm, P, Px, nJrecord0)
+pnn.connectivity()
 
-#%%
+# %%
 # Generate Poisson ffwd spike trains.
-pnn.ffwd_spikes(cx, rx, taujitter, T)
+pnn.ffwd_spikes(T, cx, rx)
 
-#%%
+# %%
 # Simulate plastic network.
 # Note that spike trains are recorded in s as follows:
 # s(0,:) are the spike times
 # s(1,:) are the associated neuron indices
 (
     s,
     sx,
@@ -227,46 +147,48 @@
     JRec_ii,
     IeRec,
     IiRec,
     IxRec,
     VRec,
     timeRecord,
 ) = pnn.simulate(
-    Cm,
-    gL,
-    VT,
-    Vre,
-    Vth,
-    EL,
-    DeltaT,
-    taue,
-    taui,
-    taux,
-    tauSTDP,
-    numrecord,
-    eta_ee_hebb,
-    Jmax_ee,
-    eta_ee_koh,
-    beta,
-    eta_ie_homeo,
-    alpha_ie,
-    eta_ie_hebb,
-    Jmax_ie_hebb,
-    eta_ei,
-    alpha_ei,
-    eta_ii,
-    alpha_ii,
-    dt,
-    nBinsRecord,
+    eta_ee_hebb=eta_ee_hebb,
+    eta_ee_koh=eta_ee_koh,
+    eta_ie_homeo=eta_ie_homeo,
+    eta_ie_hebb=eta_ie_hebb,
+    eta_ei=eta_ei,
+    eta_ii=eta_ii,
 )
 
-#%% [markdown]
+# %%
+# If one uses default parameters from the pnn class, we can easily access them like this:
+frac_exc = pnn.frac_exc
+frac_ext = pnn.frac_ext
+jee = pnn.jee
+jie = pnn.jie
+jei = pnn.jei
+jii = pnn.jii
+jex = pnn.jex
+jix = pnn.jix
+p_ee = pnn.p_ee
+p_ie = pnn.p_ie
+p_ei = pnn.p_ei
+p_ii = pnn.p_ii
+p_ex = pnn.p_ex
+p_ix = pnn.p_ix
+tauSTDP = pnn.tauSTDP
+beta = pnn.beta
+jmax_ee = pnn.jmax_ee
+jmax_ie_hebb = pnn.jmax_ie_hebb
+dt = pnn.dt
+
+# %% [markdown]
 ## Save and load relevant data variables for analysis and plotting.
 
-#%%
+# %%
 # Save data containing relevant variables.
 np.savez(
     DATA_FILE_PATH,  # File name
     s=s,
     sx=sx,
     JRec_ee=JRec_ee,
     JRec_ie=JRec_ie,
@@ -276,54 +198,59 @@
     IiRec=IiRec,
     IxRec=IxRec,
     VRec=VRec,
     timeRecord=timeRecord,
     N=N,
     frac_exc=frac_exc,
     frac_ext=frac_ext,
-    P=P,
-    Px=Px,
-    Jm=Jm,
-    Jxm=Jxm,
+    p_ee=p_ee,
+    p_ie=p_ie,
+    p_ei=p_ei,
+    p_ii=p_ii,
+    p_ex=p_ex,
+    p_ix=p_ix,
+    jee=jee,
+    jie=jie,
+    jei=jei,
+    jii=jii,
+    jex=jex,
+    jix=jix,
     T=T,
     dt=dt,
     cx=cx,
     rx=rx,
     tauSTDP=tauSTDP,
-    Jmax_ee=Jmax_ee,
+    jmax_ee=jmax_ee,
     eta_ee_hebb=eta_ee_hebb,
     beta=beta,
     eta_ee_koh=eta_ee_koh,
-    Jmax_ie_hebb=Jmax_ie_hebb,
+    jmax_ie_hebb=jmax_ie_hebb,
     eta_ie_hebb=eta_ie_hebb,
-    Jnorm_ie=Jnorm_ie,
     eta_ie_homeo=eta_ie_homeo,
     rho_ie=rho_ie,
-    Jnorm_ei=Jnorm_ei,
     eta_ei=eta_ei,
     rho_ei=rho_ei,
-    Jnorm_ii=Jnorm_ii,
     eta_ii=eta_ii,
-    rho_ii=rho_ii
-    )
+    rho_ii=rho_ii,
+)
 
-#%%
+# %%
 # Load data from previous runs.
 data = np.load(DATA_FILE_PATH)
 # loop through the variables and set them as local variables with the same name as the key
-for key, value in data.items():
+for key, _value in data.items():
     exec(f"{key} = value")
 
 # %% [markdown]
 ### Analysis of simulation
 
 # %% [markdown]
 # Raster plot of neurons firing.
 
-#%%
+# %%
 # Raster plot.
 fig = plt.figure(figsize=(8, 5))
 ax = plt.subplot(111)
 
 sns.set()
 sns.set_style("whitegrid")
 sns.set_style("white")
@@ -488,185 +415,81 @@
 
 sns.despine()
 plt.show()
 
 # %% [markdown]
 # Time course of firing rates.
 
-#%%
-# Time course of firing rates.
-
-# Compute histogram of rates (over time)
-dtRate = 100  # ms
-timeVector = np.arange(dtRate, T + dtRate, dtRate) / 1000
-hist, bin_edges = np.histogram(s[0, s[1, :] < frac_exc * N], bins=len(timeVector))
-eRateT = hist / (dtRate * frac_exc * N) * 1000
-
-hist, bin_edges = np.histogram(s[0, s[1, :] >= frac_exc * N], bins=len(timeVector))
-iRateT = hist / (dtRate * (1 - frac_exc) * N) * 1000
-
-# Slide a window over the rates to smooth them.
-window = 5
-Num_points = int(len(eRateT) - window)
-eRate_New = np.zeros((Num_points, 1))
-iRate_New = np.zeros((Num_points, 1))
-for i in range(Num_points):
-    eRate_New[i, 0] = np.mean(eRateT[i : i + window])
-    iRate_New[i, 0] = np.mean(iRateT[i : i + window])
+# %%
+# Compute smoothed histogram of rates (over time)
+eRateT, iRateT, timeVector = compute_firing_rate(s, T, N, frac_exc=0.8, dtRate=10, window_size=10)
 
 # Start the figure.
 fig = plt.figure(figsize=(8, 5))
 ax = plt.subplot(111)
 sns.set()
 sns.set_style("whitegrid")
 sns.set_style("white")
 sns.set_style("ticks")
 sns.set_context("talk", font_scale=1.9, rc={"lines.linewidth": 3.3})
 
 # Plot time-dependent rates
-plt.plot(np.linspace(0, T / 1000, num=Num_points), eRate_New, color="blue", label=r"e")
-plt.plot(np.linspace(0, T / 1000, num=Num_points), iRate_New, color="red", label=r"i")
+plt.plot(timeVector, eRateT, color="blue", label=r"e")
+plt.plot(timeVector, iRateT, color="red", label=r"i")
 
 plt.ylabel("rate (Hz)")
 plt.xlabel("time (s)")
 plt.xticks((0, T / 1000))
 plt.xlim((0, T / 1000))
 
 leg = plt.legend(loc="upper right", fontsize=18, frameon="none", markerscale=1)
 leg.get_frame().set_linewidth(0.0)
 
 sns.despine()
 plt.show()
 
 # %% [markdown]
-# Define functions to compute empirical spike train covariances and correlations.
+# Compute empirical spike train covariances and correlations.
 
 # %%
-
-#  Compute spike count covariance matrix.
-#  s is a 2x(ns) matrix where ns is the number of spikes
-#  s(0,:) lists spike times
-#  and s(1,:) lists corresponding neuron indices
-#  Neuron indices are assumed to go from 1 to N
-
-#  Spikes are counts starting at time T1 and ending at
-#  time T2.
-
-#  winsize is the window size over which spikes are counted,
-#  so winsize is assumed to be much smaller than T2-T1
-
-#  Covariances are only computed between neurons whose
-#  indices are listed in the vector Inds. If Inds is not
-#  passed in then all NxN covariances are computed.
-
-
-def SpikeCountCov(s, N, T1, T2, winsize):
-
-    Inds = np.arange(0, N)
-
-    #   Count only spikes between T1, T2
-    s1 = s[:, (s[0, :] <= T2) & (s[1, :] >= T1)]
-
-    #   Count only for neurons between 0, N
-    s1 = s[:, (s[1, :] < N) & (s[1, :] >= 0)]
-
-    #   Edges for histogram
-    edgest = np.arange(T1, T2, winsize)
-    edgesi = np.arange(0, N + 1)
-
-    #   Get 2D histogram of spike indices and times
-    counts, xedges, yedges = np.histogram2d(s1[0, :], s1[1, :], bins=(edgest, edgesi))
-
-    #   Compute and return covariance matrix
-    return np.array(np.cov(counts.transpose()))
-
-
-def cov2corr(cov):
-    """convert covariance matrix to correlation matrix
-
-    Parameters
-    ----------
-    cov : array_like, 2d
-        covariance matrix, see Notes
-
-    Returns
-    -------
-    corr : ndarray (subclass)
-        correlation matrix
-    return_std : bool
-        If this is true then the standard deviation is also returned.
-        By default only the correlation matrix is returned.
-
-    Notes
-    -----
-    This function does not convert subclasses of ndarrays. This requires
-    that division is defined elementwise. np.ma.array and np.matrix are allowed.
-
-    """
-    cov = np.asanyarray(cov)
-    std_ = np.sqrt(np.diag(cov))
-    corr = cov / np.outer(std_, std_)
-    return corr
-
-
-# %% [markdown]
-# Apply functions above to compute covariances and correlations.
-
-#%%
 # Compute spike count covariances over windows of size
 # winsize starting at time T1 and ending at time T2.
 winsize = 250  # ms
 T1 = T / 2  # ms
 T2 = T  # ms
 # Do computation
-C = SpikeCountCov(s, N, T1, T2, winsize)
-
+C = spike_count_cov(s, N, T1, T2, winsize)
 
-# Get mean spike count covariances over each sub-pop
-II, JJ = np.meshgrid(np.arange(0, N), np.arange(0, N))
-mCee = np.nanmean(C[(II < frac_exc * N) & (JJ < II)])
-mCei = np.nanmean(C[(II < frac_exc * N) & (JJ >= frac_exc * N)])
-mCii = np.nanmean(C[(II > frac_exc * N) & (JJ > II)])
-
-# Mean-field spike count cov matrix
-# Compare this to the theoretical prediction
-mC = [[mCee, mCei], [mCei, mCii]]
+mC = average_cov_corr_over_subpops(C, N, frac_exc)
 
 # Compute spike count correlations
-# This takes a while, so make it optional
-ComputeSpikeCountCorrs = 1
-if ComputeSpikeCountCorrs:
-
-    #    Get correlation matrix from cov matrix
-    start_time = time.time()
-    R = cov2corr(C)
-    elapsed_time = time.time() - start_time
-    print(elapsed_time / 60, "minutes")
-
-    mRee = np.nanmean(R[(II < frac_exc * N) & (JJ < II)])
-    mRei = np.nanmean(R[(II < frac_exc * N) & (JJ >= frac_exc * N)])
-    mRii = np.nanmean(R[(II > frac_exc * N) & (JJ > II)])
-
-    # Mean-field spike count correlation matrix
-    mR = [[mRee, mRei], [mRei, mRii]]
-    print("mR =", mR)
+# Get correlation matrix from cov matrix
+start_time = time.time()
+R = cov2corr(C)
+elapsed_time = time.time() - start_time
+print(elapsed_time / 60, "minutes")
+
+mR = average_cov_corr_over_subpops(R, N, frac_exc)
+print("mR =", mR)
 
 # %% [markdown]
 # Plot distributions of EE, EI, IE, II correlations.
 
 # %%
 # Plot distributions of EE, EI, IE, II correlations.
 fig = plt.figure(figsize=(8, 5))
 ax = plt.subplot(111)
 sns.set()
 sns.set_style("whitegrid")
 sns.set_style("white")
 sns.set_style("ticks")
 sns.set_context("talk", font_scale=1.9, rc={"lines.linewidth": 3.3})
 
+II, JJ = np.meshgrid(np.arange(0, N), np.arange(0, N))
+
 sns.histplot(
     R[(II < frac_exc * N) & (JJ < II)],
     bins=100,
     kde=False,
     stat="density",
     element="step",
     fill=False,
```

### Comparing `plastic_balanced_network-0.0.3/src/plastic_balanced_network/helpers.py` & `plastic_balanced_network-0.1.0/src/plastic_balanced_network/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,84 @@
 """
 Functions to build and simulate a plastic balanced network.
 """
 __author__ = "Alan Akil (alan.akil@yahoo.com)"
 __date__ = "MARCH 2023"
 
-#%%
+# %%
 import numpy as np
 import random2
 import math
 import time
 import logging
+import sys
 
-#%%
-class plasticNeuralNetwork:
-    """
-    plasticNeuralNetwork is a class that builds a neural network with
+
+# %%
+class PlasticNeuralNetwork:
+    """plasticNeuralNetwork is a class that builds a neural network with
     correlated or uncorrelated firing as well as with plastic or static
     synaptic weights on any connection.
     It contains functions to define the connectivity, simulate feedforward external
     spike trains, and to simulate the recurrent network's firing.
+
+    Inputs
+    :param N: Total number of neurons in recurrent neural network.
+    :type N: int
+    :param T: Total time of simulation in milliseconds.
+    :type T: int
+    :param frac_exc: Fraction of excitatory neurons. Defaults to 0.8.
+    :type frac_exc: float or int
+    :param frac_ext: Fraction of excitatory neurons in external layer. Defaults to 0.2.
+    :type frac_ext: float or int
+    :param dt: Time bin size in milliseconds for time discretization. Defaults to 0.1 ms.
+    :type dt: float or int
+    :param jestim: Added constant current to excitatory neurons. Defaults to 0.
+    :type jestim: float or int
+    :param jistim: Added constant current to inhibitory neurons. Defaults to 0.
+    :type jistim: float or int
+    :param nBinsRecord: Number of bins to record average and record over. Defaults to 10.
+    :type nBinsRecord: int
+
+    Returns as part of self.
+    :return: Number of excitatory neurons (Ne); Number of inhibitory neurons (Ni); Number of external neurons (Nx);
+    Total number of discretized time points (Nt); Time vector of added constant stimulatiom (Istim);
+    Weight coupling for Istim (Jstim); Maximum number of spikes to terminate pathologic behavior (maxns);
+    Discretized recorded time domain (timeRecord); Number of points in discretized recorded time domain (Ntrec).
+    :rtype: tuple(int, int, int, int, np.ndarray, np.ndarray, float or int, np.ndarray, int)
     """
+
     def __init__(
         self,
         N,
-        frac_exc,
-        frac_ext,
         T,
-        dt,
-        jestim,
-        jistim,
-        nBinsRecord,
+        frac_exc=0.8,
+        frac_ext=0.2,
+        dt=0.1,
+        jestim=0,
+        jistim=0,
+        nBinsRecord=10,
     ):
-        """
-        Initializing function.
-
-        Inputs
-        :param N: Total number of neurons in recurrent neural network.
-        :type N: int
-        :param frac_exc: Fraction of excitatory neurons. Typically 0.8.
-        :type frac_exc: float or int 
-        :param frac_ext: Fraction of excitatory neurons in external layer. Typically 0.2.
-        :type frac_ext: float or int 
-        :param T: Total time of simulation in milliseconds.
-        :type T: int
-        :param dt: Time bin size for time discretization.
-        :type dt: float or int 
-        :param jestim: Added constant current to excitatory neurons.
-        :type jestim: float or int 
-        :param jistim: Added constant current to inhibitory neurons.
-        :type jistim: float or int 
-        :param nBinsRecord: Number of bins to record average and record over.
-        :type nBinsRecord: int
-
-        Returns
-        Ne : int
-            Number of excitatory neurons.
-        Ni : int
-            Number of inhibitory neurons.
-        Nx : int
-            Number of external neurons.
-        Nt : int
-            Total number of discretized time points.
-        Istim : np.ndarray
-            Time vector of added constant stimulation.
-        Jstim : np.ndarray
-            Weight coupling for Istim.
-        maxns : float or int
-            Maximum number of spikes to terminate pathologic behavior.
-        timeRecord : np.ndarray
-            Discretized recorded time domain.
-        Ntrec : int
-            Number of points in discretized recorded time domain.
-        """
+        # None error.
+        if N is None:
+            err = ValueError(
+                """ERROR: N cannot be None. Pick an integer number of total neurons.
+                A number in the order of 10^3 is a good place to start.
+                """
+            )
+            logging.exception(err)
+            raise err
+        if T is None:
+            err = ValueError(
+                """ERROR: T cannot be None. Pick an integer number of total simulation time.
+                A number in the order of 10^3 is a good place to start for a quick simulation.
+                """
+            )
+            logging.exception(err)
+            raise err
         # Type tests.
         if not isinstance(N, (int, np.integer)):
             err = TypeError("ERROR: N is not int")
             logging.exception(err)
             raise err
         if not isinstance(frac_exc, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: frac_exc is not one of these - int, float")
@@ -129,288 +132,337 @@
         if nBinsRecord <= 0:
             err = ValueError("ERROR: nBinsRecord has to be positive.")
             logging.exception(err)
             raise err
 
         # Start the simulation.
         start_time = time.time()
-        
+
         self.N = N
+        self.frac_exc = frac_exc
+        self.frac_ext = frac_ext
         self.Ne = int(round(frac_exc * N))
         self.Ni = int(round((1 - frac_exc) * N))
         self.Nx = int(round(frac_ext * N))
         self.Nt = round(T / dt)
         self.total_time = np.arange(dt, T + dt, dt)  # Time discretized domain.
         self.Istim = np.zeros(len(self.total_time))
         self.Istim[self.total_time > T / 2] = 0
-        self.Jstim = np.sqrt(N) * np.hstack(
-            (jestim * np.ones((1, self.Ne)), jistim * np.ones((1, self.Ni)))
-        )
+        self.Jstim = np.sqrt(N) * np.hstack((jestim * np.ones((1, self.Ne)), jistim * np.ones((1, self.Ni))))
         self.maxns = round(0.05 * N * T)  # Max num of spikes (50 Hz).
         dtRecord = nBinsRecord * dt
         self.timeRecord = np.arange(dtRecord, T + dtRecord, dtRecord)
         self.Ntrec = len(self.timeRecord)
+        self.dt = dt
+        self.nBinsRecord = nBinsRecord
 
         logging.info(f"Simulating a network of {self.N} neurons.")
         logging.info(f"{self.Ne} neurons are excitatory.")
         logging.info(f"{self.Ni} neurons are inhibitory.")
         logging.info(f"The external layer, X, provides input from {self.Nx} excitatory neurons.")
         logging.info(f"The network will be simulated for {T/1000} seconds.")
 
         elapsed_time = time.time() - start_time
         logging.info(f"Time for initializing the class: {round(elapsed_time/60,2)} minutes.")
 
-    def connectivity(self, Jm, Jxm, P, Px, nJrecord0):
+    def connectivity(
+        self,
+        jee=25,
+        jie=112.5,
+        jei=-150,
+        jii=-250,
+        jex=180,
+        jix=135,
+        p_ee=0.1,
+        p_ie=0.1,
+        p_ei=0.1,
+        p_ii=0.1,
+        p_ex=0.1,
+        p_ix=0.1,
+        nJrecord0=100,
+    ):
         """
         Create connectivity matrix and arrays to record individual weights of all four connections.
-        
+
         Inputs
-        :param Jm: Mean field matrix J for recurrent connections. It contains avg value of connection for recurrent connections.
-        :type Jm: np.ndarray
-        :param Jxm: Mean field matrix Jx for feedforward connections. It contains avg value of connection for feedforward connections.
-        :type Jxm: np.ndarray
-        :param P: Matrix containing probability of connection for each pair of populations.
-        :type P: np.ndarray
-        :param Px: Matrix containing probability of connection for each pair of populations from external to recurrent.
-        :type Px: np.ndarray
+        :param jee: Unscaled coupling strength from E to E neurons. Defaults to 25.
+        :type jee: float
+        :param jie: Unscaled coupling strength from E to I neurons. Defaults to 112.5.
+        :type jie: float
+        :param jei: Unscaled coupling strength from I to E neurons. Defaults to -150.
+        :type jei: float
+        :param jii: Unscaled coupling strength from I to I neurons. Defaults to -250.
+        :type jii: float
+        :param jex: Unscaled coupling strength from X to E neurons. Defaults to 180.
+        :type jex: float
+        :param jix: Unscaled coupling strength from X to I neurons. Defaults to 135.
+        :type jix: float
+        :param p_ee: Probability of connection from E to E neurons. Defaults to 0.1.
+        :type p_ee: float
+        :param p_ie: Probability of connection from E to I neurons. Defaults to 0.1.
+        :type p_ie: float
+        :param p_ei: Probability of connection from I to E neurons. Defaults to 0.1.
+        :type p_ei: float
+        :param p_ii: Probability of connection from I to I neurons. Defaults to 0.1.
+        :type p_ii: float
+        :param p_ex: Probability of connection from X to E neurons. Defaults to 0.1.
+        :type p_ex: float
+        :param p_ix: Probability of connection from X to I neurons. Defaults to 0.1.
+        :type p_ix: float
         :param nJrecord0: Count of synaptic weights recorded. Relevant when network is plastic.
         :type nJrecord0: int
 
-        Returns (as part of `self`)
-        J : np.ndarray
-            Recurrent connectivity matrix.
-        Jx : np.ndarray
-            External feedforward connectivity matrix.
-        Jrecord_ee : np.ndarray
-            Indices of recorded EE synaptic weights.
-        Jrecord_ie : np.ndarray
-            Indices of recorded IE synaptic weights.
-        Jrecord_ei : np.ndarray
-            Indices of recorded EI synaptic weights.
-        Jrecord_ii : np.ndarray
-            Indices of recorded II synaptic weights.
-        numrecordJ_ee : int
-            Number of recorded EE synaptic weights.
-        numrecordJ_ie : int
-            Number of recorded IE synaptic weights.
-        numrecordJ_ei : int
-            Number of recorded EI synaptic weights.
-        numrecordJ_ii : int
-            Number of recorded II synaptic weights.
+        Returns as part of self.
+        :return: Recurrent connectivity matrix (J); External feedforward connectivity matrix (Jx);
+        Indices of recorded EE synaptic weights (Jrecord_ee);
+        Indices of recorded IE synaptic weights (Jrecord_ie); Indices of recorded EI synaptic weights (Jrecord_ei);
+        Indices of recorded II synaptic weights (Jrecord_ii); Number of recorded EE synaptic weights (numrecordJ_ee);
+        Number of recorded IE synaptic weights (numrecordJ_ie); Number of recorded EI synaptic weights (numrecordJ_ei);
+        Number of recorded II synaptic weights (numrecordJ_ii).
+        :rtype: tuple(np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray,  int, int, int, int)
         """
         # Test types
-        if type(Jm) not in [np.ndarray]:
-            err = TypeError("ERROR: Jm is not np.array.")
+        if not isinstance(jee, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: jee is not int nor float.")
+            logging.exception(err)
+            raise err
+        if not isinstance(jie, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: jie is not int nor float.")
+            logging.exception(err)
+            raise err
+        if not isinstance(jei, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: jei is not int nor float.")
             logging.exception(err)
             raise err
-        if type(Jxm) not in [np.ndarray]:
-            err = TypeError("ERROR: Jm is not np.array.")
+        if not isinstance(jii, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: jii is not int nor float.")
             logging.exception(err)
             raise err
-        if type(P) not in [np.ndarray]:
-            err = TypeError("ERROR: P is not np.array.")
+        if not isinstance(jex, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: jex is not int nor float.")
             logging.exception(err)
             raise err
-        if type(Px) not in [np.ndarray]:
-            err = TypeError("ERROR: Px is not np.array.")
+        if not isinstance(jix, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: jix is not int nor float.")
+            logging.exception(err)
+            raise err
+        if not isinstance(p_ee, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: p_ee is not int nor float.")
+            logging.exception(err)
+            raise err
+        if not isinstance(p_ie, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: p_ie is not int nor float.")
+            logging.exception(err)
+            raise err
+        if not isinstance(p_ei, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: p_ei is not int nor float.")
+            logging.exception(err)
+            raise err
+        if not isinstance(p_ii, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: p_ii is not int nor float.")
+            logging.exception(err)
+            raise err
+        if not isinstance(p_ex, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: p_ex is not int nor float.")
+            logging.exception(err)
+            raise err
+        if not isinstance(p_ix, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: p_ix is not int nor float.")
             logging.exception(err)
             raise err
         if not isinstance(nJrecord0, (int, np.integer)):
             err = TypeError("ERROR: nJrecord0 is not int.")
             logging.exception(err)
             raise err
         # Value tests.
-        if Jm[0,0] <= 0:
-            err = ValueError("ERROR: Jm[0,0], EE syn strength, has to be positive.")
+        if jee <= 0:
+            err = ValueError("ERROR: jee, EE syn strength, has to be positive.")
             logging.exception(err)
             raise err
-        if Jm[1,0] <= 0:
-            err = ValueError("ERROR: Jm[1,0], IE syn strength, has to be positive.")
+        if jie <= 0:
+            err = ValueError("ERROR: jie, IE syn strength, has to be positive.")
             logging.exception(err)
             raise err
-        if Jm[0,1] >= 0:
-            err = ValueError("ERROR: Jm[0,1], EI syn strength, has to be negative.")
+        if jei >= 0:
+            err = ValueError("ERROR: jei, EI syn strength, has to be negative.")
             logging.exception(err)
             raise err
-        if Jm[1,1] >= 0:
-            err = ValueError("ERROR: Jm[1,1], II syn strength, has to be negative.")
+        if jii >= 0:
+            err = ValueError("ERROR: jii, II syn strength, has to be negative.")
             logging.exception(err)
             raise err
-        if Jxm[0,0] <= 0:
-            err = ValueError("ERROR: Jxm[0,0], EX syn strength, has to be positive.")
+        if jex <= 0:
+            err = ValueError("ERROR: jex, EX syn strength, has to be positive.")
             logging.exception(err)
             raise err
-        if Jxm[1,0] <= 0:
-            err = ValueError("ERROR: Jxm[1,0], IX syn strength, has to be positive.")
+        if jix <= 0:
+            err = ValueError("ERROR: jix, IX syn strength, has to be positive.")
             logging.exception(err)
             raise err
-        if (P[0,0] > 1) | (P[0,0] < 0):
-            err = ValueError("ERROR: P[0,0], EE Prob of connection, has to be between 0 and 1.")
+        if (p_ee > 1) | (p_ee < 0):
+            err = ValueError("ERROR: p_ee, EE Prob of connection, has to be between 0 and 1.")
             logging.exception(err)
             raise err
-        if (P[1,0] > 1) | (P[1,0] < 0):
-            err = ValueError("ERROR: P[1,0], IE Prob of connection, has to be between 0 and 1.")
+        if (p_ie > 1) | (p_ie < 0):
+            err = ValueError("ERROR: p_ie, IE Prob of connection, has to be between 0 and 1.")
             logging.exception(err)
             raise err
-        if (P[0,1] > 1) | (P[0,1] < 0):
-            err = ValueError("ERROR: P[0,1], EI Prob of connection, has to be between 0 and 1.")
+        if (p_ei > 1) | (p_ei < 0):
+            err = ValueError("ERROR: p_ei, EI Prob of connection, has to be between 0 and 1.")
             logging.exception(err)
             raise err
-        if (P[1,1] > 1) | (P[1,1] < 0):
-            err = ValueError("ERROR: P[1,1], II Prob of connection, has to be between 0 and 1.")
+        if (p_ii > 1) | (p_ii < 0):
+            err = ValueError("ERROR: p_ii, II Prob of connection, has to be between 0 and 1.")
             logging.exception(err)
             raise err
-        if (Px[0,0] > 1) | (Px[0,0] < 0):
-            err = ValueError("ERROR: Px[0,0], EX Prob of connection, has to be between 0 and 1.")
+        if (p_ex > 1) | (p_ex < 0):
+            err = ValueError("ERROR: p_ex, EX Prob of connection, has to be between 0 and 1.")
             logging.exception(err)
             raise err
-        if (Px[1,0] > 1) | (Px[1,0] < 0):
-            err = ValueError("ERROR: P[0,0], IX Prob of connection, has to be between 0 and 1.")
+        if (p_ix > 1) | (p_ix < 0):
+            err = ValueError("ERROR: p_ix, IX Prob of connection, has to be between 0 and 1.")
             logging.exception(err)
             raise err
         if nJrecord0 <= 0:
             err = ValueError("ERROR: nJrecord0, number of syn weights recorded, has to be positive.")
             logging.exception(err)
             raise err
 
+        # Make defaults accessible.
+        self.jee = jee
+        self.jie = jie
+        self.jei = jei
+        self.jii = jii
+        self.jex = jex
+        self.jix = jix
+        self.p_ee = p_ee
+        self.p_ie = p_ie
+        self.p_ei = p_ei
+        self.p_ii = p_ii
+        self.p_ex = p_ex
+        self.p_ix = p_ix
+
         # Start the simulation.
         start_time = time.time()
 
+        # Recurrent net connection probabilities.
+        P = np.array([[p_ee, p_ei], [p_ie, p_ii]])
+        # Ffwd connection probs.
+        Px = np.array([[p_ex], [p_ix]])
+        # Define mean field matrices.
+        Jm = np.array([[jee, jei], [jie, jii]]) / np.sqrt(self.N)
+        Jxm = np.array([[jex], [jix]]) / np.sqrt(self.N)
+
         # Define connectivity
         self.J = np.vstack(
             (
                 np.hstack(
                     (
-                        np.array(
-                            Jm[0, 0]
-                            * np.random.binomial(1, P[0, 0], (self.Ne, self.Ne))
-                        ),
-                        np.array(
-                            Jm[0, 1]
-                            * np.random.binomial(1, P[0, 1], (self.Ne, self.Ni))
-                        ),
+                        np.array(Jm[0, 0] * np.random.binomial(1, P[0, 0], (self.Ne, self.Ne))),
+                        np.array(Jm[0, 1] * np.random.binomial(1, P[0, 1], (self.Ne, self.Ni))),
                     )
                 ),
                 np.hstack(
                     (
-                        np.array(
-                            Jm[1, 0]
-                            * np.random.binomial(1, P[1, 0], (self.Ni, self.Ne))
-                        ),
-                        np.array(
-                            Jm[1, 1]
-                            * np.random.binomial(1, P[1, 1], (self.Ni, self.Ni))
-                        ),
+                        np.array(Jm[1, 0] * np.random.binomial(1, P[1, 0], (self.Ni, self.Ne))),
+                        np.array(Jm[1, 1] * np.random.binomial(1, P[1, 1], (self.Ni, self.Ni))),
                     )
                 ),
             )
         )
 
         self.Jx = np.vstack(
             (
-                np.array(
-                    Jxm[0, 0] * np.random.binomial(1, Px[0, 0], (self.Ne, self.Nx))
-                ),
-                np.array(
-                    Jxm[1, 0] * np.random.binomial(1, Px[1, 0], (self.Ni, self.Nx))
-                ),
+                np.array(Jxm[0, 0] * np.random.binomial(1, Px[0, 0], (self.Ne, self.Nx))),
+                np.array(Jxm[1, 0] * np.random.binomial(1, Px[1, 0], (self.Ni, self.Nx))),
             )
         )
 
         logging.info(f"Connectivity matrices J and Jx were built successfully.")
 
         # Define variables to record changes in weights.
         # Synaptic weights EE to record.
         # The first row of Jrecord is the postsynaptic indices
         # The second row is the presynaptic indices
-        IIJJ_rec = np.argwhere(
-            self.J[0 : self.Ne, 0 : self.Ne]
-        )  # Find non-zero E to E weights
+        IIJJ_rec = np.argwhere(self.J[0 : self.Ne, 0 : self.Ne])  # Find non-zero E to E weights
         II = IIJJ_rec[:, 0]
         JJ = IIJJ_rec[:, 1]
-        sampled_indices = np.random.choice(
-            len(IIJJ_rec[:, 0]), size=nJrecord0, replace=False
-        )
+        sampled_indices = np.random.choice(len(IIJJ_rec[:, 0]), size=nJrecord0, replace=False)
         II = II[sampled_indices]
         JJ = JJ[sampled_indices]
         self.Jrecord_ee = np.array([II, JJ])  # Record these
         self.numrecordJ_ee = len(JJ)
 
         # Synaptic weights IE to record.
         # The first row of Jrecord is the postsynaptic indices
         # The second row is the presynaptic indices
-        IIJJ_rec = np.argwhere(
-            self.J[self.Ne : self.N, 0 : self.Ne]
-        )  # Find non-zero E to I weights
+        IIJJ_rec = np.argwhere(self.J[self.Ne : self.N, 0 : self.Ne])  # Find non-zero E to I weights
         II = IIJJ_rec[:, 0]
         JJ = IIJJ_rec[:, 1]
-        sampled_indices = np.random.choice(
-            len(IIJJ_rec[:, 0]), size=nJrecord0, replace=False
-        )
+        sampled_indices = np.random.choice(len(IIJJ_rec[:, 0]), size=nJrecord0, replace=False)
         II = II[sampled_indices]
         JJ = JJ[sampled_indices]
         self.Jrecord_ie = np.array([II + self.Ne, JJ])  # Record these
         self.numrecordJ_ie = len(JJ)
 
         # Synaptic weights EI to record.
         # The first row of Jrecord is the postsynaptic indices
         # The second row is the presynaptic indices
-        IIJJ_rec = np.argwhere(
-            self.J[0 : self.Ne, self.Ne : self.N]
-        )  # Find non-zero I to E weights
+        IIJJ_rec = np.argwhere(self.J[0 : self.Ne, self.Ne : self.N])  # Find non-zero I to E weights
         II = IIJJ_rec[:, 0]
         JJ = IIJJ_rec[:, 1]
-        sampled_indices = np.random.choice(
-            len(IIJJ_rec[:, 0]), size=nJrecord0, replace=False
-        )
+        sampled_indices = np.random.choice(len(IIJJ_rec[:, 0]), size=nJrecord0, replace=False)
         II = II[sampled_indices]
         JJ = JJ[sampled_indices]
         self.Jrecord_ei = np.array([II, JJ + self.Ne])  # Record these
         self.numrecordJ_ei = len(JJ)
 
         # Synaptic weights II to record.
         # The first row of Jrecord is the postsynaptic indices
         # The second row is the presynaptic indices
-        IIJJ_rec = np.argwhere(
-            self.J[self.Ne : self.N, self.Ne : self.N]
-        )  # Find non-zero I to I weights
+        IIJJ_rec = np.argwhere(self.J[self.Ne : self.N, self.Ne : self.N])  # Find non-zero I to I weights
         II = IIJJ_rec[:, 0]
         JJ = IIJJ_rec[:, 1]
-        sampled_indices = np.random.choice(
-            len(IIJJ_rec[:, 0]), size=nJrecord0, replace=False
-        )
+        sampled_indices = np.random.choice(len(IIJJ_rec[:, 0]), size=nJrecord0, replace=False)
         II = II[sampled_indices]
         JJ = JJ[sampled_indices]
         self.Jrecord_ii = np.array([II + self.Ne, JJ + self.Ne])  # Record these
         self.numrecordJ_ii = len(JJ)
 
         elapsed_time = time.time() - start_time
         logging.info(f"Time for building connectivity matrix: {round(elapsed_time/60,2)} minutes.")
-        
 
-    def ffwd_spikes(self, cx, rx, taujitter, T):
+    def ffwd_spikes(self, T, cx=0.1, rx=10 / 1000, taujitter=5):
         """
         Create all spike trains of the Poisson feedforward, external layer.
 
         Inputs
-        :param cx: Value of mean correlation between feedforward Poisson spike trains.
+        :param T: Total time of simulation.
+        :type T: int
+        :param cx: Value of mean correlation between feedforward Poisson spike trains. Defaults to 0.1.
         :type cx: float or int
-        :param rx: Rate of feedforward Poisson neurons in Hz.
+        :param rx: Rate of feedforward Poisson neurons in Hz. Defaults to 0.01 kHz.
         :type rx: float or int
-        :param taujitter: Spike trains are jittered by taujitter milliseconds to avoid perfect synchrony.
+        :param taujitter: Spike trains are jittered by taujitter milliseconds to avoid perfect synchrony. Defaults to 5 ms.
         :type taujitter: float or int
-        :param T: Total time of simulation.
-        :type T: int
-            
+
         Returns (as part of `self`)
-        sx : np.ndarray
-            Feedforward, Poisson spike trains recorded as spike time and neuron index.
-        nspikeX : int
-            Total number of spikes in sx.
+        :return: Feedforward, Poisson spike trains recorded as spike time and neuron index (sx);
+        Total number of spikes in sx (nspikeX).
+        :rtype: tuple(np.ndarray, int)
         """
+        # None errors.
+        if T is None:
+            err = ValueError(
+                """ERROR: T cannot be None. Pick an integer number of total simulation time.
+                A number in the order of 10^3 is a good place to start for a quick simulation.
+                """
+            )
+            logging.exception(err)
+            raise err
         # Type errors
         if not isinstance(cx, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: cx is not int nor float.")
             logging.exception(err)
             raise err
         if not isinstance(rx, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: rx is not int nor float.")
@@ -421,173 +473,168 @@
             logging.exception(err)
             raise err
         if not isinstance(T, (int, np.integer)):
             err = TypeError("ERROR: T is not int")
             logging.exception(err)
             raise err
         # Value tests.
+        if T < 1:
+            err = ValueError("ERROR: T has to be greater than 1 ms.")
+            logging.exception(err)
+            raise err
         if (cx > 1) | (cx < 0):
             err = ValueError("ERROR: cx, input corrs, have to be between 0 and 1.")
             logging.exception(err)
             raise err
         if rx <= 0:
             err = ValueError("ERROR: rx, input rate, has to be greater than 0.")
             logging.exception(err)
             raise err
         if taujitter <= 0:
             err = ValueError("ERROR: taujitter has to be greater than 0.")
             logging.exception(err)
             raise err
-        if T < 1:
-            err = ValueError("ERROR: T has to be greater than 0.")
-            logging.exception(err)
-            raise err
-        
+
         # Start the simulation.
         start_time = time.time()
 
         if cx < 1e-5:  # If uncorrelated
             self.nspikeX = np.random.poisson(self.Nx * rx * T)
             st = np.random.uniform(0, 1, (1, self.nspikeX)) * T
             self.sx = np.zeros((2, len(st[0])))
             self.sx[0, :] = np.sort(st)[0]  # spike time
-            self.sx[1, :] = np.random.randint(
-                1, self.Nx, (1, len(st[0]))
-            )  # neuron index that spiked
+            self.sx[1, :] = np.random.randint(1, self.Nx, (1, len(st[0])))  # neuron index that spiked
             logging.info(f"Uncorrelated ffwd spike trains (cx={cx} and rate={rx} kHz) were generated successfully.")
         else:  # If correlated
             rm = rx / cx  # Firing rate of mother process
             nstm = np.random.poisson(rm * T)  # Number of mother spikes
-            stm = (
-                np.random.uniform(0, 1, (nstm, 1)) * T
-            )  # spike times of mother process
+            stm = np.random.uniform(0, 1, (nstm, 1)) * T  # spike times of mother process
             maxnsx = int(T * rx * self.Nx * 1.2)  # Max num spikes
             sx = np.zeros((2, maxnsx))
             ns = 0
             for j in np.arange(1, self.Nx, 1):  # For each ffwd spike train
-                ns0 = np.random.binomial(
-                    nstm, cx
-                )  # Number of spikes for this spike train
+                ns0 = np.random.binomial(nstm, cx)  # Number of spikes for this spike train
                 st = random2.sample(list(stm[:, 0]), ns0)  # Sample spike times randomly
-                st = st + taujitter * np.random.normal(
-                    0, 1, size=len(st)
-                )  # jitter spike times
+                st = st + taujitter * np.random.normal(0, 1, size=len(st))  # jitter spike times
                 st = st[(st > 0) & (st < T)]  # Get rid of out-of-bounds times
                 ns0 = len(st)  # Re-compute spike count
                 sx[0, ns + 1 : ns + ns0 + 1] = st  # Set the spike times and indices
                 sx[1, ns + 1 : ns + ns0 + 1] = j
                 ns = ns + ns0
 
             # Get rid of padded zeros
             sx = sx[:, sx[0, :] > 0]
 
             # Sort by spike time
             I = np.argsort(sx[0, :])
             self.sx = sx[:, I]
             self.nspikeX = len(sx[0, :])
-            
+
             logging.info(f"Correlated ffwd spike trains (cx={cx} and rate={rx} kHz) were generated successfully.")
 
         elapsed_time = time.time() - start_time
         logging.info(f"Time for generating feedforward Poisson spike trains: {round(elapsed_time/60,2)} minutes.")
 
-
     def simulate(
         self,
-        Cm,
-        gL,
-        VT,
-        Vre,
-        Vth,
-        EL,
-        DeltaT,
-        taue,
-        taui,
-        taux,
-        tauSTDP,
-        numrecord,
-        eta_ee_hebb,
-        Jmax_ee,
-        eta_ee_koh,
-        beta,
-        eta_ie_homeo,
-        alpha_ie,
-        eta_ie_hebb,
-        Jmax_ie_hebb,
-        eta_ei,
-        alpha_ei,
-        eta_ii,
-        alpha_ii,
-        dt,
-        nBinsRecord,
+        Cm=1,
+        gL=1 / 15,
+        VT=-55,
+        Vre=-75,
+        Vth=-50,
+        EL=-72,
+        DeltaT=1,
+        taue=8,
+        taui=4,
+        taux=10,
+        tauSTDP=200,
+        numrecord=100,
+        eta_ee_hebb=0,
+        jmax_ee=30,
+        eta_ee_koh=0,
+        beta=2,
+        eta_ie_homeo=0,
+        rho_ie=0.020,
+        eta_ie_hebb=0,
+        jmax_ie_hebb=125,
+        eta_ei=0,
+        rho_ei=0.010,
+        eta_ii=0,
+        rho_ii=0.020,
     ):
         """
         Execute Network simulation.
 
         Inputs
-        :param Cm: Membrane capacitance.
+        :param Cm: Membrane capacitance. Defaults to 1.
         :type Cm: float or int
-        :param gL: Leak conductance.
+        :param gL: Leak conductance. Defaults to 1/15.
         :type gL: float or int
-        :param VT: Threshold in EIF neuron.
+        :param VT: Threshold in EIF neuron. Defaults to -55.
         :type VT: float or int
-        :param Vre: Reset voltage.
+        :param Vre: Reset voltage. Defaults to -75.
         :type Vre: float or int
-        :param Vth: Hard threshold that determines when a spike happened.
+        :param Vth: Hard threshold that determines when a spike happened. Defaults to -50.
         :type Vth: float or int
-        :param EL: Resting potential.
+        :param EL: Resting potential. Defaults to -72.
         :type EL: float or int
-        :param DeltaT: EIF neuron parameter. Determines the shape of the rise to spike.
+        :param DeltaT: EIF neuron parameter. Determines the shape of the rise to spike. Defaults to 1.
         :type DeltaT: float or int
-        :param taue: Timescale of excitatory neurons in milliseconds.
+        :param taue: Timescale of excitatory neurons in milliseconds. Defaults to 8 ms.
         :type taue: float or int
-        :param taui: Timescale of inhibitory neurons in milliseconds.
+        :param taui: Timescale of inhibitory neurons in milliseconds. Defaults to 4 ms.
         :type taui: float or int
-        :param taux: Timescale of external neurons in milliseconds.
+        :param taux: Timescale of external neurons in milliseconds. Defaults to 10 ms.
         :type taux: float or int
-        :param tauSTDP: Timescale of eligibility trace used for STDP.
+        :param tauSTDP: Timescale of eligibility trace used for STDP. Defaults to 200 ms.
         :type tauSTDP: float or int
-        :param numrecord: Number of neurons to record currents and voltage from.
-        :type numrecord: int 
-        :param eta_ee_hebb: Learning rate of EE Hebbian STDP.
+        :param numrecord: Number of neurons to record currents and voltage from. Defaults to 100.
+        :type numrecord: int
+        :param eta_ee_hebb: Learning rate of EE Hebbian STDP. Defaults to 0.
+        Pick a value in the approximate order of 10^-3 or lower as a start point.
         :type eta_ee_hebb: float or int
-        :param Jmax_ee: Hard constraint on EE Hebbian STDP.
+        :param Jmax_ee: Hard constraint on EE Hebbian STDP. Defaults to 30/np.sqrt(N).
         :type Jmax_ee: float or int
-        :param eta_ee_koh: Learning rate of Kohonen STDP.
+        :param eta_ee_koh: Learning rate of Kohonen STDP. Defaults to 0.
+        Pick a value in the approximate order of 10^-3 or lower as a start point.
         :type eta_ee_koh: float or int
-        :param beta: Parameter for Kohonen STDP.
+        :param beta: Parameter for Kohonen STDP. Defaults to 2/np.sqrt(N).
         :type beta: float or int
-        :param eta_ie_homeo: Learning rate of iSTDP.
+        :param eta_ie_homeo: Learning rate of iSTDP. Defaults to 0.
+        Pick a value in the approximate order of 10^-3 or lower as a start point.
         :type eta_ie_homeo: float or int
-        :param alpha_ie: Parameter that determines target rate in iSTDP.
-        :type alpha_ie: float or int
-        :param eta_ie_hebb: Learning rate of IE Hebbian STDP.
+        :param rho_ie: Target rate of I neurons in iSTDP. Defaults to 0.020 kHz.
+        :type rho_ie: float or int
+        :param eta_ie_hebb: Learning rate of IE Hebbian STDP. Defaults to 0.
+        Pick a value in the approximate order of 10^-3 as a start point.
         :type eta_ie_hebb: float or int
-        :param Jmax_ie_hebb: Hard constraint on IE Hebbian STDP.
+        :param Jmax_ie_hebb: Hard constraint on IE Hebbian STDP. Defaults to 125/np.sqrt(N).
         :type Jmax_ie_hebb: float or int
-        :param eta_ei: Learning rate of iSTDP.
+        :param eta_ei: Learning rate of iSTDP. Defaults to 0.
+        Pick a value in the approximate order of 10^-3 or lower as a start point.
         :type eta_ei: float or int
-        :param alpha_ei: Parameter that determines target rate in iSTDP.
-        :type alpha_ei: float or int
-        :param eta_ii: Learning rate of iSTDP.
+        :param rho_ei: Parameter that determines target rate in iSTDP. Defaults to 0.010 kHz.
+        :type rho_ei: float or int
+        :param eta_ii: Learning rate of iSTDP. Defaults to 0.
+        Pick a value in the approximate order of 10^-3 or lower as a start point.
         :type eta_ii: float or int
-        :param alpha_ii: Parameter that determines target rate in iSTDP.
-        :type alpha_ii: float or int
-        :param dt: Time bin size in ms.
-        :type dt: float or int
-        :param nBinsRecord: Number of bins to record average and record over.
-        :type nBinsRecord: int 
+        :param rho_ii: Parameter that determines target rate in iSTDP. Defaults to 0.020 kHz.
+        :type rho_ii: float or int
 
         Returns
-        :return: A tuple containing spike train of all neurons in recurrent neural network (s); spike train of all feedforward neurons (sx), 
-        matrices of neurons (rows) by time bins (cols) for EE, EI, IE, and II recorded weights (JRec_ee, JRec_ie, JRec_ei, JRec_ii); 
+        :return: A tuple containing spike train of all neurons in recurrent neural network (s);
+        spike train of all feedforward neurons (sx),
+        matrices of neurons (rows) by time bins (cols) for EE, EI, IE,
+        and II recorded weights (JRec_ee, JRec_ie, JRec_ei, JRec_ii);
         matrices of neurons (rows) by time bins (cols) for E, I, and X input currents (IeRec, IiRec, IxRec);
-        matrix of neurons (rows) by time bins (cols) for recurrent network voltages (VRec); and discretized recorded time domain (timeRecord).
-        :rtype: (np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray)
-            
+        matrix of neurons (rows) by time bins (cols) for recurrent network voltages (VRec);
+        and discretized recorded time domain (timeRecord).
+        :rtype: tuple(np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray,
+        np.ndarray, np.ndarray, np.ndarray, np.ndarray)
+
         """
         # Type errors.
         if not isinstance(Cm, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: Cm is not int nor float.")
             logging.exception(err)
             raise err
         if not isinstance(gL, (float, np.floating, int, np.integer)):
@@ -630,64 +677,56 @@
             err = TypeError("ERROR: tauSTDP is not int nor float.")
             logging.exception(err)
             raise err
         if not isinstance(eta_ee_hebb, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: eta_ee_hebb is not int,float.")
             logging.exception(err)
             raise err
-        if not isinstance(Jmax_ee, (float, np.floating, int, np.integer)):
-            err = TypeError("ERROR: Jmax_ee is not int,float.")
+        if not isinstance(jmax_ee, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: jmax_ee is not int,float.")
             logging.exception(err)
             raise err
         if not isinstance(eta_ee_koh, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: eta_ee_koh is not int,float.")
             logging.exception(err)
             raise err
         if not isinstance(beta, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: beta is not int,float.")
             logging.exception(err)
             raise err
         if not isinstance(eta_ie_homeo, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: eta_ie_homeo is not int,float.")
             logging.exception(err)
             raise err
-        if not isinstance(alpha_ie, (float, np.floating, int, np.integer)):
-            err = TypeError("ERROR: alpha_ie is not int,float.")
+        if not isinstance(rho_ie, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: rho_ie is not int,float.")
             logging.exception(err)
             raise err
         if not isinstance(eta_ie_hebb, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: eta_ie_hebb is not int,float.")
             logging.exception(err)
             raise err
-        if not isinstance(Jmax_ie_hebb, (float, np.floating, int, np.integer)):
-            err = TypeError("ERROR: Jmax_ie_hebb is not int,float.")
+        if not isinstance(jmax_ie_hebb, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: jmax_ie_hebb is not int,float.")
             logging.exception(err)
             raise err
         if not isinstance(eta_ei, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: eta_ei is not int,float.")
             logging.exception(err)
             raise err
-        if not isinstance(alpha_ei, (float, np.floating, int, np.integer)):
-            err = TypeError("ERROR: alpha_ei is not int,float.")
+        if not isinstance(rho_ei, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: rho_ei is not int,float.")
             logging.exception(err)
             raise err
         if not isinstance(eta_ii, (float, np.floating, int, np.integer)):
             err = TypeError("ERROR: eta_ii is not int,float.")
             logging.exception(err)
             raise err
-        if not isinstance(alpha_ii, (float, np.floating, int, np.integer)):
-            err = TypeError("ERROR: alpha_ii is not int,float.")
-            logging.exception(err)
-            raise err
-        if not isinstance(dt, (float, np.floating, int, np.integer)):
-            err = TypeError("ERROR: dt is not int,float.")
-            logging.exception(err)
-            raise err
-        if not isinstance(nBinsRecord, (int, np.integer)):
-            err = TypeError("ERROR: nBinsRecord is not int.")
+        if not isinstance(rho_ii, (float, np.floating, int, np.integer)):
+            err = TypeError("ERROR: rho_ii is not int,float.")
             logging.exception(err)
             raise err
         # Value tests.
         if Cm <= 0:
             err = ValueError("ERROR: Cm has to be greater than zero.")
             logging.exception(err)
             raise err
@@ -735,68 +774,85 @@
             err = ValueError("ERROR: numrecord has to be greater than zero.")
             logging.exception(err)
             raise err
         if eta_ee_hebb < 0:
             err = ValueError("ERROR: eta_ee_hebb has to be greater than or equal to zero.")
             logging.exception(err)
             raise err
-        if Jmax_ee < 0:
-            err = ValueError("ERROR: Jmax_ee has to be greater than or equal to zero.")
+        if jmax_ee <= 0:
+            err = ValueError("ERROR: Jmax_ee has to be greater than zero.")
             logging.exception(err)
             raise err
         if eta_ee_koh < 0:
             err = ValueError("ERROR: eta_ee_koh has to be greater than or equal to zero.")
             logging.exception(err)
             raise err
-        if beta < 0:
-            err = ValueError("ERROR: beta has to be greater than or equal to zero.")
+        if beta <= 0:
+            err = ValueError("ERROR: beta has to be greater than zero.")
             logging.exception(err)
             raise err
         if eta_ie_homeo < 0:
             err = ValueError("ERROR: eta_ie_homeo has to be greater than or equal to zero.")
             logging.exception(err)
             raise err
-        if alpha_ie < 0:
-            err = ValueError("ERROR: alpha_ie has to be greater than or equal to zero.")
+        if rho_ie <= 0:
+            err = ValueError("ERROR: rho_ie has to be greater than zero.")
             logging.exception(err)
             raise err
         if eta_ie_hebb < 0:
             err = ValueError("ERROR: eta_ie_hebb has to be greater than or equal to zero.")
             logging.exception(err)
             raise err
-        if Jmax_ie_hebb < 0:
-            err = ValueError("ERROR: Jmax_ie_hebb has to be greater than or equal to zero.")
+        if jmax_ie_hebb <= 0:
+            err = ValueError("ERROR: jmax_ie_hebb has to be greater than zero.")
             logging.exception(err)
             raise err
-        if eta_ei > 0:
+        if eta_ei < 0:
             err = ValueError("ERROR: eta_ei has to be greater than or equal to zero.")
             logging.exception(err)
             raise err
-        if alpha_ei <= 0:
-            err = ValueError("ERROR: alpha_ei has to be greater than or equal to zero.")
+        if rho_ei <= 0:
+            err = ValueError("ERROR: rho_ei has to be greater than zero.")
             logging.exception(err)
             raise err
-        if eta_ii > 0:
+        if eta_ii < 0:
             err = ValueError("ERROR: eta_ii has to be greater than or equal to zero.")
             logging.exception(err)
             raise err
-        if alpha_ii <= 0:
-            err = ValueError("ERROR: alpha_ii has to be greater than or equal to zero.")
+        if rho_ii <= 0:
+            err = ValueError("ERROR: rho_ii has to be greater than zero.")
             logging.exception(err)
             raise err
-        if  dt <= 0:
-            err = ValueError("ERROR: dt has to be greater than zero.")
+        # We cannot allow for two plasticity rules to act on the same synapse type at the same time.
+        if (eta_ee_hebb != 0) & (eta_ee_koh != 0):
+            err = ValueError("ERROR: You cannot have both Kohonen and Hebb STDP's at the same time on EE connections!")
             logging.exception(err)
             raise err
-        if nBinsRecord <= 0:
-            err = ValueError("ERROR: nBinsRecord has to be greater than zero.")
+        if (eta_ie_hebb != 0) & (eta_ie_homeo != 0):
+            err = ValueError(
+                "ERROR: You cannot have both Homeostatic and Hebb STDP's at the same time on IE connections!"
+            )
             logging.exception(err)
             raise err
 
+        # Make defaults accessible.
+        self.tauSTDP = tauSTDP
+        self.beta = beta
+        self.jmax_ee = jmax_ee
+        self.jmax_ie_hebb = jmax_ie_hebb
         # Initialize some variables
+        alpha_ie = 2 * rho_ie * tauSTDP
+        alpha_ei = 2 * rho_ei * tauSTDP
+        alpha_ii = 2 * rho_ii * tauSTDP
+        beta = beta / np.sqrt(self.N)
+        Jmax_ee = jmax_ee / np.sqrt(self.N)
+        Jmax_ie_hebb = jmax_ie_hebb / np.sqrt(self.N)
+        Jnorm_ie = 112.5 / np.sqrt(self.N)
+        Jnorm_ei = -150 / np.sqrt(self.N)
+        Jnorm_ii = -250 / np.sqrt(self.N)
         # Random initial voltages
         V0 = np.random.uniform(0, 1, (1, self.N)) * (VT - Vre) + Vre
         V = V0
         # Initialize current vectors.
         Ie = np.zeros((1, self.N))
         Ii = np.zeros((1, self.N))
         Ix = np.zeros((1, self.N))
@@ -809,27 +865,21 @@
                     random2.sample(list(np.arange(0, self.Ne)), numrecord),
                     random2.sample(list(np.arange(self.Ne, self.N)), numrecord),
                 ]
             ]
         )
         Ierecord = np.sort(Irecord[0, 0]).astype(int)
         Iirecord = np.sort(Irecord[0, 1]).astype(int)
-        Ixrecord = np.sort(random2.sample(list(np.arange(0, self.Ne)), numrecord)).astype(
-            int
-        )
+        Ixrecord = np.sort(random2.sample(list(np.arange(0, self.Ne)), numrecord)).astype(int)
         Vrecord = (
             np.sort(
                 [
                     [
-                        random2.sample(
-                            list(np.arange(0, self.Ne)), int(round(numrecord / 2))
-                        ),
-                        random2.sample(
-                            list(np.arange(self.Ne, self.N)), int(round(numrecord / 2))
-                        ),
+                        random2.sample(list(np.arange(0, self.Ne)), int(round(numrecord / 2))),
+                        random2.sample(list(np.arange(self.Ne, self.N)), int(round(numrecord / 2))),
                     ]
                 ]
             )[0]
             .reshape(1, numrecord)
             .astype(int)[0]
         )
         del Irecord
@@ -844,15 +894,14 @@
         JRec_ii = np.zeros((self.numrecordJ_ii, self.Ntrec))
         # Initial spike related variables.
         iFspike = 0
         # s(0,:) are the spike times
         # s(1,:) are the associated neuron indices
         s = np.zeros((2, self.maxns))
         nspike = 0
-        TooManySpikes = 0
 
         logging.info(f"We will record currents and membrane potential from {numrecord} E and {numrecord} I neurons.")
 
         # If there is EE Hebbian plasticity
         if eta_ee_hebb != 0:
             logging.info("EE connections will evolve according to Hebbian STDP.")
             logging.info(f"We will record {self.numrecordJ_ee} plastic EE weights.")
@@ -878,48 +927,38 @@
             logging.info(f"We will record {self.numrecordJ_ii} plastic II weights.")
 
         # Start the simulation.
         start_time = time.time()
 
         for i in range(len(self.total_time)):
             # Propagate ffwd spikes
-            while (self.sx[0, iFspike] <= self.total_time[i]) & (
-                iFspike < self.nspikeX - 1
-            ):
+            while (self.sx[0, iFspike] <= self.total_time[i]) & (iFspike < self.nspikeX - 1):
                 jpre = int(self.sx[1, iFspike])
                 Ix += self.Jx[:, jpre] / taux
                 iFspike += 1
 
             # Euler update to V
             V += (
-                dt
+                self.dt
                 / Cm
-                * (
-                    self.Istim[i] * self.Jstim
-                    + Ie
-                    + Ii
-                    + Ix
-                    + gL * (EL - V)
-                    + gL * DeltaT * np.exp((V - VT) / DeltaT)
-                )
+                * (self.Istim[i] * self.Jstim + Ie + Ii + Ix + gL * (EL - V) + gL * DeltaT * np.exp((V - VT) / DeltaT))
             )
 
             # Find which neurons spiked
             Ispike = np.argwhere(V >= Vth)[:, 1]
 
             # If there are spikes
             if len(Ispike) != 0:
-
                 # Store spike times and neuron indices
                 if nspike + len(Ispike) <= self.maxns:
                     s[0, nspike + 1 : nspike + len(Ispike) + 1] = self.total_time[i]
                     s[1, nspike + 1 : nspike + len(Ispike) + 1] = Ispike
                 else:
-                    TooManySpikes = 1
-                    break
+                    logging.error("Stopped simulation. Too many spikes.")
+                    sys.exit(1)
 
                 # Update synaptic currents
                 Ie += np.sum(self.J[:, Ispike[Ispike <= self.Ne]], 1) / taue
                 Ii += np.sum(self.J[:, Ispike[Ispike > self.Ne]], 1) / taui
 
                 # If there is EE Hebbian plasticity
                 if eta_ee_hebb != 0:
@@ -942,48 +981,42 @@
                 # If there is EE Kohonen plasticity
                 if eta_ee_koh != 0:
                     # Update synaptic weights according to plasticity rules
                     # E to E after a pre spike
                     self.J[0 : self.Ne, Ispike[Ispike <= self.Ne]] += np.tile(
                         beta * eta_ee_koh * (x[0, 0 : self.Ne]),
                         (np.count_nonzero(Ispike <= self.Ne), 1),
-                    ).transpose() * (
-                        self.J[0 : self.Ne, Ispike[Ispike <= self.Ne]] != 0
-                    )
+                    ).transpose() * (self.J[0 : self.Ne, Ispike[Ispike <= self.Ne]] != 0)
                     # E to E after a post spike
                     self.J[Ispike[Ispike < self.Ne], 0 : self.Ne] -= (
                         eta_ee_koh * self.J[Ispike[Ispike < self.Ne], 0 : self.Ne]
                     )
 
                 # If there is IE *Homeo* plasticity
                 if eta_ie_homeo != 0:
                     # Update synaptic weights according to plasticity rules
                     # E to I after a pre spike
                     self.J[self.Ne : self.N, Ispike[Ispike <= self.Ne]] -= np.tile(
-                        eta_ie_homeo * (x[0, self.Ne : self.N] - alpha_ie),
+                        eta_ie_homeo / Jnorm_ie * (x[0, self.Ne : self.N] - alpha_ie),
                         (np.count_nonzero(Ispike <= self.Ne), 1),
-                    ).transpose() * (
-                        self.J[self.Ne : self.N, Ispike[Ispike <= self.Ne]]
-                    )
+                    ).transpose() * (self.J[self.Ne : self.N, Ispike[Ispike <= self.Ne]])
                     # E to I after a post spike
                     self.J[Ispike[Ispike > self.Ne], 0 : self.Ne] -= np.tile(
-                        eta_ie_homeo * x[0, 0 : self.Ne].transpose(),
+                        eta_ie_homeo / Jnorm_ie * x[0, 0 : self.Ne].transpose(),
                         (np.count_nonzero(Ispike > self.Ne), 1),
                     ) * (self.J[Ispike[Ispike > self.Ne], 0 : self.Ne])
 
                 # If there is IE *Hebbian* plasticity
                 if eta_ie_hebb != 0:
                     # Update synaptic weights according to plasticity rules
                     # E to I after a pre spike
                     self.J[self.Ne : self.N, Ispike[Ispike <= self.Ne]] -= np.tile(
                         eta_ie_hebb * (x[0, self.Ne : self.N]),
                         (np.count_nonzero(Ispike <= self.Ne), 1),
-                    ).transpose() * (
-                        self.J[self.Ne : self.N, Ispike[Ispike <= self.Ne]] != 0
-                    )
+                    ).transpose() * (self.J[self.Ne : self.N, Ispike[Ispike <= self.Ne]] != 0)
                     # E to I after a post spike
                     self.J[Ispike[Ispike > self.Ne], 0 : self.Ne] += (
                         np.tile(
                             eta_ie_hebb * x[0, 0 : self.Ne].transpose(),
                             (np.count_nonzero(Ispike > self.Ne), 1),
                         )
                         * Jmax_ie_hebb
@@ -991,81 +1024,79 @@
                     )
 
                 # If there is EI plasticity
                 if eta_ei != 0:
                     # Update synaptic weights according to plasticity rules
                     # I to E after an I spike
                     self.J[0 : self.Ne, Ispike[Ispike >= self.Ne]] -= np.tile(
-                        eta_ei * (x[0, 0 : self.Ne] - alpha_ei),
+                        eta_ei / Jnorm_ei * (x[0, 0 : self.Ne] - alpha_ei),
                         (np.count_nonzero(Ispike >= self.Ne), 1),
                     ).transpose() * (self.J[0 : self.Ne, Ispike[Ispike >= self.Ne]])
                     # I to E after an E spike
                     self.J[Ispike[Ispike < self.Ne], self.Ne : self.N] -= np.tile(
-                        eta_ei * x[0, self.Ne : self.N].transpose(),
+                        eta_ei / Jnorm_ei * x[0, self.Ne : self.N].transpose(),
                         (np.count_nonzero(Ispike < self.Ne), 1),
                     ) * (self.J[Ispike[Ispike < self.Ne], self.Ne : self.N])
 
                 # If there is II plasticity
                 if eta_ii != 0:
                     # Update synaptic weights according to plasticity rules
                     # I to E after an I spike
                     self.J[self.Ne : self.N, Ispike[Ispike >= self.Ne]] -= np.tile(
-                        eta_ii * (x[0, self.Ne : self.N] - alpha_ii),
+                        eta_ii / Jnorm_ii * (x[0, self.Ne : self.N] - alpha_ii),
                         (np.count_nonzero(Ispike >= self.Ne), 1),
-                    ).transpose() * (
-                        self.J[self.Ne : self.N, Ispike[Ispike >= self.Ne]]
-                    )
+                    ).transpose() * (self.J[self.Ne : self.N, Ispike[Ispike >= self.Ne]])
                     # I to E after an E spike
                     self.J[Ispike[Ispike > self.Ne], self.Ne : self.N] -= np.tile(
-                        eta_ii * x[0, self.Ne : self.N].transpose(),
+                        eta_ii / Jnorm_ii * x[0, self.Ne : self.N].transpose(),
                         (np.count_nonzero(Ispike > self.Ne), 1),
                     ) * (self.J[Ispike[Ispike > self.Ne], self.Ne : self.N])
 
                 # Update rate estimates for plasticity rules
                 x[0, Ispike] += 1
 
                 # Update cumulative number of spikes
                 nspike += len(Ispike)
 
             # Euler update to synaptic currents
-            Ie -= dt * Ie / taue
-            Ii -= dt * Ii / taui
-            Ix -= dt * Ix / taux
+            Ie -= self.dt * Ie / taue
+            Ii -= self.dt * Ii / taui
+            Ix -= self.dt * Ix / taux
 
             # Update time-dependent firing rates for plasticity
-            x[0 : self.Ne] -= dt * x[0 : self.Ne] / tauSTDP
-            x[self.Ne : self.N] -= dt * x[self.Ne : self.N] / tauSTDP
+            x[0 : self.Ne] -= self.dt * x[0 : self.Ne] / tauSTDP
+            x[self.Ne : self.N] -= self.dt * x[self.Ne : self.N] / tauSTDP
 
             # This makes plots of V(t) look better.
             # All action potentials reach Vth exactly.
             # This has no real effect on the network sims
             V[0, Ispike] = Vth
 
             # Store recorded variables
-            ii = int(math.floor(i / nBinsRecord))
+            ii = int(math.floor(i / self.nBinsRecord))
             IeRec[:, ii] += Ie[0, Ierecord]
             IiRec[:, ii] += Ii[0, Iirecord]
             IxRec[:, ii] += Ix[0, Ixrecord]
             VRec[:, ii] += V[0, Vrecord]
             JRec_ee[:, ii] += self.J[self.Jrecord_ee[0, :], self.Jrecord_ee[1, :]]
             JRec_ie[:, ii] += self.J[self.Jrecord_ie[0, :], self.Jrecord_ie[1, :]]
             JRec_ei[:, ii] += self.J[self.Jrecord_ei[0, :], self.Jrecord_ei[1, :]]
             JRec_ii[:, ii] += self.J[self.Jrecord_ii[0, :], self.Jrecord_ii[1, :]]
 
             # Reset mem pot.
             V[0, Ispike] = Vre
 
-        IeRec = IeRec / nBinsRecord  # Normalize recorded variables by # bins
-        IiRec = IiRec / nBinsRecord
-        IxRec = IxRec / nBinsRecord
-        VRec = VRec / nBinsRecord
-        JRec_ee = JRec_ee * np.sqrt(self.N) / nBinsRecord
-        JRec_ie = JRec_ie * np.sqrt(self.N) / nBinsRecord
-        JRec_ei = JRec_ei * np.sqrt(self.N) / nBinsRecord
-        JRec_ii = JRec_ii * np.sqrt(self.N) / nBinsRecord
+        IeRec = IeRec / self.nBinsRecord  # Normalize recorded variables by # bins
+        IiRec = IiRec / self.nBinsRecord
+        IxRec = IxRec / self.nBinsRecord
+        VRec = VRec / self.nBinsRecord
+        JRec_ee = JRec_ee * np.sqrt(self.N) / self.nBinsRecord
+        JRec_ie = JRec_ie * np.sqrt(self.N) / self.nBinsRecord
+        JRec_ei = JRec_ei * np.sqrt(self.N) / self.nBinsRecord
+        JRec_ii = JRec_ii * np.sqrt(self.N) / self.nBinsRecord
 
         s = s[:, 0:nspike]  # Get rid of padding in s
 
         logging.info(f"The plastic balanced network has been simulated successfully.")
 
         elapsed_time = time.time() - start_time
         logging.info(f"Time for simulation: {round(elapsed_time/60,2)} minutes.")
@@ -1079,7 +1110,139 @@
             JRec_ii,
             IeRec,
             IiRec,
             IxRec,
             VRec,
             self.timeRecord,
         )
+
+
+# %%
+
+
+def compute_firing_rate(s, T, N, frac_exc=0.8, dtRate=10, window_size=10):
+    """
+    Calculate the mean firing rate of E and I populations as a function of time.
+    Inputs
+    :param s: Matrix of covariances or correlations.
+    :type s: np.ndarray
+    :param T: Total time of simulation.
+    :type T: int
+    :param N: Total number of neurons.
+    :type N: int
+    :param frac_exc: Fraction of E neurons. Defaults to 0.8.
+    :type frac_exc: float
+    :param dtRate: Size of time bin to count spikes over. Defaults to 10 ms.
+    :type dtRate: int
+    :param windowsize: Size of window for moving average. Defaults to 10 bins.
+    :type windowsize: int
+
+    Returns
+    :return: Time varying firing rate of E and I neurons, respectively (eRateT, iRateT).
+    :rtype: tuple(np.ndarray,np.ndarray)
+    """
+    timeVector = np.arange(dtRate, T + dtRate, dtRate) / 1000
+
+    hist, bin_edges = np.histogram(s[0, s[1, :] < frac_exc * N], bins=len(timeVector))
+    eRateT = hist / (dtRate * frac_exc * N) * 1000
+    hist, bin_edges = np.histogram(s[0, s[1, :] >= frac_exc * N], bins=len(timeVector))
+    iRateT = hist / (dtRate * (1 - frac_exc) * N) * 1000
+
+    # Smooth rates. We multiplied by 1000 to get them in units of Hz.
+    eRateT = np.convolve(eRateT, np.ones(window_size) / window_size, mode="same")
+    iRateT = np.convolve(iRateT, np.ones(window_size) / window_size, mode="same")
+
+    return eRateT, iRateT, timeVector
+
+
+# %%
+
+
+def spike_count_cov(s, N, T1, T2, winsize=250):
+    """
+    Compute NxN spike count covariance matrix.
+    s is a 2x(ns) matrix where ns is the number of spikes
+    s(0,:) lists spike times
+    and s(1,:) lists corresponding neuron indices
+    Neuron indices are assumed to go from 0 to N-1
+
+    Spikes are counts starting at time T1 and ending at
+    time T2.
+
+    winsize is the window size over which spikes are counted,
+    so winsize is assumed to be much smaller than T2-T1
+
+    Inputs
+    :param s: Spike trains of all neurons.
+    :type s: np.ndarray
+    :param N: Total number of neurons
+    :type N: int
+    :param T1: Start time to count spikes for covariance calculation.
+    :type T1: float or int
+    :param T2: End time to count spikes for covariance calculation.
+    :type T2: float or int
+    :param winsize: Time window over which spikes are counted. Defaults to 250 ms.
+    :type winsize: int
+
+    Returns (as part of `self`)
+    :return C: Full spike count covariance matrix.
+    :rtype C: np.ndarray
+    """
+    #   Count only spikes between T1, T2
+    s1 = s[:, (s[0, :] <= T2) & (s[1, :] >= T1)]
+
+    #   Count only for neurons between 0, N
+    s1 = s[:, (s[1, :] < N) & (s[1, :] >= 0)]
+
+    #   Edges for histogram
+    edgest = np.arange(T1, T2, winsize)
+    edgesi = np.arange(0, N + 1)
+
+    #   Get 2D histogram of spike indices and times
+    counts, xedges, yedges = np.histogram2d(s1[0, :], s1[1, :], bins=(edgest, edgesi))
+
+    #   Compute and return covariance N x N matrix
+    return np.array(np.cov(counts.transpose()))
+
+
+def cov2corr(cov):
+    """convert covariance matrix to correlation matrix
+
+    Inputs
+    :param cov: Covariance matrix.
+    :type cov: np.ndarray
+
+    Returns (as part of `self`)
+    :return corr: Full spike count correlation matrix.
+    :rtype corr: np.ndarray
+    """
+    cov = np.asanyarray(cov)
+    std_ = np.sqrt(np.diag(cov))
+    corr = cov / np.outer(std_, std_)
+    return corr
+
+
+def average_cov_corr_over_subpops(C, N, frac_exc=0.8):
+    """
+    Average covariances or correlations over subpopulations.
+    Inputs
+    :param C: Matrix of covariances or correlations.
+    :type C: np.ndarray
+    :param N: Total number of neurons.
+    :type N: int
+    :param frac_exc: Fraction of E neurons. Defaults to 0.8.
+    :type frac_exc: float
+
+    Returns
+    :return mC: Mean spike count covariance matrix.
+    :rtype mC: np.ndarray
+    """
+    # Get mean spike count covariances over each sub-pop
+    II, JJ = np.meshgrid(np.arange(0, N), np.arange(0, N))
+    mCee = np.nanmean(C[(II < frac_exc * N) & (JJ < II)])
+    mCei = np.nanmean(C[(II < frac_exc * N) & (JJ >= frac_exc * N)])
+    mCii = np.nanmean(C[(II > frac_exc * N) & (JJ > II)])
+
+    # Mean-field spike count cov matrix
+    # Compare this to the theoretical prediction
+    mC = [[mCee, mCei], [mCei, mCii]]
+    return mC
```

