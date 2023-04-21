# Comparing `tmp/python_whiteprint-0.8.0.tar.gz` & `tmp/python_whiteprint-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_whiteprint-0.8.0.tar", max compression
+gzip compressed data, was "python_whiteprint-0.8.1.tar", max compression
```

## Comparing `python_whiteprint-0.8.0.tar` & `python_whiteprint-0.8.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0        0        0        0 2023-04-20 15:19:14.678068 python_whiteprint-0.8.0/LICENSES/
--rw-r--r--   0        0        0     4299 2023-04-20 15:19:14.678068 python_whiteprint-0.8.0/README.md
--rw-r--r--   0        0        0    30239 2023-04-20 15:19:35.018393 python_whiteprint-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      223 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/__init__.py
--rw-r--r--   0        0        0      162 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/__init__.py
--rwxr-xr-x   0        0        0      222 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/__main__.py
--rw-r--r--   0        0        0      786 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/_callback.py
--rw-r--r--   0        0        0      624 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/_click_app.py
--rw-r--r--   0        0        0     1198 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/_logging.py
--rw-r--r--   0        0        0     2130 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/entrypoint.py
--rw-r--r--   0        0        0    18375 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/init.py
--rw-r--r--   0        0        0      417 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/type.py
--rw-r--r--   0        0        0      322 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/console.py
--rw-r--r--   0        0        0      912 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/filesystem.py
--rw-r--r--   0        0        0     5306 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/git.py
--rw-r--r--   0        0        0      474 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/loc.py
--rw-r--r--   0        0        0      286 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/locale/base.pot
--rw-r--r--   0        0        0      100 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/locale/base.pot.license
--rw-r--r--   0        0        0      420 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      100 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po.license
--rw-r--r--   0        0        0     2402 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/nox.py
--rw-r--r--   0        0        0     1111 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/poetry.py
--rw-r--r--   0        0        0      199 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/py.typed
--rw-r--r--   0        0        0      294 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/version.py
--rw-r--r--   0        0        0     6219 1970-01-01 00:00:00.000000 python_whiteprint-0.8.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-21 15:42:55.672473 python_whiteprint-0.8.1/LICENSES/
+-rw-r--r--   0        0        0     4299 2023-04-21 15:42:55.672473 python_whiteprint-0.8.1/README.md
+-rw-r--r--   0        0        0    30239 2023-04-21 15:43:18.245028 python_whiteprint-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/__init__.py
+-rw-r--r--   0        0        0      162 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/cli/__init__.py
+-rwxr-xr-x   0        0        0      222 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/cli/__main__.py
+-rw-r--r--   0        0        0      786 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/cli/_callback.py
+-rw-r--r--   0        0        0      624 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/cli/_click_app.py
+-rw-r--r--   0        0        0     1198 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/cli/_logging.py
+-rw-r--r--   0        0        0     2130 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/cli/entrypoint.py
+-rw-r--r--   0        0        0    19057 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/cli/init.py
+-rw-r--r--   0        0        0      417 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/cli/type.py
+-rw-r--r--   0        0        0      322 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/console.py
+-rw-r--r--   0        0        0      912 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/filesystem.py
+-rw-r--r--   0        0        0     6895 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/git.py
+-rw-r--r--   0        0        0      474 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/loc.py
+-rw-r--r--   0        0        0      286 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/locale/base.pot
+-rw-r--r--   0        0        0      100 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/locale/base.pot.license
+-rw-r--r--   0        0        0      420 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      100 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po.license
+-rw-r--r--   0        0        0     2402 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/nox.py
+-rw-r--r--   0        0        0     1111 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/poetry.py
+-rw-r--r--   0        0        0      199 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/py.typed
+-rw-r--r--   0        0        0      294 2023-04-21 15:42:55.676473 python_whiteprint-0.8.1/src/python_whiteprint/version.py
+-rw-r--r--   0        0        0     6219 1970-01-01 00:00:00.000000 python_whiteprint-0.8.1/PKG-INFO
```

### Comparing `python_whiteprint-0.8.0/README.md` & `python_whiteprint-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.8.0/pyproject.toml` & `python_whiteprint-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: © 2023 Romain Brault <mail@romainbrault.com>
 #
 # SPDX-License-Identifier: MIT
 
 [tool.poetry]
 name = "python_whiteprint"
-version = "0.8.0"
+version = "0.8.1"
 description = "Generating Python projects using best practices"
 authors = [
     "Romain Brault <mail@romainbrault.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/RomainBrault/python-whiteprint"
```

### Comparing `python_whiteprint-0.8.0/src/python_whiteprint/cli/_callback.py` & `python_whiteprint-0.8.1/src/python_whiteprint/cli/_callback.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.8.0/src/python_whiteprint/cli/_click_app.py` & `python_whiteprint-0.8.1/src/python_whiteprint/cli/_click_app.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.8.0/src/python_whiteprint/cli/_logging.py` & `python_whiteprint-0.8.1/src/python_whiteprint/cli/_logging.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.8.0/src/python_whiteprint/cli/entrypoint.py` & `python_whiteprint-0.8.1/src/python_whiteprint/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.8.0/src/python_whiteprint/cli/init.py` & `python_whiteprint-0.8.1/src/python_whiteprint/cli/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,25 +186,27 @@
 def _post_processing(
     destination: pathlib.Path,
     *,
     default_venv_backend: DefaultVenvBackend,
     skip_tests: bool,
     python: Optional[str],
     github_token: Optional[str],
+    https_origin: bool,
 ) -> None:
     """Apply post processing steps after rendering the template wit Copier.
 
     Args:
         destination: path to the python project.
         default_venv_backend: default virtual environment backend for Nox.
         skip_tests: skip the Nox tests step.
         python: force using the given python interpreter for the post
             processing.
         github_token: Github Token to push the newly created repository to
             Github. The token must have writing permissions.
+        https_origin: force the origin to be an HTTPS URL.
     """
     git = importlib.import_module(
         "python_whiteprint.git",
         __package__,
     )
     nox = importlib.import_module(
         "python_whiteprint.nox",
@@ -262,19 +264,23 @@
 
     if github_token:
         copier_answers = read_yaml(destination / COPIER_ANSWER_FILE)
         git.setup_github_repository(
             repository,
             project_slug=copier_answers["project_slug"],
             github_token=github_token,
+            github_login=copier_answers["github_user"],
             labels=destination / LABEL_FILE,
         )
         git.protect_repository(
+            repository,
             project_slug=copier_answers["project_slug"],
             github_token=github_token,
+            github_login=copier_answers["github_user"],
+            https_origin=https_origin,
         )
 
 
 @beartype
 def _autocomplete_suffix(incomplete: pathlib.Path) -> List[str]:
     """Autocomplete by listing files with a YAML extension.
 
@@ -507,14 +513,22 @@
     help=_(
         "Github Token to push the newly created repository to Github. The"
         " token must have writing permissions."
     ),
     envvar="WHITEPRINT_GITHUB_TOKEN",
 )
 """see `python_whiteprint.cli.init.init` option `github_token`."""
+_option_https_origin = params.Option(
+    os.environ.get("WHITEPRINT_HTTPS_ORIGIN", False),
+    "--https-origin",
+    "-H",
+    envvar="WHITEPRINT_HTTPS_ORIGIN",
+    help=_("Force the origin to be an https URL."),
+)
+"""see `python_whiteprint.cli.init.init` option `https_origin`."""
 
 
 @beartype
 def _check_dict(data: Dict[str, Any]) -> TypeGuard[Dict[str, Union[str, int]]]:
     """Check if the values type of a given dictionary are strings or integers.
 
     Args:
@@ -544,14 +558,15 @@
     default_venv_backend: DefaultVenvBackend = _option_default_venv_backend,
     skip_tests: bool = _option_skip_tests,
     data: pathlib.Path = _option_data,
     no_data: bool = _option_no_data,
     user_defaults: Optional[pathlib.Path] = _option_user_defaults,
     python: Optional[str] = _option_python,
     github_token: Optional[str] = _option_github_token,
+    https_origin: bool = _option_https_origin,
 ) -> None:
     """Initalize a new Python project.
 
     This command mostly forwards copier's CLI. For more details see
     https://copier.readthedocs.io/en/stable/reference/cli/#copier.cli.CopierApp.
 
     Args:
@@ -579,14 +594,15 @@
         data: user data used to answer questions.
         no_data: force not using `--data`.
         user_defaults: user defaults choices.
         python: force using the given python interpreter for the post
             processing.
         github_token: Github Token to push the newly created repository to
             Github. The token must have writing permissions.
+        https_origin: force the origin to be an HTTPS URL.
     """
     data_dict = {} if no_data or data is None else read_yaml(data)
     data_dict.update(
         {
             "git_platform": (
                 "no_git_platform" if github_token is None else "github"
             )
@@ -616,8 +632,9 @@
 
     _post_processing(
         destination,
         default_venv_backend=default_venv_backend,
         skip_tests=skip_tests,
         python=python,
         github_token=github_token,
+        https_origin=https_origin,
     )
```

### Comparing `python_whiteprint-0.8.0/src/python_whiteprint/filesystem.py` & `python_whiteprint-0.8.1/src/python_whiteprint/filesystem.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.8.0/src/python_whiteprint/git.py` & `python_whiteprint-0.8.1/src/python_whiteprint/git.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pathlib
 from typing import Final
 
 import github
 import pygit2
 import yaml
 from beartype import beartype
-from beartype.typing import Iterable, Optional
+from beartype.typing import Iterable, Optional, Union
 
 
 HEAD: Final = "HEAD"
 """Git HEAD ref."""
 
 INITIAL_HEAD_NAME = "main"
 """Git default branch."""
@@ -129,35 +129,71 @@
         parents=[],
     )
 
     return repo
 
 
 @beartype
+def _find_entity(
+    github_user: github.AuthenticatedUser.AuthenticatedUser,
+    *,
+    github_login: str,
+) -> Union[
+    github.AuthenticatedUser.AuthenticatedUser,
+    github.Organization.Organization,
+]:
+    """Find and return an organization or user from the GitHub loging name.
+
+    Args:
+        github_user: an authenticated GitHub user.
+        github_login: the GitHub login name of the user or the organization
+            login.
+
+    Returns:
+        THe organization or user depending on the loging name.
+    """
+    organizations = [
+        organization
+        for organization in github_user.get_orgs()
+        if organization.login == github_login
+    ]
+    return organizations[0] if len(organizations) == 1 else github_user
+
+
+@beartype
 def setup_github_repository(
     repo: pygit2.repository.Repository,
     *,
     project_slug: str,
     github_token: str,
+    github_login: str,
     labels: pathlib.Path,
 ) -> None:
     """Create a repository on GitHub and push the local one.
 
     Args:
         repo: the local repository.
         project_slug: a slug of the project name.
         github_token: a GitHub token with repository write, delete, workflows
             and packages authorizations.
+        github_login: the GitHub login name of the user or the organization
+            login.
         labels: a path to a yaml file containing a list of labels with their
             descriptions.
     """
     github_user = github.Github(github_token, retry=3).get_user()
-    github_repository = github_user.create_repo(project_slug)
 
-    repo.remotes.set_url("origin", github_repository.clone_url)
+    github_repository = _find_entity(
+        github_user, github_login=github_login
+    ).create_repo(project_slug)
+
+    repo.remotes.set_url(
+        "origin",
+        github_repository.clone_url,
+    )
     repo.remotes.add_fetch("origin", "+refs/heads/*:refs/remotes/origin/*")
 
     logger = logging.getLogger(__name__)
     for label in yaml.safe_load(labels.read_text()):
         try:
             github_repository.create_label(**label)
         except github.GithubException as github_exception:
@@ -170,31 +206,49 @@
             credentials=pygit2.UserPass("x-access-token", github_token)
         ),
     )
 
 
 @beartype
 def protect_repository(
-    project_slug: str,
+    repo: pygit2.repository.Repository,
     *,
+    project_slug: str,
     github_token: str,
+    github_login: str,
+    https_origin: bool,
 ) -> None:
     """Protect a Github repository.
 
     Args:
+        repo: the local repository.
         project_slug: a slug of the project name (Repository to delete).
         github_token: a GitHub token with repository writing authorization.
+        github_login: the GitHub login name of the user or the organization
+            login.
+        https_origin: force the origin to be an HTTPS URL.
     """
     github_user = github.Github(github_token, retry=3).get_user()
-    github_repository = github_user.get_repo(project_slug)
+    github_repository = _find_entity(
+        github_user, github_login=github_login
+    ).get_repo(project_slug)
+
     branch = github_repository.get_branch(INITIAL_HEAD_NAME)
     branch.edit_protection(
         strict=True, enforce_admins=True, require_code_owner_reviews=True
     )
 
+    # We do not test coverage here as it is too complex for little gains (e.g.
+    # it requires the creation of an SSH key for the test session).
+    if not https_origin:  # pragma: no cover
+        repo.remotes.set_url(
+            "origin",
+            github_repository.ssh_url,
+        )
+
 
 def delete_github_repository(
     project_slug: str,
     *,
     github_token: str,
 ) -> None:
     """Delete a GitHub repository.
```

### Comparing `python_whiteprint-0.8.0/src/python_whiteprint/nox.py` & `python_whiteprint-0.8.1/src/python_whiteprint/nox.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.8.0/src/python_whiteprint/poetry.py` & `python_whiteprint-0.8.1/src/python_whiteprint/poetry.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.8.0/PKG-INFO` & `python_whiteprint-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-whiteprint
-Version: 0.8.0
+Version: 0.8.1
 Summary: Generating Python projects using best practices
 Home-page: https://github.com/RomainBrault/python-whiteprint
 License: MIT
 Keywords: Python,Cookiecutter,copier,template,rich,typer,nox,poetry,beartype,oci-image,container,docker,podman,ruff
 Author: Romain Brault
 Author-email: mail@romainbrault.com
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-whiteprint Version: 0.8.0 Summary:
+Metadata-Version: 2.1 Name: python-whiteprint Version: 0.8.1 Summary:
 Generating Python projects using best practices Home-page: https://github.com/
 RomainBrault/python-whiteprint License: MIT Keywords:
 Python,Cookiecutter,copier,template,rich,typer,nox,poetry,beartype,oci-
 image,container,docker,podman,ruff Author: Romain Brault Author-email:
 mail@romainbrault.com Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*,
 !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.* Classifier: Development
 Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
```

