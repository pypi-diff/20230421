# Comparing `tmp/almasru-1.0.8.tar.gz` & `tmp/almasru-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almasru-1.0.8.tar", last modified: Thu Mar 30 13:50:25 2023, max compression
+gzip compressed data, was "almasru-1.1.0.tar", last modified: Fri Apr 21 05:34:08 2023, max compression
```

## Comparing `almasru-1.0.8.tar` & `almasru-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 13:50:25.545256 almasru-1.0.8/
--rw-rw-rw-   0        0        0     1107 2023-03-30 13:50:25.545256 almasru-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-03-30 13:50:00.000000 almasru-1.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-30 13:50:25.515022 almasru-1.0.8/almasru/
--rw-rw-rw-   0        0        0       69 2023-03-02 01:54:08.000000 almasru-1.0.8/almasru/__init__.py
--rw-rw-rw-   0        0        0    36919 2023-03-30 13:46:54.000000 almasru-1.0.8/almasru/client.py
--rw-rw-rw-   0        0        0      807 2023-03-01 22:29:54.000000 almasru-1.0.8/almasru/configlog.py
--rw-rw-rw-   0        0        0     7426 2023-03-02 08:53:23.000000 almasru-1.0.8/almasru/utils.py
--rw-rw-rw-   0        0        0       23 2023-03-30 13:47:10.000000 almasru-1.0.8/almasru/version.py
-drwxrwxrwx   0        0        0        0 2023-03-30 13:50:25.527860 almasru-1.0.8/almasru.egg-info/
--rw-rw-rw-   0        0        0     1107 2023-03-30 13:50:25.000000 almasru-1.0.8/almasru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-03-30 13:50:25.000000 almasru-1.0.8/almasru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 13:50:25.000000 almasru-1.0.8/almasru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-30 13:50:25.000000 almasru-1.0.8/almasru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-03-01 22:29:54.000000 almasru-1.0.8/licence.txt
--rw-rw-rw-   0        0        0      566 2023-03-30 13:50:00.000000 almasru-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-30 13:50:25.545256 almasru-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      502 2023-03-01 22:29:54.000000 almasru-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 13:50:25.544156 almasru-1.0.8/test/
--rw-rw-rw-   0        0        0        0 2023-02-19 19:45:16.000000 almasru-1.0.8/test/__init__.py
--rw-rw-rw-   0        0        0     7064 2023-03-30 09:37:58.000000 almasru-1.0.8/test/test_sruclient.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:34:08.789131 almasru-1.1.0/
+-rw-rw-rw-   0        0        0     1107 2023-04-21 05:34:08.789131 almasru-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-04-21 05:33:06.000000 almasru-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 05:34:08.752465 almasru-1.1.0/almasru/
+-rw-rw-rw-   0        0        0       69 2023-03-02 01:54:08.000000 almasru-1.1.0/almasru/__init__.py
+-rw-rw-rw-   0        0        0    37778 2023-04-21 05:23:52.000000 almasru-1.1.0/almasru/client.py
+-rw-rw-rw-   0        0        0      807 2023-03-01 22:29:54.000000 almasru-1.1.0/almasru/configlog.py
+-rw-rw-rw-   0        0        0     7643 2023-04-21 05:05:37.000000 almasru-1.1.0/almasru/utils.py
+-rw-rw-rw-   0        0        0       23 2023-04-21 05:30:42.000000 almasru-1.1.0/almasru/version.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:34:08.789131 almasru-1.1.0/almasru.egg-info/
+-rw-rw-rw-   0        0        0     1107 2023-04-21 05:34:08.000000 almasru-1.1.0/almasru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-04-21 05:34:08.000000 almasru-1.1.0/almasru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 05:34:08.000000 almasru-1.1.0/almasru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 05:34:08.000000 almasru-1.1.0/almasru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-03-01 22:29:54.000000 almasru-1.1.0/licence.txt
+-rw-rw-rw-   0        0        0      566 2023-04-21 05:33:06.000000 almasru-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 05:34:08.789131 almasru-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      502 2023-03-01 22:29:54.000000 almasru-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:34:08.789131 almasru-1.1.0/test/
+-rw-rw-rw-   0        0        0        0 2023-02-19 19:45:16.000000 almasru-1.1.0/test/__init__.py
+-rw-rw-rw-   0        0        0     7064 2023-03-30 09:37:58.000000 almasru-1.1.0/test/test_sruclient.py
```

### Comparing `almasru-1.0.8/PKG-INFO` & `almasru-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almasru
-Version: 1.0.8
+Version: 1.1.0
 Summary: This python module is a tool to use Alma SRU. it manages the logs and the backup of the records.
 Author-email: Raphaël Rey <raphael.rey@slsp.ch>
 Project-URL: Homepage, https://github.com/Swiss-Library-Service-Platform/almasru
 Project-URL: Bug Tracker, https://github.com/Swiss-Library-Service-Platform/almasru/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `almasru-1.0.8/README.rst` & `almasru-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `almasru-1.0.8/almasru/client.py` & `almasru-1.1.0/almasru/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,39 +459,42 @@
                             and len([other_sys_id for other_sys_id in record.get_035_fields()
                                      if other_sys_id.startswith('(CKB)')]) == 0    # Ignore CZ records
                             ]
 
             if len(temp_records) == 0:
                 continue
 
-            # Use sets to avoid duplicated records
-            records.update(temp_records)
+            # Use to ignore records linked with 035 that are not real children
+            temp_records_duplicates = set()
 
             for record in temp_records:
                 temp_fields = record.data.xpath(f'./m:datafield/m:subfield[contains(text(), "{sys_num}")]',
                                                 namespaces=SruClient.nsmap)
 
                 if len(temp_fields) > 0:
                     for field in temp_fields:
                         code = field.attrib['code']
                         tag = field.getparent().attrib['tag']
 
                         if tag == '035':
+                            temp_records_duplicates.add(record)
                             self.warning = True
                             self.warning_messages.append(f'More than one record with same 035, {self.mms_id} '
                                                          f'and {record.mms_id} are probably duplicated records')
-
-                        fields_related_records.append({'child_MMS_ID': record.mms_id,
-                                                       'field': f'{tag}${code}',
-                                                       'content': field.text})
+                        else:
+                            fields_related_records.append({'child_MMS_ID': record.mms_id,
+                                                           'field': f'{tag}${code}',
+                                                           'content': field.text})
                 else:
                     logging.warning(f'{repr(self)} record {repr(record)} found with SRU but no linking field')
                     fields_related_records.append({'child_MMS_ID': record.mms_id,
                                                    'field': f'UNKNOWN',
                                                    'content': sys_num})
+            # Use sets to avoid duplicated records
+            records.update(set(temp_records) - temp_records_duplicates)
 
         if len(records) == 0:
             related_record_found = False
         else:
             related_record_found = True
 
         self._child_rec_num_sys = {'MMS_ID': self.mms_id,
@@ -542,38 +545,40 @@
                             and len([other_sys_id for other_sys_id in record.get_035_fields()
                                      if other_sys_id.startswith('(CKB)')]) == 0
                             ]
 
             if len(temp_records) == 0:
                 continue
 
-            # Use sets to avoid duplicated records
-            records.update(temp_records)
+            # Use to ignore records linked with 020 or 022 that are not real children
+            temp_records_duplicates = set()
 
             for record in temp_records:
                 temp_fields = record.data.xpath(f'./m:datafield/m:subfield[contains(text(), "{std_num}")]',
                                                 namespaces=SruClient.nsmap)
 
                 if len(temp_fields) > 0:
                     for field in temp_fields:
                         code = field.attrib['code']
                         tag = field.getparent().attrib['tag']
                         if tag in ['020', '022']:
                             self.warning = True
                             self.warning_messages.append(f'More than one record with same {tag}, {self.mms_id} '
                                                          f'and {record.mms_id} are probably duplicated records')
-
-                        fields_related_records.append({'child_MMS_ID': record.mms_id,
-                                                       'field': f'{tag}${code}',
-                                                       'content': field.text})
+                        else:
+                            fields_related_records.append({'child_MMS_ID': record.mms_id,
+                                                           'field': f'{tag}${code}',
+                                                           'content': field.text})
                 else:
                     logging.warning(f'{repr(self)} record {repr(record)} found with SRU but no linking field')
                     fields_related_records.append({'child_MMS_ID': record.mms_id,
                                                    'field': f'UNKNOWN',
                                                    'content': std_num})
+            # Use sets to avoid duplicated records
+            records.update(set(temp_records) - temp_records_duplicates)
 
         if len(records) == 0:
             related_record_found = False
         else:
             related_record_found = True
 
         self._child_rec_std_num = {'MMS_ID': self.mms_id,
@@ -742,34 +747,41 @@
         for link in children_analysis['fields_related_records']:
             if link['field'] == '773$w':
                 analytical_children.append(SruRecord(link['child_MMS_ID']))
 
         return analytical_children
 
     @check_error
-    def is_removable(self) -> Tuple[bool, str]:
-        """is_removable(self) -> Tuple[bool, str]
+    def is_removable(self, removable_rec_mms_id: Optional[List[str]] = None) -> Tuple[bool, str]:
+        """is_removable(self, removable_rec_mms_id: Optional[List[str]] = None) -> Tuple[bool, str]
         Check if a record is safe to be removed
 
         The method checks related records and inventory in other IZ.
         1. Test if the record has 852 fields. It would indicate existing holding in any IZ
         2. Test if record has analytical records children (children linked with 773 field)
         3. Test if the record is target of 8xx or 773 fields of other records
         4. Test if the record has a 773 field targeting a record with inventory
 
         :return: tuple containing bool indicating if the record can be safely removed and a message.
         """
+        # Set default value for removable_rec_mms_id
+        if removable_rec_mms_id is None:
+            removable_rec_mms_id = []
+
         # Check if record used by other IZ and has holdings
         list_izs = self.get_iz_using_rec()
         if len(list_izs) > 0:
             logging.warning(f'{repr(self)} cannot be deleted: record used in other IZs: {", ".join(list_izs)}')
             return False, 'Record used in other IZ'
 
         # No deletion if records has analytical records among children
-        analytical_children = self.get_child_analytical_records()
+        # Filter the list with the list of removable records.
+        analytical_children = [rec for rec in self.get_child_analytical_records()
+                               if rec.mms_id not in removable_rec_mms_id]
+
         if len(analytical_children) > 0:
             logging.warning(f'{repr(self)} cannot be deleted: record has at least one child '
                             f'analytical record: {repr(analytical_children[0])}')
             return False, 'Has analytical record as child'
 
         # Check if the record has children with inventory. The child must have be linked with a 8xx field
         # or 773. Normally analytical records linked with 773 should not have holdings anyway.
```

### Comparing `almasru-1.0.8/almasru/configlog.py` & `almasru-1.1.0/almasru/configlog.py`

 * *Files identical despite different names*

### Comparing `almasru-1.0.8/almasru/utils.py` & `almasru-1.1.0/almasru/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,24 +63,26 @@
 
     # This set contains all processed records, useful to avoid to process twice the same record
     processed_records = set()
 
     # Fetch all records to analyse
     records = [SruRecord(mms_id) for mms_id in mms_ids]
 
+    removable_rec_mms_ids = []
+
     while len(records) > 0:
-        rec = records.pop()
+        rec = records.pop(0)
         logging.info(f'Processed: {len(processed_records)} / remaining: {len(records)} / current: {repr(rec)}')
 
         # Avoid to analyse the same record twice
         if rec in processed_records:
             continue
 
         # Check if the record is removable
-        is_removable = rec.is_removable()
+        is_removable = rec.is_removable(removable_rec_mms_ids)
 
         # Add the record to the list of processed records to avoid twice analyses
         processed_records.add(rec)
 
         # Record encountered an error
         if rec.error is True:
             df.loc[rec.mms_id] = [False,
@@ -116,14 +118,17 @@
                               '|'.join(rec.get_iz_using_rec()),
                               '|'.join(children),
                               '|'.join(parents),
                               np.nan,
                               np.nan if rec.warning is False else rec.warning_messages[-1],
                               rec.error]
 
+        # Get list of mms_id to ignore when checking for existing child analytical records
+        removable_rec_mms_ids = df.loc[df.removable].index.values
+
     df['additional_mms_id'] = ~df.index.isin(mms_ids)
 
     # Check the children, if some links exist that will be broken if the record is removed.
     removable_rec_mms_ids = df.loc[df.removable].index.values
 
     # Get the list of removable records, check of links is only meaningful for removable records
     removable_records = [SruRecord(mms_id) for mms_id in removable_rec_mms_ids]
```

### Comparing `almasru-1.0.8/almasru.egg-info/PKG-INFO` & `almasru-1.1.0/almasru.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almasru
-Version: 1.0.8
+Version: 1.1.0
 Summary: This python module is a tool to use Alma SRU. it manages the logs and the backup of the records.
 Author-email: Raphaël Rey <raphael.rey@slsp.ch>
 Project-URL: Homepage, https://github.com/Swiss-Library-Service-Platform/almasru
 Project-URL: Bug Tracker, https://github.com/Swiss-Library-Service-Platform/almasru/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `almasru-1.0.8/licence.txt` & `almasru-1.1.0/licence.txt`

 * *Files identical despite different names*

### Comparing `almasru-1.0.8/pyproject.toml` & `almasru-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "almasru"
-version = "1.0.8"
+version = "1.1.0"
 authors = [
   { name="Raphaël Rey", email="raphael.rey@slsp.ch" },
 ]
 description = "This python module is a tool to use Alma SRU. it manages the logs and the backup of the records."
 readme = "readme.rst"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `almasru-1.0.8/test/test_sruclient.py` & `almasru-1.1.0/test/test_sruclient.py`

 * *Files identical despite different names*

