# Comparing `tmp/csvcubed-0.3.6-py3-none-any.whl.zip` & `tmp/csvcubed-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,25 @@
-Zip file size: 212061 bytes, number of entries: 180
+Zip file size: 216823 bytes, number of entries: 184
 -rw-r--r--  2.0 unx     1515 b- defN 80-Jan-01 00:00 csvcubed/README.md
 -rw-r--r--  2.0 unx      218 b- defN 80-Jan-01 00:00 csvcubed/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/__init__.py
--rw-r--r--  2.0 unx     2876 b- defN 80-Jan-01 00:00 csvcubed/cli/build.py
--rw-r--r--  2.0 unx     1414 b- defN 80-Jan-01 00:00 csvcubed/cli/build_code_list.py
--rw-r--r--  2.0 unx     4800 b- defN 80-Jan-01 00:00 csvcubed/cli/entrypoint.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/buildcsvw/__init__.py
+-rw-r--r--  2.0 unx     2881 b- defN 80-Jan-01 00:00 csvcubed/cli/buildcsvw/build.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/codelist/__init__.py
+-rw-r--r--  2.0 unx     1414 b- defN 80-Jan-01 00:00 csvcubed/cli/codelist/build_code_list.py
+-rw-r--r--  2.0 unx     5742 b- defN 80-Jan-01 00:00 csvcubed/cli/entrypoint.py
 -rw-r--r--  2.0 unx     9572 b- defN 80-Jan-01 00:00 csvcubed/cli/error_mapping.py
--rw-r--r--  2.0 unx      238 b- defN 80-Jan-01 00:00 csvcubed/cli/inspect/README.md
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/inspect/__init__.py
--rw-r--r--  2.0 unx     4292 b- defN 80-Jan-01 00:00 csvcubed/cli/inspect/inspect.py
--rw-r--r--  2.0 unx     3342 b- defN 80-Jan-01 00:00 csvcubed/cli/inspect/inspectdatasetmanager.py
--rw-r--r--  2.0 unx     1517 b- defN 80-Jan-01 00:00 csvcubed/cli/inspect/metadatainputvalidator.py
--rw-r--r--  2.0 unx    13702 b- defN 80-Jan-01 00:00 csvcubed/cli/inspect/metadataprinter.py
+-rw-r--r--  2.0 unx      238 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/README.md
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/__init__.py
+-rw-r--r--  2.0 unx     4300 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/inspect.py
+-rw-r--r--  2.0 unx     3333 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/inspectdatasetmanager.py
+-rw-r--r--  2.0 unx     1517 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/metadatainputvalidator.py
+-rw-r--r--  2.0 unx    13706 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/metadataprinter.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/pullcsvw/__init__.py
+-rw-r--r--  2.0 unx    13791 b- defN 80-Jan-01 00:00 csvcubed/cli/pullcsvw/pull.py
 -rw-r--r--  2.0 unx      840 b- defN 80-Jan-01 00:00 csvcubed/definitions.py
 -rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 csvcubed/inputs.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/models/codelistconfig/__init__.py
 -rw-r--r--  2.0 unx     8467 b- defN 80-Jan-01 00:00 csvcubed/models/codelistconfig/code_list_config.py
 -rw-r--r--  2.0 unx    14542 b- defN 80-Jan-01 00:00 csvcubed/models/csvcubedexception.py
 -rw-r--r--  2.0 unx      409 b- defN 80-Jan-01 00:00 csvcubed/models/csvwtype.py
@@ -66,15 +70,15 @@
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/readers/catalogmetadata/v1/__init__.py
 -rw-r--r--  2.0 unx     1637 b- defN 80-Jan-01 00:00 csvcubed/readers/catalogmetadata/v1/catalog_metadata_reader.py
 -rw-r--r--  2.0 unx     6719 b- defN 80-Jan-01 00:00 csvcubed/readers/codelistconfig/codelist_schema_versions.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/__init__.py
 -rw-r--r--  2.0 unx     4878 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/schema_versions.py
 -rw-r--r--  2.0 unx     1814 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/__init__.py
--rw-r--r--  2.0 unx    20171 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/columnschema.py
+-rw-r--r--  2.0 unx    20180 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/columnschema.py
 -rw-r--r--  2.0 unx    14157 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/configdeserialiser.py
 -rw-r--r--  2.0 unx      629 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/constants.py
 -rw-r--r--  2.0 unx     4071 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/datatypes.py
 -rw-r--r--  2.0 unx     9137 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/mapcolumntocomponent.py
 -rw-r--r--  2.0 unx      182 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/readme.md
 -rw-r--r--  2.0 unx      911 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/README.md
 -rw-r--r--  2.0 unx      210 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/calendar-day.json
@@ -151,15 +155,15 @@
 -rw-r--r--  2.0 unx     1339 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_dsd_qube_components.sparql
 -rw-r--r--  2.0 unx      757 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_is_pivoted_shape_for_measures_in_data_set.sparql
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_labels_for_resource_uris.sparql
 -rw-r--r--  2.0 unx      379 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_metadata_dependencies.sparql
 -rw-r--r--  2.0 unx      466 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_table_schema_properties.sparql
 -rw-r--r--  2.0 unx      367 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_units.sparql
 -rw-r--r--  2.0 unx    11626 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparqlquerymanager.py
--rw-r--r--  2.0 unx     8831 b- defN 80-Jan-01 00:00 csvcubed/utils/tableschema.py
+-rw-r--r--  2.0 unx     9198 b- defN 80-Jan-01 00:00 csvcubed/utils/tableschema.py
 -rw-r--r--  2.0 unx      356 b- defN 80-Jan-01 00:00 csvcubed/utils/text.py
 -rw-r--r--  2.0 unx     3467 b- defN 80-Jan-01 00:00 csvcubed/utils/uri.py
 -rw-r--r--  2.0 unx    11239 b- defN 80-Jan-01 00:00 csvcubed/utils/validations.py
 -rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 csvcubed/utils/validators/__init__.py
 -rw-r--r--  2.0 unx     4360 b- defN 80-Jan-01 00:00 csvcubed/utils/validators/schema.py
 -rw-r--r--  2.0 unx      268 b- defN 80-Jan-01 00:00 csvcubed/utils/version.py
 -rw-r--r--  2.0 unx       62 b- defN 80-Jan-01 00:00 csvcubed/writers/__init__.py
@@ -170,13 +174,13 @@
 -rw-r--r--  2.0 unx    27378 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/qbwriter/urihelper.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/__init__.py
 -rw-r--r--  2.0 unx      157 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/constants.py
 -rw-r--r--  2.0 unx     2437 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/newresourceurigenerator.py
 -rw-r--r--  2.0 unx    20804 b- defN 80-Jan-01 00:00 csvcubed/writers/qbwriter.py
 -rw-r--r--  2.0 unx     9470 b- defN 80-Jan-01 00:00 csvcubed/writers/skoscodelistwriter.py
 -rw-r--r--  2.0 unx      283 b- defN 80-Jan-01 00:00 csvcubed/writers/writerbase.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 csvcubed-0.3.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     3925 b- defN 80-Jan-01 00:00 csvcubed-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 csvcubed-0.3.6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    18103 b- defN 16-Jan-01 00:00 csvcubed-0.3.6.dist-info/RECORD
-180 files, 766608 bytes uncompressed, 182367 bytes compressed:  76.2%
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 csvcubed-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3925 b- defN 80-Jan-01 00:00 csvcubed-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 csvcubed-0.4.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    18495 b- defN 16-Jan-01 00:00 csvcubed-0.4.0.dist-info/RECORD
+184 files, 782117 bytes uncompressed, 186481 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -3,42 +3,54 @@
 
 Filename: csvcubed/__init__.py
 Comment: 
 
 Filename: csvcubed/cli/__init__.py
 Comment: 
 
-Filename: csvcubed/cli/build.py
+Filename: csvcubed/cli/buildcsvw/__init__.py
 Comment: 
 
-Filename: csvcubed/cli/build_code_list.py
+Filename: csvcubed/cli/buildcsvw/build.py
+Comment: 
+
+Filename: csvcubed/cli/codelist/__init__.py
+Comment: 
+
+Filename: csvcubed/cli/codelist/build_code_list.py
 Comment: 
 
 Filename: csvcubed/cli/entrypoint.py
 Comment: 
 
 Filename: csvcubed/cli/error_mapping.py
 Comment: 
 
-Filename: csvcubed/cli/inspect/README.md
+Filename: csvcubed/cli/inspectcsvw/README.md
+Comment: 
+
+Filename: csvcubed/cli/inspectcsvw/__init__.py
+Comment: 
+
+Filename: csvcubed/cli/inspectcsvw/inspect.py
 Comment: 
 
-Filename: csvcubed/cli/inspect/__init__.py
+Filename: csvcubed/cli/inspectcsvw/inspectdatasetmanager.py
 Comment: 
 
-Filename: csvcubed/cli/inspect/inspect.py
+Filename: csvcubed/cli/inspectcsvw/metadatainputvalidator.py
 Comment: 
 
-Filename: csvcubed/cli/inspect/inspectdatasetmanager.py
+Filename: csvcubed/cli/inspectcsvw/metadataprinter.py
 Comment: 
 
-Filename: csvcubed/cli/inspect/metadatainputvalidator.py
+Filename: csvcubed/cli/pullcsvw/__init__.py
 Comment: 
 
-Filename: csvcubed/cli/inspect/metadataprinter.py
+Filename: csvcubed/cli/pullcsvw/pull.py
 Comment: 
 
 Filename: csvcubed/definitions.py
 Comment: 
 
 Filename: csvcubed/inputs.py
 Comment: 
@@ -519,23 +531,23 @@
 
 Filename: csvcubed/writers/skoscodelistwriter.py
 Comment: 
 
 Filename: csvcubed/writers/writerbase.py
 Comment: 
 
-Filename: csvcubed-0.3.6.dist-info/LICENSE
+Filename: csvcubed-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: csvcubed-0.3.6.dist-info/METADATA
+Filename: csvcubed-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: csvcubed-0.3.6.dist-info/WHEEL
+Filename: csvcubed-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: csvcubed-0.3.6.dist-info/entry_points.txt
+Filename: csvcubed-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: csvcubed-0.3.6.dist-info/RECORD
+Filename: csvcubed-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## csvcubed/cli/entrypoint.py

```diff
@@ -6,17 +6,18 @@
 import logging
 import sys
 from pathlib import Path
 
 import click
 
 from csvcubed import __version__
-from csvcubed.cli.build import build
-from csvcubed.cli.build_code_list import build_code_list
-from csvcubed.cli.inspect.inspect import inspect
+from csvcubed.cli.buildcsvw.build import build_csvw
+from csvcubed.cli.codelist.build_code_list import build_code_list
+from csvcubed.cli.inspectcsvw.inspect import inspect
+from csvcubed.cli.pullcsvw.pull import pull
 from csvcubed.models.errorurl import HasErrorUrl
 from csvcubed.utils.log import log_exception, start_logging
 
 _logger = logging.getLogger(__name__)
 
 _VALIDATION_FILE_NAME = "validation-errors.json"
 
@@ -93,17 +94,17 @@
 ):
     """Build a qb-flavoured CSV-W from a tidy CSV."""
     validation_errors_file_name = (
         _VALIDATION_FILE_NAME if validation_errors_to_file else None
     )
     out.mkdir(parents=True, exist_ok=True)
 
-    start_logging(log_dir_name="csvcubed-cli", selected_logging_level=log_level)
+    _init_logging(log_level)
     try:
-        build(
+        build_csvw(
             config_path=config,
             output_directory=out,
             csv_path=csv,
             fail_when_validation_error_occurs=fail_when_validation_error,
             validation_errors_file_name=validation_errors_file_name,
         )
 
@@ -117,26 +118,29 @@
 @click.argument(
     "csvw_metadata_json_path",
     type=click.Path(exists=True, path_type=Path),
     metavar="CSVW_METADATA_JSON_PATH",
 )
 def inspect_command(log_level: str, csvw_metadata_json_path: Path) -> None:
     """Inspect the contents of a CSV-W generated by csvcubed."""
-    start_logging(log_dir_name="csvcubed-cli", selected_logging_level=log_level)
+    _init_logging(log_level)
     try:
         inspect(csvw_metadata_json_path)
     except Exception as e:
         log_exception(_logger, e)
         if isinstance(e, HasErrorUrl):
             _logger.error(f"More information available at {e.get_error_url()}")
         sys.exit(1)
 
 
-@entry_point.group("code-list", help="Create a SKOS code list from a JSON file")
+@entry_point.group("code-list")
 def code_list():
+    """
+    Create a code list from a JSON file.
+    """
     ...
 
 
 @code_list.command("build")
 @out_option
 @fail_option
 @validation_option
@@ -155,19 +159,53 @@
 ):
     """Build a skos-flavoured code list CSV-W from a tidy code list JSON file."""
     validation_errors_file_name = (
         _VALIDATION_FILE_NAME if validation_errors_to_file else None
     )
 
     out.mkdir(parents=True, exist_ok=True)
-    start_logging(log_dir_name="csvcubed-cli", selected_logging_level=log_level)
+    _init_logging(log_level)
     try:
         build_code_list(
             config_path=config,
             output_directory=out,
             fail_when_validation_error_occurs=fail_when_validation_error,
             validation_errors_file_name=validation_errors_file_name,
         )
 
     except Exception as e:
         log_exception(_logger, e)
         sys.exit(1)
+
+
+@entry_point.command("pull")
+@log_option
+# N.B. The `out` directory for the `pull` command is different and defaults to the current working directory.
+@click.option(
+    "--out",
+    "-o",
+    help="Location of the CSV-W and dependencies.",
+    default=Path(".").absolute(),
+    show_default=True,
+    type=click.Path(path_type=Path, file_okay=False, dir_okay=True),
+    metavar="OUT_DIR",
+)
+@click.argument(
+    "csvw_metadata_json_url",
+    type=click.STRING,
+    metavar="CSVW_METADATA_JSON_URL",
+)
+def csvw_pull(csvw_metadata_json_url: str, out: Path, log_level: str) -> None:
+    """
+    Pull a CSV-W and all relatively defined dependent files.
+    """
+    _init_logging(log_level)
+    try:
+        pull(csvw_metadata_url=csvw_metadata_json_url, output_dir=out)
+        print(f"Pull Complete @ {out.resolve()}")
+    except Exception as e:
+        log_exception(_logger, e)
+        sys.exit(1)
+
+
+def _init_logging(log_level):
+    start_logging(log_dir_name="csvcubed-cli", selected_logging_level=log_level)
```

## csvcubed/readers/cubeconfig/v1/columnschema.py

```diff
@@ -12,15 +12,15 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional, Tuple, TypeVar, Union
 
 import uritemplate
 from csvcubedmodels.dataclassbase import DataClassBase
 
-from csvcubed.cli.build_code_list import get_code_list_versioned_deserialiser
+from csvcubed.cli.codelist.build_code_list import get_code_list_versioned_deserialiser
 from csvcubed.inputs import PandasDataTypes, pandas_input_to_columnar_optional_str
 from csvcubed.models.cube.cube import CatalogMetadata
 from csvcubed.models.cube.qb.components.attribute import (
     ExistingQbAttribute,
     ExistingQbAttributeLiteral,
     NewQbAttribute,
     NewQbAttributeLiteral,
```

## csvcubed/utils/tableschema.py

```diff
@@ -173,16 +173,27 @@
         path_to_file_uri_for_rdflib(paths_relative_to)
         if isinstance(paths_relative_to, Path)
         else paths_relative_to
     )
 
     if follow_relative_path_dependencies_only and any(dependencies_to_load):
         _logger.debug("Dropping non-relative dependencies.")
+        absolute_dependency_urls = {
+            d.data_dump for d in dependencies_to_load if looks_like_uri(d.data_dump)
+        }
+        for dep in absolute_dependency_urls:
+            _logger.warning(
+                "Not following RDF dependency '%s' since it is an absolute dependency.",
+                dep,
+            )
+
         dependencies_to_load = [
-            d for d in dependencies_to_load if not looks_like_uri(d.data_dump)
+            d
+            for d in dependencies_to_load
+            if d.data_dump not in absolute_dependency_urls
         ]
 
     if not any(dependencies_to_load):
         _logger.debug("Did not find any RDF dependencies to load.")
 
     for dependency in dependencies_to_load:
         if not looks_like_uri(dependency.data_dump):
```

## Comparing `csvcubed/cli/build.py` & `csvcubed/cli/buildcsvw/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from csvcubed.utils.cli import log_validation_and_json_schema_errors
 from csvcubed.utils.qb.validation.cube import validate_qb_component_constraints
 from csvcubed.writers.qbwriter import QbWriter
 
 _logger = logging.getLogger(__name__)
 
 
-def build(
+def build_csvw(
     csv_path: Path,
     config_path: Optional[Path] = None,
     output_directory: Path = Path(".", "out").resolve(),
     fail_when_validation_error_occurs: bool = False,
     validation_errors_file_name: Optional[str] = None,
 ) -> Tuple[QbCube, List[ValidationError]]:
     cube, json_schema_validation_errors, validation_errors = _extract_and_validate_cube(
```

## Comparing `csvcubed/cli/build_code_list.py` & `csvcubed/cli/codelist/build_code_list.py`

 * *Files identical despite different names*

## Comparing `csvcubed/cli/inspect/inspect.py` & `csvcubed/cli/inspectcsvw/inspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 """
 
 import logging
 from os import linesep
 from pathlib import Path
 from typing import Tuple
 
-from csvcubed.cli.inspect.metadatainputvalidator import MetadataValidator
-from csvcubed.cli.inspect.metadataprinter import MetadataPrinter
+from csvcubed.cli.inspectcsvw.metadatainputvalidator import MetadataValidator
+from csvcubed.cli.inspectcsvw.metadataprinter import MetadataPrinter
 from csvcubed.models.csvcubedexception import FailedToLoadRDFGraphException
 from csvcubed.models.csvwtype import CSVWType
 from csvcubed.utils.sparql_handler.code_list_inspector import CodeListInspector
 from csvcubed.utils.sparql_handler.csvw_inspector import CsvWInspector
 from csvcubed.utils.sparql_handler.data_cube_inspector import DataCubeInspector
 from csvcubed.utils.tableschema import CsvWRdfManager
```

## Comparing `csvcubed/cli/inspect/inspectdatasetmanager.py` & `csvcubed/cli/inspectcsvw/inspectdatasetmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 import logging
 from pathlib import Path
 from typing import Optional
 
 import pandas as pd
 
 from csvcubed.cli.error_mapping import friendly_error_mapping
-from csvcubed.models.csvcubedexception import (
-    CsvToDataFrameLoadFailedException,
-)
+from csvcubed.models.csvcubedexception import CsvToDataFrameLoadFailedException
 from csvcubed.models.csvwtype import CSVWType
 from csvcubed.models.cube.cube_shape import CubeShape
 from csvcubed.models.inspectdataframeresults import (
     CodelistHierarchyInfoResult,
     DatasetObservationsByMeasureUnitInfoResult,
     DatasetObservationsInfoResult,
 )
```

## Comparing `csvcubed/cli/inspect/metadatainputvalidator.py` & `csvcubed/cli/inspectcsvw/metadatainputvalidator.py`

 * *Files identical despite different names*

## Comparing `csvcubed/cli/inspect/metadataprinter.py` & `csvcubed/cli/inspectcsvw/metadataprinter.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from os import linesep
 from pathlib import Path
 from textwrap import indent
 from typing import Dict, List, Optional, Tuple, Union
 
 from pandas import DataFrame
 
-from csvcubed.cli.inspect.inspectdatasetmanager import (
+from csvcubed.cli.inspectcsvw.inspectdatasetmanager import (
     get_concepts_hierarchy_info,
     get_dataset_observations_info,
     get_dataset_val_counts_info,
     load_csv_to_dataframe,
 )
 from csvcubed.models.csvcubedexception import (
     InputNotSupportedException,
```

## Comparing `csvcubed-0.3.6.dist-info/LICENSE` & `csvcubed-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `csvcubed-0.3.6.dist-info/METADATA` & `csvcubed-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvcubed
-Version: 0.3.6
+Version: 0.4.0
 Summary: A tool to generate RDF Data Cube style CSV-W cubes from tidy CSV files. Part of the csvcubed family.
 License: Apache-2.0
 Author: Integrated Data Service - Dissemination
 Author-email: csvcubed@gsscogs.uk
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `csvcubed-0.3.6.dist-info/RECORD` & `csvcubed-0.4.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 csvcubed/README.md,sha256=cMpCUdrf8r5IV0AWyYZar5RkZRKXNTXNcUiVb3G-WYY,1515
 csvcubed/__init__.py,sha256=8pEisVqkkwt_521bRO5PIZfJrE2PKrlJL-l9NsoXMiI,218
 csvcubed/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-csvcubed/cli/build.py,sha256=cltzYlsoOhGLRMQ_-slmV-Du0bM8_5qzetIastiRFKU,2876
-csvcubed/cli/build_code_list.py,sha256=5blizIwZKfzhD8Dx_PSsEgfW6EskDqRq0ikSfPfxBjY,1414
-csvcubed/cli/entrypoint.py,sha256=4xmfeq79a_OId46lZwCvVqXhLVlPxqrGkYxEfB4Arsc,4800
+csvcubed/cli/buildcsvw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+csvcubed/cli/buildcsvw/build.py,sha256=HXHaCD4ZQXhbeWzg-xVfxD68_RkuxKFYJNZNRZ0iilM,2881
+csvcubed/cli/codelist/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+csvcubed/cli/codelist/build_code_list.py,sha256=5blizIwZKfzhD8Dx_PSsEgfW6EskDqRq0ikSfPfxBjY,1414
+csvcubed/cli/entrypoint.py,sha256=fyjDEiXA9LV5s1Z_CTyj2tghJRDm1yhcbPnvYujYg7Y,5742
 csvcubed/cli/error_mapping.py,sha256=1XpOAMOnZN5v44z5csHlhWNDlrBGF6ckDkmpajkUYqw,9572
-csvcubed/cli/inspect/README.md,sha256=1zx59skhdF11RyYiJUsV28pF6Xfhb85u1xDQbe1841o,238
-csvcubed/cli/inspect/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-csvcubed/cli/inspect/inspect.py,sha256=2kyWyha62PHyl_EUCIHA4I7n24bPq07FeUuVWEyIugw,4292
-csvcubed/cli/inspect/inspectdatasetmanager.py,sha256=VSx8tH_BQrUahG-LxLJJwzjWtuJbKl_6FpbaeRd7R60,3342
-csvcubed/cli/inspect/metadatainputvalidator.py,sha256=TUWJ4542lhdEye5XhU0paGIWi9LTjyKuU7_Vg9wSRtw,1517
-csvcubed/cli/inspect/metadataprinter.py,sha256=i9rIDyqeiTtD4ugHEkym1ifwsjthbHnLp9KQtGk-Jvk,13702
+csvcubed/cli/inspectcsvw/README.md,sha256=1zx59skhdF11RyYiJUsV28pF6Xfhb85u1xDQbe1841o,238
+csvcubed/cli/inspectcsvw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+csvcubed/cli/inspectcsvw/inspect.py,sha256=5l_jwepkIcSlHYFACEZThDzjzzcoyFFfoJIPfOfeuYI,4300
+csvcubed/cli/inspectcsvw/inspectdatasetmanager.py,sha256=48RwoGglHmCZrvaESmGRAwqkvpN4DwK7W3-XHKrzEs8,3333
+csvcubed/cli/inspectcsvw/metadatainputvalidator.py,sha256=TUWJ4542lhdEye5XhU0paGIWi9LTjyKuU7_Vg9wSRtw,1517
+csvcubed/cli/inspectcsvw/metadataprinter.py,sha256=YoJS8IOUTcIrZBNiybHSvyD-U-PwyVY2YtDHDYhgsjs,13706
+csvcubed/cli/pullcsvw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+csvcubed/cli/pullcsvw/pull.py,sha256=F2cXz6EivdwhHLgHgivXgo5EGnWPZQKxBu3uaKFwLds,13791
 csvcubed/definitions.py,sha256=l5mLOMGAdHEXfx7vIJUSxlargSWBW97IEzHvpblIUlg,840
 csvcubed/inputs.py,sha256=x2mTOfwIwz3mEjRJRwnVG-sns71Eyk_hEXGssXXe7i8,1981
 csvcubed/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/models/codelistconfig/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/models/codelistconfig/code_list_config.py,sha256=dkPPoTyazqpYPuOJ2jUzCOL1DIDu16EveiqOEstLUSQ,8467
 csvcubed/models/csvcubedexception.py,sha256=cfE3N-06CZ_bjMJV5gZ4KK6JLuFdq7Jcbe4uZiA-Krc,14542
 csvcubed/models/csvwtype.py,sha256=7WXT5EcWT48YNFn3oyPJkgPKRDPoyJZZrXHvaeWC6Jk,409
@@ -65,15 +69,15 @@
 csvcubed/readers/catalogmetadata/v1/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/readers/catalogmetadata/v1/catalog_metadata_reader.py,sha256=BqmMn8wEc5KCcAhtCkXfNr78BZe6bRvKAywQ5m_gMgY,1637
 csvcubed/readers/codelistconfig/codelist_schema_versions.py,sha256=tbCSAiFKIHPdgOQeAL2DxCnETllJZ2RYXAO0YAznVbg,6719
 csvcubed/readers/cubeconfig/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/readers/cubeconfig/schema_versions.py,sha256=DRtWlYhy6QbBJyrmfdtIVhvDuvceujjLC5-F85wG9aY,4878
 csvcubed/readers/cubeconfig/utils.py,sha256=CCq1Fu5SbGPSi02MPLsR-08tje0ByK5wc3xw5_esRGc,1814
 csvcubed/readers/cubeconfig/v1/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-csvcubed/readers/cubeconfig/v1/columnschema.py,sha256=FwscYOfjSs-uyH0XwdxvfG9Drqq_fRP_aDxiGDh3ktc,20171
+csvcubed/readers/cubeconfig/v1/columnschema.py,sha256=Jvs-dINoRDfGOffaUxGHM-VI9Rf1NwSbYJOvV9attyc,20180
 csvcubed/readers/cubeconfig/v1/configdeserialiser.py,sha256=QstbhGGcOrbSHnC8YJe4ZzUdK9rDx8xzla4mZGTedfQ,14157
 csvcubed/readers/cubeconfig/v1/constants.py,sha256=gUVnAVgrNF3HLlBn4MuEYPsIcDsD_Tjt5-GOSHyPtpE,629
 csvcubed/readers/cubeconfig/v1/datatypes.py,sha256=ORpESm5zGMUjLa78MZzxNUeSqj75DxPz5jeeoiGkeLo,4071
 csvcubed/readers/cubeconfig/v1/mapcolumntocomponent.py,sha256=Pkx0sPoNg7o4WOELVPBNkwd5y-b26Idyjjzc0VloQks,9137
 csvcubed/readers/cubeconfig/v1_0/readme.md,sha256=PlZMtxW93oA89UzwpvukvgpdB9bKoTz-EzDf4bk6I3M,182
 csvcubed/readers/cubeconfig/v1_0/templates/README.md,sha256=7o-Osoki8FBzRiU9sdTAfBlf5S1GUsbInHubMZKpaaI,911
 csvcubed/readers/cubeconfig/v1_0/templates/calendar-day.json,sha256=oXr64AxuPOMSOMYTGDTY432C8t3vCEq8mBUpFPYeoSM,210
@@ -150,15 +154,15 @@
 csvcubed/utils/sparql_handler/sparql_queries/select_dsd_qube_components.sparql,sha256=_5LF2eWp_udc09q-U2F0ZwMHIxWwliF8tkKOgYGyXNw,1339
 csvcubed/utils/sparql_handler/sparql_queries/select_is_pivoted_shape_for_measures_in_data_set.sparql,sha256=HAKnXxouSVGIue0V_1YPHCMMcFR9lTxhxS-ljP0jMLY,757
 csvcubed/utils/sparql_handler/sparql_queries/select_labels_for_resource_uris.sparql,sha256=R0e2hBvyTggTJW3iyRubeOsLomLlyoP_q_m6wi12dEM,179
 csvcubed/utils/sparql_handler/sparql_queries/select_metadata_dependencies.sparql,sha256=rmCH3---NlDNQXu1hlq-fvvMIAckNYkHZPe3tdlXdLU,379
 csvcubed/utils/sparql_handler/sparql_queries/select_table_schema_properties.sparql,sha256=2al7ZhCLHtPEVkvubzigAlmrTuT5AHup5B6WtoQxzBw,466
 csvcubed/utils/sparql_handler/sparql_queries/select_units.sparql,sha256=uuA1L0fywz9oosVyGd3WIKCILBi1KvYlZqfj519rmQE,367
 csvcubed/utils/sparql_handler/sparqlquerymanager.py,sha256=f_H6c8ryd5uh-lcyeDPhMlE5VlrxL6-UMpWRvHecNfo,11626
-csvcubed/utils/tableschema.py,sha256=erd6PZ9l3fLRTXv-L9NwnU5DmxJPO7nhivf7bOb0m_I,8831
+csvcubed/utils/tableschema.py,sha256=N6zuJU1-RWWQNNZWPLsqhhU0LK54FM8u9gztSoadbJw,9198
 csvcubed/utils/text.py,sha256=bIj2Ykra-bXaUk-EyrYCy07LrHZdY6dYXsYO8A6I_i0,356
 csvcubed/utils/uri.py,sha256=ZEX3IQG0r_xV4W_p4omhKs6x8YdXLnOGxa8vmwH_r4o,3467
 csvcubed/utils/validations.py,sha256=uWuLPturZRk6p59ya-U_zymGZBC4tM0MdGbeaGy7IE0,11239
 csvcubed/utils/validators/__init__.py,sha256=fHGeu6xOpC030v5SM2wzkvnKad8uC8_LavMJU5UxKho,45
 csvcubed/utils/validators/schema.py,sha256=txW2VLdGv1-Wo15aTgWjEiGLM3Jac1T4iU0k7eIifIc,4360
 csvcubed/utils/version.py,sha256=T-I5rVx5T08tqrTNldwwDYQVzarYtwQ_ap0g8JbgTbw,268
 csvcubed/writers/__init__.py,sha256=njopI6UIMFsqWF6i5v5huPhvRvixU-creIptscLQBUg,62
@@ -169,12 +173,12 @@
 csvcubed/writers/helpers/qbwriter/urihelper.py,sha256=BzVnUueyoE1DBncTByKnigeLozePdfFRfxzaguwCtxY,27378
 csvcubed/writers/helpers/skoscodelistwriter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/writers/helpers/skoscodelistwriter/constants.py,sha256=FjVa2JsAc7uIxzQOJgNg3zf8Ha-YZvMzF75sqq_e93g,157
 csvcubed/writers/helpers/skoscodelistwriter/newresourceurigenerator.py,sha256=DWkL2zO4QsLV8Oo-nVXxS4cxA1ic4stSBp7NZpClbps,2437
 csvcubed/writers/qbwriter.py,sha256=fDesUmhWU1211z_wDQi8xFdfpB0CqdSHG7pM-YlsJQc,20804
 csvcubed/writers/skoscodelistwriter.py,sha256=dCK3RaOrv4jeD6l4SZ2PT9tr8zqZwR2x8kbRTsASIMc,9470
 csvcubed/writers/writerbase.py,sha256=lzEHMgqdWBIFbxthYjf5JuE3i5gp5Vbb1Xw359TY3to,283
-csvcubed-0.3.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-csvcubed-0.3.6.dist-info/METADATA,sha256=k_XMVhEwfA1lVEzLxuOvEyrfXBdRqWI-mrxjcwbqIR4,3925
-csvcubed-0.3.6.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-csvcubed-0.3.6.dist-info/entry_points.txt,sha256=sGis93BsSIrPNIht5YkyuYCvefbri5nvVdOyI9ImAFs,64
-csvcubed-0.3.6.dist-info/RECORD,,
+csvcubed-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+csvcubed-0.4.0.dist-info/METADATA,sha256=pB9NW-rb3JIvC-186G8MrnLMvOmJ9trP9xt_V-yV5Xc,3925
+csvcubed-0.4.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+csvcubed-0.4.0.dist-info/entry_points.txt,sha256=sGis93BsSIrPNIht5YkyuYCvefbri5nvVdOyI9ImAFs,64
+csvcubed-0.4.0.dist-info/RECORD,,
```

