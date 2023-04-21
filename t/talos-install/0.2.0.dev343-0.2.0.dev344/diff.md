# Comparing `tmp/talos_install-0.2.0.dev343.tar.gz` & `tmp/talos_install-0.2.0.dev344.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talos_install-0.2.0.dev343.tar", last modified: Fri Apr 21 11:50:54 2023, max compression
+gzip compressed data, was "talos_install-0.2.0.dev344.tar", last modified: Fri Apr 21 12:03:26 2023, max compression
```

## Comparing `talos_install-0.2.0.dev343.tar` & `talos_install-0.2.0.dev344.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.839318 talos_install-0.2.0.dev343/
--rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-04-21 11:50:54.000000 talos_install-0.2.0.dev343/AUTHORS
--rw-rw-r--   0 installer  (3002) installer  (3002)    11364 2023-04-21 11:50:54.000000 talos_install-0.2.0.dev343/ChangeLog
--rw-rw-r--   0 installer  (3002) installer  (3002)     1960 2023-04-21 11:50:54.839318 talos_install-0.2.0.dev343/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     1300 2023-04-20 16:49:40.000000 talos_install-0.2.0.dev343/README.md
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.813318 talos_install-0.2.0.dev343/ansible/
--rw-rw-r--   0 installer  (3002) installer  (3002)      309 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/ansible.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.813318 talos_install-0.2.0.dev343/ansible/group_vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)       23 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/group_vars/all.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.810318 talos_install-0.2.0.dev343/ansible/roles/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.799318 talos_install-0.2.0.dev343/ansible/roles/cli/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.813318 talos_install-0.2.0.dev343/ansible/roles/cli/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev343/ansible/roles/cli/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.814318 talos_install-0.2.0.dev343/ansible/roles/cli/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      819 2023-04-18 16:24:47.000000 talos_install-0.2.0.dev343/ansible/roles/cli/tasks/clone.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1527 2023-04-19 08:23:48.000000 talos_install-0.2.0.dev343/ansible/roles/cli/tasks/env.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-04-17 07:40:14.000000 talos_install-0.2.0.dev343/ansible/roles/cli/tasks/logrotate.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      474 2023-04-17 07:40:14.000000 talos_install-0.2.0.dev343/ansible/roles/cli/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     2748 2023-04-19 14:54:32.000000 talos_install-0.2.0.dev343/ansible/roles/cli/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1488 2023-04-17 09:13:53.000000 talos_install-0.2.0.dev343/ansible/roles/cli/tasks/web.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.817318 talos_install-0.2.0.dev343/ansible/roles/cli/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3793 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev343/ansible/roles/cli/templates/agent.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      742 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev343/ansible/roles/cli/templates/app.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev343/ansible/roles/cli/templates/cli.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev343/ansible/roles/cli/templates/env_talos.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-04-19 14:05:02.000000 talos_install-0.2.0.dev343/ansible/roles/cli/templates/globals.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/cli/templates/my-httpd.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      351 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/cli/templates/passwords.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/cli/templates/talos-logrotate.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-04-16 16:14:02.000000 talos_install-0.2.0.dev343/ansible/roles/cli/templates/talos.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/cli/templates/talospass.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.800318 talos_install-0.2.0.dev343/ansible/roles/common/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.817318 talos_install-0.2.0.dev343/ansible/roles/common/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev343/ansible/roles/common/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.818318 talos_install-0.2.0.dev343/ansible/roles/common/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-04-20 16:08:13.000000 talos_install-0.2.0.dev343/ansible/roles/common/tasks/install_extra_pkgs.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-04-17 08:59:47.000000 talos_install-0.2.0.dev343/ansible/roles/common/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev343/ansible/roles/common/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.800318 talos_install-0.2.0.dev343/ansible/roles/gather_facts/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.818318 talos_install-0.2.0.dev343/ansible/roles/gather_facts/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-04-17 07:54:44.000000 talos_install-0.2.0.dev343/ansible/roles/gather_facts/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.818318 talos_install-0.2.0.dev343/ansible/roles/gather_facts/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      964 2023-04-19 08:35:48.000000 talos_install-0.2.0.dev343/ansible/roles/gather_facts/vars/RedHat.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      964 2023-04-17 07:30:11.000000 talos_install-0.2.0.dev343/ansible/roles/gather_facts/vars/Rocky.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.801318 talos_install-0.2.0.dev343/ansible/roles/install_ansible/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.801318 talos_install-0.2.0.dev343/ansible/roles/install_ansible/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.819318 talos_install-0.2.0.dev343/ansible/roles/install_ansible/files/inventory_plugins/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.819318 talos_install-0.2.0.dev343/ansible/roles/install_ansible/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev343/ansible/roles/install_ansible/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.819318 talos_install-0.2.0.dev343/ansible/roles/install_ansible/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      389 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev343/ansible/roles/install_ansible/tasks/install_ansible_collection.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1263 2023-04-19 14:57:18.000000 talos_install-0.2.0.dev343/ansible/roles/install_ansible/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.819318 talos_install-0.2.0.dev343/ansible/roles/install_ansible/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      718 2023-04-16 13:01:28.000000 talos_install-0.2.0.dev343/ansible/roles/install_ansible/templates/ansible.cfg.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.802318 talos_install-0.2.0.dev343/ansible/roles/install_certificates/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.820318 talos_install-0.2.0.dev343/ansible/roles/install_certificates/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev343/ansible/roles/install_certificates/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.820318 talos_install-0.2.0.dev343/ansible/roles/install_certificates/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-04-19 14:04:55.000000 talos_install-0.2.0.dev343/ansible/roles/install_certificates/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.802318 talos_install-0.2.0.dev343/ansible/roles/install_docker/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.820318 talos_install-0.2.0.dev343/ansible/roles/install_docker/handlers/
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-17 07:42:54.000000 talos_install-0.2.0.dev343/ansible/roles/install_docker/handlers/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.820318 talos_install-0.2.0.dev343/ansible/roles/install_docker/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev343/ansible/roles/install_docker/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.821318 talos_install-0.2.0.dev343/ansible/roles/install_docker/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1085 2023-04-20 12:42:13.000000 talos_install-0.2.0.dev343/ansible/roles/install_docker/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      626 2023-04-17 14:19:59.000000 talos_install-0.2.0.dev343/ansible/roles/install_docker/tasks/upstream.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.821318 talos_install-0.2.0.dev343/ansible/roles/install_docker/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/install_docker/templates/daemon.json.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/install_docker/templates/docker-ce.repo.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.803318 talos_install-0.2.0.dev343/ansible/roles/install_python/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.822318 talos_install-0.2.0.dev343/ansible/roles/install_python/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      440 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev343/ansible/roles/install_python/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.822318 talos_install-0.2.0.dev343/ansible/roles/install_python/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/install_python/vars/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.807318 talos_install-0.2.0.dev343/ansible/roles/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.822318 talos_install-0.2.0.dev343/ansible/roles/nagios/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-04-19 14:27:39.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.804318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.803318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.822318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/etc/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.822318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/etc/nagios/conf.d/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.823318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/etc/nagios/monitor/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/etc/nagios/monitor/.ID
--rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-04-17 14:32:36.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/etc/nagios/resource.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.806318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.823318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.804318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/apache2/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.823318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.805318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.823318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/apache/
--rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/apache/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.824318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/nagios/
--rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.824318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/postfix/
--rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.824318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
--rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.806318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.805318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.824318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.825318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.825318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
--rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1573 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
--rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.826318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.826318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
--rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
--rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.806318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.827318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.806318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/usr/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.806318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/usr/local/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.827318 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/usr/local/bin/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.828318 talos_install-0.2.0.dev343/ansible/roles/nagios/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-04-20 16:16:42.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.829318 talos_install-0.2.0.dev343/ansible/roles/nagios/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/templates/cgi.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/templates/contacts.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3642 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/templates/localhost.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/nagios/templates/nagios.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.809318 talos_install-0.2.0.dev343/ansible/roles/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.829318 talos_install-0.2.0.dev343/ansible/roles/opendcim/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.831318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/apache2.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/apache2.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-04-20 12:27:23.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/default.sql
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.807318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.808318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/etc/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.831318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/etc/opendcim/drawings/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.831318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/etc/opendcim/pictures/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/mysqld.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.808318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.808318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.808318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.831318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.832318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
--rw-rw-r--   0 installer  (3002) installer  (3002)    53192 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
--rw-rw-r--   0 installer  (3002) installer  (3002)    20091 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.832318 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-04-20 13:50:07.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/pre-conf.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-04-20 15:35:00.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/files/startup.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.832318 talos_install-0.2.0.dev343/ansible/roles/opendcim/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.833318 talos_install-0.2.0.dev343/ansible/roles/opendcim/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.834318 talos_install-0.2.0.dev343/ansible/roles/opendcim/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-04-20 13:12:20.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-04-20 09:06:15.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/templates/first-run.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/opendcim/templates/opendcim.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.809318 talos_install-0.2.0.dev343/ansible/roles/os_tune/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.834318 talos_install-0.2.0.dev343/ansible/roles/os_tune/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1305 2023-04-21 11:49:37.000000 talos_install-0.2.0.dev343/ansible/roles/os_tune/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.810318 talos_install-0.2.0.dev343/ansible/roles/talos_users/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.835318 talos_install-0.2.0.dev343/ansible/roles/talos_users/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/talos_users/files/talos
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.835318 talos_install-0.2.0.dev343/ansible/roles/talos_users/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev343/ansible/roles/talos_users/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.835318 talos_install-0.2.0.dev343/ansible/roles/talos_users/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      659 2023-04-17 07:48:59.000000 talos_install-0.2.0.dev343/ansible/roles/talos_users/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.835318 talos_install-0.2.0.dev343/ansible/roles/wiki/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.835318 talos_install-0.2.0.dev343/ansible/roles/wiki/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      536 2023-04-17 07:46:15.000000 talos_install-0.2.0.dev343/ansible/roles/wiki/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.836318 talos_install-0.2.0.dev343/ansible/roles/wiki/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev343/ansible/roles/wiki/meta/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/wiki/requirements.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.836318 talos_install-0.2.0.dev343/ansible/roles/wiki/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-04-17 09:16:59.000000 talos_install-0.2.0.dev343/ansible/roles/wiki/tasks/compose.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      222 2023-04-17 07:47:31.000000 talos_install-0.2.0.dev343/ansible/roles/wiki/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-04-17 07:36:52.000000 talos_install-0.2.0.dev343/ansible/roles/wiki/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.837318 talos_install-0.2.0.dev343/ansible/roles/wiki/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1153 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev343/ansible/roles/wiki/templates/docker-compose.yml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/wiki/templates/wiki.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev343/ansible/roles/wiki/templates/wikidump.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1588 2023-04-19 08:30:31.000000 talos_install-0.2.0.dev343/ansible/site.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.838318 talos_install-0.2.0.dev343/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      570 2023-04-19 13:42:43.000000 talos_install-0.2.0.dev343/etc/globals.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev343/etc/inventory
--rw-rw-r--   0 installer  (3002) installer  (3002)     1625 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev343/etc/talos.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1068 2023-04-21 11:50:54.850318 talos_install-0.2.0.dev343/setup.cfg
--rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-04-20 16:36:43.000000 talos_install-0.2.0.dev343/setup.py
--rwxrwxr-x   0 installer  (3002) installer  (3002)     5797 2023-04-21 11:27:29.000000 talos_install-0.2.0.dev343/talos_install
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 11:50:54.839318 talos_install-0.2.0.dev343/talos_install.egg-info/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1960 2023-04-21 11:50:54.000000 talos_install-0.2.0.dev343/talos_install.egg-info/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     5419 2023-04-21 11:50:54.000000 talos_install-0.2.0.dev343/talos_install.egg-info/SOURCES.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-21 11:50:54.000000 talos_install-0.2.0.dev343/talos_install.egg-info/dependency_links.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-20 13:58:32.000000 talos_install-0.2.0.dev343/talos_install.egg-info/not-zip-safe
--rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-04-21 11:50:54.000000 talos_install-0.2.0.dev343/talos_install.egg-info/pbr.json
--rw-rw-r--   0 installer  (3002) installer  (3002)      109 2023-04-21 11:50:54.000000 talos_install-0.2.0.dev343/talos_install.egg-info/requires.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-21 11:50:54.000000 talos_install-0.2.0.dev343/talos_install.egg-info/top_level.txt
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.073715 talos_install-0.2.0.dev344/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-04-21 12:03:25.000000 talos_install-0.2.0.dev344/AUTHORS
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11388 2023-04-21 12:03:25.000000 talos_install-0.2.0.dev344/ChangeLog
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1960 2023-04-21 12:03:26.073715 talos_install-0.2.0.dev344/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1300 2023-04-20 16:49:40.000000 talos_install-0.2.0.dev344/README.md
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.050715 talos_install-0.2.0.dev344/ansible/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      309 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/ansible.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.051715 talos_install-0.2.0.dev344/ansible/group_vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       23 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/group_vars/all.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.048714 talos_install-0.2.0.dev344/ansible/roles/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.038715 talos_install-0.2.0.dev344/ansible/roles/cli/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.051715 talos_install-0.2.0.dev344/ansible/roles/cli/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev344/ansible/roles/cli/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.052715 talos_install-0.2.0.dev344/ansible/roles/cli/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      819 2023-04-18 16:24:47.000000 talos_install-0.2.0.dev344/ansible/roles/cli/tasks/clone.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1527 2023-04-19 08:23:48.000000 talos_install-0.2.0.dev344/ansible/roles/cli/tasks/env.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-04-17 07:40:14.000000 talos_install-0.2.0.dev344/ansible/roles/cli/tasks/logrotate.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      474 2023-04-17 07:40:14.000000 talos_install-0.2.0.dev344/ansible/roles/cli/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2748 2023-04-19 14:54:32.000000 talos_install-0.2.0.dev344/ansible/roles/cli/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1488 2023-04-17 09:13:53.000000 talos_install-0.2.0.dev344/ansible/roles/cli/tasks/web.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.054715 talos_install-0.2.0.dev344/ansible/roles/cli/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3793 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev344/ansible/roles/cli/templates/agent.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      742 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev344/ansible/roles/cli/templates/app.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev344/ansible/roles/cli/templates/cli.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev344/ansible/roles/cli/templates/env_talos.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-04-19 14:05:02.000000 talos_install-0.2.0.dev344/ansible/roles/cli/templates/globals.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/cli/templates/my-httpd.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      351 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/cli/templates/passwords.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/cli/templates/talos-logrotate.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-04-16 16:14:02.000000 talos_install-0.2.0.dev344/ansible/roles/cli/templates/talos.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/cli/templates/talospass.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.038715 talos_install-0.2.0.dev344/ansible/roles/common/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.054715 talos_install-0.2.0.dev344/ansible/roles/common/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev344/ansible/roles/common/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.055715 talos_install-0.2.0.dev344/ansible/roles/common/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-04-20 16:08:13.000000 talos_install-0.2.0.dev344/ansible/roles/common/tasks/install_extra_pkgs.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-04-17 08:59:47.000000 talos_install-0.2.0.dev344/ansible/roles/common/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev344/ansible/roles/common/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.039715 talos_install-0.2.0.dev344/ansible/roles/gather_facts/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.055715 talos_install-0.2.0.dev344/ansible/roles/gather_facts/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-04-17 07:54:44.000000 talos_install-0.2.0.dev344/ansible/roles/gather_facts/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.055715 talos_install-0.2.0.dev344/ansible/roles/gather_facts/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      964 2023-04-19 08:35:48.000000 talos_install-0.2.0.dev344/ansible/roles/gather_facts/vars/RedHat.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      964 2023-04-17 07:30:11.000000 talos_install-0.2.0.dev344/ansible/roles/gather_facts/vars/Rocky.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.040715 talos_install-0.2.0.dev344/ansible/roles/install_ansible/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.039715 talos_install-0.2.0.dev344/ansible/roles/install_ansible/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.055715 talos_install-0.2.0.dev344/ansible/roles/install_ansible/files/inventory_plugins/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.055715 talos_install-0.2.0.dev344/ansible/roles/install_ansible/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev344/ansible/roles/install_ansible/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.056715 talos_install-0.2.0.dev344/ansible/roles/install_ansible/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      389 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev344/ansible/roles/install_ansible/tasks/install_ansible_collection.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1263 2023-04-19 14:57:18.000000 talos_install-0.2.0.dev344/ansible/roles/install_ansible/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.056715 talos_install-0.2.0.dev344/ansible/roles/install_ansible/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      718 2023-04-16 13:01:28.000000 talos_install-0.2.0.dev344/ansible/roles/install_ansible/templates/ansible.cfg.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.040715 talos_install-0.2.0.dev344/ansible/roles/install_certificates/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.056715 talos_install-0.2.0.dev344/ansible/roles/install_certificates/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev344/ansible/roles/install_certificates/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.056715 talos_install-0.2.0.dev344/ansible/roles/install_certificates/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-04-19 14:04:55.000000 talos_install-0.2.0.dev344/ansible/roles/install_certificates/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.041715 talos_install-0.2.0.dev344/ansible/roles/install_docker/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.057715 talos_install-0.2.0.dev344/ansible/roles/install_docker/handlers/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-17 07:42:54.000000 talos_install-0.2.0.dev344/ansible/roles/install_docker/handlers/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.057715 talos_install-0.2.0.dev344/ansible/roles/install_docker/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev344/ansible/roles/install_docker/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.057715 talos_install-0.2.0.dev344/ansible/roles/install_docker/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1085 2023-04-20 12:42:13.000000 talos_install-0.2.0.dev344/ansible/roles/install_docker/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      626 2023-04-17 14:19:59.000000 talos_install-0.2.0.dev344/ansible/roles/install_docker/tasks/upstream.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.058715 talos_install-0.2.0.dev344/ansible/roles/install_docker/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/install_docker/templates/daemon.json.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/install_docker/templates/docker-ce.repo.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.041715 talos_install-0.2.0.dev344/ansible/roles/install_python/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.058715 talos_install-0.2.0.dev344/ansible/roles/install_python/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      440 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev344/ansible/roles/install_python/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.058715 talos_install-0.2.0.dev344/ansible/roles/install_python/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/install_python/vars/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.045715 talos_install-0.2.0.dev344/ansible/roles/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.058715 talos_install-0.2.0.dev344/ansible/roles/nagios/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-04-19 14:27:39.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.042715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.042715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.058715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/etc/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.059715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/etc/nagios/conf.d/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.059715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/etc/nagios/monitor/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/etc/nagios/monitor/.ID
+-rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-04-17 14:32:36.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/etc/nagios/resource.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.044715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.059715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.042715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/apache2/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.059715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.043715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.059715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/apache/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/apache/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.060715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/nagios/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.060715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/postfix/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.060715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.044715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.044715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.060715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.061715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.061715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1573 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.062715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.062715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
+-rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.044715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.062715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.045715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/usr/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.045715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/usr/local/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.062715 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/usr/local/bin/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.063715 talos_install-0.2.0.dev344/ansible/roles/nagios/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-04-20 16:16:42.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.064715 talos_install-0.2.0.dev344/ansible/roles/nagios/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/templates/cgi.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/templates/contacts.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3642 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/templates/localhost.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/nagios/templates/nagios.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.047715 talos_install-0.2.0.dev344/ansible/roles/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.065715 talos_install-0.2.0.dev344/ansible/roles/opendcim/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.066715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/apache2.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/apache2.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-04-20 12:27:23.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/default.sql
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.046715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.046715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/etc/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.066715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/etc/opendcim/drawings/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.066715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/etc/opendcim/pictures/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/mysqld.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.046715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.046715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.046715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.066715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.067715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    53192 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)    20091 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.067715 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-04-20 13:50:07.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/pre-conf.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-04-20 15:35:00.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/files/startup.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.067715 talos_install-0.2.0.dev344/ansible/roles/opendcim/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.068715 talos_install-0.2.0.dev344/ansible/roles/opendcim/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.069715 talos_install-0.2.0.dev344/ansible/roles/opendcim/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-04-20 13:12:20.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-04-20 09:06:15.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/templates/first-run.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/opendcim/templates/opendcim.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.047715 talos_install-0.2.0.dev344/ansible/roles/os_tune/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.069715 talos_install-0.2.0.dev344/ansible/roles/os_tune/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1281 2023-04-21 12:02:42.000000 talos_install-0.2.0.dev344/ansible/roles/os_tune/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.048714 talos_install-0.2.0.dev344/ansible/roles/talos_users/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.069715 talos_install-0.2.0.dev344/ansible/roles/talos_users/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/talos_users/files/talos
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.069715 talos_install-0.2.0.dev344/ansible/roles/talos_users/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev344/ansible/roles/talos_users/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.069715 talos_install-0.2.0.dev344/ansible/roles/talos_users/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      659 2023-04-17 07:48:59.000000 talos_install-0.2.0.dev344/ansible/roles/talos_users/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.070715 talos_install-0.2.0.dev344/ansible/roles/wiki/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.070715 talos_install-0.2.0.dev344/ansible/roles/wiki/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      536 2023-04-17 07:46:15.000000 talos_install-0.2.0.dev344/ansible/roles/wiki/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.070715 talos_install-0.2.0.dev344/ansible/roles/wiki/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev344/ansible/roles/wiki/meta/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/wiki/requirements.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.071714 talos_install-0.2.0.dev344/ansible/roles/wiki/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-04-17 09:16:59.000000 talos_install-0.2.0.dev344/ansible/roles/wiki/tasks/compose.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      222 2023-04-17 07:47:31.000000 talos_install-0.2.0.dev344/ansible/roles/wiki/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-04-17 07:36:52.000000 talos_install-0.2.0.dev344/ansible/roles/wiki/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.071714 talos_install-0.2.0.dev344/ansible/roles/wiki/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1153 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev344/ansible/roles/wiki/templates/docker-compose.yml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/wiki/templates/wiki.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev344/ansible/roles/wiki/templates/wikidump.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1588 2023-04-19 08:30:31.000000 talos_install-0.2.0.dev344/ansible/site.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.072715 talos_install-0.2.0.dev344/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      570 2023-04-19 13:42:43.000000 talos_install-0.2.0.dev344/etc/globals.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev344/etc/inventory
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1625 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev344/etc/talos.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1068 2023-04-21 12:03:26.084715 talos_install-0.2.0.dev344/setup.cfg
+-rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-04-20 16:36:43.000000 talos_install-0.2.0.dev344/setup.py
+-rwxrwxr-x   0 installer  (3002) installer  (3002)     5797 2023-04-21 11:27:29.000000 talos_install-0.2.0.dev344/talos_install
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 12:03:26.073715 talos_install-0.2.0.dev344/talos_install.egg-info/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1960 2023-04-21 12:03:25.000000 talos_install-0.2.0.dev344/talos_install.egg-info/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5419 2023-04-21 12:03:26.000000 talos_install-0.2.0.dev344/talos_install.egg-info/SOURCES.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-21 12:03:25.000000 talos_install-0.2.0.dev344/talos_install.egg-info/dependency_links.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-20 13:58:32.000000 talos_install-0.2.0.dev344/talos_install.egg-info/not-zip-safe
+-rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-04-21 12:03:26.000000 talos_install-0.2.0.dev344/talos_install.egg-info/pbr.json
+-rw-rw-r--   0 installer  (3002) installer  (3002)      109 2023-04-21 12:03:25.000000 talos_install-0.2.0.dev344/talos_install.egg-info/requires.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-21 12:03:25.000000 talos_install-0.2.0.dev344/talos_install.egg-info/top_level.txt
```

### Comparing `talos_install-0.2.0.dev343/ChangeLog` & `talos_install-0.2.0.dev344/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGES
 =======
 
 * fix service not found
+* fix service not found
 * Add Reboot notice on bootstrap run
 * mini fix
 * add pip description
 * add pip description
 * Fix opendcim Docker
 *  Fix OpenDCIM docker
 *  Fix OpenDCIM docker
```

### Comparing `talos_install-0.2.0.dev343/PKG-INFO` & `talos_install-0.2.0.dev344/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos_install
-Version: 0.2.0.dev343
+Version: 0.2.0.dev344
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `talos_install-0.2.0.dev343/README.md` & `talos_install-0.2.0.dev344/README.md`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/tasks/clone.yaml` & `talos_install-0.2.0.dev344/ansible/roles/cli/tasks/clone.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/tasks/env.yaml` & `talos_install-0.2.0.dev344/ansible/roles/cli/tasks/env.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/tasks/misc.yaml` & `talos_install-0.2.0.dev344/ansible/roles/cli/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/tasks/web.yaml` & `talos_install-0.2.0.dev344/ansible/roles/cli/tasks/web.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/templates/agent.sh.j2` & `talos_install-0.2.0.dev344/ansible/roles/cli/templates/agent.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/templates/app.yaml.j2` & `talos_install-0.2.0.dev344/ansible/roles/cli/templates/app.yaml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/templates/cli.conf.j2` & `talos_install-0.2.0.dev344/ansible/roles/cli/templates/cli.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/templates/env_talos.j2` & `talos_install-0.2.0.dev344/ansible/roles/cli/templates/env_talos.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/templates/globals.yaml.j2` & `talos_install-0.2.0.dev344/ansible/roles/cli/templates/globals.yaml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/templates/my-httpd.conf.j2` & `talos_install-0.2.0.dev344/ansible/roles/cli/templates/my-httpd.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/cli/templates/talos.conf.j2` & `talos_install-0.2.0.dev344/ansible/roles/cli/templates/talos.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/common/tasks/misc.yaml` & `talos_install-0.2.0.dev344/ansible/roles/common/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/gather_facts/vars/RedHat.yaml` & `talos_install-0.2.0.dev344/ansible/roles/gather_facts/vars/RedHat.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/gather_facts/vars/Rocky.yaml` & `talos_install-0.2.0.dev344/ansible/roles/gather_facts/vars/Rocky.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py` & `talos_install-0.2.0.dev344/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/install_ansible/tasks/main.yaml` & `talos_install-0.2.0.dev344/ansible/roles/install_ansible/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/install_ansible/templates/ansible.cfg.j2` & `talos_install-0.2.0.dev344/ansible/roles/install_ansible/templates/ansible.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/install_certificates/tasks/main.yaml` & `talos_install-0.2.0.dev344/ansible/roles/install_certificates/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/install_docker/tasks/main.yaml` & `talos_install-0.2.0.dev344/ansible/roles/install_docker/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/install_docker/tasks/upstream.yaml` & `talos_install-0.2.0.dev344/ansible/roles/install_docker/tasks/upstream.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/install_docker/templates/docker-ce.repo.j2` & `talos_install-0.2.0.dev344/ansible/roles/install_docker/templates/docker-ce.repo.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/nagios/run` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/nagios/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/etc/sv/postfix/run` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/etc/sv/postfix/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios` & `talos_install-0.2.0.dev344/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/tasks/build.yaml` & `talos_install-0.2.0.dev344/ansible/roles/nagios/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/tasks/misc.yaml` & `talos_install-0.2.0.dev344/ansible/roles/nagios/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/tasks/run.yaml` & `talos_install-0.2.0.dev344/ansible/roles/nagios/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/templates/Dockerfile.j2` & `talos_install-0.2.0.dev344/ansible/roles/nagios/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/templates/cgi.cfg.j2` & `talos_install-0.2.0.dev344/ansible/roles/nagios/templates/cgi.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/templates/contacts.cfg.j2` & `talos_install-0.2.0.dev344/ansible/roles/nagios/templates/contacts.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/nagios/templates/localhost.cfg.j2` & `talos_install-0.2.0.dev344/ansible/roles/nagios/templates/localhost.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/files/apache2.conf` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/files/apache2.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/files/default.sql` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/files/default.sql`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/files/pre-conf.sh` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/files/pre-conf.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/files/startup.sh` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/files/startup.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/tasks/build.yaml` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/tasks/misc.yaml` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/tasks/run.yaml` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/templates/Dockerfile.j2` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/opendcim/templates/first-run.sh.j2` & `talos_install-0.2.0.dev344/ansible/roles/opendcim/templates/first-run.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/os_tune/tasks/main.yaml` & `talos_install-0.2.0.dev344/ansible/roles/os_tune/tasks/main.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,31 @@
     use: systemd
 
 - name: Stop Firewall
   ansible.builtin.service:
     name: firewalld
     enabled: false
     state: stopped
-  failed_when: "stop_disabled_services | failed and 'could not be found' not in stop_disabled_services.msg"
-  register: stop_disabled_services
+  register: results
+  failed_when: >-
+    results is failed and
+    "Could not find the requested service" not in results.msg|default('')
 
 - name: Set timezone
   community.general.timezone:
     name: "{{ customer.timezone }}"
 
 - name: Disabling SELinux
   ansible.posix.selinux:
     state: disabled
   register: selinuxdisabled
 
 - name: System will be rebooted for Selinux Changes
   ansible.builtin.pause:
-    prompt: "!!!! System will reboot in 10 seconds. CTRL-C to cancel !!!!"
+    prompt: "!!! System will reboot in 10 seconds. !!!"
     seconds: 10
   when: selinuxdisabled is changed
 
 - name: Wait for 5 Second and Reboot
   ansible.builtin.reboot:
   when: selinuxdisabled is changed
```

### Comparing `talos_install-0.2.0.dev343/ansible/roles/talos_users/tasks/main.yaml` & `talos_install-0.2.0.dev344/ansible/roles/talos_users/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/wiki/defaults/main.yaml` & `talos_install-0.2.0.dev344/ansible/roles/wiki/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/wiki/tasks/compose.yaml` & `talos_install-0.2.0.dev344/ansible/roles/wiki/tasks/compose.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/roles/wiki/templates/docker-compose.yml.j2` & `talos_install-0.2.0.dev344/ansible/roles/wiki/templates/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/ansible/site.yaml` & `talos_install-0.2.0.dev344/ansible/site.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/etc/globals.yaml` & `talos_install-0.2.0.dev344/etc/globals.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/etc/talos.yaml` & `talos_install-0.2.0.dev344/etc/talos.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/setup.cfg` & `talos_install-0.2.0.dev344/setup.cfg`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/talos_install` & `talos_install-0.2.0.dev344/talos_install`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev343/talos_install.egg-info/PKG-INFO` & `talos_install-0.2.0.dev344/talos_install.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos-install
-Version: 0.2.0.dev343
+Version: 0.2.0.dev344
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `talos_install-0.2.0.dev343/talos_install.egg-info/SOURCES.txt` & `talos_install-0.2.0.dev344/talos_install.egg-info/SOURCES.txt`

 * *Files identical despite different names*

