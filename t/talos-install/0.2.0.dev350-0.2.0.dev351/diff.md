# Comparing `tmp/talos_install-0.2.0.dev350.tar.gz` & `tmp/talos_install-0.2.0.dev351.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talos_install-0.2.0.dev350.tar", last modified: Fri Apr 21 16:15:48 2023, max compression
+gzip compressed data, was "talos_install-0.2.0.dev351.tar", last modified: Fri Apr 21 16:40:19 2023, max compression
```

## Comparing `talos_install-0.2.0.dev350.tar` & `talos_install-0.2.0.dev351.tar`

### file list

```diff
@@ -1,214 +1,216 @@
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.129928 talos_install-0.2.0.dev350/
--rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-04-21 16:15:48.000000 talos_install-0.2.0.dev350/AUTHORS
--rw-rw-r--   0 installer  (3002) installer  (3002)    11598 2023-04-21 16:15:48.000000 talos_install-0.2.0.dev350/ChangeLog
--rw-rw-r--   0 installer  (3002) installer  (3002)     1960 2023-04-21 16:15:48.129928 talos_install-0.2.0.dev350/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     1300 2023-04-20 16:49:40.000000 talos_install-0.2.0.dev350/README.md
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.103928 talos_install-0.2.0.dev350/ansible/
--rw-rw-r--   0 installer  (3002) installer  (3002)      309 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/ansible.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.103928 talos_install-0.2.0.dev350/ansible/group_vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)       23 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/group_vars/all.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.100928 talos_install-0.2.0.dev350/ansible/roles/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.089928 talos_install-0.2.0.dev350/ansible/roles/cli/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.103928 talos_install-0.2.0.dev350/ansible/roles/cli/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev350/ansible/roles/cli/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.104928 talos_install-0.2.0.dev350/ansible/roles/cli/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      869 2023-04-21 14:29:00.000000 talos_install-0.2.0.dev350/ansible/roles/cli/tasks/clone.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1527 2023-04-19 08:23:48.000000 talos_install-0.2.0.dev350/ansible/roles/cli/tasks/env.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-04-17 07:40:14.000000 talos_install-0.2.0.dev350/ansible/roles/cli/tasks/logrotate.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      401 2023-04-21 14:29:02.000000 talos_install-0.2.0.dev350/ansible/roles/cli/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     2748 2023-04-19 14:54:32.000000 talos_install-0.2.0.dev350/ansible/roles/cli/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1488 2023-04-17 09:13:53.000000 talos_install-0.2.0.dev350/ansible/roles/cli/tasks/web.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.107928 talos_install-0.2.0.dev350/ansible/roles/cli/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3793 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev350/ansible/roles/cli/templates/agent.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      742 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev350/ansible/roles/cli/templates/app.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev350/ansible/roles/cli/templates/cli.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev350/ansible/roles/cli/templates/env_talos.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-04-19 14:05:02.000000 talos_install-0.2.0.dev350/ansible/roles/cli/templates/globals.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/cli/templates/my-httpd.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      351 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/cli/templates/passwords.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/cli/templates/talos-logrotate.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-04-16 16:14:02.000000 talos_install-0.2.0.dev350/ansible/roles/cli/templates/talos.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/cli/templates/talospass.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.090928 talos_install-0.2.0.dev350/ansible/roles/common/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.107928 talos_install-0.2.0.dev350/ansible/roles/common/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev350/ansible/roles/common/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.108928 talos_install-0.2.0.dev350/ansible/roles/common/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-04-20 16:08:13.000000 talos_install-0.2.0.dev350/ansible/roles/common/tasks/install_extra_pkgs.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-04-17 08:59:47.000000 talos_install-0.2.0.dev350/ansible/roles/common/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev350/ansible/roles/common/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.090928 talos_install-0.2.0.dev350/ansible/roles/gather_facts/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.108928 talos_install-0.2.0.dev350/ansible/roles/gather_facts/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-04-17 07:54:44.000000 talos_install-0.2.0.dev350/ansible/roles/gather_facts/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.108928 talos_install-0.2.0.dev350/ansible/roles/gather_facts/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      964 2023-04-19 08:35:48.000000 talos_install-0.2.0.dev350/ansible/roles/gather_facts/vars/RedHat.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      964 2023-04-17 07:30:11.000000 talos_install-0.2.0.dev350/ansible/roles/gather_facts/vars/Rocky.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.091928 talos_install-0.2.0.dev350/ansible/roles/install_ansible/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.091928 talos_install-0.2.0.dev350/ansible/roles/install_ansible/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.108928 talos_install-0.2.0.dev350/ansible/roles/install_ansible/files/inventory_plugins/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.109928 talos_install-0.2.0.dev350/ansible/roles/install_ansible/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev350/ansible/roles/install_ansible/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.109928 talos_install-0.2.0.dev350/ansible/roles/install_ansible/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      389 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev350/ansible/roles/install_ansible/tasks/install_ansible_collection.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1563 2023-04-21 15:41:33.000000 talos_install-0.2.0.dev350/ansible/roles/install_ansible/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.109928 talos_install-0.2.0.dev350/ansible/roles/install_ansible/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      718 2023-04-16 13:01:28.000000 talos_install-0.2.0.dev350/ansible/roles/install_ansible/templates/ansible.cfg.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.091928 talos_install-0.2.0.dev350/ansible/roles/install_certificates/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.110928 talos_install-0.2.0.dev350/ansible/roles/install_certificates/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev350/ansible/roles/install_certificates/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.110928 talos_install-0.2.0.dev350/ansible/roles/install_certificates/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-04-19 14:04:55.000000 talos_install-0.2.0.dev350/ansible/roles/install_certificates/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.092929 talos_install-0.2.0.dev350/ansible/roles/install_docker/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.110928 talos_install-0.2.0.dev350/ansible/roles/install_docker/handlers/
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-17 07:42:54.000000 talos_install-0.2.0.dev350/ansible/roles/install_docker/handlers/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.110928 talos_install-0.2.0.dev350/ansible/roles/install_docker/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev350/ansible/roles/install_docker/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.111928 talos_install-0.2.0.dev350/ansible/roles/install_docker/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1085 2023-04-20 12:42:13.000000 talos_install-0.2.0.dev350/ansible/roles/install_docker/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      626 2023-04-17 14:19:59.000000 talos_install-0.2.0.dev350/ansible/roles/install_docker/tasks/upstream.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.111928 talos_install-0.2.0.dev350/ansible/roles/install_docker/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/install_docker/templates/daemon.json.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/install_docker/templates/docker-ce.repo.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.093928 talos_install-0.2.0.dev350/ansible/roles/install_python/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.111928 talos_install-0.2.0.dev350/ansible/roles/install_python/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      440 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev350/ansible/roles/install_python/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.112928 talos_install-0.2.0.dev350/ansible/roles/install_python/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/install_python/vars/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.097928 talos_install-0.2.0.dev350/ansible/roles/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.112928 talos_install-0.2.0.dev350/ansible/roles/nagios/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-04-19 14:27:39.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.094928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.093928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.112928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/etc/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.112928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/etc/nagios/conf.d/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.112928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/etc/nagios/monitor/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/etc/nagios/monitor/.ID
--rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-04-17 14:32:36.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/etc/nagios/resource.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.096928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.113928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.094928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/apache2/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.113928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.095928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.113928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/apache/
--rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/apache/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.113928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/nagios/
--rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.114928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/postfix/
--rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.114928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
--rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.096928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.095928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.114928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.115929 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.115929 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
--rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1573 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
--rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.116928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.116928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
--rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
--rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.096928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.116928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.096928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/usr/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.096928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/usr/local/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.116928 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/usr/local/bin/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.117928 talos_install-0.2.0.dev350/ansible/roles/nagios/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-04-20 16:16:42.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.119928 talos_install-0.2.0.dev350/ansible/roles/nagios/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/templates/cgi.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/templates/contacts.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3642 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/templates/localhost.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/nagios/templates/nagios.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.099928 talos_install-0.2.0.dev350/ansible/roles/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.119928 talos_install-0.2.0.dev350/ansible/roles/opendcim/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.120928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/apache2.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/apache2.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-04-20 12:27:23.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/default.sql
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.097928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.098928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/etc/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.120928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/etc/opendcim/drawings/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.121928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/etc/opendcim/pictures/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/mysqld.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.098928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.098928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.098928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.121928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.121928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
--rw-rw-r--   0 installer  (3002) installer  (3002)    53192 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
--rw-rw-r--   0 installer  (3002) installer  (3002)    20091 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.122928 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-04-20 13:50:07.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/pre-conf.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-04-20 15:35:00.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/files/startup.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.122928 talos_install-0.2.0.dev350/ansible/roles/opendcim/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.123928 talos_install-0.2.0.dev350/ansible/roles/opendcim/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.123928 talos_install-0.2.0.dev350/ansible/roles/opendcim/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-04-20 13:12:20.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-04-20 09:06:15.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/templates/first-run.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/opendcim/templates/opendcim.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.099928 talos_install-0.2.0.dev350/ansible/roles/os_tune/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.124928 talos_install-0.2.0.dev350/ansible/roles/os_tune/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1281 2023-04-21 12:02:42.000000 talos_install-0.2.0.dev350/ansible/roles/os_tune/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.100928 talos_install-0.2.0.dev350/ansible/roles/talos_users/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.124928 talos_install-0.2.0.dev350/ansible/roles/talos_users/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/talos_users/files/talos
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.124928 talos_install-0.2.0.dev350/ansible/roles/talos_users/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev350/ansible/roles/talos_users/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.124928 talos_install-0.2.0.dev350/ansible/roles/talos_users/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      659 2023-04-17 07:48:59.000000 talos_install-0.2.0.dev350/ansible/roles/talos_users/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.124928 talos_install-0.2.0.dev350/ansible/roles/wiki/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.125928 talos_install-0.2.0.dev350/ansible/roles/wiki/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      536 2023-04-17 07:46:15.000000 talos_install-0.2.0.dev350/ansible/roles/wiki/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.125928 talos_install-0.2.0.dev350/ansible/roles/wiki/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev350/ansible/roles/wiki/meta/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/wiki/requirements.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.126928 talos_install-0.2.0.dev350/ansible/roles/wiki/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-04-17 09:16:59.000000 talos_install-0.2.0.dev350/ansible/roles/wiki/tasks/compose.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      222 2023-04-17 07:47:31.000000 talos_install-0.2.0.dev350/ansible/roles/wiki/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-04-17 07:36:52.000000 talos_install-0.2.0.dev350/ansible/roles/wiki/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.126928 talos_install-0.2.0.dev350/ansible/roles/wiki/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1153 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev350/ansible/roles/wiki/templates/docker-compose.yml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/wiki/templates/wiki.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev350/ansible/roles/wiki/templates/wikidump.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1588 2023-04-19 08:30:31.000000 talos_install-0.2.0.dev350/ansible/site.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.127928 talos_install-0.2.0.dev350/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      570 2023-04-19 13:42:43.000000 talos_install-0.2.0.dev350/etc/globals.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev350/etc/inventory
--rw-rw-r--   0 installer  (3002) installer  (3002)     1625 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev350/etc/talos.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-04-21 16:15:48.130928 talos_install-0.2.0.dev350/setup.cfg
--rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-04-21 16:00:17.000000 talos_install-0.2.0.dev350/setup.py
--rwxrwxr-x   0 installer  (3002) installer  (3002)     5797 2023-04-21 11:27:29.000000 talos_install-0.2.0.dev350/talos_install
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:15:48.128928 talos_install-0.2.0.dev350/talos_install.egg-info/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1960 2023-04-21 16:15:48.000000 talos_install-0.2.0.dev350/talos_install.egg-info/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     5419 2023-04-21 16:15:48.000000 talos_install-0.2.0.dev350/talos_install.egg-info/SOURCES.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-21 16:15:48.000000 talos_install-0.2.0.dev350/talos_install.egg-info/dependency_links.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-20 13:58:32.000000 talos_install-0.2.0.dev350/talos_install.egg-info/not-zip-safe
--rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-04-21 16:15:48.000000 talos_install-0.2.0.dev350/talos_install.egg-info/pbr.json
--rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-04-21 16:15:48.000000 talos_install-0.2.0.dev350/talos_install.egg-info/requires.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-21 16:15:48.000000 talos_install-0.2.0.dev350/talos_install.egg-info/top_level.txt
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.654961 talos_install-0.2.0.dev351/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/AUTHORS
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11635 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/ChangeLog
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2018 2023-04-21 16:40:19.654961 talos_install-0.2.0.dev351/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1358 2023-04-21 16:36:01.000000 talos_install-0.2.0.dev351/README.md
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.627961 talos_install-0.2.0.dev351/ansible/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      309 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/ansible.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.627961 talos_install-0.2.0.dev351/ansible/group_vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       23 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/group_vars/all.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.624961 talos_install-0.2.0.dev351/ansible/roles/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.613961 talos_install-0.2.0.dev351/ansible/roles/cli/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.627961 talos_install-0.2.0.dev351/ansible/roles/cli/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-21 16:33:02.000000 talos_install-0.2.0.dev351/ansible/roles/cli/files/FOUNDMEDEVKEY
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.627961 talos_install-0.2.0.dev351/ansible/roles/cli/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev351/ansible/roles/cli/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.629961 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1227 2023-04-21 16:39:14.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/clone.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1527 2023-04-19 08:23:48.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/env.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-04-17 07:40:14.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/logrotate.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      401 2023-04-21 14:29:02.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2748 2023-04-19 14:54:32.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1488 2023-04-17 09:13:53.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/web.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.631961 talos_install-0.2.0.dev351/ansible/roles/cli/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3793 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/agent.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      742 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/app.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/cli.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/env_talos.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-04-19 14:05:02.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/globals.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/my-httpd.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      351 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/passwords.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/talos-logrotate.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-04-16 16:14:02.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/talos.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/talospass.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.614961 talos_install-0.2.0.dev351/ansible/roles/common/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.631961 talos_install-0.2.0.dev351/ansible/roles/common/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev351/ansible/roles/common/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.632961 talos_install-0.2.0.dev351/ansible/roles/common/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-04-20 16:08:13.000000 talos_install-0.2.0.dev351/ansible/roles/common/tasks/install_extra_pkgs.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-04-17 08:59:47.000000 talos_install-0.2.0.dev351/ansible/roles/common/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev351/ansible/roles/common/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.614961 talos_install-0.2.0.dev351/ansible/roles/gather_facts/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.632961 talos_install-0.2.0.dev351/ansible/roles/gather_facts/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-04-17 07:54:44.000000 talos_install-0.2.0.dev351/ansible/roles/gather_facts/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.633961 talos_install-0.2.0.dev351/ansible/roles/gather_facts/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      964 2023-04-19 08:35:48.000000 talos_install-0.2.0.dev351/ansible/roles/gather_facts/vars/RedHat.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      964 2023-04-17 07:30:11.000000 talos_install-0.2.0.dev351/ansible/roles/gather_facts/vars/Rocky.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.615961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.615961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.633961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/files/inventory_plugins/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.633961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev351/ansible/roles/install_ansible/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.633961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      389 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev351/ansible/roles/install_ansible/tasks/install_ansible_collection.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1563 2023-04-21 15:41:33.000000 talos_install-0.2.0.dev351/ansible/roles/install_ansible/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.634961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      718 2023-04-16 13:01:28.000000 talos_install-0.2.0.dev351/ansible/roles/install_ansible/templates/ansible.cfg.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.615961 talos_install-0.2.0.dev351/ansible/roles/install_certificates/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.634961 talos_install-0.2.0.dev351/ansible/roles/install_certificates/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev351/ansible/roles/install_certificates/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.634961 talos_install-0.2.0.dev351/ansible/roles/install_certificates/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-04-19 14:04:55.000000 talos_install-0.2.0.dev351/ansible/roles/install_certificates/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.616961 talos_install-0.2.0.dev351/ansible/roles/install_docker/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.634961 talos_install-0.2.0.dev351/ansible/roles/install_docker/handlers/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-17 07:42:54.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/handlers/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.635961 talos_install-0.2.0.dev351/ansible/roles/install_docker/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.635961 talos_install-0.2.0.dev351/ansible/roles/install_docker/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1085 2023-04-20 12:42:13.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      626 2023-04-17 14:19:59.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/tasks/upstream.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.635961 talos_install-0.2.0.dev351/ansible/roles/install_docker/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/templates/daemon.json.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/templates/docker-ce.repo.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.616961 talos_install-0.2.0.dev351/ansible/roles/install_python/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.636961 talos_install-0.2.0.dev351/ansible/roles/install_python/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      440 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev351/ansible/roles/install_python/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.636961 talos_install-0.2.0.dev351/ansible/roles/install_python/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/install_python/vars/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.621961 talos_install-0.2.0.dev351/ansible/roles/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.636961 talos_install-0.2.0.dev351/ansible/roles/nagios/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-04-19 14:27:39.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.618961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.617961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.636961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.637961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/conf.d/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.637961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/monitor/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/monitor/.ID
+-rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-04-17 14:32:36.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/resource.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.620961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.637961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.618961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/apache2/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.637961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.619961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.638961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/apache/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/apache/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.638961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/nagios/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.638961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/postfix/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.638961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.620961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.619961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.638961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.639961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.640961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1573 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.640961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.640961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
+-rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.620961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.641961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.620961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/usr/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.620961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/usr/local/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.641961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/usr/local/bin/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.642961 talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-04-20 16:16:42.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.643961 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/cgi.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/contacts.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3642 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/localhost.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/nagios.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.623961 talos_install-0.2.0.dev351/ansible/roles/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.643961 talos_install-0.2.0.dev351/ansible/roles/opendcim/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.645961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/apache2.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/apache2.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-04-20 12:27:23.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/default.sql
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.621961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.622961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.645961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/drawings/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.645961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/pictures/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/mysqld.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.622961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.622961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.622961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.645961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.646961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    53192 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)    20091 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.646961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-04-20 13:50:07.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/pre-conf.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-04-20 15:35:00.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/startup.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.647961 talos_install-0.2.0.dev351/ansible/roles/opendcim/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.648961 talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.648961 talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-04-20 13:12:20.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-04-20 09:06:15.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/first-run.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/opendcim.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.623961 talos_install-0.2.0.dev351/ansible/roles/os_tune/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.649961 talos_install-0.2.0.dev351/ansible/roles/os_tune/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1281 2023-04-21 12:02:42.000000 talos_install-0.2.0.dev351/ansible/roles/os_tune/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.624961 talos_install-0.2.0.dev351/ansible/roles/talos_users/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.649961 talos_install-0.2.0.dev351/ansible/roles/talos_users/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/talos_users/files/talos
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.649961 talos_install-0.2.0.dev351/ansible/roles/talos_users/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev351/ansible/roles/talos_users/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.649961 talos_install-0.2.0.dev351/ansible/roles/talos_users/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      659 2023-04-17 07:48:59.000000 talos_install-0.2.0.dev351/ansible/roles/talos_users/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.650961 talos_install-0.2.0.dev351/ansible/roles/wiki/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.650961 talos_install-0.2.0.dev351/ansible/roles/wiki/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      536 2023-04-17 07:46:15.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.650961 talos_install-0.2.0.dev351/ansible/roles/wiki/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/meta/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/requirements.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.651961 talos_install-0.2.0.dev351/ansible/roles/wiki/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-04-17 09:16:59.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/tasks/compose.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      222 2023-04-17 07:47:31.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-04-17 07:36:52.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.651961 talos_install-0.2.0.dev351/ansible/roles/wiki/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1153 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/templates/docker-compose.yml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/templates/wiki.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/templates/wikidump.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1588 2023-04-19 08:30:31.000000 talos_install-0.2.0.dev351/ansible/site.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.652961 talos_install-0.2.0.dev351/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      570 2023-04-19 13:42:43.000000 talos_install-0.2.0.dev351/etc/globals.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev351/etc/inventory
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1625 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev351/etc/talos.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-04-21 16:40:19.655961 talos_install-0.2.0.dev351/setup.cfg
+-rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-04-21 16:00:17.000000 talos_install-0.2.0.dev351/setup.py
+-rwxrwxr-x   0 installer  (3002) installer  (3002)     5949 2023-04-21 16:39:36.000000 talos_install-0.2.0.dev351/talos_install
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.654961 talos_install-0.2.0.dev351/talos_install.egg-info/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2018 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5457 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/SOURCES.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/dependency_links.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-20 13:58:32.000000 talos_install-0.2.0.dev351/talos_install.egg-info/not-zip-safe
+-rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/pbr.json
+-rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/requires.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/top_level.txt
```

### Comparing `talos_install-0.2.0.dev350/ChangeLog` & `talos_install-0.2.0.dev351/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES
 =======
 
+* fix missing dev\_keys installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix service not found
```

### Comparing `talos_install-0.2.0.dev350/PKG-INFO` & `talos_install-0.2.0.dev351/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos_install
-Version: 0.2.0.dev350
+Version: 0.2.0.dev351
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: AUTHORS
 
 # All in One installation
 
 KEY REQUIRED
 Ask for dev_key and dev_key.pub to download TALOS-CLI from GIT
+Save key in your \<HOME>/.ssh folder
 
 ## OS requirements
 
 Supported OS is Rocky Linux 8 (or any RHEL Like distibution)
 
 An **user with sudo permissions** is MANDATORY, don't use root directly.
 
@@ -32,16 +33,16 @@
 - python >= 3.9
 - pip >= 3.9
 - ansible >= 7
 
 ```bash
 sudo dnf install epel-release -y
 
-# Install Python 3.9
-sudo dnf install python39  python39-pip -y
+# Install Python 3.9 requirements
+sudo dnf install python39  python39-pip sshpass -y
 
 # Update pip
 pip3.9 install --upgrade pip
 
 # Install package
 pip install talos-install
 ```
```

### Comparing `talos_install-0.2.0.dev350/README.md` & `talos_install-0.2.0.dev351/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # All in One installation
 
 KEY REQUIRED
 Ask for dev_key and dev_key.pub to download TALOS-CLI from GIT
+Save key in your \<HOME>/.ssh folder
 
 ## OS requirements
 
 Supported OS is Rocky Linux 8 (or any RHEL Like distibution)
 
 An **user with sudo permissions** is MANDATORY, don't use root directly.
 
@@ -14,16 +15,16 @@
 - python >= 3.9
 - pip >= 3.9
 - ansible >= 7
 
 ```bash
 sudo dnf install epel-release -y
 
-# Install Python 3.9
-sudo dnf install python39  python39-pip -y
+# Install Python 3.9 requirements
+sudo dnf install python39  python39-pip sshpass -y
 
 # Update pip
 pip3.9 install --upgrade pip
 
 # Install package
 pip install talos-install
 ```
```

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/tasks/clone.yaml` & `talos_install-0.2.0.dev351/ansible/roles/cli/tasks/clone.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,23 @@
 ---
+- name: Copy dev key
+  ansible.builtin.copy:
+    src: "{{ item.file }}"
+    dest: "/home/{{ master.user }}/.ssh/{{ item.file }}"
+    mode: '{{ item.mode }}'
+    owner: "{{ master.user }}"
+    group: "{{ master.user }}"
+  loop:
+    - file: dev_key
+      mode: "600"
+    - file: dev_key.pub
+      mode: "644"
+  become_user: "{{ master.user }}"
+  become: true
+
 - name: Ensure ssh config exist
   ansible.builtin.file:
     path: "/home/{{ master.user }}/.ssh/config"
     state: touch
     mode: '0600'
     owner: "{{ master.user }}"
     group: "{{ master.user }}"
```

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/tasks/env.yaml` & `talos_install-0.2.0.dev351/ansible/roles/cli/tasks/env.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/tasks/misc.yaml` & `talos_install-0.2.0.dev351/ansible/roles/cli/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/tasks/web.yaml` & `talos_install-0.2.0.dev351/ansible/roles/cli/tasks/web.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/templates/agent.sh.j2` & `talos_install-0.2.0.dev351/ansible/roles/cli/templates/agent.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/templates/app.yaml.j2` & `talos_install-0.2.0.dev351/ansible/roles/cli/templates/app.yaml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/templates/cli.conf.j2` & `talos_install-0.2.0.dev351/ansible/roles/cli/templates/cli.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/templates/env_talos.j2` & `talos_install-0.2.0.dev351/ansible/roles/cli/templates/env_talos.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/templates/globals.yaml.j2` & `talos_install-0.2.0.dev351/ansible/roles/cli/templates/globals.yaml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/templates/my-httpd.conf.j2` & `talos_install-0.2.0.dev351/ansible/roles/cli/templates/my-httpd.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/cli/templates/talos.conf.j2` & `talos_install-0.2.0.dev351/ansible/roles/cli/templates/talos.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/common/tasks/misc.yaml` & `talos_install-0.2.0.dev351/ansible/roles/common/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/gather_facts/vars/RedHat.yaml` & `talos_install-0.2.0.dev351/ansible/roles/gather_facts/vars/RedHat.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/gather_facts/vars/Rocky.yaml` & `talos_install-0.2.0.dev351/ansible/roles/gather_facts/vars/Rocky.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py` & `talos_install-0.2.0.dev351/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/install_ansible/tasks/main.yaml` & `talos_install-0.2.0.dev351/ansible/roles/install_ansible/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/install_ansible/templates/ansible.cfg.j2` & `talos_install-0.2.0.dev351/ansible/roles/install_ansible/templates/ansible.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/install_certificates/tasks/main.yaml` & `talos_install-0.2.0.dev351/ansible/roles/install_certificates/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/install_docker/tasks/main.yaml` & `talos_install-0.2.0.dev351/ansible/roles/install_docker/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/install_docker/tasks/upstream.yaml` & `talos_install-0.2.0.dev351/ansible/roles/install_docker/tasks/upstream.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/install_docker/templates/docker-ce.repo.j2` & `talos_install-0.2.0.dev351/ansible/roles/install_docker/templates/docker-ce.repo.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/nagios/run` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/nagios/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/etc/sv/postfix/run` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/postfix/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios` & `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/tasks/build.yaml` & `talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/tasks/misc.yaml` & `talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/tasks/run.yaml` & `talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/templates/Dockerfile.j2` & `talos_install-0.2.0.dev351/ansible/roles/nagios/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/templates/cgi.cfg.j2` & `talos_install-0.2.0.dev351/ansible/roles/nagios/templates/cgi.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/templates/contacts.cfg.j2` & `talos_install-0.2.0.dev351/ansible/roles/nagios/templates/contacts.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/nagios/templates/localhost.cfg.j2` & `talos_install-0.2.0.dev351/ansible/roles/nagios/templates/localhost.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/files/apache2.conf` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/apache2.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/files/default.sql` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/default.sql`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/files/pre-conf.sh` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/pre-conf.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/files/startup.sh` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/startup.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/tasks/build.yaml` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/tasks/misc.yaml` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/tasks/run.yaml` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/templates/Dockerfile.j2` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/opendcim/templates/first-run.sh.j2` & `talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/first-run.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/os_tune/tasks/main.yaml` & `talos_install-0.2.0.dev351/ansible/roles/os_tune/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/talos_users/tasks/main.yaml` & `talos_install-0.2.0.dev351/ansible/roles/talos_users/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/wiki/defaults/main.yaml` & `talos_install-0.2.0.dev351/ansible/roles/wiki/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/wiki/tasks/compose.yaml` & `talos_install-0.2.0.dev351/ansible/roles/wiki/tasks/compose.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/roles/wiki/templates/docker-compose.yml.j2` & `talos_install-0.2.0.dev351/ansible/roles/wiki/templates/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/ansible/site.yaml` & `talos_install-0.2.0.dev351/ansible/site.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/etc/globals.yaml` & `talos_install-0.2.0.dev351/etc/globals.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/etc/talos.yaml` & `talos_install-0.2.0.dev351/etc/talos.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/setup.cfg` & `talos_install-0.2.0.dev351/setup.cfg`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev350/talos_install` & `talos_install-0.2.0.dev351/talos_install`

 * *Files 3% similar despite different names*

```diff
@@ -109,14 +109,22 @@
 
 dir=$(which talos_install)
 dir="$(dirname $dir)"
 dir="$(dirname $dir)"
 
 basedir=${dir}/share/talos_install
 
+if [[ -f ~/.ssh/dev_key ]]; then
+  \cp ~/.ssh/dev_key* ${basedir}/ansible/roles/cli/files/
+else
+  echo "Missing dev_key in ~/.ssh folder"
+  exit 2
+fi
+
+
 ANSIBLE_CONFIG="${basedir}/ansible/ansible.cfg"
 config_dir="${basedir}/etc"
 inventory="${basedir}/etc/inventory"
 playbook="${basedir}/ansible/site.yml"
 verbosity=""
 extra_opts=""
 target=""
```

### Comparing `talos_install-0.2.0.dev350/talos_install.egg-info/PKG-INFO` & `talos_install-0.2.0.dev351/talos_install.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos-install
-Version: 0.2.0.dev350
+Version: 0.2.0.dev351
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: AUTHORS
 
 # All in One installation
 
 KEY REQUIRED
 Ask for dev_key and dev_key.pub to download TALOS-CLI from GIT
+Save key in your \<HOME>/.ssh folder
 
 ## OS requirements
 
 Supported OS is Rocky Linux 8 (or any RHEL Like distibution)
 
 An **user with sudo permissions** is MANDATORY, don't use root directly.
 
@@ -32,16 +33,16 @@
 - python >= 3.9
 - pip >= 3.9
 - ansible >= 7
 
 ```bash
 sudo dnf install epel-release -y
 
-# Install Python 3.9
-sudo dnf install python39  python39-pip -y
+# Install Python 3.9 requirements
+sudo dnf install python39  python39-pip sshpass -y
 
 # Update pip
 pip3.9 install --upgrade pip
 
 # Install package
 pip install talos-install
 ```
```

### Comparing `talos_install-0.2.0.dev350/talos_install.egg-info/SOURCES.txt` & `talos_install-0.2.0.dev351/talos_install.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 setup.cfg
 setup.py
 talos_install
 ansible/ansible.cfg
 ansible/site.yaml
 ansible/group_vars/all.yaml
+ansible/roles/cli/files/FOUNDMEDEVKEY
 ansible/roles/cli/meta/main.yaml
 ansible/roles/cli/tasks/clone.yaml
 ansible/roles/cli/tasks/env.yaml
 ansible/roles/cli/tasks/logrotate.yaml
 ansible/roles/cli/tasks/main.yaml
 ansible/roles/cli/tasks/misc.yaml
 ansible/roles/cli/tasks/web.yaml
```

