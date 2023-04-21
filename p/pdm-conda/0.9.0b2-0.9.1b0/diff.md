# Comparing `tmp/pdm_conda-0.9.0b2.tar.gz` & `tmp/pdm_conda-0.9.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.9.0b2.tar", last modified: Wed Apr 19 18:21:51 2023, max compression
+gzip compressed data, was "pdm_conda-0.9.1b0.tar", last modified: Fri Apr 21 13:49:14 2023, max compression
```

## Comparing `pdm_conda-0.9.0b2.tar` & `pdm_conda-0.9.1b0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.0b2/LICENSE
--rw-r--r--   0        0        0     5649 2023-04-19 17:36:40.659039 pdm_conda-0.9.0b2/README.md
--rw-r--r--   0        0        0     1979 2023-04-19 18:21:51.984162 pdm_conda-0.9.0b2/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-19 18:21:34.158877 pdm_conda-0.9.0b2/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.0b2/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.0b2/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3087 2023-04-19 15:05:35.481829 pdm_conda-0.9.0b2/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.0b2/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.9.0b2/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    14710 2023-04-19 18:21:22.125888 pdm_conda-0.9.0b2/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.0b2/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.9.0b2/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2307 2023-04-18 22:35:19.397503 pdm_conda-0.9.0b2/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3043 2023-04-18 01:05:14.781588 pdm_conda-0.9.0b2/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.0b2/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.0b2/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     7946 2023-04-18 23:13:02.100650 pdm_conda-0.9.0b2/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     1818 2023-04-18 01:05:14.782254 pdm_conda-0.9.0b2/src/pdm_conda/models/conda.py
--rw-r--r--   0        0        0     8612 2023-04-18 23:02:22.362754 pdm_conda-0.9.0b2/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3095 2023-04-19 17:13:01.223457 pdm_conda-0.9.0b2/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     6581 2023-04-19 14:41:57.331734 pdm_conda-0.9.0b2/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0    11268 2023-04-18 23:02:59.727692 pdm_conda-0.9.0b2/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.9.0b2/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     8311 2023-04-19 18:14:37.792025 pdm_conda-0.9.0b2/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.0b2/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     2418 2023-04-18 22:33:52.217660 pdm_conda-0.9.0b2/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     8575 2023-04-19 16:34:29.164097 pdm_conda-0.9.0b2/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.0b2/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     7497 1970-01-01 00:00:00.000000 pdm_conda-0.9.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.1b0/LICENSE
+-rw-r--r--   0        0        0     5649 2023-04-19 19:04:02.148249 pdm_conda-0.9.1b0/README.md
+-rw-r--r--   0        0        0     1979 2023-04-21 13:49:14.694094 pdm_conda-0.9.1b0/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-21 13:49:03.960609 pdm_conda-0.9.1b0/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.1b0/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.1b0/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3087 2023-04-19 19:04:02.150645 pdm_conda-0.9.1b0/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.1b0/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     3009 2023-04-21 13:41:55.576203 pdm_conda-0.9.1b0/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    15656 2023-04-21 13:47:33.761660 pdm_conda-0.9.1b0/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.1b0/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2613 2023-04-21 13:39:15.232993 pdm_conda-0.9.1b0/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2307 2023-04-19 19:04:02.152461 pdm_conda-0.9.1b0/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3043 2023-04-19 19:04:02.153381 pdm_conda-0.9.1b0/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.1b0/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.1b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     7463 2023-04-21 13:38:37.339450 pdm_conda-0.9.1b0/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1818 2023-04-19 19:04:02.154757 pdm_conda-0.9.1b0/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     8612 2023-04-19 19:04:02.155447 pdm_conda-0.9.1b0/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3095 2023-04-19 19:04:02.155978 pdm_conda-0.9.1b0/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     6740 2023-04-21 13:42:34.892731 pdm_conda-0.9.1b0/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0    11268 2023-04-19 19:04:02.157597 pdm_conda-0.9.1b0/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.9.1b0/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8311 2023-04-19 19:04:02.158361 pdm_conda-0.9.1b0/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.1b0/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     2418 2023-04-19 19:04:02.159092 pdm_conda-0.9.1b0/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     8601 2023-04-19 19:04:02.159990 pdm_conda-0.9.1b0/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.1b0/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     7497 1970-01-01 00:00:00.000000 pdm_conda-0.9.1b0/PKG-INFO
```

### Comparing `pdm_conda-0.9.0b2/LICENSE` & `pdm_conda-0.9.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/README.md` & `pdm_conda-0.9.1b0/README.md`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/pyproject.toml` & `pdm_conda-0.9.1b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "pdm~=2.4.0",
     "requests>=2.28.1",
 ]
-version = "0.9.0b2"
+version = "0.9.1b0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
```

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/__init__.py` & `pdm_conda-0.9.1b0/src/pdm_conda/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.9.0b2"
+__version__ = "0.9.1b0"
```

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.9.1b0/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.9.1b0/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/cli/utils.py` & `pdm_conda-0.9.1b0/src/pdm_conda/cli/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import functools
 
 from pdm.models.candidates import Candidate
 from pdm.models.requirements import Requirement
 from pdm.project import Project
 
+from pdm_conda.models.candidates import CondaCandidate
 from pdm_conda.models.requirements import CondaRequirement
 
 _patched = False
 
 
 def remove_quotes(req: str) -> str:
     for quote in ("'", '"'):
@@ -40,20 +41,38 @@
         mapping: dict[str, Candidate],
         fetched_dependencies: dict[tuple[str, str | None], list[Requirement]],
     ) -> dict:
         for deps in fetched_dependencies.values():
             for i, dep in enumerate(deps):
                 if isinstance(dep, CondaRequirement):
                     setattr(dep, "as_line", functools.partial(dep.as_line, with_build_string=True))
-        res = func(project, mapping, fetched_dependencies)
-        for deps in fetched_dependencies.values():
-            for i, dep in enumerate(deps):
-                if isinstance(dep, CondaRequirement):
-                    setattr(dep, "as_line", dep.as_line.func)  # type: ignore
-        return res
+        version_mapping = {}
+        for name, can in mapping.items():
+            if isinstance(can, CondaCandidate):
+                fetched_dependencies[(can.name, can.conda_version)] = fetched_dependencies.pop(
+                    (can.name, can.version),
+                    [],
+                )
+                version_mapping[name] = can.version
+                can.version = can.conda_version
+        try:
+            res = func(project, mapping, fetched_dependencies)
+            return res
+        finally:
+            for deps in fetched_dependencies.values():
+                for i, dep in enumerate(deps):
+                    if isinstance(dep, CondaRequirement):
+                        setattr(dep, "as_line", dep.as_line.func)  # type: ignore
+            for name, version in version_mapping.items():
+                can = mapping[name]
+                can.version = version
+                fetched_dependencies[(can.name, can.version)] = fetched_dependencies.pop(
+                    (can.name, can.conda_version),
+                    [],
+                )
 
     return wrapper
 
 
 if not _patched:
     from pdm.cli import actions, utils
```

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/conda.py` & `pdm_conda-0.9.1b0/src/pdm_conda/conda.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 from functools import lru_cache
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Iterable
 
 from pdm import termui
 from pdm.cli.commands.venv.backends import VirtualenvCreateError
-from pdm.exceptions import PdmException, RequirementError
+from pdm.exceptions import (
+    InstallationError,
+    PdmException,
+    RequirementError,
+    UninstallError,
+)
 from pdm.models.setup import Setup
 from pdm.termui import Verbosity
 
 from pdm_conda.models.candidates import CondaCandidate, parse_channel
 from pdm_conda.models.conda import ChannelSorter
 from pdm_conda.models.config import CondaRunner
 from pdm_conda.models.requirements import (
@@ -28,22 +33,22 @@
 
 
 class CondaResolutionError(PdmException):
     pass
 
 
 @contextlib.contextmanager
-def _optional_temporary_file(environment: dict):
+def _optional_temporary_file(environment: dict | list):
     """
     If environment contains data then creates temporary file else yield None
     :param environment: environment data
     :return: Temporary file or None
     """
     if environment:
-        with NamedTemporaryFile(mode="w+", suffix=".yml") as f:
+        with NamedTemporaryFile(mode="w+", suffix=".yml" if isinstance(environment, dict) else ".lock") as f:
             yield f
     else:
         yield
 
 
 def run_conda(
     cmd,
@@ -52,31 +57,35 @@
     **environment,
 ) -> dict:
     """
     Optionally creates temporary environment file and run conda command
     :param cmd: conda command
     :param exception_cls: exception to raise on error
     :param exception_msg: base message to show on error
-    :param environment: environment data
+    :param environment: environment or lockfile data
     :return: conda command response
     """
-    with _optional_temporary_file(environment) as f:
-        if environment:
-            for name, options in environment.items():
-                if options:
-                    f.write(f"{name}:")
-                    if isinstance(options, str):
-                        f.write(f" {options}\n")
-                        continue
-                    else:
-                        f.write("\n")
-                    for v in options:
-                        f.write(f"  - {v}\n")
+    lockfile = environment.get("lockfile", [])
+    with _optional_temporary_file(lockfile or environment) as f:
+        if lockfile or environment:
+            if lockfile:
+                f.writelines(lockfile)
+            elif environment:
+                for name, options in environment.items():
+                    if options:
+                        f.write(f"{name}:")
+                        if isinstance(options, str):
+                            f.write(f" {options}\n")
+                            continue
+                        else:
+                            f.write("\n")
+                        for v in options:
+                            f.write(f"  - {v}\n")
             f.seek(0)
-            cmd = cmd + ["-f", f.name]
+            cmd = cmd + ["--file", f.name]
         logger.debug(f"cmd: {' '.join(cmd)}")
         if environment:
             logger.debug(f"env: {environment}")
         process = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, encoding="utf-8")
     if "--json" in cmd:
         try:
             response = json.loads(process.stdout)
@@ -181,15 +190,15 @@
 
 
 @lru_cache(maxsize=None)
 def _conda_search(
     project: CondaProject,
     requirement: str,
     channels: tuple[str],
-) -> list[CondaCandidate]:
+) -> list[dict]:
     """
     Search conda candidates for a requirement
     :param project: PDM project
     :param requirement: requirement
     :param channels: requirement channels
     :return: list of conda candidates
     """
@@ -210,41 +219,44 @@
         else:
             raise
 
     if config.runner == CondaRunner.CONDA:
         packages = result.get(parse_requirement(f"conda:{requirement}").name, [])
     else:
         packages = result.get("result", dict()).get("pkgs", [])
-
-    return _parse_candidates(project, packages=packages)
+    return packages
 
 
 def conda_search(
     project: CondaProject,
     requirement: CondaRequirement | str,
     channel: str | None = None,
 ) -> list[CondaCandidate]:
     """
     Search conda candidates for a requirement
     :param project: PDM project
     :param requirement: requirement
     :param channel: requirement channel
     :return: list of conda candidates
     """
-    if isinstance(requirement, CondaRequirement):
-        channel = channel or requirement.channel
-        requirement = requirement.as_line(with_build_string=True, conda_compatible=True).replace(" ", "=")
-    if "::" in requirement:
-        channel, requirement = requirement.split("::", maxsplit=1)
+    _requirement = requirement
+    if isinstance(_requirement, CondaRequirement):
+        channel = channel or _requirement.channel
+        _requirement = _requirement.as_line(with_build_string=True, conda_compatible=True).replace(" ", "=")
+    if "::" in _requirement:
+        channel, _requirement = _requirement.split("::", maxsplit=1)
+    if isinstance(requirement, str):
+        requirement = parse_requirement(f"conda::{requirement}")
     channels = _ensure_channels(
         project,
         [channel] if channel else [],
         f"No channel specified for searching [req]{requirement}[/] using defaults if exist.",
     )
-    return _conda_search(project, requirement, tuple(channels))
+    packages = _conda_search(project, _requirement, tuple(channels))
+    return _parse_candidates(project, packages, requirement)
 
 
 def conda_create(
     project: CondaProject,
     requirements: list[CondaRequirement],
     channels: list[str] | None = None,
     prefix: Path | str | None = None,
@@ -303,44 +315,56 @@
     fetch_packages = {pkg["name"]: pkg for pkg in actions.get("FETCH", [])}
     packages = actions.get("LINK", [])
     for i, pkg in enumerate(packages):
         pkg = fetch_packages.get(pkg["name"], pkg)
         if any(True for n in ("constrains", "depends") if n not in pkg):
             pkg = conda_search(
                 project,
-                f'{pkg["name"]} {pkg["version"]} {pkg["build_string"]}',
+                f'{pkg["name"]}={pkg["version"]}={pkg["build_string"]}',
                 parse_channel(pkg["channel"]),
-            )[0]
+            )
         packages[i] = pkg
 
     _requirements = {req.conda_name: req for req in requirements}
     for pkg in packages:
-        name = pkg["name"]
-        candidates[name] = _parse_candidates(
-            project,
-            packages=[pkg],
-            requirement=_requirements.get(name, None),
-        )
+        # if is list of candidates then it comes from search
+        if isinstance(pkg, list):
+            if pkg:
+                candidates[pkg[0].name] = pkg
+        else:
+            name = pkg["name"]
+            candidates[name] = _parse_candidates(
+                project,
+                packages=[pkg],
+                requirement=_requirements.get(name, None),
+            )
     return candidates
 
 
 def _conda_install(
-    project: CondaProject,
     command: list[str],
     packages: str | list[str] | None = None,
+    exception_cls: type[PdmException] = InstallationError,
     dry_run: bool = False,
+    explicit: bool = False,
 ):
     if isinstance(packages, str):
         packages = [packages]
-    if packages:
+    if not packages:
+        raise exception_cls(f"No packages used for {' '.join(command[:3])} command.")
+    if explicit:
+        packages.insert(0, "@EXPLICIT")
+    else:
         command.extend(packages)
     if dry_run:
         command.append("--dry-run")
-    response = run_conda(command + ["--json"])
-    project.core.ui.echo(response, verbosity=Verbosity.DEBUG)
+    kwargs: dict = dict()
+    if explicit:
+        kwargs["lockfile"] = packages
+    run_conda(command + ["--json"], **kwargs)
 
 
 def conda_install(
     project: CondaProject,
     packages: str | list[str],
     dry_run: bool = False,
     no_deps: bool = False,
@@ -361,15 +385,15 @@
 
     if config.installation_method == "copy":
         _copy = "copy"
         if config.runner == CondaRunner.MICROMAMBA:
             _copy = f"always-{_copy}"
         command.append(f"--{_copy}")
 
-    _conda_install(project, command, packages, dry_run=dry_run)
+    _conda_install(command, packages, dry_run=dry_run, explicit=True)
 
 
 def conda_uninstall(
     project: CondaProject,
     packages: str | list[str],
     dry_run: bool = False,
     no_deps: bool = False,
@@ -389,15 +413,15 @@
         command = config.command("remove")
 
     if no_deps:
         if config.runner == CondaRunner.MICROMAMBA:
             command.append("--no-prune")
         command.append("--force")
 
-    _conda_install(project, command, packages, dry_run=dry_run)
+    _conda_install(command, packages, dry_run=dry_run, exception_cls=UninstallError)
 
 
 def not_initialized_warning(project):
     project.core.ui.echo(
         "[warning]Tried to execute a conda command but no pdm-conda configs were found on pyproject.toml.[/]",
     )
```

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/installers/manager.py` & `pdm_conda-0.9.1b0/src/pdm_conda/installers/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,19 @@
         Install candidate, use conda if conda package else default installer
         :param candidate: candidate to install
         """
         if isinstance(candidate, CondaCandidate):
             try:
                 self._batch_install.append(candidate)
                 if len(self._batch_install) >= self._num_install:
-                    conda_install(self.environment.project, [c.link.url for c in self._batch_install], no_deps=True)
+                    conda_install(
+                        self.environment.project,
+                        [f"{c.link.url_without_fragment}#{c.link.hash}" for c in self._batch_install],
+                        no_deps=True,
+                    )
                     self._batch_install.clear()
             except (RequirementError, ValueError) as e:
                 raise InstallerError(e) from e
         else:
             super().install(candidate)
 
     def uninstall(self, dist: Distribution) -> None:
```

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.9.1b0/src/pdm_conda/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/mapping.py` & `pdm_conda-0.9.1b0/src/pdm_conda/mapping.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/models/candidates.py` & `pdm_conda-0.9.1b0/src/pdm_conda/models/candidates.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import functools
 import re
 from importlib.metadata import Distribution
 from pathlib import Path
 from typing import Any, cast
 from urllib.parse import urlparse
 
 from pdm.models.candidates import Candidate, PreparedCandidate
@@ -15,16 +14,14 @@
     Requirement,
     as_conda_requirement,
     parse_conda_version,
     parse_requirement,
 )
 from pdm_conda.models.setup import CondaSetupDistribution
 
-_patched = False
-
 
 def parse_channel(channel_url: str) -> str:
     """
     Parse channel from channel url
     :param channel_url: channel url from package
     :return: channel
     """
@@ -63,16 +60,19 @@
         channel: str | None = None,
         track_feature: str = "",
     ):
         super().__init__(req, name, version, link)
         self._req = cast(CondaRequirement, req)  # type: ignore
         self._preferred = None
         self._prepared: CondaPreparedCandidate | None = None
-        self.dependencies: list[CondaRequirement] = [parse_requirement(f"conda:{r}") for r in (dependencies or [])]
+        self.dependencies: list[CondaRequirement] = [
+            cast(CondaRequirement, parse_requirement(f"conda:{r}")) for r in (dependencies or [])
+        ]
         self.constrains: dict[str, CondaRequirement] = dict()
+        self.hashes = {self.link: f"{self.link.hash_name}:{self.link.hash}"}
         for r in constrains or []:
             c = cast(CondaRequirement, parse_requirement(f"conda:{r}"))
             self.constrains[str(c.conda_name)] = c
         self.build_string = build_string
         self.build_number = build_number
         self.timestamp = timestamp
         self.channel = channel
@@ -92,29 +92,28 @@
     @property
     def distribution(self):
         return CondaSetupDistribution(
             Setup(
                 name=self.name,
                 summary="",
                 version=self.version,
-                install_requires=[d.as_line(as_conda=True, with_build_string=True) for d in self.dependencies],
+                install_requires=self.dependencies_lines,
                 python_requires=self.requires_python,
             ),
         )
 
     @property
     def dependencies_lines(self):
         return [dep.as_line(as_conda=True, with_build_string=True, with_channel=True) for dep in self.dependencies]
 
     def as_lockfile_entry(self, project_root: Path) -> dict[str, Any]:
         result = super().as_lockfile_entry(project_root)
         result["conda_managed"] = True
         if self.link is None:
             raise ValueError("Uninitialized conda requirement")
-        result["url"] = self.link.url
         result["channel"] = self.channel
         if self.build_string is not None:
             result["build_string"] = self.build_string
         result["build_number"] = self.build_number
         if self.track_feature:
             result["track_feature"] = self.track_feature
         if self.constrains:
@@ -157,15 +156,15 @@
                 to_delete.append(d)
             elif match := re.match(r"python( .+|$)", d):
                 to_delete.append(d)
                 if requires_python is None:
                     requires_python = match.group(1).strip().split(" ")[0] or "*"
         for d in to_delete:
             dependencies.remove(d)
-        hashes = {h: package[h] for h in ["sha256", "md5"] if h in package}
+        hashes = {h: package[h] for h in ["md5"] if h in package}
         url = package["url"]
         for k, v in hashes.items():
             url += f"#{k}={v}"
         name, version = package["name"], package["version"]
         build_string = package.get("build", package.get("build_string", ""))
         channel = parse_channel(package["channel"])
         if requirement is not None:
@@ -197,23 +196,7 @@
         if self.req.is_named:
             return f"{self.name}@{self.conda_version}"
         return super().__str__()
 
     def format(self) -> str:
         """Format for output."""
         return f"[req]{self.name}[/] [warning]{self.conda_version}[/]"
-
-
-def wrap_as_lockfile_entry(func):
-    @functools.wraps(func)
-    def wrapper(self, *args, **kwargs) -> dict[str, Any]:
-        res = func(self, *args, **kwargs)
-        if (conda_name := self.req.conda_name) is not None and conda_name != self.name:
-            res["conda_name"] = conda_name
-        return res
-
-    return wrapper
-
-
-if not _patched:
-    setattr(Candidate, "as_lockfile_entry", wrap_as_lockfile_entry(Candidate.as_lockfile_entry))
-    _patched = True
```

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/models/conda.py` & `pdm_conda-0.9.1b0/src/pdm_conda/models/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/models/config.py` & `pdm_conda-0.9.1b0/src/pdm_conda/models/config.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/models/environment.py` & `pdm_conda-0.9.1b0/src/pdm_conda/models/environment.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/models/repositories.py` & `pdm_conda-0.9.1b0/src/pdm_conda/models/repositories.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Any, Iterable, Mapping, cast
 
 from pdm._types import Source
 from pdm.models.repositories import BaseRepository, LockedRepository, PyPIRepository
 from pdm.models.requirements import Requirement
 from pdm.models.specifiers import PySpecSet
 from pdm.resolver.python import PythonRequirement
-from unearth import Link
 
 from pdm_conda.conda import conda_create, sort_candidates
 from pdm_conda.models.candidates import Candidate, CondaCandidate
 from pdm_conda.models.environment import CondaEnvironment, Environment
 from pdm_conda.models.requirements import (
     CondaRequirement,
     NamedRequirement,
@@ -65,19 +64,14 @@
                         dependencies[i] = constrain
             requires_python = PySpecSet(candidate.requires_python)
             summary = candidate.summary
         else:
             dependencies, requires_python, summary = super().get_dependencies(candidate)
         return dependencies, requires_python, summary
 
-    def get_hashes(self, candidate: Candidate) -> dict[Link, str] | None:
-        if isinstance(candidate, CondaCandidate):
-            return None
-        return super().get_hashes(candidate)
-
 
 class PyPICondaRepository(PyPIRepository, CondaRepository):
     def update_conda_resolution(
         self,
         requirements: list[Requirement] | None = None,
         resolution: dict | None = None,
     ) -> list[CondaRequirement]:
@@ -132,21 +126,29 @@
             candidates = super()._find_candidates(requirement)
         return candidates
 
 
 class LockedCondaRepository(LockedRepository, CondaRepository):
     def _read_lockfile(self, lockfile: Mapping[str, Any]) -> None:
         packages = lockfile.get("package", [])
-        conda_packages = [p for p in packages if p.get("conda_managed", False)]
+        conda_packages = [copy(p) for p in packages if p.get("conda_managed", False)]
         packages = [p for p in packages if not p.get("conda_managed", False)]
-        super()._read_lockfile({"package": packages})
+        super()._read_lockfile({"package": packages, "metadata": lockfile.get("metadata", {})})
 
         for package in conda_packages:
+            link, _hash = list(self.file_hashes[(package["name"], package["version"])].items())[0]
+            name, value = _hash.split(":", maxsplit=1)
+            package[name] = value
+            package["url"] = link.url_without_fragment
             can = CondaCandidate.from_lock_package(package)
             can_id = self._identify_candidate(can)
             self.packages[can_id] = can
-            self.candidate_info[can_id] = (can.dependencies_lines, package.get("requires_python", ""), "")
+            self.candidate_info[can_id] = (
+                can.dependencies_lines,
+                package.get("requires_python", ""),
+                package.get("summary", ""),
+            )
 
     def _identify_candidate(self, candidate: Candidate) -> tuple:
         if isinstance(candidate, CondaCandidate):
             return candidate.identify(), candidate.version, None, False
         return super()._identify_candidate(candidate)
```

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/models/requirements.py` & `pdm_conda-0.9.1b0/src/pdm_conda/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/models/setup.py` & `pdm_conda-0.9.1b0/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/project.py` & `pdm_conda-0.9.1b0/src/pdm_conda/project.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.9.1b0/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/resolvers.py` & `pdm_conda-0.9.1b0/src/pdm_conda/resolvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                     # todo msg
                     self._add_to_criteria(criteria, constrain, parent=candidate)
 
     def _update_conda_resolution(self, criteria, parent) -> bool:
         requirements = [
             criterion.information[-1].requirement
             for i, criterion in criteria.items()
-            if i not in (CONDA_RESOLUTION_KEY, CONSTRAINS_KEY)
+            if i not in (CONDA_RESOLUTION_KEY, CONSTRAINS_KEY) and criterion.information
         ]
         if parent is not None:
             requirements.extend(self._p.get_dependencies(candidate=parent))
         self._ensure_criteria(criteria)
         changed = self._p.repository.update_conda_resolution(requirements, criteria[CONDA_RESOLUTION_KEY])
         for req in changed:
             self._add_to_criteria(criteria, req, parent)
```

### Comparing `pdm_conda-0.9.0b2/src/pdm_conda/utils.py` & `pdm_conda-0.9.1b0/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b2/PKG-INFO` & `pdm_conda-0.9.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.9.0b2
+Version: 0.9.1b0
 Summary: A PDM plugin to resolve/install/uninstall project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
```

