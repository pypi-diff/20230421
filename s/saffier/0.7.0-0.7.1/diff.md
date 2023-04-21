# Comparing `tmp/saffier-0.7.0.tar.gz` & `tmp/saffier-0.7.1.tar.gz`

## Comparing `saffier-0.7.0.tar` & `saffier-0.7.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/exceptions.py
--rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/fields.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/metaclass.py
--rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/models.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/py.typed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/testclient.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/types.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/conf/enums.py
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/conf/functional.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/conf/global_settings.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/conf/module_import.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/__init__.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/base.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/datastructures.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/events.py
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/formats.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/registry.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/schemas.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/sync.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/unique.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/terminal/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/terminal/base.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/terminal/print.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/core/terminal/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/connection.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/constants.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/datastructures.py
--rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/fields.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/manager.py
--rw-r--r--   0        0        0    23146 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/queryset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/query/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/db/query/protocols.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/__init__.py
--rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/base.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/cli.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/constants.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/decorators.py
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/env.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/branches.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/check.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/current.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/downgrade.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/edit.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/heads.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/history.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/init.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/list_templates.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/makemigrations.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/merge.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/migrate.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/revision.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/show.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/stamp.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/__init__.py
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/enums.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/ipython.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/ptpython.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/operations/shell/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/templates/default/README
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/templates/default/alembic.ini.mako
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/templates/default/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/migrations/templates/default/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/sqlalchemy/fields.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/sqlalchemy/protocols.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.7.0/saffier/sqlalchemy/types.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.7.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.7.0/LICENSE
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.7.0/README.md
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 saffier-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 saffier-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/exceptions.py
+-rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/fields.py
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/metaclass.py
+-rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/models.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/py.typed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/testclient.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/types.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/conf/enums.py
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/conf/functional.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/conf/global_settings.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/conf/module_import.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/__init__.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/base.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/datastructures.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/events.py
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/formats.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/registry.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/schemas.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/sync.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/unique.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/terminal/base.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/terminal/print.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/core/terminal/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/db/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/db/connection.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/db/constants.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/db/datastructures.py
+-rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/db/fields.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/db/manager.py
+-rw-r--r--   0        0        0    23146 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/db/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/db/query/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/db/query/protocols.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/__init__.py
+-rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/base.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/cli.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/constants.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/decorators.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/env.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/branches.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/check.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/current.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/downgrade.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/edit.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/heads.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/history.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/init.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/list_templates.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/makemigrations.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/merge.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/migrate.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/revision.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/show.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/stamp.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/shell/enums.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/operations/shell/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/templates/default/README
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/templates/default/alembic.ini.mako
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/templates/default/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/migrations/templates/default/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/sqlalchemy/fields.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/sqlalchemy/protocols.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.7.1/saffier/sqlalchemy/types.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.7.1/README.md
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 saffier-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 saffier-0.7.1/PKG-INFO
```

### Comparing `saffier-0.7.0/saffier/__init__.py` & `saffier-0.7.1/saffier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 from saffier.conf import settings
 from saffier.conf.global_settings import SaffierSettings
 
 from .core.registry import Registry
 from .db.connection import Database
 from .db.constants import CASCADE, RESTRICT, SET_NULL
```

### Comparing `saffier-0.7.0/saffier/exceptions.py` & `saffier-0.7.1/saffier/exceptions.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/fields.py` & `saffier-0.7.1/saffier/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/metaclass.py` & `saffier-0.7.1/saffier/metaclass.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/models.py` & `saffier-0.7.1/saffier/models.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/conf/__init__.py` & `saffier-0.7.1/saffier/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/conf/functional.py` & `saffier-0.7.1/saffier/conf/functional.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/conf/global_settings.py` & `saffier-0.7.1/saffier/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/conf/module_import.py` & `saffier-0.7.1/saffier/conf/module_import.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/base.py` & `saffier-0.7.1/saffier/core/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/datastructures.py` & `saffier-0.7.1/saffier/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/events.py` & `saffier-0.7.1/saffier/core/events.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/formats.py` & `saffier-0.7.1/saffier/core/formats.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/registry.py` & `saffier-0.7.1/saffier/core/registry.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/schemas.py` & `saffier-0.7.1/saffier/core/schemas.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/sync.py` & `saffier-0.7.1/saffier/core/sync.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/unique.py` & `saffier-0.7.1/saffier/core/unique.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/utils.py` & `saffier-0.7.1/saffier/core/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/terminal/base.py` & `saffier-0.7.1/saffier/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/terminal/print.py` & `saffier-0.7.1/saffier/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/core/terminal/terminal.py` & `saffier-0.7.1/saffier/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/db/datastructures.py` & `saffier-0.7.1/saffier/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/db/fields.py` & `saffier-0.7.1/saffier/db/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/db/manager.py` & `saffier-0.7.1/saffier/db/manager.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/db/queryset.py` & `saffier-0.7.1/saffier/db/queryset.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/db/query/protocols.py` & `saffier-0.7.1/saffier/db/query/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/base.py` & `saffier-0.7.1/saffier/migrations/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/cli.py` & `saffier-0.7.1/saffier/migrations/cli.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/env.py` & `saffier-0.7.1/saffier/migrations/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/__init__.py` & `saffier-0.7.1/saffier/migrations/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/branches.py` & `saffier-0.7.1/saffier/migrations/operations/branches.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/current.py` & `saffier-0.7.1/saffier/migrations/operations/current.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/downgrade.py` & `saffier-0.7.1/saffier/migrations/operations/downgrade.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/heads.py` & `saffier-0.7.1/saffier/migrations/operations/heads.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/history.py` & `saffier-0.7.1/saffier/migrations/operations/history.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/init.py` & `saffier-0.7.1/saffier/migrations/operations/init.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/makemigrations.py` & `saffier-0.7.1/saffier/migrations/operations/makemigrations.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/merge.py` & `saffier-0.7.1/saffier/migrations/operations/merge.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/migrate.py` & `saffier-0.7.1/saffier/migrations/operations/migrate.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/revision.py` & `saffier-0.7.1/saffier/migrations/operations/revision.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/stamp.py` & `saffier-0.7.1/saffier/migrations/operations/stamp.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/shell/base.py` & `saffier-0.7.1/saffier/migrations/operations/shell/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         sys.platform != "win32"
         and not sys.stdin.isatty()
         and select.select([sys.stdin], [], [], 0)[0]
     ):
         exec(sys.stdin.read(), globals())
         return
 
-    on_startup = getattr(env.app, "on_startup", None)
-    on_shutdown = getattr(env.app, "on_shutdown", None)
+    on_startup = getattr(env.app, "on_startup", [])
+    on_shutdown = getattr(env.app, "on_shutdown", [])
     lifespan = getattr(env.app, "lifespan", None)
     lifespan = handle_lifespan_events(
         on_startup=on_startup, on_shutdown=on_shutdown, lifespan=lifespan
     )
     execsync(run_shell)(env.app, lifespan, registry, kernel)
     return None
 
@@ -69,12 +69,10 @@
     lifespan: Optional[Any] = None,
 ) -> Any:
     """Handles with the lifespan events in the new Starlette format of lifespan.
     This adds a mask that keeps the old `on_startup` and `on_shutdown` events variable
     declaration for legacy and comprehension purposes and build the async context manager
     for the lifespan.
     """
-    if on_startup or on_shutdown:
-        return AyncLifespanContextManager(on_startup=on_startup, on_shutdown=on_shutdown)
-    elif lifespan:
+    if lifespan:
         return lifespan
-    return None
+    return AyncLifespanContextManager(on_startup=on_startup, on_shutdown=on_shutdown)
```

### Comparing `saffier-0.7.0/saffier/migrations/operations/shell/ipython.py` & `saffier-0.7.1/saffier/migrations/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/shell/ptpython.py` & `saffier-0.7.1/saffier/migrations/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/operations/shell/utils.py` & `saffier-0.7.1/saffier/migrations/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/templates/default/alembic.ini.mako` & `saffier-0.7.1/saffier/migrations/templates/default/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/migrations/templates/default/env.py` & `saffier-0.7.1/saffier/migrations/templates/default/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/sqlalchemy/fields.py` & `saffier-0.7.1/saffier/sqlalchemy/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/saffier/sqlalchemy/protocols.py` & `saffier-0.7.1/saffier/sqlalchemy/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/LICENSE` & `saffier-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/README.md` & `saffier-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/pyproject.toml` & `saffier-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `saffier-0.7.0/PKG-INFO` & `saffier-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saffier
-Version: 0.7.0
+Version: 0.7.1
 Summary: The only python ORM you will ever need.
 Project-URL: Homepage, https://github.com/tarsil/saffier
 Project-URL: Documentation, https://saffier.tarsild.io/
 Project-URL: Changelog, https://saffier.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/saffier
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
```

