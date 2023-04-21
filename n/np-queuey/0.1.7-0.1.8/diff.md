# Comparing `tmp/np_queuey-0.1.7.tar.gz` & `tmp/np_queuey-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_queuey-0.1.7.tar", last modified: Tue Apr 18 17:04:57 2023, max compression
+gzip compressed data, was "np_queuey-0.1.8.tar", last modified: Fri Apr 21 18:48:10 2023, max compression
```

## Comparing `np_queuey-0.1.7.tar` & `np_queuey-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      227 2023-04-13 16:35:48.733260 np_queuey-0.1.7/README.md
--rw-r--r--   0        0        0     2448 2023-04-18 17:04:57.425135 np_queuey-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-13 23:41:50.797573 np_queuey-0.1.7/src/np_queuey/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.7/src/np_queuey/hueys/__init__.py
--rw-r--r--   0        0        0     8732 2023-04-18 16:02:58.142537 np_queuey-0.1.7/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.7/src/np_queuey/jobs/__init__.py
--rw-r--r--   0        0        0     6844 2023-04-18 16:06:53.861920 np_queuey-0.1.7/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.1.7/src/np_queuey/jobs/run_small_jobs.py
--rw-r--r--   0        0        0     3177 2023-04-18 17:04:45.613009 np_queuey-0.1.7/src/np_queuey/queues.py
--rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.7/src/np_queuey/tasks.py
--rw-r--r--   0        0        0      140 2023-04-15 00:21:38.620120 np_queuey-0.1.7/src/np_queuey/utils.py
--rw-r--r--   0        0        0      593 2023-04-13 20:34:38.147095 np_queuey-0.1.7/tests/test_huey.py
--rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 np_queuey-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.1.8/README.md
+-rw-r--r--   0        0        0     2495 2023-04-21 18:48:10.734070 np_queuey-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-19 04:15:23.199506 np_queuey-0.1.8/src/np_queuey/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.8/src/np_queuey/hueys/__init__.py
+-rw-r--r--   0        0        0     9080 2023-04-21 18:42:21.408358 np_queuey-0.1.8/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.8/src/np_queuey/jobs/__init__.py
+-rw-r--r--   0        0        0     6936 2023-04-18 18:55:14.478321 np_queuey-0.1.8/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.1.8/src/np_queuey/jobs/run_small_jobs.py
+-rw-r--r--   0        0        0     3136 2023-04-19 04:15:23.202499 np_queuey-0.1.8/src/np_queuey/queues.py
+-rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.8/src/np_queuey/tasks.py
+-rw-r--r--   0        0        0      140 2023-04-19 04:15:23.203497 np_queuey-0.1.8/src/np_queuey/utils.py
+-rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.1.8/tests/test_huey.py
+-rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 np_queuey-0.1.8/PKG-INFO
```

### Comparing `np_queuey-0.1.7/pyproject.toml` & `np_queuey-0.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [project]
 name = "np_queuey"
-version = "0.1.7"
+version = "0.1.8"
 description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "huey>=2.4.5",
+    "peewee>=3.16.1",
+    "sqlite-web>=0.4.1",
     "np-config>=0.4.17",
     "np-logging>=0.5.1",
-    "np-tools>=0.1.0",
+    "np-tools>=0.1.2",
     "np-session>=0.5.1",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `np_queuey-0.1.7/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.8/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,237 +1,240 @@
-from __future__ import annotations
-
-import pathlib
-import json
-from typing_extensions import Literal
-
-import huey as _huey
-import np_config
-import np_logging
-import np_session
-import np_tools
-
-import np_queuey
-from np_queuey.jobs import dynamicrouting_behavior_session_mtrain_upload as job
-import np_queuey.utils as utils
-
-logger = np_logging.getLogger()
-
-huey = np_queuey.HueyQueue(utils.DEFAULT_HUEY_SQLITE_DB_PATH).huey
-
-UPLOAD_JSON_DIR_CONFIG_KEY = (
-    'dynamicrouting_behavior_session_mtrain_upload_json_dir'
-)
-"""Single leading fwd slash, for unix compatibility on hpc"""
-
-
-@huey.periodic_task(_huey.crontab(minute='*/10', strict=True))
-def upload_outstanding_sessions() -> None:
-    sessions: list[
-        tuple[str, str]
-    ] = job.get_outstanding_behavior_sessions_for_processing()
-    if not sessions:
-        logger.info('No outstanding sessions to upload')
-        return
-    logger.info('Found %d outstanding sessions to upload', len(sessions))
-    for foraging_id_and_filename in sessions:
-        upload_session_on_hpc(foraging_id_and_filename)
-
-
-@huey.task()
-def upload_session_on_hpc(foraging_id_and_filename: tuple[str, str]) -> None:
-    if is_behavior_session_in_mtrain(foraging_id_and_filename):
-        logger.info(
-            'Behavior session %r already in mtrain', foraging_id_and_filename
-        )
-        job.mark_behavior_session_as_uploaded(foraging_id_and_filename[0])
-        return
-    np_logging.web('np_queuey').info(
-        'Starting behavior session upload to mtrain: %r',
-        foraging_id_and_filename,
-    )
-    write_input_json(foraging_id_and_filename)
-    write_shell_script(foraging_id_and_filename)
-    with np_tools.ssh('hpc-login') as ssh:
-        logger.debug(
-            'Launching mtrain_lims on hpc for %s', foraging_id_and_filename
-        )
-        ssh.run(hpc_cmd(foraging_id_and_filename))
-    verify_behavior_session_uploaded.schedule(
-        (foraging_id_and_filename,), delay=60
-    )
-
-
-@huey.task(retry_delay=60, retries=3)
-def verify_behavior_session_uploaded(
-    foraging_id_and_filename: tuple[str, str]
-) -> None:
-    _, output_json = input_output_jsons(foraging_id_and_filename)
-
-    if not np_config.normalize_path(output_json).exists():
-        msg = f'{output_json} does not exist'
-        np_logging.web('np_queuey').warning(msg)
-        raise FileNotFoundError(msg)
-
-    if not is_behavior_session_in_mtrain(foraging_id_and_filename):
-        msg = f'Could not find behavior session {foraging_id_and_filename[0]} in mtrain'
-        np_logging.web('np_queuey').warning(msg)
-        raise ValueError(msg)
-
-    job.mark_behavior_session_as_uploaded(foraging_id_and_filename[0])
-    np_logging.web('np_queuey').info(
-        'Behavior session %r verified in mtrain', foraging_id_and_filename
-    )
-
-
-def is_behavior_session_in_mtrain(
-    foraging_id_and_filename: tuple[str, str]
-) -> bool:
-    """
-    >>> is_behavior_session_in_mtrain(('e4d6666e-3c0d-4726-9dd8-afccd124e872', 'DynamicRouting1_660023_20230417_162846.hdf5'))
-    True
-    """
-    _, filename = foraging_id_and_filename
-    _, mouse_id, date, time = job.parse_filename(filename)
-    mtrain = np_session.Mouse(mouse_id).mtrain
-    return foraging_id_and_filename[0].replace('-', '') in [
-        _['id'].replace('-', '') for _ in mtrain.all_behavior_sessions
-    ]
-
-
-def write_input_json(foraging_id_and_filename: tuple[str, str]) -> None:
-    input_json, _ = input_output_jsons(foraging_id_and_filename)
-    logger.debug('Writing %s', input_json)
-    path = pathlib.Path(np_config.normalize_path(input_json))
-    path.parent.mkdir(parents=True, exist_ok=True)
-    path.write_text(
-        json.dumps(get_input_json_contents(foraging_id_and_filename))
-    )
-
-
-def input_output_jsons(
-    foraging_id_and_filename: tuple[str, str]
-) -> tuple[str, str]:
-    upload_json_dir = np_config.fetch('/projects/np_queuey/config')[
-        UPLOAD_JSON_DIR_CONFIG_KEY
-    ]
-    return tuple(
-        f'{upload_json_dir}/UPLOAD_TO_MTRAIN_{foraging_id_and_filename[0]}_{x}.json'
-        for x in ('input', 'output')
-    )
-
-
-def hpc_cmd(foraging_id_and_filename) -> str:
-    path = shell_script(foraging_id_and_filename).as_posix()
-    return f"sbatch {path.replace('//', '/')}"
-
-
-def get_behavior_session_storage_dir(foraging_id_and_filename) -> pathlib.Path:
-    """
-    * `storage_directory` isn't being populated in LIMS if upload job fails
-    * will need to manually construct path
-
-    >>> d = get_behavior_session_storage_dir(('3b70feba-8572-4cd8-884b-35ff62975d39', 'DynamicRouting1_366122_20230414_120213.hdf5'))
-    >>> d.as_posix()
-    '//allen/programs/braintv/production/neuralcoding/prod0/specimen_657428270/behavior_session_1264106353'
-    """
-    foraging_id, filename = foraging_id_and_filename
-    _, mouse_id, date, time = job.parse_filename(filename)
-    mouse = np_session.Mouse(mouse_id)
-    if not mouse.lims:
-        raise ValueError(f'Could not find mouse {mouse_id} in LIMS')
-    if not mouse.lims.get('behavior_sessions'):
-        raise ValueError(
-            f'Could not find behavior sessions for mouse {mouse_id} in LIMS'
-        )
-    behavior_sessions = tuple(
-        _
-        for _ in mouse.lims['behavior_sessions']
-        if _['foraging_id'].replace('-', '') == foraging_id.replace('-', '')
-    )
-    if not behavior_sessions:
-        raise ValueError(
-            f'Could not find behavior session for foraging_id {foraging_id} in LIMS'
-        )
-    return np_config.normalize_path(
-        mouse.lims.path / f'behavior_session_{behavior_sessions[0]["id"]}'
-    )
-
-
-def get_input_json_contents(
-    foraging_id_and_filename: tuple[str, str]
-) -> dict[Literal['inc'], dict[str, str]]:
-    """
-
-    >>> r = get_input_json_contents(('3b70feba-8572-4cd8-884b-35ff62975d39', 'DynamicRouting1_366122_20230414_120213.hdf5'))
-    >>> r['inc']['foraging_file_name']
-    '/allen/programs/braintv/production/neuralcoding/prod0/specimen_657428270/behavior_session_1264106353/DynamicRouting1_366122_20230414_120213.hdf5'
-    """
-    foraging_id, filename = foraging_id_and_filename
-    try:
-        storage_directory = get_behavior_session_storage_dir(
-            foraging_id_and_filename
-        )
-    except ValueError as exc:
-        np_logging.web('np_queuey').exception(exc)
-        raise exc
-    else:
-        file = storage_directory / filename
-        if not file.exists():
-            msg = (
-                f'Preparing for mtrain upload but file does not exist: {file}'
-            )
-            np_logging.web('np_queuey').error(msg)
-            raise FileNotFoundError(msg)
-        return {
-            'inc': {
-                'API_BASE': 'http://mtrain:5000',
-                'foraging_id': foraging_id,
-                'foraging_file_name': f'{file.as_posix()[1:] if file.as_posix().startswith("//") else file.as_posix()}',  # TODO remove leading slash,
-            }
-        }
-
-
-def shell_script(foraging_id_and_filename: tuple[str, str]) -> pathlib.Path:
-    return pathlib.Path(
-        f'//allen/scratch/aibstemp/svc_neuropix/mtrain_upload/mtrain_upload_{foraging_id_and_filename[0]}.sh'
-    )
-
-
-def write_shell_script(foraging_id_and_filename: tuple[str, str]) -> None:
-    path = shell_script(foraging_id_and_filename)
-    logger.debug('Writing %s', path.as_posix())
-    with path.open('w', newline='\n') as f:
-        f.write(get_shell_script_contents(foraging_id_and_filename))
-
-
-def get_shell_script_contents(
-    foraging_id_and_filename: tuple[str, str]
-) -> str:
-    foraging_id, filename = foraging_id_and_filename
-    input_json, output_json = input_output_jsons(foraging_id_and_filename)
-    return f"""#!/bin/bash
-#SBATCH --job-name=npexp_to_incoming                        # Job name
-#SBATCH --mail-type=FAIL                                    # Mail events (NONE, BEGIN, END, FAIL, ALL)
-#SBATCH --mail-user=ben.hardcaslt@alleninstitute.org        # Where to send mail  
-#SBATCH --ntasks=1                                          # Run on a single CPU
-#SBATCH --mem=1gb                                           # Job memory request (per node)
-#SBATCH --time=00:10:00                                     # Time limit hrs:min:sec
-#SBATCH --output=mtrain_upload_{foraging_id}.log            # Standard output and error log
-#SBATCH --partition braintv                                 # Partition used for processing
-#SBATCH --tmp=100M                                          # Request the amount of space your jobs needs on /scratch/fast
-
-pwd; hostname; date
-
-echo 'Running mtrain upload job on a single thread'
-
-source activate /allen/aibs/technology/conda/production/mtrain_upload
-mtrain_lims --input_json {input_json} --output_json {output_json}
-
-date
-"""
-
-
-if __name__ == '__main__':
-    import doctest
-
-    doctest.testmod(verbose=False)
+from __future__ import annotations
+
+import pathlib
+import json
+from typing_extensions import Literal
+
+import huey as _huey
+import np_config
+import np_logging
+import np_session
+import np_tools
+
+import np_queuey
+from np_queuey.jobs import dynamicrouting_behavior_session_mtrain_upload as job
+import np_queuey.utils as utils
+
+logger = np_logging.getLogger()
+
+huey = np_queuey.HueyQueue(utils.DEFAULT_HUEY_SQLITE_DB_PATH).huey
+
+UPLOAD_JSON_DIR_CONFIG_KEY = (
+    'dynamicrouting_behavior_session_mtrain_upload_json_dir'
+)
+"""Single leading fwd slash, for unix compatibility on hpc"""
+
+
+@huey.periodic_task(_huey.crontab(minute='*/10', strict=True))
+def upload_outstanding_sessions() -> None:
+    sessions: list[
+        tuple[str, str]
+    ] = job.get_outstanding_behavior_sessions_for_processing()
+    if not sessions:
+        logger.info('No outstanding sessions to upload')
+        return
+    logger.info('Found %d outstanding sessions to upload', len(sessions))
+    for foraging_id_and_filename in sessions:
+        upload_session_on_hpc(foraging_id_and_filename)
+
+
+@huey.task()
+def upload_session_on_hpc(foraging_id_and_filename: tuple[str, str]) -> None:
+    if is_behavior_session_in_mtrain(foraging_id_and_filename):
+        logger.info(
+            'Behavior session %r already in mtrain', foraging_id_and_filename
+        )
+        job.mark_behavior_session_as_uploaded(foraging_id_and_filename[0])
+        return
+    np_logging.web('np_queuey').info(
+        'Starting behavior session upload to mtrain: %r',
+        foraging_id_and_filename,
+    )
+    write_input_json(foraging_id_and_filename)
+    write_shell_script(foraging_id_and_filename)
+    with np_tools.ssh('hpc-login') as ssh:
+        logger.debug(
+            'Launching mtrain_lims on hpc for %s', foraging_id_and_filename
+        )
+        ssh.run(hpc_cmd(foraging_id_and_filename))
+    verify_behavior_session_uploaded.schedule(
+        (foraging_id_and_filename,), delay=60
+    )
+
+
+@huey.task(retry_delay=60, retries=3)
+def verify_behavior_session_uploaded(
+    foraging_id_and_filename: tuple[str, str]
+) -> None:
+    _, output_json = input_output_jsons(foraging_id_and_filename)
+
+    if not np_config.normalize_path(output_json).exists():
+        msg = f'{output_json} does not exist'
+        np_logging.web('np_queuey').warning(msg)
+        raise FileNotFoundError(msg)
+
+    if not is_behavior_session_in_mtrain(foraging_id_and_filename):
+        msg = f'Could not find behavior session {foraging_id_and_filename[0]} in mtrain'
+        np_logging.web('np_queuey').warning(msg)
+        raise ValueError(msg)
+
+    job.mark_behavior_session_as_uploaded(foraging_id_and_filename[0])
+    np_logging.web('np_queuey').info(
+        'Behavior session %r verified in mtrain', foraging_id_and_filename
+    )
+
+
+def is_behavior_session_in_mtrain(
+    foraging_id_and_filename: tuple[str, str]
+) -> bool:
+    """
+    >>> is_behavior_session_in_mtrain(('e4d6666e-3c0d-4726-9dd8-afccd124e872', 'DynamicRouting1_660023_20230417_162846.hdf5'))
+    True
+    """
+    _, filename = foraging_id_and_filename
+    _, mouse_id, date, time = job.parse_filename(filename)
+    mtrain = np_session.Mouse(mouse_id).mtrain
+    return foraging_id_and_filename[0].replace('-', '') in [
+        _['id'].replace('-', '') for _ in mtrain.all_behavior_sessions
+    ]
+
+
+def write_input_json(foraging_id_and_filename: tuple[str, str]) -> None:
+    input_json, _ = input_output_jsons(foraging_id_and_filename)
+    logger.debug('Writing %s', input_json)
+    path = pathlib.Path(np_config.normalize_path(input_json))
+    path.parent.mkdir(parents=True, exist_ok=True)
+    path.write_text(
+        json.dumps(get_input_json_contents(foraging_id_and_filename))
+    )
+
+
+def input_output_jsons(
+    foraging_id_and_filename: tuple[str, str]
+) -> tuple[str, str]:
+    upload_json_dir = np_config.fetch('/projects/np_queuey/config')[
+        UPLOAD_JSON_DIR_CONFIG_KEY
+    ]
+    return tuple(
+        f'{upload_json_dir}/UPLOAD_TO_MTRAIN_{foraging_id_and_filename[0]}_{x}.json'
+        for x in ('input', 'output')
+    )
+
+
+def hpc_cmd(foraging_id_and_filename) -> str:
+    path = shell_script(foraging_id_and_filename).as_posix()
+    return f"sbatch {path.replace('//', '/')}"
+
+
+def get_behavior_session_storage_dir(foraging_id_and_filename) -> pathlib.Path:
+    """
+    * `storage_directory` isn't being populated in LIMS if upload job fails
+    * will need to manually construct path
+
+    >>> d = get_behavior_session_storage_dir(('3b70feba-8572-4cd8-884b-35ff62975d39', 'DynamicRouting1_366122_20230414_120213.hdf5'))
+    >>> d.as_posix()
+    '//allen/programs/braintv/production/neuralcoding/prod0/specimen_657428270/behavior_session_1264106353'
+    """
+    foraging_id, filename = foraging_id_and_filename
+    _, mouse_id, date, time = job.parse_filename(filename)
+    mouse = np_session.Mouse(mouse_id)
+    if not mouse.lims:
+        raise ValueError(f'Could not find mouse {mouse_id} in LIMS')
+    if not mouse.lims.get('behavior_sessions'):
+        raise ValueError(
+            f'Could not find behavior sessions for mouse {mouse_id} in LIMS'
+        )
+    behavior_sessions = tuple(
+        _
+        for _ in mouse.lims['behavior_sessions']
+        if _['foraging_id'].replace('-', '') == foraging_id.replace('-', '')
+    )
+    if not behavior_sessions:
+        raise ValueError(
+            f'Could not find behavior session for foraging_id {foraging_id} in LIMS'
+        )
+    return np_config.normalize_path(
+        mouse.lims.path / f'behavior_session_{behavior_sessions[0]["id"]}'
+    )
+
+
+def get_input_json_contents(
+    foraging_id_and_filename: tuple[str, str]
+) -> dict[Literal['inc'], dict[str, str]]:
+    """
+
+    >>> r = get_input_json_contents(('3b70feba-8572-4cd8-884b-35ff62975d39', 'DynamicRouting1_366122_20230414_120213.hdf5'))
+    >>> r['inc']['foraging_file_name']
+    '/allen/programs/braintv/production/neuralcoding/prod0/specimen_657428270/behavior_session_1264106353/DynamicRouting1_366122_20230414_120213.hdf5'
+    """
+    foraging_id, filename = foraging_id_and_filename
+    try:
+        storage_directory = get_behavior_session_storage_dir(
+            foraging_id_and_filename
+        )
+    except ValueError as exc:
+        np_logging.web('np_queuey').exception(exc)
+        raise exc
+    else:
+        file = storage_directory / filename
+        if not file.exists():
+            msg = (
+                f'Preparing for mtrain upload but file does not exist: {file}'
+            )
+            np_logging.web('np_queuey').error(msg)
+            raise FileNotFoundError(msg)
+        np_logging.web('np_queuey').info(
+            'File found for upload to mtrain: %r', file
+        )
+        return {
+            'inc': {
+                'API_BASE': 'http://mtrain:5000',
+                'foraging_id': foraging_id,
+                'foraging_file_name': f'{file.as_posix()[1:] if file.as_posix().startswith("//") else file.as_posix()}',  # TODO remove leading slash,
+            }
+        }
+
+
+def shell_script(foraging_id_and_filename: tuple[str, str]) -> pathlib.Path:
+    return pathlib.Path(
+        f'//allen/scratch/aibstemp/svc_neuropix/mtrain_upload/mtrain_upload_{foraging_id_and_filename[0]}.sh'
+    )
+
+
+def write_shell_script(foraging_id_and_filename: tuple[str, str]) -> None:
+    path = shell_script(foraging_id_and_filename)
+    logger.debug('Writing %s', path.as_posix())
+    with path.open('w', newline='\n') as f:
+        f.write(get_shell_script_contents(foraging_id_and_filename))
+
+
+def get_shell_script_contents(
+    foraging_id_and_filename: tuple[str, str]
+) -> str:
+    foraging_id, filename = foraging_id_and_filename
+    input_json, output_json = input_output_jsons(foraging_id_and_filename)
+    return f"""#!/bin/bash
+#SBATCH --job-name=npexp_to_incoming                        # Job name
+#SBATCH --mail-type=FAIL                                    # Mail events (NONE, BEGIN, END, FAIL, ALL)
+#SBATCH --mail-user=ben.hardcaslt@alleninstitute.org        # Where to send mail  
+#SBATCH --ntasks=1                                          # Run on a single CPU
+#SBATCH --mem=1gb                                           # Job memory request (per node)
+#SBATCH --time=00:10:00                                     # Time limit hrs:min:sec
+#SBATCH --output=mtrain_upload_{foraging_id}.log            # Standard output and error log
+#SBATCH --partition braintv                                 # Partition used for processing
+#SBATCH --tmp=100M                                          # Request the amount of space your jobs needs on /scratch/fast
+
+pwd; hostname; date
+
+echo 'Running mtrain upload job on a single thread'
+
+source activate /allen/aibs/technology/conda/production/mtrain_upload
+mtrain_lims --input_json {input_json} --output_json {output_json}
+
+date
+"""
+
+
+if __name__ == '__main__':
+    import doctest
+
+    doctest.testmod(verbose=False)
```

### Comparing `np_queuey-0.1.7/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.8/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,16 @@
 def dynamic_routing_task_db():
     """
     >>> conn = dynamic_routing_task_db()
     >>> _ = conn.cursor()
     """
     conn = sqlite3.connect(DB_PATH, timeout=1)
     conn.isolation_level = None  # autocommit mode
+    conn.execute('pragma journal_mode="truncate"')
+    conn.execute('pragma synchronous=2')
     return conn
 
 
 @contextlib.contextmanager
 def task_db_cursor():
     """
     >>> with task_db_cursor() as c:
```

### Comparing `np_queuey-0.1.7/src/np_queuey/queues.py` & `np_queuey-0.1.8/src/np_queuey/queues.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     """`huey` object for submitting tasks"""
 
     db_path: str
     """Path to the sqlite database for `huey`"""
 
     def __init__(self, sqlite_db_path: Optional[str] = None, **kwargs) -> None:
         self.db_path = sqlite_db_path or utils.DEFAULT_HUEY_SQLITE_DB_PATH
-        # kwargs.setdefault('journal_mode', 'truncate')
-        # kwargs.setdefault('fsync', True)
-        self.huey = huey.SqliteHuey(filename=self.db_path, journal_mode='truncate', fsync=True, **kwargs)
+        kwargs.setdefault('journal_mode', 'truncate')
+        kwargs.setdefault('fsync', True)
+        self.huey = huey.SqliteHuey(filename=self.db_path, **kwargs)
         for task in (
             _ for _ in dir(tasks) if isinstance(getattr(tasks, _), Callable)
         ):
             self.add_task(task)
 
     def add_task(self, task: str) -> None:
         setattr(self, task, self.huey.task()(getattr(tasks, task)))
```

### Comparing `np_queuey-0.1.7/tests/test_huey.py` & `np_queuey-0.1.8/tests/test_huey.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.7/PKG-INFO` & `np_queuey-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-queuey
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,17 +12,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Project-URL: Repository, https://github.com/AllenInstitute/np_queuey
 Project-URL: Bug tracker, https://github.com/AllenInstitute/np_queuey/issues
 Requires-Python: >=3.8
 Requires-Dist: huey>=2.4.5
+Requires-Dist: peewee>=3.16.1
+Requires-Dist: sqlite-web>=0.4.1
 Requires-Dist: np-config>=0.4.17
 Requires-Dist: np-logging>=0.5.1
-Requires-Dist: np-tools>=0.1.0
+Requires-Dist: np-tools>=0.1.2
 Requires-Dist: np-session>=0.5.1
 Requires-Dist: blue>=0.9.1; extra == "dev"
 Requires-Dist: pytest>=7.2.2; extra == "dev"
 Requires-Dist: mypy>=1.1.1; extra == "dev"
 Requires-Dist: coverage[toml]>=7.2.2; extra == "dev"
 Requires-Dist: pdm>=2.4.9; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
```

