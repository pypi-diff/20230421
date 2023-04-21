# Comparing `tmp/cjdb-1.1.0.tar.gz` & `tmp/cjdb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjdb-1.1.0.tar", max compression
+gzip compressed data, was "cjdb-1.2.0.tar", max compression
```

## Comparing `cjdb-1.1.0.tar` & `cjdb-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1065 2023-03-24 08:47:24.943711 cjdb-1.1.0/LICENSE
--rw-r--r--   0        0        0     1820 2023-04-06 14:32:49.893157 cjdb-1.1.0/README.md
--rw-r--r--   0        0        0     9397 2023-04-06 15:36:36.056059 cjdb-1.1.0/cjdb/README.md
--rw-r--r--   0        0        0        0 2023-03-24 08:47:24.944366 cjdb-1.1.0/cjdb/__init__.py
--rw-r--r--   0        0        0      564 2023-04-05 10:23:47.428044 cjdb-1.1.0/cjdb/main.py
--rw-r--r--   0        0        0     5008 2023-04-06 08:58:50.702731 cjdb-1.1.0/cjdb/model/README.md
--rw-r--r--   0        0        0        0 2023-03-24 08:47:24.987486 cjdb-1.1.0/cjdb/model/__init__.py
--rw-r--r--   0        0        0     4778 2023-04-06 11:09:51.718769 cjdb-1.1.0/cjdb/model/sqlalchemy_models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 08:47:24.944484 cjdb-1.1.0/cjdb/modules/__init__.py
--rw-r--r--   0        0        0     3199 2023-04-05 14:27:23.970495 cjdb-1.1.0/cjdb/modules/arg_parser.py
--rw-r--r--   0        0        0     2162 2023-04-05 12:24:10.108456 cjdb-1.1.0/cjdb/modules/checks.py
--rw-r--r--   0        0        0     1926 2023-04-05 12:24:10.110402 cjdb-1.1.0/cjdb/modules/extensions.py
--rw-r--r--   0        0        0     6836 2023-04-05 12:24:10.103852 cjdb-1.1.0/cjdb/modules/geometric.py
--rw-r--r--   0        0        0    15976 2023-04-06 12:46:29.824095 cjdb-1.1.0/cjdb/modules/importer.py
--rw-r--r--   0        0        0     1375 2023-04-05 12:24:10.114393 cjdb-1.1.0/cjdb/modules/utils.py
--rw-r--r--   0        0        0        0 2023-03-24 08:47:24.944949 cjdb-1.1.0/cjdb/resources/__init__.py
--rw-r--r--   0        0        0      783 2023-03-24 08:47:24.945006 cjdb-1.1.0/cjdb/resources/object_types.py
--rw-r--r--   0        0        0      798 2023-03-24 08:47:24.945052 cjdb-1.1.0/cjdb/resources/post_import.sql
--rw-r--r--   0        0        0     2079 2023-03-24 08:47:24.945116 cjdb-1.1.0/cjdb/resources/strings.py
--rw-r--r--   0        0        0      862 2023-04-06 15:13:09.211742 cjdb-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 cjdb-1.1.0/setup.py
--rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 cjdb-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-24 08:47:24.943711 cjdb-1.2.0/LICENSE
+-rw-r--r--   0        0        0    12711 2023-04-21 14:57:08.421775 cjdb-1.2.0/README.md
+-rw-r--r--   0        0        0      167 2023-04-21 14:57:08.422846 cjdb-1.2.0/cjdb/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-21 14:57:08.423404 cjdb-1.2.0/cjdb/logger.py
+-rw-r--r--   0        0        0      648 2023-04-21 14:57:08.423822 cjdb-1.2.0/cjdb/main.py
+-rw-r--r--   0        0        0     4966 2023-04-21 14:57:08.424374 cjdb-1.2.0/cjdb/model/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 07:29:22.588412 cjdb-1.2.0/cjdb/model/__init__.py
+-rw-r--r--   0        0        0     5239 2023-04-21 14:57:08.424706 cjdb-1.2.0/cjdb/model/sqlalchemy_models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:29:22.588804 cjdb-1.2.0/cjdb/modules/__init__.py
+-rw-r--r--   0        0        0     3410 2023-04-21 14:57:08.425457 cjdb-1.2.0/cjdb/modules/arg_parser.py
+-rw-r--r--   0        0        0     2180 2023-04-21 14:57:08.425797 cjdb-1.2.0/cjdb/modules/checks.py
+-rw-r--r--   0        0        0      838 2023-04-21 14:57:08.426042 cjdb-1.2.0/cjdb/modules/exceptions.py
+-rw-r--r--   0        0        0     2081 2023-04-21 14:57:08.426320 cjdb-1.2.0/cjdb/modules/extensions.py
+-rw-r--r--   0        0        0     6847 2023-04-21 14:57:08.426679 cjdb-1.2.0/cjdb/modules/geometric.py
+-rw-r--r--   0        0        0    16607 2023-04-21 14:57:08.426996 cjdb-1.2.0/cjdb/modules/importer.py
+-rw-r--r--   0        0        0     1599 2023-04-21 14:57:08.427292 cjdb-1.2.0/cjdb/modules/utils.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:29:22.590399 cjdb-1.2.0/cjdb/resources/__init__.py
+-rw-r--r--   0        0        0      875 2023-04-21 14:57:08.427663 cjdb-1.2.0/cjdb/resources/object_types.py
+-rw-r--r--   0        0        0      802 2023-04-21 14:57:08.427887 cjdb-1.2.0/cjdb/resources/post_import.sql
+-rw-r--r--   0        0        0     2107 2023-04-21 14:57:08.428211 cjdb-1.2.0/cjdb/resources/strings.py
+-rw-r--r--   0        0        0      926 2023-04-21 14:57:08.429390 cjdb-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    14134 1970-01-01 00:00:00.000000 cjdb-1.2.0/setup.py
+-rw-r--r--   0        0        0    13597 1970-01-01 00:00:00.000000 cjdb-1.2.0/PKG-INFO
```

### Comparing `cjdb-1.1.0/LICENSE` & `cjdb-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cjdb-1.1.0/cjdb/main.py` & `cjdb-1.2.0/cjdb/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from cjdb.modules.arg_parser import Parser, validate_args
 from cjdb.modules.importer import Importer
+from cjdb.modules.utils import get_db_engine
 
 
 def get_args():
     parser = Parser()
     args = parser.parse_args()
     validation_result, validation_msg = validate_args(args)
-    
+
     if validation_result:
         return args
     else:
         raise Exception(validation_msg)
 
 
 # organized like this to be able to call it in tests and also as CLI
 def run(args):
-    with Importer(args) as imp:
+    engine = get_db_engine(args)
+    with Importer(engine, args) as imp:
         imp.run_import()
 
+
 def main():
     args = get_args()
     run(args)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `cjdb-1.1.0/cjdb/model/README.md` & `cjdb-1.2.0/cjdb/model/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,34 +36,34 @@
 ### 1. import_meta <a name="import_meta"></a>
 
 The import_meta table stores information from imported files, e.g. name or metadata of the source file. Belowing section describes its attributes.
 
 <**id**: import_meta record's index within the database.<br/>
 **source_file**: name of the source file.<br/>
 **version**: cityJSON version used.<br/>
-**metadata**: [cityJSON metadata object](https://www.cityjson.org/specs/1.1.2/#metadata), a JSON object describing the creator, dataset extent or coordinate reference system used, etc.<br/>
-**transform**:[cityJSON transform object](https://www.cityjson.org/specs/1.1.2/#transform-object), a JSON object describing how to decompress the integer coordinates of the geometries to obtain real-world coordinates.<br/>
-**geometry_templates**: [cityJSON geometry-templates object](https://www.cityjson.org/specs/1.1.2/#geometry-templates), a JSON object containing the templates that can be reused by different City Objects (usually for trees).<br/>
+**metadata**: [cityJSON metadata object](https://www.cityjson.org/specs/#metadata), a JSON object describing the creator, dataset extent or coordinate reference system used, etc.<br/>
+**transform**:[cityJSON transform object](https://www.cityjson.org/specs/#transform-object), a JSON object describing how to decompress the integer coordinates of the geometries to obtain real-world coordinates.<br/>
+**geometry_templates**: [cityJSON geometry-templates object](https://www.cityjson.org/specs/#geometry-templates), a JSON object containing the templates that can be reused by different City Objects (usually for trees).<br/>
 **srid**: Coordinate reference system (CRS) of the imported city objects in the database. If not specified when importing, the CRS will be the same with the source file's CRS. If specified when importing, the CRS will be the specified CRS.<br/>
-**extensions**: [cityJSON Extensions](https://www.cityjson.org/specs/1.1.2/#extensions), a JSON file that documents how the core data model of CityJSON is extended.<br/>
-**extra_properties**: [extraRootProperties](https://www.cityjson.org/specs/1.1.2/#case-2-adding-new-properties-at-the-root-of-a-document), a JSON object with added new properties at the root of the imported document.<br/>
+**extensions**: [cityJSON Extensions](https://www.cityjson.org/specs/#extensions), a JSON file that documents how the core data model of CityJSON is extended.<br/>
+**extra_properties**: [extraRootProperties](https://www.cityjson.org/specs/#case-2-adding-new-properties-at-the-root-of-a-document), a JSON object with added new properties at the root of the imported document.<br/>
 **started_at**: importing start time.<br/>
 **finished_at**: importing finish time. `null` if not finished.<br/>
 **Bounding box**: bounding box is taken from the `geographicExtent` object from the `metadata` section
 
 ### 2. cj_object <a name="cj_object"></a>
 
 The cj_object model stores individual city objects, for instance buildings, roads, or bridges. Its attributes are described below. The **attributes** and **geometry** are seperated into two jsonb column for query optimization purpose.
 
 **id**: city object's index within the database.<br/>
 **import_meta_id**: the source file id of the city object, foriegn key to the id column of import_meta table.<br/>
 **object_id**: the identification string of the city object (e.g. NL.IMBAG.Pand.0503100000000033-0).<br/>
 **type**: type of the city object (e.g. building, buildingparts, etc.).<br/>
-**attributes**:[cityJSON attributes](https://www.cityjson.org/specs/1.1.2/#attributes-for-all-city-objects), a JSON object that describes attributes of the city object (e.g. roof type, area, etc.).<br/>
-**geometry**: [cityJSON geometry](https://www.cityjson.org/specs/1.1.2/#geometry-objects), a JSON object that describes the geometry of the city object.<br/>
+**attributes**:[cityJSON attributes](https://www.cityjson.org/specs/#attributes-for-all-city-objects), a JSON object that describes attributes of the city object (e.g. roof type, area, etc.).<br/>
+**geometry**: [cityJSON geometry](https://www.cityjson.org/specs/#geometry-objects), a JSON object that describes the geometry of the city object.<br/>
 **ground_geometry**: ground geometry of the city object, in geometry type.<br/>
 
 ### 3. Family <a name="family"></a>
 The family model stores the relations between city objects.
 
 **id**: family object's index within the database.<br/>
 **parent_id**: the identification id of the parent object.<br/>
```

### Comparing `cjdb-1.1.0/cjdb/model/sqlalchemy_models/__init__.py` & `cjdb-1.2.0/cjdb/model/sqlalchemy_models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,114 +1,142 @@
-from sqlalchemy import Column, ForeignKey, \
-    String, func, Integer, UniqueConstraint
-from sqlalchemy.orm import relationship, declarative_base
-from sqlalchemy.dialects.postgresql import JSONB, TIMESTAMP
+import sys
+
 from geoalchemy2 import Geometry
+from sqlalchemy import (Column, ForeignKey, Integer, String, UniqueConstraint,
+                        func)
+from sqlalchemy.dialects.postgresql import JSONB, TIMESTAMP
+from sqlalchemy.orm import declarative_base, relationship
+
+from cjdb.logger import logger
 
 Base = declarative_base()
 
+
 class BaseModel(Base):
     __abstract__ = True
     id = Column(Integer, primary_key=True)
 
 
 def NullableJSONB():
     return JSONB(none_as_null=True)
 
 
 class ImportMetaModel(BaseModel):
-    __tablename__ = 'import_meta'
-    __table_args__ = {'schema':'cjdb'}
+    __tablename__ = "import_meta"
+    __table_args__ = {"schema": "cjdb"}
     source_file = Column(String)
     version = Column(String(10), nullable=False)
     meta = Column(JSONB, name="metadata")
     transform = Column(NullableJSONB())
     geometry_templates = Column(NullableJSONB())
     srid = Column(Integer)
     extensions = Column(NullableJSONB())
     extra_properties = Column(NullableJSONB())
     started_at = Column(TIMESTAMP, default=func.now())
     finished_at = Column(TIMESTAMP)
-    bbox = Column(Geometry('Polygon'))
+    bbox = Column(Geometry("Polygon"))
 
-    def compare_existing(self, session, ignore_repeated_file):
+    def compare_existing(self, session, ignore_repeated_file, update_existing):
         result_ok = True
 
         # check if the file was already imported
-        if self.source_file.lower() != 'stdin' and not ignore_repeated_file:
-            same_source_import = session.query(ImportMetaModel)\
-                .filter_by(source_file=self.source_file)\
-                .filter(ImportMetaModel.finished_at.isnot(None))\
-                .order_by(ImportMetaModel.finished_at.desc())\
+        if self.source_file.lower() != "stdin" and \
+           not ignore_repeated_file and \
+           not update_existing:
+            same_source_import = (
+                session.query(ImportMetaModel)
+                .filter_by(source_file=self.source_file)
+                .filter(ImportMetaModel.finished_at.isnot(None))
+                .order_by(ImportMetaModel.finished_at.desc())
                 .first()
+            )
             if same_source_import:
-                print(f"\nFile '{self.source_file}' was previously imported at {same_source_import.finished_at}.\n" \
-                        "Use the -g flag to suppress this warning")
-                user_answer = input("Should the import continue? " +
-                                    "Already imported City Objects will " +
-                                    "be skipped. If you want to update " +
-                                    "use the flag --update-existing. \n" +
-                                    " [y / n]\n")
+                logger.warning(
+                    "File %s was previously imported at %s. "
+                    "Use the -g flag to suppress this warning.",
+                    self.source_file,  same_source_import.finished_at
+                )
+
+                user_answer = input(
+                    "Should the import continue? "
+                    "Already imported City Objects will be skipped. "
+                    "If you want to update them instead "
+                    "use the flag --update-existing. \n"
+                    " [y / n]\n"
+                )
                 if user_answer.lower() != "y":
-                    return False
-    
+                    logger.info("Import process terminated by user.")
+                    sys.exit(1)
+
         # check if the CRS is consistent with other imports
-        different_srid_meta = session.query(ImportMetaModel)\
-                            .filter(ImportMetaModel.srid != self.srid)\
-                            .filter(ImportMetaModel.finished_at.isnot(None))\
-                            .order_by(ImportMetaModel.finished_at.desc())\
-                            .first()
+        different_srid_meta = (
+            session.query(ImportMetaModel)
+            .filter(ImportMetaModel.srid != self.srid)
+            .filter(ImportMetaModel.finished_at.isnot(None))
+            .order_by(ImportMetaModel.finished_at.desc())
+            .first()
+        )
 
         if different_srid_meta:
-            print("Inconsistent Coordinate Reference Systems detected")
-            print(f"Currently imported SRID: {self.srid}")
-            print(f"Recently imported SRID: {different_srid_meta.srid}")
-            print("Use the '-I/--srid' flag to reproject everything to a single specified CRS",
-                    "or modify source data.")
+            logger.error("Inconsistent Coordinate Reference Systems detected."
+                         "\nCurrently imported SRID: %s \n"
+                         "Recently imported SRID: %s "
+                         "\nUse the '-I/--srid' flag to reproject everything "
+                         "to a single specified CRS or modify source data.",
+                         self.srid, different_srid_meta.srid
+                         )
             return False
 
         return result_ok
 
 
 class CjObjectModel(BaseModel):
-    __tablename__ = 'cj_object'
-    __table_args__ = {'schema':'cjdb'}
+    __tablename__ = "cj_object"
+    __table_args__ = {"schema": "cjdb"}
     import_meta_id = Column(Integer, ForeignKey(ImportMetaModel.id))
     object_id = Column(String, nullable=False, unique=True)
     type = Column(String, nullable=False)
     attributes = Column(NullableJSONB())
     geometry = Column(NullableJSONB())
-    ground_geometry=Column(Geometry('MultiPolygon'))
+    ground_geometry = Column(Geometry("MultiPolygon"))
     import_meta = relationship(ImportMetaModel)
 
     @classmethod
     def get_attributes_and_types(cls, session):
         # sample attributes for each object type
-        # this is needed to create proper indexes and also to use those indexes when querying
-        sampled_objects = session.query(cls)\
-            .distinct(cls.type)\
-            .filter(cls.attributes.isnot(None))\
-            .order_by(cls.type, cls.id.desc())\
+        # this is needed to create proper indexes and also
+        # to use those indexes when querying
+        sampled_objects = (
+            session.query(cls)
+            .distinct(cls.type)
+            .filter(cls.attributes.isnot(None))
+            .order_by(cls.type, cls.id.desc())
             .all()
+        )
 
-        # create type mapping for each attribute appearing across all object types
-        # this considers that different object types have different attributes
-        # if same object types have different attributes, then this will not work correctly
+        # create type mapping for each attribute appearing
+        # across all object types this considers that different
+        # object types have different attributes if same object
+        # types have different attributes, then this will not work correctly
         type_mapping = {}
         if sampled_objects:
             for cj_obj in sampled_objects:
                 for attr_name, value in cj_obj.attributes.items():
                     type_mapping[attr_name] = type(value)
 
         return type_mapping
 
 
 class FamilyModel(BaseModel):
-    __tablename__ = 'family'
-    __table_args__ = {'schema':'cjdb'}
+    __tablename__ = "family"
+    __table_args__ = {"schema": "cjdb"}
     parent_id = Column(String, ForeignKey(CjObjectModel.object_id))
     child_id = Column(String, ForeignKey(CjObjectModel.object_id))
 
-    parent = relationship(CjObjectModel, foreign_keys=[parent_id], post_update=True)
-    child = relationship(CjObjectModel, foreign_keys=[child_id], post_update=True)
+    parent = relationship(CjObjectModel,
+                          foreign_keys=[parent_id],
+                          post_update=True)
+    child = relationship(CjObjectModel,
+                         foreign_keys=[child_id],
+                         post_update=True)
 
     parent_child_unique = UniqueConstraint(parent_id, child_id)
```

### Comparing `cjdb-1.1.0/cjdb/modules/arg_parser.py` & `cjdb-1.2.0/cjdb/modules/arg_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import os
 from getpass import getpass
 
+from cjdb import __version__
 from cjdb.resources import strings as s
 
 
 def Parser():
     parser = argparse.ArgumentParser(
         description="Import CityJSONL to a PostgreSQL database",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -16,81 +17,96 @@
         nargs="?",
         default="stdin",
         type=str,
         metavar="file_or_directory",
         help=s.filepath_help,
     )
 
+    parser.add_argument(
+        "--version",
+        action="version",
+        version='%(prog)s ' + __version__,
+        help=s.version_help,
+    )
+
     db = parser.add_argument_group(title="Database connection arguments")
 
     db.add_argument(
         "-H",
         "--host",
         type=str,
         default="localhost",
         help=s.host_help,
         dest="db_host"
     )
+
     db.add_argument(
         "-p",
         "--port",
         type=int,
         default=5432,
         help=s.port_help,
         dest="db_port"
     )
+
     db.add_argument(
         "-U",
         "--user",
         type=str,
         required=True,
         help=s.user_help,
         dest="db_user"
     )
+
     db.add_argument(
         "-W",
         "--password",
         type=str,
         default=os.getenv("PGPASSWORD", None),
         help=s.password_help,
         dest="db_password",
     )
+
     db.add_argument(
         "-d",
         "--database",
         type=str,
         required=True,
         help=s.database_help,
         dest="db_name",
     )
+
     db.add_argument(
         "-s",
         "--schema",
         type=str,
-        default="public",
+        default="cjdb",
         help=s.schema_help,
         dest="db_schema",
     )
+
     parser.add_argument(
         "-I",
         "--srid",
         type=int,
         default=None,
         help=s.srid_help,
         dest="target_srid"
     )
+
     parser.add_argument(
         "-x",
         "--attr-index",
         type=str,
         action="append",
         default=[],
         help=s.index_help,
         dest="indexed_attributes",
     )
+
     parser.add_argument(
         "-px",
         "--partial-attr-index",
         type=str,
         action="append",
         default=[],
         help=s.partial_index_help,
@@ -104,23 +120,25 @@
         action="store_const",
         const=True,
         help=s.ignore_file_help,
         dest="ignore_repeated_file",
     )
 
     mode = parser.add_mutually_exclusive_group()
+
     mode.add_argument(
         "-a",
         "--append",
         default=False,
         action="store_const",
         const=True,
         help=s.append_help,
         dest="append_mode",
     )
+
     mode.add_argument(
         "-o",
         "--overwrite",
         default=False,
         action="store_const",
         const=True,
         help=s.overwrite_help,
@@ -141,10 +159,12 @@
 
 
 # perform some other checks for validity
 def validate_args(args):
     result = True
     msg = ""
     if not args.db_password:
-        args.db_password = getpass(prompt=f'Password for user "{args.db_user}": ') # noqa
+        args.db_password = getpass(
+            prompt=f'Password for user "{args.db_user}": '
+        )  # noqa
 
     return result, msg
```

### Comparing `cjdb-1.1.0/cjdb/modules/extensions.py` & `cjdb-1.2.0/cjdb/modules/extensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import json
 
 import requests
 
+from cjdb.logger import logger
+
 
 class ExtensionHandler:
     def __init__(self, extensions):
         self.full_definitions = {}
         self.extra_root_properties = []
         self.extra_attributes = {}
         self.extra_city_objects = []
-        
+
         if extensions:
             self.get_extensions(extensions)
 
     def get_extensions(self, extensions):
         for ext_name, content in extensions.items():
             url = content.get("url")
             if url:
@@ -23,31 +25,32 @@
                     resp = None
 
                 if resp and resp.status_code == 200:
                     try:
                         ext_definition = json.loads(resp.text)
                         self.full_definitions[ext_name] = ext_definition
                     except ValueError as e:
-                        print(f"Extension url: {url} did not provide a correct json schema")
+                        logger.error(
+                            "Extension url: %s did not provide a correct json"
+                            " schema", url
+                        )
                         # raise
                         # throw this exception or ignore it?
                         return
 
                     for prop_name in ext_definition["extraRootProperties"]:
                         self.extra_root_properties.append(prop_name)
 
-                    for obj_type, extra_attributes in ext_definition["extraAttributes"].items():
+                    for obj_type, extra_attributes in ext_definition[
+                        "extraAttributes"
+                    ].items():
                         if obj_type not in self.extra_attributes:
                             self.extra_attributes[obj_type] = []
                         for attr_name in extra_attributes:
                             self.extra_attributes[obj_type].append(attr_name)
 
                     for obj_type in ext_definition["extraCityObjects"]:
                         self.extra_city_objects.append(obj_type)
                 else:
                     msg = f"Extension url: {url} did not return a correct response"
                     # raise Exception(msg)
                     return
-
-    
-
-
```

### Comparing `cjdb-1.1.0/cjdb/modules/geometric.py` & `cjdb-1.2.0/cjdb/modules/geometric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
-from collections import OrderedDict
 
 import numpy as np
 from pyproj import CRS, Transformer
-from pyproj.transformer import TransformerGroup
-from shapely.geometry import MultiPolygon, Point, Polygon, box
-from shapely.validation import explain_validity, make_valid
+from shapely.geometry import MultiPolygon, Point, Polygon
+from shapely.validation import explain_validity
+
+from cjdb.logger import logger
 
 
 # get srid from a CRS string definition
 def get_srid(crs):
     if crs:
         proj = CRS.from_string(crs)
         srid = proj.to_epsg()
@@ -36,30 +36,32 @@
 
 
 def reproject_vertex_list(vertices, srid_from, srid_to):
     source_proj = CRS.from_epsg(srid_from)
     target_proj = CRS.from_epsg(srid_to)
 
     # prepare transformer from crs to crs
-    transformer = Transformer.from_crs(source_proj, target_proj, always_xy=True)
+    transformer = Transformer.from_crs(source_proj,
+                                       target_proj,
+                                       always_xy=True)
 
     # transform all the coordinates
     reprojected_xyz = transformer.transform(*zip(*vertices))
     reprojected_xyz = [list(i) for i in zip(*reprojected_xyz)]
 
     return reprojected_xyz
 
 
 def resolve(lod_level, vertices, inplace=True):
     if inplace:
         resolvable = lod_level
     else:
         resolvable = copy.deepcopy(lod_level)
 
-    for boundary in resolvable['boundaries']:
+    for boundary in resolvable["boundaries"]:
         for i, shell in enumerate(boundary):
             if type(shell[0]) is list:
                 for j, ring in enumerate(shell):
                     new_ring = []
                     for vertex_id in ring:
                         xyz = vertices[vertex_id]
                         new_ring.append(xyz)
@@ -69,124 +71,137 @@
                 for vertex_id in shell:
                     xyz = vertices[vertex_id]
                     new_shell.append(xyz)
                 boundary[i] = new_shell
 
     return resolvable
 
-def resolve_template(lod_level, vertices, geometry_templates, source_target_srid):
+
+def resolve_template(lod_level,
+                     vertices,
+                     geometry_templates,
+                     source_target_srid):
     # get anchor point
     vertex_id = lod_level["boundaries"][0]
     anchor = vertices[vertex_id]
 
     # apply transformation matrix to the template vertices
-    template_vertices = [transform_with_rotation(v, lod_level["transformationMatrix"]) 
-            for v in geometry_templates["vertices-templates"]]
+    template_vertices = [
+        transform_with_rotation(v, lod_level["transformationMatrix"])
+        for v in geometry_templates["vertices-templates"]
+    ]
 
     # add anchor point to the vertices
     template_vertices = [list(np.array(v) + anchor) for v in template_vertices]
 
     # reproject vertices if needed
     if source_target_srid:
-        template_vertices = reproject_vertex_list(template_vertices, *source_target_srid)
+        template_vertices = reproject_vertex_list(
+            template_vertices, *source_target_srid
+        )
 
     # dereference template vertices
     template_id = lod_level["template"]
     template = geometry_templates["templates"][template_id]
-    
-    # inplace=False, because the template can be resolved differently for some other cityobject
+
+    # inplace=False, because the template can be resolved differently
+    # for some other cityobject
     resolved_template = resolve(template, template_vertices, inplace=False)
     return resolved_template
 
 
-def resolve_geometry_vertices(geometry, vertices, 
-                                geometry_templates, source_target_srid):
-
-    # use ready vertices to resolve coordinate values for the geometry (or geometry template)
+def resolve_geometry_vertices(
+    geometry, vertices, geometry_templates, source_target_srid
+):
+    # use ready vertices to resolve coordinate values
+    # for the geometry (or geometry template)
     for i, lod_level in enumerate(geometry):
         if lod_level["type"] == "GeometryInstance":
-            resolved_template = resolve_template(lod_level, 
-                                                vertices,
-                                                geometry_templates,
-                                                source_target_srid)
+            resolved_template = resolve_template(
+                lod_level, vertices, geometry_templates, source_target_srid
+            )
             geometry[i] = resolved_template
         else:
             # resolve without geometry template
             resolve(lod_level, vertices)
 
     return geometry
 
 
 def get_ground_geometry(geometry, obj_id):
     # returns a shapely multipolygon (see shapely.geometry.MultiPolygon)
     # the MultiPolygon should be a 2D geometry (Z coordinate is omitted)
-    # this geometry should be obtained by parsing the "geometry" object from cityjson -> the argument of this function
-    # the geometry is a multipolygon of all the ground surfaces in the lowest available LOD
+    # this geometry should be obtained by parsing the "geometry" object
+    # from cityjson -> the argument of this function
+    # the geometry is a multipolygon of all the ground
+    # surfaces in the lowest available LOD
 
-    planes=dict()
-    z_min=0
+    planes = dict()
+    z_min = 0
     for boundary in geometry[0]["boundaries"]:
         for i, shell in enumerate(boundary):
             if type(shell[0]) is list:
                 if type(shell[0][0]) is list:
                     for ring in shell:
-                        Point_list=[]
-                        z_tot=0
-                        z_count=0
-                        for x,y,z in ring:
-                            z_tot=z+z_tot
-                            z_count=z_count+1
-                            p=Point(x,y,z)
+                        Point_list = []
+                        z_tot = 0
+                        z_count = 0
+                        for x, y, z in ring:
+                            z_tot = z + z_tot
+                            z_count = z_count + 1
+                            p = Point(x, y, z)
                             Point_list.append(p)
-                        z_avg=round(z_tot/z_count,6)
-                        z_min=z_avg
-                        planes[str(z_avg)]=Point_list                
+                        z_avg = round(z_tot / z_count, 6)
+                        z_min = z_avg
+                        planes[str(z_avg)] = Point_list
                 else:
-                    Point_list=[]                   
-                    z_tot=0
-                    z_count=0
-                    for x,y,z in shell:
-                        z_tot=z+z_tot
-                        z_count=z_count+1
-                        p=Point(x,y,z)
+                    Point_list = []
+                    z_tot = 0
+                    z_count = 0
+                    for x, y, z in shell:
+                        z_tot = z + z_tot
+                        z_count = z_count + 1
+                        p = Point(x, y, z)
                         Point_list.append(p)
-                    z_avg=round(z_tot/z_count,6)
-                    z_min=z_avg
-                    planes[str(z_avg)]=Point_list
-    
+                    z_avg = round(z_tot / z_count, 6)
+                    z_min = z_avg
+                    planes[str(z_avg)] = Point_list
+
     for key in planes:
-        z_num=float(key)
-        if(z_num<z_min):
-            z_min=z_num
+        z_num = float(key)
+        if z_num < z_min:
+            z_min = z_num
 
-    ground_points=[]
-    ground_points_dic={}
+    ground_points = []
+    ground_points_dic = {}
 
     for key in planes:
-        if(abs(float(key)-z_min)<0.3):
-            poly = Polygon([[p.x, p.y] for p in planes[key]])
+        if abs(float(key) - z_min) < 0.3:
             for p in planes[key]:
-                str_p=str(p.x)+" "+str(p.y)
-                if((str_p in ground_points_dic.keys())is False):
-                    ground_points_dic[str_p]=0
-    
+                str_p = str(p.x) + " " + str(p.y)
+                if (str_p in ground_points_dic.keys()) is False:
+                    ground_points_dic[str_p] = 0
+
     for key in ground_points_dic:
-        p_x=key.split()[0]
-        p_y=key.split()[1]
-        p=Point(float(p_x),float(p_y))
-        ground_points.append(p) 
+        p_x = key.split()[0]
+        p_y = key.split()[1]
+        p = Point(float(p_x), float(p_y))
+        ground_points.append(p)
 
-    if(len(ground_points)>=3):
-        ground_polygon=Polygon([[p.x, p.y] for p in ground_points])
+    if len(ground_points) >= 3:
+        ground_polygon = Polygon([[p.x, p.y] for p in ground_points])
     else:
-        print(f"Warning: Ground geometry for object ID=({obj_id}) could not be calculated.")
+        logger.warning(
+            f"Ground geometry for object ID=({obj_id}) could not be"
+            " calculated."
+        )
         return None
-    
-    if(ground_polygon.is_valid==False):
-        ground_polygon=ground_polygon.buffer(0)
-        if(ground_polygon.is_valid==False):
-            print(explain_validity(ground_polygon))
 
-    if (type(ground_polygon) is Polygon):
-        ground_polygon=MultiPolygon([ground_polygon])
+    if ground_polygon.is_valid is False:
+        ground_polygon = ground_polygon.buffer(0)
+        if ground_polygon.is_valid is False:
+            logger.info(explain_validity(ground_polygon))
+
+    if type(ground_polygon) is Polygon:
+        ground_polygon = MultiPolygon([ground_polygon])
 
-    return ground_polygon
+    return ground_polygon
```

### Comparing `cjdb-1.1.0/cjdb/modules/importer.py` & `cjdb-1.2.0/cjdb/modules/importer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 import json
 import os
 import sys
 from pathlib import Path
+from typing import Optional, Tuple
 
+from shapely.geometry.base import BaseGeometry
 from sqlalchemy import func, text
 from sqlalchemy.dialects.postgresql import insert
 from sqlalchemy.orm import Session
 
-from cjdb.modules.checks import (
-    check_object_type,
-    check_reprojection,
-    check_root_properties,
-)
+from cjdb.logger import logger
+from cjdb.model.sqlalchemy_models import (BaseModel, CjObjectModel,
+                                          FamilyModel, ImportMetaModel)
+from cjdb.modules.checks import (check_object_type, check_reprojection,
+                                 check_root_properties)
+from cjdb.modules.exceptions import (InvalidCityJSONObjectException,
+                                     InvalidMetadataException)
 from cjdb.modules.extensions import ExtensionHandler
-from cjdb.modules.geometric import (
-    get_ground_geometry,
-    get_srid,
-    reproject_vertex_list,
-    resolve_geometry_vertices,
-    transform_vertex,
-)
-from cjdb.modules.utils import (
-    find_extra_properties,
-    get_cj_object_types,
-    get_db_engine,
-    to_dict,
-)
-from cjdb.model.sqlalchemy_models import (
-    BaseModel,
-    CjObjectModel,
-    FamilyModel,
-    ImportMetaModel,
-)
+from cjdb.modules.geometric import (get_ground_geometry, get_srid,
+                                    reproject_vertex_list,
+                                    resolve_geometry_vertices,
+                                    transform_vertex)
+from cjdb.modules.utils import (find_extra_properties, get_cj_object_types,
+                                is_cityjson_object, to_dict)
 
 
 # class to store variables per file import - for clarity
 class SingleFileImport:
     def __init__(self, file="stdin"):
         self.file = file
         self.target_srid = None
@@ -46,310 +37,321 @@
         )
         self.cj_objects = []
         self.families = []
 
 
 # importer class called once per whole import
 class Importer:
-    def __init__(self, args):
+    def __init__(self, engine, args):
+        self.engine = engine
         self.args = args
         # get allowed types for validation
         self.cj_object_types = get_cj_object_types()
         self.current = SingleFileImport()
 
         for table in BaseModel.metadata.tables.values():
             table.schema = self.args.db_schema
 
     def __enter__(self):
-        self.engine = get_db_engine(self.args)
         self.session = Session(self.engine)
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.session.close()
 
-    def run_import(self):
+    def run_import(self) -> None:
         # create model if in create mode, else append data
         if not self.args.append_mode:
             self.prepare_database()
         self.parse_cityjson()
         self.session.commit()
         # post import operations like clustering, indexing...
         if not self.args.append_mode:
             self.post_import()
         self.current.import_meta.finished_at = func.now()
         self.session.commit()
-        print(f"Imported from {self.args.filepath} successfully")
+        logger.info(f"Imported from {self.args.filepath} successfully")
 
-    def prepare_database(self):
+    def prepare_database(self) -> None:
+        """Adds the postgis extension and creates
+        the schema and the tables."""
         with self.engine.connect() as conn:
+            conn.execute(text("""CREATE EXTENSION IF NOT EXISTS postgis"""))
             if self.args.overwrite:
-                conn.execute(
-                    text(f"""DROP SCHEMA
+                conn.execute(text(f"""DROP SCHEMA
                              IF EXISTS {self.args.db_schema}
-                             CASCADE""")
-                )
+                             CASCADE"""))
             conn.execute(text(f"""CREATE SCHEMA IF NOT EXISTS
                                   {self.args.db_schema}"""))
-
+            conn.commit()
         # create all tables defined as SqlAlchemy models
         for table in BaseModel.metadata.tables.values():
             table.create(self.engine, checkfirst=True)
 
-    def parse_cityjson(self):
+    def parse_cityjson(self) -> None:
+        """Parses the input path."""
         source_path = self.args.filepath
 
         if os.path.isfile(source_path) or source_path.lower() == "stdin":
             self.process_file(source_path)
 
         elif os.path.isdir(source_path):
             self.process_directory(source_path)
 
         else:
             raise Exception(f"Path: '{source_path}' not found")
 
-    def post_import(self):
-        # post import operations like clustering, indexing...
+    def post_import(self) -> None:
+        """Perform post import operation on the schema,
+           like clustering and indexing"""
 
         cur_path = Path(__file__).parent
         sql_path = os.path.join(cur_path.parent, "resources/post_import.sql")
 
         with open(sql_path) as f:
             cmd = f.read().format(schema=self.args.db_schema)
         with self.engine.connect() as conn:
             conn.execute(text(cmd))
         self.index_attributes()
 
-    def process_line(self, line):
-        line_json = json.loads(line)
-        if "metadata" in line_json:
-            extra_root_properties = find_extra_properties(line_json)
-            self.current.source_srid = get_srid(
-                line_json["metadata"].get("referenceSystem")
-            )
-            if not self.current.source_srid:
-                print(
-                    """Warning: No Coordinate Reference System
-                       specified for the dataset."""
-                )
-
-            # use specified target SRID for all the geometries
-            # If not specified use same as source.
-            if self.args.target_srid and self.current.source_srid:
-                self.current.target_srid = self.args.target_srid
-                check_reprojection(self.current.source_srid, self.current.target_srid) # noqa
-            elif self.args.target_srid:
-                self.current.target_srid = self.args.target_srid
-            else:
-                self.current.target_srid = self.current.source_srid
+    def extract_import_metadata(self, line_json):
+        if "metadata" not in line_json:
+            raise InvalidMetadataException("The file should contain a member"
+                                           "'metadata', in the first object")
+
+        extra_root_properties = find_extra_properties(line_json)
+        self.current.source_srid = get_srid(
+            line_json["metadata"].get("referenceSystem")
+        )
+        if not self.current.source_srid:
+            logger.warning("No Coordinate Reference System"
+                           " specified for the dataset.")
+
+        # use specified target SRID for all the geometries
+        # If not specified use same as source.
+        if self.args.target_srid and self.current.source_srid:
+            self.current.target_srid = self.args.target_srid
+            check_reprojection(self.current.source_srid,
+                               self.current.target_srid)
+        elif self.args.target_srid:
+            self.current.target_srid = self.args.target_srid
+        else:
+            self.current.target_srid = self.current.source_srid
 
-            # calculate dataset bbox based on geographicalExtent
-            bbox = None
-            if "geographicalExtent" in line_json["metadata"]:
-                bbox_coords = line_json["metadata"]["geographicalExtent"]
-                bbox_vertices = [bbox_coords[:3], bbox_coords[3:]]
-
-                if (
-                    self.current.source_srid
-                    and self.current.target_srid != self.current.source_srid
-                ):
-                    bbox_vertices = reproject_vertex_list(
-                        bbox_vertices,
-                        self.current.source_srid,
-                        self.current.target_srid,
-                    )
+        # calculate dataset bbox based on geographicalExtent
+        bbox = None
+        if "geographicalExtent" in line_json["metadata"]:
+            bbox_coords = line_json["metadata"]["geographicalExtent"]
+            bbox_vertices = [bbox_coords[:3], bbox_coords[3:]]
 
-                bbox = func.st_makeenvelope(
-                    bbox_vertices[0][0],
-                    bbox_vertices[0][1],
-                    bbox_vertices[1][0],
-                    bbox_vertices[1][1],
+            if (
+                self.current.source_srid
+                and self.current.target_srid != self.current.source_srid
+            ):
+                bbox_vertices = reproject_vertex_list(
+                    bbox_vertices,
+                    self.current.source_srid,
                     self.current.target_srid,
                 )
 
-            # store extensions data - extra root properties, extra city objects
-            self.current.extension_handler = ExtensionHandler(
-                line_json.get("extensions")
+            bbox = func.st_makeenvelope(
+                bbox_vertices[0][0],
+                bbox_vertices[0][1],
+                bbox_vertices[1][0],
+                bbox_vertices[1][1],
+                self.current.target_srid,
             )
 
-            # prepare extra properties coming from extensions
-            # they will be placed in the extra_properties jsonb column
-            extra_properties_obj = {}
-            for prop_name in extra_root_properties:
-                extra_properties_obj[prop_name] = line_json[prop_name]
-
-            # check the occurring properties against
-            # the extension defined extra properties
-            check_root_properties(
-                extra_root_properties,
-                self.current.extension_handler.extra_root_properties,
-            )
+        # store extensions data - extra root properties, extra city objects
+        self.current.extension_handler = ExtensionHandler(
+            line_json.get("extensions")
+        )
 
-            # "or None" is added to change empty json "{}" to database null
-            import_meta = ImportMetaModel(
-                source_file=os.path.basename(self.current.file),
-                version=line_json["version"],
-                meta=line_json.get("metadata") or None,
-                transform=line_json.get("transform") or None,
-                geometry_templates=line_json.get("geometry-templates") or None,
-                srid=self.current.target_srid,
-                extensions=line_json.get("extensions") or None,
-                extra_properties=extra_properties_obj or None,
-                bbox=bbox,
-            )
+        # prepare extra properties coming from extensions
+        # they will be placed in the extra_properties jsonb column
+        extra_properties_obj = {}
+        for prop_name in extra_root_properties:
+            extra_properties_obj[prop_name] = line_json[prop_name]
+
+        # check the occurring properties against
+        # the extension defined extra properties
+        check_root_properties(
+            extra_root_properties,
+            self.current.extension_handler.extra_root_properties,
+        )
 
-            # compare to existing import metas
-            # for example to detect inconsistent CRS from different files
-            result_ok = import_meta.compare_existing(
-                self.session, self.args.ignore_repeated_file
-            )
-            if not result_ok:
-                print("Cancelling import")
-                sys.exit(1)
-
-            # add metadata to the database
-            import_meta.__table__.schema = self.args.db_schema
-            self.current.import_meta = import_meta
-            self.session.add(import_meta)
-            self.session.commit()
+        # "or None" is added to change empty json "{}" to database null
+        import_meta = ImportMetaModel(
+            source_file=os.path.basename(self.current.file),
+            version=line_json["version"],
+            meta=line_json.get("metadata") or None,
+            transform=line_json.get("transform") or None,
+            geometry_templates=line_json.get("geometry-templates") or None,
+            srid=self.current.target_srid,
+            extensions=line_json.get("extensions") or None,
+            extra_properties=extra_properties_obj or None,
+            bbox=bbox,
+        )
 
-        else:
-            # unpack vertices for the cityobjects based on
-            # the CityJSON transform
-            # this is done once for the CityJSONFeature
-            vertices = [
-                transform_vertex(v, self.current.import_meta.transform)
-                for v in line_json["vertices"]
-            ]
+        # compare to existing import metas
+        # for example to detect inconsistent CRS from different files
+        result_ok = import_meta.compare_existing(
+            self.session,
+            self.args.ignore_repeated_file,
+            self.args.update_existing
+        )
+        if not result_ok:
+            raise InvalidMetadataException()
 
-            # reproject if needed
-            source_target_srid = None
-            if (
-                self.current.source_srid
-                and self.current.target_srid != self.current.source_srid
-            ):
-                source_target_srid = (
-                    self.current.source_srid,
-                    self.current.target_srid,
-                )
-                vertices = reproject_vertex_list(vertices, *source_target_srid)
+        # add metadata to the database
+        import_meta.__table__.schema = self.args.db_schema
+        self.current.import_meta = import_meta
+        self.session.add(import_meta)
+        self.session.commit()
 
-            # list of relationships for the CityJSONFeature
-            family_ties = []
-            # objects for the CityJSONFeature
-            cj_feature_objects = {}
-
-            # create CityJSONObjects
-            for obj_id, cityobj in line_json["CityObjects"].items():
-                obj_to_update = None
-
-                # optionally check if the object exists - 
-                # to skip it or update it
-                if self.args.update_existing:
-                    existing = (
-                        self.session.query(CjObjectModel)
-                        .filter_by(object_id=obj_id)
-                        .first()
-                    )
+    def process_line(self, line_json) -> None:
+        # unpack vertices for the cityobjects based on
+        # the CityJSON transform
+        # this is done once for the CityJSONFeature
+        vertices = [
+            transform_vertex(v, self.current.import_meta.transform)
+            for v in line_json["vertices"]
+        ]
+
+        # reproject if needed
+        source_target_srid = None
+        if (
+            self.current.source_srid
+            and self.current.target_srid != self.current.source_srid
+        ):
+            source_target_srid = (
+                self.current.source_srid,
+                self.current.target_srid,
+            )
+            vertices = reproject_vertex_list(vertices, *source_target_srid)
 
-                    if existing:
-                        # TODO: proper logging
-                        print(f"CityObject (id:{obj_id}) already exists. Updating.") # noqa
-                        obj_to_update = existing
-
-                # get 3D geom, ground geom and bbox
-                geometry, ground_geometry = self.get_geometries(
-                    obj_id, cityobj, vertices, source_target_srid
+        # list of relationships for the CityJSONFeature
+        family_ties = []
+        # objects for the CityJSONFeature
+        cj_feature_objects = {}
+
+        # create CityJSONObjects
+        for obj_id, cityobj in line_json["CityObjects"].items():
+            obj_to_update = None
+
+            # optionally check if the object exists -
+            # to skip it or update it
+            if self.args.update_existing:
+                existing = (
+                    self.session.query(CjObjectModel)
+                    .filter_by(object_id=obj_id)
+                    .first()
                 )
 
-                # check if the object type is allowed by the official
-                # spec or extension
-                check_result, message = check_object_type(
-                    cityobj.get("type"),
-                    self.cj_object_types,
-                    self.current.extension_handler.extra_city_objects,
+                if existing:
+                    logger.warning(f"CityObject (id:{obj_id}) already exists. Updating.")  # noqa
+                    obj_to_update = existing
+
+            # get 3D geom, ground geom and bbox
+            geometry, ground_geometry = self.get_geometries(
+                obj_id, cityobj, vertices, source_target_srid
+            )
+
+            # check if the object type is allowed by the official
+            # spec or extension
+            check_result, message = check_object_type(
+                cityobj.get("type"),
+                self.cj_object_types,
+                self.current.extension_handler.extra_city_objects,
+            )
+            if not check_result:
+                logger.info(message)
+
+            # update or insert the object
+            # 'or None' is added to change empty json "{}" to database null
+            if obj_to_update:
+                cj_object = obj_to_update
+                cj_object.type = cityobj.get("type")
+                cj_object.attributes = cityobj.get("attributes") or None
+                cj_object.geometry = geometry
+                cj_object.ground_geometry = ground_geometry
+                cj_object.import_meta = self.current.import_meta
+            else:
+                cj_object = CjObjectModel(
+                    object_id=obj_id,
+                    type=cityobj.get("type"),
+                    attributes=cityobj.get("attributes") or None,
+                    geometry=geometry,
+                    ground_geometry=ground_geometry,
                 )
-                if not check_result:
-                    print(message)
 
-                # update or insert the object
-                # 'or None' is added to change empty json "{}" to database null
+                # add CityJson object to the database
+                cj_object.__table__.schema = self.args.db_schema
+                cj_object.import_meta_id = self.current.import_meta.id
+                self.current.cj_objects.append(to_dict(cj_object))
+
+            cj_feature_objects[obj_id] = cj_object
+
+            # save children-parent links
+            for child_id in cityobj.get("children", []):
+                family_ties.append((obj_id, child_id))
+
+                # delete previous ties if updating object
                 if obj_to_update:
-                    cj_object = obj_to_update
-                    cj_object.type = cityobj.get("type")
-                    cj_object.attributes = cityobj.get("attributes") or None
-                    cj_object.geometry = geometry
-                    cj_object.ground_geometry = ground_geometry
-                    cj_object.import_meta = self.current.import_meta
-                else:
-                    cj_object = CjObjectModel(
-                        object_id=obj_id,
-                        type=cityobj.get("type"),
-                        attributes=cityobj.get("attributes") or None,
-                        geometry=geometry,
-                        ground_geometry=ground_geometry,
+                    children = self.session.query(FamilyModel).filter_by(
+                        child_id=child_id
                     )
+                    children.delete()
 
-                    # add CityJson object to the database
-                    cj_object.__table__.schema = self.args.db_schema
-                    cj_object.import_meta_id = self.current.import_meta.id
-                    self.current.cj_objects.append(to_dict(cj_object))
-
-                cj_feature_objects[obj_id] = cj_object
-
-                # save children-parent links
-                for child_id in cityobj.get("children", []):
-                    family_ties.append((obj_id, child_id))
-
-                    # delete previous ties if updating object
-                    if obj_to_update:
-                        children = self.session.query(FamilyModel).filter_by(
-                            child_id=child_id
-                        )
-                        children.delete()
-
-            # create children-parent links after all objects
-            # from the CityJSONFeature already exist
-            for parent_id, child_id in family_ties:
-                self.current.families.append(
-                    {"parent_id": parent_id, "child_id": child_id}
-                )
+        # create children-parent links after all objects
+        # from the CityJSONFeature already exist
+        for parent_id, child_id in family_ties:
+            self.current.families.append({"parent_id": parent_id,
+                                          "child_id": child_id})
 
-    def process_file(self, filepath):
+    def process_file(self, filepath) -> None:
+        """Process a single cityJSON file"""
         self.current = SingleFileImport(filepath)
-        print("Running import for file: ", filepath)
+        logger.info("Running import for file: %s", filepath)
 
         if filepath.lower() == "stdin":
-            for line in sys.stdin:
-                self.process_line(line.rstrip("\n"))
+            f = sys.stdin
         else:
-            with open(filepath) as f:
-                for line in f.readlines():
-                    self.process_line(line)
+            f = open(filepath, "rt")
+
+        first_line = f.readline()
+        first_line_json = json.loads(first_line.rstrip("\n"))
+        if not is_cityjson_object(first_line_json):
+            raise InvalidCityJSONObjectException()
+        self.extract_import_metadata(first_line_json)
+        for line in f.readlines():
+            line_json = json.loads(line.rstrip("\n"))
+            self.process_line(line_json)
 
         if self.current.cj_objects:
             obj_insert = (
                 insert(CjObjectModel)
                 .values(self.current.cj_objects)
                 .on_conflict_do_nothing()
-            )  # noqa
+            )
             self.session.execute(obj_insert)
 
         if self.current.families:
             family_insert = (
                 insert(FamilyModel)
                 .values(self.current.families)
                 .on_conflict_do_nothing()
             )  # noqa
             self.session.execute(family_insert)
         self.current.import_meta.finished_at = func.now()
         self.session.commit()
 
-    def process_directory(self, dir_path):
-        print("Running import for directory: ", dir_path)
+    def process_directory(self, dir_path) -> None:
+        """Process all files in a directory."""
+        logger.info("Running import for directory: %s", dir_path)
         ext = ".jsonl"
         for f in os.scandir(dir_path):
             if f.path.endswith(ext):
                 self.process_file(f.path)
 
     def index_attributes(self):
         # postgres types to be used in type casted index
@@ -367,51 +369,55 @@
         cmd_base = (
             "create index if not exists {table}_{attr_name}_idx "
             + "on {schema}.{table} using "
             + "btree(((attributes->>'{attr_name}')::{attr_type}))"
         )
 
         # prepare partial and non partial indexes in one list
-        attributes = [(a, True) for a in self.args.partial_indexed_attributes] + [ #noqa
+        attributes = [
+            (a, True) for a in self.args.partial_indexed_attributes
+        ] + [  # noqa
             (a, False) for a in self.args.indexed_attributes
         ]
 
         # for each attribute to be indexed
         for attr_name, is_partial in attributes:
             msg = f"Indexing CityObject attribute: '{attr_name}'"
             if is_partial:
                 msg += " with partial index"
-            print(msg)
+            logger.info(msg)
 
             # get proper postgres type
             if attr_name in type_mapping:
                 postgres_type = postgres_type_mapping[type_mapping[attr_name]]
 
                 # prepare and run sql command
                 if is_partial:
                     cmd = cmd_base
-                    + " WHERE attributes->>'{attr_name}' IS NOT NULL"
+                    +" WHERE attributes->>'{attr_name}' IS NOT NULL"
                 else:
                     cmd = cmd_base
 
                 cmd = cmd.format(
                     table=CjObjectModel.__table__.name,
                     schema=CjObjectModel.__table__.schema,
                     attr_name=attr_name,
                     attr_type=postgres_type,
                 )
                 with self.engine.connect() as conn:
                     conn.execute(text(cmd))
 
             else:
-                print(
-                    f"Specified attribute to be indexed: '{attr_name}' does not exist" # noqa
+                logger.warning(
+                    f"Specified attribute to be indexed: '{attr_name}' does not exist"  # noqa
                 )
 
-    def get_geometries(self, obj_id, cityobj, vertices, source_target_srid):
+    def get_geometries(
+        self, obj_id, cityobj, vertices, source_target_srid
+    ) -> Tuple[Optional[BaseGeometry], Optional[BaseGeometry]]:
         if "geometry" not in cityobj:
             return None, None
 
         # returned geometry is already in the required projection
         geometry = resolve_geometry_vertices(
             cityobj["geometry"],
             vertices,
```

### Comparing `cjdb-1.1.0/cjdb/modules/utils.py` & `cjdb-1.2.0/cjdb/modules/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-import os
-from pathlib import Path
+from typing import Any, Dict
 
 import psycopg2
 from psycopg2.extras import RealDictCursor
 from sqlalchemy import create_engine
 
 from cjdb.resources import object_types
 
 
 def get_db_engine(args, echo=False):
-    conn_string = f"postgresql://{args.db_user}:{args.db_password}"\
+    conn_string = (
+        f"postgresql://{args.db_user}:{args.db_password}"
         f"@{args.db_host}:{args.db_port}/{args.db_name}"
+    )
 
     engine = create_engine(conn_string, echo=echo)
 
     return engine
 
 
 def open_connection(args):
-    conn = psycopg2.connect(database=args.db_name,
-                            host=args.db_host,
-                            user=args.db_user,
-                            port=args.db_port,
-                            cursor_factory=RealDictCursor)
-    
+    conn = psycopg2.connect(
+        database=args.db_name,
+        host=args.db_host,
+        user=args.db_user,
+        port=args.db_port,
+        cursor_factory=RealDictCursor,
+    )
+
     return conn
 
 
 # todo - this should take available object types from the official spec
 def get_cj_object_types():
     types = object_types.types
 
@@ -37,21 +40,34 @@
         if val:
             for v in val:
                 type_list.append(v)
 
     return sorted(type_list)
 
 
+def is_cityjson_object(json: Dict[str, Any]) -> bool:
+    """Check if the json is a cityjson object"""
+    if (
+        "version" in json
+        and "transform" in json
+        and "type" in json
+        and json["type"] == "CityJSON"
+    ):
+        return True
+    return False
+
+
 # find extended properties
 def find_extra_properties(json_obj):
     property_names = []
     for key in json_obj:
         if key.startswith("+"):
             property_names.append(key)
 
     return property_names
 
+
 # Sqlalchemy model as dict
 def to_dict(model):
     d = dict(model.__dict__)
-    d.pop('_sa_instance_state', None)
-    return d
+    d.pop("_sa_instance_state", None)
+    return d
```

### Comparing `cjdb-1.1.0/cjdb/resources/strings.py` & `cjdb-1.2.0/cjdb/resources/strings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,68 @@
-filepath_help = "Source CityJSONL file or a directory with CityJSONL files. " \
-    + "STDIN if not specified. " \
-    + "If specifying a directory, all the *.jsonl files inside of it will be imported."
+filepath_help = (
+    "Source a CityJSONL file or a directory with CityJSONL files. "
+    "If a path is not specified, STDIN will be used."
+)
+
+version_help = "Get the current version"
 
 host_help = "PostgreSQL database host"
 
 port_help = "PostgreSQL database port"
 
 user_help = "PostgreSQL database user name"
 
 password_help = "PostgreSQL database user password"
 
 database_help = "PostgreSQL database name"
 
 schema_help = "Target database schema"
 
-srid_help = "Target coordinate system SRID. " +\
+srid_help = (
+    "Target coordinate system SRID. "
     "All 3D and 2D geometries will be reprojected."
+)
 
-index_help = "CityObject attribute to be indexed using a btree index. " +\
+index_help = (
+    "CityObject attribute to be indexed using a btree index. "
     "Can be specified multiple times, for each attribute once."
+)
 
-partial_index_help = "CityObject attribute to be indexed using a btree partial index. " +\
-    "Can be specified multiple times, for each attribute once. " + \
-    "This index indexes on a condition 'where {{ATTR_NAME}} is not null'. " + \
-    "This means that it saves space and improves query performance when the attribute " +\
-    "is not present for all imported CityObjects."
-
-append_help = "Run in append mode (as opposed to default create mode). " +\
-            "This assumes the database structure exists already and new data is to be appended."
-
-overwrite_help = "Overwrite the data that is currently in the database schema. " + \
-                "Warning: this causes the loss of what was imported before to the database schema."
-
-ignore_file_help = "Ignore repeated file names warning when importing. " +\
-    "By default, the importer will send out warnings if a specific file has already been imported."
-
-skip_existing = "Check if the object with given ID exists before inserting, and skip it if it does. " +\
-    "By default, the importer does not check existence for performance reasons, " +\
-    "which means that importing the same object twice will result in an error."
-
-update_existing = "Check if the object with given ID exists before inserting, and update it if it does. " +\
+partial_index_help = (
+    "CityObject attribute to be indexed using a btree partial index. "
+    "Can be specified multiple times, for each attribute once. "
+    "This index indexes on a condition 'where {{ATTR_NAME}} is not null'. "
+    "This means that it saves space and improves query performance when the "
+    "attribute is not present for all imported CityObjects."
+)
+
+append_help = (
+    "Run in append mode (as opposed to default create mode). "
+    "This assumes the database structure exists already and "
+    "new data is to be appended."
+)
+
+overwrite_help = (
+    "Overwrite the data that is currently in the database schema. "
+    "Warning: this causes the loss of what was imported before "
+    "to the database schema."
+)
+
+ignore_file_help = (
+    "Ignore repeated file names warning when importing. "
+    "By default, the importer will send out warnings if a specific "
+    "file has already been imported."
+)
+
+skip_existing = (
+    "Check if the object with given ID exists before inserting, and "
+    "skip it if it does. "
+    "By default, the importer does not check existence for "
+    "performance reasons, which means that importing the same object "
+    "twice will result in an error."
+)
+
+update_existing = (
+    "Check if the object with given ID exists before inserting, and "
+    "update it if it does. "
     "The old object will be updated with the new object's properties."
+)
```

### Comparing `cjdb-1.1.0/pyproject.toml` & `cjdb-1.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cjdb"
-version = "1.1.0"
+version = "1.2.0"
 description = "CJDB is a tool that enables CityJSON integration with a PostgreSQL database"
 authors = ["Cynthia Cai", "Lan Yan", "Yitong Xia", "Chris Poon", "Siebren Meines", "Leon Powalka"]
 maintainers = ["Gina Stavropoulou <g.stavropoulou@tudelft.nl>"]
 license = "MIT"
 repository = "https://github.com/tudelft3d/cjdb"
 readme = "README.md"
 keywords = ["CityJSON", "PostgreSQL"]
@@ -16,18 +16,21 @@
 python = "^3.11"
 shapely = "^2.0.1"
 numpy = "^1.24.2"
 pyproj = "^3.5.0"
 requests = "^2.28.2"
 psycopg2-binary = "^2.9.6"
 geoalchemy2 = "^0.13.1"
+cjio = "^0.8.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.1.1"
 isort = "^5.12.0"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 pytest = "^7.2.2"
+pytest-postgresql = "^4.1.1"
+psycopg = "^3.1.8"
 
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
```

