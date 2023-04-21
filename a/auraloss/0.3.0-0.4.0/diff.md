# Comparing `tmp/auraloss-0.3.0.tar.gz` & `tmp/auraloss-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/auraloss/auraloss/dist/.tmp-me2ubsvj/auraloss-0.3.0.tar", last modified: Mon Jan  9 19:58:09 2023, max compression
+gzip compressed data, was "/home/runner/work/auraloss/auraloss/dist/.tmp-1ahxaisi/auraloss-0.4.0.tar", last modified: Fri Apr 21 09:21:30 2023, max compression
```

## Comparing `auraloss-0.3.0.tar` & `auraloss-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 19:58:09.000000 auraloss-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-09 19:57:54.000000 auraloss-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-01-09 19:58:09.000000 auraloss-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-01-09 19:57:54.000000 auraloss-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 19:58:09.000000 auraloss-0.3.0/auraloss/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-09 19:57:54.000000 auraloss-0.3.0/auraloss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18615 2023-01-09 19:57:54.000000 auraloss-0.3.0/auraloss/freq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-01-09 19:57:54.000000 auraloss-0.3.0/auraloss/perceptual.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-01-09 19:57:54.000000 auraloss-0.3.0/auraloss/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-01-09 19:57:54.000000 auraloss-0.3.0/auraloss/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-09 19:57:54.000000 auraloss-0.3.0/auraloss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 19:58:09.000000 auraloss-0.3.0/auraloss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-01-09 19:58:09.000000 auraloss-0.3.0/auraloss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-09 19:58:09.000000 auraloss-0.3.0/auraloss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 19:58:09.000000 auraloss-0.3.0/auraloss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-09 19:58:09.000000 auraloss-0.3.0/auraloss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-09 19:58:09.000000 auraloss-0.3.0/auraloss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-01-09 19:57:54.000000 auraloss-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 19:58:09.000000 auraloss-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-01-09 19:57:54.000000 auraloss-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:21:30.000000 auraloss-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 09:21:18.000000 auraloss-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-04-21 09:21:30.000000 auraloss-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-21 09:21:18.000000 auraloss-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:21:30.000000 auraloss-0.4.0/auraloss/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 09:21:18.000000 auraloss-0.4.0/auraloss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21505 2023-04-21 09:21:18.000000 auraloss-0.4.0/auraloss/freq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-04-21 09:21:18.000000 auraloss-0.4.0/auraloss/perceptual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-21 09:21:18.000000 auraloss-0.4.0/auraloss/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-21 09:21:18.000000 auraloss-0.4.0/auraloss/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-21 09:21:18.000000 auraloss-0.4.0/auraloss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:21:30.000000 auraloss-0.4.0/auraloss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-04-21 09:21:30.000000 auraloss-0.4.0/auraloss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-21 09:21:30.000000 auraloss-0.4.0/auraloss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:21:30.000000 auraloss-0.4.0/auraloss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 09:21:30.000000 auraloss-0.4.0/auraloss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 09:21:30.000000 auraloss-0.4.0/auraloss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-21 09:21:18.000000 auraloss-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 09:21:30.000000 auraloss-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-21 09:21:18.000000 auraloss-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:21:30.000000 auraloss-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-21 09:21:18.000000 auraloss-0.4.0/tests/test_auraloss.py
```

### Comparing `auraloss-0.3.0/LICENSE` & `auraloss-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auraloss-0.3.0/PKG-INFO` & `auraloss-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: auraloss
-Version: 0.3.0
-Summary: Collection of audio-focused loss functions in PyTorch.
-Home-page: https://github.com/csteinmetz1/auraloss
-Author: Christian Steinmetz
-Author-email: c.j.steinmetz@qmul.ac.uk
-License: Apache License 2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: all
-License-File: LICENSE
-
-
 <div  align="center">
 
 # auraloss
 
 <img width="200px" src="docs/auraloss-logo.svg">
 
 A collection of audio-focused loss functions in PyTorch. 
@@ -50,14 +32,55 @@
 
 input = torch.rand(8,1,44100)
 target = torch.rand(8,1,44100)
 
 loss = mrstft(input, target)
 ```
 
+**NEW**: Perceptual weighting with mel scaled spectrograms.
+
+```python
+
+bs = 8
+chs = 1
+seq_len = 131072
+sample_rate = 44100
+
+# some audio you want to compare
+target = torch.rand(bs, chs, seq_len)
+pred = torch.rand(bs, chs, seq_len)
+
+# define the loss function
+loss_fn = auraloss.freq.MultiResolutionSTFTLoss(
+    fft_sizes=[1024, 2048, 8192],
+    hop_sizes=[256, 512, 2048],
+    win_lengths=[1024, 2048, 8192],
+    scale="mel",
+    n_bins=128,
+    sample_rate=sample_rate,
+    perceptual_weighting=True,
+)
+
+# compute
+loss = loss_fn(pred, target)
+
+```
+
+## Citation
+If you use this code in your work please consider citing us.
+```bibtex
+@inproceedings{steinmetz2020auraloss,
+    title={auraloss: {A}udio focused loss functions in {PyTorch}},
+    author={Steinmetz, Christian J. and Reiss, Joshua D.},
+    booktitle={Digital Music Research Network One-day Workshop (DMRN+15)},
+    year={2020}
+}
+```
+
+
 # Loss functions
 
 We categorize the loss functions as either time-domain or frequency-domain approaches. 
 Additionally, we include perceptual transforms.
 
 <table>
     <tr>
@@ -150,49 +173,59 @@
 For details please refer to the details in [`examples/compressor`](examples/compressor). 
 We provide pre-trained models, evaluation scripts to compute the metrics in the [paper](https://www.christiansteinmetz.com/s/DMRN15__auraloss__Audio_focused_loss_functions_in_PyTorch.pdf), as well as scripts to retrain models. 
 
 There are some more advanced things you can do based upon the `STFTLoss` class. 
 For example, you can compute both linear and log scaled STFT errors as in [Engel et al., 2020](https://arxiv.org/abs/2001.04643).
 In this case we do not include the spectral convergence term. 
 ```python
-stft_loss = auraloss.freq.STFTLoss(w_log_mag=1.0, 
-                                   w_lin_mag=1.0, 
-                                   w_sc=0.0, )
+stft_loss = auraloss.freq.STFTLoss(
+    w_log_mag=1.0, 
+    w_lin_mag=1.0, 
+    w_sc=0.0,
+)
 ```
 
 There is also a Mel-scaled STFT loss, which has some special requirements. 
 This loss requires you set the sample rate as well as specify the correct device. 
 ```python
 sample_rate = 44100
 melstft_loss = auraloss.freq.MelSTFTLoss(sample_rate, device="cuda")
 ```
 
 You can also build a multi-resolution Mel-scaled STFT loss with 64 bins easily. 
 Make sure you pass the correct device where the tensors you are comparing will be. 
 ```python
-mrmelstft_loss = auraloss.freq.MultiResolutionSTFTLoss(scale="mel", 
-                                                       n_bins=64,
-                                                       sample_rate=sample_rate,
-                                                       device="cuda")
+loss_fn = auraloss.freq.MultiResolutionSTFTLoss(
+    scale="mel", 
+    n_bins=64,
+    sample_rate=sample_rate,
+    device="cuda"
+)
 ```
 
-# Development
+If you are computing a loss on stereo audio you may want to consider the sum and difference (mid/side) loss. 
+Below we have shown an example of using this loss function with the perceptual weighting and mel scaling for 
+further perceptual relevance. 
 
-We currently have no tests, but those will also be coming soon, so use caution at the moment. 
-Future loss functions to be included will target neural network based perceptual losses, 
-which tend to be a bit more sophisticated than those we have included so far. 
+```python
 
-If you are interested in adding a loss function please make a pull request. 
+target = torch.rand(8, 2, 44100)
+pred = torch.rand(8, 2, 44100)
 
-## Loss functions to be added
-- [Spectral Energy Distance](https://arxiv.org/abs/2008.01160)
-- [TFGAN Losses](https://arxiv.org/abs/2011.12206)
+loss_fn = auraloss.freq.SumAndDifferenceSTFTLoss(
+    fft_sizes=[1024, 2048, 8192],
+    hop_sizes=[256, 512, 2048],
+    win_lengths=[1024, 2048, 8192],
+    perceptual_weighting=True,
+    sample_rate=44100,
+    scale="mel",
+    n_bins=128,
+)
 
-# Cite
-If you use this code in your work please consider citing us.
-```
-@inproceedings{steinmetz2020auraloss,
-    title={auraloss: {A}udio focused loss functions in {PyTorch}},
-    author={Steinmetz, Christian J. and Reiss, Joshua D.},
-    booktitle={Digital Music Research Network One-day Workshop (DMRN+15)},
-    year={2020}}
+loss = loss_fn(pred, target)
 ```
+
+# Development
+
+Run tests locally with pytest. 
+
+```python -m pytest```
```

#### html2text {}

```diff
@@ -1,25 +1,29 @@
-Metadata-Version: 2.1 Name: auraloss Version: 0.3.0 Summary: Collection of
-audio-focused loss functions in PyTorch. Home-page: https://github.com/
-csteinmetz1/auraloss Author: Christian Steinmetz Author-email:
-c.j.steinmetz@qmul.ac.uk License: Apache License 2.0 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Topic :: Multimedia :: Sound/
-Audio Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
-all License-File: LICENSE
     # auraloss [docs/auraloss-logo.svg] A collection of audio-focused loss
       functions in PyTorch. [[PDF](https://www.christiansteinmetz.com/s/
         DMRN15__auraloss__Audio_focused_loss_functions_in_PyTorch.pdf)]
 ## Setup ``` pip install auraloss ``` If you want to use `MelSTFTLoss()` or
 `FIRFilter()` you will need to specify the extra install (librosa and scipy).
 ``` pip install auraloss[all] ``` ## Usage ```python import torch import
 auraloss mrstft = auraloss.freq.MultiResolutionSTFTLoss() input = torch.rand
-(8,1,44100) target = torch.rand(8,1,44100) loss = mrstft(input, target) ``` #
-Loss functions We categorize the loss functions as either time-domain or
-frequency-domain approaches. Additionally, we include perceptual transforms.
+(8,1,44100) target = torch.rand(8,1,44100) loss = mrstft(input, target) ```
+**NEW**: Perceptual weighting with mel scaled spectrograms. ```python bs = 8
+chs = 1 seq_len = 131072 sample_rate = 44100 # some audio you want to compare
+target = torch.rand(bs, chs, seq_len) pred = torch.rand(bs, chs, seq_len) #
+define the loss function loss_fn = auraloss.freq.MultiResolutionSTFTLoss
+( fft_sizes=[1024, 2048, 8192], hop_sizes=[256, 512, 2048], win_lengths=[1024,
+2048, 8192], scale="mel", n_bins=128, sample_rate=sample_rate,
+perceptual_weighting=True, ) # compute loss = loss_fn(pred, target) ``` ##
+Citation If you use this code in your work please consider citing us. ```bibtex
+@inproceedings{steinmetz2020auraloss, title={auraloss: {A}udio focused loss
+functions in {PyTorch}}, author={Steinmetz, Christian J. and Reiss, Joshua D.},
+booktitle={Digital Music Research Network One-day Workshop (DMRN+15)}, year=
+{2020} } ``` # Loss functions We categorize the loss functions as either time-
+domain or frequency-domain approaches. Additionally, we include perceptual
+transforms.
 Loss function   Interface                              Reference
                                                    Time domain
 Error-to-signal auraloss.time.ESRLoss()                Wright_&_VÃ¤limÃ¤ki,
 ratio (ESR)                                            2019
 DC error (DC)   auraloss.time.DCLoss()                 Wright_&_VÃ¤limÃ¤ki,
                                                        2019
 Log hyperbolic
@@ -66,27 +70,25 @@
 trained models, evaluation scripts to compute the metrics in the [paper](https:
 //www.christiansteinmetz.com/s/
 DMRN15__auraloss__Audio_focused_loss_functions_in_PyTorch.pdf), as well as
 scripts to retrain models. There are some more advanced things you can do based
 upon the `STFTLoss` class. For example, you can compute both linear and log
 scaled STFT errors as in [Engel et al., 2020](https://arxiv.org/abs/
 2001.04643). In this case we do not include the spectral convergence term.
-```python stft_loss = auraloss.freq.STFTLoss(w_log_mag=1.0, w_lin_mag=1.0,
+```python stft_loss = auraloss.freq.STFTLoss( w_log_mag=1.0, w_lin_mag=1.0,
 w_sc=0.0, ) ``` There is also a Mel-scaled STFT loss, which has some special
 requirements. This loss requires you set the sample rate as well as specify the
 correct device. ```python sample_rate = 44100 melstft_loss =
 auraloss.freq.MelSTFTLoss(sample_rate, device="cuda") ``` You can also build a
 multi-resolution Mel-scaled STFT loss with 64 bins easily. Make sure you pass
 the correct device where the tensors you are comparing will be. ```python
-mrmelstft_loss = auraloss.freq.MultiResolutionSTFTLoss(scale="mel", n_bins=64,
-sample_rate=sample_rate, device="cuda") ``` # Development We currently have no
-tests, but those will also be coming soon, so use caution at the moment. Future
-loss functions to be included will target neural network based perceptual
-losses, which tend to be a bit more sophisticated than those we have included
-so far. If you are interested in adding a loss function please make a pull
-request. ## Loss functions to be added - [Spectral Energy Distance](https://
-arxiv.org/abs/2008.01160) - [TFGAN Losses](https://arxiv.org/abs/2011.12206) #
-Cite If you use this code in your work please consider citing us. ```
-@inproceedings{steinmetz2020auraloss, title={auraloss: {A}udio focused loss
-functions in {PyTorch}}, author={Steinmetz, Christian J. and Reiss, Joshua D.},
-booktitle={Digital Music Research Network One-day Workshop (DMRN+15)}, year=
-{2020}} ```
+loss_fn = auraloss.freq.MultiResolutionSTFTLoss( scale="mel", n_bins=64,
+sample_rate=sample_rate, device="cuda" ) ``` If you are computing a loss on
+stereo audio you may want to consider the sum and difference (mid/side) loss.
+Below we have shown an example of using this loss function with the perceptual
+weighting and mel scaling for further perceptual relevance. ```python target =
+torch.rand(8, 2, 44100) pred = torch.rand(8, 2, 44100) loss_fn =
+auraloss.freq.SumAndDifferenceSTFTLoss( fft_sizes=[1024, 2048, 8192],
+hop_sizes=[256, 512, 2048], win_lengths=[1024, 2048, 8192],
+perceptual_weighting=True, sample_rate=44100, scale="mel", n_bins=128, ) loss =
+loss_fn(pred, target) ``` # Development Run tests locally with pytest.
+```python -m pytest```
```

### Comparing `auraloss-0.3.0/auraloss/freq.py` & `auraloss-0.4.0/auraloss/freq.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import torch
 import numpy as np
-from .utils import apply_reduction
+from typing import List, Any
 
+from .utils import apply_reduction
 from .perceptual import SumAndDifference, FIRFilter
 
 
 class SpectralConvergenceLoss(torch.nn.Module):
     """Spectral convergence loss module.
 
     See [Arik et al., 2018](https://arxiv.org/abs/1808.06719).
@@ -65,101 +66,127 @@
         w_lin_mag_mag (float, optional): Weight of the linear magnitude loss term. Default: 0.0
         w_phs (float, optional): Weight of the spectral phase loss term. Default: 0.0
         sample_rate (int, optional): Sample rate. Required when scale = 'mel'. Default: None
         scale (str, optional): Optional frequency scaling method, options include:
             ['mel', 'chroma']
             Default: None
         n_bins (int, optional): Number of scaling frequency bins. Default: None.
+        perceptual_weighting (bool, optional): Apply perceptual A-weighting (Sample rate must be supplied). Default: False
         scale_invariance (bool, optional): Perform an optimal scaling of the target. Default: False
         eps (float, optional): Small epsilon value for stablity. Default: 1e-8
         output (str, optional): Format of the loss returned.
             'loss' : Return only the raw, aggregate loss term.
             'full' : Return the raw loss, plus intermediate loss terms.
             Default: 'loss'
         reduction (str, optional): Specifies the reduction to apply to the output:
             'none': no reduction will be applied,
             'mean': the sum of the output will be divided by the number of elements in the output,
             'sum': the output will be summed.
             Default: 'mean'
+        mag_distance (str, optional): Distance function ["L1", "L2"] for the magnitude loss terms.
         device (str, optional): Place the filterbanks on specified device. Default: None
 
     Returns:
         loss:
             Aggreate loss term. Only returned if output='loss'. By default.
         loss, sc_mag_loss, log_mag_loss, lin_mag_loss, phs_loss:
             Aggregate and intermediate loss terms. Only returned if output='full'.
     """
 
     def __init__(
         self,
-        fft_size=1024,
-        hop_size=256,
-        win_length=1024,
-        window="hann_window",
-        w_sc=1.0,
-        w_log_mag=1.0,
-        w_lin_mag=0.0,
-        w_phs=0.0,
-        sample_rate=None,
-        scale=None,
-        n_bins=None,
-        scale_invariance=False,
-        eps=1e-8,
-        output="loss",
-        reduction="mean",
-        device=None,
+        fft_size: int = 1024,
+        hop_size: int = 256,
+        win_length: int = 1024,
+        window: str = "hann_window",
+        w_sc: float = 1.0,
+        w_log_mag: float = 1.0,
+        w_lin_mag: float = 0.0,
+        w_phs: float = 0.0,
+        sample_rate: float = None,
+        scale: str = None,
+        n_bins: int = None,
+        perceptual_weighting: bool = False,
+        scale_invariance: bool = False,
+        eps: float = 1e-8,
+        output: str = "loss",
+        reduction: str = "mean",
+        mag_distance: str = "L1",
+        device: Any = None,
     ):
-        super(STFTLoss, self).__init__()
+        super().__init__()
         self.fft_size = fft_size
         self.hop_size = hop_size
         self.win_length = win_length
         self.window = getattr(torch, window)(win_length)
         self.w_sc = w_sc
         self.w_log_mag = w_log_mag
         self.w_lin_mag = w_lin_mag
         self.w_phs = w_phs
         self.sample_rate = sample_rate
         self.scale = scale
         self.n_bins = n_bins
+        self.perceptual_weighting = perceptual_weighting
         self.scale_invariance = scale_invariance
         self.eps = eps
         self.output = output
         self.reduction = reduction
+        self.mag_distance = mag_distance
         self.device = device
 
         self.spectralconv = SpectralConvergenceLoss()
-        self.logstft = STFTMagnitudeLoss(log=True, reduction=reduction)
-        self.linstft = STFTMagnitudeLoss(log=False, reduction=reduction)
+        self.logstft = STFTMagnitudeLoss(
+            log=True,
+            reduction=reduction,
+            distance=mag_distance,
+        )
+        self.linstft = STFTMagnitudeLoss(
+            log=False,
+            reduction=reduction,
+            distance=mag_distance,
+        )
 
         # setup mel filterbank
         if scale is not None:
-
             try:
                 import librosa.filters
             except Exception as e:
                 print(e)
                 print("Try `pip install auraloss[all]`.")
 
             if self.scale == "mel":
                 assert sample_rate != None  # Must set sample rate to use mel scale
                 assert n_bins <= fft_size  # Must be more FFT bins than Mel bins
                 fb = librosa.filters.mel(sr=sample_rate, n_fft=fft_size, n_mels=n_bins)
-                self.fb = torch.tensor(fb).unsqueeze(0)
+                fb = torch.tensor(fb).unsqueeze(0)
 
             elif self.scale == "chroma":
                 assert sample_rate != None  # Must set sample rate to use chroma scale
                 assert n_bins <= fft_size  # Must be more FFT bins than chroma bins
-                fb = librosa.filters.chroma(sr=sample_rate, n_fft=fft_size, n_chroma=n_bins)
-                self.fb = torch.tensor(fb).unsqueeze(0)
+                fb = librosa.filters.chroma(
+                    sr=sample_rate, n_fft=fft_size, n_chroma=n_bins
+                )
+
             else:
-                raise ValueError(f"Invalid scale: {self.scale}. Must be 'mel' or 'chroma'.")
+                raise ValueError(
+                    f"Invalid scale: {self.scale}. Must be 'mel' or 'chroma'."
+                )
+
+            self.register_buffer("fb", fb)
 
         if scale is not None and device is not None:
             self.fb = self.fb.to(self.device)  # move filterbank to device
 
+        if self.perceptual_weighting:
+            if sample_rate is None:
+                raise ValueError(
+                    f"`sample_rate` must be supplied when `perceptual_weighting = True`."
+                )
+            self.prefilter = FIRFilter(filter_type="aw", fs=sample_rate)
+
     def stft(self, x):
         """Perform STFT.
         Args:
             x (Tensor): Input signal tensor (B, T).
 
         Returns:
             Tensor: x_mag, x_phs
@@ -170,33 +197,49 @@
             self.fft_size,
             self.hop_size,
             self.win_length,
             self.window,
             return_complex=True,
         )
         x_mag = torch.sqrt(
-            torch.clamp((x_stft.real ** 2) + (x_stft.imag ** 2), min=self.eps)
+            torch.clamp((x_stft.real**2) + (x_stft.imag**2), min=self.eps)
         )
         x_phs = torch.angle(x_stft)
         return x_mag, x_phs
 
-    def forward(self, x, y):
+    def forward(self, input: torch.Tensor, target: torch.Tensor):
+        bs, chs, seq_len = input.size()
+
+        if self.perceptual_weighting:  # apply optional A-weighting via FIR filter
+            # since FIRFilter only support mono audio we will move channels to batch dim
+            input = input.view(bs * chs, 1, -1)
+            target = target.view(bs * chs, 1, -1)
+
+            # now apply the filter to both
+            self.prefilter.to(input.device)
+            input, target = self.prefilter(input, target)
+
+            # now move the channels back
+            input = input.view(bs, chs, -1)
+            target = target.view(bs, chs, -1)
+
         # compute the magnitude and phase spectra of input and target
-        self.window = self.window.to(x.device)
-        x_mag, x_phs = self.stft(x.view(-1, x.size(-1)))
-        y_mag, y_phs = self.stft(y.view(-1, y.size(-1)))
+        self.window = self.window.to(input.device)
+        x_mag, x_phs = self.stft(input.view(-1, input.size(-1)))
+        y_mag, y_phs = self.stft(target.view(-1, target.size(-1)))
 
         # apply relevant transforms
         if self.scale is not None:
+            self.fb = self.fb.to(input.device)
             x_mag = torch.matmul(self.fb, x_mag)
             y_mag = torch.matmul(self.fb, y_mag)
 
         # normalize scales
         if self.scale_invariance:
-            alpha = (x_mag * y_mag).sum([-2, -1]) / ((y_mag ** 2).sum([-2, -1]))
+            alpha = (x_mag * y_mag).sum([-2, -1]) / ((y_mag**2).sum([-2, -1]))
             y_mag = y_mag * alpha.unsqueeze(-1)
 
         # compute loss terms
         sc_mag_loss = self.spectralconv(x_mag, y_mag) if self.w_sc else 0.0
         log_mag_loss = self.logstft(x_mag, y_mag) if self.w_log_mag else 0.0
         lin_mag_loss = self.linstft(x_mag, y_mag) if self.w_lin_mag else 0.0
         phs_loss = torch.nn.functional.mse_loss(x_phs, y_phs) if self.w_phs else 0.0
@@ -305,29 +348,30 @@
             Default: None
         n_bins (int, optional): Number of mel frequency bins. Required when scale = 'mel'. Default: None.
         scale_invariance (bool, optional): Perform an optimal scaling of the target. Default: False
     """
 
     def __init__(
         self,
-        fft_sizes=[1024, 2048, 512],
-        hop_sizes=[120, 240, 50],
-        win_lengths=[600, 1200, 240],
-        window="hann_window",
-        w_sc=1.0,
-        w_log_mag=1.0,
-        w_lin_mag=0.0,
-        w_phs=0.0,
-        sample_rate=None,
-        scale=None,
-        n_bins=None,
-        scale_invariance=False,
+        fft_sizes: List[int] = [1024, 2048, 512],
+        hop_sizes: List[int] = [120, 240, 50],
+        win_lengths: List[int] = [600, 1200, 240],
+        window: str = "hann_window",
+        w_sc: float = 1.0,
+        w_log_mag: float = 1.0,
+        w_lin_mag: float = 0.0,
+        w_phs: float = 0.0,
+        sample_rate: float = None,
+        scale: str = None,
+        n_bins: int = None,
+        perceptual_weighting: bool = False,
+        scale_invariance: bool = False,
         **kwargs,
     ):
-        super(MultiResolutionSTFTLoss, self).__init__()
+        super().__init__()
         assert len(fft_sizes) == len(hop_sizes) == len(win_lengths)  # must define all
         self.fft_sizes = fft_sizes
         self.hop_sizes = hop_sizes
         self.win_lengths = win_lengths
 
         self.stft_losses = torch.nn.ModuleList()
         for fs, ss, wl in zip(fft_sizes, hop_sizes, win_lengths):
@@ -340,14 +384,15 @@
                     w_sc,
                     w_log_mag,
                     w_lin_mag,
                     w_phs,
                     sample_rate,
                     scale,
                     n_bins,
+                    perceptual_weighting,
                     scale_invariance,
                     **kwargs,
                 )
             ]
 
     def forward(self, x, y):
         mrstft_loss = 0.0
@@ -407,15 +452,15 @@
         w_phs=0.0,
         sample_rate=None,
         scale=None,
         n_mels=None,
         randomize_rate=1,
         **kwargs,
     ):
-        super(RandomResolutionSTFTLoss, self).__init__()
+        super().__init__()
         self.resolutions = resolutions
         self.min_fft_size = min_fft_size
         self.max_fft_size = max_fft_size
         self.min_hop_size = min_hop_size
         self.max_hop_size = max_hop_size
         self.windows = windows
         self.randomize_rate = randomize_rate
@@ -487,53 +532,74 @@
 
 class SumAndDifferenceSTFTLoss(torch.nn.Module):
     """Sum and difference sttereo STFT loss module.
 
     See [Steinmetz et al., 2020](https://arxiv.org/abs/2010.10291)
 
     Args:
-        fft_sizes (list, optional): List of FFT sizes.
-        hop_sizes (list, optional): List of hop sizes.
-        win_lengths (list, optional): List of window lengths.
+        fft_sizes (List[int]): List of FFT sizes.
+        hop_sizes (List[int]): List of hop sizes.
+        win_lengths (List[int]): List of window lengths.
         window (str, optional): Window function type.
         w_sum (float, optional): Weight of the sum loss component. Default: 1.0
         w_diff (float, optional): Weight of the difference loss component. Default: 1.0
+        perceptual_weighting (bool, optional): Apply perceptual A-weighting (Sample rate must be supplied). Default: False
+        mel_stft (bool, optional): Use Multi-resoltuion mel spectrograms. Default: False
+        n_mel_bins (int, optional): Number of mel bins to use when mel_stft = True. Default: 128
+        sample_rate (float, optional): Audio sample rate. Default: None
         output (str, optional): Format of the loss returned.
             'loss' : Return only the raw, aggregate loss term.
             'full' : Return the raw loss, plus intermediate loss terms.
             Default: 'loss'
-
-    Returns:
-        loss:
-            Aggreate loss term. Only returned if output='loss'.
-        loss, sum_loss, diff_loss:
-            Aggregate and intermediate loss terms. Only returned if output='full'.
     """
 
     def __init__(
         self,
-        fft_sizes=[1024, 2048, 512],
-        hop_sizes=[120, 240, 50],
-        win_lengths=[600, 1200, 240],
-        window="hann_window",
-        w_sum=1.0,
-        w_diff=1.0,
-        output="loss",
+        fft_sizes: List[int],
+        hop_sizes: List[int],
+        win_lengths: List[int],
+        window: str = "hann_window",
+        w_sum: float = 1.0,
+        w_diff: float = 1.0,
+        output: str = "loss",
+        **kwargs,
     ):
-        super(SumAndDifferenceSTFTLoss, self).__init__()
+        super().__init__()
         self.sd = SumAndDifference()
-        self.w_sum = 1.0
-        self.w_diff = 1.0
+        self.w_sum = w_sum
+        self.w_diff = w_diff
         self.output = output
-        self.mrstft = MultiResolutionSTFTLoss(fft_sizes, hop_sizes, win_lengths, window)
+        self.mrstft = MultiResolutionSTFTLoss(
+            fft_sizes,
+            hop_sizes,
+            win_lengths,
+            window,
+            **kwargs,
+        )
 
-    def forward(self, input, target):
+    def forward(self, input: torch.Tensor, target: torch.Tensor):
+        """This loss function assumes batched input of stereo audio in the time domain.
+
+        Args:
+            input (torch.Tensor): Input tensor with shape (batch size, 2, seq_len).
+            target (torch.Tensor): Target tensor with shape (batch size, 2, seq_len).
+
+        Returns:
+            loss (torch.Tensor): Aggreate loss term. Only returned if output='loss'.
+            loss (torch.Tensor), sum_loss (torch.Tensor), diff_loss (torch.Tensor):
+                Aggregate and intermediate loss terms. Only returned if output='full'.
+        """
+        assert input.shape == target.shape  # must have same shape
+        bs, chs, seq_len = input.size()
+
+        # compute sum and difference signals for both
         input_sum, input_diff = self.sd(input)
         target_sum, target_diff = self.sd(target)
 
+        # compute error in STFT domain
         sum_loss = self.mrstft(input_sum, target_sum)
         diff_loss = self.mrstft(input_diff, target_diff)
         loss = ((self.w_sum * sum_loss) + (self.w_diff * diff_loss)) / 2
 
         if self.output == "loss":
             return loss
         elif self.output == "full":
```

### Comparing `auraloss-0.3.0/auraloss/perceptual.py` & `auraloss-0.4.0/auraloss/perceptual.py`

 * *Files identical despite different names*

### Comparing `auraloss-0.3.0/auraloss/plotting.py` & `auraloss-0.4.0/auraloss/plotting.py`

 * *Files identical despite different names*

### Comparing `auraloss-0.3.0/auraloss/time.py` & `auraloss-0.4.0/auraloss/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import torch
+from torch import Tensor as T
+
 from .utils import apply_reduction
 
 
 class ESRLoss(torch.nn.Module):
     """Error-to-signal ratio loss function module.
 
     See [Wright & Välimäki, 2019](https://arxiv.org/abs/1911.08922).
@@ -13,20 +15,23 @@
         'mean': the sum of the output will be divided by the number of elements in the output,
         'sum': the output will be summed. Default: 'mean'
     Shape:
         - input : :math:`(batch, nchs, ...)`.
         - target: :math:`(batch, nchs, ...)`.
     """
 
-    def __init__(self, reduction="mean"):
-        super(ESRLoss, self).__init__()
+    def __init__(self, eps: float = 1e-8, reduction: str = "mean") -> None:
+        super().__init__()
+        self.eps = eps
         self.reduction = reduction
 
-    def forward(self, input, target):
-        losses = ((target - input).abs() ** 2).sum(-1) / (target.abs() ** 2).sum(-1)
+    def forward(self, input: T, target: T) -> T:
+        num = ((target - input) ** 2).sum(dim=-1)
+        denom = (target ** 2).sum(dim=-1) + self.eps
+        losses = num / denom
         losses = apply_reduction(losses, reduction=self.reduction)
         return losses
 
 
 class DCLoss(torch.nn.Module):
     """DC loss function module.
 
@@ -38,20 +43,23 @@
         'mean': the sum of the output will be divided by the number of elements in the output,
         'sum': the output will be summed. Default: 'mean'
     Shape:
         - input : :math:`(batch, nchs, ...)`.
         - target: :math:`(batch, nchs, ...)`.
     """
 
-    def __init__(self, reduction="mean"):
-        super(DCLoss, self).__init__()
+    def __init__(self, eps: float = 1e-8, reduction: str = "mean") -> None:
+        super().__init__()
+        self.eps = eps
         self.reduction = reduction
 
-    def forward(self, input, target):
-        losses = ((target - input).mean(-1) ** 2).abs() / (target.abs().mean(-1) ** 2)
+    def forward(self, input: T, target: T) -> T:
+        num = (target - input).mean(dim=-1) ** 2
+        denom = (target ** 2).mean(dim=-1) + self.eps
+        losses = num / denom
         losses = apply_reduction(losses, self.reduction)
         return losses
 
 
 class LogCoshLoss(torch.nn.Module):
     """Log-cosh loss function module.
```

### Comparing `auraloss-0.3.0/auraloss.egg-info/PKG-INFO` & `auraloss-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auraloss
-Version: 0.3.0
+Version: 0.4.0
 Summary: Collection of audio-focused loss functions in PyTorch.
 Home-page: https://github.com/csteinmetz1/auraloss
 Author: Christian Steinmetz
 Author-email: c.j.steinmetz@qmul.ac.uk
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Multimedia :: Sound/Audio
@@ -50,14 +50,55 @@
 
 input = torch.rand(8,1,44100)
 target = torch.rand(8,1,44100)
 
 loss = mrstft(input, target)
 ```
 
+**NEW**: Perceptual weighting with mel scaled spectrograms.
+
+```python
+
+bs = 8
+chs = 1
+seq_len = 131072
+sample_rate = 44100
+
+# some audio you want to compare
+target = torch.rand(bs, chs, seq_len)
+pred = torch.rand(bs, chs, seq_len)
+
+# define the loss function
+loss_fn = auraloss.freq.MultiResolutionSTFTLoss(
+    fft_sizes=[1024, 2048, 8192],
+    hop_sizes=[256, 512, 2048],
+    win_lengths=[1024, 2048, 8192],
+    scale="mel",
+    n_bins=128,
+    sample_rate=sample_rate,
+    perceptual_weighting=True,
+)
+
+# compute
+loss = loss_fn(pred, target)
+
+```
+
+## Citation
+If you use this code in your work please consider citing us.
+```bibtex
+@inproceedings{steinmetz2020auraloss,
+    title={auraloss: {A}udio focused loss functions in {PyTorch}},
+    author={Steinmetz, Christian J. and Reiss, Joshua D.},
+    booktitle={Digital Music Research Network One-day Workshop (DMRN+15)},
+    year={2020}
+}
+```
+
+
 # Loss functions
 
 We categorize the loss functions as either time-domain or frequency-domain approaches. 
 Additionally, we include perceptual transforms.
 
 <table>
     <tr>
@@ -150,49 +191,59 @@
 For details please refer to the details in [`examples/compressor`](examples/compressor). 
 We provide pre-trained models, evaluation scripts to compute the metrics in the [paper](https://www.christiansteinmetz.com/s/DMRN15__auraloss__Audio_focused_loss_functions_in_PyTorch.pdf), as well as scripts to retrain models. 
 
 There are some more advanced things you can do based upon the `STFTLoss` class. 
 For example, you can compute both linear and log scaled STFT errors as in [Engel et al., 2020](https://arxiv.org/abs/2001.04643).
 In this case we do not include the spectral convergence term. 
 ```python
-stft_loss = auraloss.freq.STFTLoss(w_log_mag=1.0, 
-                                   w_lin_mag=1.0, 
-                                   w_sc=0.0, )
+stft_loss = auraloss.freq.STFTLoss(
+    w_log_mag=1.0, 
+    w_lin_mag=1.0, 
+    w_sc=0.0,
+)
 ```
 
 There is also a Mel-scaled STFT loss, which has some special requirements. 
 This loss requires you set the sample rate as well as specify the correct device. 
 ```python
 sample_rate = 44100
 melstft_loss = auraloss.freq.MelSTFTLoss(sample_rate, device="cuda")
 ```
 
 You can also build a multi-resolution Mel-scaled STFT loss with 64 bins easily. 
 Make sure you pass the correct device where the tensors you are comparing will be. 
 ```python
-mrmelstft_loss = auraloss.freq.MultiResolutionSTFTLoss(scale="mel", 
-                                                       n_bins=64,
-                                                       sample_rate=sample_rate,
-                                                       device="cuda")
+loss_fn = auraloss.freq.MultiResolutionSTFTLoss(
+    scale="mel", 
+    n_bins=64,
+    sample_rate=sample_rate,
+    device="cuda"
+)
 ```
 
-# Development
+If you are computing a loss on stereo audio you may want to consider the sum and difference (mid/side) loss. 
+Below we have shown an example of using this loss function with the perceptual weighting and mel scaling for 
+further perceptual relevance. 
 
-We currently have no tests, but those will also be coming soon, so use caution at the moment. 
-Future loss functions to be included will target neural network based perceptual losses, 
-which tend to be a bit more sophisticated than those we have included so far. 
+```python
 
-If you are interested in adding a loss function please make a pull request. 
+target = torch.rand(8, 2, 44100)
+pred = torch.rand(8, 2, 44100)
 
-## Loss functions to be added
-- [Spectral Energy Distance](https://arxiv.org/abs/2008.01160)
-- [TFGAN Losses](https://arxiv.org/abs/2011.12206)
+loss_fn = auraloss.freq.SumAndDifferenceSTFTLoss(
+    fft_sizes=[1024, 2048, 8192],
+    hop_sizes=[256, 512, 2048],
+    win_lengths=[1024, 2048, 8192],
+    perceptual_weighting=True,
+    sample_rate=44100,
+    scale="mel",
+    n_bins=128,
+)
 
-# Cite
-If you use this code in your work please consider citing us.
-```
-@inproceedings{steinmetz2020auraloss,
-    title={auraloss: {A}udio focused loss functions in {PyTorch}},
-    author={Steinmetz, Christian J. and Reiss, Joshua D.},
-    booktitle={Digital Music Research Network One-day Workshop (DMRN+15)},
-    year={2020}}
+loss = loss_fn(pred, target)
 ```
+
+# Development
+
+Run tests locally with pytest. 
+
+```python -m pytest```
```

#### html2text {}

```diff
@@ -1,25 +1,37 @@
-Metadata-Version: 2.1 Name: auraloss Version: 0.3.0 Summary: Collection of
+Metadata-Version: 2.1 Name: auraloss Version: 0.4.0 Summary: Collection of
 audio-focused loss functions in PyTorch. Home-page: https://github.com/
 csteinmetz1/auraloss Author: Christian Steinmetz Author-email:
 c.j.steinmetz@qmul.ac.uk License: Apache License 2.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Topic :: Multimedia :: Sound/
 Audio Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
 all License-File: LICENSE
     # auraloss [docs/auraloss-logo.svg] A collection of audio-focused loss
       functions in PyTorch. [[PDF](https://www.christiansteinmetz.com/s/
         DMRN15__auraloss__Audio_focused_loss_functions_in_PyTorch.pdf)]
 ## Setup ``` pip install auraloss ``` If you want to use `MelSTFTLoss()` or
 `FIRFilter()` you will need to specify the extra install (librosa and scipy).
 ``` pip install auraloss[all] ``` ## Usage ```python import torch import
 auraloss mrstft = auraloss.freq.MultiResolutionSTFTLoss() input = torch.rand
-(8,1,44100) target = torch.rand(8,1,44100) loss = mrstft(input, target) ``` #
-Loss functions We categorize the loss functions as either time-domain or
-frequency-domain approaches. Additionally, we include perceptual transforms.
+(8,1,44100) target = torch.rand(8,1,44100) loss = mrstft(input, target) ```
+**NEW**: Perceptual weighting with mel scaled spectrograms. ```python bs = 8
+chs = 1 seq_len = 131072 sample_rate = 44100 # some audio you want to compare
+target = torch.rand(bs, chs, seq_len) pred = torch.rand(bs, chs, seq_len) #
+define the loss function loss_fn = auraloss.freq.MultiResolutionSTFTLoss
+( fft_sizes=[1024, 2048, 8192], hop_sizes=[256, 512, 2048], win_lengths=[1024,
+2048, 8192], scale="mel", n_bins=128, sample_rate=sample_rate,
+perceptual_weighting=True, ) # compute loss = loss_fn(pred, target) ``` ##
+Citation If you use this code in your work please consider citing us. ```bibtex
+@inproceedings{steinmetz2020auraloss, title={auraloss: {A}udio focused loss
+functions in {PyTorch}}, author={Steinmetz, Christian J. and Reiss, Joshua D.},
+booktitle={Digital Music Research Network One-day Workshop (DMRN+15)}, year=
+{2020} } ``` # Loss functions We categorize the loss functions as either time-
+domain or frequency-domain approaches. Additionally, we include perceptual
+transforms.
 Loss function   Interface                              Reference
                                                    Time domain
 Error-to-signal auraloss.time.ESRLoss()                Wright_&_VÃ¤limÃ¤ki,
 ratio (ESR)                                            2019
 DC error (DC)   auraloss.time.DCLoss()                 Wright_&_VÃ¤limÃ¤ki,
                                                        2019
 Log hyperbolic
@@ -66,27 +78,25 @@
 trained models, evaluation scripts to compute the metrics in the [paper](https:
 //www.christiansteinmetz.com/s/
 DMRN15__auraloss__Audio_focused_loss_functions_in_PyTorch.pdf), as well as
 scripts to retrain models. There are some more advanced things you can do based
 upon the `STFTLoss` class. For example, you can compute both linear and log
 scaled STFT errors as in [Engel et al., 2020](https://arxiv.org/abs/
 2001.04643). In this case we do not include the spectral convergence term.
-```python stft_loss = auraloss.freq.STFTLoss(w_log_mag=1.0, w_lin_mag=1.0,
+```python stft_loss = auraloss.freq.STFTLoss( w_log_mag=1.0, w_lin_mag=1.0,
 w_sc=0.0, ) ``` There is also a Mel-scaled STFT loss, which has some special
 requirements. This loss requires you set the sample rate as well as specify the
 correct device. ```python sample_rate = 44100 melstft_loss =
 auraloss.freq.MelSTFTLoss(sample_rate, device="cuda") ``` You can also build a
 multi-resolution Mel-scaled STFT loss with 64 bins easily. Make sure you pass
 the correct device where the tensors you are comparing will be. ```python
-mrmelstft_loss = auraloss.freq.MultiResolutionSTFTLoss(scale="mel", n_bins=64,
-sample_rate=sample_rate, device="cuda") ``` # Development We currently have no
-tests, but those will also be coming soon, so use caution at the moment. Future
-loss functions to be included will target neural network based perceptual
-losses, which tend to be a bit more sophisticated than those we have included
-so far. If you are interested in adding a loss function please make a pull
-request. ## Loss functions to be added - [Spectral Energy Distance](https://
-arxiv.org/abs/2008.01160) - [TFGAN Losses](https://arxiv.org/abs/2011.12206) #
-Cite If you use this code in your work please consider citing us. ```
-@inproceedings{steinmetz2020auraloss, title={auraloss: {A}udio focused loss
-functions in {PyTorch}}, author={Steinmetz, Christian J. and Reiss, Joshua D.},
-booktitle={Digital Music Research Network One-day Workshop (DMRN+15)}, year=
-{2020}} ```
+loss_fn = auraloss.freq.MultiResolutionSTFTLoss( scale="mel", n_bins=64,
+sample_rate=sample_rate, device="cuda" ) ``` If you are computing a loss on
+stereo audio you may want to consider the sum and difference (mid/side) loss.
+Below we have shown an example of using this loss function with the perceptual
+weighting and mel scaling for further perceptual relevance. ```python target =
+torch.rand(8, 2, 44100) pred = torch.rand(8, 2, 44100) loss_fn =
+auraloss.freq.SumAndDifferenceSTFTLoss( fft_sizes=[1024, 2048, 8192],
+hop_sizes=[256, 512, 2048], win_lengths=[1024, 2048, 8192],
+perceptual_weighting=True, sample_rate=44100, scale="mel", n_bins=128, ) loss =
+loss_fn(pred, target) ``` # Development Run tests locally with pytest.
+```python -m pytest```
```

### Comparing `auraloss-0.3.0/setup.py` & `auraloss-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "auraloss"
 DESCRIPTION = "Audio-focused loss functions in PyTorch"
 URL = "https://github.com/csteinmetz1/auraloss"
 EMAIL = "c.j.steinmetz@qmul.ac.uk"
 AUTHOR = "Christian Steinmetz"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.3.0"
+VERSION = "0.4.0"
 
 HERE = Path(__file__).parent
 
 try:
     with open(HERE / "README.md", encoding="utf-8") as f:
         long_description = "\n" + f.read()
 except FileNotFoundError:
@@ -28,15 +28,15 @@
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=["auraloss"],
     install_requires=["torch", "numpy"],
-    extras_require={"test": ["resampy"], "all": ["matplotlib",  "librosa", "scipy"]},
+    extras_require={"test": ["resampy"], "all": ["matplotlib", "librosa", "scipy"]},
     include_package_data=True,
     license="Apache License 2.0",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Multimedia :: Sound/Audio",
         "Topic :: Scientific/Engineering",
     ],
```

