# Comparing `tmp/vamb-4.0.1.tar.gz` & `tmp/vamb-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vamb-4.0.1.tar", last modified: Thu Mar 30 13:04:42 2023, max compression
+gzip compressed data, was "vamb-4.1.0.tar", last modified: Fri Apr 21 09:42:18 2023, max compression
```

## Comparing `vamb-4.0.1.tar` & `vamb-4.1.0.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-03-30 13:04:42.724694 vamb-4.0.1/
--rw-r--r--   0 jakni     (1000) jakni     (1000)     1081 2023-03-10 08:42:57.000000 vamb-4.0.1/LICENSE
--rw-r--r--   0 jakni     (1000) jakni     (1000)       24 2023-03-10 08:42:57.000000 vamb-4.0.1/MANIFEST.in
--rw-r--r--   0 jakni     (1000) jakni     (1000)      103 2023-03-30 13:04:42.724694 vamb-4.0.1/PKG-INFO
--rw-r--r--   0 jakni     (1000) jakni     (1000)    15245 2023-03-30 12:20:17.000000 vamb-4.0.1/README.md
--rw-r--r--   0 jakni     (1000) jakni     (1000)      970 2023-03-30 12:20:17.000000 vamb-4.0.1/pyproject.toml
--rw-r--r--   0 jakni     (1000) jakni     (1000)       94 2023-03-30 13:04:42.724694 vamb-4.0.1/setup.cfg
--rw-r--r--   0 jakni     (1000) jakni     (1000)      128 2023-03-10 08:42:57.000000 vamb-4.0.1/setup.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-03-30 13:04:42.724694 vamb-4.0.1/src/
--rw-r--r--   0 jakni     (1000) jakni     (1000)     2846 2023-03-10 08:42:57.000000 vamb-4.0.1/src/_vambtools.pyx
--rw-r--r--   0 jakni     (1000) jakni     (1000)     1804 2023-03-30 12:20:17.000000 vamb-4.0.1/src/concatenate.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-03-30 13:04:42.724694 vamb-4.0.1/test/
--rw-r--r--   0 jakni     (1000) jakni     (1000)     1417 2023-03-30 12:20:17.000000 vamb-4.0.1/test/testtools.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-03-30 13:04:42.724694 vamb-4.0.1/vamb/
--rw-r--r--   0 jakni     (1000) jakni     (1000)      808 2023-03-30 12:56:43.000000 vamb-4.0.1/vamb/__init__.py
--rwxr-xr-x   0 jakni     (1000) jakni     (1000)    42759 2023-03-30 12:20:17.000000 vamb-4.0.1/vamb/__main__.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    18002 2023-03-30 12:20:17.000000 vamb-4.0.1/vamb/aamb_encode.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    25151 2023-03-10 08:42:57.000000 vamb-4.0.1/vamb/benchmark.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    19264 2023-03-30 12:52:45.000000 vamb-4.0.1/vamb/cluster.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    22056 2023-03-30 12:20:17.000000 vamb-4.0.1/vamb/encode.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    77187 2022-04-05 08:20:29.000000 vamb-4.0.1/vamb/kernel.npz
--rw-r--r--   0 jakni     (1000) jakni     (1000)     7796 2023-03-30 12:20:17.000000 vamb-4.0.1/vamb/parsebam.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     7037 2023-03-10 08:42:57.000000 vamb-4.0.1/vamb/parsecontigs.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    21288 2023-03-10 08:42:57.000000 vamb-4.0.1/vamb/vambtools.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-03-30 13:04:42.724694 vamb-4.0.1/vamb.egg-info/
--rw-r--r--   0 jakni     (1000) jakni     (1000)      103 2023-03-30 13:04:42.000000 vamb-4.0.1/vamb.egg-info/PKG-INFO
--rw-r--r--   0 jakni     (1000) jakni     (1000)      464 2023-03-30 13:04:42.000000 vamb-4.0.1/vamb.egg-info/SOURCES.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)        1 2023-03-30 13:04:42.000000 vamb-4.0.1/vamb.egg-info/dependency_links.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-03-30 13:04:42.000000 vamb-4.0.1/vamb.egg-info/entry_points.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)       38 2023-03-30 13:04:42.000000 vamb-4.0.1/vamb.egg-info/requires.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)        5 2023-03-30 13:04:42.000000 vamb-4.0.1/vamb.egg-info/top_level.txt
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-21 09:42:18.090484 vamb-4.1.0/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1081 2023-03-10 08:42:57.000000 vamb-4.1.0/LICENSE
+-rw-r--r--   0 jakni     (1000) jakni     (1000)       24 2023-03-10 08:42:57.000000 vamb-4.1.0/MANIFEST.in
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      101 2023-04-21 09:42:18.090484 vamb-4.1.0/PKG-INFO
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    15245 2023-03-30 12:20:17.000000 vamb-4.1.0/README.md
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1005 2023-04-21 09:41:38.000000 vamb-4.1.0/pyproject.toml
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      146 2023-04-21 09:42:18.090484 vamb-4.1.0/setup.cfg
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      128 2023-03-10 08:42:57.000000 vamb-4.1.0/setup.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-21 09:42:18.087151 vamb-4.1.0/src/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     2846 2023-03-10 08:42:57.000000 vamb-4.1.0/src/_vambtools.pyx
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1804 2023-03-30 12:20:17.000000 vamb-4.1.0/src/concatenate.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-21 09:42:18.087151 vamb-4.1.0/test/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    12734 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_benchmark.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     4879 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_cluster.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     7231 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_encode.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     3392 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_parsebam.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     3841 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_parsecontigs.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     5604 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_results.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    18325 2023-04-12 11:37:11.000000 vamb-4.1.0/test/test_vambtools.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1425 2023-04-12 11:37:11.000000 vamb-4.1.0/test/testtools.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-21 09:42:18.090484 vamb-4.1.0/vamb/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      941 2023-04-21 09:41:38.000000 vamb-4.1.0/vamb/__init__.py
+-rwxr-xr-x   0 jakni     (1000) jakni     (1000)    42915 2023-04-21 09:30:49.000000 vamb-4.1.0/vamb/__main__.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    17951 2023-04-21 09:30:49.000000 vamb-4.1.0/vamb/aamb_encode.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    25117 2023-04-19 06:13:21.000000 vamb-4.1.0/vamb/benchmark.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    19328 2023-04-21 09:30:49.000000 vamb-4.1.0/vamb/cluster.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    22117 2023-04-21 09:30:49.000000 vamb-4.1.0/vamb/encode.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    77187 2022-04-05 08:20:29.000000 vamb-4.1.0/vamb/kernel.npz
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     7902 2023-04-17 07:28:18.000000 vamb-4.1.0/vamb/parsebam.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     7041 2023-04-17 07:28:18.000000 vamb-4.1.0/vamb/parsecontigs.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    21213 2023-04-21 09:41:38.000000 vamb-4.1.0/vamb/vambtools.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-21 09:42:18.090484 vamb-4.1.0/vamb.egg-info/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      101 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/PKG-INFO
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      620 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/SOURCES.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)        1 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/dependency_links.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/entry_points.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/requires.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)        5 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/top_level.txt
```

### Comparing `vamb-4.0.1/LICENSE` & `vamb-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vamb-4.0.1/README.md` & `vamb-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vamb-4.0.1/pyproject.toml` & `vamb-4.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "vamb"
 dynamic = ["version"]
 dependencies = [
-    "numpy ~= 1.20",
-    "torch ~= 1.13",
-    "pycoverm ~= 0.6"
+    "numpy == 1.24.2",
+    "torch == 1.13.1",
+    "pycoverm == 0.6.0"
 ]
 # Currently pycoverm does not have binaries for Python > 3.11.
 # The dependency resolver, will not error on Python 3.11, but attempt
 # to build pycoverm from source, but will not get the deps required for that.
-requires-python = "<3.12.*,>=3.9.0"
+requires-python = "<3.12,>=3.9.0"
 scripts = {vamb = "vamb.__main__:main"}
 
 [metadata]
 authors = [
     {name="Jakob Nybo Nissen", email="jakobnybonissen@gmail.com"},
     {name="Pau Piera", email="pau.piera@cpr.ku.dk"},
     {name="Simon Rasmussen", email="simon.rasmussen@cpr.ku.dk"}
@@ -24,7 +24,10 @@
 [tool.setuptools.dynamic]
 version = {attr = "vamb.__version__"}
 readme = {file = "README.md"}
 
 [build-system]
 requires = ["setuptools ~= 63.0", "Cython ~= 0.29"]
 build-backend = "setuptools.build_meta"
+
+[tool.ruff]
+ignore = ["E501"]
```

### Comparing `vamb-4.0.1/src/_vambtools.pyx` & `vamb-4.1.0/src/_vambtools.pyx`

 * *Files identical despite different names*

### Comparing `vamb-4.0.1/src/concatenate.py` & `vamb-4.1.0/src/concatenate.py`

 * *Files identical despite different names*

### Comparing `vamb-4.0.1/test/testtools.py` & `vamb-4.1.0/test/testtools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import string
 import os
 
 import vamb
 
 PARENTDIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 DATADIR = os.path.join(PARENTDIR, "test", "data")
-BAM_FILES = [
-    os.path.join(DATADIR, "bam", i) for i in os.listdir(os.path.join(DATADIR, "bam"))
-]
+BAM_FILES = sorted(
+    [os.path.join(DATADIR, "bam", i) for i in os.listdir(os.path.join(DATADIR, "bam"))]
+)
 
 BAM_NAMES = [
     "S27C175628",
     "S27C95602",
     "S27C25358",
     "S26C115410",
     "S4C529736",
```

### Comparing `vamb-4.0.1/vamb/__init__.py` & `vamb-4.1.0/vamb/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,16 +15,26 @@
 3) Calculate a Composition of contigs using vamb.parsecontigs
 4) Create Abundance object from BAM files using vamb.parsebam
 5) Train autoencoder using vamb.encode
 6) Cluster latent representation using vamb.cluster
 7) Split bins using vamb.vambtools
 """
 
-__version__ = (4, 0, 1)
+__version__ = (4, 1, 0)
 
 from . import vambtools
 from . import parsebam
 from . import parsecontigs
 from . import cluster
 from . import benchmark
 from . import encode
 from . import aamb_encode
+
+__all__ = [
+    "vambtools",
+    "parsebam",
+    "parsecontigs",
+    "cluster",
+    "benchmark",
+    "encode",
+    "aamb_encode",
+]
```

### Comparing `vamb-4.0.1/vamb/__main__.py` & `vamb-4.1.0/vamb/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 os.environ["OMP_NUM_THREADS"] = str(DEFAULT_THREADS)
 
 # Append vamb to sys.path to allow vamb import even if vamb was not installed
 # using pip
 parentdir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 sys.path.append(parentdir)
 
+
 def try_make_dir(name):
     try:
         os.mkdir(name)
     except FileExistsError:
         pass
-    except:
-        raise
+
 
 class FASTAPath(type(Path())):
     pass
 
 
 class CompositionPath(type(Path())):
     pass
@@ -281,15 +281,15 @@
         self,
         encoder_options: EncoderOptions,
         vae_options: Optional[VAETrainingOptions],
         aae_options: Optional[AAETrainingOptions],
         lrate: float,
     ):
         assert isinstance(lrate, float)
-        
+
         assert (encoder_options.vae_options is None) == (vae_options is None)
         assert (encoder_options.aae_options is None) == (aae_options is None)
 
         if lrate <= 0.0:
             raise argparse.ArgumentTypeError("Learning rate must be positive")
         self.lrate = lrate
 
@@ -348,38 +348,42 @@
 
 class VambOptions:
     __slots__ = [
         "out_dir",
         "n_threads",
         "comp_options",
         "min_fasta_output_size",
+        "seed",
         "cuda",
     ]
 
     def __init__(
         self,
         out_dir: Path,
         n_threads: int,
         comp_options: CompositionOptions,
         min_fasta_output_size: Optional[int],
+        seed: int,
         cuda: bool,
     ):
         assert isinstance(out_dir, Path)
         assert isinstance(n_threads, int)
         assert isinstance(comp_options, CompositionOptions)
         assert isinstance(min_fasta_output_size, (int, type(None)))
+        assert isinstance(seed, int)
         assert isinstance(cuda, bool)
 
         # Outdir does not exist
         if out_dir.exists():
             raise FileExistsError(out_dir)
 
         # Outdir is in an existing parent dir
-        if not out_dir.parent.is_dir():
-            raise NotADirectoryError(parentdir)
+        parent_dir = out_dir.parent
+        if not parent_dir.is_dir():
+            raise NotADirectoryError(parent_dir)
         self.out_dir = out_dir
 
         if n_threads < 1:
             raise ValueError(f"Must pass at least 1 thread, not {n_threads}")
         self.n_threads = n_threads
 
         if min_fasta_output_size is not None:
@@ -394,14 +398,15 @@
                 )
         self.min_fasta_output_size = min_fasta_output_size
 
         if cuda and not torch.cuda.is_available():
             raise ModuleNotFoundError(
                 "Cuda is not available on your PyTorch installation"
             )
+        self.seed = seed
         self.cuda = cuda
 
 
 def log(string: str, logfile: IO[str], indent: int = 0):
     print(("\t" * indent) + string, file=logfile)
     logfile.flush()
 
@@ -445,27 +450,26 @@
 def calc_rpkm(
     abundance_options: AbundanceOptions,
     outdir: Path,
     comp_metadata: vamb.parsecontigs.CompositionMetaData,
     nthreads: int,
     logfile: IO[str],
 ) -> vamb.parsebam.Abundance:
-
     begintime = time.time()
     log("\nLoading depths", logfile)
     log(
         f'Reference hash: {comp_metadata.refhash.hex() if abundance_options.refcheck else "None"}',
         logfile,
         1,
     )
 
     path = abundance_options.path
     if isinstance(path, AbundancePath):
         log(f"Loading depths from npz array {str(path)}", logfile, 1)
-        
+
         abundance = vamb.parsebam.Abundance.load(
             path, comp_metadata.refhash if abundance_options.refcheck else None
         )
         # I don't want this check in any constructors of abundance, since the constructors
         # should be able to skip this check in case comp and abundance are independent.
         # But when running the main Vamb workflow, we need to assert this.
         if abundance.nseqs != comp_metadata.nseqs:
@@ -475,15 +479,15 @@
                 f"but composition has {comp_metadata.nseqs}."
             )
     else:
         assert isinstance(path, list)
         log(f"Parsing {len(path)} BAM files with {nthreads} threads", logfile, 1)
 
         abundance = vamb.parsebam.Abundance.from_files(
-            [str(i) for i in path],
+            path,
             outdir.joinpath("tmp").joinpath("pycoverm"),
             comp_metadata,
             abundance_options.refcheck,
             abundance_options.min_alignment_id,
             nthreads,
         )
         abundance.save(outdir.joinpath("abundance.npz"))
@@ -504,27 +508,27 @@
     training_options: VAETrainingOptions,
     vamb_options: VambOptions,
     lrate: float,
     alpha: Optional[float],
     data_loader: DataLoader,
     logfile: IO[str],
 ) -> np.ndarray:
-
     begintime = time.time()
     log("\nCreating and training VAE", logfile)
 
     nsamples = data_loader.dataset.tensors[0].shape[1]
     vae = vamb.encode.VAE(
         nsamples,
         nhiddens=vae_options.nhiddens,
         nlatent=vae_options.nlatent,
         alpha=alpha,
         beta=vae_options.beta,
         dropout=vae_options.dropout,
         cuda=vamb_options.cuda,
+        seed=vamb_options.seed,
     )
 
     log("Created VAE", logfile, 1)
     modelpath = vamb_options.out_dir.joinpath("model.pt")
     vae.trainmodel(
         vamb.encode.set_batchsize(data_loader, training_options.batchsize),
         nepochs=training_options.nepochs,
@@ -552,28 +556,28 @@
     training_options: AAETrainingOptions,
     vamb_options: VambOptions,
     lrate: float,
     alpha: Optional[float],  # set automatically if None
     logfile: IO[str],
     contignames: Sequence[str],
 ) -> tuple[np.ndarray, dict[str, set[str]]]:
-
     begintime = time.time()
     log("\nCreating and training AAE", logfile)
     nsamples = data_loader.dataset.tensors[0].shape[1]
 
     aae = vamb.aamb_encode.AAE(
         nsamples,
         aae_options.nhiddens,
         aae_options.nlatent_z,
         aae_options.nlatent_y,
         aae_options.sl,
         aae_options.slr,
         alpha,
         _cuda=vamb_options.cuda,
+        seed=vamb_options.seed,
     )
 
     log("Created AAE", logfile, 1)
     modelpath = os.path.join(vamb_options.out_dir, "aae_model.pt")
     aae.trainmodel(
         vamb.encode.set_batchsize(data_loader, training_options.batchsize),
         training_options.nepochs,
@@ -583,45 +587,47 @@
         logfile,
         modelpath,
     )
 
     print("", file=logfile)
     log("Encoding to latent representation", logfile, 1)
     clusters_y_dict, latent = aae.get_latents(contignames, data_loader)
-    vamb.vambtools.write_npz(os.path.join(vamb_options.out_dir, "aae_z_latent.npz"), latent)
+    vamb.vambtools.write_npz(
+        os.path.join(vamb_options.out_dir, "aae_z_latent.npz"), latent
+    )
 
     del aae  # Needed to free "latent" array's memory references?
 
     elapsed = round(time.time() - begintime, 2)
     log(f"Trained AAE and encoded in {elapsed} seconds.", logfile, 1)
 
     return latent, clusters_y_dict
 
 
 def cluster(
     cluster_options: ClusterOptions,
     clusterspath: Path,
     latent: np.ndarray,
     contignames: Sequence[str],  # of dtype object
-    cuda: bool,
+    vamb_options: VambOptions,
     logfile: IO[str],
     cluster_prefix: str,
 ) -> None:
     begintime = time.time()
 
     log("\nClustering", logfile)
     log(f"Windowsize: {cluster_options.window_size}", logfile, 1)
     log(
         f"Min successful thresholds detected: {cluster_options.min_successes}",
         logfile,
         1,
     )
     log(f"Max clusters: {cluster_options.max_clusters}", logfile, 1)
     log(f"Min cluster size: {cluster_options.min_cluster_size}", logfile, 1)
-    log(f"Use CUDA for clustering: {cuda}", logfile, 1)
+    log(f"Use CUDA for clustering: {vamb_options.cuda}", logfile, 1)
     log(
         "Separator: {}".format(
             None
             if cluster_options.binsplit_separator is None
             else ('"' + cluster_options.binsplit_separator + '"')
         ),
         logfile,
@@ -630,15 +636,16 @@
 
     cluster_generator = vamb.cluster.ClusterGenerator(
         latent,
         windowsize=cluster_options.window_size,
         minsuccesses=cluster_options.min_successes,
         destroy=True,
         normalized=False,
-        cuda=cuda,
+        cuda=vamb_options.cuda,
+        seed=vamb_options.seed,
     )
 
     renamed = (
         (str(cluster_index + 1), {contignames[i] for i in members})
         for (cluster_index, (_, members)) in enumerate(
             map(lambda x: x.as_tuple(), cluster_generator)
         )
@@ -745,21 +752,25 @@
         abundance_options,
         vamb_options.out_dir,
         composition.metadata,
         vamb_options.n_threads,
         logfile,
     )
     time_generating_input = round(time.time() - begintime, 2)
-    log(f"\nTNF and coabundances generated in {time_generating_input} seconds.", logfile, 1)
+    log(
+        f"\nTNF and coabundances generated in {time_generating_input} seconds.",
+        logfile,
+        1,
+    )
 
     data_loader, mask = vamb.encode.make_dataloader(
         abundance.matrix,
         composition.matrix,
         composition.metadata.lengths,
-        256, # dummy value - we change this before using the actual loader
+        256,  # dummy value - we change this before using the actual loader
         destroy=True,
         cuda=vamb_options.cuda,
     )
     composition.metadata.filter_mask(mask)
 
     print("", file=logfile)
     log("Created dataloader and mask", logfile, 0)
@@ -767,45 +778,41 @@
     n_discarded = len(mask) - mask.sum()
     log(f"Number of sequences unsuitable for encoding: {n_discarded}", logfile, 1)
     log(f"Number of sequences remaining: {len(mask) - n_discarded}", logfile, 1)
 
     latent = None
     if vae_options is not None:
         assert vae_training_options is not None
-        begin_train_vae = time.time()
         # Train, save model
         latent = trainvae(
             vae_options=vae_options,
             training_options=vae_training_options,
             vamb_options=vamb_options,
             lrate=training_options.lrate,
             alpha=encoder_options.alpha,
             data_loader=data_loader,
             logfile=logfile,
         )
-        time_training_vae = round(time.time() - begin_train_vae, 2)
         print("", file=logfile)
 
     clusters_y_dict = None
     latent_z = None
     if aae_options is not None:
         assert aae_training_options is not None
-        begin_train_aae = time.time()
         # Train, save model
         latent_z, clusters_y_dict = trainaae(
             data_loader=data_loader,
             aae_options=aae_options,
             vamb_options=vamb_options,
             training_options=aae_training_options,
             lrate=training_options.lrate,
             alpha=encoder_options.alpha,
             logfile=logfile,
             contignames=composition.metadata.identifiers,
         )
-        time_training_aae = round(time.time() - begin_train_aae, 2)
         print("", file=logfile)
 
     # Free up memory
     comp_metadata = composition.metadata
     del composition, abundance
 
     # Write contignames and contiglengths needed for dereplication purposes
@@ -822,19 +829,19 @@
         # Cluster, save tsv file
         clusterspath = vamb_options.out_dir.joinpath("vae_clusters.tsv")
         cluster(
             cluster_options,
             clusterspath,
             latent,
             comp_metadata.identifiers,
-            vamb_options.cuda,
+            vamb_options,
             logfile,
             "vae_",
         )
-        log(f"VAE latent clustered", logfile, 1)
+        log("VAE latent clustered", logfile, 1)
 
         del latent
         fin_cluster_latent = time.time()
 
         if vamb_options.min_fasta_output_size is not None:
             path = comp_options.path
             assert isinstance(path, FASTAPath)
@@ -860,21 +867,21 @@
         clusterspath = vamb_options.out_dir.joinpath("aae_z_clusters.tsv")
 
         cluster(
             cluster_options,
             clusterspath,
             latent_z,
             comp_metadata.identifiers,
-            vamb_options.cuda,
+            vamb_options,
             logfile,
-            "aae_z",
+            "aae_z_",
         )
 
         fin_cluster_latent_z = time.time()
-        log(f"AAE z latent clustered.", logfile, 1)
+        log("AAE z latent clustered.", logfile, 1)
 
         del latent_z
 
         if vamb_options.min_fasta_output_size is not None:
             path = comp_options.path
             assert isinstance(path, FASTAPath)
             write_fasta(
@@ -890,15 +897,17 @@
         time_writing_bins_z = time.time()
         writing_bins_time_z = round(time_writing_bins_z - fin_cluster_latent_z, 2)
         log(f"AAE z bins written in {writing_bins_time_z} seconds.", logfile, 1)
 
         clusterspath = vamb_options.out_dir.joinpath("aae_y_clusters.tsv")
         # Binsplit if given a separator
         if cluster_options.binsplit_separator is not None:
-            maybe_split = vamb.vambtools.binsplit(clusters_y_dict.items(), cluster_options.binsplit_separator)
+            maybe_split = vamb.vambtools.binsplit(
+                clusters_y_dict.items(), cluster_options.binsplit_separator
+            )
         else:
             maybe_split = clusters_y_dict.items()
         with open(clusterspath, "w") as clustersfile:
             clusternumber, ncontigs = vamb.vambtools.write_clusters(
                 clustersfile,
                 maybe_split,
                 max_clusters=cluster_options.max_clusters,
@@ -925,21 +934,22 @@
             )
         time_writing_bins_y = time.time()
         writing_bins_time_y = round(time_writing_bins_y - time_start_writin_z_bins, 2)
         log(f"AAE y bins written in {writing_bins_time_y} seconds.", logfile, 1)
 
     log(f"\nCompleted Vamb in {round(time.time() - begintime, 2)} seconds.", logfile, 0)
 
+
 def main():
     doc = f"""Avamb: Adversarial and Variational autoencoders for metagenomic binning.
-    
+
     Version: {'.'.join([str(i) for i in vamb.__version__])}
 
     Default use, good for most datasets:
-    vamb --outdir out --fasta my_contigs.fna --bamfiles *.bam -o C 
+    vamb --outdir out --fasta my_contigs.fna --bamfiles *.bam -o C
 
     For advanced use and extensions of Avamb, check documentation of the package
     at https://github.com/RasmussenLab/vamb."""  # must be updated with the new github
     parser = argparse.ArgumentParser(
         prog="vamb",
         description=doc,
         formatter_class=argparse.RawDescriptionHelpFormatter,
@@ -955,46 +965,58 @@
         action="version",
         version=f'Vamb {".".join(map(str, vamb.__version__))}',
     )
 
     # Positional arguments
     reqos = parser.add_argument_group(title="Output (required)", description=None)
     reqos.add_argument(
-        "--outdir", 
+        "--outdir",
         metavar="",
-        type=Path, 
-        required=True, 
-        help="output directory to create"
+        type=Path,
+        required=True,
+        help="output directory to create",
+    )
+
+    # Other arguments
+    otheros = parser.add_argument_group(title="Other options", description=None)
+    otheros.add_argument(
+        "--seed",
+        metavar="",
+        type=Optional[int],
+        default=0,
+        help="Random seed [random] (determinism not guaranteed)",
     )
 
     # TNF arguments
     tnfos = parser.add_argument_group(
         title="TNF input (either fasta or all .npz files required)"
     )
     tnfos.add_argument("--fasta", metavar="", type=Path, help="path to fasta file")
-    tnfos.add_argument("--composition", metavar="",type=Path, help="path to .npz of composition")
+    tnfos.add_argument(
+        "--composition", metavar="", type=Path, help="path to .npz of composition"
+    )
 
     # RPKM arguments
     rpkmos = parser.add_argument_group(
         title="RPKM input (either BAMs or .npz required)"
     )
     rpkmos.add_argument(
-        "--bamfiles", 
-        dest='bampaths',
-        metavar="", 
+        "--bamfiles",
+        dest="bampaths",
+        metavar="",
         type=Path,
-        help="paths to (multiple) BAM files", 
-        nargs="+"
+        help="paths to (multiple) BAM files",
+        nargs="+",
     )
     rpkmos.add_argument(
-        "--rpkm", 
+        "--rpkm",
         metavar="",
         dest="abundancepath",
-        type=Path,  
-        help="path to .npz of RPKM (abundances)"
+        type=Path,
+        help="path to .npz of RPKM (abundances)",
     )
 
     # Optional arguments
     inputos = parser.add_argument_group(title="IO options", description=None)
 
     inputos.add_argument(
         "-m",
@@ -1255,24 +1277,20 @@
 
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit()
 
     args = parser.parse_args()
 
-    comp_options = CompositionOptions(
-        args.fasta, args.composition, args.minlength
-
-    )
+    comp_options = CompositionOptions(args.fasta, args.composition, args.minlength)
 
     abundance_options = AbundanceOptions(
         args.bampaths,
         args.abundancepath,
         args.min_alignment_id,
-
         not args.norefcheck,
     )
 
     if args.model in ("vae", "vae-aae"):
         vae_options = VAEOptions(
             nhiddens=args.nhiddens,
             nlatent=args.nlatent,
@@ -1284,24 +1302,26 @@
             nepochs=args.nepochs, batchsize=args.batchsize, batchsteps=args.batchsteps
         )
     else:
         assert args.model == "aae"
         vae_options = None
         vae_training_options = None
 
-        for (name, arg, default) in [
+        for name, arg, default in [
             ("-n", args.nhiddens, None),
             ("-l", args.nlatent, 32),
             ("-b", args.beta, 200.0),
             ("-d", args.dropout, None),
             ("-t", args.batchsize, 256),
-            ("-q", args.batchsteps, [25, 75, 150, 225])
+            ("-q", args.batchsteps, [25, 75, 150, 225]),
         ]:
             if arg != default:
-                raise ValueError(f"VAE model not used, but VAE-specific arg \"{name}\" used")
+                raise ValueError(
+                    f'VAE model not used, but VAE-specific arg "{name}" used'
+                )
 
     if args.model in ("aae", "vae-aae"):
         aae_options = AAEOptions(
             nhiddens=args.nhiddens_aae,
             nlatent_z=args.nlatent_aae_z,
             nlatent_y=args.nlatent_aae_y,
             sl=args.sl,
@@ -1315,27 +1335,29 @@
             temp=args.temp,
         )
     else:
         assert args.model == "vae"
         aae_options = None
         aae_training_options = None
 
-        for (name, arg, default) in [
+        for name, arg, default in [
             ("--n_aae", args.nhiddens_aae, 547),
             ("--z_aae", args.nlatent_aae_z, 283),
             ("--y_aae", args.nlatent_aae_y, 700),
             ("--sl_aae", args.sl, 0.00964),
             ("--slr_aae", args.slr, 0.5),
             ("--aae_temp", args.temp, 0.1596),
             ("--e_aae", args.nepochs_aae, 70),
             ("--t_aae", args.batchsize_aae, 256),
             ("--q_aae", args.batchsteps_aae, [25, 50]),
         ]:
             if arg != default:
-                raise ValueError(f"AAE model not used, but AAE-specific arg \"{name}\" used")
+                raise ValueError(
+                    f'AAE model not used, but AAE-specific arg "{name}" used'
+                )
 
     encoder_options = EncoderOptions(
         vae_options=vae_options, aae_options=aae_options, alpha=args.alpha
     )
     training_options = TrainingOptions(
         encoder_options=encoder_options,
         vae_options=vae_training_options,
@@ -1348,26 +1370,25 @@
         args.min_successes,
         args.min_cluster_size,
         args.max_clusters,
         args.binsplit_separator,
     )
 
     vamb_options = VambOptions(
-        args.outdir, args.nthreads, comp_options, args.min_fasta_output_size, args.cuda
+        args.outdir,
+        args.nthreads,
+        comp_options,
+        args.min_fasta_output_size,
+        args.seed,
+        args.cuda,
     )
 
     torch.set_num_threads(vamb_options.n_threads)
 
     try_make_dir(vamb_options.out_dir)
-    try_make_dir(vamb_options.out_dir.joinpath("tmp"))
-
-    if aae_options is not None:
-        try_make_dir(vamb_options.out_dir.joinpath("tmp", "ripped_bins"))
-        try_make_dir(vamb_options.out_dir.joinpath("tmp", "checkm2_all"))
-        try_make_dir(vamb_options.out_dir.joinpath( "NC_bins"))
 
     with open(vamb_options.out_dir.joinpath("log.txt"), "w") as logfile:
         run(
             vamb_options=vamb_options,
             comp_options=comp_options,
             abundance_options=abundance_options,
             encoder_options=encoder_options,
```

### Comparing `vamb-4.0.1/vamb/aamb_encode.py` & `vamb-4.1.0/vamb/aamb_encode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 """Adversarial autoencoders (AAE) for metagenomics binning, this files contains the implementation of the AAE"""
 
 
 import numpy as np
 from math import log
 import time
-from torch.utils.data.dataset import TensorDataset as TensorDataset
 from torch.autograd import Variable
 from torch.distributions.relaxed_categorical import RelaxedOneHotCategorical
 import torch.nn as nn
 import torch.nn.functional as F
 import torch
 from vamb.encode import set_batchsize
 
 from collections.abc import Sequence
 from typing import Optional, IO, Union
 
-random_seed = 42
-torch.manual_seed(random_seed)
-torch.cuda.manual_seed(random_seed)
-torch.backends.cudnn.deterministic = True
-torch.backends.cudnn.benchmark = False
-np.random.seed(random_seed)
 
 ############################################################################# MODEL ###########################################################
 class AAE(nn.Module):
     def __init__(
         self,
         nsamples: int,
         nhiddens: int,
         nlatent_l: int,
         nlatent_y: int,
         sl: float,
         slr: float,
         alpha: Optional[float],
         _cuda: bool,
+        seed: int,
     ):
         if nsamples is None:
             raise ValueError(
                 f"Number of samples  should be provided to define the encoder input layer as well as the categorical latent dimension, not {nsamples}"
             )
 
+        torch.manual_seed(seed)
+        torch.cuda.manual_seed(seed)
+        torch.backends.cudnn.deterministic = True
+        torch.backends.cudnn.benchmark = False
+
         super(AAE, self).__init__()
         if alpha is None:
             alpha = 0.15 if nsamples > 1 else 0.50
 
         self.nsamples = nsamples
         input_len = 103 + self.nsamples
         self.h_n = nhiddens
         self.ld = nlatent_l
         self.y_len = nlatent_y
         self.input_len = int(input_len)
         self.sl = sl
         self.slr = slr
         self.alpha = alpha
         self.usecuda = _cuda
+        self.rng = np.random.Generator(np.random.PCG64(seed))
 
         # encoder
         self.encoder = nn.Sequential(
             nn.Linear(self.input_len, self.h_n),
             nn.BatchNorm1d(self.h_n),
             nn.LeakyReLU(),
             nn.Linear(self.h_n, self.h_n),
@@ -101,19 +101,18 @@
         )
 
         if _cuda:
             self.cuda()
 
     ## Reparametrisation trick
     def _reparameterization(self, mu, logvar):
-
         Tensor = torch.cuda.FloatTensor if self.usecuda else torch.FloatTensor
 
         std = torch.exp(logvar / 2)
-        sampled_z = Variable(Tensor(np.random.normal(0, 1, (mu.size(0), self.ld))))
+        sampled_z = Variable(Tensor(self.rng.normal(0, 1, (mu.size(0), self.ld))))
 
         if self.usecuda:
             sampled_z = sampled_z.cuda()
         z = sampled_z * std + mu
 
         return z
 
@@ -194,15 +193,14 @@
         nepochs: int,
         batchsteps: list[int],
         T,
         lr: float,
         logfile: Optional[IO[str]] = None,
         modelfile: Union[None, str, IO[bytes]] = None,
     ):
-
         Tensor = torch.cuda.FloatTensor if self.usecuda else torch.FloatTensor
         batchsteps_set = set(batchsteps)
         ncontigs, _ = data_loader.dataset.tensors[0].shape
 
         # Initialize generator and discriminator
 
         if logfile is not None:
@@ -286,15 +284,15 @@
                         torch.tensor([T], device="cuda"),
                         torch.ones([nrows, self.y_len], device="cuda"),
                     )
                     y_prior = ohc.sample()
                     y_prior = y_prior.cuda()
 
                 else:
-                    z_prior = Variable(Tensor(np.random.normal(0, 1, (nrows, self.ld))))
+                    z_prior = Variable(Tensor(self.rng.normal(0, 1, (nrows, self.ld))))
                     ohc = RelaxedOneHotCategorical(T, torch.ones([nrows, self.y_len]))
                     y_prior = ohc.sample()
 
                 del ohc
 
                 if self.usecuda:
                     depths_in = depths_in.cuda()
@@ -422,15 +420,17 @@
 
                 except:
                     pass
 
         return None
 
     ########### funciton that retrieves the clusters from Y latents
-    def get_latents(self, contignames: Sequence[str], data_loader, last_epoch: bool = True):
+    def get_latents(
+        self, contignames: Sequence[str], data_loader, last_epoch: bool = True
+    ):
         """Retrieve the categorical latent representation (y) and the contiouous latents (l) of the inputs
 
         Inputs:
             dataloader
             contignames
             last_epoch
 
@@ -446,42 +446,39 @@
         length = len(depths_array)
         latent = np.empty((length, self.ld), dtype=np.float32)
         index_contigname = 0
         row = 0
         clust_y_dict = dict()
         Tensor = torch.cuda.FloatTensor if self.usecuda else torch.FloatTensor
         with torch.no_grad():
-
             for depths_in, tnfs_in, _ in new_data_loader:
                 nrows, _ = depths_in.shape
                 if self.usecuda:
                     z_prior = torch.cuda.FloatTensor(nrows, self.ld).normal_()
                     z_prior.cuda()
                     ohc = RelaxedOneHotCategorical(
                         torch.tensor([0.15], device="cuda"),
                         torch.ones([nrows, self.y_len], device="cuda"),
                     )
                     y_prior = ohc.sample()
                     y_prior = y_prior.cuda()
 
                 else:
-                    z_prior = Variable(Tensor(np.random.normal(0, 1, (nrows, self.ld))))
+                    z_prior = Variable(Tensor(self.rng.normal(0, 1, (nrows, self.ld))))
                     ohc = RelaxedOneHotCategorical(
                         0.15, torch.ones([nrows, self.y_len])
                     )
                     y_prior = ohc.sample()
 
                 if self.usecuda:
                     depths_in = depths_in.cuda()
                     tnfs_in = tnfs_in.cuda()
 
                 if last_epoch:
-                    mu, _, _, _, y_sample = self(depths_in, tnfs_in)[
-                        0:5
-                    ]
+                    mu, _, _, _, y_sample = self(depths_in, tnfs_in)[0:5]
                 else:
                     y_sample = self(depths_in, tnfs_in)[4]
 
                 if self.usecuda:
                     Ys = y_sample.cpu().detach().numpy()
                     if last_epoch:
                         mu = mu.cpu().detach().numpy()
```

### Comparing `vamb-4.0.1/vamb/benchmark.py` & `vamb-4.1.0/vamb/benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         return result
 
     def _finalize(self, genomeof: dict[Contig, Genome]) -> None:
         self.intersections.clear()
         by_source: defaultdict[tuple[Genome, str], list[Contig]] = defaultdict(list)
         for contig in self.contigs:
             by_source[(genomeof[contig], contig.subject)].append(contig)
-        for ((genome, _), contigs) in by_source.items():
+        for (genome, _), contigs in by_source.items():
             self.intersections[genome] = self.intersections.get(
                 genome, 0
             ) + self._intersection(contigs)
         self.breadth = sum(self.intersections.values())
 
     def confusion_matrix(self, genome: Genome) -> tuple[int, int, int]:
         "Given a genome and a binname, returns TP, FP, FN"
@@ -349,69 +349,69 @@
         if binsplit_sep is not None:
             clusters = vambtools.binsplit(clusters, binsplit_sep)
         return self.load_bins(clusters)
 
     def load_bins(self, bins: Iterable[tuple[str, Iterable[str]]]) -> list[Bin]:
         """Convert a set of bin names to a list of Bins"""
         result: list[Bin] = list()
-        for (binname, contignames) in bins:
+        for binname, contignames in bins:
             contigs = (self.contig_by_name[name] for name in contignames)
             result.append(Bin.from_contigs(binname, contigs, self.genomeof))
 
         return result
 
     @classmethod
     def from_file(cls: type[R], io: IO[str]) -> R:
         json_dict = json.load(io)
         return cls.from_dict(json_dict)
 
     @classmethod
     def from_dict(cls: type[R], json_dict: dict[str, Any]) -> R:
         instance = cls()
-        for (genomename, sourcesdict) in json_dict["genomes"].items():
+        for genomename, sourcesdict in json_dict["genomes"].items():
             genome = Genome(genomename)
             instance._add_genome(genome)
-            for (sourcename, (sourcelen, contigdict)) in sourcesdict.items():
+            for sourcename, (sourcelen, contigdict) in sourcesdict.items():
                 genome.add(sourcename, sourcelen)
-                for (contigname, (start, end)) in contigdict.items():
+                for contigname, (start, end) in contigdict.items():
                     # JSON format is 1-indexed and includes endpoints, whereas
                     # Contig struct is not, so compensate.
                     contig = Contig(contigname, sourcename, start - 1, end)
                     instance._add_contig(contig, genome)
 
         for _ in range(len(json_dict["taxmaps"]) - 1):
             instance.taxmaps.append(dict())
-        for (level, taxmap) in enumerate(json_dict["taxmaps"]):
-            for (child, parent) in taxmap.items():
+        for level, taxmap in enumerate(json_dict["taxmaps"]):
+            for child, parent in taxmap.items():
                 instance._add_taxonomy(level, child, parent)
 
         return instance
 
     def save(self, io: IO[str]) -> None:
         json_dict: dict[str, Any] = {"genomes": dict(), "taxmaps": []}
 
         # "genomes": {genomename: [subject_len, {contigname: [start, stop]}]}
         genome_dict = json_dict["genomes"]
         for genome in self.genomes:
             source_dict: dict[str, list[Any]] = dict()
             genome_dict[genome.name] = source_dict
-            for (sourcename, length) in genome.sources.items():
+            for sourcename, length in genome.sources.items():
                 source_dict[sourcename] = [length, dict()]
 
-        for (contig, genome) in self.genomeof.items():
+        for contig, genome in self.genomeof.items():
             # JSON format is 1-indexes and includes endpoints, whereas
             # Contig struct is not, so compensate.
             genome_dict[genome.name][contig.subject][1][contig.name] = [
                 contig.start + 1,
                 contig.end,
             ]
 
         for taxmap in self.taxmaps:
             d: dict[str, str] = dict()
-            for (child, parent) in taxmap.items():
+            for child, parent in taxmap.items():
                 if parent is not None:
                     d[child] = parent
             if len(d) > 0:
                 json_dict["taxmaps"].append(d)
 
         json.dump(json_dict, io)
 
@@ -577,18 +577,18 @@
     def _get_seen_bitvectors(
         self, rp_by_name: dict[str, dict[Bin, tuple[float, float]]]
     ) -> dict[str, int]:
         recalls: tuple[float] = self.recalls
         precisions: tuple[float] = self.precisions
         bitvectors: dict[str, int] = dict()
 
-        for (cladename, d) in rp_by_name.items():
+        for cladename, d in rp_by_name.items():
             bitvector = 0
-            for (recall, precision) in d.values():
-                for (i, (min_recall, min_precision)) in enumerate(
+            for recall, precision in d.values():
+                for i, (min_recall, min_precision) in enumerate(
                     product(recalls, precisions)
                 ):
                     if recall >= min_recall and precision >= min_precision:
                         bitvector |= 1 << i
                     # Shortcut: Once we pass min recall, rest of values can be skipped
                     elif recall < min_recall:
                         break
@@ -601,31 +601,31 @@
         self, bitvectors: dict[str, int]
     ) -> dict[tuple[float, float], int]:
         recalls: tuple[float] = self.recalls
         precisions: tuple[float] = self.precisions
         result: dict[tuple[float, float], int] = {
             (r, p): 0 for (r, p) in product(recalls, precisions)
         }
-        for (_, bitvector) in bitvectors.items():
-            for (i, rp) in enumerate(product(recalls, precisions)):
+        for _, bitvector in bitvectors.items():
+            for i, rp in enumerate(product(recalls, precisions)):
                 result[rp] += (bitvector >> i) & 1
 
         return result
 
     def _uprank_rp_by_name(
         self, fromrank: int, rp_by_name: dict[str, dict[Bin, tuple[float, float]]]
     ) -> dict[str, dict[Bin, tuple[float, float]]]:
         result: dict[str, dict[Bin, tuple[float, float]]] = dict()
-        for (child, parent) in self.reference.taxmaps[fromrank].items():
+        for child, parent in self.reference.taxmaps[fromrank].items():
             # If no parent clade, we just name the "parent" same as child
             if parent is None:
                 parent = child
 
             if parent not in result:
                 result[parent] = dict()
 
             parent_dict = result[parent]
-            for (bin, (old_recall, old_prec)) in rp_by_name[child].items():
+            for bin, (old_recall, old_prec) in rp_by_name[child].items():
                 (new_recall, new_prec) = parent_dict.get(bin, (0.0, 0.0))
                 parent_dict[bin] = (max(old_recall, new_recall), old_prec + new_prec)
 
         return result
```

### Comparing `vamb-4.0.1/vamb/cluster.py` & `vamb-4.1.0/vamb/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,37 +202,38 @@
         matrix: _np.ndarray,
         maxsteps: int = 25,
         windowsize: int = 200,
         minsuccesses: int = 20,
         destroy: bool = False,
         normalized: bool = False,
         cuda: bool = False,
+        seed: int = 0,
     ):
         self._check_params(matrix, maxsteps, windowsize, minsuccesses)
         if not destroy:
             matrix = matrix.copy()
 
         # Shuffle matrix in unison to prevent seed sampling bias. Indices keeps
         # track of which points are which.
-        _np.random.RandomState(0).shuffle(matrix)
-        indices = _np.random.RandomState(0).permutation(len(matrix))
+        _np.random.Generator(_np.random.PCG64(seed)).shuffle(matrix)
+        indices = _np.random.Generator(_np.random.PCG64(seed)).permutation(len(matrix))
         indices = _torch.from_numpy(indices)
         torch_matrix = _torch.from_numpy(matrix)
 
         if not normalized:
             _normalize(torch_matrix, inplace=True)
 
         # Move to GPU
         if cuda:
             torch_matrix = torch_matrix.cuda()
 
         self.maxsteps: int = maxsteps
         self.minsuccesses: int = minsuccesses
         self.cuda: bool = cuda
-        self.rng: _random.Random = _random.Random(0)
+        self.rng: _random.Random = _random.Random(seed)
 
         self.matrix = torch_matrix
         # This refers to the indices of the original matrix. As we remove points, these
         # indices do not correspond to merely range(len(matrix)) anymore.
         self.indices = indices
         self.seed = -1
         self.nclusters = 0
@@ -281,15 +282,15 @@
         # Keep looping until we find a cluster
         distances = None
         while threshold is None:
             # If on GPU, we need to take next seed which has not already been clusted out.
             # if not, clustered points have been removed, so we can just take next seed
             if self.cuda:
                 self.seed = (self.seed + 1) % len(self.matrix)
-                while self.kept_mask[self.seed] == False:
+                while not self.kept_mask[self.seed]:
                     self.seed = (self.seed + 1) % len(self.matrix)
             else:
                 self.seed = (self.seed + 1) % len(self.matrix)
 
             medoid, distances = _wander_medoid(
                 self.matrix,
                 self.kept_mask,
@@ -448,15 +449,16 @@
     return threshold, success
 
 
 def _smaller_indices(
     tensor: _Tensor, kept_mask: _Tensor, threshold: float, cuda: bool
 ) -> _Tensor:
     """Get all indices where the tensor is smaller than the threshold.
-    Uses Numpy because Torch is slow - See https://github.com/pytorch/pytorch/pull/15190"""
+    Uses Numpy because Torch is slow - See https://github.com/pytorch/pytorch/pull/15190
+    """
 
     # If it's on GPU, we remove the already clustered points at this step.
     if cuda:
         return _torch.nonzero((tensor <= threshold) & kept_mask).flatten().cpu()
     else:
         arr = tensor.numpy()
         indices = (arr <= threshold).nonzero()[0]
```

### Comparing `vamb-4.0.1/vamb/encode.py` & `vamb-4.1.0/vamb/encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,32 +24,34 @@
 """
 
 __cmd_doc__ = """Encode depths and TNF using a VAE to latent representation"""
 
 import numpy as _np
 import torch as _torch
 
-_torch.manual_seed(0)
 
-def set_batchsize(data_loader: _DataLoader, batch_size: int, encode=False) -> _DataLoader:
+def set_batchsize(
+    data_loader: _DataLoader, batch_size: int, encode=False
+) -> _DataLoader:
     """Effectively copy the data loader, but with a different batch size.
 
     The `encode` option is used to copy the dataloader to use before encoding.
     This will not drop the last minibatch whose size may not be the requested
     batch size, and will also not shuffle the data.
     """
     return _DataLoader(
         dataset=data_loader.dataset,
-        batch_size= batch_size,
+        batch_size=batch_size,
         shuffle=not encode,
         drop_last=not encode,
         num_workers=1 if encode else data_loader.num_workers,
         pin_memory=data_loader.pin_memory,
     )
 
+
 def make_dataloader(
     rpkm: _np.ndarray,
     tnf: _np.ndarray,
     lengths: _np.ndarray,
     batchsize: int = 256,
     destroy: bool = False,
     cuda: bool = False,
@@ -183,14 +185,15 @@
         nsamples: int,
         nhiddens: Optional[list[int]] = None,
         nlatent: int = 32,
         alpha: Optional[float] = None,
         beta: float = 200.0,
         dropout: Optional[float] = 0.2,
         cuda: bool = False,
+        seed: int = 0,
     ):
         if nlatent < 1:
             raise ValueError(f"Minimum 1 latent neuron, not {nlatent}")
 
         if nsamples < 1:
             raise ValueError(f"nsamples must be > 0, not {nsamples}")
 
@@ -212,14 +215,15 @@
 
         if not (0 < alpha < 1):
             raise ValueError(f"alpha must be 0 < alpha < 1, not {alpha}")
 
         if not (0 <= dropout < 1):
             raise ValueError(f"dropout must be 0 <= dropout < 1, not {dropout}")
 
+        _torch.manual_seed(seed)
         super(VAE, self).__init__()
 
         # Initialize simple attributes
         self.usecuda = cuda
         self.nsamples = nsamples
         self.ntnf = 103
         self.alpha = alpha
@@ -369,15 +373,15 @@
 
         epoch_loss = 0.0
         epoch_kldloss = 0.0
         epoch_sseloss = 0.0
         epoch_celoss = 0.0
 
         if epoch in batchsteps:
-            data_loader =  set_batchsize(data_loader, data_loader.batch_size * 2)
+            data_loader = set_batchsize(data_loader, data_loader.batch_size * 2)
 
         for depths_in, tnf_in, weights in data_loader:
             depths_in.requires_grad = True
             tnf_in.requires_grad = True
 
             if self.usecuda:
                 depths_in = depths_in.cuda()
@@ -424,15 +428,17 @@
         Input: data_loader: As generated by train_vae
 
         Output: A (n_contigs x n_latent) Numpy array of latent repr.
         """
 
         self.eval()
 
-        new_data_loader = set_batchsize(data_loader, data_loader.batch_size, encode=True)
+        new_data_loader = set_batchsize(
+            data_loader, data_loader.batch_size, encode=True
+        )
 
         depths_array, _, _ = data_loader.dataset.tensors
         length = len(depths_array)
 
         # We make a Numpy array instead of a Torch array because, if we create
         # a Torch array, then convert it to Numpy, Numpy will believe it doesn't
         # own the memory block, and array resizes will not be permitted.
```

### Comparing `vamb-4.0.1/vamb/kernel.npz` & `vamb-4.1.0/vamb/kernel.npz`

 * *Files identical despite different names*

### Comparing `vamb-4.0.1/vamb/parsebam.py` & `vamb-4.1.0/vamb/parsebam.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pycoverm
 import os as _os
 import numpy as _np
 from math import isfinite
 from vamb.parsecontigs import CompositionMetaData
 from vamb import vambtools
 from typing import Optional, TypeVar, Union, IO, Sequence
-from collections.abc import Iterator
 from pathlib import Path
 import shutil
 
 _ncpu = _os.cpu_count()
 DEFAULT_THREADS = 8 if _ncpu is None else _ncpu
 
 A = TypeVar("A", bound="Abundance")
@@ -54,16 +53,17 @@
 
     @staticmethod
     def verify_refhash(refhash: bytes, target_refhash: bytes) -> None:
         if refhash != target_refhash:
             raise ValueError(
                 f"At least one BAM file reference name hash to {refhash.hex()}, "
                 f"expected {target_refhash.hex()}. "
-                "Make sure all BAM and FASTA headers are identical "
-                "and in the same order."
+                "Make sure all BAM and FASTA identifiers are identical "
+                "and in the same order. "
+                "Note that the identifier is the header before any whitespace."
             )
 
     def save(self, io: Union[Path, IO[bytes]]):
         _np.savez_compressed(
             io,
             matrix=self.matrix,
             samplenames=self.samplenames,
@@ -86,15 +86,15 @@
             cls.verify_refhash(abundance.refhash, refhash)
 
         return abundance
 
     @classmethod
     def from_files(
         cls: type[A],
-        paths: list[str],
+        paths: list[Path],
         cache_directory: Optional[Path],
         comp_metadata: CompositionMetaData,
         verify_refhash: bool,
         minid: float,
         nthreads: int,
     ) -> A:
         """Input:
@@ -113,15 +113,15 @@
         # (issue #7). Can be solved by setting it to a low value
         minid = minid if minid > 0.001 else 0.001
 
         for path in paths:
             if not _os.path.isfile(path):
                 raise FileNotFoundError(path)
 
-            if not pycoverm.is_bam_sorted(path):
+            if not pycoverm.is_bam_sorted(str(path)):
                 raise ValueError(f"Path {path} is not sorted by reference.")
 
         if nthreads < 1:
             raise ValueError(f"nthreads must be > 0, not {nthreads}")
 
         chunksize = min(nthreads, len(paths))
 
@@ -134,15 +134,15 @@
         if chunksize >= len(paths):
             (matrix, refhash) = cls.run_pycoverm(
                 paths,
                 minid,
                 comp_metadata.refhash if verify_refhash else None,
                 comp_metadata.mask,
             )
-            return cls(matrix, paths, minid, refhash)
+            return cls(matrix, [str(p) for p in paths], minid, refhash)
         # Else, we load it in chunks, then assemble afterwards
         else:
             if cache_directory is None:
                 raise ValueError(
                     "If min(16, nthreads) < len(paths), cache_directory must not be None"
                 )
             return cls.chunkwise_loading(
@@ -153,15 +153,15 @@
                 comp_metadata.refhash if verify_refhash else None,
                 comp_metadata.mask,
             )
 
     @classmethod
     def chunkwise_loading(
         cls: type[A],
-        paths: list[str],
+        paths: list[Path],
         cache_directory: Path,
         nthreads: int,
         minid: float,
         target_refhash: Optional[bytes],
         mask: _np.ndarray,
     ) -> A:
         _os.mkdir(cache_directory)
@@ -172,42 +172,42 @@
         filenames = [
             _os.path.join(cache_directory, str(i) + ".npz") for i in range(len(chunks))
         ]
         assert len(chunks) > 1
 
         # Load from BAM and store them chunkwise
         refhash = None
-        for (filename, (chunkstart, chunkstop)) in zip(filenames, chunks):
+        for filename, (chunkstart, chunkstop) in zip(filenames, chunks):
             (matrix, refhash) = cls.run_pycoverm(
                 paths[chunkstart:chunkstop],
                 minid,
                 target_refhash,
                 mask,
             )
             vambtools.write_npz(filename, matrix)
 
         # Initialize matrix, the load them chunkwise. Delete the temp files when done
         matrix = _np.empty((mask.sum(), len(paths)), dtype=_np.float32)
-        for (filename, (chunkstart, chunkstop)) in zip(filenames, chunks):
+        for filename, (chunkstart, chunkstop) in zip(filenames, chunks):
             matrix[:, chunkstart:chunkstop] = vambtools.read_npz(filename)
 
         shutil.rmtree(cache_directory)
 
         assert refhash is not None
-        return cls(matrix, paths, minid, refhash)
+        return cls(matrix, [str(p) for p in paths], minid, refhash)
 
     @staticmethod
     def run_pycoverm(
-        paths: list[str],
+        paths: list[Path],
         minid: float,
         target_refhash: Optional[bytes],
         mask: _np.ndarray,
     ) -> tuple[_np.ndarray, bytes]:
         (headers, coverage) = pycoverm.get_coverages_from_bam(
-            paths,
+            [str(p) for p in paths],
             threads=len(paths),
             min_identity=minid,
             # Note: pycoverm's trim_upper=0.1 is same as CoverM trim-upper 90.
             trim_upper=0.1,
             trim_lower=0.1,
         )
```

### Comparing `vamb-4.0.1/vamb/parsecontigs.py` & `vamb-4.1.0/vamb/parsecontigs.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
             raw.extend(entry.kmercounts(4))
 
             if len(raw) > 256000:
                 Composition._convert(raw, projected)
 
             lengths.append(len(entry))
-            contignames.append(entry.header)
+            contignames.append(entry.identifier)
 
         # Convert rest of contigs
         Composition._convert(raw, projected)
         tnfs_arr = projected.take()
 
         # Don't use reshape since it creates a new array object with shared memory
         tnfs_arr.shape = (len(tnfs_arr) // 103, 103)
```

### Comparing `vamb-4.0.1/vamb/vambtools.py` & `vamb-4.1.0/vamb/vambtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,15 +430,15 @@
     Inputs:
         directory: Directory to create or put files in
         bins: dict[str: set[str]] (can be loaded from
         clusters.tsv using vamb.cluster.read_clusters)
         fastaio: bytes iterator containing FASTA file with all sequences
         maxbins: None or else raise an error if trying to make more bins than this [250]
         minsize: Minimum number of nucleotides in cluster to be output [0]
-        separator: string that separates the contig/cluster name from the sample ; i.e. sample_id_separator_contig_name/cluster_name 
+        separator: string that separates the contig/cluster name from the sample ; i.e. sample_id_separator_contig_name/cluster_name
     Output: None
     """
 
     # Safety measure so someone doesn't accidentally make 50000 tiny bins
     # If you do this on a compute cluster it can grind the entire cluster to
     # a halt and piss people off like you wouldn't believe.
     if maxbins is not None and len(bins) > maxbins:
@@ -466,16 +466,14 @@
         )
 
     # Make the directory if it does not exist - if it does, do nothing
     try:
         _os.mkdir(directory)
     except FileExistsError:
         pass
-    except:
-        raise
 
     # Now actually print all the contigs to files
     for binname, contigs in bins.items():
         size = 0
         if separator is not None:
             binsample = next(iter(contigs)).split(separator)[0]
         else:
@@ -489,24 +487,22 @@
             size += byteslen[1]
 
         if size < minsize:
             continue
 
         # Split bin files into sample dirs
         if binsample is not None:
-            bin_dir = _os.path.join(directory,binsample)
+            bin_dir = _os.path.join(directory, binsample)
             try:
                 _os.mkdir(bin_dir)
             except FileExistsError:
                 pass
-            except:
-                raise
         else:
             bin_dir = directory
-    
+
         # Print bin to file
         filename = _os.path.join(bin_dir, binname + ".fna")
 
         with open(filename, "wb") as file:
             for contig in contigs:
                 file.write(_gzip.decompress(byteslen_by_id[contig][0]))
                 file.write(b"\n")
@@ -562,18 +558,17 @@
         minlength: Minimum contig length to keep [2000]
         rename: Rename headers
 
     Output: None
     """
 
     identifiers: set[str] = set()
-    for (inpathno, inpath) in enumerate(inpaths):
+    for inpathno, inpath in enumerate(inpaths):
         try:
             with Reader(inpath) as infile:
-
                 # If we rename, seq identifiers only have to be unique for each sample
                 if rename:
                     identifiers.clear()
 
                 for entry in byte_iterfasta(infile):
                     if len(entry) < minlength:
                         continue
```

