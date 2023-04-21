# Comparing `tmp/psycopg2_mq-0.8.3.tar.gz` & `tmp/psycopg2_mq-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg2_mq-0.8.3.tar", last modified: Fri Apr 15 17:48:31 2022, max compression
+gzip compressed data, was "psycopg2_mq-0.9.tar", last modified: Fri Apr 21 16:15:01 2023, max compression
```

## Comparing `psycopg2_mq-0.8.3.tar` & `psycopg2_mq-0.9.tar`

### file list

```diff
@@ -1,25 +1,37 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-04-15 17:48:31.519083 psycopg2_mq-0.8.3/
--rw-r--r--   0 michael    (501) staff       (20)      171 2018-09-05 00:46:14.000000 psycopg2_mq-0.8.3/.coveragerc
--rw-r--r--   0 michael    (501) staff       (20)     8124 2022-04-15 17:47:34.000000 psycopg2_mq-0.8.3/CHANGES.rst
--rw-r--r--   0 michael    (501) staff       (20)     1060 2018-09-05 00:49:01.000000 psycopg2_mq-0.8.3/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)      180 2020-12-22 17:29:25.000000 psycopg2_mq-0.8.3/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)    13192 2022-04-15 17:48:31.519284 psycopg2_mq-0.8.3/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     4251 2021-01-09 21:29:18.000000 psycopg2_mq-0.8.3/README.rst
--rw-r--r--   0 michael    (501) staff       (20)      380 2022-04-15 17:48:31.520236 psycopg2_mq-0.8.3/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1465 2022-04-15 17:48:14.000000 psycopg2_mq-0.8.3/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-04-15 17:48:31.512686 psycopg2_mq-0.8.3/src/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-04-15 17:48:31.516459 psycopg2_mq-0.8.3/src/psycopg2_mq/
--rw-r--r--   0 michael    (501) staff       (20)      146 2022-04-15 16:26:28.000000 psycopg2_mq-0.8.3/src/psycopg2_mq/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     5002 2022-04-15 17:22:06.000000 psycopg2_mq-0.8.3/src/psycopg2_mq/model.py
--rw-r--r--   0 michael    (501) staff       (20)    10826 2022-04-15 16:50:21.000000 psycopg2_mq-0.8.3/src/psycopg2_mq/source.py
--rw-r--r--   0 michael    (501) staff       (20)      476 2021-01-09 21:24:33.000000 psycopg2_mq-0.8.3/src/psycopg2_mq/trigger.py
--rw-r--r--   0 michael    (501) staff       (20)     2302 2021-03-01 00:11:20.000000 psycopg2_mq-0.8.3/src/psycopg2_mq/util.py
--rw-r--r--   0 michael    (501) staff       (20)    28524 2022-04-15 17:47:48.000000 psycopg2_mq-0.8.3/src/psycopg2_mq/worker.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-04-15 17:48:31.518860 psycopg2_mq-0.8.3/src/psycopg2_mq.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    13192 2022-04-15 17:48:31.000000 psycopg2_mq-0.8.3/src/psycopg2_mq.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      473 2022-04-15 17:48:31.000000 psycopg2_mq-0.8.3/src/psycopg2_mq.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2022-04-15 17:48:31.000000 psycopg2_mq-0.8.3/src/psycopg2_mq.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2018-09-05 01:36:30.000000 psycopg2_mq-0.8.3/src/psycopg2_mq.egg-info/not-zip-safe
--rw-r--r--   0 michael    (501) staff       (20)       88 2022-04-15 17:48:31.000000 psycopg2_mq-0.8.3/src/psycopg2_mq.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       12 2022-04-15 17:48:31.000000 psycopg2_mq-0.8.3/src/psycopg2_mq.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)      532 2022-04-15 16:08:13.000000 psycopg2_mq-0.8.3/tox.ini
+drwxr-xr-x   0 michael    (502) staff       (20)        0 2023-04-21 16:15:01.856115 psycopg2_mq-0.9/
+-rw-r--r--   0 michael    (502) staff       (20)      171 2022-02-25 01:23:06.000000 psycopg2_mq-0.9/.coveragerc
+-rw-r--r--   0 michael    (502) staff       (20)      373 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/.flake8
+drwxr-xr-x   0 michael    (502) staff       (20)        0 2023-04-21 16:15:01.853728 psycopg2_mq-0.9/.github/
+-rw-r--r--   0 michael    (502) staff       (20)      218 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/.github/dependabot.yml
+drwxr-xr-x   0 michael    (502) staff       (20)        0 2023-04-21 16:15:01.853850 psycopg2_mq-0.9/.github/workflows/
+-rw-r--r--   0 michael    (502) staff       (20)     2314 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/.github/workflows/ci-tests.yml
+-rw-r--r--   0 michael    (502) staff       (20)     8844 2023-04-21 16:12:22.000000 psycopg2_mq-0.9/CHANGES.rst
+-rw-r--r--   0 michael    (502) staff       (20)     1060 2022-02-25 01:23:06.000000 psycopg2_mq-0.9/LICENSE.txt
+-rw-r--r--   0 michael    (502) staff       (20)      252 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/MANIFEST.in
+-rw-r--r--   0 michael    (502) staff       (20)    14432 2023-04-21 16:15:01.856197 psycopg2_mq-0.9/PKG-INFO
+-rw-r--r--   0 michael    (502) staff       (20)     4642 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/README.rst
+-rw-r--r--   0 michael    (502) staff       (20)      607 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/pyproject.toml
+-rw-r--r--   0 michael    (502) staff       (20)       96 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/pytest.ini
+-rw-r--r--   0 michael    (502) staff       (20)     1244 2023-04-21 16:15:01.856602 psycopg2_mq-0.9/setup.cfg
+-rw-r--r--   0 michael    (502) staff       (20)       38 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/setup.py
+drwxr-xr-x   0 michael    (502) staff       (20)        0 2023-04-21 16:15:01.852039 psycopg2_mq-0.9/src/
+drwxr-xr-x   0 michael    (502) staff       (20)        0 2023-04-21 16:15:01.854584 psycopg2_mq-0.9/src/psycopg2_mq/
+-rw-r--r--   0 michael    (502) staff       (20)      127 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/src/psycopg2_mq/__init__.py
+-rw-r--r--   0 michael    (502) staff       (20)     5009 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/src/psycopg2_mq/model.py
+-rw-r--r--   0 michael    (502) staff       (20)    11746 2023-04-21 15:59:05.000000 psycopg2_mq-0.9/src/psycopg2_mq/source.py
+-rw-r--r--   0 michael    (502) staff       (20)      613 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/src/psycopg2_mq/trigger.py
+-rw-r--r--   0 michael    (502) staff       (20)     2232 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/src/psycopg2_mq/util.py
+-rw-r--r--   0 michael    (502) staff       (20)    28645 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/src/psycopg2_mq/worker.py
+drwxr-xr-x   0 michael    (502) staff       (20)        0 2023-04-21 16:15:01.855498 psycopg2_mq-0.9/src/psycopg2_mq.egg-info/
+-rw-r--r--   0 michael    (502) staff       (20)    14432 2023-04-21 16:15:01.000000 psycopg2_mq-0.9/src/psycopg2_mq.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (502) staff       (20)      645 2023-04-21 16:15:01.000000 psycopg2_mq-0.9/src/psycopg2_mq.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (502) staff       (20)        1 2023-04-21 16:15:01.000000 psycopg2_mq-0.9/src/psycopg2_mq.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (502) staff       (20)        1 2022-02-25 01:23:17.000000 psycopg2_mq-0.9/src/psycopg2_mq.egg-info/not-zip-safe
+-rw-r--r--   0 michael    (502) staff       (20)      144 2023-04-21 16:15:01.000000 psycopg2_mq-0.9/src/psycopg2_mq.egg-info/requires.txt
+-rw-r--r--   0 michael    (502) staff       (20)       12 2023-04-21 16:15:01.000000 psycopg2_mq-0.9/src/psycopg2_mq.egg-info/top_level.txt
+drwxr-xr-x   0 michael    (502) staff       (20)        0 2023-04-21 16:15:01.856001 psycopg2_mq-0.9/tests/
+-rw-r--r--   0 michael    (502) staff       (20)     1671 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/tests/conftest.py
+-rw-r--r--   0 michael    (502) staff       (20)     1909 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/tests/test_integration.py
+-rw-r--r--   0 michael    (502) staff       (20)     1971 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/tests/test_source.py
+-rw-r--r--   0 michael    (502) staff       (20)      305 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/tests/test_util.py
+-rw-r--r--   0 michael    (502) staff       (20)     1307 2023-04-21 15:49:31.000000 psycopg2_mq-0.9/tox.ini
```

### Comparing `psycopg2_mq-0.8.3/CHANGES.rst` & `psycopg2_mq-0.9/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,57 @@
+Changes
+=======
+
+0.9 (2023-04-21)
+----------------
+
+- Add support for Python 3.10, and 3.11.
+
+- [breaking] Prevent retrying of collapsible jobs. Require them to be invoked
+  using ``call`` instead for an opportunity to specify a ``conflict_resolver``.
+
+- Fix a bug in the default model schema in which the collapsible database
+  index was not marked unique.
+
+- Copy trace info when retrying a job.
+
+- Capture the stringified exception to the job result in the ``message`` key,
+  alongside the existing ``tb``, ``exc``, and ``args`` keys.
+
+- The worker was not recognizing ``capture_signals=False``, causing problems
+  when running the event loop in other threads.
+
+- Blackify the codebase and add some real tests. Yay!
+
 0.8.3 (2022-04-15)
-==================
+------------------
 
 - [breaking] Remove ``MQWorker.make_job_context``.
 
 0.8.2 (2022-04-15)
-==================
+------------------
 
 - Drop Python 3.6 support.
 
 - [breaking] Require SQLAlchemy 1.4+ and resolve deprecation warnings related to
   SQLAlchemy 2.0.
 
 - [breaking] Rename ``update_job_id`` to ``updated_job_id`` in the
   ``JobCursor`` model.
 
 0.8.1 (2022-04-15)
-==================
+------------------
 
 - Ensure the ``trace`` attribute is populated on the ``JobContext``.
 
 - Add ``MQWorker.make_job_context`` which can be defined to completely override
   the ``JobContext`` factory using the ``Job`` object and open database session.
 
 0.8.0 (2022-04-15)
-==================
+------------------
 
 - [breaking] Add ``update_job_id`` foreign key to the ``JobCursor`` model to
   make it possible to know which job last updated the value in the cursor.
 
 - [breaking] Add ``trace`` json blob to the ``Job`` model.
 
 - Support a ``trace`` json blob when creating new jobs. This value is available
@@ -38,142 +62,142 @@
   See ``JobContext.trace`` attribute when handling jobs.
 
 - Add a standard ``FailedJobError`` exception which can be raised by jobs to
   mark a failure with a custom result object. This is different from unhandled
   exceptions that cause the ``MQWorker.result_from_error`` method to be invoked.
 
 0.7.0 (2022-03-03)
-==================
+------------------
 
 - Fix a corner case with lost jobs attached to cursors. In scenarios where
   multiple workers are running, if one loses a database connection then the
   other is designed to notice and mark jobs lost. However, it's possible the
   job is not actually lost and the worker can then recover after resuming
   its connection, and marking the job running again. In this situation, we
   do not want another job to begin on the same cursor. To fix this issue,
   new jobs will not be run if another job is marked lost on the same cursor.
   You will be required to recover the job by marking it as not lost (probably
   failed) first to unblock the rest of the jobs on the cursor.
 
 0.6.2 (2022-03-01)
-==================
+------------------
 
 - Prioritize maintenance work higher than running new jobs.
   There was a chicken-and-egg issue where a job would be marked running
   but needs to be marked lost. However marking it lost is lower priority than
   trying to start new jobs. In the case where a lot of jobs were scheduled
   at the same time, the worker always tried to start new jobs and didn't
   run the maintenance so the job never got marked lost, effectively blocking
   the queue.
 
 0.6.1 (2022-01-15)
-==================
+------------------
 
 - Fix a bug introduced in the 0.6.0 release when scheduling new jobs.
 
 0.6.0 (2022-01-14)
-==================
+------------------
 
 - [breaking] Add model changes to mark jobs as collapsible.
 
 - [breaking] Add model changes to the cursor index.
 
 - Allow multiple pending jobs to be scheduled on the same cursor if either:
 
   1. The queue or method are different from existing pending jobs on the cursor.
 
   2. ``collapse_on_cursor`` is set to ``False`` when scheduling the job.
 
 0.5.7 (2021-03-07)
-==================
+------------------
 
 - Add a ``schedule_id`` attribute to the job context for use in jobs that want
   to know whether they were executed from a schedule or not.
 
 0.5.6 (2021-02-28)
-==================
+------------------
 
 - Some UnicodeDecodeError exceptions raised from jobs could trigger a
   serialization failure (UntranslatableCharacter) because it would contain
   the sequence ``\u0000``` which, while valid in Python, is not allowed
   in postgres. So when dealing with the raw bytes, we'll decode it with
   the replacement character that can be properly stored. Not ideal, but
   better than failing to store the error at all.
 
 0.5.5 (2021-01-22)
-==================
+------------------
 
 - Fixed some old code causing the worker lock to release after a job
   completed.
 
 0.5.4 (2021-01-20)
-==================
+------------------
 
 - Log at the error level when marking a job as lost.
 
 0.5.3 (2021-01-11)
-==================
+------------------
 
 - Copy the ``schedule_id`` information to retried jobs.
 
 0.5.2 (2021-01-11)
-==================
+------------------
 
 - [breaking] Require ``call_schedule`` to accept an id instead of an object.
 
 0.5.1 (2021-01-09)
-==================
+------------------
 
 - Drop the ``UNIQUE`` constraint on the background job ``lock_id`` column.
 
 0.5 (2021-01-09)
-================
+----------------
 
 - Add a scheduler model with support for emitting periodic jobs based on
   RRULE syntax.
   See https://github.com/mmerickel/psycopg2_mq/pull/11
 
 - Enable the workers to coordinate on a per-queue basis who is in control
   of scheduling jobs.
   See https://github.com/mmerickel/psycopg2_mq/pull/12
 
 - Reduce the number of advisory locks held from one per job to one per worker.
   See https://github.com/mmerickel/psycopg2_mq/pull/12
 
 0.4.5 (2020-12-22)
-==================
+------------------
 
 - Use column objects in the insert statement to support ORM-level synonyms,
   enabling the schema to have columns with different names.
 
 0.4.4 (2019-11-07)
-==================
+------------------
 
 - Ensure the advisory locks are released when a job completes.
 
 0.4.3 (2019-10-31)
-==================
+------------------
 
 - Ensure maintenance (finding lost jobs) always runs at set intervals defined
   by the ``timeout`` parameter.
 
 0.4.2 (2019-10-30)
-==================
+------------------
 
 - Recover active jobs when the connection is lost by re-locking them
   and ensuring they are marked running.
 
 0.4.1 (2019-10-30)
-==================
+------------------
 
 - Attempt to reconnect to the database after losing the connection.
   If the reconnect attempt fails then crash.
 
 0.4 (2019-10-28)
-================
+----------------
 
 - Add a ``worker`` column to the ``Job`` model to track what worker
   is handling a job.
 
 - Add an optional ``name`` argument to ``MQWorker`` to name the worker -
   the value will be recorded in each job.
 
@@ -184,77 +208,77 @@
 - Add ``capture_signals`` argument (default=``True``) to ``MQWorker`` which
   will capture ``SIGTERM``, ``SIGINT`` and ``SIGUSR1``. The first two will
   trigger graceful shutdown - they will make the process stop handling new
   jobs while finishing active jobs. The latter will dump to ``stderr`` a
   JSON dump of the current status of the worker.
 
 0.3.3 (2019-10-23)
-==================
+------------------
 
 - Only save a cursor update if the job is completed successfully.
 
 0.3.2 (2019-10-22)
-==================
+------------------
 
 - Mark lost jobs during timeouts instead of just when a worker starts in order
   to catch them earlier.
 
 0.3.1 (2019-10-17)
-==================
+------------------
 
 - When attempting to schedule a job with a cursor and a ``scheduled_time``
   earlier than a pending job on the same cursor, the job will be updated to
   run at the earlier time.
 
 - When attempting to schedule a job with a cursor and a pending job already
   exists on the same cursor, a ``conflict_resolver`` function may be
   supplied to ``MQSource.call`` to update the job properties, merging the
   arguments however the user wishes.
 
 0.3 (2019-10-15)
-================
+----------------
 
 - Add a new column ``cursor_snapshot`` to the ``Job`` model which will
   contain the value of the cursor when the job begins.
 
 0.2 (2019-10-09)
-================
+----------------
 
 - Add cursor support for jobs. This requires a schema migration to add
   a ``cursor_key`` column, a new ``JobCursor`` model, and some new indices.
 
 0.1.6 (2019-10-07)
-==================
+------------------
 
 - Support passing custom kwargs to the job in ``psycopg2_mq.MQSource.call``
   to allow custom columns on the job table.
 
 0.1.5 (2019-05-17)
-==================
+------------------
 
 - Fix a regression when serializing errors with strings or cycles.
 
 0.1.4 (2019-05-09)
-==================
+------------------
 
 - More safely serialize exception objects when jobs fail.
 
 0.1.3 (2018-09-04)
-==================
+------------------
 
 - Rename the thread to contain the job id while it's handling a job.
 
 0.1.2 (2018-09-04)
-==================
+------------------
 
 - Rename ``Job.params`` to ``Job.args``.
 
 0.1.1 (2018-09-04)
-==================
+------------------
 
 - Make ``psycopg2`` an optional dependency in order to allow apps to depend
   on ``psycopg2-binary`` if they wish.
 
 0.1 (2018-09-04)
-================
+----------------
 
 - Initial release.
```

### Comparing `psycopg2_mq-0.8.3/LICENSE.txt` & `psycopg2_mq-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psycopg2_mq-0.8.3/PKG-INFO` & `psycopg2_mq-0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: psycopg2_mq
-Version: 0.8.3
+Version: 0.9
 Summary: A message queue written around PostgreSQL.
 Home-page: https://github.com/mmerickel/psycopg2_mq
 Author: Michael Merickel
 Author-email: oss@m.merickel.org
-License: UNKNOWN
-Keywords: psycopg2,postgres,postgresql
-Platform: UNKNOWN
+Keywords: psycopg2,postgres,postgresql,message queue,background jobs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 ===========
 psycopg2_mq
 ===========
 
 .. image:: https://img.shields.io/pypi/v/psycopg2_mq.svg
     :target: https://pypi.org/pypi/psycopg2_mq
 
+.. image:: https://github.com/mmerickel/psycopg2_mq/workflows/Build%20and%20test/badge.svg?branch=main
+    :target: https://github.com/mmerickel/psycopg2_mq/actions?query=workflow%3A%22Build+and+test%22
+    :alt: main CI Status
+
 ``psycopg2_mq`` is a message queue implemented on top of
 `PostgreSQL <https://www.postgresql.org/>`__,
 `SQLAlchemy <https://www.sqlalchemy.org/>`__, and
 `psycopg2 <http://initd.org/psycopg/>`__.
 
 Currently the library provides only the low-level constructs that can be used
 to build a multithreaded worker system. It is broken into two components:
@@ -40,14 +45,18 @@
   single-threaded worker that can accept jobs and execute them. An application
   should create worker per thread. It supports an API for thread-safe graceful
   shutdown.
 
 - ``psycopg2_mq.MQSource`` - a source object providing a client-side API for
   invoking and querying job states.
 
+It is expected that these core components are then wrapped into your own
+application in any way that you see fit, without dictating a specific CLI
+or framework.
+
 Data Model
 ==========
 
 Queues
 ------
 
 Workers run jobs defined in queues. Currently each queue will run jobs
@@ -155,41 +164,64 @@
         mq = MQSource(
             dbsession=dbsession,
             model=model,
         )
         job = mq.call('echo', 'hello', {'name': 'Andy'})
         print(f'queued job={job.id}')
 
+Changes
+=======
+
+0.9 (2023-04-21)
+----------------
+
+- Add support for Python 3.10, and 3.11.
+
+- [breaking] Prevent retrying of collapsible jobs. Require them to be invoked
+  using ``call`` instead for an opportunity to specify a ``conflict_resolver``.
+
+- Fix a bug in the default model schema in which the collapsible database
+  index was not marked unique.
+
+- Copy trace info when retrying a job.
+
+- Capture the stringified exception to the job result in the ``message`` key,
+  alongside the existing ``tb``, ``exc``, and ``args`` keys.
+
+- The worker was not recognizing ``capture_signals=False``, causing problems
+  when running the event loop in other threads.
+
+- Blackify the codebase and add some real tests. Yay!
 
 0.8.3 (2022-04-15)
-==================
+------------------
 
 - [breaking] Remove ``MQWorker.make_job_context``.
 
 0.8.2 (2022-04-15)
-==================
+------------------
 
 - Drop Python 3.6 support.
 
 - [breaking] Require SQLAlchemy 1.4+ and resolve deprecation warnings related to
   SQLAlchemy 2.0.
 
 - [breaking] Rename ``update_job_id`` to ``updated_job_id`` in the
   ``JobCursor`` model.
 
 0.8.1 (2022-04-15)
-==================
+------------------
 
 - Ensure the ``trace`` attribute is populated on the ``JobContext``.
 
 - Add ``MQWorker.make_job_context`` which can be defined to completely override
   the ``JobContext`` factory using the ``Job`` object and open database session.
 
 0.8.0 (2022-04-15)
-==================
+------------------
 
 - [breaking] Add ``update_job_id`` foreign key to the ``JobCursor`` model to
   make it possible to know which job last updated the value in the cursor.
 
 - [breaking] Add ``trace`` json blob to the ``Job`` model.
 
 - Support a ``trace`` json blob when creating new jobs. This value is available
@@ -200,142 +232,142 @@
   See ``JobContext.trace`` attribute when handling jobs.
 
 - Add a standard ``FailedJobError`` exception which can be raised by jobs to
   mark a failure with a custom result object. This is different from unhandled
   exceptions that cause the ``MQWorker.result_from_error`` method to be invoked.
 
 0.7.0 (2022-03-03)
-==================
+------------------
 
 - Fix a corner case with lost jobs attached to cursors. In scenarios where
   multiple workers are running, if one loses a database connection then the
   other is designed to notice and mark jobs lost. However, it's possible the
   job is not actually lost and the worker can then recover after resuming
   its connection, and marking the job running again. In this situation, we
   do not want another job to begin on the same cursor. To fix this issue,
   new jobs will not be run if another job is marked lost on the same cursor.
   You will be required to recover the job by marking it as not lost (probably
   failed) first to unblock the rest of the jobs on the cursor.
 
 0.6.2 (2022-03-01)
-==================
+------------------
 
 - Prioritize maintenance work higher than running new jobs.
   There was a chicken-and-egg issue where a job would be marked running
   but needs to be marked lost. However marking it lost is lower priority than
   trying to start new jobs. In the case where a lot of jobs were scheduled
   at the same time, the worker always tried to start new jobs and didn't
   run the maintenance so the job never got marked lost, effectively blocking
   the queue.
 
 0.6.1 (2022-01-15)
-==================
+------------------
 
 - Fix a bug introduced in the 0.6.0 release when scheduling new jobs.
 
 0.6.0 (2022-01-14)
-==================
+------------------
 
 - [breaking] Add model changes to mark jobs as collapsible.
 
 - [breaking] Add model changes to the cursor index.
 
 - Allow multiple pending jobs to be scheduled on the same cursor if either:
 
   1. The queue or method are different from existing pending jobs on the cursor.
 
   2. ``collapse_on_cursor`` is set to ``False`` when scheduling the job.
 
 0.5.7 (2021-03-07)
-==================
+------------------
 
 - Add a ``schedule_id`` attribute to the job context for use in jobs that want
   to know whether they were executed from a schedule or not.
 
 0.5.6 (2021-02-28)
-==================
+------------------
 
 - Some UnicodeDecodeError exceptions raised from jobs could trigger a
   serialization failure (UntranslatableCharacter) because it would contain
   the sequence ``\u0000``` which, while valid in Python, is not allowed
   in postgres. So when dealing with the raw bytes, we'll decode it with
   the replacement character that can be properly stored. Not ideal, but
   better than failing to store the error at all.
 
 0.5.5 (2021-01-22)
-==================
+------------------
 
 - Fixed some old code causing the worker lock to release after a job
   completed.
 
 0.5.4 (2021-01-20)
-==================
+------------------
 
 - Log at the error level when marking a job as lost.
 
 0.5.3 (2021-01-11)
-==================
+------------------
 
 - Copy the ``schedule_id`` information to retried jobs.
 
 0.5.2 (2021-01-11)
-==================
+------------------
 
 - [breaking] Require ``call_schedule`` to accept an id instead of an object.
 
 0.5.1 (2021-01-09)
-==================
+------------------
 
 - Drop the ``UNIQUE`` constraint on the background job ``lock_id`` column.
 
 0.5 (2021-01-09)
-================
+----------------
 
 - Add a scheduler model with support for emitting periodic jobs based on
   RRULE syntax.
   See https://github.com/mmerickel/psycopg2_mq/pull/11
 
 - Enable the workers to coordinate on a per-queue basis who is in control
   of scheduling jobs.
   See https://github.com/mmerickel/psycopg2_mq/pull/12
 
 - Reduce the number of advisory locks held from one per job to one per worker.
   See https://github.com/mmerickel/psycopg2_mq/pull/12
 
 0.4.5 (2020-12-22)
-==================
+------------------
 
 - Use column objects in the insert statement to support ORM-level synonyms,
   enabling the schema to have columns with different names.
 
 0.4.4 (2019-11-07)
-==================
+------------------
 
 - Ensure the advisory locks are released when a job completes.
 
 0.4.3 (2019-10-31)
-==================
+------------------
 
 - Ensure maintenance (finding lost jobs) always runs at set intervals defined
   by the ``timeout`` parameter.
 
 0.4.2 (2019-10-30)
-==================
+------------------
 
 - Recover active jobs when the connection is lost by re-locking them
   and ensuring they are marked running.
 
 0.4.1 (2019-10-30)
-==================
+------------------
 
 - Attempt to reconnect to the database after losing the connection.
   If the reconnect attempt fails then crash.
 
 0.4 (2019-10-28)
-================
+----------------
 
 - Add a ``worker`` column to the ``Job`` model to track what worker
   is handling a job.
 
 - Add an optional ``name`` argument to ``MQWorker`` to name the worker -
   the value will be recorded in each job.
 
@@ -346,79 +378,77 @@
 - Add ``capture_signals`` argument (default=``True``) to ``MQWorker`` which
   will capture ``SIGTERM``, ``SIGINT`` and ``SIGUSR1``. The first two will
   trigger graceful shutdown - they will make the process stop handling new
   jobs while finishing active jobs. The latter will dump to ``stderr`` a
   JSON dump of the current status of the worker.
 
 0.3.3 (2019-10-23)
-==================
+------------------
 
 - Only save a cursor update if the job is completed successfully.
 
 0.3.2 (2019-10-22)
-==================
+------------------
 
 - Mark lost jobs during timeouts instead of just when a worker starts in order
   to catch them earlier.
 
 0.3.1 (2019-10-17)
-==================
+------------------
 
 - When attempting to schedule a job with a cursor and a ``scheduled_time``
   earlier than a pending job on the same cursor, the job will be updated to
   run at the earlier time.
 
 - When attempting to schedule a job with a cursor and a pending job already
   exists on the same cursor, a ``conflict_resolver`` function may be
   supplied to ``MQSource.call`` to update the job properties, merging the
   arguments however the user wishes.
 
 0.3 (2019-10-15)
-================
+----------------
 
 - Add a new column ``cursor_snapshot`` to the ``Job`` model which will
   contain the value of the cursor when the job begins.
 
 0.2 (2019-10-09)
-================
+----------------
 
 - Add cursor support for jobs. This requires a schema migration to add
   a ``cursor_key`` column, a new ``JobCursor`` model, and some new indices.
 
 0.1.6 (2019-10-07)
-==================
+------------------
 
 - Support passing custom kwargs to the job in ``psycopg2_mq.MQSource.call``
   to allow custom columns on the job table.
 
 0.1.5 (2019-05-17)
-==================
+------------------
 
 - Fix a regression when serializing errors with strings or cycles.
 
 0.1.4 (2019-05-09)
-==================
+------------------
 
 - More safely serialize exception objects when jobs fail.
 
 0.1.3 (2018-09-04)
-==================
+------------------
 
 - Rename the thread to contain the job id while it's handling a job.
 
 0.1.2 (2018-09-04)
-==================
+------------------
 
 - Rename ``Job.params`` to ``Job.args``.
 
 0.1.1 (2018-09-04)
-==================
+------------------
 
 - Make ``psycopg2`` an optional dependency in order to allow apps to depend
   on ``psycopg2-binary`` if they wish.
 
 0.1 (2018-09-04)
-================
+----------------
 
 - Initial release.
-
-
```

### Comparing `psycopg2_mq-0.8.3/README.rst` & `psycopg2_mq-0.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 ===========
 psycopg2_mq
 ===========
 
 .. image:: https://img.shields.io/pypi/v/psycopg2_mq.svg
     :target: https://pypi.org/pypi/psycopg2_mq
 
+.. image:: https://github.com/mmerickel/psycopg2_mq/workflows/Build%20and%20test/badge.svg?branch=main
+    :target: https://github.com/mmerickel/psycopg2_mq/actions?query=workflow%3A%22Build+and+test%22
+    :alt: main CI Status
+
 ``psycopg2_mq`` is a message queue implemented on top of
 `PostgreSQL <https://www.postgresql.org/>`__,
 `SQLAlchemy <https://www.sqlalchemy.org/>`__, and
 `psycopg2 <http://initd.org/psycopg/>`__.
 
 Currently the library provides only the low-level constructs that can be used
 to build a multithreaded worker system. It is broken into two components:
@@ -17,14 +21,18 @@
   single-threaded worker that can accept jobs and execute them. An application
   should create worker per thread. It supports an API for thread-safe graceful
   shutdown.
 
 - ``psycopg2_mq.MQSource`` - a source object providing a client-side API for
   invoking and querying job states.
 
+It is expected that these core components are then wrapped into your own
+application in any way that you see fit, without dictating a specific CLI
+or framework.
+
 Data Model
 ==========
 
 Queues
 ------
 
 Workers run jobs defined in queues. Currently each queue will run jobs
```

### Comparing `psycopg2_mq-0.8.3/src/psycopg2_mq/model.py` & `psycopg2_mq-0.9/src/psycopg2_mq/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 import sqlalchemy as sa
 from sqlalchemy.dialects import postgresql as pg
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import relationship
-from sqlalchemy.schema import Column, CheckConstraint, ForeignKey, Index
-from sqlalchemy.types import (
-    BigInteger,
-    Boolean,
-    DateTime,
-    Enum,
-    Integer,
-    Text,
-)
+from sqlalchemy.schema import CheckConstraint, Column, ForeignKey, Index
+from sqlalchemy.types import BigInteger, Boolean, DateTime, Enum, Integer, Text
 
 
 class Model:
     channel_prefix = 'mq_'
 
     def __init__(self, Job, JobStates, JobCursor, JobSchedule, Lock):
         self.Job = Job
@@ -39,15 +32,15 @@
     state_enum = Enum(
         JobStates.PENDING,
         JobStates.RUNNING,
         JobStates.COMPLETED,
         JobStates.FAILED,
         JobStates.LOST,
         metadata=metadata,
-        name='mq_job_state'
+        name='mq_job_state',
     )
 
     class Job(Base):
         __tablename__ = 'mq_job'
 
         id = Column(BigInteger, primary_key=True)
         start_time = Column(DateTime)
@@ -83,19 +76,22 @@
                     state != JobStates.RUNNING,
                     lock_id != sa.null(),
                 ),
                 name='ck_mq_job_lock_id',
             ),
             Index(
                 'uq_mq_job_pending_cursor_key_queue_method',
-                cursor_key, queue, method,
+                cursor_key,
+                queue,
+                method,
                 postgresql_where=sa.and_(
                     state == JobStates.PENDING,
                     collapsible == sa.true(),
                 ),
+                unique=True,
             ),
             Index(
                 'uq_mq_job_running_cursor_key',
                 cursor_key,
                 postgresql_where=state == JobStates.RUNNING,
                 unique=True,
             ),
@@ -120,15 +116,15 @@
         properties = Column(pg.JSONB, default=dict, nullable=False)
 
         updated_job_id = Column(
             ForeignKey('mq_job.id', ondelete='set null', onupdate='cascade'),
         )
 
         def __repr__(self):
-            return '<JobCursor(key="{0.key}")>'.format(self)
+            return f'<JobCursor(key="{self.key}")>'
 
     class JobSchedule(Base):
         __tablename__ = 'mq_job_schedule'
 
         id = Column(BigInteger, primary_key=True)
 
         created_time = Column(DateTime, nullable=False)
@@ -151,16 +147,15 @@
             return (
                 '<JobSchedule('
                 'queue="{0.queue}"'
                 ', method="{0.method}"'
                 ', rrule="{0.rrule}"'
                 ', cursor_key="{0.cursor_key}"'
                 ', is_enabled={0.is_enabled}'
-                '>'
-                .format(self)
+                '>'.format(self)
             )
 
     class Lock(Base):
         __tablename__ = 'mq_lock'
 
         queue = Column(Text, primary_key=True)
         key = Column(Text, primary_key=True)
```

### Comparing `psycopg2_mq-0.8.3/src/psycopg2_mq/source.py` & `psycopg2_mq-0.9/src/psycopg2_mq/source.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import json
 import sqlalchemy as sa
 from sqlalchemy.dialects.postgresql import insert
 from zope.sqlalchemy import mark_changed
 
 from .util import datetime_to_int, get_next_rrule_time
 
-
 log = __import__('logging').getLogger(__name__)
 
 
 class MQSource:
     def __init__(
         self,
         *,
@@ -30,15 +29,15 @@
         *,
         when=None,
         now=None,
         cursor_key=None,
         job_kwargs=None,
         conflict_resolver=None,
         schedule_id=None,
-        collapse_on_cursor=True,
+        collapse_on_cursor=None,
         trace=None,
     ):
         """
         Dispatch a new job.
 
         :param conflict_resolver:
             A callable that accepts the old job as its only argument. This will
@@ -49,70 +48,84 @@
         :param collapse_on_cursor:
             If set to ``False``, then new jobs will always be created.
             When ``True`` and there is already a job on this cursor in the
             pending state with the same queue/method and marked collapsible then
             the ``conflict_resolver`` will be invoked with the existing job and
             the new request will be collapsed into the previous pending job.
 
+            By default, this is ``True`` when ``cursor_key`` is set. It is an
+            error to set it to ``True`` without using a cursor.
+
         """
         if now is None:
             now = datetime.utcnow()
         if when is None:
             when = now
         if args is None:
             args = {}
         if job_kwargs is None:
             job_kwargs = {}
 
         Job = self.model.Job
         JobStates = self.model.JobStates
 
-        collapsible = cursor_key is not None and collapse_on_cursor
+        if collapse_on_cursor is None and cursor_key:
+            collapse_on_cursor = True
+
+        if collapse_on_cursor and not cursor_key:
+            raise ValueError('cannot collapse a job that is not using a cursor')
 
         job_id = None
         notify = False
         # there is a race condition here in READ COMMITTED mode where
         # a job could start between the insert and the query, so if we
         # do not get a locked job record here we will loop until we either
         # insert a new row or get a locked one
         while True:
             job_id = self.dbsession.execute(
                 insert(Job.__table__)
-                .values({
-                    Job.queue: queue,
-                    Job.method: method,
-                    Job.args: args,
-                    Job.created_time: now,
-                    Job.scheduled_time: when,
-                    Job.state: JobStates.PENDING,
-                    Job.cursor_key: cursor_key,
-                    Job.schedule_id: schedule_id,
-                    Job.collapsible: collapsible,
-                    Job.trace: trace,
-                    **job_kwargs,
-                })
+                .values(
+                    {
+                        Job.queue: queue,
+                        Job.method: method,
+                        Job.args: args,
+                        Job.created_time: now,
+                        Job.scheduled_time: when,
+                        Job.state: JobStates.PENDING,
+                        Job.cursor_key: cursor_key,
+                        Job.schedule_id: schedule_id,
+                        Job.collapsible: collapse_on_cursor,
+                        Job.trace: trace,
+                        **job_kwargs,
+                    }
+                )
                 .on_conflict_do_nothing(
                     index_elements=[Job.cursor_key, Job.queue, Job.method],
                     index_where=sa.and_(
                         Job.state == JobStates.PENDING,
                         Job.collapsible == sa.true(),
                     ),
                 )
                 .returning(Job.id)
             ).scalar()
             if job_id is not None:
                 if schedule_id is not None:
                     log.info(
                         'created new job=%s on queue=%s, method=%s from schedule=%s',
-                        job_id, queue, method, schedule_id,
+                        job_id,
+                        queue,
+                        method,
+                        schedule_id,
                     )
                 else:
                     log.info(
                         'created new job=%s on queue=%s, method=%s',
-                        job_id, queue, method,
+                        job_id,
+                        queue,
+                        method,
                     )
                 notify = True
                 break
 
             # a job already exists, load it and resolve conflicts
             # XXX this will only occur on jobs with a cursor
             job = (
@@ -144,17 +157,19 @@
                         mark_changed(self.dbsession)
 
                 break
 
         if notify:
             epoch_seconds = datetime_to_int(when)
             payload = json.dumps({'j': job_id, 't': epoch_seconds})
-            self.dbsession.execute(sa.select(
-                sa.func.pg_notify(f'{self.model.channel_prefix}{queue}', payload),
-            ))
+            self.dbsession.execute(
+                sa.select(
+                    sa.func.pg_notify(f'{self.model.channel_prefix}{queue}', payload),
+                )
+            )
             # XXX notify is always true when the raw insert works above so we
             # handle the two scenarios (notify and raw insert) in which
             # mark_changed needs to be called with only a single call
             if self.transaction_manager:
                 mark_changed(self.dbsession)
 
         return job_id
@@ -177,19 +192,28 @@
         job = self.find_job(job_id)
         if job is None or job.state not in {
             self.model.JobStates.COMPLETED,
             self.model.JobStates.FAILED,
             self.model.JobStates.LOST,
         }:
             raise RuntimeError('job is not in a retryable state')
+        if job.collapsible:
+            raise ValueError(
+                'cannot automatically retry a collapsible job, instead'
+                ' reinvoke call() with an appropriate conflict_resolver'
+            )
         return self.call(
-            job.queue, job.method, job.args,
+            job.queue,
+            job.method,
+            job.args,
             when=job.scheduled_time,
             cursor_key=job.cursor_key,
             schedule_id=job.schedule_id,
+            collapse_on_cursor=False,
+            trace=job.trace,
         )
 
     def reload_scheduler(self, queue, *, now=None):
         """
         Trigger the scheduler to reload information about modified schedules.
 
         For example, this should be used if ``reload=False`` is used with
@@ -197,17 +221,19 @@
         :ref:`.enable_schedule` in order to batch changes prior to reloading.
 
         """
         if now is None:
             now = datetime.utcnow()
         epoch_seconds = datetime_to_int(now)
         payload = json.dumps({'s': None, 't': epoch_seconds})
-        self.dbsession.execute(sa.select(
-            sa.func.pg_notify(f'{self.model.channel_prefix}{queue}', payload),
-        ))
+        self.dbsession.execute(
+            sa.select(
+                sa.func.pg_notify(f'{self.model.channel_prefix}{queue}', payload),
+            )
+        )
 
     def add_schedule(
         self,
         queue,
         method,
         args,
         *,
@@ -270,29 +296,31 @@
             log.info('schedule=%s is already disabled', schedule_id)
             return
         schedule.is_enabled = False
         schedule.next_execution_time = None
         log.debug('disabled schedule=%s', schedule_id)
 
     def enable_schedule(self, schedule_id, *, now=None, reload=True):
-        """ Enable a schedule for execution at its next scheduled time."""
+        """Enable a schedule for execution at its next scheduled time."""
         if now is None:
             now = datetime.utcnow()
         schedule = self.get_schedule(schedule_id, for_update=True)
         if schedule.is_enabled:
             log.info('schedule=%s is already enabled', schedule_id)
             return
         schedule.is_enabled = True
         schedule.next_execution_time = get_next_rrule_time(
-            schedule.rrule, schedule.created_time, now)
+            schedule.rrule, schedule.created_time, now
+        )
         if reload and schedule.next_execution_time is not None:
             self.reload_scheduler(schedule.queue, now=schedule.next_execution_time)
         log.debug(
             'enabling schedule=%s, next execution time=%s',
-            schedule_id, schedule.next_execution_time,
+            schedule_id,
+            schedule.next_execution_time,
         )
 
     def call_schedule(self, schedule_id, *, now=None, reload=True, when=None):
         """
         Manually invoke a schedule, dispatching a job immediately.
 
         This is useful when a job may have been skipped because no schedulers
@@ -313,13 +341,14 @@
             now=now,
             when=when,
             schedule_id=schedule.id,
         )
 
         if schedule.is_enabled:
             schedule.next_execution_time = get_next_rrule_time(
-                schedule.rrule, schedule.created_time, now)
+                schedule.rrule, schedule.created_time, now
+            )
 
             if reload and schedule.next_execution_time is not None:
                 self.reload_scheduler(schedule.queue, now=schedule.next_execution_time)
 
         return job_id
```

### Comparing `psycopg2_mq-0.8.3/src/psycopg2_mq/util.py` & `psycopg2_mq-0.9/src/psycopg2_mq/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,27 +24,23 @@
 
 
 # cribbed from sentry_sdk
 def safe_object(obj, *, memo=None):
     if memo is None:
         memo = Memo()
     if memo.memoize(obj):
-        return '<cycle type={}>'.format(type(obj).__name__)
+        return f'<cycle type={type(obj).__name__}>'
 
     try:
         if isinstance(obj, (tuple, list)):
-            return [
-                safe_object(x, memo=memo)
-                for x in obj
-            ]
+            return [safe_object(x, memo=memo) for x in obj]
 
         if isinstance(obj, Mapping):
             return {
-                safe_str(k): safe_object(v, memo=memo)
-                for k, v in list(obj.items())
+                safe_str(k): safe_object(v, memo=memo) for k, v in list(obj.items())
             }
 
         return safe_repr(obj)
 
     finally:
         memo.unmemoize(obj)
```

### Comparing `psycopg2_mq-0.8.3/src/psycopg2_mq/worker.py` & `psycopg2_mq-0.9/src/psycopg2_mq/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,22 @@
 import psycopg2
 import random
 import select
 import signal
 import sqlalchemy as sa
 from sqlalchemy.dialects.postgresql import insert
 from sqlalchemy.orm import Session
-from sqlalchemy.sql import table, column
+from sqlalchemy.sql import column, table
 import sys
 import threading
 import traceback
 
 from .source import MQSource
 from .trigger import Trigger
-from .util import (
-    class_name,
-    get_next_rrule_time,
-    int_to_datetime,
-    safe_object,
-)
-
+from .util import class_name, get_next_rrule_time, int_to_datetime, safe_object
 
 DEFAULT_TIMEOUT = 60
 DEFAULT_JITTER = 1
 DEFAULT_LOCK_KEY = 1250360252  # selected via random.randint(0, 2**31-1)
 
 
 log = __import__('logging').getLogger(__name__)
@@ -84,15 +78,14 @@
 
     def __init__(
         self,
         *,
         engine,
         queues,
         model,
-
         timeout=DEFAULT_TIMEOUT,
         jitter=DEFAULT_JITTER,
         lock_key=DEFAULT_LOCK_KEY,
         threads=1,
         capture_signals=True,
         name=None,
     ):
@@ -144,14 +137,15 @@
 
         finally:
             self._running = False
 
     def result_from_error(self, ex):
         return {
             'exc': class_name(ex.__class__),
+            'message': str(ex),
             'args': safe_object(ex.args),
             'tb': traceback.format_tb(ex.__traceback__),
         }
 
     def get_status(self):
         # shallow copy to avoid iterating a shared reference
         active_jobs = self._active_jobs.copy()
@@ -183,14 +177,15 @@
     return f'{hostname}.{pid}'
 
 
 @contextmanager
 def maybe_capture_signals(ctx):
     if not ctx._capture_signals:
         yield
+        return
 
     def onsigterm(*args):
         # heroku may send multiple sigterm and we want to only respond
         # to the first one so we'll ignore all the others here
         signal.signal(signal.SIGTERM, signal.SIG_IGN)
         log.info('received SIGTERM, triggering workers to shutdown')
         ctx.shutdown_gracefully()
@@ -217,15 +212,14 @@
         signal.signal(signal.SIGINT, signal.SIG_DFL)
 
 
 @contextmanager
 def connect_db(ctx):
     rotate_dbconn(ctx)
     try:
-
         yield
 
     finally:
         if ctx._dbconn is not None:
             try:
                 release_worker_locks(ctx, retry=False)
             except Exception:
@@ -315,14 +309,15 @@
                 log.warning(
                     'connection closed unexpectedly, error="%s"',
                     str(ex).strip(),
                 )
                 rotate_dbconn(ctx)
                 return fn(ctx, *args, **kwargs)
             raise
+
     return wrapper
 
 
 def dbsession(fn):
     @retry_dbconn
     @functools.wraps(fn)
     def wrapper(ctx, *args, **kwargs):
@@ -337,14 +332,15 @@
                 kwargs['db'] = db
                 kwargs['model'] = ctx._model
                 result = fn(ctx, *args, **kwargs)
                 db.commit()
                 return result
             finally:
                 db.close()
+
     return wrapper
 
 
 @dbsession
 def run_maintenance(ctx, *, db, model):
     release_stale_locks(ctx, db=db, model=model)
     mark_lost_jobs(ctx, db=db, model=model)
@@ -357,19 +353,22 @@
 @dbsession
 def release_stale_locks(ctx, *, db, model):
     Lock = model.Lock
     lock_sq = (
         db.query(Lock.queue, Lock.key)
         # do not block rows that are being cleaned by another transaction
         .with_for_update(of=Lock, skip_locked=True)
-        .outerjoin(pg_locks, sa.and_(
-            pg_locks.c.locktype == 'advisory',
-            pg_locks.c.classid == ctx._lock_key,
-            pg_locks.c.objid == Lock.lock_id,
-        ))
+        .outerjoin(
+            pg_locks,
+            sa.and_(
+                pg_locks.c.locktype == 'advisory',
+                pg_locks.c.classid == ctx._lock_key,
+                pg_locks.c.objid == Lock.lock_id,
+            ),
+        )
         .filter(
             Lock.queue.in_(ctx._queues.keys()),
             Lock.lock_id != sa.null(),
             pg_locks.c.objid == sa.null(),
         )
         .subquery()
     )
@@ -517,33 +516,24 @@
 
     finally:
         current_thread.name = old_thread_name
 
 
 @dbsession
 def finish_job(ctx, job_id, success, result, cursor, *, db, model):
-    job = (
-        db.query(model.Job)
-        .with_for_update()
-        .filter_by(id=job_id)
-        .one()
-    )
+    job = db.query(model.Job).with_for_update().filter_by(id=job_id).one()
 
     if cursor is not None:
         if job.cursor_key is not None:
             save_cursor(db, model, job.cursor_key, cursor, job.id)
 
         elif cursor is not None:
             log.warning('ignoring cursor for job=%s without a cursor_key', job_id)
 
-    job.state = (
-        model.JobStates.COMPLETED
-        if success
-        else model.JobStates.FAILED
-    )
+    job.state = model.JobStates.COMPLETED if success else model.JobStates.FAILED
     job.result = result
     job.end_time = ctx._now()
     job.lock_id = None
     log.info('finished processing job=%s, state="%s"', job_id, job.state)
 
 
 def save_cursor(db, model, key, cursor, job_id=None):
@@ -569,19 +559,22 @@
 
 
 @dbsession
 def mark_lost_jobs(ctx, *, db, model):
     job_q = (
         db.query(model.Job)
         .with_for_update(of=model.Job)
-        .outerjoin(pg_locks, sa.and_(
-            pg_locks.c.locktype == 'advisory',
-            pg_locks.c.classid == ctx._lock_key,
-            pg_locks.c.objid == model.Job.lock_id,
-        ))
+        .outerjoin(
+            pg_locks,
+            sa.and_(
+                pg_locks.c.locktype == 'advisory',
+                pg_locks.c.classid == ctx._lock_key,
+                pg_locks.c.objid == model.Job.lock_id,
+            ),
+        )
         .filter(
             model.Job.state == model.JobStates.RUNNING,
             model.Job.queue.in_(ctx._queues.keys()),
             model.Job.lock_id != sa.null(),
             pg_locks.c.objid == sa.null(),
         )
         .order_by(model.Job.start_time.asc())
@@ -590,20 +583,17 @@
     for job in job_q:
         job.state = model.JobStates.LOST
         job.lock_id = None
         job.end_time = ctx._now()
         log.error('marking job=%s as lost', job.id)
         lost_job_ids.add(job.id)
 
-    job_q = (
-        db.query(model.Job)
-        .filter(
-            model.Job.state == model.JobStates.LOST,
-            model.Job.cursor_key.isnot(None),
-        )
+    job_q = db.query(model.Job).filter(
+        model.Job.state == model.JobStates.LOST,
+        model.Job.cursor_key.isnot(None),
     )
     for job in job_q:
         # avoid warning about jobs that were just marked lost
         if job.id in lost_job_ids:
             continue
         log.warning(
             'job=%s is lost and blocking execution of cursor=%s for %d seconds',
@@ -715,20 +705,22 @@
         now = ctx._now()
 
     Lock = model.Lock
     new_queues = set()
     for queue in (q for q in ctx._queues if q not in ctx._scheduler_queues):
         result = db.execute(
             insert(Lock.__table__)
-            .values({
-                Lock.queue: queue,
-                Lock.key: 'scheduler',
-                Lock.lock_id: ctx._lock_id,
-                Lock.worker: ctx._name,
-            })
+            .values(
+                {
+                    Lock.queue: queue,
+                    Lock.key: 'scheduler',
+                    Lock.lock_id: ctx._lock_id,
+                    Lock.worker: ctx._name,
+                }
+            )
             .on_conflict_do_nothing()
             .returning(Lock.queue)
         ).scalar()
         if result is not None:
             new_queues.add(queue)
 
     if new_queues:
@@ -744,19 +736,21 @@
             model.JobSchedule.is_enabled == sa.true(),
             model.JobSchedule.next_execution_time < stale_cutoff_time,
         )
         .all()
     )
     for s in stale_schedules:
         next_execution_time = get_next_rrule_time(
-            s.rrule, s.created_time, stale_cutoff_time)
+            s.rrule, s.created_time, stale_cutoff_time
+        )
         log.warning(
             'execution time on schedule=%s is very old (%s seconds), skipping '
             'to next time=%s',
-            s.id, (now - s.next_execution_time).total_seconds(),
+            s.id,
+            (now - s.next_execution_time).total_seconds(),
             next_execution_time,
         )
         s.next_execution_time = next_execution_time
 
     set_next_schedule_time(ctx, db=db, model=model)
 
 
@@ -871,15 +865,15 @@
 
     event = NotifyEvent()
     while conn.notifies:
         notify = conn.notifies.pop(0)
         channel, payload = notify.channel, notify.payload
 
         try:
-            queue = channel[len(ctx._model.channel_prefix):]
+            queue = channel[len(ctx._model.channel_prefix) :]
             data = json.loads(payload)
             t = data['t']
             event_time = int_to_datetime(t)
 
             if 'j' in data:
                 if event_time < event.next_job_time:
                     event = NotifyEvent()
@@ -893,16 +887,19 @@
                     event = NotifyEvent()
                     event.next_schedule_time = event_time
 
             else:
                 raise Exception
 
         except Exception:
-            log.exception('error while handling event from channel=%s, '
-                          'payload=%s', channel, payload)
+            log.exception(
+                'error while handling event from channel=%s, payload=%s',
+                channel,
+                payload,
+            )
             continue
 
     return event
 
 
 def get_next_event(ctx):
     conn = ctx._dbconn.connection
```

### Comparing `psycopg2_mq-0.8.3/src/psycopg2_mq.egg-info/PKG-INFO` & `psycopg2_mq-0.9/src/psycopg2_mq.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: psycopg2-mq
-Version: 0.8.3
+Version: 0.9
 Summary: A message queue written around PostgreSQL.
 Home-page: https://github.com/mmerickel/psycopg2_mq
 Author: Michael Merickel
 Author-email: oss@m.merickel.org
-License: UNKNOWN
-Keywords: psycopg2,postgres,postgresql
-Platform: UNKNOWN
+Keywords: psycopg2,postgres,postgresql,message queue,background jobs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 ===========
 psycopg2_mq
 ===========
 
 .. image:: https://img.shields.io/pypi/v/psycopg2_mq.svg
     :target: https://pypi.org/pypi/psycopg2_mq
 
+.. image:: https://github.com/mmerickel/psycopg2_mq/workflows/Build%20and%20test/badge.svg?branch=main
+    :target: https://github.com/mmerickel/psycopg2_mq/actions?query=workflow%3A%22Build+and+test%22
+    :alt: main CI Status
+
 ``psycopg2_mq`` is a message queue implemented on top of
 `PostgreSQL <https://www.postgresql.org/>`__,
 `SQLAlchemy <https://www.sqlalchemy.org/>`__, and
 `psycopg2 <http://initd.org/psycopg/>`__.
 
 Currently the library provides only the low-level constructs that can be used
 to build a multithreaded worker system. It is broken into two components:
@@ -40,14 +45,18 @@
   single-threaded worker that can accept jobs and execute them. An application
   should create worker per thread. It supports an API for thread-safe graceful
   shutdown.
 
 - ``psycopg2_mq.MQSource`` - a source object providing a client-side API for
   invoking and querying job states.
 
+It is expected that these core components are then wrapped into your own
+application in any way that you see fit, without dictating a specific CLI
+or framework.
+
 Data Model
 ==========
 
 Queues
 ------
 
 Workers run jobs defined in queues. Currently each queue will run jobs
@@ -155,41 +164,64 @@
         mq = MQSource(
             dbsession=dbsession,
             model=model,
         )
         job = mq.call('echo', 'hello', {'name': 'Andy'})
         print(f'queued job={job.id}')
 
+Changes
+=======
+
+0.9 (2023-04-21)
+----------------
+
+- Add support for Python 3.10, and 3.11.
+
+- [breaking] Prevent retrying of collapsible jobs. Require them to be invoked
+  using ``call`` instead for an opportunity to specify a ``conflict_resolver``.
+
+- Fix a bug in the default model schema in which the collapsible database
+  index was not marked unique.
+
+- Copy trace info when retrying a job.
+
+- Capture the stringified exception to the job result in the ``message`` key,
+  alongside the existing ``tb``, ``exc``, and ``args`` keys.
+
+- The worker was not recognizing ``capture_signals=False``, causing problems
+  when running the event loop in other threads.
+
+- Blackify the codebase and add some real tests. Yay!
 
 0.8.3 (2022-04-15)
-==================
+------------------
 
 - [breaking] Remove ``MQWorker.make_job_context``.
 
 0.8.2 (2022-04-15)
-==================
+------------------
 
 - Drop Python 3.6 support.
 
 - [breaking] Require SQLAlchemy 1.4+ and resolve deprecation warnings related to
   SQLAlchemy 2.0.
 
 - [breaking] Rename ``update_job_id`` to ``updated_job_id`` in the
   ``JobCursor`` model.
 
 0.8.1 (2022-04-15)
-==================
+------------------
 
 - Ensure the ``trace`` attribute is populated on the ``JobContext``.
 
 - Add ``MQWorker.make_job_context`` which can be defined to completely override
   the ``JobContext`` factory using the ``Job`` object and open database session.
 
 0.8.0 (2022-04-15)
-==================
+------------------
 
 - [breaking] Add ``update_job_id`` foreign key to the ``JobCursor`` model to
   make it possible to know which job last updated the value in the cursor.
 
 - [breaking] Add ``trace`` json blob to the ``Job`` model.
 
 - Support a ``trace`` json blob when creating new jobs. This value is available
@@ -200,142 +232,142 @@
   See ``JobContext.trace`` attribute when handling jobs.
 
 - Add a standard ``FailedJobError`` exception which can be raised by jobs to
   mark a failure with a custom result object. This is different from unhandled
   exceptions that cause the ``MQWorker.result_from_error`` method to be invoked.
 
 0.7.0 (2022-03-03)
-==================
+------------------
 
 - Fix a corner case with lost jobs attached to cursors. In scenarios where
   multiple workers are running, if one loses a database connection then the
   other is designed to notice and mark jobs lost. However, it's possible the
   job is not actually lost and the worker can then recover after resuming
   its connection, and marking the job running again. In this situation, we
   do not want another job to begin on the same cursor. To fix this issue,
   new jobs will not be run if another job is marked lost on the same cursor.
   You will be required to recover the job by marking it as not lost (probably
   failed) first to unblock the rest of the jobs on the cursor.
 
 0.6.2 (2022-03-01)
-==================
+------------------
 
 - Prioritize maintenance work higher than running new jobs.
   There was a chicken-and-egg issue where a job would be marked running
   but needs to be marked lost. However marking it lost is lower priority than
   trying to start new jobs. In the case where a lot of jobs were scheduled
   at the same time, the worker always tried to start new jobs and didn't
   run the maintenance so the job never got marked lost, effectively blocking
   the queue.
 
 0.6.1 (2022-01-15)
-==================
+------------------
 
 - Fix a bug introduced in the 0.6.0 release when scheduling new jobs.
 
 0.6.0 (2022-01-14)
-==================
+------------------
 
 - [breaking] Add model changes to mark jobs as collapsible.
 
 - [breaking] Add model changes to the cursor index.
 
 - Allow multiple pending jobs to be scheduled on the same cursor if either:
 
   1. The queue or method are different from existing pending jobs on the cursor.
 
   2. ``collapse_on_cursor`` is set to ``False`` when scheduling the job.
 
 0.5.7 (2021-03-07)
-==================
+------------------
 
 - Add a ``schedule_id`` attribute to the job context for use in jobs that want
   to know whether they were executed from a schedule or not.
 
 0.5.6 (2021-02-28)
-==================
+------------------
 
 - Some UnicodeDecodeError exceptions raised from jobs could trigger a
   serialization failure (UntranslatableCharacter) because it would contain
   the sequence ``\u0000``` which, while valid in Python, is not allowed
   in postgres. So when dealing with the raw bytes, we'll decode it with
   the replacement character that can be properly stored. Not ideal, but
   better than failing to store the error at all.
 
 0.5.5 (2021-01-22)
-==================
+------------------
 
 - Fixed some old code causing the worker lock to release after a job
   completed.
 
 0.5.4 (2021-01-20)
-==================
+------------------
 
 - Log at the error level when marking a job as lost.
 
 0.5.3 (2021-01-11)
-==================
+------------------
 
 - Copy the ``schedule_id`` information to retried jobs.
 
 0.5.2 (2021-01-11)
-==================
+------------------
 
 - [breaking] Require ``call_schedule`` to accept an id instead of an object.
 
 0.5.1 (2021-01-09)
-==================
+------------------
 
 - Drop the ``UNIQUE`` constraint on the background job ``lock_id`` column.
 
 0.5 (2021-01-09)
-================
+----------------
 
 - Add a scheduler model with support for emitting periodic jobs based on
   RRULE syntax.
   See https://github.com/mmerickel/psycopg2_mq/pull/11
 
 - Enable the workers to coordinate on a per-queue basis who is in control
   of scheduling jobs.
   See https://github.com/mmerickel/psycopg2_mq/pull/12
 
 - Reduce the number of advisory locks held from one per job to one per worker.
   See https://github.com/mmerickel/psycopg2_mq/pull/12
 
 0.4.5 (2020-12-22)
-==================
+------------------
 
 - Use column objects in the insert statement to support ORM-level synonyms,
   enabling the schema to have columns with different names.
 
 0.4.4 (2019-11-07)
-==================
+------------------
 
 - Ensure the advisory locks are released when a job completes.
 
 0.4.3 (2019-10-31)
-==================
+------------------
 
 - Ensure maintenance (finding lost jobs) always runs at set intervals defined
   by the ``timeout`` parameter.
 
 0.4.2 (2019-10-30)
-==================
+------------------
 
 - Recover active jobs when the connection is lost by re-locking them
   and ensuring they are marked running.
 
 0.4.1 (2019-10-30)
-==================
+------------------
 
 - Attempt to reconnect to the database after losing the connection.
   If the reconnect attempt fails then crash.
 
 0.4 (2019-10-28)
-================
+----------------
 
 - Add a ``worker`` column to the ``Job`` model to track what worker
   is handling a job.
 
 - Add an optional ``name`` argument to ``MQWorker`` to name the worker -
   the value will be recorded in each job.
 
@@ -346,79 +378,77 @@
 - Add ``capture_signals`` argument (default=``True``) to ``MQWorker`` which
   will capture ``SIGTERM``, ``SIGINT`` and ``SIGUSR1``. The first two will
   trigger graceful shutdown - they will make the process stop handling new
   jobs while finishing active jobs. The latter will dump to ``stderr`` a
   JSON dump of the current status of the worker.
 
 0.3.3 (2019-10-23)
-==================
+------------------
 
 - Only save a cursor update if the job is completed successfully.
 
 0.3.2 (2019-10-22)
-==================
+------------------
 
 - Mark lost jobs during timeouts instead of just when a worker starts in order
   to catch them earlier.
 
 0.3.1 (2019-10-17)
-==================
+------------------
 
 - When attempting to schedule a job with a cursor and a ``scheduled_time``
   earlier than a pending job on the same cursor, the job will be updated to
   run at the earlier time.
 
 - When attempting to schedule a job with a cursor and a pending job already
   exists on the same cursor, a ``conflict_resolver`` function may be
   supplied to ``MQSource.call`` to update the job properties, merging the
   arguments however the user wishes.
 
 0.3 (2019-10-15)
-================
+----------------
 
 - Add a new column ``cursor_snapshot`` to the ``Job`` model which will
   contain the value of the cursor when the job begins.
 
 0.2 (2019-10-09)
-================
+----------------
 
 - Add cursor support for jobs. This requires a schema migration to add
   a ``cursor_key`` column, a new ``JobCursor`` model, and some new indices.
 
 0.1.6 (2019-10-07)
-==================
+------------------
 
 - Support passing custom kwargs to the job in ``psycopg2_mq.MQSource.call``
   to allow custom columns on the job table.
 
 0.1.5 (2019-05-17)
-==================
+------------------
 
 - Fix a regression when serializing errors with strings or cycles.
 
 0.1.4 (2019-05-09)
-==================
+------------------
 
 - More safely serialize exception objects when jobs fail.
 
 0.1.3 (2018-09-04)
-==================
+------------------
 
 - Rename the thread to contain the job id while it's handling a job.
 
 0.1.2 (2018-09-04)
-==================
+------------------
 
 - Rename ``Job.params`` to ``Job.args``.
 
 0.1.1 (2018-09-04)
-==================
+------------------
 
 - Make ``psycopg2`` an optional dependency in order to allow apps to depend
   on ``psycopg2-binary`` if they wish.
 
 0.1 (2018-09-04)
-================
+----------------
 
 - Initial release.
-
-
```

