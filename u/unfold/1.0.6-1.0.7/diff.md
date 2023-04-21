# Comparing `tmp/unfold-1.0.6.tar.gz` & `tmp/unfold-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfold-1.0.6.tar", last modified: Fri Mar 31 19:11:46 2023, max compression
+gzip compressed data, was "unfold-1.0.7.tar", last modified: Fri Apr 21 12:39:45 2023, max compression
```

## Comparing `unfold-1.0.6.tar` & `unfold-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:11:46.256283 unfold-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-31 19:11:36.000000 unfold-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-31 19:11:36.000000 unfold-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-03-31 19:11:46.256283 unfold-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-03-31 19:11:36.000000 unfold-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 19:11:46.256283 unfold-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-31 19:11:36.000000 unfold-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:11:46.256283 unfold-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-31 19:11:36.000000 unfold-1.0.6/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-31 19:11:36.000000 unfold-1.0.6/tests/test_reproducing_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:11:46.256283 unfold-1.0.6/unfold/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 19:11:36.000000 unfold-1.0.6/unfold/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:11:46.256283 unfold-1.0.6/unfold/data/
--rw-r--r--   0 runner    (1001) docker     (123)   395147 2023-03-31 19:11:36.000000 unfold-1.0.6/unfold/data/flows_biosphere_38.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-31 19:11:36.000000 unfold-1.0.6/unfold/data/outdated_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-03-31 19:11:36.000000 unfold-1.0.6/unfold/data_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-31 19:11:36.000000 unfold-1.0.6/unfold/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-03-31 19:11:36.000000 unfold-1.0.6/unfold/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)    42501 2023-03-31 19:11:36.000000 unfold-1.0.6/unfold/unfold.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-31 19:11:36.000000 unfold-1.0.6/unfold/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:11:46.256283 unfold-1.0.6/unfold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-03-31 19:11:46.000000 unfold-1.0.6/unfold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-31 19:11:46.000000 unfold-1.0.6/unfold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:11:46.000000 unfold-1.0.6/unfold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 19:11:46.000000 unfold-1.0.6/unfold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 19:11:46.000000 unfold-1.0.6/unfold.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:39:45.065472 unfold-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-21 12:39:34.000000 unfold-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-21 12:39:34.000000 unfold-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-04-21 12:39:45.065472 unfold-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-21 12:39:34.000000 unfold-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:39:45.065472 unfold-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-21 12:39:34.000000 unfold-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:39:45.061472 unfold-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-21 12:39:34.000000 unfold-1.0.7/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-21 12:39:34.000000 unfold-1.0.7/tests/test_reproducing_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:39:45.061472 unfold-1.0.7/unfold/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:39:45.061472 unfold-1.0.7/unfold/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   395147 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/data/flows_biosphere_38.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/data/outdated_flows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/data_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45022 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/unfold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:39:45.061472 unfold-1.0.7/unfold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-04-21 12:39:45.000000 unfold-1.0.7/unfold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-21 12:39:45.000000 unfold-1.0.7/unfold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:39:45.000000 unfold-1.0.7/unfold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-21 12:39:45.000000 unfold-1.0.7/unfold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 12:39:45.000000 unfold-1.0.7/unfold.egg-info/top_level.txt
```

### Comparing `unfold-1.0.6/LICENSE` & `unfold-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unfold-1.0.6/PKG-INFO` & `unfold-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfold
-Version: 1.0.6
+Version: 1.0.7
 Summary: Unpacks LCA scenario databases.
 Home-page: https://github.com/polca/premise
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `unfold-1.0.6/README.md` & `unfold-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `unfold-1.0.6/setup.py` & `unfold-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         for filename in filenames:
             paths.append(os.path.join("..", path, filename))
     return paths
 
 
 setup(
     name="unfold",
-    version="1.0.6",
+    version="1.0.7",
     python_requires=">=3.9",
     packages=packages,
     author="Romain Sacchi <romain.sacchi@psi.ch>",
     license=open("LICENSE").read(),
     # Only if you have non-python data (CSV, etc.). Might need to change the directory name as well.
     include_package_data=True,
     install_requires=[
```

### Comparing `unfold-1.0.6/tests/test_reproducing_db.py` & `unfold-1.0.7/tests/test_reproducing_db.py`

 * *Files identical despite different names*

### Comparing `unfold-1.0.6/unfold/data/flows_biosphere_38.csv` & `unfold-1.0.7/unfold/data/flows_biosphere_38.csv`

 * *Files identical despite different names*

### Comparing `unfold-1.0.6/unfold/data/outdated_flows.yaml` & `unfold-1.0.7/unfold/data/outdated_flows.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -61,8 +61,65 @@
 "[Deleted]Carfentrazone ethyl ester": Carfentrazone-ethyl
 Cesium-137: Caesium-137
 Cesium-134: Caesium-134
 Cesium-136: Caesium-136
 Silver, ion: Silver I
 VOC, volatile organic compounds, unspecified origin: VOC, volatile organic compounds
 Carfentrazone ethyl ester: Carfentrazone-ethyl
-Iprodion: Iprodione
+Iprodion: Iprodione
+Beta-cyfluthrin: Cyfluthrin
+Chloride: Chloride, ion
+Dimethyldichlorosilane: Dichlorodimethylsilane
+Ethylene: Ethene
+Trichloroethylene: Ethene, trichloro-
+Gangue: Gangue, bauxite, in ground
+Haloxyfop-P-methyl: Haloxyfop- (R) Methylester
+Hydrochloric acid: Hydrogen chloride
+Lithium I: Lithium, ion
+Methane, fossil: Methane
+Methylamine: Methyl amine
+Zineb: Metiram
+Naphthalene: Naphtalene
+Nickel II: Nickel
+Potassium I: Potassium, ion
+Quizalofop-ethyl: Quizalofop ethyl ester
+Sulfate: Sulfate, ion
+Antimony ion: Antimony
+Arsenic ion: Arsenic
+Barium II: Barium
+Cadmium II: Cadmium, ion
+Chromium III: Chromium
+Cobalt II: Cobalt
+Copper ion: Copper
+Lead II: Lead
+Manganese II: Manganese
+Mercury II: Mercury
+Molybdenum VI: Molybdenum
+NMVOC, non-methane volatile organic compounds: NMVOC, non-methane volatile organic compounds, unspecified origin
+Selenium IV: Selenium
+Vanadium V: Vanadium
+Zinc II: Zinc
+Particulate Matter, < 2.5 um: Particulates, < 2.5 um
+Particulate Matter, > 2.5 um and < 10um: Particulates, > 2.5 um, and < 10um
+Particulate Matter, > 10 um: Particulates, > 10 um
+AOX, Adsorbable Organic Halogen: AOX, Adsorbable Organic Halogen as Cl
+Aluminium III: Aluminium
+Calcium II: Calcium, ion
+Iron ion: Iron, ion
+Sodium I: Sodium, ion
+Lithium: Lithium, in ground
+Oil, crude: Oil, crude, in ground
+Bromine: Bromine, in water
+Fluorspar: Fluorspar, in ground
+Iodine: Iodine, in water
+Silver I: Silver, ion
+Tin ion: Tin
+Ammonium: Ammonium, ion
+Iridium: Iridium, in ground
+Tebupirimfos: Tebupirimphos
+Pyraclostrobin: Pyraclostrobin (prop)
+Caesium-137: Cesium-137
+Caesium-134: Cesium-134
+Caesium-136: Cesium-136
+VOC, volatile organic compounds: VOC, volatile organic compounds, unspecified origin
+Carfentrazone-ethyl: Carfentrazone ethyl ester
+Iprodione: Iprodion
```

### Comparing `unfold-1.0.6/unfold/data_cleaning.py` & `unfold-1.0.7/unfold/data_cleaning.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,22 @@
     ]
 
     def clean_up(exc: dict) -> dict:
         """Cleans up an exchange"""
 
         for field in list(exc.keys()):
             if exc[field] is None or exc[field] == "None":
-                del exc[field]
+                if field in exc:
+                    del exc[field]
             if exc["type"] == "biosphere" and field in FORBIDDEN_FIELDS_BIO:
-                del exc[field]
+                if field in exc:
+                    del exc[field]
             if exc["type"] == "technosphere" and field in FORBIDDEN_FIELDS_TECH:
-                del exc[field]
+                if field in exc:
+                    del exc[field]
 
         return exc
 
     for dataset in data:
         for key, value in list(dataset.items()):
             if not value:
                 del dataset[key]
```

### Comparing `unfold-1.0.6/unfold/export.py` & `unfold-1.0.7/unfold/export.py`

 * *Files identical despite different names*

### Comparing `unfold-1.0.6/unfold/fold.py` & `unfold-1.0.7/unfold/fold.py`

 * *Files identical despite different names*

### Comparing `unfold-1.0.6/unfold/unfold.py` & `unfold-1.0.7/unfold/unfold.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,47 @@
     """Remove list of elements from mapping."""
     for key in to_remove:
         del mapping[key]
 
     return mapping
 
 
+def get_list_unique_exchanges(databases: list) -> list:
+    """
+    Gets a list of all unique exchanges found in a list of databases.
+
+    :param databases: A list of Brightway2-style databases to extract unique exchanges from.
+    :return: A list of tuples representing unique exchanges, where each tuple contains the following information:
+        - name: The name of the exchange.
+        - product: The reference product of the exchange.
+        - categories: The categories of the exchange.
+        - location: The location of the exchange.
+        - unit: The unit of the exchange.
+        - type: The type of the exchange (either "technosphere" or "biosphere").
+    """
+
+    return list(
+        set(
+            [
+                (
+                    exchange["name"],
+                    exchange.get("product"),
+                    exchange.get("categories"),
+                    exchange.get("location"),
+                    exchange.get("unit"),
+                    exchange.get("type"),
+                )
+                for database in databases
+                for dataset in database
+                for exchange in dataset["exchanges"]
+            ]
+        )
+    )
+
+
 class Unfold:
     """Extracts datapackage files."""
 
     def __init__(self, path: Union[str, Path]):
         self.dict_meta = None
         self.acts_indices = None
         self.reversed_acts_indices = None
@@ -69,14 +102,15 @@
         self.scenarios = self.package.descriptor["scenarios"]
         self.scenario_df = None
         self.show_scenarios()
         self.database = []
         self.databases_to_export = {}
         self.dependency_mapping = {}
         self.factors = {}
+        self.name = None
 
     def show_scenarios(self):
         """Shows the scenarios."""
         print("The data package contains the following scenarios:")
         table = PrettyTable()
         table.field_names = ["No.", "Scenario", "Description"]
         for i, scenario in enumerate(self.package.descriptor["scenarios"]):
@@ -286,46 +320,14 @@
         factors.
 
         """
         self.factors = (
             self.scenario_df.groupby("flow id").sum(numeric_only=True).to_dict("index")
         )
 
-    def get_list_unique_exchanges(self, databases: list) -> list:
-        """
-        Gets a list of all unique exchanges found in a list of databases.
-
-        :param databases: A list of Brightway2-style databases to extract unique exchanges from.
-        :return: A list of tuples representing unique exchanges, where each tuple contains the following information:
-            - name: The name of the exchange.
-            - product: The reference product of the exchange.
-            - categories: The categories of the exchange.
-            - location: The location of the exchange.
-            - unit: The unit of the exchange.
-            - type: The type of the exchange (either "technosphere" or "biosphere").
-        """
-
-        return list(
-            set(
-                [
-                    (
-                        exchange["name"],
-                        exchange.get("product"),
-                        exchange.get("categories"),
-                        exchange.get("location"),
-                        exchange.get("unit"),
-                        exchange.get("type"),
-                    )
-                    for database in databases
-                    for dataset in database
-                    for exchange in dataset["exchanges"]
-                ]
-            )
-        )
-
     def store_datasets_metadata(self) -> None:
         """
         Stores metadata for each dataset in the database attribute.
 
         The resulting metadata is stored in the dict_meta attribute, which is a dictionary that maps dataset identifiers to their
         metadata.
 
@@ -355,15 +357,15 @@
             }
             for dataset in self.database
         }
 
     def generate_activities_indices(self) -> None:
         """Generates the indices of the unique activities."""
         # Get all unique activities from self.database.
-        list_unique_acts = self.get_list_unique_exchanges(databases=[self.database])
+        list_unique_acts = get_list_unique_exchanges(databases=[self.database])
 
         # Add additional exchanges to list_unique_acts.
         for act in list_unique_acts:
             if act[-1] == "production":
                 new_id = list(act)
                 new_id[-1] = "technosphere"
                 new_id = tuple(new_id)
@@ -407,17 +409,64 @@
         name, ref, cat, loc, unit, flow_type = self.acts_indices[ind]
         _ = lambda x: x if x != 0 else 1.0
 
         def fix_key(key: tuple) -> tuple:
             if key in self.dependency_mapping:
                 return self.dependency_mapping[key]
             else:
-                return self.dependency_mapping[
-                    (self.outdated_flows.get(key[0], key[0]), key[1], key[2], key[3])
-                ]
+                if key[0] in self.outdated_flows:
+                    if (
+                        self.outdated_flows[key[0]],
+                        key[1],
+                        key[2],
+                        key[3],
+                    ) in self.dependency_mapping:
+                        return self.dependency_mapping[
+                            (self.outdated_flows[key[0]], key[1], key[2], key[3])
+                        ]
+                    elif (
+                        self.outdated_flows[key[0]].replace(", ion", ""),
+                        key[1],
+                        key[2],
+                        key[3],
+                    ) in self.dependency_mapping:
+                        return self.dependency_mapping[
+                            (
+                                self.outdated_flows[key[0]].replace(", ion", ""),
+                                key[1],
+                                key[2],
+                                key[3],
+                            )
+                        ]
+                    elif (
+                        self.outdated_flows[key[0]] + ", ion",
+                        key[1],
+                        key[2],
+                        key[3],
+                    ) in self.dependency_mapping:
+                        return self.dependency_mapping[
+                            (
+                                self.outdated_flows[key[0]] + ", ion",
+                                key[1],
+                                key[2],
+                                key[3],
+                            )
+                        ]
+                    elif (
+                        key[0] + ", in ground",
+                        key[1],
+                        key[2],
+                        key[3],
+                    ) in self.dependency_mapping:
+                        return self.dependency_mapping[
+                            (key[0] + ", in ground", key[1], key[2], key[3])
+                        ]
+                    else:
+                        print("Could not find key", key)
+                        return key
 
         return {
             "name": name,
             "product": ref,
             "unit": unit,
             "location": loc,
             "categories": cat,
@@ -598,26 +647,26 @@
 
         # Build a list of activities and exchanges from the indices.
         new_db = []
         for k, v in inds_d.items():
             # Get the dictionary representing the current activity from the database.
             act = self.get_act_dict_structure(
                 ind=k,
-                scenario_name=self.package.descriptor["name"],
+                scenario_name=self.name or self.package.descriptor["name"],
             )
 
             # Update the activity dictionary with metadata.
             act.update(self.dict_meta[self.acts_indices[k]])
 
             # Add exchanges to the activity dictionary for each non-zero element in the row.
             act["exchanges"].extend(
                 self.get_exchange(
                     ind=j,
                     amount=matrix[j, k, 0],
-                    scenario_name=self.package.descriptor["name"],
+                    scenario_name=self.name or self.package.descriptor["name"],
                 )
                 for j in v
             )
 
             # Add the updated activity dictionary to the list of activities and exchanges.
             new_db.append(act)
 
@@ -899,35 +948,46 @@
             # Update the factor values for each scenario by multiplying with the corresponding matrix value
             for scenario, val in factor.items():
                 factor[scenario] = val * _(matrix[consumer_idx, supplier_idx])
 
         # Create a new scenario dataframe from the updated factors dictionary
         self.scenario_df = pd.DataFrame.from_dict(self.factors).T.reset_index()
 
-        # Rename columns and add new columns for database information and metadata
+        # Rename columns
+        # and add new columns
+        # for database information and metadata
         self.scenario_df.columns = [
             "to activity name",
             "to reference product",
             "to location",
             "to unit",
             "from activity name",
             "from reference product",
             "from location",
             "from categories",
             "from unit",
             "flow type",
         ] + [s["name"] for s in self.scenarios]
 
-        self.scenario_df["to database"] = self.package.descriptor["name"]
+        self.scenario_df["to database"] = self.name or self.package.descriptor["name"]
         self.scenario_df["to categories"] = None
         self.scenario_df["to key"] = None
         self.scenario_df["from key"] = None
         self.scenario_df = self.scenario_df.replace({np.nan: None})
 
-        # Use the dependency_mapping dictionary to add "from key" and "to key" columns
+        # if self.name is not None, we change the name of the database
+        # in self.dependency_mapping to the name of the superstructure
+        if self.name:
+            self.dependency_mapping = {
+                k: (self.name, v[1]) if v[0] == self.package.descriptor["name"] else v
+                for k, v in self.dependency_mapping.items()
+            }
+
+        # Use the dependency_mapping dictionary
+        # to add "from key" and "to key" columns
         self.scenario_df.loc[:, "from key"] = self.scenario_df.apply(
             lambda x: self.dependency_mapping.get(
                 (
                     x["from activity name"],
                     x["from reference product"],
                     x["from location"],
                     x["from categories"],
@@ -946,15 +1006,15 @@
             ),
             axis=1,
         )
 
         # Add "from database" column based on flow type
         self.scenario_df.loc[
             (self.scenario_df["flow type"] == "technosphere"), "from database"
-        ] = self.package.descriptor["name"]
+        ] = (self.name or self.package.descriptor["name"])
         self.scenario_df.loc[
             (self.scenario_df["flow type"] == "biosphere"), "from database"
         ] = "biosphere3"
         self.scenario_df = self.scenario_df[
             [
                 "from activity name",
                 "from reference product",
@@ -974,36 +1034,39 @@
         ]
 
     def unfold(
         self,
         scenarios: List[int] = None,
         dependencies: dict = None,
         superstructure: bool = False,
+        name: str = None,
     ):
         """
         unfold() is a method of the Unfold class, which extracts specific scenarios from the input LCA database and writes them as new databases.
 
         :param scenarios: A list of integers indicating the indices of the scenarios to extract. If None, all scenarios are extracted. Default is None.
         :param dependencies: A dictionary containing additional inventory databases that may be needed for extraction. Default is None.
         :param superstructure: A boolean indicating whether to generate a scenario difference file and a superstructure database. Default is False.
+        :param name: A string indicating the name of the superstructure database. Default is None.
         :return: None
 
         Behavior:
 
         Calls the check_dependencies() method to ensure that all required inventory databases are present.
         Calls the extract_source_database() method to extract the original LCA database.
         Calls the extract_additional_inventories() method to extract any additional inventory databases required.
         Calls the format_dataframe() method to format the scenario data into a Pandas DataFrame.
         Calls the generate_factors() method to generate the factors for the scenarios.
         If superstructure is False, calls the generate_single_databases() method to generate a separate LCA database for each scenario, and stores them in the databases_to_export dictionary.
         If superstructure is True, calls the format_superstructure_dataframe() method to generate a scenario difference file and a superstructure database.
-        Calls the write() method to write the databases to disk.
+        Calls write() method to write the databases to disk.
 
         """
 
+        self.name = name
         self.check_dependencies(dependencies)
         self.extract_source_database()
         self.extract_additional_inventories()
 
         self.format_dataframe(scenarios=scenarios, superstructure=superstructure)
         self.generate_factors()
 
@@ -1042,15 +1105,15 @@
                 correct_fields_format(database, scenario)
                 print(f"Writing database for scenario {scenario}...")
                 UnfoldExporter(scenario, database).write_database()
 
         else:
             try:
                 self.scenario_df.to_excel(
-                    f"{self.package.descriptor['name']}.xlsx", index=False
+                    f"{self.name or self.package.descriptor['name']}.xlsx", index=False
                 )
             except ValueError:
                 # from https://stackoverflow.com/questions/66356152/splitting-a-dataframe-into-multiple-sheets
                 GROUP_LENGTH = 1000000  # set nr of rows to slice df
                 with pd.ExcelWriter(
                     f"{self.package.descriptor['name']}.xlsx"
                 ) as writer:
@@ -1060,18 +1123,20 @@
                         )
 
             print(
                 f"Scenario difference file exported to {self.package.descriptor['name']}.xlsx!"
             )
             print("")
             print("Writing superstructure database...")
-            change_db_name(self.database, self.package.descriptor["name"])
+            change_db_name(self.database, self.name or self.package.descriptor["name"])
             self.database = check_exchanges_input(
                 self.database, self.dependency_mapping
             )
             link_internal(self.database)
             check_internal_linking(self.database)
             check_duplicate_codes(self.database)
-            correct_fields_format(self.database, self.package.descriptor["name"])
+            correct_fields_format(
+                self.database, self.name or self.package.descriptor["name"]
+            )
             UnfoldExporter(
-                self.package.descriptor["name"], self.database
+                self.name or self.package.descriptor["name"], self.database
             ).write_database()
```

### Comparing `unfold-1.0.6/unfold.egg-info/PKG-INFO` & `unfold-1.0.7/unfold.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfold
-Version: 1.0.6
+Version: 1.0.7
 Summary: Unpacks LCA scenario databases.
 Home-page: https://github.com/polca/premise
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

