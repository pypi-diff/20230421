# Comparing `tmp/space_rocks-1.7.5.tar.gz` & `tmp/space_rocks-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_rocks-1.7.5.tar", max compression
+gzip compressed data, was "space_rocks-1.7.6.tar", max compression
```

## Comparing `space_rocks-1.7.5.tar` & `space_rocks-1.7.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2023-02-19 15:02:51.509244 space_rocks-1.7.5/LICENSE
--rw-r--r--   0        0        0     1902 2023-02-19 15:02:41.635801 space_rocks-1.7.5/README.md
--rw-r--r--   0        0        0     1490 2023-03-09 14:01:05.445549 space_rocks-1.7.5/pyproject.toml
--rw-r--r--   0        0        0      450 2023-03-09 14:02:43.929550 space_rocks-1.7.5/rocks/__init__.py
--rw-r--r--   0        0        0     4726 2023-02-19 15:02:48.499210 space_rocks-1.7.5/rocks/cache.py
--rw-r--r--   0        0        0    11448 2023-02-21 10:52:31.613902 space_rocks-1.7.5/rocks/cli.py
--rw-r--r--   0        0        0     7078 2023-02-19 15:02:48.499210 space_rocks-1.7.5/rocks/config.py
--rw-r--r--   0        0        0    37532 2023-03-09 13:51:36.573544 space_rocks-1.7.5/rocks/core.py
--rw-r--r--   0        0        0    32924 2023-03-09 13:53:50.569545 space_rocks-1.7.5/rocks/datacloud.py
--rw-r--r--   0        0        0    12708 2023-03-03 09:25:33.816871 space_rocks-1.7.5/rocks/index.py
--rw-r--r--   0        0        0      982 2023-02-19 15:02:48.499210 space_rocks-1.7.5/rocks/logging.py
--rw-r--r--   0        0        0     3274 2023-02-19 15:02:48.455876 space_rocks-1.7.5/rocks/metadata.py
--rw-r--r--   0        0        0     6300 2023-02-19 15:02:48.465877 space_rocks-1.7.5/rocks/plots.py
--rw-r--r--   0        0        0    12680 2023-03-03 09:25:11.292871 space_rocks-1.7.5/rocks/resolve.py
--rw-r--r--   0        0        0    12017 2023-02-20 13:54:44.114559 space_rocks-1.7.5/rocks/ssodnet.py
--rw-r--r--   0        0        0     3334 1970-01-01 00:00:00.000000 space_rocks-1.7.5/setup.py
--rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 space_rocks-1.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 07:53:47.207007 space_rocks-1.7.6/LICENSE
+-rw-r--r--   0        0        0     1731 2023-04-21 07:53:47.207007 space_rocks-1.7.6/README.md
+-rw-r--r--   0        0        0     1552 2023-04-21 08:05:18.107013 space_rocks-1.7.6/pyproject.toml
+-rw-r--r--   0        0        0      450 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/__init__.py
+-rw-r--r--   0        0        0     4886 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/cache.py
+-rw-r--r--   0        0        0    11459 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/cli.py
+-rw-r--r--   0        0        0     7078 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/config.py
+-rw-r--r--   0        0        0    39456 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/core.py
+-rw-r--r--   0        0        0    32930 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/datacloud.py
+-rw-r--r--   0        0        0    13116 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/index.py
+-rw-r--r--   0        0        0      982 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/logging.py
+-rw-r--r--   0        0        0     3765 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/metadata.py
+-rw-r--r--   0        0        0     6300 2023-02-19 15:02:48.465877 space_rocks-1.7.6/rocks/plots.py
+-rw-r--r--   0        0        0    12653 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/resolve.py
+-rw-r--r--   0        0        0    12231 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/ssodnet.py
+-rw-r--r--   0        0        0     3161 1970-01-01 00:00:00.000000 space_rocks-1.7.6/setup.py
+-rw-r--r--   0        0        0     3304 1970-01-01 00:00:00.000000 space_rocks-1.7.6/PKG-INFO
```

### Comparing `space_rocks-1.7.5/LICENSE` & `space_rocks-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.5/README.md` & `space_rocks-1.7.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,14 @@
   <a href="https://arxiv.org/abs/2209.10697">
     <img src="https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg"/>
   </a>
 </div>
 
 <br>
 
-*Disclaimer: The SsODNet service and its database are in an alpha version and under constant revision. The provided values and access methods may change without notice.*
-
 ## Features
 
 Explore asteroid data on the command-line...
 
 ``` sh
 $ rocks id 221
 (221) Eos
```

#### html2text {}

```diff
@@ -2,19 +2,17 @@
                                 logo_rocks.svg]
                       Features - Install - Documentation
 
  [https://img.shields.io/pypi/pyversions/space-rocks] [https://img.shields.io/
       pypi/v/space-rocks] [https://readthedocs.org/projects/rocks/badge/
   ?version=latest] [https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg]
 
-*Disclaimer: The SsODNet service and its database are in an alpha version and
-under constant revision. The provided values and access methods may change
-without notice.* ## Features Explore asteroid data on the command-line... ```
-sh $ rocks id 221 (221) Eos $ rocks class Eos MB>Outer $ rocks albedo Eos 0.136
-+- 0.004 $ rocks taxonomy Eos K $ rocks density Eos 4.559e+03 +- 1.139e+03 kg/
-m$^3$ ``` ... and in a `python` script. ``` python >>> import rocks >>>
-rocks.identify("1902ug") ('Fortuna', 19) >>> ceres = rocks.Rock("ceres") >>>
-ceres.diameter.value 848.4 >>> ceres.diameter.unit 'km' >>> ceres.mass.value
-9.384e+20 >>> ceres.mass.error 6.711e+17 ``` ## Install Install from PyPi using
-`pip`: $ pip install space-rocks The minimum required `python` version is 3.7.
-## Documentation Check out the documentation at [rocks.readthedocs.io](https://
+## Features Explore asteroid data on the command-line... ``` sh $ rocks id 221
+(221) Eos $ rocks class Eos MB>Outer $ rocks albedo Eos 0.136 +- 0.004 $ rocks
+taxonomy Eos K $ rocks density Eos 4.559e+03 +- 1.139e+03 kg/m$^3$ ``` ... and
+in a `python` script. ``` python >>> import rocks >>> rocks.identify("1902ug")
+('Fortuna', 19) >>> ceres = rocks.Rock("ceres") >>> ceres.diameter.value 848.4
+>>> ceres.diameter.unit 'km' >>> ceres.mass.value 9.384e+20 >>>
+ceres.mass.error 6.711e+17 ``` ## Install Install from PyPi using `pip`: $ pip
+install space-rocks The minimum required `python` version is 3.7. ##
+Documentation Check out the documentation at [rocks.readthedocs.io](https://
 rocks.readthedocs.io/en/latest/) or run $ rocks docs
```

### Comparing `space_rocks-1.7.5/pyproject.toml` & `space_rocks-1.7.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "space-rocks"
-version = "1.7.5"
+version = "1.7.6"
 description = "Python client for SsODNet data access."
 authors = ["Max Mahlke <max.mahlke@oca.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rocks.readthedocs.io/en/latest/"
 documentation = "https://rocks.readthedocs.io/en/latest/"
 repository = "https://github.com/maxmahlke/rocks.git"
@@ -43,13 +43,16 @@
 [tool.poetry.dev-dependencies]
 sphinx-redactor-theme = {version = "^0.0.1", optional = true}
 sphinx-hoverxref = {version = "*", optional = true}
 jinja2 = {version = "<3.1", optional = true}
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
+[tool.poetry.group.dev.dependencies]
+pytest-sugar = "^0.9.6"
+
 [tool.pytest.ini_options]
 addopts = "-v --cov=rocks --cov-report html"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `space_rocks-1.7.5/rocks/cache.py` & `space_rocks-1.7.6/rocks/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     # Get all JSONs in cache
     cached_jsons = set(file_ for file_ in config.PATH_CACHE.glob("*.json"))
 
     cached_cards = []
     cached_catalogues = []
 
     for file_ in cached_jsons:
-
         # Is it metadata?
         if file_ in [config.PATH_MAPPINGS, config.PATH_AUTHORS]:
             continue
 
         # Datacloud catalogue or ssoCard?
         if any(cat["ssodnet_name"] in str(file_) for cat in config.DATACLOUD.values()):
             *ssodnet_id, catalogue = file_.stem.split("_")
@@ -109,49 +108,53 @@
     else:
         _, _, ids_new = zip(
             *resolve.identify(ids, return_id=True, local=False, progress=True)
         )
 
     # Did any ID change?
     for id_, id_new in zip(ids, ids_new):
-
         if id_ == id_new:
             continue
 
         # This is fun to know
         rich.print(f"{id_} is now known as {id_new}.")
 
         # Remove the outdated card
         (config.PATH_CACHE / f"{id_}.json").unlink()
 
     # Update all cards
     ssodnet.get_ssocard(ids, progress=True, local=False)
 
+    # Update metadata and authors
+    for which in ["authors", "mappings"]:
+        metadata.retrieve(which)
+
 
 def update_catalogues(cached_catalogues):
     """Update the cached datacloud catalogues.
 
     Parameters
     ----------
     cached_catalogues: list of tuple
         The SsODNet IDs and names of the cached datacloud catalogues.
     """
 
     # Update catalogues on a per-type basis
     for catalogue in set(catalogues[1] for catalogues in cached_catalogues):
-
         ids = [id_ for id_, cat in cached_catalogues if cat == catalogue]
         ssodnet.get_datacloud_catalogue(ids, catalogue, local=False, progress=True)
 
 
 def retrieve_all_ssocards():
     """Retrieves all ssoCards and stores them in the cache directory.
 
     Warning: This will slow down the '$ rocks status' command considerably.
     """
+    import shutil
+    from rich.progress import track
 
     # Retrieve archive of ssoCards
     PATH_ARCHIVE = "/tmp/ssoCard-latest.tar.gz"
 
     URL = "https://ssp.imcce.fr/webservices/ssodnet/api/ssocard/ssoCard-latest.tar.bz2"
 
     response = requests.get(URL, stream=True)
@@ -160,13 +163,12 @@
         shutil.copyfileobj(response.raw, fp)
 
     # Extract to the cache directory
     cards = tarfile.open(PATH_ARCHIVE, mode="r:bz2")
     members = cards.getmembers()
 
     for member in track(members, total=len(members), description="Unpacking ssoCards"):
-
         if not member.name.endswith(".json"):
             continue
 
         member.path = member.path.split("/")[-1]
         cards.extract(member, config.PATH_CACHE)
```

### Comparing `space_rocks-1.7.5/rocks/cli.py` & `space_rocks-1.7.6/rocks/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,16 @@
             choices=["0", "1"],
             show_choices=False,
             default="1",
         )
 
         if decision == "1":
             click.echo()
-            index._build_index()
+    if update:
+        index._build_index()
 
 
 @cli_rocks.command()
 @click.argument("id_", nargs=-1)
 def who(id_):
     """Get name citation of asteroid from MPC."""
     import textwrap
```

### Comparing `space_rocks-1.7.5/rocks/config.py` & `space_rocks-1.7.6/rocks/config.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.5/rocks/core.py` & `space_rocks-1.7.6/rocks/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 # ------
 # ssoCard as pydantic model
 def add_paths(cls, values, parent):
     values["path"] = parent
 
     for name, value in values.items():
         if isinstance(value, (Parameter, FloatValue, StringValue, IntegerValue)):
-
             if keyword.iskeyword(name.strip("_")):
                 name = name.strip("_")
 
             if any(
                 parameter in parent for parameter in ["color", "phase_function", "spin"]
             ):
                 value.path = f"{parent}.<id>.{name}"
@@ -42,15 +41,14 @@
 class Error(pydantic.BaseModel):
     min_: float = pydantic.Field(np.nan, alias="min")
     max_: float = pydantic.Field(np.nan, alias="max")
 
 
 # The second lowest level is the Parameter. Values inherit from Parameter.
 class Parameter(pydantic.BaseModel):
-
     _label: str = pydantic.Field("", exclude=True)
     _format: str = pydantic.Field("", exclude=True)
     _symbol: str = pydantic.Field("", exclude=True)
     _description: str = pydantic.Field("", exclude=True)
     path: str = pydantic.Field("", exclude=True)
 
     def __str__(self):
@@ -125,15 +123,14 @@
     def unit(self):
         if "unit" in metadata.load_mappings()[self.path]:
             return metadata.load_mappings()[self.path]["unit"]
         return ""
 
     @pydantic.root_validator(pre=True)
     def _compute_mean_error(cls, values):
-
         if "error" in values:
             if "min" in values["error"] and "max" in values["error"]:
                 values["error_"] = np.mean(
                     [np.abs(values["error"][which]) for which in ["min", "max"]]
                 )
 
         return values
@@ -181,14 +178,15 @@
 
 # Other common branches are bibref, links and method
 class Method(Parameter):
     doi: str = ""
     name: str = ""
     year: int = None
     title: str = ""
+    source: str = ""
     bibcode: str = ""
     shortbib: str = ""
 
 
 class Bibref(Parameter):
     doi: str = ""
     year: int = None
@@ -257,16 +255,18 @@
     mean_motion: FloatValue = FloatValue(**{})
     orbital_arc: IntegerValue = IntegerValue(**{})
     eccentricity: FloatValue = FloatValue(**{})
     mean_anomaly: FloatValue = FloatValue(**{})
     node_longitude: FloatValue = FloatValue(**{})
     orbital_period: FloatValue = FloatValue(**{})
     semi_major_axis: FloatValue = FloatValue(**{})
+    aphelion_distance: FloatValue = FloatValue(**{})
     number_observation: FloatValue = FloatValue(**{})
     perihelion_argument: FloatValue = FloatValue(**{})
+    perihelion_distance: FloatValue = FloatValue(**{})
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.dynamical.orbital_elements")
 
     _convert_list_to_parameterlist: classmethod = pydantic.validator(
         "bibref", allow_reuse=True, pre=True
@@ -287,14 +287,24 @@
     proper_frequency_perihelion_longitude: FloatValue = FloatValue(**{})
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.dynamical.proper_elements")
 
 
+class SourceRegions(Parameter):
+    hun: FloatValue = FloatValue(**{})
+    nu6: FloatValue = FloatValue(**{})
+    pho: FloatValue = FloatValue(**{})
+    mm31: FloatValue = FloatValue(**{})
+    mm21: FloatValue = FloatValue(**{})
+    method: List[Method] = [Method(**{})]
+    links: LinksParameter = LinksParameter(**{})
+
+
 class Family(Parameter):
     links: LinksParameter = LinksParameter(**{})
     bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     method: List[Method] = [Method(**{})]
     family_name: StringValue = StringValue(**{})
     family_number: IntegerValue = IntegerValue(**{})
     family_status: StringValue = StringValue(**{})
@@ -313,29 +323,49 @@
         return add_paths(cls, values, "parameters.dynamical.family")
 
     _convert_list_to_parameterlist: classmethod = pydantic.validator(
         "bibref", allow_reuse=True, pre=True
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
+class MOID(Parameter):
+    mercury: FloatValue = pydantic.Field(FloatValue(**{}), alias="Mercury")
+    venus: FloatValue = pydantic.Field(FloatValue(**{}), alias="Venus")
+    emb: FloatValue = pydantic.Field(FloatValue(**{}), alias="EMB")
+    mars: FloatValue = pydantic.Field(FloatValue(**{}), alias="Mars")
+    jupiter: FloatValue = pydantic.Field(FloatValue(**{}), alias="Jupiter")
+    saturn: FloatValue = pydantic.Field(FloatValue(**{}), alias="Saturn")
+    uranus: FloatValue = pydantic.Field(FloatValue(**{}), alias="Uranus")
+    neptune: FloatValue = pydantic.Field(FloatValue(**{}), alias="Neptune")
+    method: List[Method] = [Method(**{})]
+    links: LinksParameter = LinksParameter(**{})
+
+    @pydantic.root_validator()
+    def _add_paths(cls, values):
+        return add_paths(cls, values, "parameters.dynamical.MOID")
+
+
 class Pair(Parameter):
     age: FloatValue = FloatValue(**{})
     distance: FloatValue = FloatValue(**{})
     sibling_name: StringValue = StringValue(**{})
     sibling_number: IntegerValue = IntegerValue(**{})
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.dynamical.pair")
 
 
 class TisserandParameter(Parameter):
     jupiter: FloatValue = pydantic.Field(FloatValue(**{}), alias="Jupiter")
-    method: List[Method] = [Bibref(**{})]
-    bibref: ListWithAttributes = [Method(**{})]
+    saturn: FloatValue = pydantic.Field(FloatValue(**{}), alias="Saturn")
+    uranus: FloatValue = pydantic.Field(FloatValue(**{}), alias="Uranus")
+    neptune: FloatValue = pydantic.Field(FloatValue(**{}), alias="Neptune")
+    method: List[Method] = [Method(**{})]
+    bibref: ListWithAttributes = [Bibref(**{})]
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.dynamical.tisserand_parameter")
 
 
 class Yarkovsky(Parameter):
@@ -351,16 +381,18 @@
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.dynamical.yarkovsky")
 
 
 class DynamicalParameters(Parameter):
+    moid: MOID = MOID(**{})
     pair: Pair = pydantic.Field(Pair(**{}), alias="pairs")
     family: Family = Family(**{})
+    source_regions: SourceRegions = SourceRegions(**{})
     tisserand_parameter: TisserandParameter = TisserandParameter(**{})
     yarkovsky: Yarkovsky = Yarkovsky(**{})
     proper_elements: ProperElements = ProperElements(**{})
     orbital_elements: OrbitalElements = OrbitalElements(**{})
 
     def __str__(self):
         return self.json()
@@ -529,14 +561,15 @@
     G1: FloatValue = FloatValue(**{})
     G2: FloatValue = FloatValue(**{})
     rms: FloatValue = FloatValue(**{})
     phase: Error = Error(**{})
     links: LinksParameter = LinksParameter(**{})
     bibref: ListWithAttributes = [Bibref(**{})]
     facility: StringValue = StringValue(**{})
+    technique: StringValue = StringValue(**{})
     name_filter: StringValue = StringValue(**{})
 
     def __bool__(self):
         return bool(np.isfinite(self.H.value))
 
     def __str__(self):
         if not np.isnan(self.H.value):
@@ -547,14 +580,16 @@
         "bibref", allow_reuse=True, pre=True
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
 class PhaseFunction(Parameter):
     # Generic
     generic_johnson_V: Phase = pydantic.Field(Phase(**{}), alias="Generic/Johnson.V")
+    # Gaia
+    gaia_gaia3_g: Phase = pydantic.Field(Phase(**{}), alias="GAIA/GAIA3.G")
     # ATLAS
     misc_atlas_cyan: Phase = pydantic.Field(Phase(**{}), alias="Misc/Atlas.cyan")
     misc_atlas_orange: Phase = pydantic.Field(Phase(**{}), alias="Misc/Atlas.orange")
 
     def __getattr__(self, name):
         """Implement attribute shortcuts. Gets called if __getattribute__ fails."""
 
@@ -563,25 +598,31 @@
         raise AttributeError
 
     def __bool__(self):
         return any(
             [
                 np.isfinite(getattr(self, filter_).H.value)
                 for filter_ in [
+                    "gaia_gaia3_g",
                     "generic_johnson_V",
                     "misc_atlas_cyan",
                     "misc_atlas_orange",
                 ]
             ]
         )
 
     def __str__(self):
         observed = []
 
-        for filter_ in ["generic_johnson_V", "misc_atlas_cyan", "misc_atlas_orange"]:
+        for filter_ in [
+            "gaia_gaia3_g",
+            "generic_johnson_V",
+            "misc_atlas_cyan",
+            "misc_atlas_orange",
+        ]:
             entry = getattr(self, filter_)
             if not np.isnan(entry.H.value):
                 observed.append(
                     rf"H: {entry.H.value:.2f}  G1: {entry.G1.value:.2f}  G2: {entry.G2.value:.2f}  [{filter_}]"
                 )
         if observed:
             return "\n".join(observed)
@@ -597,19 +638,21 @@
     Wp: FloatValue = FloatValue(**{})
     id_: IntegerValue = IntegerValue(**{})
     lat: FloatValue = FloatValue(**{})
     RA0: FloatValue = FloatValue(**{})
     DEC0: FloatValue = FloatValue(**{})
     links: LinksParameter = LinksParameter(**{})
     long_: FloatValue = pydantic.Field(FloatValue(**{}), alias="long")
+    bibref: ListWithAttributes = [Bibref(**{})]
+    method: List[Method] = [Method(**{})]
     period: FloatValue = FloatValue(**{})
     obliquity: FloatValue = FloatValue(**{})
-    method: List[Method] = [Method(**{})]
-    bibref: ListWithAttributes = [Bibref(**{})]
     technique: StringValue = StringValue(**{})
+    technique: StringValue = StringValue(**{})
+    period_type: StringValue = StringValue(**{})
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.physical.spins")
 
     _convert_list_to_parameterlist: classmethod = pydantic.validator(
         "bibref", allow_reuse=True, pre=True
@@ -845,34 +888,31 @@
 
                 if on_404 == "warning":
                     logger.error(MESSAGE)
                 elif on_404 == "error":
                     raise ValueError(MESSAGE)
 
             else:
-
                 if datacloud is not None:
                     for catalogue in datacloud:
                         ssocard = self.__add_datacloud_catalogue(
                             id_, catalogue, ssocard
                         )
         else:
             # Something failed. Instantiate minimal ssoCard for meaningful error output.
             ssocard = {"name": id_provided}
 
         # Deserialize the asteroid data
         try:
             super().__init__(**ssocard)  # type: ignore
         except pydantic.ValidationError as message:
-
             self.__parse_error_message(message, id_, ssocard)
 
             # Set the offending properties to None to allow for instantiation anyway
             for error in message.errors():
-
                 # Dynamically remove offending parts of the ssoCard
                 offending_part = ssocard
 
                 location_list = error["loc"][:-1]
 
                 if any(
                     property_ in location_list for property_ in ["taxonomy", "spin"]
@@ -885,26 +925,24 @@
                             entry, idx_list = location_list[idx + 1 : idx + 3]
 
                             try:
                                 del ssocard["parameters"]["physical"][property_]
                             except KeyError:
                                 pass
                 else:
-
                     for location in error["loc"][:-1]:
                         offending_part = offending_part[location]
 
                     del offending_part[error["loc"][-1]]
 
             super().__init__(**ssocard)  # type: ignore
 
         # Convert the retrieve datacloud catalogues into DataCloudDataFrame objects
         if datacloud is not None:
             for catalogue in datacloud:
-
                 if catalogue in ["diameters", "albedos"]:
                     catalogue = "diamalbedo"
 
                 # Ensure that all catalogue entries have the right length
                 catalogue_dict = getattr(self, catalogue).dict()
 
                 REQUIRED_LENGTH = max(len(val) for val in catalogue_dict.values())
@@ -1066,21 +1104,19 @@
     else:
         _, _, ids = zip(*resolve.identify(ids, return_id=True, progress=progress))
 
     # Load ssoCards asynchronously
     ssodnet.get_ssocard([id_ for id_ in ids if not id_ is None], progress=progress)
 
     if datacloud is not None:
-
         if isinstance(datacloud, str):
             datacloud = [datacloud]
 
         # Load datacloud catalogues asynchronously
         for cat in datacloud:
-
             if cat not in config.DATACLOUD.keys():
                 raise ValueError(
                     f"Unknown datacloud catalogue name: '{cat}'"
                     f"\nChoose from {config.DATACLOUD.keys()}"
                 )
 
             ssodnet.get_datacloud_catalogue(
```

### Comparing `space_rocks-1.7.5/rocks/datacloud.py` & `space_rocks-1.7.6/rocks/datacloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 import re
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 import pydantic
 import rich
-from rich.table import Table
 
 from rocks import config
 from rocks import core
 from rocks.logging import logger
 
+
 # ------
 # Pretty-printing
 def pretty_print(rock, catalogue, parameter):
     """Print datacloud catalogue using a nice table format.
 
     Parameters
     ----------
     rock : rocks.Rock
         The Rock instance the catalogue is associated to.
     catalogue : pd.DataFrame
         The datacloud catalogue to print.
     parameter : str
         The name of the user-requested parameter to echo.
     """
+    from rich.table import Table
+
     if len(catalogue) == 1 and pd.isna(catalogue.number[0]):
         print(f"No {parameter} on record for ({rock.number}) {rock.name}.")
         return
 
     # Sort catalogue by year of reference
     if "year" in catalogue.columns:
         catalogue = catalogue.sort_values("year").reset_index()
@@ -73,15 +75,14 @@
     # Some catalogues do not have a "preferred" attribute
     # if not hasattr(catalogue, "preferred"):
     #     preferred = [False for _ in range(len(catalogue))]
     # else:
 
     # Add rows to table, styling by preferred-state of entry
     for i, pref in enumerate(preferred):
-
         if parameter in ["diamalbedos"]:
             if pref:
                 if (
                     catalogue.preferred_albedo[i]
                     and not catalogue.preferred_diameter[i]
                 ):
                     style = "bold yellow"
@@ -213,14 +214,15 @@
     return preferred
 
 
 # ------
 # SsODNet catalogues as pydantic model
 # https://ssp.imcce.fr/data/ssodnet_datacloud.sql
 
+
 # Metacatalogues
 class Collection(pydantic.BaseModel):
     """Table de definition des references des jeux de donnees de la base SsODNet.datacloud"""
 
     link: List[Optional[str]] = [""]
     title: List[Optional[str]] = [""]
     shortbib: List[Optional[str]] = [""]
```

### Comparing `space_rocks-1.7.5/rocks/index.py` & `space_rocks-1.7.6/rocks/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,30 @@
 
 
 # ------
 # Building the index
 def _build_index():
     """Build asteroid name-number index from SsODNet sso_index."""
 
+    config.PATH_INDEX.mkdir(exist_ok=True, parents=True)
+
     tasks_descs = [
         (_build_fuzzy_searchable_index, ":kiwi_fruit: Differentiating parent bodies"),
         (_build_number_index, ":ringed_planet: Cleaning out resonances"),
         (_build_name_index, ":waning_gibbous_moon: Gardening the regolith"),
         (_build_designation_index, ":five:  Assigning numbers"),
         (_build_palomar_transit_index, ":u6307: Composing name citations"),
         (_build_index_of_aliases, ":comet: Index updated"),
     ]
 
     with progress.Progress(
         "[progress.description]{task.description}",
         progress.BarColumn(),
         "[progress.percentage]{task.percentage:>3.0f}%",
     ) as pbar:
-
         # Initiate progress bar and retrieve index from SsODNet
         steps = pbar.add_task(
             ":telescope: Counting minor bodies", total=len(tasks_descs) + 1
         )
         index = _retrieve_index_from_ssodnet()
         pbar.update(steps, description=f":telescope: Found {len(index):,} ", advance=1)
 
@@ -80,15 +81,14 @@
     SIZE = 1e3  # Build chunks of 1k entries
 
     # Find next 10,000 to largest number
     numbered = index[~pd.isna(index.Number)]
     parts = np.arange(1, np.ceil(numbered.Number.max() / SIZE) * SIZE, SIZE, dtype=int)
 
     for part in parts:
-
         part_index = numbered.loc[
             (part <= numbered.Number) & (numbered.Number < part + SIZE)
         ]
 
         part_index = dict(
             zip(
                 part_index.Number,
@@ -114,15 +114,14 @@
 
     index = index[~pd.isna(index.Number)]
 
     names = set(red for red in index.Reduced if re.match(r"^[a-z\'-]*$", red))
     names.add(r"g!kun||'homdima")  # everyone's favourite shell injection
 
     for part in parts:
-
         names_subset = set(name for name in names if name.startswith(part))
 
         if part == "a":
             names_subset.add(
                 "'aylo'chaxnim"
             )  # another edge case for the daughter of venus
         part_index = index.loc[index.Reduced.isin(names_subset)]
@@ -160,15 +159,14 @@
     parts = [
         "18",
         "19",
         *[f"20{year:02}" for year in range(0, max_year + 1)],
     ]
 
     for part in parts:
-
         part_designations = set(desi for desi in designations if desi.startswith(part))
 
         # Asteroids in this chunk
         part_index = index.loc[index.Reduced.isin(part_designations)]
 
         no_number = pd.isna(part_index.Number)
         has_number = part_index[~no_number]
@@ -350,22 +348,27 @@
             index_number = index_range[index_range <= id_][-1]
         # The passed id_ is larger than 1e6
         except IndexError:
             index_number = 1
         which = f"{index_number}.pkl"
 
         if not (config.PATH_INDEX / which).exists():
-            logger.error(
-                f"The provided number '{id_}' is larger than the largest number of any asteroid."
-            )
+
+            if id_ > 1e6:
+                logger.error(
+                    f"The provided number {id_} is larger than the largest number of any asteroid."
+                )
+            else:
+                logger.error(
+                    f"Could not resolve asteroid number {id_}. The index may be broken, run \n'$ rocks status --update' to update it."
+                )
             sys.exit()
 
     # Is it a name?
     elif re.match(r"^[a-z\'-]*$", id_) or id_ == r"g!kun||'homdima":
-
         if id_[0] == "'":  # catch 'aylo'chaxnim
             which = f"{id_[0]}.pkl"
         else:
             which = config.PATH_INDEX / f"{id_[0]}.pkl"
 
     # Is it a designation?
     elif re.match(
@@ -396,15 +399,18 @@
 
     with open(config.PATH_INDEX / which, "rb") as file_:
         return pickle.load(file_)
 
 
 def get_modification_date():
     """Get modification date of index pickle files."""
-    date_index = (config.PATH_INDEX / "1.pkl").stat().st_mtime
+    check_file = config.PATH_INDEX / "1.pkl"
+    if not check_file.is_file():
+        return "[red][Index is broken, update it.][/red]"
+    date_index = check_file.stat().st_mtime
     return time.strftime("%d %b %Y", time.localtime(date_index))
 
 
 def find_candidates(id_):
     """Identify possible matches among all asteroid names based on Levenshtein distance.
 
     Parameters
```

### Comparing `space_rocks-1.7.5/rocks/logging.py` & `space_rocks-1.7.6/rocks/logging.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.5/rocks/metadata.py` & `space_rocks-1.7.6/rocks/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Functionality for SsODNet metadata interaction with rocks."""
 
 from functools import lru_cache
 import json
 import re
+import unicodedata
 
 import requests
 import rich
 
 from rocks import config
 from rocks.logging import logger
 from rocks import __version__
@@ -69,26 +70,47 @@
     with open(config.PATH_AUTHORS, "r") as file_:
         ssodnet_biblio = json.load(file_)
 
     author_found = False
 
     for category, datasets in ssodnet_biblio["ssodnet_biblio"]["datasets"].items():
         for dataset in datasets:
-            if author.capitalize() in dataset["shortbib"]:
+            if author.capitalize() in remove_diacritics(dataset["shortbib"]):
                 rich.print(
                     f" [magenta]{dataset['bibcode']}[/magenta]  {dataset['shortbib']:<20} [{category}]"
                 )
                 author_found = True
 
     if not author_found:
         logger.info(
             f"Could not find articles by '{author.capitalize()}' in SsODNet. You can email 'benoit.carry (at) oca.eu' if you are missing data."
         )
 
 
+def remove_diacritics(text):
+    """Remove accents from characters for a wider search.
+
+    Parameters
+    ----------
+    text : str
+        The text to strip the accents from.
+
+    Returns
+    -------
+    str
+        The accent-free string.
+
+    Notes
+    -----
+    Merci to https://stackoverflow.com/a/35783136
+    """
+    normalized = unicodedata.normalize("NFKD", text)
+    return "".join(c for c in normalized if unicodedata.category(c) != "Mn")
+
+
 def rocks_is_outdated():
     """Compare the local rocks __version__ to the one on the GitHub repository.
 
     Returns
     -------
     bool, str
         True if the local version is below the one on GitHub, else
```

### Comparing `space_rocks-1.7.5/rocks/plots.py` & `space_rocks-1.7.6/rocks/plots.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.5/rocks/resolve.py` & `space_rocks-1.7.6/rocks/resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         id_ = id_.tolist()
     elif isinstance(id_, (set, range)):
         id_ = list(id_)
     elif id_ is None:
         logger.warning(f"Received id_ of type {type(id_)}.")
         return (None, np.nan) if not return_id else (None, np.nan, None)  # type: ignore
     elif not isinstance(id_, (list, np.ndarray)):
-
         try:
             id_ = id_.to_list()  # pandas Series
         except AttributeError:
             raise TypeError(
                 f"Received id_ of type {type(id_)}, expected one of: "
                 "str, int, float, list, set, range, np.ndarray"
             )
@@ -94,27 +93,25 @@
     if not id_:
         logger.warning("Received empty list of identifiers.")
         return (None, np.nan) if not return_id else (None, np.nan, None)  # type: ignore
 
     # ------
     # For a single name, try local lookup right away, async process has overhead
     if len(id_) == 1 and local:
-
         success, (name, number, ssodnet_id) = _local_lookup(id_[0])
 
         if success:
             if not return_id:
                 return (name, number)
             else:
                 return (name, number, ssodnet_id)
 
     # ------
     # Run asynchronous event loop for name resolution
     with Progress(disable=not progress) as progress_bar:
-
         task = progress_bar.add_task("Identifying rocks", total=len(id_))  # type: ignore
         loop = get_or_create_eventloop()
         results = loop.run_until_complete(_identify(id_, local, progress_bar, task))
 
         # ------
         # Check if any failed due to 502 and rerun them
         idx_failed = [
@@ -139,15 +136,14 @@
     return results  # type: ignore
 
 
 async def _identify(id_, local, progress_bar, task):
     """Establish the asynchronous HTTP session and launch the name resolution."""
 
     async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout()) as session:
-
         tasks = [
             asyncio.ensure_future(_resolve(i, session, local, progress_bar, task))
             for i in id_
         ]
 
         results = await asyncio.gather(*tasks)
 
@@ -280,29 +276,27 @@
 
         # Asteroid designation
         elif re.match(
             r"(^([1A][8-9][0-9]{2}[ _]?[A-Za-z]{2}[0-9]{0,3}$)|"
             r"(^20[0-9]{2}[_ ]?[A-Za-z]{2}[0-9]{0,3}$))",
             id_,
         ):
-
             # Ensure whitespace between year and id_
             id_ = re.sub(r"[\W_]+", "", id_)
             ind = re.search(r"[A18920]{1,2}[0-9]{2}", id_).end()  # type: ignore
             id_ = f"{id_[:ind]} {id_[ind:]}"
 
             # Replace A by 1
             id_ = re.sub(r"^A", "1", id_)
 
             # Ensure uppercase
             id_ = id_.upper()
 
         # Palomar-Leiden / Transit
         elif re.match(r"^[1-9][0-9]{3}[ _]?(P-L|T-[1-3])$", id_):
-
             # Ensure whitespace
             id_ = re.sub(r"[ _]+", "", id_)
             id_ = f"{id_[:4]} {id_[4:]}"
 
         # Comet
         elif re.match(r"(^[PDCXAI]/[- 0-9A-Za-z]*)", id_):
             pass
@@ -348,19 +342,19 @@
 
     try:
         response = await response.json(content_type=None)
     except aiohttp.ContentTypeError:
         return None
 
     if "data" not in response.keys():  # no match found
-        logger.error(f"Could not find match for id {id_}.")
+        logger.error(f"Could not identify '{id_}'.")
         return False
 
     elif not response["data"]:  # empty response
-        logger.error(f"Could not find match for id {id_}.")
+        logger.error(f"Could not identify '{id_}'.")
         return False
 
     return response
 
 
 def _parse_quaero_response(data, id_):
     """Parse JSON response from Quaero.
@@ -387,15 +381,15 @@
             break
         elif match["id"].lower() == id_:
             break
         elif any(alias.lower() == id_ for alias in match["aliases"]):
             break
     else:
         # Unclear which match is correct.
-        logger.warning(f"Could not find match for id {id_}.")
+        logger.warning(f"Could not identify '{id_}'.")
         return (None, np.nan, None)
 
     # Found match
     numeric = [int(alias) for alias in match["aliases"] if alias.isnumeric()]
     number = min(numeric) if numeric else np.nan
     return (match["name"], number, match["id"])
```

### Comparing `space_rocks-1.7.5/rocks/ssodnet.py` & `space_rocks-1.7.6/rocks/ssodnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 
     return cards
 
 
 async def _get_ssocard(id_ssodnet, progress_bar, progress, local):
     """Get ssoCard asynchronously. First attempt local lookup, then query SsODNet."""
     async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout()) as session:
-
         tasks = [
             asyncio.ensure_future(
                 _local_or_remote(i, session, progress_bar, progress, local)
             )
             for i in id_ssodnet
         ]
 
@@ -95,15 +94,14 @@
 
 async def _local_or_remote(id_ssodnet, session, progress_bar, progress, local):
     """Check for presence of ssoCard in cache directory. Else, query from SsODNet."""
 
     PATH_CARD = config.PATH_CACHE / f"{id_ssodnet}.json"
 
     if PATH_CARD.is_file() and local:
-
         _update_progress(progress_bar, progress)
 
         with open(PATH_CARD, "r") as file_card:
             return json.load(file_card)
 
     # Local retrieval failed, do remote query
     card = await _query_ssodnet(id_ssodnet, session)
@@ -187,15 +185,14 @@
     if "spins" not in card["parameters"]["physical"]:
         card["parameters"]["physical"]["spins"] = {}
 
     spins = card["parameters"]["physical"]["spins"]
     spin_solutions = []
 
     for key, spin in spins.items():
-
         # spin entries have integer ids
         if not key.isnumeric():
             continue
 
         # convert the spin key to an entry in the solution dict
         spin["id_"] = {
             "value": key,
@@ -266,15 +263,14 @@
         loop = get_or_create_eventloop()
         catalogues = loop.run_until_complete(
             _get_datacloud_catalogue(id_catalogue, None, None, local)
         )[0]
 
     else:
         with Progress(disable=not progress) as progress_bar:
-
             progress = progress_bar.add_task(
                 "Getting catalogues" if len(catalogue) > 1 else catalogue[0],
                 total=len(id_catalogue),
             )
 
             # Run async loop to get ssoCard
             loop = get_or_create_eventloop()
@@ -301,15 +297,14 @@
     -------
     list of dict
         list containing len(id_) list with dictionaries corresponding to the
     catalogues of the passed identifiers. If the catalogue is not available, the dict
     is empty.
     """
     async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout()) as session:
-
         tasks = [
             asyncio.ensure_future(
                 _local_or_remote_catalogue(
                     i[0], i[1], session, progress_bar, progress, local
                 )
             )
             for i in id_catalogue
@@ -339,15 +334,21 @@
 
     # Local retrieval failed, do remote query
     cat = await _query_datacloud(id_ssodnet, catalogue, session)
     cat = cat["data"]
 
     # Always save the result, even if catalogue is empty
     if cat is not None:
-        cat = cat[0]["datacloud"]
+        try:
+            cat = cat[0]["datacloud"]
+        except (IndexError, KeyError):
+            logger.error(
+                f"Catalogue '{catalogue}' for '{id_ssodnet}' got an invalid response from datacloud."
+            )
+            cat = {}
         if catalogue in cat:
             cat = cat[catalogue]
         else:
             cat = {}
     else:
         cat = {}
```

### Comparing `space_rocks-1.7.5/setup.py` & `space_rocks-1.7.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 {'docs': ['sphinx>=5,<6', 'sphinx-hoverxref']}
 
 entry_points = \
 {'console_scripts': ['rocks = rocks.cli:cli_rocks']}
 
 setup_kwargs = {
     'name': 'space-rocks',
-    'version': '1.7.5',
+    'version': '1.7.6',
     'description': 'Python client for SsODNet data access.',
-    'long_description': '<p align="center">\n  <img width="260" src="https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/logo_rocks.svg">\n</p>\n\n<p align="center">\n  <a href="https://github.com/maxmahlke/rocks#features"> Features </a> - <a href="https://github.com/maxmahlke/rocks#install"> Install </a> - <a href="https://github.com/maxmahlke/rocks#documentation"> Documentation </a>\n</p>\n\n<br>\n\n<div align="center">\n  <a href="https://img.shields.io/pypi/pyversions/space-rocks">\n    <img src="https://img.shields.io/pypi/pyversions/space-rocks"/>\n  </a>\n  <a href="https://img.shields.io/pypi/v/space-rocks">\n    <img src="https://img.shields.io/pypi/v/space-rocks"/>\n  </a>\n  <a href="https://readthedocs.org/projects/rocks/badge/?version=latest">\n    <img src="https://readthedocs.org/projects/rocks/badge/?version=latest"/>\n  </a>\n  <a href="https://arxiv.org/abs/2209.10697">\n    <img src="https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg"/>\n  </a>\n</div>\n\n<br>\n\n*Disclaimer: The SsODNet service and its database are in an alpha version and under constant revision. The provided values and access methods may change without notice.*\n\n## Features\n\nExplore asteroid data on the command-line...\n\n``` sh\n$ rocks id 221\n(221) Eos\n\n$ rocks class Eos\nMB>Outer\n\n$ rocks albedo Eos\n0.136 +- 0.004\n\n$ rocks taxonomy Eos\nK\n\n$ rocks density Eos\n4.559e+03 +- 1.139e+03 kg/m$^3$\n```\n\n... and in a `python` script.\n\n``` python\n>>> import rocks\n>>> rocks.identify("1902ug")\n(\'Fortuna\', 19)\n>>> ceres = rocks.Rock("ceres")\n>>> ceres.diameter.value\n848.4\n>>> ceres.diameter.unit\n\'km\'\n>>> ceres.mass.value\n9.384e+20\n>>> ceres.mass.error\n6.711e+17\n```\n\n## Install\n\nInstall from PyPi using `pip`:\n\n     $ pip install space-rocks\n\nThe minimum required `python` version is 3.7.\n\n\n## Documentation\n\nCheck out the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/latest/) or run\n\n     $ rocks docs\n',
+    'long_description': '<p align="center">\n  <img width="260" src="https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/logo_rocks.svg">\n</p>\n\n<p align="center">\n  <a href="https://github.com/maxmahlke/rocks#features"> Features </a> - <a href="https://github.com/maxmahlke/rocks#install"> Install </a> - <a href="https://github.com/maxmahlke/rocks#documentation"> Documentation </a>\n</p>\n\n<br>\n\n<div align="center">\n  <a href="https://img.shields.io/pypi/pyversions/space-rocks">\n    <img src="https://img.shields.io/pypi/pyversions/space-rocks"/>\n  </a>\n  <a href="https://img.shields.io/pypi/v/space-rocks">\n    <img src="https://img.shields.io/pypi/v/space-rocks"/>\n  </a>\n  <a href="https://readthedocs.org/projects/rocks/badge/?version=latest">\n    <img src="https://readthedocs.org/projects/rocks/badge/?version=latest"/>\n  </a>\n  <a href="https://arxiv.org/abs/2209.10697">\n    <img src="https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg"/>\n  </a>\n</div>\n\n<br>\n\n## Features\n\nExplore asteroid data on the command-line...\n\n``` sh\n$ rocks id 221\n(221) Eos\n\n$ rocks class Eos\nMB>Outer\n\n$ rocks albedo Eos\n0.136 +- 0.004\n\n$ rocks taxonomy Eos\nK\n\n$ rocks density Eos\n4.559e+03 +- 1.139e+03 kg/m$^3$\n```\n\n... and in a `python` script.\n\n``` python\n>>> import rocks\n>>> rocks.identify("1902ug")\n(\'Fortuna\', 19)\n>>> ceres = rocks.Rock("ceres")\n>>> ceres.diameter.value\n848.4\n>>> ceres.diameter.unit\n\'km\'\n>>> ceres.mass.value\n9.384e+20\n>>> ceres.mass.error\n6.711e+17\n```\n\n## Install\n\nInstall from PyPi using `pip`:\n\n     $ pip install space-rocks\n\nThe minimum required `python` version is 3.7.\n\n\n## Documentation\n\nCheck out the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/latest/) or run\n\n     $ rocks docs\n',
     'author': 'Max Mahlke',
     'author_email': 'max.mahlke@oca.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://rocks.readthedocs.io/en/latest/',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -5,35 +5,33 @@
 'cchardet>=2.1.7,<3.0.0', 'click>=8.0.1,<9.0.0', 'furo>=2022.9.15,<2023.0.0',
 'matplotlib>=3.4.3,<4.0.0', 'nest-asyncio>=1.5.1,<2.0.0',
 'numpy>=1.21.2,<2.0.0', 'pandas>=1.3.2,<2.0.0', 'platformdirs>=2.6.2,<3.0.0',
 'pydantic>=1.8.2,<2.0.0', 'requests>=2.26.0,<3.0.0', 'rich>=12,<13', 'sphinx-
 copybutton>=0.5.0,<0.6.0', 'sphinx_design>=0.3.0,<0.4.0'] extras_require = \
 {'docs': ['sphinx>=5,<6', 'sphinx-hoverxref']} entry_points = \
 {'console_scripts': ['rocks = rocks.cli:cli_rocks']} setup_kwargs = { 'name':
-'space-rocks', 'version': '1.7.5', 'description': 'Python client for SsODNet
+'space-rocks', 'version': '1.7.6', 'description': 'Python client for SsODNet
 data access.', 'long_description': '
   \n [https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/
                                logo_rocks.svg]\n
 \n\n
                     \n Features - Install - Documentation\n
 \n\n
 \n\n
   \n \n_[https://img.shields.io/pypi/pyversions/space-rocks]\n\n \n_[https://
  img.shields.io/pypi/v/space-rocks]\n\n \n_[https://readthedocs.org/projects/
    rocks/badge/?version=latest]\n\n \n_[https://img.shields.io/badge/arXiv-
                           2209.10697-f9f107.svg]\n\n
 \n\n
-\n\n*Disclaimer: The SsODNet service and its database are in an alpha version
-and under constant revision. The provided values and access methods may change
-without notice.*\n\n## Features\n\nExplore asteroid data on the command-
-line...\n\n``` sh\n$ rocks id 221\n(221) Eos\n\n$ rocks class
-Eos\nMB>Outer\n\n$ rocks albedo Eos\n0.136 +- 0.004\n\n$ rocks taxonomy
-Eos\nK\n\n$ rocks density Eos\n4.559e+03 +- 1.139e+03 kg/m$^3$\n```\n\n... and
-in a `python` script.\n\n``` python\n>>> import rocks\n>>> rocks.identify
-("1902ug")\n(\'Fortuna\', 19)\n>>> ceres = rocks.Rock("ceres")\n>>>
+\n\n## Features\n\nExplore asteroid data on the command-line...\n\n``` sh\n$
+rocks id 221\n(221) Eos\n\n$ rocks class Eos\nMB>Outer\n\n$ rocks albedo
+Eos\n0.136 +- 0.004\n\n$ rocks taxonomy Eos\nK\n\n$ rocks density
+Eos\n4.559e+03 +- 1.139e+03 kg/m$^3$\n```\n\n... and in a `python`
+script.\n\n``` python\n>>> import rocks\n>>> rocks.identify("1902ug")\n
+(\'Fortuna\', 19)\n>>> ceres = rocks.Rock("ceres")\n>>>
 ceres.diameter.value\n848.4\n>>> ceres.diameter.unit\n\'km\'\n>>>
 ceres.mass.value\n9.384e+20\n>>> ceres.mass.error\n6.711e+17\n```\n\n##
 Install\n\nInstall from PyPi using `pip`:\n\n $ pip install space-rocks\n\nThe
 minimum required `python` version is 3.7.\n\n\n## Documentation\n\nCheck out
 the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/
 latest/) or run\n\n $ rocks docs\n', 'author': 'Max Mahlke', 'author_email':
 'max.mahlke@oca.eu', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
```

### Comparing `space_rocks-1.7.5/PKG-INFO` & `space_rocks-1.7.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-rocks
-Version: 1.7.5
+Version: 1.7.6
 Summary: Python client for SsODNet data access.
 Home-page: https://rocks.readthedocs.io/en/latest/
 License: MIT
 Author: Max Mahlke
 Author-email: max.mahlke@oca.eu
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -61,16 +61,14 @@
   <a href="https://arxiv.org/abs/2209.10697">
     <img src="https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg"/>
   </a>
 </div>
 
 <br>
 
-*Disclaimer: The SsODNet service and its database are in an alpha version and under constant revision. The provided values and access methods may change without notice.*
-
 ## Features
 
 Explore asteroid data on the command-line...
 
 ``` sh
 $ rocks id 221
 (221) Eos
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: space-rocks Version: 1.7.5 Summary: Python client
+Metadata-Version: 2.1 Name: space-rocks Version: 1.7.6 Summary: Python client
 for SsODNet data access. Home-page: https://rocks.readthedocs.io/en/latest/
 License: MIT Author: Max Mahlke Author-email: max.mahlke@oca.eu Requires-
 Python: >=3.7.1,<3.11 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Provides-Extra: docs
 Requires-Dist: Levenshtein (>=0.16.0,<0.17.0) Requires-Dist: aiodns
@@ -23,19 +23,17 @@
                                 logo_rocks.svg]
                       Features - Install - Documentation
 
  [https://img.shields.io/pypi/pyversions/space-rocks] [https://img.shields.io/
       pypi/v/space-rocks] [https://readthedocs.org/projects/rocks/badge/
   ?version=latest] [https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg]
 
-*Disclaimer: The SsODNet service and its database are in an alpha version and
-under constant revision. The provided values and access methods may change
-without notice.* ## Features Explore asteroid data on the command-line... ```
-sh $ rocks id 221 (221) Eos $ rocks class Eos MB>Outer $ rocks albedo Eos 0.136
-+- 0.004 $ rocks taxonomy Eos K $ rocks density Eos 4.559e+03 +- 1.139e+03 kg/
-m$^3$ ``` ... and in a `python` script. ``` python >>> import rocks >>>
-rocks.identify("1902ug") ('Fortuna', 19) >>> ceres = rocks.Rock("ceres") >>>
-ceres.diameter.value 848.4 >>> ceres.diameter.unit 'km' >>> ceres.mass.value
-9.384e+20 >>> ceres.mass.error 6.711e+17 ``` ## Install Install from PyPi using
-`pip`: $ pip install space-rocks The minimum required `python` version is 3.7.
-## Documentation Check out the documentation at [rocks.readthedocs.io](https://
+## Features Explore asteroid data on the command-line... ``` sh $ rocks id 221
+(221) Eos $ rocks class Eos MB>Outer $ rocks albedo Eos 0.136 +- 0.004 $ rocks
+taxonomy Eos K $ rocks density Eos 4.559e+03 +- 1.139e+03 kg/m$^3$ ``` ... and
+in a `python` script. ``` python >>> import rocks >>> rocks.identify("1902ug")
+('Fortuna', 19) >>> ceres = rocks.Rock("ceres") >>> ceres.diameter.value 848.4
+>>> ceres.diameter.unit 'km' >>> ceres.mass.value 9.384e+20 >>>
+ceres.mass.error 6.711e+17 ``` ## Install Install from PyPi using `pip`: $ pip
+install space-rocks The minimum required `python` version is 3.7. ##
+Documentation Check out the documentation at [rocks.readthedocs.io](https://
 rocks.readthedocs.io/en/latest/) or run $ rocks docs
```

