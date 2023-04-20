# Comparing `tmp/pre_commit_update-0.0.5.tar.gz` & `tmp/pre_commit_update-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit_update-0.0.5.tar", max compression
+gzip compressed data, was "pre_commit_update-0.0.6.tar", max compression
```

## Comparing `pre_commit_update-0.0.5.tar` & `pre_commit_update-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1058 2023-01-31 22:07:02.485087 pre_commit_update-0.0.5/LICENSE
--rw-r--r--   0        0        0     3046 2023-01-31 22:05:51.622492 pre_commit_update-0.0.5/README.md
--rw-r--r--   0        0        0     1603 2023-01-31 22:07:02.511754 pre_commit_update-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-08 18:52:38.743777 pre_commit_update-0.0.5/src/pre_commit_update/__init__.py
--rw-r--r--   0        0        0     4384 2023-01-31 22:09:34.783506 pre_commit_update-0.0.5/src/pre_commit_update/cli.py
--rw-r--r--   0        0        0        0 2022-04-01 23:18:33.555504 pre_commit_update-0.0.5/src/pre_commit_update/py.typed
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 pre_commit_update-0.0.5/setup.py
--rw-r--r--   0        0        0     4829 1970-01-01 00:00:00.000000 pre_commit_update-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-01-31 22:07:02.485087 pre_commit_update-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3643 2023-04-20 21:34:05.787878 pre_commit_update-0.0.6/README.md
+-rw-r--r--   0        0        0     1603 2023-04-20 22:00:19.597647 pre_commit_update-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-08 18:52:38.743777 pre_commit_update-0.0.6/src/pre_commit_update/__init__.py
+-rw-r--r--   0        0        0     5098 2023-04-20 21:34:08.321191 pre_commit_update-0.0.6/src/pre_commit_update/cli.py
+-rw-r--r--   0        0        0        0 2022-04-01 23:18:33.555504 pre_commit_update-0.0.6/src/pre_commit_update/py.typed
+-rw-r--r--   0        0        0     4715 1970-01-01 00:00:00.000000 pre_commit_update-0.0.6/setup.py
+-rw-r--r--   0        0        0     5426 1970-01-01 00:00:00.000000 pre_commit_update-0.0.6/PKG-INFO
```

### Comparing `pre_commit_update-0.0.5/LICENSE` & `pre_commit_update-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.0.5/pyproject.toml` & `pre_commit_update-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pre-commit-update"
-version = "0.0.5"
+version = "0.0.6"
 description = "Simple CLI tool to check and update pre-commit hooks."
 authors = ["Vojko Pribudić <dmanthing@gmail.com>"]
 maintainers = ["Vojko Pribudić <dmanthing@gmail.com>"]
 repository = "https://gitlab.com/vojko.pribudic/pre-commit-update"
 readme = "README.md"
 license = "MIT"
 classifiers = [
```

### Comparing `pre_commit_update-0.0.5/src/pre_commit_update/cli.py` & `pre_commit_update-0.0.6/src/pre_commit_update/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,51 +49,65 @@
             parsed_tag = parsed_tag.replace("refs/tags/", "")
             tags.append(parsed_tag)
         return tags
     except GitCommandError:
         raise Exception(f"No tags found for repo: {url}")
 
 
-def run(dry_run: bool, all_versions: bool, verbose: bool, exclude: tuple) -> None:
+def run(
+    dry_run: bool, all_versions: bool, verbose: bool, exclude: tuple, keep: tuple
+) -> None:
     os.environ["GIT_TERMINAL_PROMPT"] = "0"
     try:
         file_path: str = os.path.join(os.getcwd(), ".pre-commit-config.yaml")
         yaml_str: str = _read_yaml_file(file_path)
         data: Any = load(yaml_str, Loader)
         no_diff: list = []
         diff: list = []
         ignored: list = []
+        kept: list = []
 
         with ThreadPoolExecutor(max_workers=10) as pool:
             tasks: list = []
             for i in range(len(data["repos"])):
                 rep: dict = data["repos"][i]
                 tasks.append(pool.submit(_parse_tags, rep))
 
         for i, repository in enumerate(data["repos"]):
             if not repository["repo"].startswith("http"):
                 continue
             rep = data["repos"][i]
-            hook: str = rep["repo"].split("/")[-1]
+            repo_name: str = rep["repo"].split("/")[-1]
             tag_versions: list = tasks[i].result()
             tag_versions.reverse()
             target_ver: str = _get_target_tag(tag_versions, all_versions)
-            if any(ex.get("id", "N/A") in exclude for ex in rep["hooks"]):
-                ignored.append(f"{hook} - {_colorize(rep['rev'] + ' ★', 'magenta')}")
+            if repo_name in exclude:
+                ignored.append(
+                    f"{repo_name} - {_colorize(rep['rev'] + ' ★', 'magenta')}"
+                )
+                continue
+            if repo_name in keep:
+                if rep["rev"] != target_ver:
+                    kept.append(
+                        f"{repo_name} - {_colorize(rep['rev'] + ' -> ' + target_ver + ' ◉', 'blue')}"
+                    )
+                else:
+                    kept.append(f"{repo_name} - {_colorize(rep['rev'] + ' ◉', 'blue')}")
                 continue
             if rep["rev"] != target_ver:
                 diff.append(
-                    f"{hook} - {_colorize(rep['rev'], 'yellow')} -> {_colorize(target_ver + ' ✘', 'red')}"
+                    f"{repo_name} - {_colorize(rep['rev'], 'yellow')} -> {_colorize(target_ver + ' ✘', 'red')}"
                 )
                 data["repos"][i]["rev"] = target_ver
             else:
-                no_diff.append(f"{hook} - {_colorize(rep['rev'] + ' ✔', 'green')}")
+                no_diff.append(f"{repo_name} - {_colorize(rep['rev'] + ' ✔', 'green')}")
 
         if verbose:
             click.echo("\n".join(ignored))
+            click.echo("\n".join(kept))
             click.echo("\n".join(no_diff))
 
         if diff:
             click.echo("\n".join(diff))
             if not dry_run:
                 _save_yaml_file(".pre-commit-config.yaml", data)
                 click.echo(_colorize("Changes detected and applied", "green"))
@@ -109,38 +123,45 @@
 @click.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.option(
     "-d",
     "--dry-run",
     is_flag=True,
     show_default=True,
     default=False,
-    help="Dry run only checks for the new versions",
+    help="Dry run only checks for the new versions without updating",
 )
 @click.option(
     "-a",
     "--all-versions",
     is_flag=True,
     show_default=True,
     default=False,
-    help="Include the alpha/beta versions",
+    help="Include the alpha/beta versions when updating",
 )
 @click.option(
     "-v",
     "--verbose",
     is_flag=True,
     show_default=True,
     default=False,
     help="Display the complete output",
 )
 @click.option(
     "-e",
     "--exclude",
     multiple=True,
     default=[],
-    help="Exclude specific hook(s) by the `id` of a hook",
+    help="Exclude specific repo(s) by the `repo` url trim",
+)
+@click.option(
+    "-k",
+    "--keep",
+    multiple=True,
+    default=[],
+    help="Keep the version of specific repo(s) by the `repo` url trim (still checks for the new versions)",
 )
-def cli(dry_run: bool, all_versions: bool, verbose: bool, exclude: tuple):
-    run(dry_run, all_versions, verbose, exclude)
+def cli(dry_run: bool, all_versions: bool, verbose: bool, exclude: tuple, keep: tuple):
+    run(dry_run, all_versions, verbose, exclude, keep)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `pre_commit_update-0.0.5/setup.py` & `pre_commit_update-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['GitPython>=3.1.29,<4.0.0', 'click>=8.1,<9.0', 'pyyaml>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['pre-commit-update = pre_commit_update.cli:cli']}
 
 setup_kwargs = {
     'name': 'pre-commit-update',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'Simple CLI tool to check and update pre-commit hooks.',
-    'long_description': '# pre-commit-update\n\n![Version](https://img.shields.io/pypi/pyversions/pre-commit-update)\n![Downloads](https://pepy.tech/badge/pre-commit-update)\n![Formatter](https://img.shields.io/badge/code%20style-black-black)\n![License](https://img.shields.io/pypi/l/pre-commit-update)\n\n**pre-commit-update** is a simple CLI tool to check and update pre-commit hooks.\n\n## Table of contents\n\n1. [ Reasoning ](#reasoning)\n2. [ Installation ](#installation)\n3. [ Usage ](#usage)\n    1. [ Pipeline usage example ](#usage-pipeline)\n    2. [ pre-commit hook usage example ](#usage-hook)\n\n<a name="reasoning"></a>\n## 1. Reasoning\n\n`pre-commit` is a nice little tool that helps you polish your code before releasing it into the wild.\nIt is fairly easy to use. A single `pre-commit-config.yaml` file can hold multiple hooks (checks) that will go through\nyour code or repository and do certain checks. The trick is that file is static and once you pin your hook versions\nafter a while they get outdated.\n\n`pre-commit` has a CLI that helps with that by making use of `pre-commit autoupdate` command so the question is\nwhy the f* are you reading this?\n\n`pre-commit-update` was created mostly because there is no easy way to update your hooks by using\n`pre-commit autoupdate` and avoiding non-stable (alpha, beta, ...) hook versions. `pre-commit-update` comes\nwith a CLI that can be configured to solve that problem - along with other use cases.\n\nOther than that - I was bored ^^\n\n\n<a name="installation"></a>\n## 2. Installation\n\n`pre-commit-update` is available on PyPI:\n```console \n$ python -m pip install pre-commit-update\n```\nPython >= 3.7 is supported.\n\n*NOTE:* Please make sure that `git` is installed.\n\n\n<a name="usage"></a>\n## 3. Usage\n\n`pre-commit-update` CLI can be used as below:\n\n```console\nUsage: pre-commit-update [OPTIONS]\n\nOptions:\n  -d, --dry-run       Dry run only checks for the new versions\n  -a, --all-versions  Include the alpha/beta versions\n  -v, --verbose       Display the complete output\n  -e, --exclude TEXT  Exclude specific hook(s) by the `id` of a hook\n  -h, --help          Show this message and exit.\n```\n\nIf you want to just check for updates (without updating `pre-commit-config.yaml`), for example, you would use:\n```python\npre-commit-update -d\nOR\npre-commit-update --dry-run\n```\n\n<a name="usage-pipeline"></a>\n### Pipeline usage example\n#### GitLab job:\n\n```yaml\npre-commit-hooks-update:\n  stage: update\n  script:\n    # install git if not present in the image\n    - pip install pre-commit-update\n    - pre-commit-update --dry-run\n  except:\n    - main\n  when: manual\n  allow_failure: true\n```\n\n*NOTE*: This is just an example, feel free to do your own configuration\n\n<a name="usage-hook"></a>\n### pre-commit hook usage example\n\nYou can also use `pre-commit-update` as a hook in your `pre-commit` hooks:\n\n```yaml\n- repo: local\n  hooks:\n    - id: pre-commit-update\n      entry: pre-commit-update\n      language: python\n      name: pre-commit-update\n      pass_filenames: false\n      args: [--dry-run --exclude black --exclude isort]\n```\n',
+    'long_description': '# pre-commit-update\n\n![Version](https://img.shields.io/pypi/pyversions/pre-commit-update)\n![Downloads](https://pepy.tech/badge/pre-commit-update)\n![Formatter](https://img.shields.io/badge/code%20style-black-black)\n![License](https://img.shields.io/pypi/l/pre-commit-update)\n\n**pre-commit-update** is a simple CLI tool to check and update pre-commit hooks.\n\n## Table of contents\n\n1. [ Reasoning ](#reasoning)\n2. [ Installation ](#installation)\n3. [ Usage ](#usage)\n    1. [ Pipeline usage example ](#usage-pipeline)\n    2. [ pre-commit hook usage example ](#usage-hook)\n\n<a name="reasoning"></a>\n## 1. Reasoning\n\n`pre-commit` is a nice little tool that helps you polish your code before releasing it into the wild.\nIt is fairly easy to use. A single `pre-commit-config.yaml` file can hold multiple hooks (checks) that will go through\nyour code or repository and do certain checks. The trick is that file is static and once you pin your hook versions\nafter a while they get outdated.\n\n`pre-commit` has a CLI that helps with that by making use of `pre-commit autoupdate` command so the question is\nwhy the f* are you reading this?\n\n`pre-commit-update` was created mostly because there is no easy way to update your hooks by using\n`pre-commit autoupdate` and avoiding non-stable (alpha, beta, ...) hook versions. `pre-commit-update` comes\nwith a CLI that can be configured to solve that problem - along with other use cases.\n\nOther than that - I was bored ^^\n\n\n<a name="installation"></a>\n## 2. Installation\n\n`pre-commit-update` is available on PyPI:\n```console \n$ python -m pip install pre-commit-update\n```\nPython >= 3.7 is supported.\n\n**NOTE:** Please make sure that `git` is installed.\n\n\n<a name="usage"></a>\n## 3. Usage\n\n`pre-commit-update` CLI can be used as below:\n\n```console\nUsage: pre-commit-update [OPTIONS]\n\nOptions:\n  -d, --dry-run       Dry run only checks for the new versions without\n                      updating\n  -a, --all-versions  Include the alpha/beta versions when updating\n  -v, --verbose       Display the complete output\n  -e, --exclude TEXT  Exclude specific repo(s) by the `repo` url trim\n  -k, --keep TEXT     Keep the version of specific repo(s) by the `repo` url trim (still checks for the new versions)\n  -h, --help          Show this message and exit.\n```\n\nIf you want to just check for updates (without updating `pre-commit-config.yaml`), for example, you would use:\n```python\npre-commit-update -d\nOR\npre-commit-update --dry-run\n```\n\n**NOTE:** If you are to use the `exclude` or `keep` options, please pass the repo url trim as a parameter.\nKeep in mind that if you have multiple hooks (id\'s) configured for a single repo and you `exclude` that repo,\n**NONE** of the hooks will be updated, whole repo will be excluded.\n\nExample of repo url trim: https://github.com/ambv/black -> `black` (you will only pass `black` as a parameter to\n`exclude` or `keep`)\n\n<a name="usage-pipeline"></a>\n### Pipeline usage example\n#### GitLab job:\n\n```yaml\npre-commit-hooks-update:\n  stage: update\n  script:\n    # install git if not present in the image\n    - pip install pre-commit-update\n    - pre-commit-update --dry-run\n  except:\n    - main\n  when: manual\n  allow_failure: true\n```\n\n**NOTE:** This is just an example, feel free to do your own configuration\n\n<a name="usage-hook"></a>\n### pre-commit hook usage example\n\nYou can also use `pre-commit-update` as a hook in your `pre-commit` hooks:\n\n```yaml\n- repo: local\n  hooks:\n    - id: pre-commit-update\n      entry: pre-commit-update\n      language: python\n      name: pre-commit-update\n      pass_filenames: false\n      args: [--dry-run --exclude black --exclude isort]\n```\n',
     'author': 'Vojko Pribudić',
     'author_email': 'dmanthing@gmail.com',
     'maintainer': 'Vojko Pribudić',
     'maintainer_email': 'dmanthing@gmail.com',
     'url': 'https://gitlab.com/vojko.pribudic/pre-commit-update',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pre_commit_update-0.0.5/PKG-INFO` & `pre_commit_update-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-commit-update
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple CLI tool to check and update pre-commit hooks.
 Home-page: https://gitlab.com/vojko.pribudic/pre-commit-update
 License: MIT
 Author: Vojko Pribudić
 Author-email: dmanthing@gmail.com
 Maintainer: Vojko Pribudić
 Maintainer-email: dmanthing@gmail.com
@@ -78,40 +78,49 @@
 
 `pre-commit-update` is available on PyPI:
 ```console 
 $ python -m pip install pre-commit-update
 ```
 Python >= 3.7 is supported.
 
-*NOTE:* Please make sure that `git` is installed.
+**NOTE:** Please make sure that `git` is installed.
 
 
 <a name="usage"></a>
 ## 3. Usage
 
 `pre-commit-update` CLI can be used as below:
 
 ```console
 Usage: pre-commit-update [OPTIONS]
 
 Options:
-  -d, --dry-run       Dry run only checks for the new versions
-  -a, --all-versions  Include the alpha/beta versions
+  -d, --dry-run       Dry run only checks for the new versions without
+                      updating
+  -a, --all-versions  Include the alpha/beta versions when updating
   -v, --verbose       Display the complete output
-  -e, --exclude TEXT  Exclude specific hook(s) by the `id` of a hook
+  -e, --exclude TEXT  Exclude specific repo(s) by the `repo` url trim
+  -k, --keep TEXT     Keep the version of specific repo(s) by the `repo` url trim (still checks for the new versions)
   -h, --help          Show this message and exit.
 ```
 
 If you want to just check for updates (without updating `pre-commit-config.yaml`), for example, you would use:
 ```python
 pre-commit-update -d
 OR
 pre-commit-update --dry-run
 ```
 
+**NOTE:** If you are to use the `exclude` or `keep` options, please pass the repo url trim as a parameter.
+Keep in mind that if you have multiple hooks (id's) configured for a single repo and you `exclude` that repo,
+**NONE** of the hooks will be updated, whole repo will be excluded.
+
+Example of repo url trim: https://github.com/ambv/black -> `black` (you will only pass `black` as a parameter to
+`exclude` or `keep`)
+
 <a name="usage-pipeline"></a>
 ### Pipeline usage example
 #### GitLab job:
 
 ```yaml
 pre-commit-hooks-update:
   stage: update
@@ -121,15 +130,15 @@
     - pre-commit-update --dry-run
   except:
     - main
   when: manual
   allow_failure: true
 ```
 
-*NOTE*: This is just an example, feel free to do your own configuration
+**NOTE:** This is just an example, feel free to do your own configuration
 
 <a name="usage-hook"></a>
 ### pre-commit hook usage example
 
 You can also use `pre-commit-update` as a hook in your `pre-commit` hooks:
 
 ```yaml
```

