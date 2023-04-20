# Comparing `tmp/itemdb-1.1.1.tar.gz` & `tmp/itemdb-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itemdb-1.1.1.tar", last modified: Thu Mar 18 21:27:14 2021, max compression
+gzip compressed data, was "itemdb-1.1.2.tar", last modified: Thu Apr 20 23:34:14 2023, max compression
```

## Comparing `itemdb-1.1.1.tar` & `itemdb-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2021-03-18 21:27:14.095900 itemdb-1.1.1/
--rw-rw-rw-   0        0        0     1374 2021-03-18 21:27:14.094905 itemdb-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2305 2021-03-17 16:14:40.000000 itemdb-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2021-03-18 21:27:14.092908 itemdb-1.1.1/itemdb.egg-info/
--rw-rw-rw-   0        0        0     1374 2021-03-18 21:27:13.000000 itemdb-1.1.1/itemdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2021-03-18 21:27:13.000000 itemdb-1.1.1/itemdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-18 21:27:13.000000 itemdb-1.1.1/itemdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2021-03-18 21:27:13.000000 itemdb-1.1.1/itemdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2020-06-09 15:16:33.000000 itemdb-1.1.1/itemdb.egg-info/zip-safe
--rw-rw-rw-   0        0        0    22790 2021-03-18 21:25:50.000000 itemdb-1.1.1/itemdb.py
--rw-rw-rw-   0        0        0       42 2021-03-18 21:27:14.095900 itemdb-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2069 2020-06-09 15:15:08.000000 itemdb-1.1.1/setup.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-20 23:34:14.249249 itemdb-1.1.2/
+-rw-r--r--   0 almar      (501) staff       (20)     1073 2023-04-20 21:02:09.000000 itemdb-1.1.2/LICENSE
+-rw-r--r--   0 almar      (501) staff       (20)     1337 2023-04-20 23:34:14.247783 itemdb-1.1.2/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     2356 2023-04-20 23:33:04.000000 itemdb-1.1.2/README.md
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-20 23:34:14.247108 itemdb-1.1.2/itemdb.egg-info/
+-rw-r--r--   0 almar      (501) staff       (20)     1337 2023-04-20 23:34:13.000000 itemdb-1.1.2/itemdb.egg-info/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)      181 2023-04-20 23:34:14.000000 itemdb-1.1.2/itemdb.egg-info/SOURCES.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2023-04-20 23:34:13.000000 itemdb-1.1.2/itemdb.egg-info/dependency_links.txt
+-rw-r--r--   0 almar      (501) staff       (20)        7 2023-04-20 23:34:13.000000 itemdb-1.1.2/itemdb.egg-info/top_level.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2023-04-20 23:34:13.000000 itemdb-1.1.2/itemdb.egg-info/zip-safe
+-rw-r--r--   0 almar      (501) staff       (20)    26808 2023-04-20 23:33:22.000000 itemdb-1.1.2/itemdb.py
+-rw-r--r--   0 almar      (501) staff       (20)       38 2023-04-20 23:34:14.249368 itemdb-1.1.2/setup.cfg
+-rw-r--r--   0 almar      (501) staff       (20)     2118 2023-04-20 21:02:09.000000 itemdb-1.1.2/setup.py
```

### Comparing `itemdb-1.1.1/PKG-INFO` & `itemdb-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 1.2
-Name: itemdb
-Version: 1.1.1
-Summary: Easy transactional database for Python dicts, backed by SQLite
-Home-page: https://github.com/almarklein/itemdb
-Author: Almar Klein
-Author-email: 
-License: MIT
-Description: 
-        The itemdb library allows you to store and retrieve Python dicts in a
-        database on the local filesystem, in an easy, fast, and reliable way.
-        
-        Based on the rock-solid and ACID compliant SQLite, but with easy and
-        explicit transactions using a ``with`` statement. It provides a simple
-        object-based API, with the flexibility to store (JSON-compatible) items
-        with arbitrary fields, and add indices when needed.
-        
-Keywords: database,sqlite,no-sql
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Database
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Metadata-Version: 2.1
+Name: itemdb
+Version: 1.1.2
+Summary: Easy transactional database for Python dicts, backed by SQLite
+Home-page: https://github.com/almarklein/itemdb
+Author: Almar Klein
+Author-email: 
+License: MIT
+Keywords: database,sqlite,no-sql
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Database
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+License-File: LICENSE
+
+
+The itemdb library allows you to store and retrieve Python dicts in a
+database on the local filesystem, in an easy, fast, and reliable way.
+
+Based on the rock-solid and ACID compliant SQLite, but with easy and
+explicit transactions using a ``with`` statement. It provides a simple
+object-based API, with the flexibility to store (JSON-compatible) items
+with arbitrary fields, and add indices when needed.
```

### Comparing `itemdb-1.1.1/README.md` & `itemdb-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![PyPI Version](https://img.shields.io/pypi/v/itemdb.svg)](https://pypi.python.org/pypi/itemdb/)
-![CI](https://github.com/almarklein/itemdb/workflows/CI/badge.svg)
+[![CI](https://github.com/almarklein/itemdb/workflows/CI/badge.svg)](https://github.com/almarklein/itemdb/actions)
 [![Documentation Status](https://readthedocs.org/projects/itemdb/badge/?version=latest)](https://itemdb.readthedocs.io/en/latest/?badge=latest)
 
 # itemdb
 
 
 The itemdb library allows you to store and retrieve Python dicts in a
 database on the local filesystem, in an easy, fast, and reliable way.
@@ -41,15 +41,15 @@
 
 # Update an item
 with db:
     db.put_one("persons", name="John", age=19, fav_number=8)
 
 # Query items
 db.count_all("persons")  # -> 4
-db.select("persons", "age > 20")  # -> list of 2 items
+db.select("persons", "age > ?", 20)  # -> list of 2 items
 ```
 
 See the [guide](https://itemdb.readthedocs.io/en/latest/guide.html) for details.
 
 
 ## Async
```

### Comparing `itemdb-1.1.1/itemdb.egg-info/PKG-INFO` & `itemdb-1.1.2/itemdb.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 1.2
-Name: itemdb
-Version: 1.1.1
-Summary: Easy transactional database for Python dicts, backed by SQLite
-Home-page: https://github.com/almarklein/itemdb
-Author: Almar Klein
-Author-email: 
-License: MIT
-Description: 
-        The itemdb library allows you to store and retrieve Python dicts in a
-        database on the local filesystem, in an easy, fast, and reliable way.
-        
-        Based on the rock-solid and ACID compliant SQLite, but with easy and
-        explicit transactions using a ``with`` statement. It provides a simple
-        object-based API, with the flexibility to store (JSON-compatible) items
-        with arbitrary fields, and add indices when needed.
-        
-Keywords: database,sqlite,no-sql
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Database
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Metadata-Version: 2.1
+Name: itemdb
+Version: 1.1.2
+Summary: Easy transactional database for Python dicts, backed by SQLite
+Home-page: https://github.com/almarklein/itemdb
+Author: Almar Klein
+Author-email: 
+License: MIT
+Keywords: database,sqlite,no-sql
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Database
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+License-File: LICENSE
+
+
+The itemdb library allows you to store and retrieve Python dicts in a
+database on the local filesystem, in an easy, fast, and reliable way.
+
+Based on the rock-solid and ACID compliant SQLite, but with easy and
+explicit transactions using a ``with`` statement. It provides a simple
+object-based API, with the flexibility to store (JSON-compatible) items
+with arbitrary fields, and add indices when needed.
```

### Comparing `itemdb-1.1.1/itemdb.py` & `itemdb-1.1.2/itemdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import json
 import queue
 import asyncio
 import sqlite3
 import threading
 
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 version_info = tuple(map(int, __version__.split(".")))
 
 __all__ = ["ItemDB", "AsyncItemDB", "asyncify"]
 
 json_encode = json.JSONEncoder(ensure_ascii=True).encode
 json_decode = json.JSONDecoder().decode
 
@@ -76,14 +76,20 @@
     asyncified_func.__name__ = "asyncified_" + func.__name__
     return asyncified_func
 
 
 class ItemDB:
     """A transactional database for storage and retrieval of dict items.
 
+    Parameters
+    ----------
+    filename : str
+        The file to open. Use ":memory:" for an in-memory db.
+
+
     The items in the database can be any JSON serializable dictionary.
     Indices can be defined for specific fields to enable fast selection
     of items based on these fields. Indices can be marked as unique to
     make a field mandatory and *identify* items based on that field.
 
     Transactions are done by using the ``with`` statement, and are mandatory
     for all operations that write to the database.
@@ -98,14 +104,15 @@
         )
         self._cur = None
         self._indices_per_table = {}
 
     @property
     def mtime(self):
         """The time that the database file was last modified, as a Unix timestamp.
+
         Is -1 if the file did not exist, or if the filename is not represented
         on the filesystem.
         """
         return self._mtime
 
     def __enter__(self):
         if self._cur is not None:
@@ -123,34 +130,44 @@
         else:
             self._conn.commit()
 
     def __del__(self):
         self._conn.close()
 
     def close(self):
-        """Close the database connection. This will be automatically
-        called when the instance is deleted. But since it can be held
-        e.g. in a traceback, consider using ``with closing(db):``.
+        """Close the database connection.
+
+        This will be automatically called when the instance is deleted.
+        But since it can be held e.g. in a traceback, consider using
+        ``with closing(db):``.
         """
         self._conn.close()
 
     def get_table_names(self):
         """Return a (sorted) list of table names present in the database."""
         cur = self._conn.cursor()
         try:
             cur.execute("SELECT name FROM sqlite_master WHERE type='table';")
             table_names = {x[0] for x in cur}
         finally:
             cur.close()
         return list(sorted(table_names))
 
     def get_indices(self, table_name):
-        """Get a set of indices for the given table. Names prefixed with "!"
-        represent fields that are required and unique. Raises KeyError if the
-        table does not exist.
+        """Get a set of index names for the given table.
+
+        Parameters
+        ----------
+        table_name : str
+            The name of the table to get the indices for.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+
+
+        Names prefixed with "!" represent fields that are required and
+        unique. Raises KeyError if the table does not exist.
         """
         # Use cached?
         try:
             return self._indices_per_table[table_name]
         except KeyError:
             pass
         except TypeError:
@@ -177,14 +194,25 @@
             return found_indices
         else:
             raise KeyError(f"Table {table_name} not present, maybe use ensure_table()?")
 
     def ensure_table(self, table_name, *indices):
         """Ensure that the given table exists and has the given indices.
 
+        Parameters
+        ----------
+        table_name : str
+            The name of the table to make sure exists.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+        indices : varargs
+            A sequence of strings, representing index names. Fields that are
+            indexed can be queried with e.g. ``select()``.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+
+
         If an index name is prefixed with "!", it indicates a field that is
         mandatory and unique. Note that new unique indices cannot be added
         when the table already exist.
 
         This method returns as quickly as possible when the table
         already exists and has the appropriate indices. Returns the
         ItemDB object, so calls to this method can be stacked.
@@ -239,60 +267,81 @@
 
         # Ensure the table.
         # If there is one unique key, make it the primary key and omit rowid.
         # This results in smaller and faster databases.
         text = f"CREATE TABLE IF NOT EXISTS {table_name} (_ob TEXT NOT NULL"
         unique_keys = sorted(x.lstrip("!") for x in indices if x.startswith("!"))
         if len(unique_keys) == 1:
-            text += f", {unique_keys[0]} NOT NULL PRIMARY KEY) WITHOUT ROWID;"
+            index_key = unique_keys[0]
+            text += f", {index_key} NOT NULL PRIMARY KEY) WITHOUT ROWID;"
         else:
-            for key in unique_keys:
-                text += f", {key} NOT NULL UNIQUE"
+            for index_key in unique_keys:
+                text += f", {index_key} NOT NULL UNIQUE"
             text += ");"
         cur.execute(text)
 
         # Ensure the columns and indices
         cur.execute(f"PRAGMA table_info('{table_name}');")
         found_indices = {(x[3] * "!" + x[1]) for x in cur}
 
         for fieldname in sorted(indices):
-            key = fieldname.lstrip("!")
+            index_key = fieldname.lstrip("!")
             if fieldname not in found_indices:
                 if fieldname.startswith("!"):
                     raise IndexError(
                         f"Cannot add unique index {fieldname!r} after the table has been created."
                     )
                 elif fieldname in {x.lstrip("!") for x in found_indices}:
                     raise IndexError(f"Given index {fieldname!r} should be unique.")
-                cur.execute(f"ALTER TABLE {table_name} ADD {key};")
+                cur.execute(f"ALTER TABLE {table_name} ADD {index_key};")
+            cmd = "CREATE INDEX IF NOT EXISTS"
             cur.execute(
-                f"CREATE INDEX IF NOT EXISTS idx_{table_name}_{key} ON {table_name} ({key})"
+                f"{cmd} idx_{table_name}_{index_key} ON {table_name} ({index_key})"
             )
 
     def delete_table(self, table_name):
         """Delete the table with the given name.
-        This method must be called within a transaction.
 
-        Warning: this deletes the whole table, including all of its items.
+        Parameters
+        ----------
+        table_name : str
+            The name of the table to delete.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+
 
-        Can raise KeyError if an invalid table is given, or IOError if not
-        used within a transaction
+        Be aware that this deletes the whole table, including all of
+        its items.
+
+        This method must be called within a transaction. Can raise
+        KeyError if an invalid table is given, or IOError if not used
+        within a transaction
         """
         self.get_indices(table_name)  # Fail with KeyError for invalid table name
         cur = self._cur
         if cur is None:
             raise IOError("Can only use delete_table() within a transaction.")
         self._indices_per_table.pop(table_name, None)
         self._cur.execute(f"DROP TABLE {table_name}")
 
     def rename_table(self, table_name, new_table_name):
-        """Rename a table. This method must be called within a transaction.
+        """Rename a table.
 
-        Can raise KeyError if an invalid table is given, or IOError if not
-        used within a transaction
+        Parameters
+        ----------
+        table_name : str
+            The current name of the table.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+        new_table_name : str
+            The new name.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+
+
+        This method must be called within a transaction. Can raise
+        KeyError if an invalid table is given, or IOError if not used
+        within a transaction
         """
         self.get_indices(table_name)  # Fail with KeyError for invalid table name
         if not (isinstance(new_table_name, str) and new_table_name.isidentifier()):
             raise TypeError(f"Table name must be a str identifier, not '{table_name}'")
         cur = self._cur
         if cur is None:
             raise IOError("Can only use rename_table() within a transaction.")
@@ -305,67 +354,93 @@
         cur = self._conn.cursor()
         try:
             cur.execute(f"SELECT COUNT(*) FROM {table_name}")
             return cur.fetchone()[0]
         finally:
             cur.close()
 
-    def count(self, table_name, query, *args):
+    def count(self, table_name, query, *save_args):
         """Get the number of items in the given table that match the given query.
 
+        Parameters
+        ----------
+        table_name : str
+            The name of the table to count items in.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+        query : str
+            The query to select items on.
+            *To avoid SQL injection, this arg should not be based on unsafe data;
+            use save_args for end-user input.*
+        save_args : varargs
+            The values to select items on.
+
+
         Examples::
 
             # Count the persons older than 20
-            db.count("persons", "age > 20")
-            # Use parameters for variables (to avoid SQL injection)
+            db.count("persons", "age > ?", 20)
+            # Count the persons older than a given value
             db.count("persons", "age > ?", min_age)
             # Use AND and OR for more precise queries
             db.count("persons", "age > ? AND age < ?", min_age, max_age)
 
-        See select() for details on queries.
+        See ``select(``) for details on queries.
 
         Can raise KeyError if an invalid table is given, IndexError if an
         invalid field is used in the query, or sqlite3.OperationalError for
         an invalid query.
         """
         self.get_indices(table_name)  # Fail with KeyError for invalid table name
         cur = self._conn.cursor()
         try:
-            cur.execute(f"SELECT COUNT(*) FROM {table_name} WHERE {query}", args)
+            cur.execute(f"SELECT COUNT(*) FROM {table_name} WHERE {query}", save_args)
             return cur.fetchone()[0]
         except sqlite3.OperationalError as err:
             if "no such column" in str(err).lower():
                 raise IndexError(str(err))
             raise err
         finally:
             cur.close()
 
     def select_all(self, table_name):
-        """Get all items in the given table. See select() for details."""
+        """Get all items in the given table. See ``select()`` for details."""
         self.get_indices(table_name)  # Fail with KeyError for invalid table name
         cur = self._conn.cursor()
         try:
             cur.execute(f"SELECT _ob FROM {table_name}")
             return [json_decode(x[0]) for x in cur]
         finally:
             cur.close()
 
-    def select(self, table_name, query, *args):
+    def select(self, table_name, query, *save_args):
         """Get the items in the given table that match the given query.
 
+        Parameters
+        ----------
+        table_name : str
+            The name of the table to select items in.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+        query : str
+            The query to select items on.
+            *To avoid SQL injection, this arg should not be based on unsafe data;
+            use save_args for end-user input.*
+        save_args : varargs
+            The values to select items on.
+
+
         The query follows SQLite syntax and can only include indexed
         fields. If needed, use ensure_table() to add indices. The query
-        is always fast (which is why this method is called select, and
-        not search).
+        is always fast (which is why this method is called 'select', and
+        not 'search').
 
         Examples::
 
             # Select the persons older than 20
-            db.select("persons", "age > 20")
-            # Use parameters for variables (to avoid SQL injection)
+            db.select("persons", "age > ?",  20)
+            # Select the persons older than a given age
             db.select("persons", "age > ?", min_age)
             # Use AND and OR for more precise queries
             db.select("persons", "age > ? AND age < ?", min_age, max_age)
 
         There is no method to filter items bases on non-indexed fields,
         because this is easy using a list comprehension, e.g.::
 
@@ -378,99 +453,146 @@
         """
         self.get_indices(table_name)  # Fail with KeyError for invalid table name
         # It is tempting to make this a generator, but also dangerous because
         # the cursor might not be closed if the generator is stored somewhere
         # and not run through the end.
         cur = self._conn.cursor()
         try:
-            cur.execute(f"SELECT _ob FROM {table_name} WHERE {query}", args)
+            cur.execute(f"SELECT _ob FROM {table_name} WHERE {query}", save_args)
             return [json_decode(x[0]) for x in cur]
         except sqlite3.OperationalError as err:
             if "no such column" in str(err).lower():
                 raise IndexError(str(err))
             raise err
         finally:
             cur.close()
 
     def select_one(self, table_name, query, *args):
         """Get the first item in the given table that match the given query.
-        Returns None if there was no match. See select() for details.
+
+        Parameters
+        ----------
+        table_name : str
+            The name of the table to select an item in.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+        query : str
+            The query to select the item on.
+            *To avoid SQL injection, this arg should not be based on unsafe data;
+            use save_args for end-user input.*
+        save_args : varargs
+            The values to select the item on.
+
+
+        Returns None if there was no match. See ``select()`` for details.
         """
         items = self.select(table_name, query, *args)
         return items[0] if items else None
 
     def put(self, table_name, *items):
         """Put one or more items into the given table.
-        This method must be called within a transaction.
 
-        Can raise KeyError if an invalid table is given, IOError if not
-        used within a transaction, TypeError if an item is not a (JSON
+        Parameters
+        ----------
+        table_name : str
+            The name of the table to put the item(s) in.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+        items : varargs
+            The dicts to add. Keys that match an index can later be used for
+            fast querying.
+
+
+        This method must be called within a transaction. Can raise
+        KeyError if an invalid table is given, IOError if not used
+        within a transaction, TypeError if an item is not a (JSON
         serializable) dict, or IndexError if an item does not have a
         required field.
         """
         cur = self._cur
         if cur is None:
             raise IOError("Can only use put() within a transaction.")
 
         # Get indices - fail with KeyError for invalid table name
         indices = self.get_indices(table_name)
 
         for item in items:
             if not isinstance(item, dict):
                 raise TypeError("Expecing each item to be a dict")
 
-            row_keys = "_ob"
+            index_keys = "_ob"
             row_plac = "?"
             row_vals = [json_encode(item)]  # Can raise TypeError
             for fieldname in indices:
-                key = fieldname.lstrip("!")
-                if key in item:
-                    row_keys += ", " + key
+                index_key = fieldname.lstrip("!")
+                if index_key in item:
+                    index_keys += ", " + index_key
                     row_plac += ", ?"
-                    row_vals.append(item[key])
+                    row_vals.append(item[index_key])
                 elif fieldname.startswith("!"):
-                    raise IndexError(f"Item does not have required field {key!r}")
+                    raise IndexError(f"Item does not have required field {index_key!r}")
 
             cur.execute(
-                f"INSERT OR REPLACE INTO {table_name} ({row_keys}) VALUES ({row_plac})",
+                f"INSERT OR REPLACE INTO {table_name} ({index_keys}) VALUES ({row_plac})",
                 row_vals,
             )
 
     def put_one(self, table_name, **item):
         """Put an item into the given table using kwargs.
+
+        Parameters
+        ----------
+        table_name : str
+            The name of the table to put the item(s) in.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+        item : kwargs
+            The dict to add. Keys that match an index can later be used for
+            fast querying.
+
+
         This method must be called within a transaction.
         """
         self.put(table_name, item)
 
-    def delete(self, table_name, query, *args):
+    def delete(self, table_name, query, *save_args):
         """Delete items from the given table.
-        This method must be called within a transaction.
+
+        Parameters
+        ----------
+        table_name : str
+            The name of the table to delete items from.
+            *To avoid SQL injection, this arg should not be based on unsafe data.*
+        query : str
+            The query to select the items to delete.
+            *To avoid SQL injection, this arg should not be based on unsafe data;
+            use save_args for end-user input.*
+        save_args : varargs
+            The values to select the item on.
+
 
         Examples::
 
             # Delete the persons older than 20
-            db.delete("persons", "age > 20")
-            # Use parameters for variables (to avoid SQL injection)
+            db.delete("persons", "age > ?", 20)
+            #  Delete the persons older than a given age
             db.delete("persons", "age > ?", min_age)
             # Use AND and OR for more precise queries
             db.delete("persons", "age > ? AND age < ?", min_age, max_age)
 
-        See select() for details on queries.
+        See ``select()`` for details on queries.
 
-        Can raise KeyError if an invalid table is given, IOError if not
-        used within a transaction, IndexError if an invalid field is
-        used in the query, or sqlite3.OperationalError for an invalid
-        query.
+        This method must be called within a transaction. Can raise
+        KeyError if an invalid table is given, IOError if not used
+        within a transaction, IndexError if an invalid field is used
+        in the query, or sqlite3.OperationalError for an invalid query.
         """
         self.get_indices(table_name)  # Fail with KeyError for invalid table name
         cur = self._cur
         if cur is None:
             raise IOError("Can only use delete() within a transaction.")
         try:
-            cur.execute(f"DELETE FROM {table_name} WHERE {query}", args)
+            cur.execute(f"DELETE FROM {table_name} WHERE {query}", save_args)
         except sqlite3.OperationalError as err:
             if "no such column" in str(err).lower():
                 raise IndexError(str(err))
             raise err
         finally:
             cur.close()
 
@@ -564,15 +686,14 @@
         Thread4AsyncItemDB._count += 1
         super().__init__(name=f"AsyncItemDB_{Thread4AsyncItemDB._count}")
         self.daemon = True
         self._queue = queue
         self.db = None
 
     def run(self) -> None:
-
         while True:
             # Continues running until all queue items are processed,
             # even after closed (so we can finalize all futures)
             future, function, args, kwargs = self._queue.get()
             if future is None:
                 break
```

### Comparing `itemdb-1.1.1/setup.py` & `itemdb-1.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,9 +59,10 @@
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
 )
```

