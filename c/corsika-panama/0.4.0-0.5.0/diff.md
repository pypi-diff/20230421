# Comparing `tmp/corsika_panama-0.4.0.tar.gz` & `tmp/corsika_panama-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corsika_panama-0.4.0.tar", max compression
+gzip compressed data, was "corsika_panama-0.5.0.tar", max compression
```

## Comparing `corsika_panama-0.4.0.tar` & `corsika_panama-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/LICENSE
--rw-r--r--   0        0        0     5625 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/README.md
--rw-r--r--   0        0        0      362 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/__init__.py
--rw-r--r--   0        0        0       41 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/cli/__init__.py
--rwxr-xr-x   0        0        0      616 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/cli/cli.py
--rw-r--r--   0        0        0     1749 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/cli/corsika_to_hdf5.py
--rw-r--r--   0        0        0     3984 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/cli/run.py
--rw-r--r--   0        0        0      883 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/constants.py
--rw-r--r--   0        0        0      175 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/fluxes/__init__.py
--rw-r--r--   0        0        0     6930 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/fluxes/fluxes.py
--rw-r--r--   0        0        0     1633 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/nbstreamreader.py
--rw-r--r--   0        0        0     3227 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/prompt.py
--rw-r--r--   0        0        0    15063 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/read.py
--rw-r--r--   0        0        0     8417 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/run.py
--rw-r--r--   0        0        0     3110 2023-04-17 00:45:53.551427 corsika_panama-0.4.0/panama/weights.py
--rw-r--r--   0        0        0     2348 2023-04-17 00:45:53.555426 corsika_panama-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6736 1970-01-01 00:00:00.000000 corsika_panama-0.4.0/setup.py
--rw-r--r--   0        0        0     6674 1970-01-01 00:00:00.000000 corsika_panama-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5625 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/README.md
+-rw-r--r--   0        0        0      364 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/panama/__init__.py
+-rw-r--r--   0        0        0       41 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/panama/cli/__init__.py
+-rwxr-xr-x   0        0        0      616 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/panama/cli/cli.py
+-rw-r--r--   0        0        0     1749 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/panama/cli/corsika_to_hdf5.py
+-rw-r--r--   0        0        0     3984 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/panama/cli/run.py
+-rw-r--r--   0        0        0      883 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/panama/constants.py
+-rw-r--r--   0        0        0      170 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/panama/fluxes/__init__.py
+-rw-r--r--   0        0        0     7326 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/panama/fluxes/cosmic_ray_fluxes.py
+-rw-r--r--   0        0        0     2575 2023-04-21 14:47:33.966777 corsika_panama-0.5.0/panama/fluxes/flux.py
+-rw-r--r--   0        0        0   279551 2023-04-21 14:47:33.970777 corsika_panama-0.5.0/panama/fluxes/gsf_data_table.txt
+-rw-r--r--   0        0        0     1865 2023-04-21 14:47:33.970777 corsika_panama-0.5.0/panama/fluxes/muon_fluxes.py
+-rw-r--r--   0        0        0     1633 2023-04-21 14:47:33.970777 corsika_panama-0.5.0/panama/nbstreamreader.py
+-rw-r--r--   0        0        0     3227 2023-04-21 14:47:33.970777 corsika_panama-0.5.0/panama/prompt.py
+-rw-r--r--   0        0        0    15035 2023-04-21 14:47:33.970777 corsika_panama-0.5.0/panama/read.py
+-rw-r--r--   0        0        0     8412 2023-04-21 14:47:33.970777 corsika_panama-0.5.0/panama/run.py
+-rw-r--r--   0        0        0     3605 2023-04-21 14:47:33.970777 corsika_panama-0.5.0/panama/weights.py
+-rw-r--r--   0        0        0     2362 2023-04-21 14:47:33.970777 corsika_panama-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6737 1970-01-01 00:00:00.000000 corsika_panama-0.5.0/setup.py
+-rw-r--r--   0        0        0     6675 1970-01-01 00:00:00.000000 corsika_panama-0.5.0/PKG-INFO
```

### Comparing `corsika_panama-0.4.0/LICENSE` & `corsika_panama-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.4.0/README.md` & `corsika_panama-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.4.0/panama/cli/cli.py` & `corsika_panama-0.5.0/panama/cli/cli.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.4.0/panama/cli/corsika_to_hdf5.py` & `corsika_panama-0.5.0/panama/cli/corsika_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.4.0/panama/cli/run.py` & `corsika_panama-0.5.0/panama/cli/run.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.4.0/panama/constants.py` & `corsika_panama-0.5.0/panama/constants.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.4.0/panama/nbstreamreader.py` & `corsika_panama-0.5.0/panama/nbstreamreader.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.4.0/panama/prompt.py` & `corsika_panama-0.5.0/panama/prompt.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.4.0/panama/read.py` & `corsika_panama-0.5.0/panama/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
         df_event_headers = pd.DataFrame(np.array(event_headers))
         valid_columns = [
             v[1] // CORSIKA_FIELD_BYTE_LEN
             for v in list(event_header_types[version].fields.values())
         ]
         valid_names = event_header_types[version].names
 
-        mapper = dict(zip(valid_columns, valid_names))  # noqa: B905
+        mapper = dict(zip(valid_columns, valid_names))
 
         df_event_headers.drop(
             columns=df_event_headers.columns.difference(valid_columns), inplace=True
         )
         df_event_headers.rename(columns=mapper, inplace=True)
         df_event_headers["run_number"] = df_event_headers["run_number"].astype(int)
         df_event_headers["event_number"] = df_event_headers["event_number"].astype(int)
@@ -232,15 +232,15 @@
 
         valid_columns = [
             v[1] // CORSIKA_FIELD_BYTE_LEN
             for v in list(particle_data_dtype.fields.values())
         ]
         valid_names = particle_data_dtype.names
 
-        mapper = dict(zip(valid_columns, valid_names))  # noqa: B905
+        mapper = dict(zip(valid_columns, valid_names))
 
         df_particles.drop(
             columns=df_particles.columns.difference(valid_columns), inplace=True
         )
         df_particles.rename(columns=mapper, inplace=True)
         df_particles.query("particle_description != 0", inplace=True)
     else:
```

### Comparing `corsika_panama-0.4.0/panama/run.py` & `corsika_panama-0.5.0/panama/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
         n_update: The number of showers finished since last poll or None if process is finished
         """
         if self.running is None:
             return None
 
         if (return_code := self.running.poll()) is not None:
             if return_code != 0:
-                logging.warning(
-                    f"Return code of corsika not 0, but {return_code} (should not be possible)"
+                logging.error(
+                    f"Return code of corsika is {return_code}. This indicates a failed run."
                 )
 
             return self.join()
 
         finished = 0
 
         assert self.stream is not None
```

### Comparing `corsika_panama-0.4.0/panama/weights.py` & `corsika_panama-0.5.0/panama/weights.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 """
 Functions to add weights to the read in corsika dataframe
 """
 from typing import Any
 
 import numpy as np
 import pandas as pd
+from particle import PDGID, Corsika7ID
 
-from .fluxes import FastHillasGaisser2012, FastPrimaryFlux
+from .fluxes import CosmicRayFlux, H3a
 
-DEFAULT_FLUX = FastHillasGaisser2012(model="H3a")
+DEFAULT_FLUX = H3a()
 
 
-def add_weight(
+def get_weights(
     df_run: pd.DataFrame,
     df_event: pd.DataFrame,
     df: pd.DataFrame,
-    model: FastPrimaryFlux = DEFAULT_FLUX,
-) -> None:
+    model: CosmicRayFlux = DEFAULT_FLUX,
+) -> pd.DataFrame:
     """
     Adds the column "weight" too df_particle to reweight for given primary flux.
 
     Parameters
     ----------
     df_run: The run dataframe (as returned by `read_corsika_particle_files_to_dataframe`)
     df_event: The event dataframe (as returned by `read_corsika_particle_files_to_dataframe`)
     df: The particle dataframe (as returned by `read_corsika_particle_files_to_dataframe`)
     model: The Cosmic Ray primary flux model (instance of CRFlux)
+
+    Returns
+    -------
+    weights: A dataframe with the weights labeled by the run and event index.
+    Can be used like this: `df['weights'] = panama.get_weights(df_run, df_event, df)`
     """
     if not df_event.index.is_monotonic_increasing:
         df_event.sort_index(inplace=True)
     if not df.index.is_monotonic_increasing:
         df.sort_index(inplace=True)
     primary_pids = df_event["particle_id"].unique()
     energy_slopes = df_run["energy_spectrum_slope"].unique()
@@ -47,46 +53,61 @@
         N = np.log(emax / emin)
     else:
         ep = energy_slope + 1
         N = (emax**ep - emin**ep) / ep
 
     weights = []
     for primary_pid in primary_pids:
+        pdgid = Corsika7ID(primary_pid).to_pdgid()
 
-        def flux(E: Any, primary_pid: Any = primary_pid) -> Any:
-            return model.nucleus_flux(primary_pid, E)
+        def flux(E: Any, id: PDGID = pdgid) -> Any:
+            return model.flux(id, E, check_valid_pdgid=False)
 
         energy = df_event["total_energy"][df_event["particle_id"] == primary_pid]
         ext_pdf = energy.shape[0] * (energy**energy_slope) / N
 
         weights += [flux(energy) / ext_pdf]
 
-    df["weight"] = pd.concat(weights)
-    df_event["weight"] = pd.concat(weights)
+    return pd.concat(weights)
 
 
-def add_weight_prompt(df: pd.DataFrame, prompt_factor: float) -> None:
+def add_weight_prompt(
+    df: pd.DataFrame,
+    prompt_factor: float,
+    weight_col_name: str = "weight_prompt",
+    is_prompt_col_name: str = "is_prompt",
+) -> None:
     """
     Adds column "weight_prompt" to df, to set a weight for every prompt particle, non prompt particles get weight 1
     """
-    df["weight_prompt"] = 1.0
-    df.loc[df["is_prompt"] is True, "weight_prompt"] = prompt_factor
+    if not df.index.is_monotonic_increasing:
+        df.sort_index(inplace=True)
+
+    df[weight_col_name] = 1.0
+    df.loc[
+        df[is_prompt_col_name] == True, weight_col_name  # noqa: E712
+    ] = prompt_factor
 
 
-def add_weight_prompt_per_event(df: pd.DataFrame, prompt_factor: float) -> None:
+def add_weight_prompt_per_event(
+    df: pd.DataFrame,
+    prompt_factor: float,
+    weight_col_name: str = "weight_prompt_per_event",
+    is_prompt_col_name: str = "is_prompt",
+) -> None:
     """
     Adds column "weight_prompt_per_event" to df, which will be `prompt_factor` for every particle, which is inside
     a shower, which has at least one prompt muon. For every other particle, it will be 1.
     """
     # For some weird reason this makes a difference, as the last line of this function does not work otherwise
     if not df.index.is_monotonic_increasing:
         df.sort_index(inplace=True)
 
-    df["weight_prompt_per_event"] = 1.0
+    df[weight_col_name] = 1.0
 
-    indexes = df.query("is_prompt == True").index
+    indexes = df.query(f"{is_prompt_col_name} == True").index
     evt_idxs: dict[int, set[Any]] = {i[0]: set() for i in indexes}
     for i in indexes:
         evt_idxs[i[0]].add(i[1])
 
     for i in evt_idxs:
-        df.loc[i].loc[list(evt_idxs[i]), "weight_prompt_per_event"] = prompt_factor
+        df.loc[i].loc[list(evt_idxs[i]), weight_col_name] = prompt_factor
```

### Comparing `corsika_panama-0.4.0/pyproject.toml` & `corsika_panama-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 [tool.poetry]
 name = "corsika-panama"
-version = "0.4.0"
+version = "0.5.0"
 description = "PANdas And Multicore utils for corsikA7"
 authors = ["Ludwig Neste <ludwig.neste@tu-dortmund.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "panama" }]
 homepage = "https://github.com/The-Ludwig/PANAMA"
 repository = "https://github.com/The-Ludwig/PANAMA"
 documentation = "https://github.com/The-Ludwig/PANAMA#readme"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">= 3.8, < 3.12"
 corsikaio =  "^0.3"
 numpy = "^1.23.4"
-pandas = "^1.5.1"
+pandas = "^2.0.0"
 click = "^8.1.3"
 particle = "^0.21.0"
 tqdm = "^4.64.1"
-crflux = "^1.0.6"
 tables = "^3.8.0"
+scipy = "^1.10.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 pytest = "^7.2.0"
 coverage = "^7.1.0"
 pre-commit = "^3.0.4"
 sphinx = "^6.1.3"
 m2r2 = "<0.3.3"
 sphinx-rtd-theme = "^1.2.0"
 sphinx-click = "^4.4.0"
 ruff = "^0.0.252"
 mypy = "^1.0.1"
 types-tqdm = "^4.65.0.1"
 codespell = "^2.2.4"
+matplotlib = "^3.7.1"
 
 [tool.poetry.scripts]
 panama = 'panama.cli:cli'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
@@ -57,15 +58,15 @@
     "ignore::DeprecationWarning",
     "ignore::UserWarning",
 ]
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
-  "B", "B904",   # flake8-bugbear
+  "B",           # flake8-bugbear
   "I",           # isort
   "C4",          # flake8-comprehensions
   "ISC",         # flake8-implicit-str-concat
   "PGH",         # pygrep-hooks
   "PIE",         # flake8-pie
   "PL",          # pylint
   "PT",          # flake8-pytest-style
@@ -74,21 +75,22 @@
   "T20",         # flake8-print
   "UP",          # pyupgrade
   "YTT",         # flake8-2020
 ]
 extend-ignore = [
   "PLR",   # Design related pylint codes
   "E501",  # Line too long
+  "B905"       # strict= parameter of zip. (not in py3.8)
 ]
 target-version = "py311"
 src = ["panama"]
 
 [tool.mypy]
 files = [
-  "panama/*.py",
+  "panama/**",
 ]
 python_version = "3.11"
 strict = true
 warn_return_any = false
 warn_unreachable = true
 show_error_codes = true
 ignore_missing_imports = true
@@ -100,11 +102,7 @@
 ]
 exclude = ["tests/"]
 
 [[tool.mypy.overrides]]
 module = "tests"
 follow_imports = "skip"
 strict = false
-
-[[tool.mypy.overrides]]
-module = "panama.fluxes"
-follow_imports = "skip"
```

### Comparing `corsika_panama-0.4.0/setup.py` & `corsika_panama-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'corsikaio>=0.3,<0.4',
- 'crflux>=1.0.6,<2.0.0',
  'numpy>=1.23.4,<2.0.0',
- 'pandas>=1.5.1,<2.0.0',
+ 'pandas>=2.0.0,<3.0.0',
  'particle>=0.21.0,<0.22.0',
+ 'scipy>=1.10.1,<2.0.0',
  'tables>=3.8.0,<4.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['panama = panama.cli:cli']}
 
 setup_kwargs = {
     'name': 'corsika-panama',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'PANdas And Multicore utils for corsikA7',
     'long_description': '# PAN*das* A*nd* M*ulticore utils for corsik*A*7*\n\n[Documentation ![Read the Docs](https://img.shields.io/readthedocs/panama?style=for-the-badge)](https://panama.readthedocs.io/en/latest/)\n\n[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/The-Ludwig/PANAMA/ci.yml?style=for-the-badge)](https://github.com/The-Ludwig/PANAMA/actions/workflows/ci.yml)\n[![Codecov](https://img.shields.io/codecov/c/github/The-Ludwig/PANAMA?label=test%20coverage&style=for-the-badge)](https://app.codecov.io/gh/The-Ludwig/PANAMA)\n[![PyPI](https://img.shields.io/pypi/v/corsika-panama?style=for-the-badge)](https://pypi.org/project/corsika-panama/)\n\n[![GitHub issues](https://img.shields.io/github/issues-raw/The-Ludwig/PANAMA?style=for-the-badge)](https://github.com/The-Ludwig/PANAMA/issues)\n[![GitHub](https://img.shields.io/github/license/The-Ludwig/PANAMA?style=for-the-badge)](https://github.com/The-Ludwig/PANAMA/blob/main/LICENSE)\n[![Codestyle](https://img.shields.io/badge/codesyle-Black-black.svg?style=for-the-badge)](https://github.com/psf/black)\n\nThanks [@Jean1995](https://github.com/Jean1995) for the silly naming idea.\n\n## Installation\n\n```\npip install corsika-panama\n```\n\n## Features\n\n### Run CORSIKA7 on multiple cores\n\nYou need to have [`CORSIKA7`](https://www.iap.kit.edu/corsika/79.php) installed to run this.\n\nRunning 100 showers on 4 cores with primary being proton:\n\n```sh\n$ panama run --corsika path/to/corsika7/executable -j4 ./tests/files/example_corsika.template\n83%|████████████████████████████████████████████████████▋        | 83.0/100 [00:13<00:02, 6.36shower/s]\nJobs should be nearly finished, now we wait for them to exit\nAll jobs terminated, cleanup now\n```\n\nInjecting 5 different primaries (Proton, Helium-4, Carbon-12, Silicon-28, Iron-54 roughly aligning with grouping in H3a) with each primary shower taking 10 jobs:\n\n```sh\n$ panama run --corsika corsika-77420/run/corsika77420Linux_SIBYLL_urqmd --jobs 10 --primary ""{2212: 500, 1000020040: 250, 1000060120: 50, 1000140280: 50, 1000260540: 50}"" ./tests/files/example_corsika.template\n...\n```\n\n### Convert CORSIKA7 DAT files to hdf5 files\n\n```sh\n$ panama hdf5 path/to/corsika/dat/files/DAT* output.hdf5\n```\n\nThe data is available under the `run_header` `event_header` and `particles` key.\n\n### Read CORSIKA7 DAT files to pandas dataframes\n\nExample: Calculate mean energy in the corsika files created in the example above:\n\n```\nIn [1]: import panama as pn\n\nIn [2]: run_header, event_header, particles = pn.read_DAT(glob="corsika_output/DAT*")\n100%|████████████████████████████████████████████████████████████| 2000/2000.0 [00:00<00:00, 10127.45it/s]\nIn [3]: particles["energy"].mean()\nOut[3]: 26525.611020413744\n```\n\n`run_header`, `event_header` and `particles` are all [pandas.DataFrames](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) and can conveniently be used.\n\nIf `CORSIKA7` is compiled with the `EHIST` option, then the mother particles are automatically deleted, by default (this behaviour can be changed with`drop_mothers=False`).\nIf you want additional columns in the real particles storing the mother information use `mother_columns=True`.\n\n### Weighting to primary spectrum\n\nThis packages also provides facility to add a `weight` column to the dataframe, so you can look at corsika-output\nin physical flux in terms of $(\\mathrm{m^2} \\mathrm{s}\\ \\mathrm{sr}\\ \\mathrm{GeV})^{-1}$.\nUsing the example above, to get the whole physical flux in the complete simulated energy region:\n\n```\nIn [1]: import panama as pn\n\nIn [2]: run_header, event_header, particles = pn.read_DAT(glob="corsika_output/DAT*")\n100%|████████████████████████████████████████████████████████████| 2000/2000.0 [00:00<00:00, 10127.45it/s]\nIn [3]: pn.add_weight(run_header, event_header, particles)\n\nIn [4]: particles["weight"].sum()*(run_header["energy_max"]-run_header["energy_min"])\nOut[4]:\nrun_number\n1.0    1234.693481\n0.0    1234.693481\n3.0    1234.693481\n2.0    1234.693481\ndtype: float32\n\n```\n\nWhich is in units of $(\\mathrm{m^2}\\ \\mathrm{s}\\ \\mathrm{sr})^{-1}$. We get a result for each run, since\nin theory we could have different energy regions. Here, we do not, so the result is always equal.\n\nWeighting can be applied to different primaries, also, if they are known by the flux model.\n\n`add_weight` can also be applied to dataframes loaded in from hdf5 files produced with PANAMA.\n\nTODO: Better documentation of weighting (what is weighted, how, proton/neutrons, area...?)\n\n#### Notes:\n\nThis started a little while ago while I was looking into the `EHIST` option\nof corsika.\nI wanted a way of conveniently running CORSIKA7 on more than 1 core.\nI ended in the same place where most CORSIKA7 users end (see e.g. [fact-project/corsika_wrapper](https://github.com/fact-project/corsika_wrapper))\nand wrote a small wrapper.\n\nread_DAT made possible by [cta-observatory/pycorsikaio](https://github.com/cta-observatory/pycorsikaio).\n\n#### Pitfalls\n\n- The whole `run` folder of CORSIKA7 must be copied for each process, so very high parallel runs have high overhead\n- If you simulate to low energies, python can\'t seem to hold up with the corsika output to `stdin` and essentially slows down corsika this is still a bug in investigation #1\n\n## What this is not\n\nBug-free or stable\n',
     'author': 'Ludwig Neste',
     'author_email': 'ludwig.neste@tu-dortmund.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/The-Ludwig/PANAMA',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `corsika_panama-0.4.0/PKG-INFO` & `corsika_panama-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: corsika-panama
-Version: 0.4.0
+Version: 0.5.0
 Summary: PANdas And Multicore utils for corsikA7
 Home-page: https://github.com/The-Ludwig/PANAMA
 License: MIT
 Author: Ludwig Neste
 Author-email: ludwig.neste@tu-dortmund.de
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: corsikaio (>=0.3,<0.4)
-Requires-Dist: crflux (>=1.0.6,<2.0.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
-Requires-Dist: pandas (>=1.5.1,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: particle (>=0.21.0,<0.22.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tables (>=3.8.0,<4.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Documentation, https://github.com/The-Ludwig/PANAMA#readme
 Project-URL: Repository, https://github.com/The-Ludwig/PANAMA
 Description-Content-Type: text/markdown
 
 # PAN*das* A*nd* M*ulticore utils for corsik*A*7*
```

