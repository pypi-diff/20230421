# Comparing `tmp/ancv-1.2.3.tar.gz` & `tmp/ancv-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ancv-1.2.3.tar", max compression
+gzip compressed data, was "ancv-1.3.0.tar", max compression
```

## Comparing `ancv-1.2.3.tar` & `ancv-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-02-05 20:02:16.870418 ancv-1.2.3/LICENSE
--rw-r--r--   0        0        0    10301 2023-02-05 20:02:16.870418 ancv-1.2.3/README.md
--rw-r--r--   0        0        0      308 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/__init__.py
--rw-r--r--   0        0        0     8719 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/__main__.py
--rw-r--r--   0        0        0        0 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/data/__init__.py
--rw-r--r--   0        0        0        0 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/data/models/__init__.py
--rw-r--r--   0        0        0     3102 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/data/models/github.py
--rw-r--r--   0        0        0    13506 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/data/models/resume.py
--rw-r--r--   0        0        0     7803 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/data/showcase.resume.json
--rw-r--r--   0        0        0      932 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/data/validation.py
--rw-r--r--   0        0        0      250 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/py.typed
--rw-r--r--   0        0        0     3115 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/reflection.py
--rw-r--r--   0        0        0     1639 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/timing.py
--rw-r--r--   0        0        0      172 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/visualization/__init__.py
--rw-r--r--   0        0        0    30290 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/visualization/templates.py
--rw-r--r--   0        0        0     4199 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/visualization/themes.py
--rw-r--r--   0        0        0     2778 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/visualization/translations.py
--rw-r--r--   0        0        0        0 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/web/__init__.py
--rw-r--r--   0        0        0     4004 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/web/client.py
--rw-r--r--   0        0        0     8835 2023-02-05 20:02:16.870418 ancv-1.2.3/ancv/web/server.py
--rw-r--r--   0        0        0     2722 2023-02-05 20:02:16.878418 ancv-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    11587 1970-01-01 00:00:00.000000 ancv-1.2.3/setup.py
--rw-r--r--   0        0        0    12351 1970-01-01 00:00:00.000000 ancv-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 19:53:30.294429 ancv-1.3.0/LICENSE
+-rw-r--r--   0        0        0    10301 2023-04-21 19:53:30.294429 ancv-1.3.0/README.md
+-rw-r--r--   0        0        0      308 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/__init__.py
+-rw-r--r--   0        0        0     8719 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/models/__init__.py
+-rw-r--r--   0        0        0     3102 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/models/github.py
+-rw-r--r--   0        0        0    13506 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/models/resume.py
+-rw-r--r--   0        0        0     7803 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/showcase.resume.json
+-rw-r--r--   0        0        0      932 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/validation.py
+-rw-r--r--   0        0        0      250 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/py.typed
+-rw-r--r--   0        0        0     3115 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/reflection.py
+-rw-r--r--   0        0        0     1639 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/timing.py
+-rw-r--r--   0        0        0      172 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/visualization/__init__.py
+-rw-r--r--   0        0        0    30290 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/visualization/templates.py
+-rw-r--r--   0        0        0     4199 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/visualization/themes.py
+-rw-r--r--   0        0        0     2778 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/visualization/translations.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/web/__init__.py
+-rw-r--r--   0        0        0     4004 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/web/client.py
+-rw-r--r--   0        0        0     8835 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/web/server.py
+-rw-r--r--   0        0        0     2732 2023-04-21 19:53:30.306429 ancv-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12351 1970-01-01 00:00:00.000000 ancv-1.3.0/PKG-INFO
```

### Comparing `ancv-1.2.3/LICENSE` & `ancv-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/README.md` & `ancv-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/__main__.py` & `ancv-1.3.0/ancv/__main__.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/data/models/github.py` & `ancv-1.3.0/ancv/data/models/github.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/data/models/resume.py` & `ancv-1.3.0/ancv/data/models/resume.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/data/showcase.resume.json` & `ancv-1.3.0/ancv/data/showcase.resume.json`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/data/validation.py` & `ancv-1.3.0/ancv/data/validation.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/reflection.py` & `ancv-1.3.0/ancv/reflection.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/timing.py` & `ancv-1.3.0/ancv/timing.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/visualization/templates.py` & `ancv-1.3.0/ancv/visualization/templates.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/visualization/themes.py` & `ancv-1.3.0/ancv/visualization/themes.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/visualization/translations.py` & `ancv-1.3.0/ancv/visualization/translations.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/web/client.py` & `ancv-1.3.0/ancv/web/client.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/ancv/web/server.py` & `ancv-1.3.0/ancv/web/server.py`

 * *Files identical despite different names*

### Comparing `ancv-1.2.3/pyproject.toml` & `ancv-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ancv"
-version = "1.2.3"
+version = "1.3.0"
 description = "Renders your (JSON) resume/CV for online & pretty terminal display"
 authors = ["Alex Povel <python@alexpovel.de>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://ancv.io"
 repository = "https://github.com/alexpovel/ancv/"
 classifiers = [
@@ -57,15 +57,15 @@
 types-cachetools = "^5.0.1"
 pydeps = "^1.10.18"
 pytest-cov = "^4.0.0"
 pytest-aiohttp = "^1.0.4"
 pytest-rerunfailures = "^10.2"
 requests = "^2.28.1"
 types-babel = "^2.10.0"
-ruff = "^0.0.224"
+ruff = ">=0.0.224,<0.0.261"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ancv = "ancv.__main__:app"
```

### Comparing `ancv-1.2.3/setup.py` & `ancv-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,259 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ancv
+Version: 1.3.0
+Summary: Renders your (JSON) resume/CV for online & pretty terminal display
+Home-page: https://ancv.io
+License: MIT
+Author: Alex Povel
+Author-email: python@alexpovel.de
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Framework :: AnyIO
+Classifier: Framework :: AsyncIO
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Natural Language :: German
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Office/Business
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Terminals
+Classifier: Topic :: Terminals :: Terminal Emulators/X Terminals
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Markup
+Classifier: Typing :: Typed
+Requires-Dist: Babel (>=2.10.3,<3.0.0)
+Requires-Dist: aiohttp[speedups] (>=3.8.1,<4.0.0)
+Requires-Dist: cachetools (>=5.2.0,<6.0.0)
+Requires-Dist: gidgethub (>=5.1.0,<6.0.0)
+Requires-Dist: humanize (>=4.1.0,<5.0.0)
+Requires-Dist: pydantic[email] (>=1.9.1,<2.0.0)
+Requires-Dist: rich (>=12.4.4,<14.0.0)
+Requires-Dist: structlog (>=21.5,<23.0)
+Requires-Dist: typer (>=0.6.1,<0.8.0)
+Project-URL: Bug Tracker, https://github.com/alexpovel/ancv/issues/
+Project-URL: Changelog, https://github.com/alexpovel/ancv/blob/main/CHANGELOG.md
+Project-URL: Pull Requests, https://github.com/alexpovel/ancv/pulls
+Project-URL: Repository, https://github.com/alexpovel/ancv/
+Description-Content-Type: text/markdown
 
-packages = \
-['ancv', 'ancv.data', 'ancv.data.models', 'ancv.visualization', 'ancv.web']
+# [ancv](https://github.com/alexpovel/ancv)
 
-package_data = \
-{'': ['*']}
+Getting your resume aka [an CV](https://youtu.be/mJUtMEJdvqM?t=16) (*[ANSI](https://en.wikipedia.org/wiki/ANSI_escape_code)-v* 🤡) straight to your and anyone else's terminals:
 
-install_requires = \
-['Babel>=2.10.3,<3.0.0',
- 'aiohttp[speedups]>=3.8.1,<4.0.0',
- 'cachetools>=5.2.0,<6.0.0',
- 'gidgethub>=5.1.0,<6.0.0',
- 'humanize>=4.1.0,<5.0.0',
- 'pydantic[email]>=1.9.1,<2.0.0',
- 'rich>=12.4.4,<14.0.0',
- 'structlog>=21.5,<23.0',
- 'typer>=0.6.1,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['ancv = ancv.__main__:app']}
-
-setup_kwargs = {
-    'name': 'ancv',
-    'version': '1.2.3',
-    'description': 'Renders your (JSON) resume/CV for online & pretty terminal display',
-    'long_description': '# [ancv](https://github.com/alexpovel/ancv)\n\nGetting your resume aka [an CV](https://youtu.be/mJUtMEJdvqM?t=16) (*[ANSI](https://en.wikipedia.org/wiki/ANSI_escape_code)-v* 🤡) straight to your and anyone else\'s terminals:\n\n![showcase cv terminal output](docs/images/showcase.svg)\n\n---\n\nBe warned though, for this is kinda useless and just for fun:\n\n<p align="center">\n   <img src="docs/images/users-venn.svg" alt="users venn diagram">\n</p>\n\n## Getting started\n\n1. Create your resume according to the [JSON Resume Schema](https://jsonresume.org/schema/) (see also the [schema specification](https://github.com/jsonresume/resume-schema/blob/master/schema.json)) either:\n\n   - manually (see [the `heyho` sample](./ancv/data/showcase.resume.json) for a possible starting point),\n   - exporting from [LinkedIn](https://www.linkedin.com/) using [Joshua Tzucker\'s LinkedIn exporter](https://joshuatz.com/projects/web-stuff/linkedin-profile-to-json-resume-exporter/) ([repo](https://github.com/joshuatz/linkedin-to-jsonresume))[^1], or\n   - exporting from one of the platforms advertised as offering [JSON resume integration](https://jsonresume.org/schema/).\n2. [Create a **public** gist](https://gist.github.com/) named `resume.json` with your resume contents.\n3. You\'re now the proud owner of an ancv.\n   Time to try it out.\n\n   The following examples work out-of-the-box.\n   **Replace `heyho` with your GitHub username** once you\'re all set up.\n\n   - curl:\n\n      ```bash\n      curl -L ancv.io/heyho\n      ```\n\n      with `-L` being shorthand for [`--location`](https://curl.se/docs/manpage.html), allowing you to follow the redirect from `http://ancv.io` through to `https://ancv.io`.\n      It\'s shorter than its also perfectly viable alternative:\n\n      ```bash\n      curl https://ancv.io/heyho\n      ```\n\n      Lastly, you might want to page the output for easiest reading, top-to-bottom:\n\n      ```bash\n      curl -sL ancv.io/heyho | less\n      ```\n\n      If that garbles the rendered output, try `less -r` aka [`--raw-control-chars`](https://man7.org/linux/man-pages/man1/less.1.html).\n\n   - wget:\n\n     ```bash\n     wget -O - --quiet ancv.io/heyho\n     ```\n\n     where `-O` is short for [`--output-document`](https://linux.die.net/man/1/wget), used here to redirect to stdout.\n\n   - PowerShell 7:\n\n     ```powershell\n     (iwr ancv.io/heyho).Content\n     ```\n\n     where `iwr` is an alias for [`Invoke-Webrequest`](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-7.2), returning an object whose `Content` we access.\n   - PowerShell 5:\n\n     ```powershell\n     (iwr -UseBasicParsing ancv.io/heyho).Content\n     ```\n\n     where `-UseBasicParsing` is *only* required if you haven\'t set up Internet Explorer yet ([yes, really](https://stackoverflow.com/q/38005341/11477374)).\n     If you have, then it works as PowerShell 7 (where that flag is deprecated and the default anyway).\n\n## Configuration\n\n*All configuration is optional.*\n\nThe CV is constructed as follows:\n\n![conceptual flow chart](docs/images/concept-flow-chart.svg)\n\nIn summary:\n\n- you control:\n  - the **template**.\n\n    Essentially the order of items, indentations, text alignment, position of dates and more.\n    Templates are like layouts/skeletons.\n  - the **theme**.\n\n    This controls colors, italics, boldface, underlining, blinking (yes, really) and more.\n    A couple themes exist but you can easily add your own one.\n  - the **language** to use.\n\n    Pre-set strings like section titles (*Education*, ...), names of months etc. are governed by *translations*, of which there are a couple available already.\n    All other text is free-form.\n  - text content like emojis and newlines to control paragraph breaks.\n\n    Emojis are user-controlled: if you want them, use them in your `resume.json`; in the future, there might be *templates* with emojis baked in, but you\'d have to actively opt into using one.\n  - date formatting, in a limited fashion through a special `dec31_as_year` toggle.\n    If that toggle is `true`, dates in the format `YYYY-12-31` will be displayed as `YYYY` only.\n  - lastly, there\'s a toggle for ASCII-only output.\n\n    It only concerns the *template* and controls the drawing of boxes and such (e.g., [`-`](https://unicode-table.com/en/002D/) versus [`─`](https://unicode-table.com/en/2500/) : only the latter will produce gapless rules).\n    If you yourself use non-ASCII characters in your texts, use a *language* containing non-ASCII characters (Spanish, French, ...) or a *theme* with non-ASCII characters (e.g., a theme might use the `•` character to print bullet points), non-ASCII Unicode will still occur.\n    As such, this toggle currently isn\'t very powerful, but with some care it *does* ultimately allow you to be ASCII-only.\n\n  If you come up with new templates, themes or translations, a PR would be highly appreciated.\n- you *do not* control:\n  - anything about a viewer\'s terminal!\n\n    Any recent terminal will support a baseline of features (e.g., colors), but large parts of the functionalities depend on the *font* used: proper Unicode support is needed for pretty output (see `ascii_only`), and ideally emojis if you\'re into that (although it\'s easy to pick an emoji-free template).\n    Many themes leverage Unicode characters as well.\n  - access to your CV: like the gist itself, it will be publicly available on GitHub.\n\n### How to configure\n\nConfiguring `ancv` requires going beyond the vanilla JSON Resume schema.\nYou will need to add an (entirely optional) `$.meta.ancv` field to your `resume.json`.\nThe [provided schema](schema.json) will be of help here:\nan editor capable of providing auto-completion based on it, like [Visual Studio Code](https://code.visualstudio.com/docs/languages/json#_json-schemas-and-settings), will make filling out the additional configuration a breeze.\n\nThe schema will further inform you of the default values (used for unspecified fields).\nSince everything is optional, a [valid JSON resume](https://github.com/jsonresume/resume-schema/blob/master/schema.json) (without an `ancv` section) is valid for `ancv` use as well.\n\n## Installation\n\n### As a library\n\nInstall the package as usual:\n\n```bash\npip install ancv\n```\n\nThis also allows you to import whatever you could want or need from the package, if anything.\nNote that it\'s pretty heavy on the dependencies.\n\n### As a container\n\nSee also the available [packages aka images](https://github.com/alexpovel/ancv/pkgs/container/ancv):\n\n```bash\ndocker pull ghcr.io/alexpovel/ancv\n```\n\nVersioned tags (so you can pin a major) are available.\n\n### Local usage\n\nOnce installed, you could for example check whether your `resume.json` is valid at all (`validate`) or get a glimpse at the final product (`render`):\n\n```bash\n# pip route:\n$ ancv render resume.json\n# container route:\n$ docker run -v $(pwd)/resume.json:/app/resume.json ghcr.io/alexpovel/ancv render\n```\n\n## Self-hosting\n\nSelf-hosting is a first-class citizen here.\n\n### Context: Cloud Hosting\n\nThe <https://ancv.io> site is hosted on [Google Cloud Run](https://cloud.google.com/run) (serverless) and deployed there [automatically](https://github.com/alexpovel/ancv/runs/8172131447), such that the latest release you see here is also the code executing in that cloud environment.\nThat\'s convenient to get started: simply create a `resume.json` gist and you\'re good to go within minutes.\nIt can also be used for debugging and playing around; it\'s a playground of sorts.\n\nYou\'re invited to use this service for as much and as long as you\'d like.\nHowever, obviously, as an individual I cannot guarantee its availability in perpetuity.\nYou might also feel uncomfortable uploading your CV onto GitHub, since it *has* to be public for this whole exercise to work.\nLastly, you might also be suspicious of me inserting funny business into your CV before serving it out.\nIf this is you, self-hosting is for you.\n\n### Setup\n\nFor simplicity, using Docker Compose (with Docker\'s recent [Compose CLI plugin](https://docs.docker.com/compose/install/compose-plugin/)):\n\n1. Clone this repository onto your server (or fork it, make your edits and clone that)\n2. `cd self-hosting`\n3. Edit [Caddy\'s config file](./self-hosting/Caddyfile) ([more info](https://caddyserver.com/docs/caddyfile)) to contain your own domain name\n4. Place your `resume.json` into the directory\n5. Run `docker compose up`\n\nCaddy (chosen here for simplicity) will handle HTTPS automatically for you, but will of course require domain names to be set up correctly to answer ACME challenges.\nHandling DNS is up to you; for dynamic DNS, I can recommend [`qmcgaw/ddns-updater`](https://github.com/qdm12/ddns-updater).\n\nIf you self-host in the cloud, the server infrastructure might be taken care of for you by your provider already (as is the case for Google Cloud Run).\nIn these cases, a dedicated proxy is unnecessary and a single [Dockerfile](./Dockerfile) might suffice (adjusted to your needs).\nTrue [serverless](https://www.serverless.com/) is also a possibility and an excellent fit here.\nFor example, one could use [Digital Ocean\'s *Functions*](https://docs.digitalocean.com/products/functions/).\nIf you go that route and succeed, please let me know! (I had given up with how depressingly hard dependency management was, as opposed to tried-and-tested container images.)\n\n---\n\n<p align="center">\n   <a href="https://github.com/alexpovel/ancv">\n     <img src="https://github.githubassets.com/images/modules/site/icons/footer/github-mark.svg" alt="github logo">\n   </a>\n</p>\n\n[^1]: The exporter has a couple caveats.\n  You will probably not be able to paste its result into a gist and have it work out of the box.\n  It is recommended to paste the export into an editor capable of helping you find errors against the contained `$schema`, like VS Code.\n  Alternatively, a local `ancv render your-file.json` will print `pydantic` validation errors, which might be helpful in debugging.\n  For example, the exporter might leave `$.basics.url` an empty string, which isn\'t a valid URI and therefore fails the schema and, by extension, `ancv`.\n  Similarly, `endDate` keys might get empty string values.\n  **Remove these entries** entirely to stay conformant to the JSON Resume Schema (to which `ancv` stays conformant).\n',
-    'author': 'Alex Povel',
-    'author_email': 'python@alexpovel.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://ancv.io',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+![showcase cv terminal output](docs/images/showcase.svg)
 
+---
+
+Be warned though, for this is kinda useless and just for fun:
+
+<p align="center">
+   <img src="docs/images/users-venn.svg" alt="users venn diagram">
+</p>
+
+## Getting started
+
+1. Create your resume according to the [JSON Resume Schema](https://jsonresume.org/schema/) (see also the [schema specification](https://github.com/jsonresume/resume-schema/blob/master/schema.json)) either:
+
+   - manually (see [the `heyho` sample](./ancv/data/showcase.resume.json) for a possible starting point),
+   - exporting from [LinkedIn](https://www.linkedin.com/) using [Joshua Tzucker's LinkedIn exporter](https://joshuatz.com/projects/web-stuff/linkedin-profile-to-json-resume-exporter/) ([repo](https://github.com/joshuatz/linkedin-to-jsonresume))[^1], or
+   - exporting from one of the platforms advertised as offering [JSON resume integration](https://jsonresume.org/schema/).
+2. [Create a **public** gist](https://gist.github.com/) named `resume.json` with your resume contents.
+3. You're now the proud owner of an ancv.
+   Time to try it out.
+
+   The following examples work out-of-the-box.
+   **Replace `heyho` with your GitHub username** once you're all set up.
+
+   - curl:
+
+      ```bash
+      curl -L ancv.io/heyho
+      ```
+
+      with `-L` being shorthand for [`--location`](https://curl.se/docs/manpage.html), allowing you to follow the redirect from `http://ancv.io` through to `https://ancv.io`.
+      It's shorter than its also perfectly viable alternative:
+
+      ```bash
+      curl https://ancv.io/heyho
+      ```
+
+      Lastly, you might want to page the output for easiest reading, top-to-bottom:
+
+      ```bash
+      curl -sL ancv.io/heyho | less
+      ```
+
+      If that garbles the rendered output, try `less -r` aka [`--raw-control-chars`](https://man7.org/linux/man-pages/man1/less.1.html).
+
+   - wget:
+
+     ```bash
+     wget -O - --quiet ancv.io/heyho
+     ```
+
+     where `-O` is short for [`--output-document`](https://linux.die.net/man/1/wget), used here to redirect to stdout.
+
+   - PowerShell 7:
+
+     ```powershell
+     (iwr ancv.io/heyho).Content
+     ```
+
+     where `iwr` is an alias for [`Invoke-Webrequest`](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-7.2), returning an object whose `Content` we access.
+   - PowerShell 5:
+
+     ```powershell
+     (iwr -UseBasicParsing ancv.io/heyho).Content
+     ```
+
+     where `-UseBasicParsing` is *only* required if you haven't set up Internet Explorer yet ([yes, really](https://stackoverflow.com/q/38005341/11477374)).
+     If you have, then it works as PowerShell 7 (where that flag is deprecated and the default anyway).
+
+## Configuration
+
+*All configuration is optional.*
+
+The CV is constructed as follows:
+
+![conceptual flow chart](docs/images/concept-flow-chart.svg)
+
+In summary:
+
+- you control:
+  - the **template**.
+
+    Essentially the order of items, indentations, text alignment, position of dates and more.
+    Templates are like layouts/skeletons.
+  - the **theme**.
+
+    This controls colors, italics, boldface, underlining, blinking (yes, really) and more.
+    A couple themes exist but you can easily add your own one.
+  - the **language** to use.
+
+    Pre-set strings like section titles (*Education*, ...), names of months etc. are governed by *translations*, of which there are a couple available already.
+    All other text is free-form.
+  - text content like emojis and newlines to control paragraph breaks.
+
+    Emojis are user-controlled: if you want them, use them in your `resume.json`; in the future, there might be *templates* with emojis baked in, but you'd have to actively opt into using one.
+  - date formatting, in a limited fashion through a special `dec31_as_year` toggle.
+    If that toggle is `true`, dates in the format `YYYY-12-31` will be displayed as `YYYY` only.
+  - lastly, there's a toggle for ASCII-only output.
+
+    It only concerns the *template* and controls the drawing of boxes and such (e.g., [`-`](https://unicode-table.com/en/002D/) versus [`─`](https://unicode-table.com/en/2500/) : only the latter will produce gapless rules).
+    If you yourself use non-ASCII characters in your texts, use a *language* containing non-ASCII characters (Spanish, French, ...) or a *theme* with non-ASCII characters (e.g., a theme might use the `•` character to print bullet points), non-ASCII Unicode will still occur.
+    As such, this toggle currently isn't very powerful, but with some care it *does* ultimately allow you to be ASCII-only.
+
+  If you come up with new templates, themes or translations, a PR would be highly appreciated.
+- you *do not* control:
+  - anything about a viewer's terminal!
+
+    Any recent terminal will support a baseline of features (e.g., colors), but large parts of the functionalities depend on the *font* used: proper Unicode support is needed for pretty output (see `ascii_only`), and ideally emojis if you're into that (although it's easy to pick an emoji-free template).
+    Many themes leverage Unicode characters as well.
+  - access to your CV: like the gist itself, it will be publicly available on GitHub.
+
+### How to configure
+
+Configuring `ancv` requires going beyond the vanilla JSON Resume schema.
+You will need to add an (entirely optional) `$.meta.ancv` field to your `resume.json`.
+The [provided schema](schema.json) will be of help here:
+an editor capable of providing auto-completion based on it, like [Visual Studio Code](https://code.visualstudio.com/docs/languages/json#_json-schemas-and-settings), will make filling out the additional configuration a breeze.
+
+The schema will further inform you of the default values (used for unspecified fields).
+Since everything is optional, a [valid JSON resume](https://github.com/jsonresume/resume-schema/blob/master/schema.json) (without an `ancv` section) is valid for `ancv` use as well.
+
+## Installation
+
+### As a library
+
+Install the package as usual:
+
+```bash
+pip install ancv
+```
+
+This also allows you to import whatever you could want or need from the package, if anything.
+Note that it's pretty heavy on the dependencies.
+
+### As a container
+
+See also the available [packages aka images](https://github.com/alexpovel/ancv/pkgs/container/ancv):
+
+```bash
+docker pull ghcr.io/alexpovel/ancv
+```
+
+Versioned tags (so you can pin a major) are available.
+
+### Local usage
+
+Once installed, you could for example check whether your `resume.json` is valid at all (`validate`) or get a glimpse at the final product (`render`):
+
+```bash
+# pip route:
+$ ancv render resume.json
+# container route:
+$ docker run -v $(pwd)/resume.json:/app/resume.json ghcr.io/alexpovel/ancv render
+```
+
+## Self-hosting
+
+Self-hosting is a first-class citizen here.
+
+### Context: Cloud Hosting
+
+The <https://ancv.io> site is hosted on [Google Cloud Run](https://cloud.google.com/run) (serverless) and deployed there [automatically](https://github.com/alexpovel/ancv/runs/8172131447), such that the latest release you see here is also the code executing in that cloud environment.
+That's convenient to get started: simply create a `resume.json` gist and you're good to go within minutes.
+It can also be used for debugging and playing around; it's a playground of sorts.
+
+You're invited to use this service for as much and as long as you'd like.
+However, obviously, as an individual I cannot guarantee its availability in perpetuity.
+You might also feel uncomfortable uploading your CV onto GitHub, since it *has* to be public for this whole exercise to work.
+Lastly, you might also be suspicious of me inserting funny business into your CV before serving it out.
+If this is you, self-hosting is for you.
+
+### Setup
+
+For simplicity, using Docker Compose (with Docker's recent [Compose CLI plugin](https://docs.docker.com/compose/install/compose-plugin/)):
+
+1. Clone this repository onto your server (or fork it, make your edits and clone that)
+2. `cd self-hosting`
+3. Edit [Caddy's config file](./self-hosting/Caddyfile) ([more info](https://caddyserver.com/docs/caddyfile)) to contain your own domain name
+4. Place your `resume.json` into the directory
+5. Run `docker compose up`
+
+Caddy (chosen here for simplicity) will handle HTTPS automatically for you, but will of course require domain names to be set up correctly to answer ACME challenges.
+Handling DNS is up to you; for dynamic DNS, I can recommend [`qmcgaw/ddns-updater`](https://github.com/qdm12/ddns-updater).
+
+If you self-host in the cloud, the server infrastructure might be taken care of for you by your provider already (as is the case for Google Cloud Run).
+In these cases, a dedicated proxy is unnecessary and a single [Dockerfile](./Dockerfile) might suffice (adjusted to your needs).
+True [serverless](https://www.serverless.com/) is also a possibility and an excellent fit here.
+For example, one could use [Digital Ocean's *Functions*](https://docs.digitalocean.com/products/functions/).
+If you go that route and succeed, please let me know! (I had given up with how depressingly hard dependency management was, as opposed to tried-and-tested container images.)
+
+---
+
+<p align="center">
+   <a href="https://github.com/alexpovel/ancv">
+     <img src="https://github.githubassets.com/images/modules/site/icons/footer/github-mark.svg" alt="github logo">
+   </a>
+</p>
+
+[^1]: The exporter has a couple caveats.
+  You will probably not be able to paste its result into a gist and have it work out of the box.
+  It is recommended to paste the export into an editor capable of helping you find errors against the contained `$schema`, like VS Code.
+  Alternatively, a local `ancv render your-file.json` will print `pydantic` validation errors, which might be helpful in debugging.
+  For example, the exporter might leave `$.basics.url` an empty string, which isn't a valid URI and therefore fails the schema and, by extension, `ancv`.
+  Similarly, `endDate` keys might get empty string values.
+  **Remove these entries** entirely to stay conformant to the JSON Resume Schema (to which `ancv` stays conformant).
 
-setup(**setup_kwargs)
```

