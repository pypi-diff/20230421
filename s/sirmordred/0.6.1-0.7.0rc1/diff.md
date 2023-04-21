# Comparing `tmp/sirmordred-0.6.1.tar.gz` & `tmp/sirmordred-0.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirmordred-0.6.1.tar", max compression
+gzip compressed data, was "sirmordred-0.7.0rc1.tar", max compression
```

## Comparing `sirmordred-0.6.1.tar` & `sirmordred-0.7.0rc1.tar`

### file list

```diff
@@ -1,97 +1,96 @@
--rw-r--r--   0        0        0    35147 2023-02-03 09:05:05.878105 sirmordred-0.6.1/LICENSE
--rw-r--r--   0        0        0    40852 2023-02-03 09:05:05.878105 sirmordred-0.6.1/README.md
--rw-r--r--   0        0        0     8246 2023-02-03 09:05:05.882106 sirmordred-0.6.1/menu.yaml
--rw-r--r--   0        0        0     2166 2023-02-03 09:05:05.882106 sirmordred-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      835 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/__init__.py
--rw-r--r--   0        0        0       86 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/_version.py
--rwxr-xr-x   0        0        0     4906 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/bin/sirmordred.py
--rw-r--r--   0        0        0    33044 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/config.py
--rw-r--r--   0        0        0     1836 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/error.py
--rw-r--r--   0        0        0     2306 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/github.py
--rwxr-xr-x   0        0        0    12799 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/sirmordred.py
--rw-r--r--   0        0        0     9525 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/task.py
--rw-r--r--   0        0        0     6487 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/task_collection.py
--rw-r--r--   0        0        0    20971 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/task_enrich.py
--rw-r--r--   0        0        0     3396 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/task_identities.py
--rw-r--r--   0        0        0     4502 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/task_manager.py
--rw-r--r--   0        0        0    29060 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/task_panels.py
--rw-r--r--   0        0        0     6484 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/task_projects.py
--rw-r--r--   0        0        0     1981 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/utils/find_affiliation_conflicts.py
--rw-r--r--   0        0        0      766 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/utils/grimoirelab_valid.yml
--rwxr-xr-x   0        0        0     4709 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/utils/healthcheck.py
--rw-r--r--   0        0        0        0 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/utils/logs/all.log
--rw-r--r--   0        0        0     7846 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/utils/micro.py
--rw-r--r--   0        0        0     2858 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/utils/panels_config.py
--rw-r--r--   0        0        0      864 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/utils/projects.json
--rw-r--r--   0        0        0     3141 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/utils/projects_json2yml.py
--rw-r--r--   0        0        0     3634 2023-02-03 09:05:05.882106 sirmordred-0.6.1/sirmordred/utils/setup.cfg
--rw-r--r--   0        0        0     4398 2023-02-03 09:05:05.882106 sirmordred-0.6.1/tests/aliases.json
--rw-r--r--   0        0        0   497664 2023-02-03 09:05:05.886106 sirmordred-0.6.1/tests/archives/askbot.archive
--rw-r--r--   0        0        0   150528 2023-02-03 09:05:05.886106 sirmordred-0.6.1/tests/archives/bugzilla.archive
--rw-r--r--   0        0        0    52224 2023-02-03 09:05:05.886106 sirmordred-0.6.1/tests/archives/bugzillarest.archive
--rw-r--r--   0        0        0    73728 2023-02-03 09:05:05.886106 sirmordred-0.6.1/tests/archives/confluence.archive
--rw-r--r--   0        0        0  7141376 2023-02-03 09:05:05.910107 sirmordred-0.6.1/tests/archives/crates.archive
--rw-r--r--   0        0        0   291840 2023-02-03 09:05:05.910107 sirmordred-0.6.1/tests/archives/discourse.archive
--rw-r--r--   0        0        0    16384 2023-02-03 09:05:05.910107 sirmordred-0.6.1/tests/archives/dockerhub.archive
--rw-r--r--   0        0        0  1713152 2023-02-03 09:05:05.914107 sirmordred-0.6.1/tests/archives/functest.archive
--rw-r--r--   0        0        0    49152 2023-02-03 09:05:05.914107 sirmordred-0.6.1/tests/archives/gerrit.archive
--rw-r--r--   0        0        0  9424896 2023-02-03 09:05:05.982109 sirmordred-0.6.1/tests/archives/github-issue.archive
--rw-r--r--   0        0        0 23023616 2023-02-03 09:05:06.006111 sirmordred-0.6.1/tests/archives/github-pull.archive
--rw-r--r--   0        0        0   208896 2023-02-03 09:05:06.010111 sirmordred-0.6.1/tests/archives/gitlab-issue.archive
--rw-r--r--   0        0        0   937984 2023-02-03 09:05:06.010111 sirmordred-0.6.1/tests/archives/gitlab-merge.archive
--rw-r--r--   0        0        0    65536 2023-02-03 09:05:06.010111 sirmordred-0.6.1/tests/archives/googlehits.archive
--rw-r--r--   0        0        0   228352 2023-02-03 09:05:06.010111 sirmordred-0.6.1/tests/archives/jenkins.archive
--rw-r--r--   0        0        0    86016 2023-02-03 09:05:06.014111 sirmordred-0.6.1/tests/archives/jira.archive
--rw-r--r--   0        0        0    69632 2023-02-03 09:05:06.014111 sirmordred-0.6.1/tests/archives/launchpad.archive
--rw-r--r--   0        0        0    31744 2023-02-03 09:05:06.014111 sirmordred-0.6.1/tests/archives/mediawiki-1.23.archive
--rw-r--r--   0        0        0   245760 2023-02-03 09:05:06.014111 sirmordred-0.6.1/tests/archives/mediawiki-1.28.archive
--rw-r--r--   0        0        0   136192 2023-02-03 09:05:06.014111 sirmordred-0.6.1/tests/archives/meetup.archive
--rw-r--r--   0        0        0  2310144 2023-02-03 09:05:06.018111 sirmordred-0.6.1/tests/archives/mozillaclub.archive
--rw-r--r--   0        0        0    35840 2023-02-03 09:05:06.018111 sirmordred-0.6.1/tests/archives/nntp.archive
--rw-r--r--   0        0        0    88064 2023-02-03 09:05:06.018111 sirmordred-0.6.1/tests/archives/phabricator.archive
--rw-r--r--   0        0        0    61440 2023-02-03 09:05:06.018111 sirmordred-0.6.1/tests/archives/redmine.archive
--rw-r--r--   0        0        0   182272 2023-02-03 09:05:06.022111 sirmordred-0.6.1/tests/archives/remo.archive
--rw-r--r--   0        0        0    25600 2023-02-03 09:05:06.022111 sirmordred-0.6.1/tests/archives/rss.archive
--rw-r--r--   0        0        0    86016 2023-02-03 09:05:06.022111 sirmordred-0.6.1/tests/archives/slack.archive
--rw-r--r--   0        0        0    17408 2023-02-03 09:05:06.022111 sirmordred-0.6.1/tests/archives/stackexchange.archive
--rw-r--r--   0        0        0    15360 2023-02-03 09:05:06.022111 sirmordred-0.6.1/tests/archives/telegram.archive
--rw-r--r--   0        0        0   385024 2023-02-03 09:05:06.022111 sirmordred-0.6.1/tests/archives/twitter.archive
--rw-r--r--   0        0        0     1769 2023-02-03 09:05:05.882106 sirmordred-0.6.1/tests/archives-test-projects.json
--rw-r--r--   0        0        0     5845 2023-02-03 09:05:05.882106 sirmordred-0.6.1/tests/archives-test.cfg
--rw-r--r--   0        0        0 15031534 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/eclipse-projects.json
--rw-r--r--   0        0        0       55 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/healthcheck_cache_invalid.json
--rw-r--r--   0        0        0       56 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/healthcheck_cache_valid.json
--rw-r--r--   0        0        0       56 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/healthcheck_cache_wrong_key.json
--rw-r--r--   0        0        0     2932 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/mordred.log
--rw-r--r--   0        0        0     3244 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/orgs_sortinghat.json
--rw-r--r--   0        0        0     3587 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/perceval_identities_sortinghat.json
--rw-r--r--   0        0        0     3607 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/remote_identities_sortinghat.json
--rw-r--r--   0        0        0     2032 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/task-identities-data.json
--rw-r--r--   0        0        0     4487 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/task-params-expected
--rw-r--r--   0        0        0     1716 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/task-params-test-projects.json
--rw-r--r--   0        0        0     4392 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/task-params-test.cfg
--rw-r--r--   0        0        0     2484 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/data/url-projects.json
--rwxr-xr-x   0        0        0     1166 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/run_tests.py
--rw-r--r--   0        0        0     6562 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/sortinghat_settings.py
--rw-r--r--   0        0        0     1451 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test-no-collection.cfg
--rw-r--r--   0        0        0     4655 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test-no-sh.cfg
--rw-r--r--   0        0        0      178 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test-projects-no-collection.json
--rw-r--r--   0        0        0     2484 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test-projects.json
--rw-r--r--   0        0        0      721 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test-repos-projects.json
--rw-r--r--   0        0        0     1798 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test-repos.cfg
--rw-r--r--   0        0        0     4936 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test.cfg
--rw-r--r--   0        0        0    14731 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_config.py
--rw-r--r--   0        0        0     1849 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_github.py
--rw-r--r--   0        0        0     3235 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_healthcheck.py
--rw-r--r--   0        0        0     2706 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_sirmordred.py
--rw-r--r--   0        0        0     7303 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_studies.cfg
--rw-r--r--   0        0        0     5392 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_task.py
--rw-r--r--   0        0        0     5956 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_task_collection.py
--rw-r--r--   0        0        0    11770 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_task_enrich.py
--rw-r--r--   0        0        0     5817 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_task_identities.py
--rw-r--r--   0        0        0    10141 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_task_manager.py
--rw-r--r--   0        0        0     6380 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_task_panels.py
--rw-r--r--   0        0        0    13869 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_task_projects.py
--rw-r--r--   0        0        0     1499 2023-02-03 09:05:06.070113 sirmordred-0.6.1/tests/test_wrong.cfg
--rw-r--r--   0        0        0    43802 1970-01-01 00:00:00.000000 sirmordred-0.6.1/setup.py
--rw-r--r--   0        0        0    42490 1970-01-01 00:00:00.000000 sirmordred-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-04-21 10:41:35.706321 sirmordred-0.7.0rc1/LICENSE
+-rw-r--r--   0        0        0    40852 2023-04-21 10:41:35.706321 sirmordred-0.7.0rc1/README.md
+-rw-r--r--   0        0        0     8246 2023-04-21 10:41:35.710322 sirmordred-0.7.0rc1/menu.yaml
+-rw-r--r--   0        0        0     2171 2023-04-21 10:41:35.710322 sirmordred-0.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      835 2023-04-21 10:41:35.710322 sirmordred-0.7.0rc1/sirmordred/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/_version.py
+-rwxr-xr-x   0        0        0     4924 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/bin/sirmordred.py
+-rw-r--r--   0        0        0    33274 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/config.py
+-rw-r--r--   0        0        0     1836 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/error.py
+-rw-r--r--   0        0        0     2306 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/github.py
+-rwxr-xr-x   0        0        0    12799 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/sirmordred.py
+-rw-r--r--   0        0        0     9687 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/task.py
+-rw-r--r--   0        0        0     6487 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/task_collection.py
+-rw-r--r--   0        0        0    21022 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/task_enrich.py
+-rw-r--r--   0        0        0     3396 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/task_identities.py
+-rw-r--r--   0        0        0     4502 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/task_manager.py
+-rw-r--r--   0        0        0    29060 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/task_panels.py
+-rw-r--r--   0        0        0     6484 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/task_projects.py
+-rw-r--r--   0        0        0     1981 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/utils/find_affiliation_conflicts.py
+-rw-r--r--   0        0        0      766 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/utils/grimoirelab_valid.yml
+-rwxr-xr-x   0        0        0     4709 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/utils/healthcheck.py
+-rw-r--r--   0        0        0        0 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/utils/logs/all.log
+-rw-r--r--   0        0        0     7846 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/utils/micro.py
+-rw-r--r--   0        0        0     2858 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/utils/panels_config.py
+-rw-r--r--   0        0        0      864 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/utils/projects.json
+-rw-r--r--   0        0        0     3141 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/utils/projects_json2yml.py
+-rw-r--r--   0        0        0     3634 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/sirmordred/utils/setup.cfg
+-rw-r--r--   0        0        0     4398 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/tests/aliases.json
+-rw-r--r--   0        0        0   497664 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/tests/archives/askbot.archive
+-rw-r--r--   0        0        0   150528 2023-04-21 10:41:35.718322 sirmordred-0.7.0rc1/tests/archives/bugzilla.archive
+-rw-r--r--   0        0        0    52224 2023-04-21 10:41:35.718322 sirmordred-0.7.0rc1/tests/archives/bugzillarest.archive
+-rw-r--r--   0        0        0    73728 2023-04-21 10:41:35.718322 sirmordred-0.7.0rc1/tests/archives/confluence.archive
+-rw-r--r--   0        0        0  7141376 2023-04-21 10:41:35.742323 sirmordred-0.7.0rc1/tests/archives/crates.archive
+-rw-r--r--   0        0        0   291840 2023-04-21 10:41:35.742323 sirmordred-0.7.0rc1/tests/archives/discourse.archive
+-rw-r--r--   0        0        0    16384 2023-04-21 10:41:35.742323 sirmordred-0.7.0rc1/tests/archives/dockerhub.archive
+-rw-r--r--   0        0        0  1713152 2023-04-21 10:41:35.746323 sirmordred-0.7.0rc1/tests/archives/functest.archive
+-rw-r--r--   0        0        0    49152 2023-04-21 10:41:35.746323 sirmordred-0.7.0rc1/tests/archives/gerrit.archive
+-rw-r--r--   0        0        0  9424896 2023-04-21 10:41:35.818326 sirmordred-0.7.0rc1/tests/archives/github-issue.archive
+-rw-r--r--   0        0        0 23023616 2023-04-21 10:41:35.850327 sirmordred-0.7.0rc1/tests/archives/github-pull.archive
+-rw-r--r--   0        0        0   208896 2023-04-21 10:41:35.850327 sirmordred-0.7.0rc1/tests/archives/gitlab-issue.archive
+-rw-r--r--   0        0        0   937984 2023-04-21 10:41:35.854327 sirmordred-0.7.0rc1/tests/archives/gitlab-merge.archive
+-rw-r--r--   0        0        0    65536 2023-04-21 10:41:35.854327 sirmordred-0.7.0rc1/tests/archives/googlehits.archive
+-rw-r--r--   0        0        0   228352 2023-04-21 10:41:35.854327 sirmordred-0.7.0rc1/tests/archives/jenkins.archive
+-rw-r--r--   0        0        0    86016 2023-04-21 10:41:35.854327 sirmordred-0.7.0rc1/tests/archives/jira.archive
+-rw-r--r--   0        0        0    69632 2023-04-21 10:41:35.854327 sirmordred-0.7.0rc1/tests/archives/launchpad.archive
+-rw-r--r--   0        0        0    31744 2023-04-21 10:41:35.854327 sirmordred-0.7.0rc1/tests/archives/mediawiki-1.23.archive
+-rw-r--r--   0        0        0   245760 2023-04-21 10:41:35.854327 sirmordred-0.7.0rc1/tests/archives/mediawiki-1.28.archive
+-rw-r--r--   0        0        0   136192 2023-04-21 10:41:35.858327 sirmordred-0.7.0rc1/tests/archives/meetup.archive
+-rw-r--r--   0        0        0  2310144 2023-04-21 10:41:35.862327 sirmordred-0.7.0rc1/tests/archives/mozillaclub.archive
+-rw-r--r--   0        0        0    35840 2023-04-21 10:41:35.862327 sirmordred-0.7.0rc1/tests/archives/nntp.archive
+-rw-r--r--   0        0        0    88064 2023-04-21 10:41:35.862327 sirmordred-0.7.0rc1/tests/archives/phabricator.archive
+-rw-r--r--   0        0        0    61440 2023-04-21 10:41:35.862327 sirmordred-0.7.0rc1/tests/archives/redmine.archive
+-rw-r--r--   0        0        0   182272 2023-04-21 10:41:35.862327 sirmordred-0.7.0rc1/tests/archives/remo.archive
+-rw-r--r--   0        0        0    25600 2023-04-21 10:41:35.862327 sirmordred-0.7.0rc1/tests/archives/rss.archive
+-rw-r--r--   0        0        0    86016 2023-04-21 10:41:35.866328 sirmordred-0.7.0rc1/tests/archives/slack.archive
+-rw-r--r--   0        0        0    17408 2023-04-21 10:41:35.866328 sirmordred-0.7.0rc1/tests/archives/stackexchange.archive
+-rw-r--r--   0        0        0    15360 2023-04-21 10:41:35.866328 sirmordred-0.7.0rc1/tests/archives/telegram.archive
+-rw-r--r--   0        0        0   385024 2023-04-21 10:41:35.866328 sirmordred-0.7.0rc1/tests/archives/twitter.archive
+-rw-r--r--   0        0        0     1769 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/tests/archives-test-projects.json
+-rw-r--r--   0        0        0     5845 2023-04-21 10:41:35.714322 sirmordred-0.7.0rc1/tests/archives-test.cfg
+-rw-r--r--   0        0        0 15031534 2023-04-21 10:41:35.914329 sirmordred-0.7.0rc1/tests/data/eclipse-projects.json
+-rw-r--r--   0        0        0       55 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/healthcheck_cache_invalid.json
+-rw-r--r--   0        0        0       56 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/healthcheck_cache_valid.json
+-rw-r--r--   0        0        0       56 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/healthcheck_cache_wrong_key.json
+-rw-r--r--   0        0        0     2932 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/mordred.log
+-rw-r--r--   0        0        0     3244 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/orgs_sortinghat.json
+-rw-r--r--   0        0        0     3587 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/perceval_identities_sortinghat.json
+-rw-r--r--   0        0        0     3607 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/remote_identities_sortinghat.json
+-rw-r--r--   0        0        0     2032 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/task-identities-data.json
+-rw-r--r--   0        0        0     4487 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/task-params-expected
+-rw-r--r--   0        0        0     1716 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/task-params-test-projects.json
+-rw-r--r--   0        0        0     4392 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/task-params-test.cfg
+-rw-r--r--   0        0        0     2484 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/data/url-projects.json
+-rwxr-xr-x   0        0        0     1166 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/run_tests.py
+-rw-r--r--   0        0        0     6562 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/sortinghat_settings.py
+-rw-r--r--   0        0        0     1451 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test-no-collection.cfg
+-rw-r--r--   0        0        0     4655 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test-no-sh.cfg
+-rw-r--r--   0        0        0      178 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test-projects-no-collection.json
+-rw-r--r--   0        0        0     2484 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test-projects.json
+-rw-r--r--   0        0        0      721 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test-repos-projects.json
+-rw-r--r--   0        0        0     1798 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test-repos.cfg
+-rw-r--r--   0        0        0     4936 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test.cfg
+-rw-r--r--   0        0        0    14731 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_config.py
+-rw-r--r--   0        0        0     1849 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_github.py
+-rw-r--r--   0        0        0     3235 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_healthcheck.py
+-rw-r--r--   0        0        0     2706 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_sirmordred.py
+-rw-r--r--   0        0        0     7303 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_studies.cfg
+-rw-r--r--   0        0        0     5392 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_task.py
+-rw-r--r--   0        0        0     5956 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_task_collection.py
+-rw-r--r--   0        0        0    11770 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_task_enrich.py
+-rw-r--r--   0        0        0     5817 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_task_identities.py
+-rw-r--r--   0        0        0    10141 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_task_manager.py
+-rw-r--r--   0        0        0     6380 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_task_panels.py
+-rw-r--r--   0        0        0    13869 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_task_projects.py
+-rw-r--r--   0        0        0     1499 2023-04-21 10:41:35.918330 sirmordred-0.7.0rc1/tests/test_wrong.cfg
+-rw-r--r--   0        0        0    42493 1970-01-01 00:00:00.000000 sirmordred-0.7.0rc1/PKG-INFO
```

### Comparing `sirmordred-0.6.1/LICENSE` & `sirmordred-0.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/README.md` & `sirmordred-0.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/menu.yaml` & `sirmordred-0.7.0rc1/menu.yaml`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/pyproject.toml` & `sirmordred-0.7.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sirmordred"
-version = "0.6.1"
+version = "0.7.0-rc.1"
 description = "Drive GrimoireLab tools to produce a dashboard"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `sirmordred-0.6.1/sirmordred/__init__.py` & `sirmordred-0.7.0rc1/sirmordred/__init__.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/bin/sirmordred.py` & `sirmordred-0.7.0rc1/sirmordred/bin/sirmordred.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -56,15 +56,15 @@
     elif args.config_files is None:
         Logger.error("Option -t or -c is required")
         return 1
 
     try:
         config = Config(args.config_files[0], args.config_files[1:])
         config_dict = config.get_conf()
-        logs_dir = config_dict['general']['logs_dir']
+        logs_dir = config_dict['general'].get('logs_dir', None)
         debug_mode = config_dict['general']['debug']
         logger = setup_logs(logs_dir, debug_mode)
     except RuntimeError as error:
         print("Error while consuming configuration: {}".format(error))
         return 1
 
     if args.phases:
@@ -83,28 +83,32 @@
     if debug_mode:
         logging_mode = logging.DEBUG
     else:
         logging_mode = logging.INFO
 
     logger = logging.getLogger()
     logger.setLevel(logging_mode)
-    # create file handler which logs even debug messages
 
-    fh_filepath = os.path.join(logs_dir, 'all.log')
-    fh = logging.FileHandler(fh_filepath)
-    fh.setLevel(logging_mode)
-    # create console handler with a higher log level
-    ch = logging.StreamHandler()
-    ch.setLevel(logging.ERROR)
     # create formatter and add it to the handlers
     formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-    fh.setFormatter(formatter)
+
+    # create file handler
+    if logs_dir:
+        fh_filepath = os.path.join(logs_dir, 'all.log')
+        fh = logging.FileHandler(fh_filepath)
+        fh.setLevel(logging_mode)
+        # Set format
+        fh.setFormatter(formatter)
+        # add the handlers to the logger
+        logger.addHandler(fh)
+
+    # create console handler
+    ch = logging.StreamHandler()
+    ch.setLevel(logging_mode)
     ch.setFormatter(formatter)
-    # add the handlers to the logger
-    logger.addHandler(fh)
     logger.addHandler(ch)
 
     # this is needed because the perceval log messages are similar to ELK/mordred ones
     if not debug_mode:
         logging.getLogger('perceval').setLevel(logging.WARNING)
 
     logging.getLogger('requests').setLevel(logging.WARNING)
```

### Comparing `sirmordred-0.6.1/sirmordred/config.py` & `sirmordred-0.7.0rc1/sirmordred/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,16 +125,16 @@
                 "debug": {
                     "optional": False,
                     "default": True,
                     "type": bool,
                     "description": "Debug mode (logging mainly)"
                 },
                 "logs_dir": {
-                    "optional": False,
-                    "default": "logs",
+                    "optional": True,
+                    "default": None,
                     "type": str,
                     "description": "Directory with the logs of sirmordred"
                 },
                 "bulk_size": {
                     "optional": True,
                     "default": 1000,
                     "type": int,
@@ -478,14 +478,20 @@
                     "description": "GraphQL server port"
                 },
                 "ssl": {
                     "optional": True,
                     "default": False,
                     "type": bool,
                     "description": "GraphQL server use SSL/TSL connection"
+                },
+                "verify_ssl": {
+                    "optional": True,
+                    "default": True,
+                    "type": bool,
+                    "description": "Verify SSL connection to the server"
                 }
             }
         }
 
         tasks_config_params = [params_collection, params_enrichment, params_panels, params_sortinghat]
         for section_params in tasks_config_params:
             params.update(section_params)
```

### Comparing `sirmordred-0.6.1/sirmordred/error.py` & `sirmordred-0.7.0rc1/sirmordred/error.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/github.py` & `sirmordred-0.7.0rc1/sirmordred/github.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/sirmordred.py` & `sirmordred-0.7.0rc1/sirmordred/sirmordred.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/task.py` & `sirmordred-0.7.0rc1/sirmordred/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,19 +51,21 @@
         self.db_sh = sortinghat['database'] if sortinghat else None
         self.db_user = sortinghat['user'] if sortinghat else None
         self.db_password = sortinghat['password'] if sortinghat else None
         self.db_host = sortinghat['host'] if sortinghat else '127.0.0.1'
         self.db_path = sortinghat.get('path', None) if sortinghat else None
         self.db_port = sortinghat.get('port', None) if sortinghat else None
         self.db_ssl = sortinghat.get('ssl', False) if sortinghat else False
+        self.db_verify_ssl = sortinghat.get('verify_ssl', True) if sortinghat else True
         self.db_unaffiliate_group = sortinghat['unaffiliated_group'] if sortinghat else None
         if sortinghat:
             self.client = SortingHatClient(host=self.db_host, port=self.db_port,
                                            path=self.db_path, ssl=self.db_ssl,
-                                           user=self.db_user, password=self.db_password)
+                                           user=self.db_user, password=self.db_password,
+                                           verify_ssl=self.db_verify_ssl)
             self.client.connect()
         else:
             self.client = None
 
         self.grimoire_con = grimoire_con(conn_retries=12)  # 30m retry
 
     @staticmethod
```

### Comparing `sirmordred-0.6.1/sirmordred/task_collection.py` & `sirmordred-0.7.0rc1/sirmordred/task_collection.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/task_enrich.py` & `sirmordred-0.7.0rc1/sirmordred/task_enrich.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,15 @@
                                None,  # args.events_enrich
                                self.db_user,
                                self.db_password,
                                self.db_host,
                                self.db_port,
                                self.db_path,
                                self.db_ssl,
+                               self.db_verify_ssl,
                                None,  # args.refresh_projects,
                                None,  # args.refresh_identities,
                                author_id=None,
                                author_uuid=None,
                                filter_raw=filter_raw,
                                jenkins_rename_file=jenkins_rename_file,
                                unaffiliated_group=self.db_unaffiliate_group,
```

### Comparing `sirmordred-0.6.1/sirmordred/task_identities.py` & `sirmordred-0.7.0rc1/sirmordred/task_identities.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/task_manager.py` & `sirmordred-0.7.0rc1/sirmordred/task_manager.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/task_panels.py` & `sirmordred-0.7.0rc1/sirmordred/task_panels.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/task_projects.py` & `sirmordred-0.7.0rc1/sirmordred/task_projects.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/utils/find_affiliation_conflicts.py` & `sirmordred-0.7.0rc1/sirmordred/utils/find_affiliation_conflicts.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/utils/grimoirelab_valid.yml` & `sirmordred-0.7.0rc1/sirmordred/utils/grimoirelab_valid.yml`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/utils/healthcheck.py` & `sirmordred-0.7.0rc1/sirmordred/utils/healthcheck.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/utils/micro.py` & `sirmordred-0.7.0rc1/sirmordred/utils/micro.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/utils/panels_config.py` & `sirmordred-0.7.0rc1/sirmordred/utils/panels_config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/utils/projects.json` & `sirmordred-0.7.0rc1/sirmordred/utils/projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/utils/projects_json2yml.py` & `sirmordred-0.7.0rc1/sirmordred/utils/projects_json2yml.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/sirmordred/utils/setup.cfg` & `sirmordred-0.7.0rc1/sirmordred/utils/setup.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/aliases.json` & `sirmordred-0.7.0rc1/tests/aliases.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/askbot.archive` & `sirmordred-0.7.0rc1/tests/archives/askbot.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/bugzilla.archive` & `sirmordred-0.7.0rc1/tests/archives/bugzilla.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/bugzillarest.archive` & `sirmordred-0.7.0rc1/tests/archives/bugzillarest.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/confluence.archive` & `sirmordred-0.7.0rc1/tests/archives/confluence.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/crates.archive` & `sirmordred-0.7.0rc1/tests/archives/crates.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/discourse.archive` & `sirmordred-0.7.0rc1/tests/archives/discourse.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/dockerhub.archive` & `sirmordred-0.7.0rc1/tests/archives/dockerhub.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/functest.archive` & `sirmordred-0.7.0rc1/tests/archives/functest.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/gerrit.archive` & `sirmordred-0.7.0rc1/tests/archives/gerrit.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/github-issue.archive` & `sirmordred-0.7.0rc1/tests/archives/github-issue.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/github-pull.archive` & `sirmordred-0.7.0rc1/tests/archives/github-pull.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/gitlab-issue.archive` & `sirmordred-0.7.0rc1/tests/archives/gitlab-issue.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/gitlab-merge.archive` & `sirmordred-0.7.0rc1/tests/archives/gitlab-merge.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/googlehits.archive` & `sirmordred-0.7.0rc1/tests/archives/googlehits.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/jenkins.archive` & `sirmordred-0.7.0rc1/tests/archives/jenkins.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/jira.archive` & `sirmordred-0.7.0rc1/tests/archives/jira.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/launchpad.archive` & `sirmordred-0.7.0rc1/tests/archives/launchpad.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/mediawiki-1.23.archive` & `sirmordred-0.7.0rc1/tests/archives/mediawiki-1.23.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/mediawiki-1.28.archive` & `sirmordred-0.7.0rc1/tests/archives/mediawiki-1.28.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/meetup.archive` & `sirmordred-0.7.0rc1/tests/archives/meetup.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/mozillaclub.archive` & `sirmordred-0.7.0rc1/tests/archives/mozillaclub.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/nntp.archive` & `sirmordred-0.7.0rc1/tests/archives/nntp.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/phabricator.archive` & `sirmordred-0.7.0rc1/tests/archives/phabricator.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/redmine.archive` & `sirmordred-0.7.0rc1/tests/archives/redmine.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/remo.archive` & `sirmordred-0.7.0rc1/tests/archives/remo.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/rss.archive` & `sirmordred-0.7.0rc1/tests/archives/rss.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/slack.archive` & `sirmordred-0.7.0rc1/tests/archives/slack.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/stackexchange.archive` & `sirmordred-0.7.0rc1/tests/archives/stackexchange.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/telegram.archive` & `sirmordred-0.7.0rc1/tests/archives/telegram.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives/twitter.archive` & `sirmordred-0.7.0rc1/tests/archives/twitter.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives-test-projects.json` & `sirmordred-0.7.0rc1/tests/archives-test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/archives-test.cfg` & `sirmordred-0.7.0rc1/tests/archives-test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/data/eclipse-projects.json` & `sirmordred-0.7.0rc1/tests/data/eclipse-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/data/mordred.log` & `sirmordred-0.7.0rc1/tests/data/mordred.log`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/data/orgs_sortinghat.json` & `sirmordred-0.7.0rc1/tests/data/orgs_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/data/perceval_identities_sortinghat.json` & `sirmordred-0.7.0rc1/tests/data/perceval_identities_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/data/remote_identities_sortinghat.json` & `sirmordred-0.7.0rc1/tests/data/remote_identities_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/data/task-identities-data.json` & `sirmordred-0.7.0rc1/tests/data/task-identities-data.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/data/task-params-expected` & `sirmordred-0.7.0rc1/tests/data/task-params-expected`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/data/task-params-test-projects.json` & `sirmordred-0.7.0rc1/tests/data/task-params-test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/data/task-params-test.cfg` & `sirmordred-0.7.0rc1/tests/data/task-params-test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/data/url-projects.json` & `sirmordred-0.7.0rc1/tests/data/url-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/run_tests.py` & `sirmordred-0.7.0rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/sortinghat_settings.py` & `sirmordred-0.7.0rc1/tests/sortinghat_settings.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test-no-collection.cfg` & `sirmordred-0.7.0rc1/tests/test-no-collection.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test-no-sh.cfg` & `sirmordred-0.7.0rc1/tests/test-no-sh.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test-projects.json` & `sirmordred-0.7.0rc1/tests/test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test-repos-projects.json` & `sirmordred-0.7.0rc1/tests/test-repos-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test-repos.cfg` & `sirmordred-0.7.0rc1/tests/test-repos.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test.cfg` & `sirmordred-0.7.0rc1/tests/test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_config.py` & `sirmordred-0.7.0rc1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_github.py` & `sirmordred-0.7.0rc1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_healthcheck.py` & `sirmordred-0.7.0rc1/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_sirmordred.py` & `sirmordred-0.7.0rc1/tests/test_sirmordred.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_studies.cfg` & `sirmordred-0.7.0rc1/tests/test_studies.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_task.py` & `sirmordred-0.7.0rc1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_task_collection.py` & `sirmordred-0.7.0rc1/tests/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_task_enrich.py` & `sirmordred-0.7.0rc1/tests/test_task_enrich.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_task_identities.py` & `sirmordred-0.7.0rc1/tests/test_task_identities.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_task_manager.py` & `sirmordred-0.7.0rc1/tests/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_task_panels.py` & `sirmordred-0.7.0rc1/tests/test_task_panels.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_task_projects.py` & `sirmordred-0.7.0rc1/tests/test_task_projects.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/tests/test_wrong.cfg` & `sirmordred-0.7.0rc1/tests/test_wrong.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.6.1/setup.py` & `sirmordred-0.7.0rc1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,1503 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sirmordred
+Version: 0.7.0rc1
+Summary: Drive GrimoireLab tools to produce a dashboard
+Home-page: https://chaoss.github.io/grimoirelab/
+License: GPL-3.0+
+Keywords: development,grimoirelab
+Author: GrimoireLab Developers
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Requires-Dist: cereslib (>=0.3)
+Requires-Dist: colorlog (==4.1.0)
+Requires-Dist: elasticsearch (==6.3.1)
+Requires-Dist: elasticsearch-dsl (==6.3.1)
+Requires-Dist: file-read-backwards (==2.0.0)
+Requires-Dist: graal (>=0.3)
+Requires-Dist: grimoire-elk (>=0.102)
+Requires-Dist: grimoirelab-panels (>=0.1)
+Requires-Dist: grimoirelab-toolkit (>=0.3)
+Requires-Dist: kidash (>=0.5)
+Requires-Dist: perceval (>=0.19)
+Requires-Dist: perceval-mozilla (>=0.3)
+Requires-Dist: perceval-opnfv (>=0.2)
+Requires-Dist: perceval-puppet (>=0.2)
+Requires-Dist: perceval-weblate (>=0.2)
+Requires-Dist: sortinghat (>=0.7.20)
+Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-sirmordred/issues
+Project-URL: Repository, https://github.com/chaoss/grimoirelab-sirmordred
+Description-Content-Type: text/markdown
 
-packages = \
-['sirmordred', 'sirmordred.bin', 'sirmordred.utils', 'tests']
+# SirMordred [![Build Status](https://github.com/chaoss/grimoirelab-sirmordred/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-sirmordred/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://coveralls.io/repos/github/chaoss/grimoirelab-sirmordred/badge.svg?branch=master)](https://coveralls.io/github/chaoss/grimoirelab-sirmordred?branch=master) [![PyPI version](https://badge.fury.io/py/sirmordred.svg)](https://badge.fury.io/py/sirmordred)
 
-package_data = \
-{'': ['*'], 'sirmordred.utils': ['logs/*'], 'tests': ['archives/*', 'data/*']}
+SirMordred is the tool used to coordinate the execution of the GrimoireLab platform, via two main configuration files, the `setup.cfg` and `projects.json`, which are summarized in their corresponding sections.
 
-install_requires = \
-['cereslib>=0.3',
- 'colorlog==4.1.0',
- 'elasticsearch-dsl==6.3.1',
- 'elasticsearch==6.3.1',
- 'file-read-backwards==2.0.0',
- 'graal>=0.3',
- 'grimoire-elk>=0.102',
- 'grimoirelab-panels>=0.1',
- 'grimoirelab-toolkit>=0.3',
- 'kidash>=0.5',
- 'perceval-mozilla>=0.3',
- 'perceval-opnfv>=0.2',
- 'perceval-puppet>=0.2',
- 'perceval-weblate>=0.2',
- 'perceval>=0.19',
- 'sortinghat>=0.7.20']
-
-entry_points = \
-{'console_scripts': ['healthcheck.py = sirmordred.utils.healthcheck:main',
-                     'micro.py = sirmordred.utils.micro:main',
-                     'panels_config.py = sirmordred.utils.panels_config:main',
-                     'sirmordred = sirmordred.bin.sirmordred:main']}
-
-setup_kwargs = {
-    'name': 'sirmordred',
-    'version': '0.6.1',
-    'description': 'Drive GrimoireLab tools to produce a dashboard',
-    'long_description': '# SirMordred [![Build Status](https://github.com/chaoss/grimoirelab-sirmordred/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-sirmordred/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://coveralls.io/repos/github/chaoss/grimoirelab-sirmordred/badge.svg?branch=master)](https://coveralls.io/github/chaoss/grimoirelab-sirmordred?branch=master) [![PyPI version](https://badge.fury.io/py/sirmordred.svg)](https://badge.fury.io/py/sirmordred)\n\nSirMordred is the tool used to coordinate the execution of the GrimoireLab platform, via two main configuration files, the `setup.cfg` and `projects.json`, which are summarized in their corresponding sections.\n\n## Contents\n\n* [Setup.cfg](#setupcfg-)\n* [Projects.json](#projectsjson-)\n* [Supported data sources](#supported-data-sources-)\n* [Micro Mordred](#micro-mordred-)\n* [Getting started](/Getting-Started.md#getting-started-)\n* [Troubleshooting](/Getting-Started.md#troubleshooting-)\n* [How to](/Getting-Started.md#how-to-)\n\n\n## Setup.cfg [&uarr;](#contents)\n\nThe setup file holds the configuration to arrange all processes underlying GrimoireLab. It is composed of sections that allow defining the general settings such as which phases to activate (e.g., collection, enrichment) and where to store the logs, as well as the location and credentials for SortingHat and the ElasticSearch instances where the raw and enriched data is stored. Furthermore, it also includes backend sections to set up the parameters used by Perceval to access the software development tools (e.g., GitHub tokens, Gerrit username) and fetch their data.\n\nDashboards can be automatically uploaded via the `setup.cfg` if the phase `panels` is enabled. The `Data Status` and `Overview` dashboards will contain\nwidgets that summarize the information of the data sources declared in the `setup.cfg`. Note that the widgets are not updated when adding\nnew data sources, thus you need to manually delete the dashboards `Data Status` and `Overview` (under **Stack Management > Saved Objects** in Kibiter), and restart mordred again (making sure that the option `panels` is enabled).\n\n### [es_collection]\n\n * **url** (str: http://172.17.0.1:9200): Elasticsearch URL (**Required**)\n### [es_enrichment]\n\n * **autorefresh** (bool: True): Execute the autorefresh of identities\n * **autorefresh_interval** (int: 2): Time interval (days) to autorefresh identities\n * **url** (str: http://172.17.0.1:9200): Elasticsearch URL (**Required**)\n### [general]\n\n * **bulk_size** (int: 1000): Number of items to write in Elasticsearch using bulk operations\n * **debug** (bool: True): Debug mode (logging mainly) (**Required**)\n * **logs_dir** (str: logs): Directory with the logs of sirmordred (**Required**)\n * **min_update_delay** (int: 60): Short delay between tasks (collect, enrich ...)\n * **scroll_size** (int: 100): Number of items to read from Elasticsearch when scrolling\n * **short_name** (str: Short name): Short name of the project (**Required**)\n * **update** (bool: False): Execute the tasks in loop (**Required**)\n * **aliases_file** (str: ./aliases.json): JSON file to define aliases for raw and enriched indexes\n * **menu_file** (str: ./menu.yaml): YAML file to define the menus to be shown in Kibiter\n * **global_data_sources** (list: bugzilla, bugzillarest, confluence, discourse, gerrit, jenkins, jira): List of data sources collected globally, they are declared in the section \'unknown\' of the projects.json\n * **retention_time** (int: None): the maximum number of minutes wrt the current date to retain the data\n * **update_hour** (int: None): The hour of the day the tasks will run ignoring `min_update_delay` (collect, enrich ...)\n### [panels]\n\n * **community** (bool: True): Include community section in dashboard\n * **kibiter_default_index** (str: git): Default index pattern for Kibiter\n * **kibiter_time_from** (str: now-90d): Default time interval for Kibiter\n * **kibiter_url** (str): Kibiter URL (**Required**)\n * **kibiter_version** (str: None): Kibiter version\n * **kafka** (bool: False): Include KIP section in dashboard\n * **github-comments** (bool: False): Enable GitHub comments menu. Note that if enabled, the github2:issue and github2:pull sections in the setup.cfg and projects.json should be declared\n * **github-events** (bool: False): Enable GitHub events menu. Note that if enabled, the github:event section in the setup.cfg and projects.json should be declared\n * **github-repos** (bool: False): Enable GitHub repo stats menu. Note that if enabled, the github:repo section in the setup.cfg and projects.json should be declared\n * **gitlab-issues** (bool: False): Enable GitLab issues menu. Note that if enabled, the gitlab:issue section in the setup.cfg and projects.json should be declared\n * **gitlab-merges** (bool: False): Enable GitLab merge requests menu. Note that if enabled, the gitlab:merge sections in the setup.cfg and projects.json should be declared\n * **mattermost** (bool: False): Enable Mattermost menu\n * **code-license** (bool: False): Enable code license menu. Note that if enabled, colic sections in the setup.cfg and projects.json should be declared\n * **code-complexity** (bool: False): Enable code complexity menu. Note that if enabled, cocom sections in the setup.cfg and projects.json should be declared\n * **strict** (bool: True): Enable strict panels loading\n * **contact** (str: None): Support repository URL\n### [phases]\n\n * **collection** (bool: True): Activate collection of items (**Required**)\n * **enrichment** (bool: True): Activate enrichment of items (**Required**)\n * **identities** (bool: True): Do the identities tasks (**Required**)\n * **panels** (bool: True): Load panels, create alias and other tasks related (**Required**)\n\n### [projects]\n\n * **projects_file** (str: projects.json): Projects file path with repositories to be collected grouped by projects\n * **projects_url** (str: None): Projects file URL, the projects_file is required to store the file locally\n### [sortinghat]\n\n * **affiliate** (bool: True): Affiliate identities to organizations (**Required**)\n * **autogender** (bool: False): Add gender to the profiles (executes autogender)\n * **autoprofile** (list: [\'customer\', \'git\', \'github\']): Order in which to get the identities information for filling the profile (**Required**)\n * **database** (str: sortinghat_db): Name of the Sortinghat database (**Required**)\n * **host** (str: 127.0.0.1):  Host with the Sortinghat database (**Required**)\n * **port** (int: None):  GraphQL server port\n * **path** (str: None) GraphQL path\n * **ssl** (bool: False) GraphQL server use SSL/TSL connection\n * **matching** (list: [\'email\']): Algorithm for matching identities in Sortinghat (**Required**)\n * **password** (str: ): Password to access the Sortinghat database (**Required**)\n * **reset_on_load** (bool: False): Unmerge and remove affiliations for all identities on load\n * **sleep_for** (int: 3600): Delay between task identities executions (**Required**)\n * **strict_mapping** (bool: True): rigorous check of values in identities matching (i.e, well formed email addresses, non-overlapping enrollment periods)\n * **unaffiliated_group** (str: Unknown): Name of the organization for unaffiliated identities (**Required**)\n * **user** (str: root): User to access the Sortinghat database (**Required**)\n### [backend-name:tag] (tag is optional)\n\n* **collect** (bool: True): enable/disable collection phase\n* **raw_index** (str: None): Index name in which to store the raw items (**Required**)\n* **enriched_index** (str: None): Index name in which to store the enriched items (**Required**)\n* **studies** (list: []): List of studies to be executed\n* **anonymize** (bool: False): enable/disable anonymization of personal user information\n* **backend-param-1**: ..\n* **backend-param-2**: ..\n* **backend-param-n**: ..\n\nThe template of a backend section is shown above.\nFurther information about Perceval backends parameters are available at:\n\n* Params details: https://perceval.readthedocs.io/en/latest/perceval/perceval-backends.html\n* Examples: https://github.com/chaoss/grimoirelab-sirmordred/blob/master/tests/test_studies.cfg\n\nNote that some backend sections allow to specify specific enrichment options, which are listed below.\n\n### [jenkins]\n* **node_regex**: regular expression for extracting node name from `builtOn` field. This\n  regular expression **must contain at least one group**. First group will be used to extract\n  node name. More groups are allowed but not used to extract anything else.\n\n### [studies-name:tag] (tag is optional)\n\n* **study-param-1**: ..\n* **study-param-2**: ..\n* **study-param-n**: ..\n\nA template of a study section is shown above. A complete list of studies parameters is available at:\n\n* https://github.com/chaoss/grimoirelab-sirmordred/blob/master/tests/test_studies.cfg\n\n## Projects.json [&uarr;](#contents)\n\nThe projects.json aims at describing the repositories grouped by a project that will be shown on the dashboards.\n\nThe project file enables the users to list the instances of the software development tools to analyse, such\nas local and remote Git repositories, the URLs of GitHub and GitLab issue trackers, and the name of Slack channels.\nFurthermore, it also allows the users to organize these instances into nested groups, which structure is reflected in\nthe visualization artifacts (i.e., documents and dashboards). Groups can be useful to represent projects within a single\ncompany, sub-projects within a large project such as Linux and Eclipse, or the organizations within a collaborative project.\n\n1. First level: project names\n2. Second level: data sources and metadata\n3. Third level: data source URLs\n\nThere are some filters, labels, and a special section:\n* Filter `--filter-no-collection=true`: This filter is used to show old enriched data within the dashboards from\nrepositories that don\'t exist anymore in upstream.\n* Filter `--filter-raw` and the section `unknown`: The data sources will only collected at the section `unknown`\nbut this allow to add the same source in different sections to enrich using the filter `--filter-raw`.\n* Label ` --labels=[example]`: The data source will have the label of `example` which can be used to create visualisations for specific sets of data\n* Section `unknown`: If the data source is only under this section it will be enriched as project `main`.\n\n```\n{\n    "Chaoss": {\n        "gerrit": [\n            "gerrit.chaoss.org --filter-raw=data.projects:CHAOSS"\n        ]\n        "git": [\n            "https:/github.com/chaoss/grimoirelab-perceval",\n            "https://<username>:<api-token>@github.com/chaoss/grimoirelab-sirmordred"\n        ],\n        "github": [\n            "https:/github.com/chaoss/grimoirelab-perceval --filter-no-collection=true",\n            "https:/github.com/chaoss/grimoirelab-sirmordred  --labels=[example]"\n        ]\n    },\n    "GrimoireLab": {\n        "gerrit": [\n            "gerrit.chaoss.org --filter-raw=data.projects:GrimoireLab"\n        ],\n        "meta": {\n            "title": "GrimoireLab",\n            "type": "Dev",\n            "program" : "Bitergia",\n            "state": "Operating"\n        },\n    }\n    "unknown": {\n        "gerrit": [\n            "gerrit.chaoss.org"\n        ],\n        "confluence": [\n            "https://wiki.chaoss.org"\n        ]\n}\n```\nIn the projects.json above:\n* The data included in the repo `gerrit.chaoss.org` will be collected entirely since the\nrepo is listed in the `unknown` section. However only the project `GrimoireLab` will be enriched as declared in the\n`GrimoireLab` section.\n* In the section `Chaoss` in the data source `github` the repository `grimoirelab-perceval` is not collected for\nraw index but it will enriched in the enriched index.\n* In the section `GrimoireLab` the metadata will showed in the enriched index as extra fields.\n* In the section `unknown` the data source `confluence` will be enriched as the project `main`.\n\n## Supported data sources [&uarr;](#contents)\n\nThese are the data sources GrimoireLab supports: [askbot](#askbot-), [bugzilla](#bugzilla-), [bugzillarest](#bugzillarest-), [cocom](#cocom-), [colic](#colic-), [confluence](#confluence-), [crates](#crates-), [discourse](#discourse-), [dockerhub](#dockerhub-), [dockerdeps](#dockerdeps-), [dockersmells](#dockersmells-), [functest](#functest-), [gerrit](#gerrit-), [git](#git-), [github](#github-), [github2](#github2-), [gitlab](#gitlab-), [gitter](#gitter-), [google_hits](#google_hits-), [groupsio](#groupsio-), [hyperkitty](#hyperkitty-), [jenkins](#jenkins-), [jira](#jira-), [kitsune](#kitsune-), [mattermost](#mattermost-), [mbox](#mbox-), [mediawiki](#mediawiki-), [meetup](#meetup-), [mozillaclub](#mozillaclub-), [nntp](#nntp-), [pagure](#pagure-), [phabricator](#phabricator-), [pipermail](#pipermail-), [puppetforge](#puppetforge-), [redmine](#redmine-), [remo](#remo-), [rocketchat](#rocketchat-), [rss](#rss-), [slack](#slack-), [stackexchange](#stackexchange-), [supybot](#supybot-), [telegram](#telegram-), [twitter](#twitter-)\n\n#### askbot [&uarr;](#supported-data-sources-)\nQuestions and answers from Askbot site\n- projects.json\n```\n{\n    "Chaoss": {\n        "askbot": [\n            "https://askbot.org/"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[askbot]\nraw_index = askbot_raw\nenriched_index = askbot_enriched\n```\n#### bugzilla [&uarr;](#supported-data-sources-)\nBugs from Bugzilla\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "bugzilla": [\n            "https://bugs.eclipse.org/bugs/"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[bugzilla]\nraw_index = bugzilla_raw\nenriched_index = bugzilla_enriched\nbackend-user = yyyy (optional)\nbackend-password = xxxx (optional)\nno-archive = true (suggested)\n```\n#### bugzillarest [&uarr;](#supported-data-sources-)\nBugs from Bugzilla server (>=5.0) using its REST API\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "bugzillarest": [\n            "https://bugzilla.mozilla.org"\n        ]\n    }\n}\n```\n\n- setup.cfg\n```\n[bugzillarest]\nraw_index = bugzillarest_raw\nenriched_index = bugzillarest_enriched\nbackend-user = yyyy (optional)\nbackend-password = xxxx (optional)\nno-archive = true (suggested)\n```\n#### cocom [&uarr;](#supported-data-sources-)\nCode complexity integration.\nSome graal dependencies like `cloc` might be required, https://github.com/chaoss/grimoirelab-graal#how-to-installcreate-the-executables\n\n- projects.json\n```\n{\n    "Chaoss":{\n        "cocom": [\n            "https://github.com/chaoss/grimoirelab-toolkit"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[cocom]\nraw_index = cocom_chaoss\nenriched_index = cocom_chaoss_enrich\ncategory = code_complexity_lizard_file\nstudies = [enrich_cocom_analysis]\nbranches = master\nworktree-path = /tmp/cocom/\n```\n#### colic [&uarr;](#supported-data-sources-)\nCode license backend.\n- projects.json\n```\n{\n    "Chaoss":{\n        "colic": [\n            "https://github.com/chaoss/grimoirelab-toolkit"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[colic]\nraw_index = colic_chaoss\nenriched_index = colic_chaoss_enrich\ncategory = code_license_nomos\nstudies = [enrich_colic_analysis]\nexec-path = /usr/share/fossology/nomos/agent/nomossa\nbranches = master\nworktree-path = /tmp/colic\n```\n#### confluence [&uarr;](#supported-data-sources-)\ncontents from Confluence\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "confluence": [\n            "https://wiki.open-o.org/"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[confluence]\nraw_index = confluence_raw\nenriched_index = confluence_enriched\nno-archive = true (suggested)\n```\n#### crates [&uarr;](#supported-data-sources-)\npackages from Crates.io\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "crates": [\n            ""\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[crates]\nraw_index = crates_raw\nenriched_index = crates_enriched\n```\n#### discourse [&uarr;](#supported-data-sources-)\nTopics from Discourse\n- projects.json\n```\n{\n    "Chaoss": {\n        "discourse": [\n            "https://foro.mozilla-hispano.org/"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[discourse]\nraw_index = discourse_raw\nenriched_index = discourse_enriched\nno-archive = true (suggested)\n```\n#### dockerhub [&uarr;](#supported-data-sources-)\nRepositories info from DockerHub\n- projects.json\n```\n{\n    "Chaoss": {\n        "dockerhub": [\n            "bitergia kibiter"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[dockerhub]\nraw_index = dockerhub_raw\nenriched_index = dockerhub_enriched\nno-archive = true (suggested)\n```\n#### dockerdeps [&uarr;](#supported-data-sources-)\nDependencies extracted from Dockerfiles. Requires https://github.com/crossminer/crossJadolint\n- projects.json\n```\n{\n    "Chaoss": {\n        "dockerdeps": [\n            "https://github.com/chaoss/grimoirelab"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[dockerdeps]\nraw_index = dockerdeps_raw\nenriched_index = dockerdeps_enrich\ncategory = code_dependencies_jadolint\nexec-path = <jadolint-local-path>/jadolint.jar\nin-paths = [Dockerfile, Dockerfile-full, Dockerfile-secured, Dockerfile-factory, Dockerfile-installed]\n```\n#### dockersmells [&uarr;](#supported-data-sources-)\nSmells extracted from Dockerfiles. Requires https://github.com/crossminer/crossJadolint\n- projects.json\n```\n{\n    "Chaoss": {\n        "dockersmells": [\n            "https://github.com/chaoss/grimoirelab"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[dockersmells]\nraw_index = dockersmells_raw\nenriched_index = dockersmells_enrich\ncategory = code_quality_jadolint\nexec-path = <jadolint-local-path>/jadolint.jar\nin-paths = [Dockerfile, Dockerfile-full, Dockerfile-secured, Dockerfile-factory, Dockerfile-installed]\n```\n#### functest [&uarr;](#supported-data-sources-)\nTests from functest\n- projects.json\n```\n{\n    "Chaoss": {\n        "functest": [\n            "http://testresults.opnfv.org/test/"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[functest]\nraw_index = functest_raw\nenriched_index = functest_enriched\nno-archive = true (suggested)\n```\n#### gerrit [&uarr;](#supported-data-sources-)\nReviews from Gerrit\n\nYou have to add your public key in the gerrit server.\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "gerrit": [\n            "review.opendev.org"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[gerrit]\nraw_index = gerrit_raw\nenriched_index = gerrit_enriched\nuser = xxxx\nno-archive = true (suggested)\nblacklist-ids = [] (optional)\nmax-reviews = 500 (optional)\nstudies = [enrich_demography:gerrit, enrich_onion:gerrit, enrich_demography_contribution:gerrit] (optional)\n\n[enrich_demography:gerrit] (optional)\n\n[enrich_onion:gerrit] (optional)\nin_index = gerrit_enriched\nout_index = gerrit-onion_enriched\n\n[enrich_demography_contribution:gerrit] (optional)\ndate_field = grimoire_creation_date\nauthor_field = author_uuid\n```\n#### git [&uarr;](#supported-data-sources-)\nCommits from Git\n\n**Note:** If you want to analyze private git repositories, make sure you pass the credentials directly in the URL.\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "git": [\n            "https:/github.com/chaoss/grimoirelab-perceval",\n            "https://<username>:<api-token>@github.com/chaoss/grimoirelab-sirmordred"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[git]\nraw_index = git_raw\nenriched_index = git_enriched\nlatest-items = true (suggested)\nstudies = [enrich_demography:git, enrich_git_branches:git, enrich_areas_of_code:git, enrich_onion:git, enrich_extra_data:git] (optional)\n\n[enrich_demography:git] (optional)\n\n[enrich_git_branches:git] (optional)\nrun_month_days = [1, 23] (optional)\n\n[enrich_areas_of_code:git] (optional)\nin_index = git_raw\nout_index = git-aoc_enriched\n\n[enrich_onion:git] (optional)\nin_index = git_enriched\nout_index = git-onion_enriched\n\n[enrich_extra_data:git]\njson_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt\n\n[enrich_forecast_activity]\nout_index = git_study_forecast\n```\n#### github [&uarr;](#supported-data-sources-)\nIssues and PRs from GitHub\n\n##### issue\n- projects.json\n```\n{\n    "Chaoss": {\n        "github:issue": [\n            "https:/github.com/chaoss/grimoirelab-perceval",\n            "https:/github.com/chaoss/grimoirelab-sirmordred"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[github:issue]\nraw_index = github_raw\nenriched_index = github_enriched\napi-token = xxxx\ncategory = issue\nsleep-for-rate = true\nno-archive = true (suggested)\nstudies = [enrich_onion:github,\n           enrich_geolocation:user,\n           enrich_geolocation:assignee,\n           enrich_extra_data:github,\n           enrich_backlog_analysis,\n           enrich_demography:github] (optional)\n\n[enrich_onion:github] (optional)\nin_index_iss = github_issues_onion-src\nin_index_prs = github_prs_onion-src\nout_index_iss = github-issues-onion_enriched\nout_index_prs = github-prs-onion_enriched\n\n[enrich_geolocation:user] (optional)\nlocation_field = user_location\ngeolocation_field = user_geolocation\n\n[enrich_geolocation:assignee] (optional)\nlocation_field = assignee_location\ngeolocation_field = assignee_geolocation\n\n[enrich_extra_data:github]\njson_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt\n\n[enrich_backlog_analysis]\nout_index = github_enrich_backlog\ninterval_days = 7\nreduced_labels = [bug,enhancement]\nmap_label = [others, bugs, enhancements]\n\n[enrich_demography:github]\n```\n##### pull request\n- projects.json\n```\n{\n    "Chaoss": {\n        "github:pull": [\n            "https:/github.com/chaoss/grimoirelab-perceval",\n            "https:/github.com/chaoss/grimoirelab-sirmordred"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[github:pull]\nraw_index = github-pull_raw\nenriched_index = github-pull_enriched\napi-token = xxxx\ncategory = pull_request\nsleep-for-rate = true\nno-archive = true (suggested)\nstudies = [enrich_geolocation:user,\n           enrich_geolocation:assignee,\n           enrich_extra_data:github,\n           enrich_demography:github] (optional)\n\n[enrich_geolocation:user]\nlocation_field = user_location\ngeolocation_field = user_geolocation\n\n[enrich_geolocation:assignee]\nlocation_field = assignee_location\ngeolocation_field = assignee_geolocation\n\n[enrich_extra_data:github]\njson_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt\n\n[enrich_demography:github]\n```\n##### repo\nThe number of forks, stars, and subscribers in the repository.\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "github:repo": [\n            "https:/github.com/chaoss/grimoirelab-perceval",\n            "https:/github.com/chaoss/grimoirelab-sirmordred"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[github:repo]\nraw_index = github-repo_raw\nenriched_index = github-repo_enriched\napi-token = xxxx\ncategory = repository\nsleep-for-rate = true\nno-archive = true (suggested)\nstudies = [enrich_extra_data:github, enrich_demography:github]\n\n[enrich_extra_data:github]\njson_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt\n\n[enrich_demography:github]\n```\n#### githubql [&uarr;](#supported-data-sources-)\nEvents from GitHub\n\nThe corresponding dashboards can be automatically uploaded by setting `github-events`\nto `true` in the `panels` section within the `setup.cfg`\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "githubql": [\n            "https://github.com/chaoss/grimoirelab-toolkit"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[panels]\ngithub-events = true\n\n[githubql]\nraw_index = github_event_raw\nenriched_index = github_event_enriched\napi-token = xxxxx\nsleep-for-rate = true\nsleep-time = "300" (optional)\nno-archive = true (suggested)\nstudies = [enrich_duration_analysis:kanban, enrich_reference_analysis] (optional)\n\n[enrich_duration_analysis:kanban]\nstart_event_type = MovedColumnsInProjectEvent\nfltr_attr = board_name\ntarget_attr = board_column\nfltr_event_types = [MovedColumnsInProjectEvent, AddedToProjectEvent]\n\n[enrich_duration_analysis:label]\nstart_event_type = UnlabeledEvent\ntarget_attr = label\nfltr_attr = label\nfltr_event_types = [LabeledEvent]\n\n[enrich_reference_analysis] (optional)\n```\n\n#### github2 [&uarr;](#supported-data-sources-)\nComments from GitHub\n\nThe corresponding dashboards can be automatically uploaded by setting `github-comments`\nto `true` in the `panels` section within the `setup.cfg`\n\n##### issue\n- projects.json\n```\n{\n    "Chaoss": {\n        "github2:issue": [\n            "https:/github.com/chaoss/grimoirelab-perceval",\n            "https:/github.com/chaoss/grimoirelab-sirmordred"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[github2:issue]\napi-token = xxxx\nraw_index = github2-issues_raw\nenriched_index = github2-issues_enriched\nsleep-for-rate = true\ncategory = issue\nno-archive = true (suggested)\nstudies = [enrich_geolocation:user, enrich_geolocation:assignee, enrich_extra_data:github2, enrich_feelings] (optional)\n\n[enrich_geolocation:user] (optional)\nlocation_field = user_location\ngeolocation_field = user_geolocation\n\n[enrich_geolocation:assignee] (optional)\nlocation_field = assignee_location\ngeolocation_field = assignee_geolocation\n\n[enrich_extra_data:github2]\njson_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt\n\n[enrich_feelings]\nattributes = [title, body]\nnlp_rest_url = http://localhost:2901\n```\n##### pull request\n- projects.json\n```\n{\n    "Chaoss": {\n        "github2:pull": [\n            "https:/github.com/chaoss/grimoirelab-perceval",\n            "https:/github.com/chaoss/grimoirelab-sirmordred"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[github2:pull]\napi-token = xxxx\nraw_index = github2-pull_raw\nenriched_index = github2-pull_enriched\nsleep-for-rate = true\ncategory = pull_request\nno-archive = true (suggested)\nstudies = [enrich_geolocation:user, enrich_geolocation:assignee, enrich_extra_data:git, enrich_feelings] (optional)\n\n[enrich_geolocation:user] (optional)\nlocation_field = user_location\ngeolocation_field = user_geolocation\n\n[enrich_geolocation:assignee] (optional)\nlocation_field = assignee_location\ngeolocation_field = assignee_geolocation\n\n[enrich_extra_data:github2]\njson_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt\n\n[enrich_feelings]\nattributes = [title, body]\nnlp_rest_url = http://localhost:2901\n```\n\n#### gitlab [&uarr;](#supported-data-sources-)\nIssues and MRs from GitLab\n\nGitLab issues and merge requests need to be configured in two different sections.\nThe corresponding dashboards can be automatically uploaded by setting `gitlab-issue` and `gitlab-merge`\nto `true` in the `panels` section within the `setup.cfg`\n\nIf a given GitLab repository is under more than 1 level, all the slashes `/` starting from the second level have to be\nreplaced by `%2F`. For instance, for a repository with a structure similar to this one\n`https://gitlab.com/Molly/lab/first`.\n##### issue\n- projects.json\n```\n{\n    "Chaoss": {\n        "gitlab:issue": [\n            "https://gitlab.com/Molly/first",\n            "https://gitlab.com/Molly/lab%2Fsecond"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[panels]\ngitlab-issues = true\n\n[gitlab:issue]\ncategory = issue\nraw_index = gitlab-issues_raw\nenriched_index = gitlab-issues_enriched\napi-token = xxxx\nsleep-for-rate = true\nno-archive = true (suggested)\nstudies = [enrich_onion:gitlab-issue] (optional)\n\n[enrich_onion:gitlab-issue] (optional)\nin_index = gitlab-issues_enriched\nout_index = gitlab-issues-onion_enriched\ndata_source = gitlab-issues\n```\n##### merge request\n- projects.json\n```\n{\n    "Chaoss": {\n        "gitlab:merge": [\n            "https://gitlab.com/Molly/first",\n            "https://gitlab.com/Molly/lab%2Fsecond"\n        ],\n    }\n}\n```\n- setup.cfg\n```\n[panels]\ngitlab-merges = true\n\n[gitlab:merge]\ncategory = merge_request\nraw_index = gitlab-mrs_raw\nenriched_index = gitlab-mrs_enriched\napi-token = xxxx\nsleep-for-rate = true\nno-archive = true (suggested)\nstudies = [enrich_onion:gitlab-merge] (optional)\n\n[enrich_onion:gitlab-merge] (optional)\nin_index = gitlab-mrs_enriched\nout_index = gitlab-mrs-onion_enriched\ndata_source = gitlab-merges\n\n```\n#### gitter [&uarr;](#supported-data-sources-)\nMessages from gitter rooms\n\nYou have to join the rooms you want to mine.\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "gitter": [\n            "https://gitter.im/jenkinsci/jenkins",\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[gitter]\nraw_index = gitter_raw\nenriched_index = gitter_enriched_raw\napi-token = xxxxx\nsleep-for-rate = true\nsleep-time = "300" (optional)\nno-archive = true (suggested)\n```\n\n#### google_hits [&uarr;](#supported-data-sources-)\nNumber of hits for a set of keywords from Google\n- projects.json\n```\n{\n    "Chaoss": {\n        "google_hits": [\n            "bitergia grimoirelab"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[google_hits]\nraw_index = google_hits_raw\nenriched_index =google_hits_enriched\n```\n#### groupsio [&uarr;](#supported-data-sources-)\nMessages from Groupsio\n\nTo know the lists you are subscribed to: https://gist.github.com/valeriocos/ad33a0b9b2d13a8336230c8c59df3c55\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "groupsio": [\n            "group1",\n            "group2"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[groupsio]\nraw_index = groupsio_raw\nenriched_index = groupsio_enriched\nemail = yyyy\npassword = xxxx\n```\n#### hyperkitty [&uarr;](#supported-data-sources-)\nMessages from a HyperKitty\n- projects.json\n```\n{\n    "Chaoss": {\n        "hyperkitty": [\n            "https://lists.mailman3.org/archives/list/mailman-users@mailman3.org"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[hyperkitty]\nraw_index = hyperkitty_raw\nenriched_index = hyperkitty_enriched\n```\n#### jenkins [&uarr;](#supported-data-sources-)\nBuilds from a Jenkins\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "jenkins": [\n            "https://build.opnfv.org/ci"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[jenkins]\nraw_index = jenkins_raw\nenriched_index = jenkins_enriched\nno-archive = true (suggested)\n```\n#### jira [&uarr;](#supported-data-sources-)\nIssues data from JIRA issue trackers\n\n- projects.json\n```\n{\n    "Chaoss":{\n        "jira": [\n            "https://jira.opnfv.org"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[jira]\nraw_index = jira_raw\nenriched_index = jira_enriched\nno-archive = true (suggested)\nbackend-user = yyyy (optional)\nbackend-password = xxxx (optional)\n```\n#### kitsune [&uarr;](#supported-data-sources-)\nQuestions and answers from KitSune\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "kitsune": [\n            ""\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[kitsune]\nraw_index = kitsune_raw\nenriched_index = kitsune_enriched\n```\n\n#### mattermost [&uarr;](#supported-data-sources-)\nMessages from Mattermost channels\n- projects.json\n```\n{\n    "Chaoss": {\n        "mattermost": [\n            "https://chat.openshift.io 8j366ft5affy3p36987pcugaoa"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[mattermost]\nraw_index = mattermost_raw\nenriched_index = mattermost_enriched\napi-token = xxxx\nstudies = [enrich_demography:mattermost] (optional)\n\n[enrich_demography:mattermost] (optional)\n```\n#### mbox [&uarr;](#supported-data-sources-)\nMessages from MBox files\n\nFor mbox files, it is needed the name of the mailing list and the path where the mboxes can be found. In the example\nbelow, the name of the mailing list is set to "mirageos-devel".\n- projects.json\n```\n{\n    "Chaoss": {\n        "mbox": [\n            "mirageos-devel /home/bitergia/mbox/mirageos-devel/"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[mbox]\nraw_index = mbox_raw\nenriched_index = mbox_enriched\n```\n#### mediawiki [&uarr;](#supported-data-sources-)\nPages and revisions from MediaWiki\n\n-projects.json\n```\n{\n    "Chaoss": {\n        "mediawiki": [\n            "https://www.mediawiki.org/w https://www.mediawiki.org/wiki"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[mediawiki]\nraw_index = mediawiki_raw\nenriched_index = mediawiki_enriched\nno-archive = true (suggested)\n```\n#### meetup [&uarr;](#supported-data-sources-)\nEvents from Meetup groups\n\nFor meetup groups it is only needed the identifier of the meetup group\nand an API token: https://chaoss.github.io/grimoirelab-tutorial/gelk/meetup.html#gathering-meetup-groups-data\n- projects.json\n```\n{\n    "Chaoss": {\n        "meetup": [\n        "Alicante-Bitergia-Users-Group",\n        "South-East-Bitergia-User-Group"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[meetup]\nraw_index = meetup_raw\nenriched_index = meetup_enriched\napi-token = xxxx\nsleep-for-rate = true\nsleep-time = "300" (optional)\nno-archive = true (suggested)\n\n```\n#### mozillaclub [&uarr;](#supported-data-sources-)\nEvents from Mozillaclub\n- projects.json\n```\n{\n    "Chaoss": {\n        "mozillaclub": [\n            "https://spreadsheets.google.com/feeds/cells/1QHl2bjBhMslyFzR5XXPzMLdzzx7oeSKTbgR5PM8qp64/ohaibtm/public/values?alt=json"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[mozillaclub]\nraw_index = mozillaclub_raw\nenriched_index = mozillaclub_enriched\n```\n#### nntp [&uarr;](#supported-data-sources-)\nArticles from NNTP newsgroups\n\nThe way to setup netnews is adding the server and the news channel to be monitored. In the example below,\nthe `news.myproject.org` is the server name.\n- projects.json\n```\n{\n    "Chaoss": {\n        "nntp": [\n            "news.myproject.org mozilla.dev.tech.crypto.checkins",\n            "news.myproject.org mozilla.dev.tech.electrolysis",\n            "news.myproject.org mozilla.dev.tech.gfx",\n            "news.myproject.org mozilla.dev.tech.java"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[nntp]\nraw_index = nntp_raw\nenriched_index =  nntp_enriched\n```\n#### pagure [&uarr;](#supported-data-sources-)\nIssues from Pagure repositories\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "pagure": [\n            "https://pagure.io/Test-group/Project-example-namespace"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[pagure]\nraw_index = pagure_raw\nenriched_index = pagure_enriched\napi-token = xxxx\nsleep-for-rate = true\nsleep-time = "300" (optional)\nno-archive = true (suggested)\n```\n#### phabricator [&uarr;](#supported-data-sources-)\nTasks from Phabricator\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "phabricator": [\n            "https://phabricator.wikimedia.org"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[phabricator]\nraw_index = phabricator_raw\nenriched_index = phabricator_enriched\napi-token = xxxx\nno-archive = true (suggested)\n```\n#### pipermail [&uarr;](#supported-data-sources-)\nMessages from Pipermail\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "pipermail": [\n            "https://lists.linuxfoundation.org/pipermail/grimoirelab-discussions/"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[pipermail]\nraw_index = pipermail_raw\nenriched_index = pipermail_enriched\n```\n#### puppetforge [&uarr;](#supported-data-sources-)\nModules and their releases from Puppet\'s forge\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "puppetforge": [\n            ""\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[puppetforge]\nraw_index = puppetforge_raw\nenriched_index = puppetforge_enriched\n```\n#### redmine [&uarr;](#supported-data-sources-)\nIssues from Redmine\n- project.json\n```\n{\n    "Chaoss": {\n        "redmine": [\n            "http://tracker.ceph.com/"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[redmine]\nraw_index = redmine_raw\nenriched_index = redmine_enriched\napi-token = XXXXX\n```\n#### remo [&uarr;](#supported-data-sources-)\nEvents, people and activities from ReMo\n- project.json\n```\n{\n    "Chaoss": {\n        "remo": [\n            "https://reps.mozilla.org"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[remo]\nraw_index = remo_raw\nenriched_index = remo_enriched\n```\n#### rocketchat [&uarr;](#supported-data-sources-)\nMessages from Rocketchat channels\n- projects.json\n```\n{\n    "Chaoss": {\n        "rocketchat": [\n            "https://open.rocket.chat general"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[rocketchat]\nraw_index = rocketchat_raw\nenriched_index = rocketchat_enriched\napi-token = xxxx\nsleep-for-rate = true\nuser-id = xxxx\nno-archive = true (suggested)\n```\n#### rss [&uarr;](#supported-data-sources-)\nEntries from RSS feeds\n\n- project.json\n```\n{\n    "Chaoss": {\n        "remo": [\n            "https://reps.mozilla.org"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[rss]\nraw_index = rss_raw\nenriched_index = rss_enriched\n```\n#### slack [&uarr;](#supported-data-sources-)\nMessages from Slack channels\n\nThe information needed to monitor slack channels is the channel id.\n- projects.json\n```\n{\n    "Chaoss": {\n        "slack": [\n            "A195YQBLL",\n            "A495YQBM2"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[slack]\nraw_index = slack_raw\nenriched_index = slack_enriched\napi-token = xxxx\nno-archive = true (suggested)\n```\n#### stackexchange [&uarr;](#supported-data-sources-)\nQuestions, answers and comments from StackExchange\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "stackexchange": [\n            "http://stackoverflow.com/questions/tagged/chef",\n            "http://stackoverflow.com/questions/tagged/chefcookbook",\n            "http://stackoverflow.com/questions/tagged/ohai",\n            "http://stackoverflow.com/questions/tagged/test-kitchen",\n            "http://stackoverflow.com/questions/tagged/knife"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[stackexchange]\nraw_index = stackexchange_raw\nenriched_index = stackexchange_enriched\napi-token = xxxx\nno-archive = true (suggested)\n```\n#### supybot [&uarr;](#supported-data-sources-)\nMessages from Supybot log files\n\nFor supybot files, it is needed the name of the IRC channel and the path where the logs can be found. In the example\nbelow, the name of the channel is set to "irc://irc.freenode.net/atomic".\n- projects.json\n```\n{\n    "Chaoss": {\n        "supybot": [\n            "irc://irc.freenode.net/atomic /home/bitergia/irc/percevalbot/logs/ChannelLogger/freenode/#atomic"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[supybot]\nraw_index = supybot_raw\nenriched_index = supybot_enriched\n```\n\n#### telegram [&uarr;](#supported-data-sources-)\nMessages from Telegram\n\nYou need to have an API token: https://github.com/chaoss/grimoirelab-perceval#telegram\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "telegram": [\n            "Mozilla_analytics"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[telegram]\nraw_index = telegram_raw\nenriched_index = telegram_enriched\napi-token = XXXXX\n```\n#### twitter [&uarr;](#supported-data-sources-)\nMessages from Twitter\n\nYou need to provide a [search query](https://developer.twitter.com/en/docs/tweets/search/guides/build-standard-query) and an API token (which requires to create an [app](https://developer.twitter.com/en/docs/basics/apps/overview)). The script at https://gist.github.com/valeriocos/7d4d28f72f53fbce49f1512ba77ef5f6 helps obtaining a token.\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "twitter": [\n            "bitergia"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[twitter]\nraw_index = twitter_raw\nenriched_index = twitter_enriched\napi-token = XXXX\n```\n\n#### weblate [&uarr;](#supported-data-sources-)\nChanges from Weblate\n\nYou need to have an API token: The token can be obtained after registering to a weblate\ninstance (e.g., https://translations.documentfoundation.org/), via the page <instance>/accounts/profile/#api\n\n- projects.json\n```\n{\n    "Chaoss": {\n        "weblate": [\n            "https://translations.documentfoundation.org"\n        ]\n    }\n}\n```\n- setup.cfg\n```\n[weblate]\nraw_index = weblate_raw\nenriched_index = weblate_enriched\napi-token = XXXX\nno-archive = true (suggested)\nsleep-for-rate = true (suggested)\nstudies = [enrich_demography:weblate] (optional)\n\n[enrich_demography:weblate] (optional)\n```\n\n## Micro Mordred [&uarr;](#contents)\n\nMicro Mordred is a simplified version of Mordred which omits the use of its scheduler. Thus, Micro Mordred allows running single Mordred tasks (e.g., raw collection, enrichment) per execution.\n\nMicro Mordred is located in the [sirmordred/utils](https://github.com/chaoss/grimoirelab-sirmordred/tree/master/sirmordred/utils/micro.py) folder of this same repository. It can be executed via command line, its parameters are summarized below:\n```\n--debug: execute Micro Mordred in debug mode\n\n--raw: activate raw task\n\n--enrich: activate enrich task\n\n--identities: activate merge identities task\n\n--panels: activate panels task\n\n--cfg: path of the configuration file\n\n--backends: list of cfg sections where the active tasks will be executed\n\n--logs-dir: single parameter denoting the path of folder in which logs are to be stored\n```\n\nExamples of possible executions are shown below:\n```\ncd .../grimoirelab-sirmordred/sirmordred/utils/\nmicro.py --raw --enrich --cfg ./setup.cfg --backends git # execute the Raw and Enrich tasks for the Git cfg section\nmicro.py --panels # execute the Panels task to load the Sigils panels to Kibiter\nmicro.py --raw --enrich --debug --cfg ./setup.cfg --backends groupsio --logs-dir logs # execute the raw and enriched tasks for the groupsio cfg section with debug mode on and logs being saved in the folder logs in the same directory as micro.py\n```\n',
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
+## Contents
+
+* [Setup.cfg](#setupcfg-)
+* [Projects.json](#projectsjson-)
+* [Supported data sources](#supported-data-sources-)
+* [Micro Mordred](#micro-mordred-)
+* [Getting started](/Getting-Started.md#getting-started-)
+* [Troubleshooting](/Getting-Started.md#troubleshooting-)
+* [How to](/Getting-Started.md#how-to-)
+
+
+## Setup.cfg [&uarr;](#contents)
+
+The setup file holds the configuration to arrange all processes underlying GrimoireLab. It is composed of sections that allow defining the general settings such as which phases to activate (e.g., collection, enrichment) and where to store the logs, as well as the location and credentials for SortingHat and the ElasticSearch instances where the raw and enriched data is stored. Furthermore, it also includes backend sections to set up the parameters used by Perceval to access the software development tools (e.g., GitHub tokens, Gerrit username) and fetch their data.
+
+Dashboards can be automatically uploaded via the `setup.cfg` if the phase `panels` is enabled. The `Data Status` and `Overview` dashboards will contain
+widgets that summarize the information of the data sources declared in the `setup.cfg`. Note that the widgets are not updated when adding
+new data sources, thus you need to manually delete the dashboards `Data Status` and `Overview` (under **Stack Management > Saved Objects** in Kibiter), and restart mordred again (making sure that the option `panels` is enabled).
+
+### [es_collection]
+
+ * **url** (str: http://172.17.0.1:9200): Elasticsearch URL (**Required**)
+### [es_enrichment]
+
+ * **autorefresh** (bool: True): Execute the autorefresh of identities
+ * **autorefresh_interval** (int: 2): Time interval (days) to autorefresh identities
+ * **url** (str: http://172.17.0.1:9200): Elasticsearch URL (**Required**)
+### [general]
+
+ * **bulk_size** (int: 1000): Number of items to write in Elasticsearch using bulk operations
+ * **debug** (bool: True): Debug mode (logging mainly) (**Required**)
+ * **logs_dir** (str: logs): Directory with the logs of sirmordred (**Required**)
+ * **min_update_delay** (int: 60): Short delay between tasks (collect, enrich ...)
+ * **scroll_size** (int: 100): Number of items to read from Elasticsearch when scrolling
+ * **short_name** (str: Short name): Short name of the project (**Required**)
+ * **update** (bool: False): Execute the tasks in loop (**Required**)
+ * **aliases_file** (str: ./aliases.json): JSON file to define aliases for raw and enriched indexes
+ * **menu_file** (str: ./menu.yaml): YAML file to define the menus to be shown in Kibiter
+ * **global_data_sources** (list: bugzilla, bugzillarest, confluence, discourse, gerrit, jenkins, jira): List of data sources collected globally, they are declared in the section 'unknown' of the projects.json
+ * **retention_time** (int: None): the maximum number of minutes wrt the current date to retain the data
+ * **update_hour** (int: None): The hour of the day the tasks will run ignoring `min_update_delay` (collect, enrich ...)
+### [panels]
+
+ * **community** (bool: True): Include community section in dashboard
+ * **kibiter_default_index** (str: git): Default index pattern for Kibiter
+ * **kibiter_time_from** (str: now-90d): Default time interval for Kibiter
+ * **kibiter_url** (str): Kibiter URL (**Required**)
+ * **kibiter_version** (str: None): Kibiter version
+ * **kafka** (bool: False): Include KIP section in dashboard
+ * **github-comments** (bool: False): Enable GitHub comments menu. Note that if enabled, the github2:issue and github2:pull sections in the setup.cfg and projects.json should be declared
+ * **github-events** (bool: False): Enable GitHub events menu. Note that if enabled, the github:event section in the setup.cfg and projects.json should be declared
+ * **github-repos** (bool: False): Enable GitHub repo stats menu. Note that if enabled, the github:repo section in the setup.cfg and projects.json should be declared
+ * **gitlab-issues** (bool: False): Enable GitLab issues menu. Note that if enabled, the gitlab:issue section in the setup.cfg and projects.json should be declared
+ * **gitlab-merges** (bool: False): Enable GitLab merge requests menu. Note that if enabled, the gitlab:merge sections in the setup.cfg and projects.json should be declared
+ * **mattermost** (bool: False): Enable Mattermost menu
+ * **code-license** (bool: False): Enable code license menu. Note that if enabled, colic sections in the setup.cfg and projects.json should be declared
+ * **code-complexity** (bool: False): Enable code complexity menu. Note that if enabled, cocom sections in the setup.cfg and projects.json should be declared
+ * **strict** (bool: True): Enable strict panels loading
+ * **contact** (str: None): Support repository URL
+### [phases]
+
+ * **collection** (bool: True): Activate collection of items (**Required**)
+ * **enrichment** (bool: True): Activate enrichment of items (**Required**)
+ * **identities** (bool: True): Do the identities tasks (**Required**)
+ * **panels** (bool: True): Load panels, create alias and other tasks related (**Required**)
+
+### [projects]
+
+ * **projects_file** (str: projects.json): Projects file path with repositories to be collected grouped by projects
+ * **projects_url** (str: None): Projects file URL, the projects_file is required to store the file locally
+### [sortinghat]
+
+ * **affiliate** (bool: True): Affiliate identities to organizations (**Required**)
+ * **autogender** (bool: False): Add gender to the profiles (executes autogender)
+ * **autoprofile** (list: ['customer', 'git', 'github']): Order in which to get the identities information for filling the profile (**Required**)
+ * **database** (str: sortinghat_db): Name of the Sortinghat database (**Required**)
+ * **host** (str: 127.0.0.1):  Host with the Sortinghat database (**Required**)
+ * **port** (int: None):  GraphQL server port
+ * **path** (str: None) GraphQL path
+ * **ssl** (bool: False) GraphQL server use SSL/TSL connection
+ * **matching** (list: ['email']): Algorithm for matching identities in Sortinghat (**Required**)
+ * **password** (str: ): Password to access the Sortinghat database (**Required**)
+ * **reset_on_load** (bool: False): Unmerge and remove affiliations for all identities on load
+ * **sleep_for** (int: 3600): Delay between task identities executions (**Required**)
+ * **strict_mapping** (bool: True): rigorous check of values in identities matching (i.e, well formed email addresses, non-overlapping enrollment periods)
+ * **unaffiliated_group** (str: Unknown): Name of the organization for unaffiliated identities (**Required**)
+ * **user** (str: root): User to access the Sortinghat database (**Required**)
+### [backend-name:tag] (tag is optional)
+
+* **collect** (bool: True): enable/disable collection phase
+* **raw_index** (str: None): Index name in which to store the raw items (**Required**)
+* **enriched_index** (str: None): Index name in which to store the enriched items (**Required**)
+* **studies** (list: []): List of studies to be executed
+* **anonymize** (bool: False): enable/disable anonymization of personal user information
+* **backend-param-1**: ..
+* **backend-param-2**: ..
+* **backend-param-n**: ..
+
+The template of a backend section is shown above.
+Further information about Perceval backends parameters are available at:
+
+* Params details: https://perceval.readthedocs.io/en/latest/perceval/perceval-backends.html
+* Examples: https://github.com/chaoss/grimoirelab-sirmordred/blob/master/tests/test_studies.cfg
+
+Note that some backend sections allow to specify specific enrichment options, which are listed below.
+
+### [jenkins]
+* **node_regex**: regular expression for extracting node name from `builtOn` field. This
+  regular expression **must contain at least one group**. First group will be used to extract
+  node name. More groups are allowed but not used to extract anything else.
+
+### [studies-name:tag] (tag is optional)
+
+* **study-param-1**: ..
+* **study-param-2**: ..
+* **study-param-n**: ..
+
+A template of a study section is shown above. A complete list of studies parameters is available at:
+
+* https://github.com/chaoss/grimoirelab-sirmordred/blob/master/tests/test_studies.cfg
+
+## Projects.json [&uarr;](#contents)
+
+The projects.json aims at describing the repositories grouped by a project that will be shown on the dashboards.
+
+The project file enables the users to list the instances of the software development tools to analyse, such
+as local and remote Git repositories, the URLs of GitHub and GitLab issue trackers, and the name of Slack channels.
+Furthermore, it also allows the users to organize these instances into nested groups, which structure is reflected in
+the visualization artifacts (i.e., documents and dashboards). Groups can be useful to represent projects within a single
+company, sub-projects within a large project such as Linux and Eclipse, or the organizations within a collaborative project.
+
+1. First level: project names
+2. Second level: data sources and metadata
+3. Third level: data source URLs
+
+There are some filters, labels, and a special section:
+* Filter `--filter-no-collection=true`: This filter is used to show old enriched data within the dashboards from
+repositories that don't exist anymore in upstream.
+* Filter `--filter-raw` and the section `unknown`: The data sources will only collected at the section `unknown`
+but this allow to add the same source in different sections to enrich using the filter `--filter-raw`.
+* Label ` --labels=[example]`: The data source will have the label of `example` which can be used to create visualisations for specific sets of data
+* Section `unknown`: If the data source is only under this section it will be enriched as project `main`.
+
+```
+{
+    "Chaoss": {
+        "gerrit": [
+            "gerrit.chaoss.org --filter-raw=data.projects:CHAOSS"
+        ]
+        "git": [
+            "https:/github.com/chaoss/grimoirelab-perceval",
+            "https://<username>:<api-token>@github.com/chaoss/grimoirelab-sirmordred"
+        ],
+        "github": [
+            "https:/github.com/chaoss/grimoirelab-perceval --filter-no-collection=true",
+            "https:/github.com/chaoss/grimoirelab-sirmordred  --labels=[example]"
+        ]
+    },
+    "GrimoireLab": {
+        "gerrit": [
+            "gerrit.chaoss.org --filter-raw=data.projects:GrimoireLab"
+        ],
+        "meta": {
+            "title": "GrimoireLab",
+            "type": "Dev",
+            "program" : "Bitergia",
+            "state": "Operating"
+        },
+    }
+    "unknown": {
+        "gerrit": [
+            "gerrit.chaoss.org"
+        ],
+        "confluence": [
+            "https://wiki.chaoss.org"
+        ]
+}
+```
+In the projects.json above:
+* The data included in the repo `gerrit.chaoss.org` will be collected entirely since the
+repo is listed in the `unknown` section. However only the project `GrimoireLab` will be enriched as declared in the
+`GrimoireLab` section.
+* In the section `Chaoss` in the data source `github` the repository `grimoirelab-perceval` is not collected for
+raw index but it will enriched in the enriched index.
+* In the section `GrimoireLab` the metadata will showed in the enriched index as extra fields.
+* In the section `unknown` the data source `confluence` will be enriched as the project `main`.
+
+## Supported data sources [&uarr;](#contents)
+
+These are the data sources GrimoireLab supports: [askbot](#askbot-), [bugzilla](#bugzilla-), [bugzillarest](#bugzillarest-), [cocom](#cocom-), [colic](#colic-), [confluence](#confluence-), [crates](#crates-), [discourse](#discourse-), [dockerhub](#dockerhub-), [dockerdeps](#dockerdeps-), [dockersmells](#dockersmells-), [functest](#functest-), [gerrit](#gerrit-), [git](#git-), [github](#github-), [github2](#github2-), [gitlab](#gitlab-), [gitter](#gitter-), [google_hits](#google_hits-), [groupsio](#groupsio-), [hyperkitty](#hyperkitty-), [jenkins](#jenkins-), [jira](#jira-), [kitsune](#kitsune-), [mattermost](#mattermost-), [mbox](#mbox-), [mediawiki](#mediawiki-), [meetup](#meetup-), [mozillaclub](#mozillaclub-), [nntp](#nntp-), [pagure](#pagure-), [phabricator](#phabricator-), [pipermail](#pipermail-), [puppetforge](#puppetforge-), [redmine](#redmine-), [remo](#remo-), [rocketchat](#rocketchat-), [rss](#rss-), [slack](#slack-), [stackexchange](#stackexchange-), [supybot](#supybot-), [telegram](#telegram-), [twitter](#twitter-)
+
+#### askbot [&uarr;](#supported-data-sources-)
+Questions and answers from Askbot site
+- projects.json
+```
+{
+    "Chaoss": {
+        "askbot": [
+            "https://askbot.org/"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[askbot]
+raw_index = askbot_raw
+enriched_index = askbot_enriched
+```
+#### bugzilla [&uarr;](#supported-data-sources-)
+Bugs from Bugzilla
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "bugzilla": [
+            "https://bugs.eclipse.org/bugs/"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[bugzilla]
+raw_index = bugzilla_raw
+enriched_index = bugzilla_enriched
+backend-user = yyyy (optional)
+backend-password = xxxx (optional)
+no-archive = true (suggested)
+```
+#### bugzillarest [&uarr;](#supported-data-sources-)
+Bugs from Bugzilla server (>=5.0) using its REST API
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "bugzillarest": [
+            "https://bugzilla.mozilla.org"
+        ]
+    }
+}
+```
+
+- setup.cfg
+```
+[bugzillarest]
+raw_index = bugzillarest_raw
+enriched_index = bugzillarest_enriched
+backend-user = yyyy (optional)
+backend-password = xxxx (optional)
+no-archive = true (suggested)
+```
+#### cocom [&uarr;](#supported-data-sources-)
+Code complexity integration.
+Some graal dependencies like `cloc` might be required, https://github.com/chaoss/grimoirelab-graal#how-to-installcreate-the-executables
+
+- projects.json
+```
+{
+    "Chaoss":{
+        "cocom": [
+            "https://github.com/chaoss/grimoirelab-toolkit"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[cocom]
+raw_index = cocom_chaoss
+enriched_index = cocom_chaoss_enrich
+category = code_complexity_lizard_file
+studies = [enrich_cocom_analysis]
+branches = master
+worktree-path = /tmp/cocom/
+```
+#### colic [&uarr;](#supported-data-sources-)
+Code license backend.
+- projects.json
+```
+{
+    "Chaoss":{
+        "colic": [
+            "https://github.com/chaoss/grimoirelab-toolkit"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[colic]
+raw_index = colic_chaoss
+enriched_index = colic_chaoss_enrich
+category = code_license_nomos
+studies = [enrich_colic_analysis]
+exec-path = /usr/share/fossology/nomos/agent/nomossa
+branches = master
+worktree-path = /tmp/colic
+```
+#### confluence [&uarr;](#supported-data-sources-)
+contents from Confluence
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "confluence": [
+            "https://wiki.open-o.org/"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[confluence]
+raw_index = confluence_raw
+enriched_index = confluence_enriched
+no-archive = true (suggested)
+```
+#### crates [&uarr;](#supported-data-sources-)
+packages from Crates.io
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "crates": [
+            ""
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[crates]
+raw_index = crates_raw
+enriched_index = crates_enriched
+```
+#### discourse [&uarr;](#supported-data-sources-)
+Topics from Discourse
+- projects.json
+```
+{
+    "Chaoss": {
+        "discourse": [
+            "https://foro.mozilla-hispano.org/"
+        ]
+    }
 }
+```
+- setup.cfg
+```
+[discourse]
+raw_index = discourse_raw
+enriched_index = discourse_enriched
+no-archive = true (suggested)
+```
+#### dockerhub [&uarr;](#supported-data-sources-)
+Repositories info from DockerHub
+- projects.json
+```
+{
+    "Chaoss": {
+        "dockerhub": [
+            "bitergia kibiter"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[dockerhub]
+raw_index = dockerhub_raw
+enriched_index = dockerhub_enriched
+no-archive = true (suggested)
+```
+#### dockerdeps [&uarr;](#supported-data-sources-)
+Dependencies extracted from Dockerfiles. Requires https://github.com/crossminer/crossJadolint
+- projects.json
+```
+{
+    "Chaoss": {
+        "dockerdeps": [
+            "https://github.com/chaoss/grimoirelab"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[dockerdeps]
+raw_index = dockerdeps_raw
+enriched_index = dockerdeps_enrich
+category = code_dependencies_jadolint
+exec-path = <jadolint-local-path>/jadolint.jar
+in-paths = [Dockerfile, Dockerfile-full, Dockerfile-secured, Dockerfile-factory, Dockerfile-installed]
+```
+#### dockersmells [&uarr;](#supported-data-sources-)
+Smells extracted from Dockerfiles. Requires https://github.com/crossminer/crossJadolint
+- projects.json
+```
+{
+    "Chaoss": {
+        "dockersmells": [
+            "https://github.com/chaoss/grimoirelab"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[dockersmells]
+raw_index = dockersmells_raw
+enriched_index = dockersmells_enrich
+category = code_quality_jadolint
+exec-path = <jadolint-local-path>/jadolint.jar
+in-paths = [Dockerfile, Dockerfile-full, Dockerfile-secured, Dockerfile-factory, Dockerfile-installed]
+```
+#### functest [&uarr;](#supported-data-sources-)
+Tests from functest
+- projects.json
+```
+{
+    "Chaoss": {
+        "functest": [
+            "http://testresults.opnfv.org/test/"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[functest]
+raw_index = functest_raw
+enriched_index = functest_enriched
+no-archive = true (suggested)
+```
+#### gerrit [&uarr;](#supported-data-sources-)
+Reviews from Gerrit
+
+You have to add your public key in the gerrit server.
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "gerrit": [
+            "review.opendev.org"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[gerrit]
+raw_index = gerrit_raw
+enriched_index = gerrit_enriched
+user = xxxx
+no-archive = true (suggested)
+blacklist-ids = [] (optional)
+max-reviews = 500 (optional)
+studies = [enrich_demography:gerrit, enrich_onion:gerrit, enrich_demography_contribution:gerrit] (optional)
+
+[enrich_demography:gerrit] (optional)
+
+[enrich_onion:gerrit] (optional)
+in_index = gerrit_enriched
+out_index = gerrit-onion_enriched
+
+[enrich_demography_contribution:gerrit] (optional)
+date_field = grimoire_creation_date
+author_field = author_uuid
+```
+#### git [&uarr;](#supported-data-sources-)
+Commits from Git
+
+**Note:** If you want to analyze private git repositories, make sure you pass the credentials directly in the URL.
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "git": [
+            "https:/github.com/chaoss/grimoirelab-perceval",
+            "https://<username>:<api-token>@github.com/chaoss/grimoirelab-sirmordred"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[git]
+raw_index = git_raw
+enriched_index = git_enriched
+latest-items = true (suggested)
+studies = [enrich_demography:git, enrich_git_branches:git, enrich_areas_of_code:git, enrich_onion:git, enrich_extra_data:git] (optional)
+
+[enrich_demography:git] (optional)
+
+[enrich_git_branches:git] (optional)
+run_month_days = [1, 23] (optional)
+
+[enrich_areas_of_code:git] (optional)
+in_index = git_raw
+out_index = git-aoc_enriched
+
+[enrich_onion:git] (optional)
+in_index = git_enriched
+out_index = git-onion_enriched
+
+[enrich_extra_data:git]
+json_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt
+
+[enrich_forecast_activity]
+out_index = git_study_forecast
+```
+#### github [&uarr;](#supported-data-sources-)
+Issues and PRs from GitHub
+
+##### issue
+- projects.json
+```
+{
+    "Chaoss": {
+        "github:issue": [
+            "https:/github.com/chaoss/grimoirelab-perceval",
+            "https:/github.com/chaoss/grimoirelab-sirmordred"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[github:issue]
+raw_index = github_raw
+enriched_index = github_enriched
+api-token = xxxx
+category = issue
+sleep-for-rate = true
+no-archive = true (suggested)
+studies = [enrich_onion:github,
+           enrich_geolocation:user,
+           enrich_geolocation:assignee,
+           enrich_extra_data:github,
+           enrich_backlog_analysis,
+           enrich_demography:github] (optional)
+
+[enrich_onion:github] (optional)
+in_index_iss = github_issues_onion-src
+in_index_prs = github_prs_onion-src
+out_index_iss = github-issues-onion_enriched
+out_index_prs = github-prs-onion_enriched
+
+[enrich_geolocation:user] (optional)
+location_field = user_location
+geolocation_field = user_geolocation
+
+[enrich_geolocation:assignee] (optional)
+location_field = assignee_location
+geolocation_field = assignee_geolocation
+
+[enrich_extra_data:github]
+json_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt
+
+[enrich_backlog_analysis]
+out_index = github_enrich_backlog
+interval_days = 7
+reduced_labels = [bug,enhancement]
+map_label = [others, bugs, enhancements]
+
+[enrich_demography:github]
+```
+##### pull request
+- projects.json
+```
+{
+    "Chaoss": {
+        "github:pull": [
+            "https:/github.com/chaoss/grimoirelab-perceval",
+            "https:/github.com/chaoss/grimoirelab-sirmordred"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[github:pull]
+raw_index = github-pull_raw
+enriched_index = github-pull_enriched
+api-token = xxxx
+category = pull_request
+sleep-for-rate = true
+no-archive = true (suggested)
+studies = [enrich_geolocation:user,
+           enrich_geolocation:assignee,
+           enrich_extra_data:github,
+           enrich_demography:github] (optional)
+
+[enrich_geolocation:user]
+location_field = user_location
+geolocation_field = user_geolocation
+
+[enrich_geolocation:assignee]
+location_field = assignee_location
+geolocation_field = assignee_geolocation
+
+[enrich_extra_data:github]
+json_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt
+
+[enrich_demography:github]
+```
+##### repo
+The number of forks, stars, and subscribers in the repository.
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "github:repo": [
+            "https:/github.com/chaoss/grimoirelab-perceval",
+            "https:/github.com/chaoss/grimoirelab-sirmordred"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[github:repo]
+raw_index = github-repo_raw
+enriched_index = github-repo_enriched
+api-token = xxxx
+category = repository
+sleep-for-rate = true
+no-archive = true (suggested)
+studies = [enrich_extra_data:github, enrich_demography:github]
+
+[enrich_extra_data:github]
+json_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt
+
+[enrich_demography:github]
+```
+#### githubql [&uarr;](#supported-data-sources-)
+Events from GitHub
+
+The corresponding dashboards can be automatically uploaded by setting `github-events`
+to `true` in the `panels` section within the `setup.cfg`
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "githubql": [
+            "https://github.com/chaoss/grimoirelab-toolkit"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[panels]
+github-events = true
+
+[githubql]
+raw_index = github_event_raw
+enriched_index = github_event_enriched
+api-token = xxxxx
+sleep-for-rate = true
+sleep-time = "300" (optional)
+no-archive = true (suggested)
+studies = [enrich_duration_analysis:kanban, enrich_reference_analysis] (optional)
+
+[enrich_duration_analysis:kanban]
+start_event_type = MovedColumnsInProjectEvent
+fltr_attr = board_name
+target_attr = board_column
+fltr_event_types = [MovedColumnsInProjectEvent, AddedToProjectEvent]
+
+[enrich_duration_analysis:label]
+start_event_type = UnlabeledEvent
+target_attr = label
+fltr_attr = label
+fltr_event_types = [LabeledEvent]
+
+[enrich_reference_analysis] (optional)
+```
+
+#### github2 [&uarr;](#supported-data-sources-)
+Comments from GitHub
+
+The corresponding dashboards can be automatically uploaded by setting `github-comments`
+to `true` in the `panels` section within the `setup.cfg`
+
+##### issue
+- projects.json
+```
+{
+    "Chaoss": {
+        "github2:issue": [
+            "https:/github.com/chaoss/grimoirelab-perceval",
+            "https:/github.com/chaoss/grimoirelab-sirmordred"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[github2:issue]
+api-token = xxxx
+raw_index = github2-issues_raw
+enriched_index = github2-issues_enriched
+sleep-for-rate = true
+category = issue
+no-archive = true (suggested)
+studies = [enrich_geolocation:user, enrich_geolocation:assignee, enrich_extra_data:github2, enrich_feelings] (optional)
+
+[enrich_geolocation:user] (optional)
+location_field = user_location
+geolocation_field = user_geolocation
+
+[enrich_geolocation:assignee] (optional)
+location_field = assignee_location
+geolocation_field = assignee_geolocation
+
+[enrich_extra_data:github2]
+json_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt
+
+[enrich_feelings]
+attributes = [title, body]
+nlp_rest_url = http://localhost:2901
+```
+##### pull request
+- projects.json
+```
+{
+    "Chaoss": {
+        "github2:pull": [
+            "https:/github.com/chaoss/grimoirelab-perceval",
+            "https:/github.com/chaoss/grimoirelab-sirmordred"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[github2:pull]
+api-token = xxxx
+raw_index = github2-pull_raw
+enriched_index = github2-pull_enriched
+sleep-for-rate = true
+category = pull_request
+no-archive = true (suggested)
+studies = [enrich_geolocation:user, enrich_geolocation:assignee, enrich_extra_data:git, enrich_feelings] (optional)
+
+[enrich_geolocation:user] (optional)
+location_field = user_location
+geolocation_field = user_geolocation
+
+[enrich_geolocation:assignee] (optional)
+location_field = assignee_location
+geolocation_field = assignee_geolocation
+
+[enrich_extra_data:github2]
+json_url = https://gist.githubusercontent.com/zhquan/bb48654bed8a835ab2ba9a149230b11a/raw/5eef38de508e0a99fa9772db8aef114042e82e47/bitergia-example.txt
+
+[enrich_feelings]
+attributes = [title, body]
+nlp_rest_url = http://localhost:2901
+```
+
+#### gitlab [&uarr;](#supported-data-sources-)
+Issues and MRs from GitLab
+
+GitLab issues and merge requests need to be configured in two different sections.
+The corresponding dashboards can be automatically uploaded by setting `gitlab-issue` and `gitlab-merge`
+to `true` in the `panels` section within the `setup.cfg`
+
+If a given GitLab repository is under more than 1 level, all the slashes `/` starting from the second level have to be
+replaced by `%2F`. For instance, for a repository with a structure similar to this one
+`https://gitlab.com/Molly/lab/first`.
+##### issue
+- projects.json
+```
+{
+    "Chaoss": {
+        "gitlab:issue": [
+            "https://gitlab.com/Molly/first",
+            "https://gitlab.com/Molly/lab%2Fsecond"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[panels]
+gitlab-issues = true
+
+[gitlab:issue]
+category = issue
+raw_index = gitlab-issues_raw
+enriched_index = gitlab-issues_enriched
+api-token = xxxx
+sleep-for-rate = true
+no-archive = true (suggested)
+studies = [enrich_onion:gitlab-issue] (optional)
+
+[enrich_onion:gitlab-issue] (optional)
+in_index = gitlab-issues_enriched
+out_index = gitlab-issues-onion_enriched
+data_source = gitlab-issues
+```
+##### merge request
+- projects.json
+```
+{
+    "Chaoss": {
+        "gitlab:merge": [
+            "https://gitlab.com/Molly/first",
+            "https://gitlab.com/Molly/lab%2Fsecond"
+        ],
+    }
+}
+```
+- setup.cfg
+```
+[panels]
+gitlab-merges = true
+
+[gitlab:merge]
+category = merge_request
+raw_index = gitlab-mrs_raw
+enriched_index = gitlab-mrs_enriched
+api-token = xxxx
+sleep-for-rate = true
+no-archive = true (suggested)
+studies = [enrich_onion:gitlab-merge] (optional)
+
+[enrich_onion:gitlab-merge] (optional)
+in_index = gitlab-mrs_enriched
+out_index = gitlab-mrs-onion_enriched
+data_source = gitlab-merges
+
+```
+#### gitter [&uarr;](#supported-data-sources-)
+Messages from gitter rooms
+
+You have to join the rooms you want to mine.
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "gitter": [
+            "https://gitter.im/jenkinsci/jenkins",
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[gitter]
+raw_index = gitter_raw
+enriched_index = gitter_enriched_raw
+api-token = xxxxx
+sleep-for-rate = true
+sleep-time = "300" (optional)
+no-archive = true (suggested)
+```
+
+#### google_hits [&uarr;](#supported-data-sources-)
+Number of hits for a set of keywords from Google
+- projects.json
+```
+{
+    "Chaoss": {
+        "google_hits": [
+            "bitergia grimoirelab"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[google_hits]
+raw_index = google_hits_raw
+enriched_index =google_hits_enriched
+```
+#### groupsio [&uarr;](#supported-data-sources-)
+Messages from Groupsio
+
+To know the lists you are subscribed to: https://gist.github.com/valeriocos/ad33a0b9b2d13a8336230c8c59df3c55
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "groupsio": [
+            "group1",
+            "group2"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[groupsio]
+raw_index = groupsio_raw
+enriched_index = groupsio_enriched
+email = yyyy
+password = xxxx
+```
+#### hyperkitty [&uarr;](#supported-data-sources-)
+Messages from a HyperKitty
+- projects.json
+```
+{
+    "Chaoss": {
+        "hyperkitty": [
+            "https://lists.mailman3.org/archives/list/mailman-users@mailman3.org"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[hyperkitty]
+raw_index = hyperkitty_raw
+enriched_index = hyperkitty_enriched
+```
+#### jenkins [&uarr;](#supported-data-sources-)
+Builds from a Jenkins
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "jenkins": [
+            "https://build.opnfv.org/ci"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[jenkins]
+raw_index = jenkins_raw
+enriched_index = jenkins_enriched
+no-archive = true (suggested)
+```
+#### jira [&uarr;](#supported-data-sources-)
+Issues data from JIRA issue trackers
+
+- projects.json
+```
+{
+    "Chaoss":{
+        "jira": [
+            "https://jira.opnfv.org"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[jira]
+raw_index = jira_raw
+enriched_index = jira_enriched
+no-archive = true (suggested)
+backend-user = yyyy (optional)
+backend-password = xxxx (optional)
+```
+#### kitsune [&uarr;](#supported-data-sources-)
+Questions and answers from KitSune
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "kitsune": [
+            ""
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[kitsune]
+raw_index = kitsune_raw
+enriched_index = kitsune_enriched
+```
+
+#### mattermost [&uarr;](#supported-data-sources-)
+Messages from Mattermost channels
+- projects.json
+```
+{
+    "Chaoss": {
+        "mattermost": [
+            "https://chat.openshift.io 8j366ft5affy3p36987pcugaoa"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[mattermost]
+raw_index = mattermost_raw
+enriched_index = mattermost_enriched
+api-token = xxxx
+studies = [enrich_demography:mattermost] (optional)
+
+[enrich_demography:mattermost] (optional)
+```
+#### mbox [&uarr;](#supported-data-sources-)
+Messages from MBox files
+
+For mbox files, it is needed the name of the mailing list and the path where the mboxes can be found. In the example
+below, the name of the mailing list is set to "mirageos-devel".
+- projects.json
+```
+{
+    "Chaoss": {
+        "mbox": [
+            "mirageos-devel /home/bitergia/mbox/mirageos-devel/"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[mbox]
+raw_index = mbox_raw
+enriched_index = mbox_enriched
+```
+#### mediawiki [&uarr;](#supported-data-sources-)
+Pages and revisions from MediaWiki
+
+-projects.json
+```
+{
+    "Chaoss": {
+        "mediawiki": [
+            "https://www.mediawiki.org/w https://www.mediawiki.org/wiki"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[mediawiki]
+raw_index = mediawiki_raw
+enriched_index = mediawiki_enriched
+no-archive = true (suggested)
+```
+#### meetup [&uarr;](#supported-data-sources-)
+Events from Meetup groups
+
+For meetup groups it is only needed the identifier of the meetup group
+and an API token: https://chaoss.github.io/grimoirelab-tutorial/gelk/meetup.html#gathering-meetup-groups-data
+- projects.json
+```
+{
+    "Chaoss": {
+        "meetup": [
+        "Alicante-Bitergia-Users-Group",
+        "South-East-Bitergia-User-Group"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[meetup]
+raw_index = meetup_raw
+enriched_index = meetup_enriched
+api-token = xxxx
+sleep-for-rate = true
+sleep-time = "300" (optional)
+no-archive = true (suggested)
+
+```
+#### mozillaclub [&uarr;](#supported-data-sources-)
+Events from Mozillaclub
+- projects.json
+```
+{
+    "Chaoss": {
+        "mozillaclub": [
+            "https://spreadsheets.google.com/feeds/cells/1QHl2bjBhMslyFzR5XXPzMLdzzx7oeSKTbgR5PM8qp64/ohaibtm/public/values?alt=json"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[mozillaclub]
+raw_index = mozillaclub_raw
+enriched_index = mozillaclub_enriched
+```
+#### nntp [&uarr;](#supported-data-sources-)
+Articles from NNTP newsgroups
+
+The way to setup netnews is adding the server and the news channel to be monitored. In the example below,
+the `news.myproject.org` is the server name.
+- projects.json
+```
+{
+    "Chaoss": {
+        "nntp": [
+            "news.myproject.org mozilla.dev.tech.crypto.checkins",
+            "news.myproject.org mozilla.dev.tech.electrolysis",
+            "news.myproject.org mozilla.dev.tech.gfx",
+            "news.myproject.org mozilla.dev.tech.java"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[nntp]
+raw_index = nntp_raw
+enriched_index =  nntp_enriched
+```
+#### pagure [&uarr;](#supported-data-sources-)
+Issues from Pagure repositories
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "pagure": [
+            "https://pagure.io/Test-group/Project-example-namespace"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[pagure]
+raw_index = pagure_raw
+enriched_index = pagure_enriched
+api-token = xxxx
+sleep-for-rate = true
+sleep-time = "300" (optional)
+no-archive = true (suggested)
+```
+#### phabricator [&uarr;](#supported-data-sources-)
+Tasks from Phabricator
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "phabricator": [
+            "https://phabricator.wikimedia.org"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[phabricator]
+raw_index = phabricator_raw
+enriched_index = phabricator_enriched
+api-token = xxxx
+no-archive = true (suggested)
+```
+#### pipermail [&uarr;](#supported-data-sources-)
+Messages from Pipermail
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "pipermail": [
+            "https://lists.linuxfoundation.org/pipermail/grimoirelab-discussions/"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[pipermail]
+raw_index = pipermail_raw
+enriched_index = pipermail_enriched
+```
+#### puppetforge [&uarr;](#supported-data-sources-)
+Modules and their releases from Puppet's forge
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "puppetforge": [
+            ""
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[puppetforge]
+raw_index = puppetforge_raw
+enriched_index = puppetforge_enriched
+```
+#### redmine [&uarr;](#supported-data-sources-)
+Issues from Redmine
+- project.json
+```
+{
+    "Chaoss": {
+        "redmine": [
+            "http://tracker.ceph.com/"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[redmine]
+raw_index = redmine_raw
+enriched_index = redmine_enriched
+api-token = XXXXX
+```
+#### remo [&uarr;](#supported-data-sources-)
+Events, people and activities from ReMo
+- project.json
+```
+{
+    "Chaoss": {
+        "remo": [
+            "https://reps.mozilla.org"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[remo]
+raw_index = remo_raw
+enriched_index = remo_enriched
+```
+#### rocketchat [&uarr;](#supported-data-sources-)
+Messages from Rocketchat channels
+- projects.json
+```
+{
+    "Chaoss": {
+        "rocketchat": [
+            "https://open.rocket.chat general"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[rocketchat]
+raw_index = rocketchat_raw
+enriched_index = rocketchat_enriched
+api-token = xxxx
+sleep-for-rate = true
+user-id = xxxx
+no-archive = true (suggested)
+```
+#### rss [&uarr;](#supported-data-sources-)
+Entries from RSS feeds
+
+- project.json
+```
+{
+    "Chaoss": {
+        "remo": [
+            "https://reps.mozilla.org"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[rss]
+raw_index = rss_raw
+enriched_index = rss_enriched
+```
+#### slack [&uarr;](#supported-data-sources-)
+Messages from Slack channels
+
+The information needed to monitor slack channels is the channel id.
+- projects.json
+```
+{
+    "Chaoss": {
+        "slack": [
+            "A195YQBLL",
+            "A495YQBM2"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[slack]
+raw_index = slack_raw
+enriched_index = slack_enriched
+api-token = xxxx
+no-archive = true (suggested)
+```
+#### stackexchange [&uarr;](#supported-data-sources-)
+Questions, answers and comments from StackExchange
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "stackexchange": [
+            "http://stackoverflow.com/questions/tagged/chef",
+            "http://stackoverflow.com/questions/tagged/chefcookbook",
+            "http://stackoverflow.com/questions/tagged/ohai",
+            "http://stackoverflow.com/questions/tagged/test-kitchen",
+            "http://stackoverflow.com/questions/tagged/knife"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[stackexchange]
+raw_index = stackexchange_raw
+enriched_index = stackexchange_enriched
+api-token = xxxx
+no-archive = true (suggested)
+```
+#### supybot [&uarr;](#supported-data-sources-)
+Messages from Supybot log files
+
+For supybot files, it is needed the name of the IRC channel and the path where the logs can be found. In the example
+below, the name of the channel is set to "irc://irc.freenode.net/atomic".
+- projects.json
+```
+{
+    "Chaoss": {
+        "supybot": [
+            "irc://irc.freenode.net/atomic /home/bitergia/irc/percevalbot/logs/ChannelLogger/freenode/#atomic"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[supybot]
+raw_index = supybot_raw
+enriched_index = supybot_enriched
+```
+
+#### telegram [&uarr;](#supported-data-sources-)
+Messages from Telegram
+
+You need to have an API token: https://github.com/chaoss/grimoirelab-perceval#telegram
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "telegram": [
+            "Mozilla_analytics"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[telegram]
+raw_index = telegram_raw
+enriched_index = telegram_enriched
+api-token = XXXXX
+```
+#### twitter [&uarr;](#supported-data-sources-)
+Messages from Twitter
+
+You need to provide a [search query](https://developer.twitter.com/en/docs/tweets/search/guides/build-standard-query) and an API token (which requires to create an [app](https://developer.twitter.com/en/docs/basics/apps/overview)). The script at https://gist.github.com/valeriocos/7d4d28f72f53fbce49f1512ba77ef5f6 helps obtaining a token.
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "twitter": [
+            "bitergia"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[twitter]
+raw_index = twitter_raw
+enriched_index = twitter_enriched
+api-token = XXXX
+```
+
+#### weblate [&uarr;](#supported-data-sources-)
+Changes from Weblate
+
+You need to have an API token: The token can be obtained after registering to a weblate
+instance (e.g., https://translations.documentfoundation.org/), via the page <instance>/accounts/profile/#api
+
+- projects.json
+```
+{
+    "Chaoss": {
+        "weblate": [
+            "https://translations.documentfoundation.org"
+        ]
+    }
+}
+```
+- setup.cfg
+```
+[weblate]
+raw_index = weblate_raw
+enriched_index = weblate_enriched
+api-token = XXXX
+no-archive = true (suggested)
+sleep-for-rate = true (suggested)
+studies = [enrich_demography:weblate] (optional)
+
+[enrich_demography:weblate] (optional)
+```
+
+## Micro Mordred [&uarr;](#contents)
+
+Micro Mordred is a simplified version of Mordred which omits the use of its scheduler. Thus, Micro Mordred allows running single Mordred tasks (e.g., raw collection, enrichment) per execution.
+
+Micro Mordred is located in the [sirmordred/utils](https://github.com/chaoss/grimoirelab-sirmordred/tree/master/sirmordred/utils/micro.py) folder of this same repository. It can be executed via command line, its parameters are summarized below:
+```
+--debug: execute Micro Mordred in debug mode
+
+--raw: activate raw task
+
+--enrich: activate enrich task
+
+--identities: activate merge identities task
+
+--panels: activate panels task
+
+--cfg: path of the configuration file
+
+--backends: list of cfg sections where the active tasks will be executed
+
+--logs-dir: single parameter denoting the path of folder in which logs are to be stored
+```
 
+Examples of possible executions are shown below:
+```
+cd .../grimoirelab-sirmordred/sirmordred/utils/
+micro.py --raw --enrich --cfg ./setup.cfg --backends git # execute the Raw and Enrich tasks for the Git cfg section
+micro.py --panels # execute the Panels task to load the Sigils panels to Kibiter
+micro.py --raw --enrich --debug --cfg ./setup.cfg --backends groupsio --logs-dir logs # execute the raw and enriched tasks for the groupsio cfg section with debug mode on and logs being saved in the folder logs in the same directory as micro.py
+```
 
-setup(**setup_kwargs)
```

