# Comparing `tmp/grimoirelab-0.8.0.tar.gz` & `tmp/grimoirelab-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoirelab-0.8.0.tar", max compression
+gzip compressed data, was "grimoirelab-0.9.0rc1.tar", max compression
```

## Comparing `grimoirelab-0.8.0.tar` & `grimoirelab-0.9.0rc1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    35141 2023-02-03 10:31:11.957242 grimoirelab-0.8.0/LICENSE
--rw-r--r--   0        0        0     8685 2023-02-03 10:31:11.961242 grimoirelab-0.8.0/README.md
--rw-r--r--   0        0        0       34 2023-02-03 10:31:12.041242 grimoirelab-0.8.0/grimoirelab/__init__.py
--rw-r--r--   0        0        0       86 2023-02-03 10:31:12.041242 grimoirelab-0.8.0/grimoirelab/_version.py
--rwxr-xr-x   0        0        0     1844 2023-02-03 10:31:12.041242 grimoirelab-0.8.0/grimoirelab/grimoirelab.py
--rw-r--r--   0        0        0     1841 2023-02-03 10:31:12.045242 grimoirelab-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9972 1970-01-01 00:00:00.000000 grimoirelab-0.8.0/setup.py
--rw-r--r--   0        0        0    10204 1970-01-01 00:00:00.000000 grimoirelab-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-04-21 11:08:17.133081 grimoirelab-0.9.0rc1/LICENSE
+-rw-r--r--   0        0        0     8685 2023-04-21 11:08:17.133081 grimoirelab-0.9.0rc1/README.md
+-rw-r--r--   0        0        0       34 2023-04-21 11:08:17.209082 grimoirelab-0.9.0rc1/grimoirelab/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-21 11:08:17.209082 grimoirelab-0.9.0rc1/grimoirelab/_version.py
+-rwxr-xr-x   0        0        0     1844 2023-04-21 11:08:17.209082 grimoirelab-0.9.0rc1/grimoirelab/grimoirelab.py
+-rw-r--r--   0        0        0     1906 2023-04-21 11:08:17.209082 grimoirelab-0.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 grimoirelab-0.9.0rc1/PKG-INFO
```

### Comparing `grimoirelab-0.8.0/LICENSE` & `grimoirelab-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoirelab-0.8.0/README.md` & `grimoirelab-0.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `grimoirelab-0.8.0/grimoirelab/grimoirelab.py` & `grimoirelab-0.9.0rc1/grimoirelab/grimoirelab.py`

 * *Files identical despite different names*

### Comparing `grimoirelab-0.8.0/pyproject.toml` & `grimoirelab-0.9.0rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoirelab"
-version = "0.8.0"
+version = "0.9.0-rc.1"
 description = "Tool set for software development analytics"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -34,27 +34,27 @@
 
 [tool.poetry.scripts]
 'grimoirelab' = 'grimoirelab.grimoirelab:main'
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 
-grimoirelab-toolkit = {version = ">=0.3.3", allow-prereleases = true}
-perceval-mozilla = {version = ">=0.3.7", allow-prereleases = true}
-perceval-opnfv = {version = ">=0.2.7", allow-prereleases = true}
-perceval-puppet = {version = ">=0.2.7", allow-prereleases = true}
-perceval-weblate = {version = ">=0.2.7", allow-prereleases = true}
-sortinghat = {version = ">=0.8.1", allow-prereleases = true}
-kidash = {version = ">=0.5.3", allow-prereleases = true}
+grimoirelab-toolkit = {version = ">=0.3.4-rc.1", allow-prereleases = true}
+perceval-mozilla = {version = ">=0.3.8-rc.2", allow-prereleases = true}
+perceval-opnfv = {version = ">=0.2.8-rc.2", allow-prereleases = true}
+perceval-puppet = {version = ">=0.2.8-rc.2", allow-prereleases = true}
+perceval-weblate = {version = ">=0.2.8-rc.2", allow-prereleases = true}
+sortinghat = {version = ">=0.9.0-rc.2", allow-prereleases = true}
+kidash = {version = ">=0.5.4-rc.1", allow-prereleases = true}
 grimoirelab-panels = {version = ">=0.2.0", allow-prereleases = true}
-grimoire-elk = {version = ">=0.104.2", allow-prereleases = true}
-sirmordred = {version = ">=0.6.1", allow-prereleases = true}
-cereslib = {version = ">=0.3.6", allow-prereleases = true}
-graal = {version = ">=0.4.4", allow-prereleases = true}
+grimoire-elk = {version = ">=0.104.3-rc.2", allow-prereleases = true}
+sirmordred = {version = ">=0.7.0-rc.1", allow-prereleases = true}
+cereslib = {version = ">=0.4.0-rc.1", allow-prereleases = true}
+graal = {version = ">=0.4.5-rc.2", allow-prereleases = true}
 statsmodels = "^0.13.2"
-perceval = {version = ">=0.21.3", allow-prereleases = true}
+perceval = {version = ">=0.21.4-rc.2", allow-prereleases = true}
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `grimoirelab-0.8.0/setup.py` & `grimoirelab-0.9.0rc1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,201 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: grimoirelab
+Version: 0.9.0rc1
+Summary: Tool set for software development analytics
+Home-page: https://chaoss.github.io/grimoirelab/
+License: GPL-3.0+
+Keywords: development,grimoirelab
+Author: GrimoireLab Developers
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Requires-Dist: cereslib (>=0.4.0-rc.1)
+Requires-Dist: graal (>=0.4.5-rc.2)
+Requires-Dist: grimoire-elk (>=0.104.3-rc.2)
+Requires-Dist: grimoirelab-panels (>=0.2.0)
+Requires-Dist: grimoirelab-toolkit (>=0.3.4-rc.1)
+Requires-Dist: kidash (>=0.5.4-rc.1)
+Requires-Dist: perceval (>=0.21.4-rc.2)
+Requires-Dist: perceval-mozilla (>=0.3.8-rc.2)
+Requires-Dist: perceval-opnfv (>=0.2.8-rc.2)
+Requires-Dist: perceval-puppet (>=0.2.8-rc.2)
+Requires-Dist: perceval-weblate (>=0.2.8-rc.2)
+Requires-Dist: sirmordred (>=0.7.0-rc.1)
+Requires-Dist: sortinghat (>=0.9.0-rc.2)
+Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
+Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab/issues
+Project-URL: Repository, https://github.com/chaoss/grimoirelab
+Description-Content-Type: text/markdown
+
+# GrimoireLab
+
+[![grimoirelab-showcase](https://user-images.githubusercontent.com/25265451/84442403-30dcce80-ac5b-11ea-9f5b-60266d875ebd.png "GrimoireLab | CHAOSS Bitergia Analytics")](https://chaoss.biterg.io/app/kibana#/dashboard/Overview)
+
+GrimoireLab is a [CHAOSS](https://chaoss.community) toolset for software development analytics. It includes a coordinated set of tools
+to retrieve data from systems used to support software development (repositories), store it in databases,
+enrich it by computing relevant metrics, and make it easy to run analytics and visualizations on it.
+
+You can learn more about GrimoireLab in the [GrimoireLab tutorial](https://chaoss.github.io/grimoirelab-tutorial/),
+or visit the [GrimoireLab website](https://chaoss.github.io/grimoirelab).
+
+Metrics available in GrimoireLab are, in part, developed in the CHAOSS project. For more information regarding CHAOSS metrics, see the latest release at: https://chaoss.community/metrics/
+
+# Getting started
+
+To ease the newcomer experience we are providing a [default setup](default-grimoirelab-settings)
+to analyze git activity for this repository. For this set up, there are several options to run GrimoireLab:
+
+## Using `docker-compose`
+
+Requirements:
+* **Software**: [git](https://git-scm.com/), [docker client](https://docs.docker.com/get-docker/) and [docker compose](https://docs.docker.com/compose/install/). An example of working configuration:
+```console
+root@test-68b8628f:~# git --version
+git version 2.17.1
+root@test-68b8628f:~# docker --version
+Docker version 19.03.1, build 74b1e89
+root@test-68b8628f:~# docker-compose --version
+docker-compose version 1.22.0, build f46880fe
+```
+* **Hardware**: 2 CPU cores, 8GB memory RAM and [enough virtual memory for Elasticsearch](https://www.elastic.co/guide/en/elasticsearch/reference/current/vm-max-map-count.html) 
+
+Steps:
+1. Clone this project:
+```console
+foo@bar:~$ git clone https://github.com/chaoss/grimoirelab
+```
+2. Go to `docker-compose` folder and run the following command:
+```console
+foo@bar:~$ cd grimoirelab/docker-compose
+foo@bar:~/grimoirelab/docker-compose$ docker-compose up -d
+```
+
+Your dashboard will be ready after a while at `http://localhost:8000`. The waiting time depends on the amount of data to fetch from a repo, for small repositories you can expect your data to be visible in the dashboard after 10-15 minutes.
+
+More details in the [docker-compose folder](./docker-compose/README.md).
+
+## Using `docker run`
+
+Requirements: 
+* **Software**: [git](https://git-scm.com/) and [docker client](https://docs.docker.com/get-docker/). An example of working configuration:
+```console
+root@test-68b8628f:~# git --version
+git version 2.17.1
+root@test-68b8628f:~# docker --version
+Docker version 19.03.1, build 74b1e89
+```
+* **Hardware**: 2 CPU cores, 8GB memory RAM and set
+* ElasticSearch and Kibana up and running.
+* SortingHat up and running
+
+Steps:
+1. Clone this project:
+```console
+$ git clone https://github.com/chaoss/grimoirelab
+```
+2. Go to the project folder and run the following command:
+```console
+foo@bar:~$ cd grimoirelab
+foo@bar:~/grimoirelab $ docker run --net=host \ 
+    -v $(pwd)/default-grimoirelab-settings/projects.json:/home/grimoire/conf/projects.json \
+    -v $(pwd)/default-grimoirelab-settings/setup-docker.cfg:/home/grimoire/conf/setup.cfg \
+    -t grimoirelab/grimoirelab
+```
+
+Your dashboard will be ready after a while at `http://localhost:8000`. The waiting time depends on the amount of data to fetch from a repo, for small repositories you can expect your data to be visible in the dashboard after 10-15 minutes.
+
+More details in the [docker folder](./docker/README.md).
+
+# GrimoireLab components
+
+Currently, GrimoireLab toolkit is organized in the following repositories:
+
+* Data retrieval related components:
+  * [Perceval](https://github.com/chaoss/grimoirelab-perceval): retrieval of data from data sources
+    * [Perceval (bundle for OPNFV)](https://github.com/chaoss/grimoirelab-perceval-opnfv)
+    * [Perceval (bundle for Mozilla)](https://github.com/chaoss/grimoirelab-perceval-mozilla)
+    * [Perceval (bundle for Puppet)](https://github.com/chaoss/grimoirelab-perceval-puppet)
+    * [Perceval (bundle for Weblate)](https://github.com/chaoss/grimoirelab-perceval-weblate)
+  * [Graal](https://github.com/chaoss/grimoirelab-graal): source data analysis with external tools
+  * [KingArthur](https://github.com/chaoss/grimoirelab-kingarthur): batch processing for massive retrieval
+* Data enrichment related components:
+  * [GrimoireElk](https://github.com/chaoss/grimoirelab-elk): storage and enrichment of data
+  * [Cereslib](https://github.com/chaoss/grimoirelab-cereslib): generic data processor
+  * [SortingHat](https://github.com/chaoss/grimoirelab-sortinghat): identity management
+* Data consumption related components:
+  * [Kibiter](https://github.com/chaoss/grimoirelab-kibiter): dashboard, downstream version of Kibana
+  * [Sigils](https://github.com/chaoss/grimoirelab-sigils): visualizations and dashboards
+  * [Kidash](https://github.com/chaoss/grimoirelab-kidash): visualizations and dashboards manager
+  * [Manuscripts](https://github.com/chaoss/grimoirelab-manuscripts): reporting
+* Platform management, orchestration, and common utils:
+  * [Mordred](https://github.com/chaoss/grimoirelab-mordred): orchestration
+  * [GrimoireLab Toolkit](https://github.com/chaoss/grimoirelab-toolkit): common utilities
+  * [Bestiary](https://github.com/chaoss/grimoirelab-bestiary): web-based user interface to manage repositories and projects for Mordred
+
+There are also some [components built by the GrimoreLab community](community_components.md),
+which can be useful for you. Other related repositories are:
+* [GrimoireLab Tutorial](https://github.com/chaoss/grimoirelab-tutorial)
+* [GrimoireLab as a whole](https://github.com/chaoss/grimoirelab) (this repository)
+
+## Contents of this repository
+
+This repository is for content relevant to GrimoireLab as a whole. For example:
+
+* Issues for new features or bug reports that affect more than one GrimoireLab module. In this case, let's open an issue here, and when implementing the fix or the feature, let´s comment about the specific tickets in the specific modules that are used. For example, when supporting a new datasource, we will need patches (at least) in `Perceval`, `GrimoireELK` and panels. In this case, we would open a feature request (or the user story) for the whole case, an issue (and later a pull request) in `Perceval` for the data retriever, same for `GrimoireELK` for the enriching code, and same for `panels` for the Kibiter panels.
+
+* Release notes for most GrimoireLab components (directory [releases](releases)).
+
+* Docker container for showcasing GrimoireLab (directory [docker](docker)).
+Includes a Dockerfile and configuration files for the GrimoireLab containers
+that can be used to demo the technology, and can be the basis for real
+deployments. See more information in the [docker README.md file](docker/README.md).
+
+* If you feel more comfortable with `docker-compose`, the [docker-compose](docker-compose)
+folder includes instructions and configuration files to deploy GrimoireLab using
+`docker-compose` command.
+
+* Source code of the GrimoireLab components is available in `src`. Each directory is a
+Git submodule, so its contents will not be available after cloning the repository. To
+fetch all the data, and get the latest version, you can run the following command:
+```console
+$ git submodule update --init --remote
+```
+
+* How releases of GrimoireLab are built and tested: [Building](BUILDING.md)
+
+## Citation
+
+If you use GrimoireLab in your research papers, please refer to [GrimoireLab: A toolset for software development analytics](https://doi.org/10.7717/peerj-cs.601):
+
+APA style:
+
+```
+Dueñas S, Cosentino V, Gonzalez-Barahona JM, del Castillo San Felix A, Izquierdo-Cortazar D, Cañas-Díaz L, Pérez García-Plaza A. 2021. GrimoireLab: A toolset for software development analytics. PeerJ Computer Science 7:e601 https://doi.org/10.7717/peerj-cs.601
+```
+
+BibTeX / BibLaTeX:
+
+```
+@Article{duenas2021:grimoirelab,
+  author = 	 {Dueñas, Santiago and Cosentino, Valerio and Gonzalez-Barahona, Jesus M. and del Castillo San Felix, Alvaro and Izquierdo-Cortazar,  Daniel and Cañas-Díaz, Luis and Pérez García-Plaza, Alberto},
+  title = 	 {GrimoireLab: A toolset for software development analytics},
+  journaltitle = {PeerJ Computer Science},
+  date = 	 {2021-07-09},
+  volume = 	 7,
+  number = 	 {e601},
+  doi = 	 {10.7717/peerj-cs.601},
+  url = 	 {https://doi.org/10.7717/peerj-cs.601}}
+```
 
-packages = \
-['grimoirelab']
+# Contributing
 
-package_data = \
-{'': ['*']}
+Contributions are welcome, please check the [Contributing Guidelines](CONTRIBUTING.md).
 
-install_requires = \
-['cereslib>=0.3.6',
- 'graal>=0.4.4',
- 'grimoire-elk>=0.104.2',
- 'grimoirelab-panels>=0.2.0',
- 'grimoirelab-toolkit>=0.3.3',
- 'kidash>=0.5.3',
- 'perceval-mozilla>=0.3.7',
- 'perceval-opnfv>=0.2.7',
- 'perceval-puppet>=0.2.7',
- 'perceval-weblate>=0.2.7',
- 'perceval>=0.21.3',
- 'sirmordred>=0.6.1',
- 'sortinghat>=0.8.1',
- 'statsmodels>=0.13.2,<0.14.0']
-
-entry_points = \
-{'console_scripts': ['grimoirelab = grimoirelab.grimoirelab:main']}
-
-setup_kwargs = {
-    'name': 'grimoirelab',
-    'version': '0.8.0',
-    'description': 'Tool set for software development analytics',
-    'long_description': '# GrimoireLab\n\n[![grimoirelab-showcase](https://user-images.githubusercontent.com/25265451/84442403-30dcce80-ac5b-11ea-9f5b-60266d875ebd.png "GrimoireLab | CHAOSS Bitergia Analytics")](https://chaoss.biterg.io/app/kibana#/dashboard/Overview)\n\nGrimoireLab is a [CHAOSS](https://chaoss.community) toolset for software development analytics. It includes a coordinated set of tools\nto retrieve data from systems used to support software development (repositories), store it in databases,\nenrich it by computing relevant metrics, and make it easy to run analytics and visualizations on it.\n\nYou can learn more about GrimoireLab in the [GrimoireLab tutorial](https://chaoss.github.io/grimoirelab-tutorial/),\nor visit the [GrimoireLab website](https://chaoss.github.io/grimoirelab).\n\nMetrics available in GrimoireLab are, in part, developed in the CHAOSS project. For more information regarding CHAOSS metrics, see the latest release at: https://chaoss.community/metrics/\n\n# Getting started\n\nTo ease the newcomer experience we are providing a [default setup](default-grimoirelab-settings)\nto analyze git activity for this repository. For this set up, there are several options to run GrimoireLab:\n\n## Using `docker-compose`\n\nRequirements:\n* **Software**: [git](https://git-scm.com/), [docker client](https://docs.docker.com/get-docker/) and [docker compose](https://docs.docker.com/compose/install/). An example of working configuration:\n```console\nroot@test-68b8628f:~# git --version\ngit version 2.17.1\nroot@test-68b8628f:~# docker --version\nDocker version 19.03.1, build 74b1e89\nroot@test-68b8628f:~# docker-compose --version\ndocker-compose version 1.22.0, build f46880fe\n```\n* **Hardware**: 2 CPU cores, 8GB memory RAM and [enough virtual memory for Elasticsearch](https://www.elastic.co/guide/en/elasticsearch/reference/current/vm-max-map-count.html) \n\nSteps:\n1. Clone this project:\n```console\nfoo@bar:~$ git clone https://github.com/chaoss/grimoirelab\n```\n2. Go to `docker-compose` folder and run the following command:\n```console\nfoo@bar:~$ cd grimoirelab/docker-compose\nfoo@bar:~/grimoirelab/docker-compose$ docker-compose up -d\n```\n\nYour dashboard will be ready after a while at `http://localhost:8000`. The waiting time depends on the amount of data to fetch from a repo, for small repositories you can expect your data to be visible in the dashboard after 10-15 minutes.\n\nMore details in the [docker-compose folder](./docker-compose/README.md).\n\n## Using `docker run`\n\nRequirements: \n* **Software**: [git](https://git-scm.com/) and [docker client](https://docs.docker.com/get-docker/). An example of working configuration:\n```console\nroot@test-68b8628f:~# git --version\ngit version 2.17.1\nroot@test-68b8628f:~# docker --version\nDocker version 19.03.1, build 74b1e89\n```\n* **Hardware**: 2 CPU cores, 8GB memory RAM and set\n* ElasticSearch and Kibana up and running.\n* SortingHat up and running\n\nSteps:\n1. Clone this project:\n```console\n$ git clone https://github.com/chaoss/grimoirelab\n```\n2. Go to the project folder and run the following command:\n```console\nfoo@bar:~$ cd grimoirelab\nfoo@bar:~/grimoirelab $ docker run --net=host \\ \n    -v $(pwd)/default-grimoirelab-settings/projects.json:/home/grimoire/conf/projects.json \\\n    -v $(pwd)/default-grimoirelab-settings/setup-docker.cfg:/home/grimoire/conf/setup.cfg \\\n    -t grimoirelab/grimoirelab\n```\n\nYour dashboard will be ready after a while at `http://localhost:8000`. The waiting time depends on the amount of data to fetch from a repo, for small repositories you can expect your data to be visible in the dashboard after 10-15 minutes.\n\nMore details in the [docker folder](./docker/README.md).\n\n# GrimoireLab components\n\nCurrently, GrimoireLab toolkit is organized in the following repositories:\n\n* Data retrieval related components:\n  * [Perceval](https://github.com/chaoss/grimoirelab-perceval): retrieval of data from data sources\n    * [Perceval (bundle for OPNFV)](https://github.com/chaoss/grimoirelab-perceval-opnfv)\n    * [Perceval (bundle for Mozilla)](https://github.com/chaoss/grimoirelab-perceval-mozilla)\n    * [Perceval (bundle for Puppet)](https://github.com/chaoss/grimoirelab-perceval-puppet)\n    * [Perceval (bundle for Weblate)](https://github.com/chaoss/grimoirelab-perceval-weblate)\n  * [Graal](https://github.com/chaoss/grimoirelab-graal): source data analysis with external tools\n  * [KingArthur](https://github.com/chaoss/grimoirelab-kingarthur): batch processing for massive retrieval\n* Data enrichment related components:\n  * [GrimoireElk](https://github.com/chaoss/grimoirelab-elk): storage and enrichment of data\n  * [Cereslib](https://github.com/chaoss/grimoirelab-cereslib): generic data processor\n  * [SortingHat](https://github.com/chaoss/grimoirelab-sortinghat): identity management\n* Data consumption related components:\n  * [Kibiter](https://github.com/chaoss/grimoirelab-kibiter): dashboard, downstream version of Kibana\n  * [Sigils](https://github.com/chaoss/grimoirelab-sigils): visualizations and dashboards\n  * [Kidash](https://github.com/chaoss/grimoirelab-kidash): visualizations and dashboards manager\n  * [Manuscripts](https://github.com/chaoss/grimoirelab-manuscripts): reporting\n* Platform management, orchestration, and common utils:\n  * [Mordred](https://github.com/chaoss/grimoirelab-mordred): orchestration\n  * [GrimoireLab Toolkit](https://github.com/chaoss/grimoirelab-toolkit): common utilities\n  * [Bestiary](https://github.com/chaoss/grimoirelab-bestiary): web-based user interface to manage repositories and projects for Mordred\n\nThere are also some [components built by the GrimoreLab community](community_components.md),\nwhich can be useful for you. Other related repositories are:\n* [GrimoireLab Tutorial](https://github.com/chaoss/grimoirelab-tutorial)\n* [GrimoireLab as a whole](https://github.com/chaoss/grimoirelab) (this repository)\n\n## Contents of this repository\n\nThis repository is for content relevant to GrimoireLab as a whole. For example:\n\n* Issues for new features or bug reports that affect more than one GrimoireLab module. In this case, let\'s open an issue here, and when implementing the fix or the feature, let´s comment about the specific tickets in the specific modules that are used. For example, when supporting a new datasource, we will need patches (at least) in `Perceval`, `GrimoireELK` and panels. In this case, we would open a feature request (or the user story) for the whole case, an issue (and later a pull request) in `Perceval` for the data retriever, same for `GrimoireELK` for the enriching code, and same for `panels` for the Kibiter panels.\n\n* Release notes for most GrimoireLab components (directory [releases](releases)).\n\n* Docker container for showcasing GrimoireLab (directory [docker](docker)).\nIncludes a Dockerfile and configuration files for the GrimoireLab containers\nthat can be used to demo the technology, and can be the basis for real\ndeployments. See more information in the [docker README.md file](docker/README.md).\n\n* If you feel more comfortable with `docker-compose`, the [docker-compose](docker-compose)\nfolder includes instructions and configuration files to deploy GrimoireLab using\n`docker-compose` command.\n\n* Source code of the GrimoireLab components is available in `src`. Each directory is a\nGit submodule, so its contents will not be available after cloning the repository. To\nfetch all the data, and get the latest version, you can run the following command:\n```console\n$ git submodule update --init --remote\n```\n\n* How releases of GrimoireLab are built and tested: [Building](BUILDING.md)\n\n## Citation\n\nIf you use GrimoireLab in your research papers, please refer to [GrimoireLab: A toolset for software development analytics](https://doi.org/10.7717/peerj-cs.601):\n\nAPA style:\n\n```\nDueñas S, Cosentino V, Gonzalez-Barahona JM, del Castillo San Felix A, Izquierdo-Cortazar D, Cañas-Díaz L, Pérez García-Plaza A. 2021. GrimoireLab: A toolset for software development analytics. PeerJ Computer Science 7:e601 https://doi.org/10.7717/peerj-cs.601\n```\n\nBibTeX / BibLaTeX:\n\n```\n@Article{duenas2021:grimoirelab,\n  author = \t {Dueñas, Santiago and Cosentino, Valerio and Gonzalez-Barahona, Jesus M. and del Castillo San Felix, Alvaro and Izquierdo-Cortazar,  Daniel and Cañas-Díaz, Luis and Pérez García-Plaza, Alberto},\n  title = \t {GrimoireLab: A toolset for software development analytics},\n  journaltitle = {PeerJ Computer Science},\n  date = \t {2021-07-09},\n  volume = \t 7,\n  number = \t {e601},\n  doi = \t {10.7717/peerj-cs.601},\n  url = \t {https://doi.org/10.7717/peerj-cs.601}}\n```\n\n# Contributing\n\nContributions are welcome, please check the [Contributing Guidelines](CONTRIBUTING.md).\n',
-    'author': 'GrimoireLab Developers',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://chaoss.github.io/grimoirelab/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

