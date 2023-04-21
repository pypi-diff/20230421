# Comparing `tmp/saffier-0.6.1.tar.gz` & `tmp/saffier-0.7.0.tar.gz`

## Comparing `saffier-0.6.1.tar` & `saffier-0.7.0.tar`

### file list

```diff
@@ -1,60 +1,77 @@
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/__init__.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/exceptions.py
--rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/fields.py
--rw-r--r--   0        0        0    12230 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/metaclass.py
--rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/models.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/py.typed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/testclient.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/__init__.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/base.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/datastructures.py
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/formats.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/registry.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/schemas.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/unique.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/connection.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/constants.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/datastructures.py
--rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/fields.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/manager.py
--rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/queryset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/query/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/query/protocols.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/__init__.py
--rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/base.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/cli.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/constants.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/decorators.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/env.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/__init__.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/branches.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/check.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/current.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/downgrade.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/edit.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/heads.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/history.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/init.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/list_templates.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/makemigrations.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/merge.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/migrate.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/revision.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/show.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/stamp.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/templates/default/README
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/templates/default/alembic.ini.mako
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/templates/default/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/templates/default/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/sqlalchemy/fields.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/sqlalchemy/protocols.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/sqlalchemy/types.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.6.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.6.1/LICENSE
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.6.1/README.md
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 saffier-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    10972 2020-02-02 00:00:00.000000 saffier-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/exceptions.py
+-rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/fields.py
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/metaclass.py
+-rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/models.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/py.typed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/testclient.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/types.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/conf/enums.py
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/conf/functional.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/conf/global_settings.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/conf/module_import.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/__init__.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/base.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/datastructures.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/events.py
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/formats.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/registry.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/schemas.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/sync.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/unique.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/terminal/base.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/terminal/print.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/terminal/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/connection.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/constants.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/datastructures.py
+-rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/fields.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/manager.py
+-rw-r--r--   0        0        0    23146 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/query/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/query/protocols.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/__init__.py
+-rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/base.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/cli.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/constants.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/decorators.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/env.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/branches.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/check.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/current.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/downgrade.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/edit.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/heads.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/history.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/init.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/list_templates.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/makemigrations.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/merge.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/migrate.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/revision.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/show.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/stamp.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/enums.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/templates/default/README
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/templates/default/alembic.ini.mako
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/templates/default/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/templates/default/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/sqlalchemy/fields.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/sqlalchemy/protocols.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/sqlalchemy/types.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.7.0/README.md
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 saffier-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 saffier-0.7.0/PKG-INFO
```

### Comparing `saffier-0.6.1/saffier/__init__.py` & `saffier-0.7.0/saffier/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-__version__ = "0.6.1"
+__version__ = "0.7.0"
+
+from saffier.conf import settings
+from saffier.conf.global_settings import SaffierSettings
 
 from .core.registry import Registry
 from .db.connection import Database
 from .db.constants import CASCADE, RESTRICT, SET_NULL
 from .db.datastructures import Index, UniqueConstraint
 from .db.manager import Manager
 from .db.queryset import QuerySet
@@ -55,14 +58,16 @@
     "MultipleObjectsReturned",
     "OneToOneField",
     "PasswordField",
     "QuerySet",
     "RESTRICT",
     "ReflectModel",
     "Registry",
+    "SaffierSettings",
     "SET_NULL",
     "TextField",
     "TimeField",
     "UniqueConstraint",
     "URLField",
     "UUIDField",
+    "settings",
 ]
```

### Comparing `saffier-0.6.1/saffier/exceptions.py` & `saffier-0.7.0/saffier/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,9 +33,9 @@
     ...
 
 
 class ImproperlyConfigured(SaffierException):
     ...
 
 
-class EnvironmentError(SaffierException):
+class CommandEnvironmentError(SaffierException):
     ...
```

### Comparing `saffier-0.6.1/saffier/fields.py` & `saffier-0.7.0/saffier/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing
 from datetime import date, datetime
 
 import sqlalchemy
+
 from saffier.db.constants import SET_NULL
 from saffier.db.fields import (
     URL,
     UUID,
     Any,
     Boolean,
     Date,
```

### Comparing `saffier-0.6.1/saffier/metaclass.py` & `saffier-0.7.0/saffier/metaclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 import inspect
 import typing
 from typing import TYPE_CHECKING
 
 import sqlalchemy
+
 from saffier import fields as saffier_fields
 from saffier.core.registry import Registry
 from saffier.db.datastructures import Index, UniqueConstraint
 from saffier.db.manager import Manager
 from saffier.exceptions import ImproperlyConfigured
 from saffier.fields import BigIntegerField, Field
 from saffier.types import DictAny
@@ -308,17 +309,19 @@
         cls, name: str, bases: typing.Tuple[typing.Type, ...], attrs: DictAny
     ) -> typing.Any:
         new_model = super().__new__(cls, name, bases, attrs)
 
         registry = new_model._meta.registry
 
         # Remove the reflected models from the registry
+        # Add the reflecte model to the views section of the refected
         if registry:
             try:
                 registry.models.pop(new_model.__name__)
+                registry.reflected[new_model.__name__] = new_model
             except KeyError:
                 ...
 
         return new_model
 
 
 class ModelMeta(metaclass=BaseModelMeta):
```

### Comparing `saffier-0.6.1/saffier/models.py` & `saffier-0.7.0/saffier/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,36 @@
+import asyncio
+import functools
 import typing
 
+import nest_asyncio
 import sqlalchemy
+from sqlalchemy.engine import Engine
+
 from saffier.core.schemas import Schema
 from saffier.core.utils import ModelUtil
 from saffier.db.datastructures import Index, UniqueConstraint
 from saffier.db.manager import Manager
 from saffier.exceptions import ImproperlyConfigured
 from saffier.metaclass import MetaInfo, ModelMeta, ReflectMeta
 
+nest_asyncio.apply()
+
+
+def async_adapter(wrapped_func):
+    """Adapter to run async functions inside the blocking"""
+
+    @functools.wraps(wrapped_func)
+    def run_sync(*args, **kwargs):
+        loop = asyncio.get_event_loop()
+        task = wrapped_func(*args, **kwargs)
+        return loop.run_until_complete(task)
+
+    return run_sync
+
 
 class Model(ModelMeta, ModelUtil):
     """
     The models will always have an id attribute as primery key.
     The primary key can be whatever desired, from IntegerField, FloatField to UUIDField as long as the `id` field is explicitly declared or else it defaults to BigIntegerField.
     """
 
@@ -169,15 +188,19 @@
                 item[first_part] = model_cls._from_row(row, select_related=[remainder])
             else:
                 model_cls = cls.fields[related].target
                 item[related] = model_cls._from_row(row)
 
         # Pull out the regular column values.
         for column in cls.table.columns:
-            if column.name not in item:
+            # Making sure when a table is reflected, maps the right fields of the ReflectModel
+            if column.name not in cls.fields.keys():
+                continue
+
+            elif column.name not in item:
                 item[column.name] = row[column]
 
         return cls(**item)
 
     def __setattr__(self, key: typing.Any, value: typing.Any) -> typing.Any:
         if key in self.fields:
             # Setting a relationship to a raw pk value should set a
@@ -197,21 +220,54 @@
 class ReflectModel(ReflectMeta, Model):
     """
     Reflect on async engines is not yet supported, therefore, we need to make a sync_engine
     call.
     """
 
     @classmethod
+    @functools.lru_cache
+    def get_engine(cls, url: str) -> Engine:
+        return sqlalchemy.create_engine(url)
+
+    @property
+    def pk(self) -> typing.Any:
+        return getattr(self, self.pkname, None)
+
+    @pk.setter
+    def pk(self, value: typing.Any) -> typing.Any:
+        setattr(self, self.pkname, value)
+
+    @classmethod
     def build_table(cls) -> typing.Any:
+        """
+        The inspect is done in an async manner and reflects the objects from the database.
+        """
+
         metadata = cls._meta.registry._metadata  # type: ignore
         tablename = cls._meta.tablename
+        return cls.reflect(tablename, metadata, cls._meta.registry.database)
 
+    @classmethod
+    def inspect(cls, connection, tablename, metadata):
         try:
             return sqlalchemy.Table(
-                tablename,
-                metadata,
-                autoload_with=cls._meta.registry.engine.sync_engine,  # type: ignore
+                tablename, metadata, autoload_with=cls._meta.registry.sync_engine
             )
         except Exception as e:
             raise ImproperlyConfigured(
                 detail=f"Table with the name {tablename} does not exist."
             ) from e
+
+    @classmethod
+    @async_adapter
+    async def reflect(
+        cls,
+        tablename: str,
+        metadata: sqlalchemy.MetaData,
+        database: typing.Any,
+    ) -> sqlalchemy.Table:
+        """SQLAlchemy doesn't support, yet, async reflection and therefore we must run
+        the event loop.
+        """
+        async with database.connection() as connection:
+            table = await connection.run_sync(cls.inspect, tablename, metadata)
+            return table
```

### Comparing `saffier-0.6.1/saffier/core/base.py` & `saffier-0.7.0/saffier/core/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/core/datastructures.py` & `saffier-0.7.0/saffier/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/core/formats.py` & `saffier-0.7.0/saffier/core/formats.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/core/schemas.py` & `saffier-0.7.0/saffier/core/schemas.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/core/unique.py` & `saffier-0.7.0/saffier/core/unique.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/core/utils.py` & `saffier-0.7.0/saffier/core/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/db/datastructures.py` & `saffier-0.7.0/saffier/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/db/fields.py` & `saffier-0.7.0/saffier/db/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/db/manager.py` & `saffier-0.7.0/saffier/db/manager.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/db/queryset.py` & `saffier-0.7.0/saffier/db/queryset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 import typing
 
 import sqlalchemy
+
 from saffier.core.schemas import Schema
 from saffier.core.utils import ModelUtil
 from saffier.db.constants import FILTER_OPERATORS
 from saffier.db.query.protocols import AwaitableQuery
 from saffier.exceptions import DoesNotFound, MultipleObjectsReturned
 from saffier.fields import CharField, TextField
 
@@ -574,15 +575,15 @@
 
         pk = getattr(self.table.c, self.pkname)
         expression = self.table.update().where(pk == sqlalchemy.bindparam(self.pkname))
         kwargs = {field: sqlalchemy.bindparam(field) for obj in new_objs for field in obj.keys()}
         pks = [{self.pkname: getattr(obj, self.pkname)} for obj in objs]
 
         query_list = []
-        for pk, value in zip(pks, new_objs):
+        for pk, value in zip(pks, new_objs):  # noqa
             query_list.append({**pk, **value})
 
         expression = expression.values(kwargs)
         self._set_query_expression(expression)
         await self.database.execute_many(str(expression), query_list)
 
     async def delete(self) -> None:
```

### Comparing `saffier-0.6.1/saffier/db/query/protocols.py` & `saffier-0.7.0/saffier/db/query/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/migrations/base.py` & `saffier-0.7.0/saffier/migrations/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/migrations/operations/branches.py` & `saffier-0.7.0/saffier/migrations/operations/heads.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-"""
-Client to interact with Saffier models and migrations.
-"""
-
-from typing import Any
-
 import click
 
-from saffier.migrations.base import branches as _branches
+from saffier.migrations.base import heads as _heads
+from saffier.migrations.env import MigrationEnv
 
 
 @click.option(
     "-d",
     "--directory",
     default=None,
     help=('Migration script directory (default is "migrations")'),
 )
 @click.option("-v", "--verbose", is_flag=True, help="Use more verbose output")
+@click.option(
+    "--resolve-dependencies", is_flag=True, help="Treat dependency versions as down revisions"
+)
 @click.command()
-@click.pass_context
-def branches(ctx: Any, directory: str, verbose: bool) -> None:
-    """Show current branch points"""
-    _branches(ctx.obj, directory, verbose)
+def heads(env: MigrationEnv, directory: str, verbose: bool, resolve_dependencies: bool) -> None:
+    """Show current available heads in the script directory"""
+    _heads(env.app, directory, verbose, resolve_dependencies)
```

### Comparing `saffier-0.6.1/saffier/migrations/operations/downgrade.py` & `saffier-0.7.0/saffier/migrations/operations/downgrade.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-"""
-Client to interact with Saffier models and migrations.
-"""
-
 from typing import Any
 
 import click
 
 from saffier.migrations.base import downgrade as _downgrade
+from saffier.migrations.env import MigrationEnv
 
 
 @click.option(
     "-d",
     "--directory",
     default=None,
     help=('Migration script directory (default is "migrations")'),
@@ -22,11 +19,12 @@
     "--tag", default=None, help=('Arbitrary "tag" name - can be used by custom env.py ' "scripts")
 )
 @click.option(
     "-x", "--arg", multiple=True, help="Additional arguments consumed by custom env.py scripts"
 )
 @click.command()
 @click.argument("revision", default="-1")
-@click.pass_context
-def downgrade(ctx: Any, directory: str, sql: bool, tag: str, arg: Any, revision: str) -> None:
+def downgrade(
+    env: MigrationEnv, directory: str, sql: bool, tag: str, arg: Any, revision: str
+) -> None:
     """Revert to a previous version"""
-    _downgrade(ctx.obj, directory, revision, sql, tag, arg)
+    _downgrade(env.app, directory, revision, sql, tag, arg)
```

### Comparing `saffier-0.6.1/saffier/migrations/operations/history.py` & `saffier-0.7.0/saffier/migrations/operations/history.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-"""
-Client to interact with Saffier models and migrations.
-"""
-
-from typing import Any
-
 import click
 
 from saffier.migrations.base import history as _history
+from saffier.migrations.env import MigrationEnv
 
 
 @click.option(
     "-d",
     "--directory",
     default=None,
     help=('Migration script directory (default is "migrations")'),
@@ -22,13 +17,12 @@
 @click.option(
     "-i",
     "--indicate-current",
     is_flag=True,
     help=("Indicate current version (Alembic 0.9.9 or greater is " "required)"),
 )
 @click.command()
-@click.pass_context
 def history(
-    ctx: Any, directory: str, rev_range: str, verbose: bool, indicate_current: bool
+    env: MigrationEnv, directory: str, rev_range: str, verbose: bool, indicate_current: bool
 ) -> None:
     """List changeset scripts in chronological order."""
-    _history(ctx.obj, directory, rev_range, verbose, indicate_current)
+    _history(env.app, directory, rev_range, verbose, indicate_current)
```

### Comparing `saffier-0.6.1/saffier/migrations/operations/init.py` & `saffier-0.7.0/saffier/migrations/operations/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-"""
-Client to interact with Saffier models and migrations.
-"""
-
-from typing import Any
-
 import click
 
 from saffier.migrations.base import init as _init
+from saffier.migrations.env import MigrationEnv
 
 
 @click.option(
     "-d",
     "--directory",
     default=None,
     help=('Migration script directory (default is "migrations")'),
@@ -20,11 +15,10 @@
 )
 @click.option(
     "--package",
     is_flag=True,
     help=("Write empty __init__.py files to the environment and " "version locations"),
 )
 @click.command(name="init")
-@click.pass_context
-def init(ctx: Any, directory: str, template: str, package: bool) -> None:
+def init(env: MigrationEnv, directory: str, template: str, package: bool) -> None:
     """Creates a new migration repository."""
-    _init(ctx.obj, directory, template, package)
+    _init(env.app, directory, template, package)
```

### Comparing `saffier-0.6.1/saffier/migrations/operations/makemigrations.py` & `saffier-0.7.0/saffier/migrations/operations/makemigrations.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from typing import Any
 
 import click
 
 from saffier.migrations.base import migrate as _migrate
+from saffier.migrations.env import MigrationEnv
 
 
 @click.option(
     "-d",
     "--directory",
     default=None,
     help=('Migration script directory (default is "migrations")'),
@@ -36,25 +37,24 @@
 @click.option(
     "--rev-id", default=None, help=("Specify a hardcoded revision id instead of generating " "one")
 )
 @click.option(
     "-x", "--arg", multiple=True, help="Additional arguments consumed by custom env.py scripts"
 )
 @click.command()
-@click.pass_context
 def makemigrations(
-    ctx: Any,
+    env: MigrationEnv,
     directory: str,
     message: str,
     sql: bool,
     head: str,
     splice: bool,
     branch_label: str,
     version_path: str,
     rev_id: str,
     arg: Any,
 ) -> None:
     """Autogenerate a new revision file (Alias for
     'revision --autogenerate')"""
     _migrate(
-        ctx.obj, directory, message, sql, head, splice, branch_label, version_path, rev_id, arg
+        env.app, directory, message, sql, head, splice, branch_label, version_path, rev_id, arg
     )
```

### Comparing `saffier-0.6.1/saffier/migrations/operations/migrate.py` & `saffier-0.7.0/saffier/migrations/operations/migrate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-"""
-Client to interact with Saffier models and migrations.
-"""
-
 from typing import Any
 
 import click
 
 from saffier.migrations.base import upgrade as _upgrade
+from saffier.migrations.env import MigrationEnv
 
 
 @click.option(
     "-d",
     "--directory",
     default=None,
     help=('Migration script directory (default is "migrations")'),
@@ -22,14 +19,15 @@
     "--tag", default=None, help=('Arbitrary "tag" name - can be used by custom env.py ' "scripts")
 )
 @click.option(
     "-x", "--arg", multiple=True, help="Additional arguments consumed by custom env.py scripts"
 )
 @click.command()
 @click.argument("revision", default="head")
-@click.pass_context
-def migrate(ctx: Any, directory: str, sql: bool, tag: str, arg: Any, revision: str) -> None:
+def migrate(
+    env: MigrationEnv, directory: str, sql: bool, tag: str, arg: Any, revision: str
+) -> None:
     """
     Upgrades to the latest version or to a specific version
     provided by the --tag.
     """
-    _upgrade(ctx.obj, directory, revision, sql, tag, arg)
+    _upgrade(env.app, directory, revision, sql, tag, arg)
```

### Comparing `saffier-0.6.1/saffier/migrations/operations/revision.py` & `saffier-0.7.0/saffier/migrations/operations/revision.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-"""
-Client to interact with Saffier models and migrations.
-"""
-
-from typing import Any
-
 import click
 
 from saffier.migrations.base import revision as _revision
+from saffier.migrations.env import MigrationEnv
 
 
 @click.option(
     "-d",
     "--directory",
     default=None,
     help=('Migration script directory (default is "migrations")'),
@@ -41,30 +36,29 @@
 @click.option(
     "--version-path", default=None, help=("Specify specific path from config for version file")
 )
 @click.option(
     "--rev-id", default=None, help=("Specify a hardcoded revision id instead of generating " "one")
 )
 @click.command()
-@click.pass_context
 def revision(
-    ctx: Any,
+    env: MigrationEnv,
     directory: str,
     message: str,
     autogenerate: bool,
     sql: bool,
     head: str,
     splice: bool,
     branch_label: str,
     version_path: str,
     rev_id: str,
 ) -> None:
     """Create a new revision file."""
     _revision(
-        ctx.obj,
+        env.app,
         directory,
         message,
         autogenerate,
         sql,
         head,
         splice,
         branch_label,
```

### Comparing `saffier-0.6.1/saffier/migrations/operations/stamp.py` & `saffier-0.7.0/saffier/migrations/operations/stamp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-"""
-Client to interact with Saffier models and migrations.
-"""
-
-from typing import Any
-
 import click
 
 from saffier.migrations.base import stamp as _stamp
+from saffier.migrations.env import MigrationEnv
 
 
 @click.option(
     "-d",
     "--directory",
     default=None,
     help=('Migration script directory (default is "migrations")'),
@@ -19,12 +14,11 @@
     "--sql", is_flag=True, help=("Don't emit SQL to database - dump to standard output " "instead")
 )
 @click.option(
     "--tag", default=None, help=('Arbitrary "tag" name - can be used by custom env.py ' "scripts")
 )
 @click.argument("revision", default="head")
 @click.command()
-@click.pass_context
-def stamp(ctx: Any, directory: str, sql: bool, tag: str, revision: str) -> None:
+def stamp(env: MigrationEnv, directory: str, sql: bool, tag: str, revision: str) -> None:
     """'stamp' the revision table with the given revision; don't run any
     migrations"""
-    _stamp(ctx.obj, directory, revision, sql, tag)
+    _stamp(env.app, directory, revision, sql, tag)
```

### Comparing `saffier-0.6.1/saffier/migrations/templates/default/alembic.ini.mako` & `saffier-0.7.0/saffier/migrations/templates/default/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/saffier/migrations/templates/default/env.py` & `saffier-0.7.0/saffier/migrations/templates/default/env.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 import logging
 import os
 import sys
 from logging.config import fileConfig
 from typing import Any, Union
 
 from alembic import context
+from databasez import DatabaseURL
 from rich.console import Console
+from sqlalchemy import create_engine
+from sqlalchemy.ext.asyncio import create_async_engine
 
+from saffier import settings
 from saffier.exceptions import SaffierException
 from saffier.migrations.constants import APP_PARAMETER
 from saffier.migrations.env import MigrationEnv
-from sqlalchemy.ext.asyncio import create_async_engine
 
 # The console used for the outputs
 console = Console()
 
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
 config: Any = context.config
@@ -111,24 +114,50 @@
         **app._saffier_db["migrate"].kwargs,
     )
 
     with context.begin_transaction():
         context.run_migrations()
 
 
+def is_async_connection(url: DatabaseURL) -> bool:
+    """
+    Verifies if is an async connection string.
+
+    Validates the type of driver against the ones supported by Saffier.
+    """
+    if not url.driver:
+        return False
+
+    if (
+        (url.driver in settings.postgres_drivers)
+        or (url.driver in settings.mysql_drivers)
+        or (url.driver in settings.sqlite_drivers)
+        or url.driver in settings.mssql_drivers
+    ):
+        return True
+    return False
+
+
 async def run_migrations_online() -> Any:
     """Run migrations in 'online' mode.
 
     In this scenario we need to create an Engine
     and associate a connection with the context.
 
     """
-    connectable = create_async_engine(get_engine_url(), echo=True)
+    database_url = DatabaseURL(get_engine_url())
+    is_async = is_async_connection(database_url)
 
-    async with connectable.connect() as connection:
-        await connection.run_sync(do_run_migrations)
+    if is_async:
+        connectable = create_async_engine(database_url._url)
+        async with connectable.connect() as connection:
+            await connection.run_sync(do_run_migrations)
+    else:
+        connectable = create_engine(database_url._url)
+        with connectable.connect() as connection:
+            do_run_migrations(connection)
 
 
 if context.is_offline_mode():
     run_migrations_offline()
 else:
     asyncio.get_event_loop().run_until_complete(run_migrations_online())
```

### Comparing `saffier-0.6.1/saffier/sqlalchemy/fields.py` & `saffier-0.7.0/saffier/sqlalchemy/fields.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ipaddress
 import uuid
 from typing import Any
 
+import sqlalchemy
 from orjson import loads
 
-import sqlalchemy
 from saffier.sqlalchemy.protocols import BaseFieldProtocol
 from saffier.sqlalchemy.types import SubList
 from saffier.types import DictAny
 
 DIALECTS = {"postgres": "postgres", "postgresql": "postgresql"}
```

### Comparing `saffier-0.6.1/saffier/sqlalchemy/protocols.py` & `saffier-0.7.0/saffier/sqlalchemy/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/LICENSE` & `saffier-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/README.md` & `saffier-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `saffier-0.6.1/pyproject.toml` & `saffier-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -35,21 +35,23 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "alembic>=1.9.3,<2.0.0",
+    "anyio>=3.6.2,<4",
     "click>=8.1.3,<9.0.0",
     "loguru>=0.6.0,<0.7.0",
-    "databasez>=0.1.0",
+    "databasez>=0.2.0",
+    "nest_asyncio>=1.5.6,<2.0.0",
     "orjson >=3.8.5,<4.0.0",
     "pydantic>=1.10.5,<2.0.0",
     "rich>=13.3.1,<14.0.0",
-    "sqlalchemy>=2.0.8,<2.0.10",
+    "sqlalchemy>=2.0.8,<2.1",
 ]
 keywords = [
     "api",
     "rest",
     "http",
     "asgi",
     "pydantic",
@@ -66,19 +68,18 @@
 Homepage = "https://github.com/tarsil/saffier"
 Documentation = "https://saffier.tarsild.io/"
 Changelog = "https://saffier.tarsild.io/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
 Source = "https://github.com/tarsil/saffier"
 
 [project.scripts]
-saffier-admin = "saffier.migrations.cli:saffier_cli"
+saffier = "saffier.migrations.cli:saffier_cli"
 
 [project.optional-dependencies]
 test = [
-    "anyio>=3.0.0,<4",
     "asyncpg>=0.27.0,<1",
     "asyncmy>=0.2.7,<0.3.0",
     "esmerald>=1.1.0",
     "pytest>=7.1.3,<8.0.0",
     "pytest-cov>=2.12.0,<5.0.0",
     "pytest-asyncio >=0.19.0",
     "mypy==1.1.1",
@@ -109,39 +110,49 @@
     "mdx-include>=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin>=0.1.7,<0.3.0",
     "mkdocstrings>=0.19.0,<0.21.0",
     "pyyaml>=5.3.1,<7.0.0",
 ]
 
 testing = ["sqlalchemy_utils>=0.40.0"]
-postgres = ["databasez[postgresql]"]
+postgres = ["databasez[postgressql]"]
 mysql = ["databasez[mysql]"]
 sqlite = ["databasez[sqlite]"]
 
+ptpython = ["ptpython>=3.0.23,<4.0.0"]
+ipython = ["ipython>=8.10.0,<9.0.0"]
+
 all = [
     "databasez[postgresql,mysql,sqlite]",
     "orjson>=3.8.5,<4.0.0",
     "pydantic>=1.10.4,<2.0.0",
+    "ptpython>=3.0.23,<4.0.0",
+    "ipython>=8.10.0,<9.0.0",
 ]
 
 [tool.hatch.version]
 path = "saffier/__init__.py"
 
 [tool.isort]
 profile = "black"
-known_third_party = ["esmerald", "pydantic", "starlette"]
-src_paths = ["saffier"]
+known_third_party = ["esmerald", "pydantic", "starlette", "saffier"]
 
 [tool.mypy]
+warn_unused_configs = true
+warn_unreachable = true
+warn_return_any = true
 strict = true
-disallow_any_generics = false
 disallow_untyped_decorators = true
-implicit_reexport = true
+disallow_any_generics = false
+implicit_reexport = false
+show_error_codes = true
 disallow_incomplete_defs = true
 disable_error_code = "attr-defined"
+warn_unused_ignores = true
+warn_redundant_casts = true
 
 [tool.ruff]
 select = [
     "E", # pycodestyle errors
     "W", # pycodestyle warnings
     "F", # pyflakes
     "C", # flake8-comprehensions
```

### Comparing `saffier-0.6.1/PKG-INFO` & `saffier-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saffier
-Version: 0.6.1
+Version: 0.7.0
 Summary: The only python ORM you will ever need.
 Project-URL: Homepage, https://github.com/tarsil/saffier
 Project-URL: Documentation, https://saffier.tarsild.io/
 Project-URL: Changelog, https://saffier.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/saffier
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -33,24 +33,28 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: alembic<2.0.0,>=1.9.3
+Requires-Dist: anyio<4,>=3.6.2
 Requires-Dist: click<9.0.0,>=8.1.3
-Requires-Dist: databasez>=0.1.0
+Requires-Dist: databasez>=0.2.0
 Requires-Dist: loguru<0.7.0,>=0.6.0
+Requires-Dist: nest-asyncio<2.0.0,>=1.5.6
 Requires-Dist: orjson<4.0.0,>=3.8.5
 Requires-Dist: pydantic<2.0.0,>=1.10.5
 Requires-Dist: rich<14.0.0,>=13.3.1
-Requires-Dist: sqlalchemy<2.0.10,>=2.0.8
+Requires-Dist: sqlalchemy<2.1,>=2.0.8
 Provides-Extra: all
 Requires-Dist: databasez[mysql,postgresql,sqlite]; extra == 'all'
+Requires-Dist: ipython<9.0.0,>=8.10.0; extra == 'all'
 Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'all'
+Requires-Dist: ptpython<4.0.0,>=3.0.23; extra == 'all'
 Requires-Dist: pydantic<2.0.0,>=1.10.4; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
 Requires-Dist: flake8>=5.0.4; extra == 'dev'
 Requires-Dist: loguru<0.7.0,>=0.6.0; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: uvicorn[standard]>=0.19.0; extra == 'dev'
@@ -59,22 +63,25 @@
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
 Requires-Dist: mkdocs-material==9.1.5; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.4.2; extra == 'doc'
 Requires-Dist: mkdocstrings<0.21.0,>=0.19.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc'
+Provides-Extra: ipython
+Requires-Dist: ipython<9.0.0,>=8.10.0; extra == 'ipython'
 Provides-Extra: mysql
 Requires-Dist: databasez[mysql]; extra == 'mysql'
 Provides-Extra: postgres
-Requires-Dist: databasez[postgresql]; extra == 'postgres'
+Requires-Dist: databasez[postgressql]; extra == 'postgres'
+Provides-Extra: ptpython
+Requires-Dist: ptpython<4.0.0,>=3.0.23; extra == 'ptpython'
 Provides-Extra: sqlite
 Requires-Dist: databasez[sqlite]; extra == 'sqlite'
 Provides-Extra: test
-Requires-Dist: anyio<4,>=3.0.0; extra == 'test'
 Requires-Dist: asyncmy<0.3.0,>=0.2.7; extra == 'test'
 Requires-Dist: asyncpg<1,>=0.27.0; extra == 'test'
 Requires-Dist: black==23.3.0; extra == 'test'
 Requires-Dist: esmerald>=1.1.0; extra == 'test'
 Requires-Dist: flake8>=5.0.4; extra == 'test'
 Requires-Dist: freezegun<2.0.0,>=1.2.2; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
```

