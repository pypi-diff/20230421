# Comparing `tmp/binarylane_cli-0.15.3.tar.gz` & `tmp/binarylane_cli-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binarylane_cli-0.15.3.tar", max compression
+gzip compressed data, was "binarylane_cli-0.16.0.tar", max compression
```

## Comparing `binarylane_cli-0.15.3.tar` & `binarylane_cli-0.16.0.tar`

### file list

```diff
@@ -1,547 +1,546 @@
--rw-r--r--   0        0        0     1078 2023-02-07 09:32:33.853646 binarylane_cli-0.15.3/LICENSE
--rw-r--r--   0        0        0    16395 2023-02-17 22:36:19.031007 binarylane_cli-0.15.3/README.md
--rw-r--r--   0        0        0       83 2023-03-29 02:52:04.102649 binarylane_cli-0.15.3/lib/binarylane/api/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.318645 binarylane_cli-0.15.3/lib/binarylane/api/accounts/__init__.py
--rw-r--r--   0        0        0     3886 2023-03-29 02:52:06.690664 binarylane_cli-0.15.3/lib/binarylane/api/accounts/get_v2_account.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.342645 binarylane_cli-0.15.3/lib/binarylane/api/actions/__init__.py
--rw-r--r--   0        0        0     5427 2023-03-29 02:52:06.774664 binarylane_cli-0.15.3/lib/binarylane/api/actions/get_v2_actions.py
--rw-r--r--   0        0        0     4698 2023-03-29 02:52:06.774664 binarylane_cli-0.15.3/lib/binarylane/api/actions/get_v2_actions_action_id.py
--rw-r--r--   0        0        0     5165 2023-03-29 02:52:06.778665 binarylane_cli-0.15.3/lib/binarylane/api/actions/post_v2_actions_action_id_proceed.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.342645 binarylane_cli-0.15.3/lib/binarylane/api/customers/__init__.py
--rw-r--r--   0        0        0     3859 2023-03-29 02:52:06.826665 binarylane_cli-0.15.3/lib/binarylane/api/customers/get_v2_customers_my_balance.py
--rw-r--r--   0        0        0     5446 2023-03-29 02:52:06.826665 binarylane_cli-0.15.3/lib/binarylane/api/customers/get_v2_customers_my_invoices.py
--rw-r--r--   0        0        0     4717 2023-03-29 02:52:06.826665 binarylane_cli-0.15.3/lib/binarylane/api/customers/get_v2_customers_my_invoices_invoice_id.py
--rw-r--r--   0        0        0     4605 2023-03-29 02:52:06.830665 binarylane_cli-0.15.3/lib/binarylane/api/customers/get_v2_customers_my_unpaid_payment_failed_invoices.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.346645 binarylane_cli-0.15.3/lib/binarylane/api/data_usages/__init__.py
--rw-r--r--   0        0        0     5635 2023-03-29 02:52:06.750664 binarylane_cli-0.15.3/lib/binarylane/api/data_usages/get_v2_data_usages_current.py
--rw-r--r--   0        0        0     4826 2023-03-29 02:52:06.750664 binarylane_cli-0.15.3/lib/binarylane/api/data_usages/get_v2_data_usages_server_id_current.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.350645 binarylane_cli-0.15.3/lib/binarylane/api/domains/__init__.py
--rw-r--r--   0        0        0     4505 2023-03-29 02:52:06.770665 binarylane_cli-0.15.3/lib/binarylane/api/domains/delete_v2_domains_domain_name.py
--rw-r--r--   0        0        0     5124 2023-03-29 02:52:06.766665 binarylane_cli-0.15.3/lib/binarylane/api/domains/delete_v2_domains_domain_name_records_record_id.py
--rw-r--r--   0        0        0     6308 2023-03-29 02:52:06.770665 binarylane_cli-0.15.3/lib/binarylane/api/domains/get_v2_domains.py
--rw-r--r--   0        0        0     4746 2023-03-29 02:52:06.762664 binarylane_cli-0.15.3/lib/binarylane/api/domains/get_v2_domains_domain_name.py
--rw-r--r--   0        0        0    11108 2023-03-29 02:52:06.766665 binarylane_cli-0.15.3/lib/binarylane/api/domains/get_v2_domains_domain_name_records.py
--rw-r--r--   0        0        0     5444 2023-03-29 02:52:06.770665 binarylane_cli-0.15.3/lib/binarylane/api/domains/get_v2_domains_domain_name_records_record_id.py
--rw-r--r--   0        0        0     3952 2023-03-29 02:52:06.770665 binarylane_cli-0.15.3/lib/binarylane/api/domains/get_v2_domains_nameservers.py
--rw-r--r--   0        0        0     4878 2023-03-29 02:52:06.762664 binarylane_cli-0.15.3/lib/binarylane/api/domains/post_v2_domains.py
--rw-r--r--   0        0        0     6881 2023-03-29 02:52:06.762664 binarylane_cli-0.15.3/lib/binarylane/api/domains/post_v2_domains_domain_name_records.py
--rw-r--r--   0        0        0     2886 2023-03-29 02:52:06.758664 binarylane_cli-0.15.3/lib/binarylane/api/domains/post_v2_domains_refresh_nameserver_cache.py
--rw-r--r--   0        0        0     7399 2023-03-29 02:52:06.766665 binarylane_cli-0.15.3/lib/binarylane/api/domains/put_v2_domains_domain_name_records_record_id.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.362645 binarylane_cli-0.15.3/lib/binarylane/api/failover_ips/__init__.py
--rw-r--r--   0        0        0     6382 2023-03-29 02:52:06.786665 binarylane_cli-0.15.3/lib/binarylane/api/failover_ips/get_v2_failover_ips_server_id.py
--rw-r--r--   0        0        0     6564 2023-03-29 02:52:06.786665 binarylane_cli-0.15.3/lib/binarylane/api/failover_ips/get_v2_failover_ips_server_id_available.py
--rw-r--r--   0        0        0     7465 2023-03-29 02:52:06.790665 binarylane_cli-0.15.3/lib/binarylane/api/failover_ips/post_v2_failover_ips_server_id.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.366645 binarylane_cli-0.15.3/lib/binarylane/api/images/__init__.py
--rw-r--r--   0        0        0     7947 2023-03-29 02:52:06.834665 binarylane_cli-0.15.3/lib/binarylane/api/images/get_v2_images.py
--rw-r--r--   0        0        0     5098 2023-03-29 02:52:06.830665 binarylane_cli-0.15.3/lib/binarylane/api/images/get_v2_images_image_id_download.py
--rw-r--r--   0        0        0     5152 2023-03-29 03:05:42.875441 binarylane_cli-0.15.3/lib/binarylane/api/images/get_v2_images_image_id_or_slug.py
--rw-r--r--   0        0        0     5969 2023-03-29 02:52:06.830665 binarylane_cli-0.15.3/lib/binarylane/api/images/put_v2_images_image_id.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.370645 binarylane_cli-0.15.3/lib/binarylane/api/keys/__init__.py
--rw-r--r--   0        0        0     4874 2023-03-29 03:05:42.875441 binarylane_cli-0.15.3/lib/binarylane/api/keys/delete_v2_account_keys_key_id.py
--rw-r--r--   0        0        0     5437 2023-03-29 02:52:06.758664 binarylane_cli-0.15.3/lib/binarylane/api/keys/get_v2_account_keys.py
--rw-r--r--   0        0        0     5116 2023-03-29 03:05:42.875441 binarylane_cli-0.15.3/lib/binarylane/api/keys/get_v2_account_keys_key_id.py
--rw-r--r--   0        0        0     4877 2023-03-29 02:52:06.754665 binarylane_cli-0.15.3/lib/binarylane/api/keys/post_v2_account_keys.py
--rw-r--r--   0        0        0     6236 2023-03-29 03:05:42.875441 binarylane_cli-0.15.3/lib/binarylane/api/keys/put_v2_account_keys_key_id.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.374645 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/__init__.py
--rw-r--r--   0        0        0     4660 2023-03-29 02:52:06.798665 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id.py
--rw-r--r--   0        0        0     6123 2023-03-29 02:52:06.794665 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id_forwarding_rules.py
--rw-r--r--   0        0        0     6072 2023-03-29 02:52:06.790665 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id_servers.py
--rw-r--r--   0        0        0     5541 2023-03-29 02:52:06.794665 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/get_v2_load_balancers.py
--rw-r--r--   0        0        0     4145 2023-03-29 02:52:06.790665 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/get_v2_load_balancers_availability.py
--rw-r--r--   0        0        0     4980 2023-03-29 02:52:06.790665 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/get_v2_load_balancers_load_balancer_id.py
--rw-r--r--   0        0        0     5584 2023-03-29 02:52:06.794665 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/post_v2_load_balancers.py
--rw-r--r--   0        0        0     6089 2023-03-29 02:52:06.798665 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/post_v2_load_balancers_load_balancer_id_forwarding_rules.py
--rw-r--r--   0        0        0     6038 2023-03-29 02:52:06.802665 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/post_v2_load_balancers_load_balancer_id_servers.py
--rw-r--r--   0        0        0     6613 2023-03-29 02:52:06.798665 binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/put_v2_load_balancers_load_balancer_id.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.386645 binarylane_cli-0.15.3/lib/binarylane/api/regions/__init__.py
--rw-r--r--   0        0        0     5178 2023-03-29 02:52:06.822665 binarylane_cli-0.15.3/lib/binarylane/api/regions/get_v2_regions.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.386645 binarylane_cli-0.15.3/lib/binarylane/api/reverse_names/__init__.py
--rw-r--r--   0        0        0     7559 2023-03-29 02:52:06.682664 binarylane_cli-0.15.3/lib/binarylane/api/reverse_names/get_v2_reverse_names_ipv6.py
--rw-r--r--   0        0        0     5530 2023-03-29 02:52:06.682664 binarylane_cli-0.15.3/lib/binarylane/api/reverse_names/post_v2_reverse_names_ipv6.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.390645 binarylane_cli-0.15.3/lib/binarylane/api/sample_sets/__init__.py
--rw-r--r--   0        0        0    12650 2023-03-29 02:52:06.822665 binarylane_cli-0.15.3/lib/binarylane/api/sample_sets/get_v2_samplesets_server_id.py
--rw-r--r--   0        0        0     7362 2023-03-29 02:52:06.822665 binarylane_cli-0.15.3/lib/binarylane/api/sample_sets/get_v2_samplesets_server_id_latest.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.394645 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/__init__.py
--rw-r--r--   0        0        0     6448 2023-03-29 02:52:06.718664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/get_v2_servers_server_id_actions.py
--rw-r--r--   0        0        0    22360 2023-03-29 02:52:06.742664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v2_servers_server_id_actions.py
--rw-r--r--   0        0        0     7190 2023-03-29 02:52:06.706664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_add_disk.py
--rw-r--r--   0        0        0     6826 2023-03-29 02:52:06.738664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_attach_backup.py
--rw-r--r--   0        0        0     6967 2023-03-29 02:52:06.694664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_advanced_features.py
--rw-r--r--   0        0        0     7044 2023-03-29 02:52:06.710664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_advanced_firewall_rules.py
--rw-r--r--   0        0        0     6823 2023-03-29 02:52:06.702664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_backup_schedule.py
--rw-r--r--   0        0        0     6643 2023-03-29 02:52:06.722664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_ipv_6.py
--rw-r--r--   0        0        0     6997 2023-03-29 02:52:06.722664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_ipv_6_reverse_nameservers.py
--rw-r--r--   0        0        0     6934 2023-03-29 02:52:06.714664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_kernel.py
--rw-r--r--   0        0        0     7495 2023-03-29 02:52:06.694664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_manage_offsite_backup_copies.py
--rw-r--r--   0        0        0     6946 2023-03-29 02:52:06.710664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_network.py
--rw-r--r--   0        0        0     7316 2023-03-29 02:52:06.694664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_offsite_backup_location.py
--rw-r--r--   0        0        0     6842 2023-03-29 02:52:06.702664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_partner.py
--rw-r--r--   0        0        0     7967 2023-03-29 02:52:06.742664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_port_blocking.py
--rw-r--r--   0        0        0     6859 2023-03-29 02:52:06.714664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_reverse_name.py
--rw-r--r--   0        0        0     7567 2023-03-29 02:52:06.746664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_separate_private_network_interface.py
--rw-r--r--   0        0        0    10443 2023-03-29 02:52:06.718664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_source_and_destination_check.py
--rw-r--r--   0        0        0     6911 2023-03-29 02:52:06.722664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_threshold_alerts.py
--rw-r--r--   0        0        0     6744 2023-03-29 02:52:06.690664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_vpc_ipv_4.py
--rw-r--r--   0        0        0     8171 2023-03-29 02:52:06.698664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_clone_using_backup.py
--rw-r--r--   0        0        0     6990 2023-03-29 02:52:06.718664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_delete_disk.py
--rw-r--r--   0        0        0     6730 2023-03-29 02:52:06.726664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_detach_backup.py
--rw-r--r--   0        0        0     8362 2023-03-29 02:52:06.734664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_disable_backups.py
--rw-r--r--   0        0        0     7074 2023-03-29 02:52:06.738664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_disable_selinux.py
--rw-r--r--   0        0        0     7574 2023-03-29 02:52:06.730664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_enable_backups.py
--rw-r--r--   0        0        0     7031 2023-03-29 02:52:06.746664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_enable_ipv_6.py
--rw-r--r--   0        0        0     6914 2023-03-29 02:52:06.714664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_is_running.py
--rw-r--r--   0        0        0     7126 2023-03-29 02:52:06.730664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_password_reset.py
--rw-r--r--   0        0        0     6881 2023-03-29 02:52:06.706664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_ping.py
--rw-r--r--   0        0        0     7034 2023-03-29 02:52:06.726664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_cycle.py
--rw-r--r--   0        0        0     6506 2023-03-29 02:52:06.706664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_off.py
--rw-r--r--   0        0        0     6690 2023-03-29 02:52:06.730664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_on.py
--rw-r--r--   0        0        0     7149 2023-03-29 02:52:06.734664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_reboot.py
--rw-r--r--   0        0        0     6829 2023-03-29 02:52:06.706664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_rebuild.py
--rw-r--r--   0        0        0     6645 2023-03-29 02:52:06.702664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_rename.py
--rw-r--r--   0        0        0     7897 2023-03-29 02:52:06.738664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_resize.py
--rw-r--r--   0        0        0     7446 2023-03-29 02:52:06.734664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_resize_disk.py
--rw-r--r--   0        0        0     6929 2023-03-29 02:52:06.698664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_restore.py
--rw-r--r--   0        0        0     7101 2023-03-29 02:52:06.746664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_shutdown.py
--rw-r--r--   0        0        0     6454 2023-03-29 02:52:06.730664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_take_backup.py
--rw-r--r--   0        0        0     6825 2023-03-29 02:52:06.710664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_uncancel.py
--rw-r--r--   0        0        0     6545 2023-03-29 02:52:06.750664 binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_uptime.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.458645 binarylane_cli-0.15.3/lib/binarylane/api/servers/__init__.py
--rw-r--r--   0        0        0     5309 2023-03-29 02:52:06.806665 binarylane_cli-0.15.3/lib/binarylane/api/servers/delete_v2_servers_server_id.py
--rw-r--r--   0        0        0     6741 2023-03-29 02:52:06.818665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers.py
--rw-r--r--   0        0        0     4698 2023-03-29 02:52:06.810665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id.py
--rw-r--r--   0        0        0     5333 2023-03-29 02:52:06.814665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_actions_action_id.py
--rw-r--r--   0        0        0     5139 2023-03-29 02:52:06.806665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_advanced_firewall_rules.py
--rw-r--r--   0        0        0     5342 2023-03-29 02:52:06.802665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_available_advanced_features.py
--rw-r--r--   0        0        0     6448 2023-03-29 02:52:06.810665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_backups.py
--rw-r--r--   0        0        0     5384 2023-03-29 02:52:06.810665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_console.py
--rw-r--r--   0        0        0     6828 2023-03-29 02:52:06.806665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_kernels.py
--rw-r--r--   0        0        0     6808 2023-03-29 02:52:06.802665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_snapshots.py
--rw-r--r--   0        0        0     6624 2023-03-29 02:52:06.814665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_software.py
--rw-r--r--   0        0        0     5405 2023-03-29 02:52:06.818665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_threshold_alerts.py
--rw-r--r--   0        0        0     4814 2023-03-29 02:52:06.814665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_user_data.py
--rw-r--r--   0        0        0     4513 2023-03-29 02:52:06.806665 binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_threshold_alerts.py
--rw-r--r--   0        0        0     5024 2023-03-29 02:52:06.814665 binarylane_cli-0.15.3/lib/binarylane/api/servers/post_v2_servers.py
--rw-r--r--   0        0        0     6101 2023-03-29 02:52:06.818665 binarylane_cli-0.15.3/lib/binarylane/api/servers/post_v2_servers_server_id_backups.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.478646 binarylane_cli-0.15.3/lib/binarylane/api/sizes/__init__.py
--rw-r--r--   0        0        0     9151 2023-03-29 03:05:42.879441 binarylane_cli-0.15.3/lib/binarylane/api/sizes/get_v2_sizes.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.478646 binarylane_cli-0.15.3/lib/binarylane/api/software/__init__.py
--rw-r--r--   0        0        0     5249 2023-03-29 02:52:06.690664 binarylane_cli-0.15.3/lib/binarylane/api/software/get_v2_software.py
--rw-r--r--   0        0        0     7624 2023-03-29 03:05:42.879441 binarylane_cli-0.15.3/lib/binarylane/api/software/get_v2_software_operating_system_operating_system_id_or_slug.py
--rw-r--r--   0        0        0     4578 2023-03-29 02:52:06.686664 binarylane_cli-0.15.3/lib/binarylane/api/software/get_v2_software_software_id.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:03.482646 binarylane_cli-0.15.3/lib/binarylane/api/vpcs/__init__.py
--rw-r--r--   0        0        0     4477 2023-03-29 02:52:06.778665 binarylane_cli-0.15.3/lib/binarylane/api/vpcs/delete_v2_vpcs_vpc_id.py
--rw-r--r--   0        0        0     5409 2023-03-29 02:52:06.782665 binarylane_cli-0.15.3/lib/binarylane/api/vpcs/get_v2_vpcs.py
--rw-r--r--   0        0        0     4524 2023-03-29 02:52:06.782665 binarylane_cli-0.15.3/lib/binarylane/api/vpcs/get_v2_vpcs_vpc_id.py
--rw-r--r--   0        0        0     8911 2023-03-29 02:52:06.786665 binarylane_cli-0.15.3/lib/binarylane/api/vpcs/get_v2_vpcs_vpc_id_members.py
--rw-r--r--   0        0        0     5833 2023-03-29 02:52:06.778665 binarylane_cli-0.15.3/lib/binarylane/api/vpcs/patch_v2_vpcs_vpc_id.py
--rw-r--r--   0        0        0     4858 2023-03-29 02:52:06.778665 binarylane_cli-0.15.3/lib/binarylane/api/vpcs/post_v2_vpcs.py
--rw-r--r--   0        0        0     6150 2023-03-29 02:52:06.782665 binarylane_cli-0.15.3/lib/binarylane/api/vpcs/put_v2_vpcs_vpc_id.py
--rw-r--r--   0        0        0     2709 2023-03-29 02:52:05.590658 binarylane_cli-0.15.3/lib/binarylane/client.py
--rw-r--r--   0        0        0      318 2023-03-29 02:52:05.558658 binarylane_cli-0.15.3/lib/binarylane/errors.py
--rw-r--r--   0        0        0        0 2023-03-29 02:52:06.646664 binarylane_cli-0.15.3/lib/binarylane/models/__init__.py
--rw-r--r--   0        0        0     3964 2023-03-29 02:52:06.922665 binarylane_cli-0.15.3/lib/binarylane/models/account.py
--rw-r--r--   0        0        0     1524 2023-03-29 02:52:07.010666 binarylane_cli-0.15.3/lib/binarylane/models/account_response.py
--rw-r--r--   0        0        0      252 2023-03-29 02:52:04.386651 binarylane_cli-0.15.3/lib/binarylane/models/account_status.py
--rw-r--r--   0        0        0     8597 2023-03-29 02:52:07.006666 binarylane_cli-0.15.3/lib/binarylane/models/action.py
--rw-r--r--   0        0        0     1639 2023-03-29 02:52:05.690658 binarylane_cli-0.15.3/lib/binarylane/models/action_link.py
--rw-r--r--   0        0        0     2943 2023-03-29 02:52:06.994666 binarylane_cli-0.15.3/lib/binarylane/models/action_progress.py
--rw-r--r--   0        0        0     1504 2023-03-29 02:52:06.990666 binarylane_cli-0.15.3/lib/binarylane/models/action_response.py
--rw-r--r--   0        0        0      237 2023-03-29 02:52:04.470651 binarylane_cli-0.15.3/lib/binarylane/models/action_status.py
--rw-r--r--   0        0        0     1813 2023-03-29 02:52:06.890665 binarylane_cli-0.15.3/lib/binarylane/models/actions_links.py
--rw-r--r--   0        0        0     2809 2023-03-29 02:52:06.906665 binarylane_cli-0.15.3/lib/binarylane/models/actions_response.py
--rw-r--r--   0        0        0     2390 2023-03-29 02:52:06.898665 binarylane_cli-0.15.3/lib/binarylane/models/add_disk.py
--rw-r--r--   0        0        0      178 2023-03-29 02:52:04.454651 binarylane_cli-0.15.3/lib/binarylane/models/add_disk_type.py
--rw-r--r--   0        0        0      494 2023-03-29 02:52:04.458651 binarylane_cli-0.15.3/lib/binarylane/models/advanced_feature.py
--rw-r--r--   0        0        0     4296 2023-03-29 02:52:06.894665 binarylane_cli-0.15.3/lib/binarylane/models/advanced_firewall_rule.py
--rw-r--r--   0        0        0      207 2023-03-29 02:52:04.298650 binarylane_cli-0.15.3/lib/binarylane/models/advanced_firewall_rule_action.py
--rw-r--r--   0        0        0      235 2023-03-29 02:52:04.506651 binarylane_cli-0.15.3/lib/binarylane/models/advanced_firewall_rule_protocol.py
--rw-r--r--   0        0        0     2325 2023-03-29 02:52:07.002666 binarylane_cli-0.15.3/lib/binarylane/models/advanced_firewall_rules_response.py
--rw-r--r--   0        0        0     4703 2023-03-29 02:52:06.866665 binarylane_cli-0.15.3/lib/binarylane/models/advanced_server_features.py
--rw-r--r--   0        0        0     1746 2023-03-29 02:52:06.962666 binarylane_cli-0.15.3/lib/binarylane/models/attach_backup.py
--rw-r--r--   0        0        0      193 2023-03-29 02:52:04.370651 binarylane_cli-0.15.3/lib/binarylane/models/attach_backup_type.py
--rw-r--r--   0        0        0     3782 2023-03-29 02:52:06.910665 binarylane_cli-0.15.3/lib/binarylane/models/attached_backup.py
--rw-r--r--   0        0        0     3789 2023-03-29 02:52:06.890665 binarylane_cli-0.15.3/lib/binarylane/models/available_advanced_server_features.py
--rw-r--r--   0        0        0     2068 2023-03-29 02:52:06.862665 binarylane_cli-0.15.3/lib/binarylane/models/available_advanced_server_features_response.py
--rw-r--r--   0        0        0     2387 2023-03-29 02:52:06.874665 binarylane_cli-0.15.3/lib/binarylane/models/backup_disk.py
--rw-r--r--   0        0        0     3714 2023-03-29 02:52:06.850665 binarylane_cli-0.15.3/lib/binarylane/models/backup_info.py
--rw-r--r--   0        0        0      256 2023-03-29 02:52:04.338651 binarylane_cli-0.15.3/lib/binarylane/models/backup_replacement_strategy.py
--rw-r--r--   0        0        0     3665 2023-03-29 02:52:06.918665 binarylane_cli-0.15.3/lib/binarylane/models/backup_settings.py
--rw-r--r--   0        0        0      245 2023-03-29 02:52:04.358651 binarylane_cli-0.15.3/lib/binarylane/models/backup_slot.py
--rw-r--r--   0        0        0     1984 2023-03-29 02:52:05.766659 binarylane_cli-0.15.3/lib/binarylane/models/backup_window.py
--rw-r--r--   0        0        0     2804 2023-03-29 02:52:07.006666 binarylane_cli-0.15.3/lib/binarylane/models/backups_response.py
--rw-r--r--   0        0        0     3413 2023-03-29 02:52:06.986666 binarylane_cli-0.15.3/lib/binarylane/models/balance.py
--rw-r--r--   0        0        0     1524 2023-03-29 02:52:06.982666 binarylane_cli-0.15.3/lib/binarylane/models/balance_response.py
--rw-r--r--   0        0        0     6741 2023-03-29 02:52:06.898665 binarylane_cli-0.15.3/lib/binarylane/models/change_advanced_features.py
--rw-r--r--   0        0        0      225 2023-03-29 02:52:04.410651 binarylane_cli-0.15.3/lib/binarylane/models/change_advanced_features_type.py
--rw-r--r--   0        0        0     2635 2023-03-29 02:52:06.970666 binarylane_cli-0.15.3/lib/binarylane/models/change_advanced_firewall_rules.py
--rw-r--r--   0        0        0      242 2023-03-29 02:52:04.474651 binarylane_cli-0.15.3/lib/binarylane/models/change_advanced_firewall_rules_type.py
--rw-r--r--   0        0        0     3061 2023-03-29 02:52:06.922665 binarylane_cli-0.15.3/lib/binarylane/models/change_backup_schedule.py
--rw-r--r--   0        0        0      219 2023-03-29 02:52:04.542652 binarylane_cli-0.15.3/lib/binarylane/models/change_backup_schedule_type.py
--rw-r--r--   0        0        0     2953 2023-03-29 02:52:06.926665 binarylane_cli-0.15.3/lib/binarylane/models/change_image.py
--rw-r--r--   0        0        0     1743 2023-03-29 02:52:06.902665 binarylane_cli-0.15.3/lib/binarylane/models/change_ipv_6.py
--rw-r--r--   0        0        0     2279 2023-03-29 02:52:06.950666 binarylane_cli-0.15.3/lib/binarylane/models/change_ipv_6_reverse_nameservers.py
--rw-r--r--   0        0        0      245 2023-03-29 02:52:04.442651 binarylane_cli-0.15.3/lib/binarylane/models/change_ipv_6_reverse_nameservers_type.py
--rw-r--r--   0        0        0      187 2023-03-29 02:52:04.294650 binarylane_cli-0.15.3/lib/binarylane/models/change_ipv_6_type.py
--rw-r--r--   0        0        0     1734 2023-03-29 02:52:06.990666 binarylane_cli-0.15.3/lib/binarylane/models/change_kernel.py
--rw-r--r--   0        0        0      193 2023-03-29 02:52:04.522652 binarylane_cli-0.15.3/lib/binarylane/models/change_kernel_type.py
--rw-r--r--   0        0        0     1859 2023-03-29 02:52:06.894665 binarylane_cli-0.15.3/lib/binarylane/models/change_licenses.py
--rw-r--r--   0        0        0     2560 2023-03-29 02:52:07.002666 binarylane_cli-0.15.3/lib/binarylane/models/change_manage_offsite_backup_copies.py
--rw-r--r--   0        0        0      256 2023-03-29 02:52:04.526651 binarylane_cli-0.15.3/lib/binarylane/models/change_manage_offsite_backup_copies_type.py
--rw-r--r--   0        0        0     1976 2023-03-29 02:52:06.898665 binarylane_cli-0.15.3/lib/binarylane/models/change_network.py
--rw-r--r--   0        0        0      196 2023-03-29 02:52:04.338651 binarylane_cli-0.15.3/lib/binarylane/models/change_network_type.py
--rw-r--r--   0        0        0     2470 2023-03-29 02:52:06.998666 binarylane_cli-0.15.3/lib/binarylane/models/change_offsite_backup_location.py
--rw-r--r--   0        0        0      242 2023-03-29 02:52:04.490651 binarylane_cli-0.15.3/lib/binarylane/models/change_offsite_backup_location_type.py
--rw-r--r--   0        0        0     2132 2023-03-29 02:52:06.902665 binarylane_cli-0.15.3/lib/binarylane/models/change_partner.py
--rw-r--r--   0        0        0      196 2023-03-29 02:52:04.522652 binarylane_cli-0.15.3/lib/binarylane/models/change_partner_type.py
--rw-r--r--   0        0        0     1835 2023-03-29 02:52:06.854665 binarylane_cli-0.15.3/lib/binarylane/models/change_port_blocking.py
--rw-r--r--   0        0        0      213 2023-03-29 02:52:04.534652 binarylane_cli-0.15.3/lib/binarylane/models/change_port_blocking_type.py
--rw-r--r--   0        0        0     2322 2023-03-29 02:52:06.966666 binarylane_cli-0.15.3/lib/binarylane/models/change_reverse_name.py
--rw-r--r--   0        0        0      210 2023-03-29 02:52:04.538652 binarylane_cli-0.15.3/lib/binarylane/models/change_reverse_name_type.py
--rw-r--r--   0        0        0     2095 2023-03-29 02:52:06.882665 binarylane_cli-0.15.3/lib/binarylane/models/change_separate_private_network_interface.py
--rw-r--r--   0        0        0      274 2023-03-29 02:52:04.430651 binarylane_cli-0.15.3/lib/binarylane/models/change_separate_private_network_interface_type.py
--rw-r--r--   0        0        0     7820 2023-03-29 02:52:06.870665 binarylane_cli-0.15.3/lib/binarylane/models/change_size_options_request.py
--rw-r--r--   0        0        0     2052 2023-03-29 02:52:06.918665 binarylane_cli-0.15.3/lib/binarylane/models/change_source_and_destination_check.py
--rw-r--r--   0        0        0      256 2023-03-29 02:52:04.386651 binarylane_cli-0.15.3/lib/binarylane/models/change_source_and_destination_check_type.py
--rw-r--r--   0        0        0     2515 2023-03-29 02:52:07.010666 binarylane_cli-0.15.3/lib/binarylane/models/change_threshold_alerts.py
--rw-r--r--   0        0        0      222 2023-03-29 02:52:04.494651 binarylane_cli-0.15.3/lib/binarylane/models/change_threshold_alerts_type.py
--rw-r--r--   0        0        0     2281 2023-03-29 02:52:06.950666 binarylane_cli-0.15.3/lib/binarylane/models/change_vpc_ipv_4.py
--rw-r--r--   0        0        0      198 2023-03-29 02:52:04.446651 binarylane_cli-0.15.3/lib/binarylane/models/change_vpc_ipv_4_type.py
--rw-r--r--   0        0        0     2306 2023-03-29 02:52:05.862659 binarylane_cli-0.15.3/lib/binarylane/models/charge_information.py
--rw-r--r--   0        0        0     2752 2023-03-29 02:52:06.846665 binarylane_cli-0.15.3/lib/binarylane/models/clone_using_backup.py
--rw-r--r--   0        0        0      207 2023-03-29 02:52:04.350651 binarylane_cli-0.15.3/lib/binarylane/models/clone_using_backup_type.py
--rw-r--r--   0        0        0     2354 2023-03-29 02:52:05.886659 binarylane_cli-0.15.3/lib/binarylane/models/console.py
--rw-r--r--   0        0        0     1524 2023-03-29 02:52:06.998666 binarylane_cli-0.15.3/lib/binarylane/models/console_response.py
--rw-r--r--   0        0        0     4825 2023-03-29 02:52:06.838665 binarylane_cli-0.15.3/lib/binarylane/models/create_load_balancer_request.py
--rw-r--r--   0        0        0     1933 2023-03-29 02:52:06.946666 binarylane_cli-0.15.3/lib/binarylane/models/create_load_balancer_response.py
--rw-r--r--   0        0        0     8213 2023-03-29 02:52:06.974666 binarylane_cli-0.15.3/lib/binarylane/models/create_server_request.py
--rw-r--r--   0        0        0     1799 2023-03-29 02:52:06.966666 binarylane_cli-0.15.3/lib/binarylane/models/create_server_response.py
--rw-r--r--   0        0        0     3204 2023-03-29 02:52:06.974666 binarylane_cli-0.15.3/lib/binarylane/models/create_vpc_request.py
--rw-r--r--   0        0        0     1571 2023-03-29 02:52:05.914660 binarylane_cli-0.15.3/lib/binarylane/models/current_server_alerts_response.py
--rw-r--r--   0        0        0      295 2023-03-29 02:52:04.366651 binarylane_cli-0.15.3/lib/binarylane/models/data_interval.py
--rw-r--r--   0        0        0     3440 2023-03-29 02:52:05.910660 binarylane_cli-0.15.3/lib/binarylane/models/data_usage.py
--rw-r--r--   0        0        0     1578 2023-03-29 02:52:06.978666 binarylane_cli-0.15.3/lib/binarylane/models/data_usage_response.py
--rw-r--r--   0        0        0     2931 2023-03-29 02:52:06.950666 binarylane_cli-0.15.3/lib/binarylane/models/data_usages_response.py
--rw-r--r--   0        0        0     1769 2023-03-29 02:52:06.898665 binarylane_cli-0.15.3/lib/binarylane/models/delete_disk.py
--rw-r--r--   0        0        0      187 2023-03-29 02:52:04.442651 binarylane_cli-0.15.3/lib/binarylane/models/delete_disk_type.py
--rw-r--r--   0        0        0     1553 2023-03-29 02:52:06.986666 binarylane_cli-0.15.3/lib/binarylane/models/detach_backup.py
--rw-r--r--   0        0        0      193 2023-03-29 02:52:04.546652 binarylane_cli-0.15.3/lib/binarylane/models/detach_backup_type.py
--rw-r--r--   0        0        0     1571 2023-03-29 02:52:06.862665 binarylane_cli-0.15.3/lib/binarylane/models/disable_backups.py
--rw-r--r--   0        0        0      199 2023-03-29 02:52:04.366651 binarylane_cli-0.15.3/lib/binarylane/models/disable_backups_type.py
--rw-r--r--   0        0        0     1562 2023-03-29 02:52:06.886665 binarylane_cli-0.15.3/lib/binarylane/models/disable_selinux.py
--rw-r--r--   0        0        0      199 2023-03-29 02:52:04.522652 binarylane_cli-0.15.3/lib/binarylane/models/disable_selinux_type.py
--rw-r--r--   0        0        0     2247 2023-03-29 02:52:06.878665 binarylane_cli-0.15.3/lib/binarylane/models/disk.py
--rw-r--r--   0        0        0      242 2023-03-29 02:52:04.554652 binarylane_cli-0.15.3/lib/binarylane/models/distribution_feature.py
--rw-r--r--   0        0        0     3740 2023-03-29 02:52:06.938665 binarylane_cli-0.15.3/lib/binarylane/models/distribution_info.py
--rw-r--r--   0        0        0     4076 2023-03-29 02:52:07.002666 binarylane_cli-0.15.3/lib/binarylane/models/distribution_surcharges.py
--rw-r--r--   0        0        0     2620 2023-03-29 02:52:06.946666 binarylane_cli-0.15.3/lib/binarylane/models/domain.py
--rw-r--r--   0        0        0     4753 2023-03-29 02:52:07.010666 binarylane_cli-0.15.3/lib/binarylane/models/domain_record.py
--rw-r--r--   0        0        0     4733 2023-03-29 02:52:06.934666 binarylane_cli-0.15.3/lib/binarylane/models/domain_record_request.py
--rw-r--r--   0        0        0     1638 2023-03-29 02:52:06.878665 binarylane_cli-0.15.3/lib/binarylane/models/domain_record_response.py
--rw-r--r--   0        0        0      299 2023-03-29 02:52:04.334650 binarylane_cli-0.15.3/lib/binarylane/models/domain_record_type.py
--rw-r--r--   0        0        0     3027 2023-03-29 02:52:06.862665 binarylane_cli-0.15.3/lib/binarylane/models/domain_records_response.py
--rw-r--r--   0        0        0     1902 2023-03-29 02:52:06.998666 binarylane_cli-0.15.3/lib/binarylane/models/domain_request.py
--rw-r--r--   0        0        0     1504 2023-03-29 02:52:06.854665 binarylane_cli-0.15.3/lib/binarylane/models/domain_response.py
--rw-r--r--   0        0        0     2809 2023-03-29 02:52:06.926665 binarylane_cli-0.15.3/lib/binarylane/models/domains_response.py
--rw-r--r--   0        0        0     1570 2023-03-29 02:52:06.862665 binarylane_cli-0.15.3/lib/binarylane/models/enable_backups.py
--rw-r--r--   0        0        0      196 2023-03-29 02:52:04.458651 binarylane_cli-0.15.3/lib/binarylane/models/enable_backups_type.py
--rw-r--r--   0        0        0     1521 2023-03-29 02:52:06.954666 binarylane_cli-0.15.3/lib/binarylane/models/enable_ipv_6.py
--rw-r--r--   0        0        0      187 2023-03-29 02:52:04.390651 binarylane_cli-0.15.3/lib/binarylane/models/enable_ipv_6_type.py
--rw-r--r--   0        0        0     1736 2023-03-29 02:52:06.014660 binarylane_cli-0.15.3/lib/binarylane/models/failover_ips_request.py
--rw-r--r--   0        0        0     2551 2023-03-29 02:52:06.838665 binarylane_cli-0.15.3/lib/binarylane/models/failover_ips_response.py
--rw-r--r--   0        0        0     1778 2023-03-29 02:52:06.838665 binarylane_cli-0.15.3/lib/binarylane/models/forwarding_rule.py
--rw-r--r--   0        0        0     2188 2023-03-29 02:52:06.886665 binarylane_cli-0.15.3/lib/binarylane/models/forwarding_rules_request.py
--rw-r--r--   0        0        0     2366 2023-03-29 02:52:07.006666 binarylane_cli-0.15.3/lib/binarylane/models/health_check.py
--rw-r--r--   0        0        0      216 2023-03-29 02:52:04.410651 binarylane_cli-0.15.3/lib/binarylane/models/health_check_protocol.py
--rw-r--r--   0        0        0     2282 2023-03-29 02:52:06.938665 binarylane_cli-0.15.3/lib/binarylane/models/host.py
--rw-r--r--   0        0        0    10687 2023-03-29 02:52:06.886665 binarylane_cli-0.15.3/lib/binarylane/models/image.py
--rw-r--r--   0        0        0     2023 2023-03-29 02:52:06.086660 binarylane_cli-0.15.3/lib/binarylane/models/image_disk_download.py
--rw-r--r--   0        0        0     2397 2023-03-29 02:52:06.878665 binarylane_cli-0.15.3/lib/binarylane/models/image_download.py
--rw-r--r--   0        0        0     1558 2023-03-29 02:52:06.986666 binarylane_cli-0.15.3/lib/binarylane/models/image_download_response.py
--rw-r--r--   0        0        0     3897 2023-03-29 02:52:06.930665 binarylane_cli-0.15.3/lib/binarylane/models/image_options.py
--rw-r--r--   0        0        0      211 2023-03-29 02:52:04.294650 binarylane_cli-0.15.3/lib/binarylane/models/image_query_type.py
--rw-r--r--   0        0        0     2106 2023-03-29 02:52:06.970666 binarylane_cli-0.15.3/lib/binarylane/models/image_request.py
--rw-r--r--   0        0        0     1484 2023-03-29 02:52:06.942665 binarylane_cli-0.15.3/lib/binarylane/models/image_response.py
--rw-r--r--   0        0        0      244 2023-03-29 02:52:04.526651 binarylane_cli-0.15.3/lib/binarylane/models/image_status.py
--rw-r--r--   0        0        0      220 2023-03-29 02:52:04.506651 binarylane_cli-0.15.3/lib/binarylane/models/image_type.py
--rw-r--r--   0        0        0     2777 2023-03-29 02:52:06.878665 binarylane_cli-0.15.3/lib/binarylane/models/images_response.py
--rw-r--r--   0        0        0     6154 2023-03-29 02:52:06.966666 binarylane_cli-0.15.3/lib/binarylane/models/invoice.py
--rw-r--r--   0        0        0     2398 2023-03-29 02:52:06.054660 binarylane_cli-0.15.3/lib/binarylane/models/invoice_line_item.py
--rw-r--r--   0        0        0     1524 2023-03-29 02:52:06.890665 binarylane_cli-0.15.3/lib/binarylane/models/invoice_response.py
--rw-r--r--   0        0        0     2841 2023-03-29 02:52:06.874665 binarylane_cli-0.15.3/lib/binarylane/models/invoices_response.py
--rw-r--r--   0        0        0     1511 2023-03-29 02:52:06.966666 binarylane_cli-0.15.3/lib/binarylane/models/is_running.py
--rw-r--r--   0        0        0      184 2023-03-29 02:52:04.454651 binarylane_cli-0.15.3/lib/binarylane/models/is_running_type.py
--rw-r--r--   0        0        0     1981 2023-03-29 02:52:06.890665 binarylane_cli-0.15.3/lib/binarylane/models/kernel.py
--rw-r--r--   0        0        0     2809 2023-03-29 02:52:06.914665 binarylane_cli-0.15.3/lib/binarylane/models/kernels_response.py
--rw-r--r--   0        0        0     1651 2023-03-29 02:52:06.078661 binarylane_cli-0.15.3/lib/binarylane/models/license_.py
--rw-r--r--   0        0        0     1854 2023-03-29 02:52:06.934666 binarylane_cli-0.15.3/lib/binarylane/models/licensed_software.py
--rw-r--r--   0        0        0     3133 2023-03-29 02:52:06.990666 binarylane_cli-0.15.3/lib/binarylane/models/licensed_softwares_response.py
--rw-r--r--   0        0        0     1554 2023-03-29 02:52:06.910665 binarylane_cli-0.15.3/lib/binarylane/models/links.py
--rw-r--r--   0        0        0     5266 2023-03-29 02:52:06.914665 binarylane_cli-0.15.3/lib/binarylane/models/load_balancer.py
--rw-r--r--   0        0        0     2768 2023-03-29 02:52:06.954666 binarylane_cli-0.15.3/lib/binarylane/models/load_balancer_availability_option.py
--rw-r--r--   0        0        0     2645 2023-03-29 02:52:06.874665 binarylane_cli-0.15.3/lib/binarylane/models/load_balancer_availability_response.py
--rw-r--r--   0        0        0     1638 2023-03-29 02:52:06.858665 binarylane_cli-0.15.3/lib/binarylane/models/load_balancer_response.py
--rw-r--r--   0        0        0      203 2023-03-29 02:52:04.374651 binarylane_cli-0.15.3/lib/binarylane/models/load_balancer_rule_protocol.py
--rw-r--r--   0        0        0      221 2023-03-29 02:52:04.550652 binarylane_cli-0.15.3/lib/binarylane/models/load_balancer_status.py
--rw-r--r--   0        0        0     3027 2023-03-29 02:52:06.894665 binarylane_cli-0.15.3/lib/binarylane/models/load_balancers_response.py
--rw-r--r--   0        0        0     1623 2023-03-29 02:52:06.122661 binarylane_cli-0.15.3/lib/binarylane/models/local_nameservers_response.py
--rw-r--r--   0        0        0     1488 2023-03-29 02:52:06.126661 binarylane_cli-0.15.3/lib/binarylane/models/meta.py
--rw-r--r--   0        0        0     3834 2023-03-29 02:52:06.962666 binarylane_cli-0.15.3/lib/binarylane/models/network.py
--rw-r--r--   0        0        0      198 2023-03-29 02:52:04.534652 binarylane_cli-0.15.3/lib/binarylane/models/network_type.py
--rw-r--r--   0        0        0     5171 2023-03-29 02:52:06.874665 binarylane_cli-0.15.3/lib/binarylane/models/networks.py
--rw-r--r--   0        0        0     3058 2023-03-29 02:52:06.154661 binarylane_cli-0.15.3/lib/binarylane/models/offsite_backup_frequency_cost.py
--rw-r--r--   0        0        0     3221 2023-03-29 02:52:06.930665 binarylane_cli-0.15.3/lib/binarylane/models/offsite_backup_settings.py
--rw-r--r--   0        0        0     2550 2023-03-29 02:52:06.982666 binarylane_cli-0.15.3/lib/binarylane/models/pages.py
--rw-r--r--   0        0        0      293 2023-03-29 02:52:04.550652 binarylane_cli-0.15.3/lib/binarylane/models/password_recovery_type.py
--rw-r--r--   0        0        0     2987 2023-03-29 02:52:06.994666 binarylane_cli-0.15.3/lib/binarylane/models/password_reset.py
--rw-r--r--   0        0        0      196 2023-03-29 02:52:04.358651 binarylane_cli-0.15.3/lib/binarylane/models/password_reset_type.py
--rw-r--r--   0        0        0     2919 2023-03-29 02:52:06.854665 binarylane_cli-0.15.3/lib/binarylane/models/patch_vpc_request.py
--rw-r--r--   0        0        0      208 2023-03-29 02:52:04.410651 binarylane_cli-0.15.3/lib/binarylane/models/payment_method.py
--rw-r--r--   0        0        0     2463 2023-03-29 02:52:06.914665 binarylane_cli-0.15.3/lib/binarylane/models/period.py
--rw-r--r--   0        0        0     1453 2023-03-29 02:52:06.978666 binarylane_cli-0.15.3/lib/binarylane/models/ping.py
--rw-r--r--   0        0        0      167 2023-03-29 02:52:04.486651 binarylane_cli-0.15.3/lib/binarylane/models/ping_type.py
--rw-r--r--   0        0        0     1523 2023-03-29 02:52:06.902665 binarylane_cli-0.15.3/lib/binarylane/models/power_cycle.py
--rw-r--r--   0        0        0      187 2023-03-29 02:52:04.538652 binarylane_cli-0.15.3/lib/binarylane/models/power_cycle_type.py
--rw-r--r--   0        0        0     1491 2023-03-29 02:52:06.918665 binarylane_cli-0.15.3/lib/binarylane/models/power_off.py
--rw-r--r--   0        0        0      181 2023-03-29 02:52:04.326650 binarylane_cli-0.15.3/lib/binarylane/models/power_off_type.py
--rw-r--r--   0        0        0     1480 2023-03-29 02:52:06.846665 binarylane_cli-0.15.3/lib/binarylane/models/power_on.py
--rw-r--r--   0        0        0      178 2023-03-29 02:52:04.518652 binarylane_cli-0.15.3/lib/binarylane/models/power_on_type.py
--rw-r--r--   0        0        0     2523 2023-03-29 02:52:06.914665 binarylane_cli-0.15.3/lib/binarylane/models/problem_details.py
--rw-r--r--   0        0        0     1559 2023-03-29 02:52:06.194661 binarylane_cli-0.15.3/lib/binarylane/models/proceed_request.py
--rw-r--r--   0        0        0     1994 2023-03-29 02:52:06.982666 binarylane_cli-0.15.3/lib/binarylane/models/processor_model.py
--rw-r--r--   0        0        0     1482 2023-03-29 02:52:06.846665 binarylane_cli-0.15.3/lib/binarylane/models/reboot.py
--rw-r--r--   0        0        0      173 2023-03-29 02:52:04.322651 binarylane_cli-0.15.3/lib/binarylane/models/reboot_type.py
--rw-r--r--   0        0        0     3251 2023-03-29 02:52:06.994666 binarylane_cli-0.15.3/lib/binarylane/models/rebuild.py
--rw-r--r--   0        0        0      176 2023-03-29 02:52:04.366651 binarylane_cli-0.15.3/lib/binarylane/models/rebuild_type.py
--rw-r--r--   0        0        0     2647 2023-03-29 02:52:06.226661 binarylane_cli-0.15.3/lib/binarylane/models/region.py
--rw-r--r--   0        0        0     2809 2023-03-29 02:52:06.970666 binarylane_cli-0.15.3/lib/binarylane/models/regions_response.py
--rw-r--r--   0        0        0     1671 2023-03-29 02:52:06.938665 binarylane_cli-0.15.3/lib/binarylane/models/rename.py
--rw-r--r--   0        0        0      173 2023-03-29 02:52:04.490651 binarylane_cli-0.15.3/lib/binarylane/models/rename_type.py
--rw-r--r--   0        0        0     6138 2023-03-29 02:52:06.930665 binarylane_cli-0.15.3/lib/binarylane/models/resize.py
--rw-r--r--   0        0        0     2158 2023-03-29 02:52:07.002666 binarylane_cli-0.15.3/lib/binarylane/models/resize_disk.py
--rw-r--r--   0        0        0      187 2023-03-29 02:52:04.510651 binarylane_cli-0.15.3/lib/binarylane/models/resize_disk_type.py
--rw-r--r--   0        0        0      173 2023-03-29 02:52:04.434651 binarylane_cli-0.15.3/lib/binarylane/models/resize_type.py
--rw-r--r--   0        0        0      325 2023-03-29 02:52:04.410651 binarylane_cli-0.15.3/lib/binarylane/models/resource_type.py
--rw-r--r--   0        0        0     1931 2023-03-29 02:52:06.986666 binarylane_cli-0.15.3/lib/binarylane/models/restore.py
--rw-r--r--   0        0        0      176 2023-03-29 02:52:04.350651 binarylane_cli-0.15.3/lib/binarylane/models/restore_type.py
--rw-r--r--   0        0        0     2659 2023-03-29 02:52:06.954666 binarylane_cli-0.15.3/lib/binarylane/models/reverse_name_servers_response.py
--rw-r--r--   0        0        0     1815 2023-03-29 02:52:06.218661 binarylane_cli-0.15.3/lib/binarylane/models/reverse_nameservers_request.py
--rw-r--r--   0        0        0     2175 2023-03-29 02:52:06.942665 binarylane_cli-0.15.3/lib/binarylane/models/route_entry.py
--rw-r--r--   0        0        0     2213 2023-03-29 02:52:06.906665 binarylane_cli-0.15.3/lib/binarylane/models/route_entry_request.py
--rw-r--r--   0        0        0     4965 2023-03-29 02:52:06.278662 binarylane_cli-0.15.3/lib/binarylane/models/sample.py
--rw-r--r--   0        0        0     2938 2023-03-29 02:52:06.858665 binarylane_cli-0.15.3/lib/binarylane/models/sample_set.py
--rw-r--r--   0        0        0     2078 2023-03-29 02:52:06.866665 binarylane_cli-0.15.3/lib/binarylane/models/sample_set_response.py
--rw-r--r--   0        0        0     2931 2023-03-29 02:52:06.950666 binarylane_cli-0.15.3/lib/binarylane/models/sample_sets_response.py
--rw-r--r--   0        0        0     3850 2023-03-29 02:52:06.286662 binarylane_cli-0.15.3/lib/binarylane/models/selected_size_options.py
--rw-r--r--   0        0        0    13805 2023-03-29 02:52:06.958666 binarylane_cli-0.15.3/lib/binarylane/models/server.py
--rw-r--r--   0        0        0     1535 2023-03-29 02:52:06.266662 binarylane_cli-0.15.3/lib/binarylane/models/server_ids_request.py
--rw-r--r--   0        0        0     1504 2023-03-29 02:52:06.882665 binarylane_cli-0.15.3/lib/binarylane/models/server_response.py
--rw-r--r--   0        0        0      231 2023-03-29 02:52:04.358651 binarylane_cli-0.15.3/lib/binarylane/models/server_status.py
--rw-r--r--   0        0        0     2809 2023-03-29 02:52:06.978666 binarylane_cli-0.15.3/lib/binarylane/models/servers_response.py
--rw-r--r--   0        0        0     1504 2023-03-29 02:52:06.982666 binarylane_cli-0.15.3/lib/binarylane/models/shutdown.py
--rw-r--r--   0        0        0      179 2023-03-29 02:52:04.434651 binarylane_cli-0.15.3/lib/binarylane/models/shutdown_type.py
--rw-r--r--   0        0        0     7284 2023-03-29 02:52:06.842665 binarylane_cli-0.15.3/lib/binarylane/models/size.py
--rw-r--r--   0        0        0     9209 2023-03-29 02:52:06.866665 binarylane_cli-0.15.3/lib/binarylane/models/size_options.py
--rw-r--r--   0        0        0     6754 2023-03-29 02:52:06.918665 binarylane_cli-0.15.3/lib/binarylane/models/size_options_request.py
--rw-r--r--   0        0        0     2055 2023-03-29 02:52:06.982666 binarylane_cli-0.15.3/lib/binarylane/models/size_type.py
--rw-r--r--   0        0        0     2745 2023-03-29 02:52:06.870665 binarylane_cli-0.15.3/lib/binarylane/models/sizes_response.py
--rw-r--r--   0        0        0     2858 2023-03-29 02:52:06.986666 binarylane_cli-0.15.3/lib/binarylane/models/snapshots_response.py
--rw-r--r--   0        0        0     4421 2023-03-29 02:52:06.922665 binarylane_cli-0.15.3/lib/binarylane/models/software.py
--rw-r--r--   0        0        0     1544 2023-03-29 02:52:06.998666 binarylane_cli-0.15.3/lib/binarylane/models/software_response.py
--rw-r--r--   0        0        0     2851 2023-03-29 02:52:06.994666 binarylane_cli-0.15.3/lib/binarylane/models/softwares_response.py
--rw-r--r--   0        0        0     2548 2023-03-29 02:52:06.934666 binarylane_cli-0.15.3/lib/binarylane/models/ssh_key.py
--rw-r--r--   0        0        0     2164 2023-03-29 02:52:06.842665 binarylane_cli-0.15.3/lib/binarylane/models/ssh_key_request.py
--rw-r--r--   0        0        0     1518 2023-03-29 02:52:06.890665 binarylane_cli-0.15.3/lib/binarylane/models/ssh_key_response.py
--rw-r--r--   0        0        0     2835 2023-03-29 02:52:06.838665 binarylane_cli-0.15.3/lib/binarylane/models/ssh_keys_response.py
--rw-r--r--   0        0        0     3772 2023-03-29 02:52:06.878665 binarylane_cli-0.15.3/lib/binarylane/models/take_backup.py
--rw-r--r--   0        0        0      187 2023-03-29 02:52:04.394651 binarylane_cli-0.15.3/lib/binarylane/models/take_backup_type.py
--rw-r--r--   0        0        0     2538 2023-03-29 02:52:06.926665 binarylane_cli-0.15.3/lib/binarylane/models/tax_code.py
--rw-r--r--   0        0        0      192 2023-03-29 02:52:04.410651 binarylane_cli-0.15.3/lib/binarylane/models/tax_code_type.py
--rw-r--r--   0        0        0     6585 2023-03-29 02:52:06.946666 binarylane_cli-0.15.3/lib/binarylane/models/threshold_alert.py
--rw-r--r--   0        0        0     4090 2023-03-29 02:52:06.842665 binarylane_cli-0.15.3/lib/binarylane/models/threshold_alert_request.py
--rw-r--r--   0        0        0      413 2023-03-29 02:52:04.474651 binarylane_cli-0.15.3/lib/binarylane/models/threshold_alert_type.py
--rw-r--r--   0        0        0     2089 2023-03-29 02:52:06.978666 binarylane_cli-0.15.3/lib/binarylane/models/threshold_alerts_response.py
--rw-r--r--   0        0        0     1504 2023-03-29 02:52:06.882665 binarylane_cli-0.15.3/lib/binarylane/models/uncancel.py
--rw-r--r--   0        0        0      179 2023-03-29 02:52:04.478651 binarylane_cli-0.15.3/lib/binarylane/models/uncancel_type.py
--rw-r--r--   0        0        0     1905 2023-03-29 02:52:06.850665 binarylane_cli-0.15.3/lib/binarylane/models/unpaid_failed_invoices_response.py
--rw-r--r--   0        0        0     4520 2023-03-29 02:52:06.946666 binarylane_cli-0.15.3/lib/binarylane/models/update_load_balancer_request.py
--rw-r--r--   0        0        0     2416 2023-03-29 02:52:06.942665 binarylane_cli-0.15.3/lib/binarylane/models/update_load_balancer_response.py
--rw-r--r--   0        0        0     2046 2023-03-29 02:52:06.990666 binarylane_cli-0.15.3/lib/binarylane/models/update_ssh_key_request.py
--rw-r--r--   0        0        0     2751 2023-03-29 02:52:06.926665 binarylane_cli-0.15.3/lib/binarylane/models/update_vpc_request.py
--rw-r--r--   0        0        0     3765 2023-03-29 02:52:06.902665 binarylane_cli-0.15.3/lib/binarylane/models/upload_image_request.py
--rw-r--r--   0        0        0     1477 2023-03-29 02:52:06.882665 binarylane_cli-0.15.3/lib/binarylane/models/uptime.py
--rw-r--r--   0        0        0      173 2023-03-29 02:52:04.498651 binarylane_cli-0.15.3/lib/binarylane/models/uptime_type.py
--rw-r--r--   0        0        0     1596 2023-03-29 02:52:06.974666 binarylane_cli-0.15.3/lib/binarylane/models/user_data.py
--rw-r--r--   0        0        0     2097 2023-03-29 02:52:06.946666 binarylane_cli-0.15.3/lib/binarylane/models/user_interaction_required.py
--rw-r--r--   0        0        0      280 2023-03-29 02:52:04.402651 binarylane_cli-0.15.3/lib/binarylane/models/user_interaction_type.py
--rw-r--r--   0        0        0     3139 2023-03-29 02:52:06.998666 binarylane_cli-0.15.3/lib/binarylane/models/validation_problem_details.py
--rw-r--r--   0        0        0     1596 2023-03-29 02:52:06.442663 binarylane_cli-0.15.3/lib/binarylane/models/validation_problem_details_errors.py
--rw-r--r--   0        0        0      266 2023-03-29 02:52:04.502652 binarylane_cli-0.15.3/lib/binarylane/models/video_device.py
--rw-r--r--   0        0        0      420 2023-03-29 02:52:04.438651 binarylane_cli-0.15.3/lib/binarylane/models/vm_machine_type.py
--rw-r--r--   0        0        0     2533 2023-03-29 02:52:06.846665 binarylane_cli-0.15.3/lib/binarylane/models/vpc.py
--rw-r--r--   0        0        0     3260 2023-03-29 02:52:06.930665 binarylane_cli-0.15.3/lib/binarylane/models/vpc_member.py
--rw-r--r--   0        0        0     2843 2023-03-29 02:52:06.962666 binarylane_cli-0.15.3/lib/binarylane/models/vpc_members_response.py
--rw-r--r--   0        0        0     1444 2023-03-29 02:52:06.906665 binarylane_cli-0.15.3/lib/binarylane/models/vpc_response.py
--rw-r--r--   0        0        0     2713 2023-03-29 02:52:06.910665 binarylane_cli-0.15.3/lib/binarylane/models/vpcs_response.py
--rw-r--r--   0        0        0       25 2023-03-29 02:52:03.074643 binarylane_cli-0.15.3/lib/binarylane/py.typed
--rw-r--r--   0        0        0     1028 2023-03-29 02:52:06.450663 binarylane_cli-0.15.3/lib/binarylane/types.py
--rw-r--r--   0        0        0     2401 2023-03-29 03:09:51.205163 binarylane_cli-0.15.3/pyproject.toml
--rw-r--r--   0        0        0     1891 2023-03-15 04:49:44.258009 binarylane_cli-0.15.3/src/binarylane/config/__init__.py
--rw-r--r--   0        0        0     4083 2023-03-15 04:49:44.258009 binarylane_cli-0.15.3/src/binarylane/config/options.py
--rw-r--r--   0        0        0     1501 2023-03-15 04:49:44.258009 binarylane_cli-0.15.3/src/binarylane/config/repository.py
--rw-r--r--   0        0        0     4802 2023-03-15 04:49:44.258009 binarylane_cli-0.15.3/src/binarylane/config/sources.py
--rw-r--r--   0        0        0        0 2023-02-07 09:32:33.869646 binarylane_cli-0.15.3/src/binarylane/console/__init__.py
--rw-r--r--   0        0        0      619 2023-03-15 04:49:44.258009 binarylane_cli-0.15.3/src/binarylane/console/__main__.py
--rw-r--r--   0        0        0     5831 2023-03-21 04:41:01.412051 binarylane_cli-0.15.3/src/binarylane/console/app.py
--rw-r--r--   0        0        0      408 2023-03-15 04:49:44.258009 binarylane_cli-0.15.3/src/binarylane/console/commands/__init__.py
--rw-r--r--   0        0        0    18051 2023-03-29 02:52:09.754682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/__init__.py
--rw-r--r--   0        0        0     1733 2023-03-29 03:05:42.879441 binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_account_keys_key_id.py
--rw-r--r--   0        0        0     1723 2023-03-29 02:52:09.498680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_domains_domain_name.py
--rw-r--r--   0        0        0     2159 2023-03-29 02:52:09.482680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_domains_domain_name_records_record_id.py
--rw-r--r--   0        0        0     1800 2023-03-29 02:52:09.558681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id.py
--rw-r--r--   0        0        0     3254 2023-03-29 02:52:09.574681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id_forwarding_rules.py
--rw-r--r--   0        0        0     2605 2023-03-29 02:52:09.590681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id_servers.py
--rw-r--r--   0        0        0     2117 2023-03-29 02:52:09.766682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_servers_server_id.py
--rw-r--r--   0        0        0     1698 2023-03-29 02:52:09.822682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_vpcs_vpc_id.py
--rw-r--r--   0        0        0     1231 2023-03-29 02:52:09.450680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_account.py
--rw-r--r--   0        0        0     2992 2023-03-29 02:52:09.554681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_account_keys.py
--rw-r--r--   0        0        0     1811 2023-03-29 03:05:42.879441 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_account_keys_key_id.py
--rw-r--r--   0        0        0     4271 2023-03-29 02:52:09.486680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_actions.py
--rw-r--r--   0        0        0     1780 2023-03-29 02:52:09.458680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_actions_action_id.py
--rw-r--r--   0        0        0     1251 2023-03-29 02:52:09.446680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_customers_my_balance.py
--rw-r--r--   0        0        0     4045 2023-03-29 02:52:09.486680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_customers_my_invoices.py
--rw-r--r--   0        0        0     1829 2023-03-29 02:52:09.458680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_customers_my_invoices_invoice_id.py
--rw-r--r--   0        0        0     3363 2023-03-29 02:52:09.482680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_customers_my_unpaid_payment_failed_invoices.py
--rw-r--r--   0        0        0     3495 2023-03-29 02:52:09.486680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_data_usages_current.py
--rw-r--r--   0        0        0     1819 2023-03-29 02:52:09.470680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_data_usages_server_id_current.py
--rw-r--r--   0        0        0     3332 2023-03-29 02:52:09.494680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_domains.py
--rw-r--r--   0        0        0     1800 2023-03-29 02:52:09.466680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_domains_domain_name.py
--rw-r--r--   0        0        0     6129 2023-03-29 02:52:09.566681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_domains_domain_name_records.py
--rw-r--r--   0        0        0     2267 2023-03-29 02:52:09.486680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_domains_domain_name_records_record_id.py
--rw-r--r--   0        0        0     1290 2023-03-29 02:52:09.470680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_domains_nameservers.py
--rw-r--r--   0        0        0     2634 2023-03-29 02:52:09.526680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_failover_ips_server_id.py
--rw-r--r--   0        0        0     2655 2023-03-29 02:52:09.522680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_failover_ips_server_id_available.py
--rw-r--r--   0        0        0     6702 2023-03-29 02:52:09.578681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_images.py
--rw-r--r--   0        0        0     1824 2023-03-29 02:52:09.530681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_images_image_id_download.py
--rw-r--r--   0        0        0     1905 2023-03-29 03:05:42.879441 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_images_image_id_or_slug.py
--rw-r--r--   0        0        0     3726 2023-03-29 02:52:09.582681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_load_balancers.py
--rw-r--r--   0        0        0     2223 2023-03-29 02:52:09.566681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_load_balancers_availability.py
--rw-r--r--   0        0        0     1908 2023-03-29 02:52:09.558681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_load_balancers_load_balancer_id.py
--rw-r--r--   0        0        0     2908 2023-03-29 02:52:09.602681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_regions.py
--rw-r--r--   0        0        0     2276 2023-03-29 02:52:09.590681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_reverse_names_ipv6.py
--rw-r--r--   0        0        0     5643 2023-03-29 02:52:09.666681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_samplesets_server_id.py
--rw-r--r--   0        0        0     2479 2023-03-29 02:52:09.610681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_samplesets_server_id_latest.py
--rw-r--r--   0        0        0     6184 2023-03-29 02:52:09.810682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers.py
--rw-r--r--   0        0        0     1780 2023-03-29 02:52:09.774682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id.py
--rw-r--r--   0        0        0     4892 2023-03-29 02:52:09.634681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_actions.py
--rw-r--r--   0        0        0     2223 2023-03-29 02:52:09.778682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_actions_action_id.py
--rw-r--r--   0        0        0     3374 2023-03-29 02:52:09.790682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_advanced_firewall_rules.py
--rw-r--r--   0        0        0     2001 2023-03-29 02:52:09.786682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_available_advanced_features.py
--rw-r--r--   0        0        0     6213 2023-03-29 02:52:09.830682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_backups.py
--rw-r--r--   0        0        0     1999 2023-03-29 02:52:09.786682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_console.py
--rw-r--r--   0        0        0     3271 2023-03-29 02:52:09.818682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_kernels.py
--rw-r--r--   0        0        0     6263 2023-03-29 02:52:09.834682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_snapshots.py
--rw-r--r--   0        0        0     3320 2023-03-29 02:52:09.826682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_software.py
--rw-r--r--   0        0        0     4995 2023-03-29 02:52:09.814682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_threshold_alerts.py
--rw-r--r--   0        0        0     1823 2023-03-29 02:52:09.802682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_user_data.py
--rw-r--r--   0        0        0     1440 2023-03-29 02:52:09.798682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_threshold_alerts.py
--rw-r--r--   0        0        0     5807 2023-03-29 03:05:42.879441 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_sizes.py
--rw-r--r--   0        0        0     3444 2023-03-29 02:52:09.858682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_software.py
--rw-r--r--   0        0        0     4469 2023-03-29 03:05:42.879441 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_software_operating_system_operating_system_id_or_slug.py
--rw-r--r--   0        0        0     1775 2023-03-29 02:52:09.818682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_software_software_id.py
--rw-r--r--   0        0        0     2746 2023-03-29 02:52:09.850682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_vpcs.py
--rw-r--r--   0        0        0     1714 2023-03-29 02:52:09.834682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_vpcs_vpc_id.py
--rw-r--r--   0        0        0     4334 2023-03-29 02:52:09.886683 binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_vpcs_vpc_id_members.py
--rw-r--r--   0        0        0     4070 2023-03-29 02:52:09.878682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/patch_v2_vpcs_vpc_id.py
--rw-r--r--   0        0        0     2666 2023-03-29 02:52:09.542681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_account_keys.py
--rw-r--r--   0        0        0     2332 2023-03-29 02:52:09.466680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_actions_action_id_proceed.py
--rw-r--r--   0        0        0     2337 2023-03-29 02:52:09.494680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_domains.py
--rw-r--r--   0        0        0     5271 2023-03-29 02:52:09.538680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_domains_domain_name_records.py
--rw-r--r--   0        0        0     1193 2023-03-29 02:52:09.490680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_domains_refresh_nameserver_cache.py
--rw-r--r--   0        0        0     2703 2023-03-29 02:52:09.526680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_failover_ips_server_id.py
--rw-r--r--   0        0        0     5120 2023-03-29 02:52:09.602681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_load_balancers.py
--rw-r--r--   0        0        0     3247 2023-03-29 02:52:09.586681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_load_balancers_load_balancer_id_forwarding_rules.py
--rw-r--r--   0        0        0     2598 2023-03-29 02:52:09.578681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_load_balancers_load_balancer_id_servers.py
--rw-r--r--   0        0        0     2316 2023-03-29 02:52:09.590681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_reverse_names_ipv6.py
--rw-r--r--   0        0        0    12108 2023-03-29 02:52:09.918683 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_servers.py
--rw-r--r--   0        0        0      827 2023-03-29 02:52:09.574681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_servers_server_id_actions.py
--rw-r--r--   0        0        0     4169 2023-03-29 02:52:09.838682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_servers_server_id_backups.py
--rw-r--r--   0        0        0     3872 2023-03-29 02:52:09.874683 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_vpcs.py
--rw-r--r--   0        0        0     3397 2023-03-29 02:52:09.626681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_add_disk.py
--rw-r--r--   0        0        0     2924 2023-03-29 02:52:09.618681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_attach_backup.py
--rw-r--r--   0        0        0     5363 2023-03-29 02:52:09.650681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_advanced_features.py
--rw-r--r--   0        0        0     5882 2023-03-29 02:52:09.674681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_advanced_firewall_rules.py
--rw-r--r--   0        0        0     3776 2023-03-29 02:52:09.638681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_backup_schedule.py
--rw-r--r--   0        0        0     2895 2023-03-29 02:52:09.626681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_ipv_6.py
--rw-r--r--   0        0        0     3254 2023-03-29 02:52:09.654681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_ipv_6_reverse_nameservers.py
--rw-r--r--   0        0        0     2902 2023-03-29 02:52:09.634681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_kernel.py
--rw-r--r--   0        0        0     3504 2023-03-29 02:52:09.638681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_manage_offsite_backup_copies.py
--rw-r--r--   0        0        0     3037 2023-03-29 02:52:09.646681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_network.py
--rw-r--r--   0        0        0     3363 2023-03-29 02:52:09.650681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_offsite_backup_location.py
--rw-r--r--   0        0        0     3079 2023-03-29 02:52:09.658681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_partner.py
--rw-r--r--   0        0        0     2985 2023-03-29 02:52:09.682681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_port_blocking.py
--rw-r--r--   0        0        0     3342 2023-03-29 02:52:09.690681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_reverse_name.py
--rw-r--r--   0        0        0     3213 2023-03-29 02:52:09.690681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_separate_private_network_interface.py
--rw-r--r--   0        0        0     3169 2023-03-29 02:52:09.694682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_source_and_destination_check.py
--rw-r--r--   0        0        0     5789 2023-03-29 02:52:09.714681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_threshold_alerts.py
--rw-r--r--   0        0        0     3308 2023-03-29 02:52:09.686681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_vpc_ipv_4.py
--rw-r--r--   0        0        0     3825 2023-03-29 02:52:09.738682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_clone_using_backup.py
--rw-r--r--   0        0        0     2920 2023-03-29 02:52:09.702681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_delete_disk.py
--rw-r--r--   0        0        0     2642 2023-03-29 02:52:09.710682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_detach_backup.py
--rw-r--r--   0        0        0     2662 2023-03-29 02:52:09.706681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_disable_backups.py
--rw-r--r--   0        0        0     2662 2023-03-29 02:52:09.694682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_disable_selinux.py
--rw-r--r--   0        0        0     2652 2023-03-29 02:52:09.710682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_enable_backups.py
--rw-r--r--   0        0        0     2625 2023-03-29 02:52:09.722682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_enable_ipv_6.py
--rw-r--r--   0        0        0     2612 2023-03-29 02:52:09.698681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_is_running.py
--rw-r--r--   0        0        0     3917 2023-03-29 02:52:09.726682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_password_reset.py
--rw-r--r--   0        0        0     2559 2023-03-29 02:52:09.722682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_ping.py
--rw-r--r--   0        0        0     2622 2023-03-29 02:52:09.742682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_cycle.py
--rw-r--r--   0        0        0     2602 2023-03-29 02:52:09.778682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_off.py
--rw-r--r--   0        0        0     2592 2023-03-29 02:52:09.746682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_on.py
--rw-r--r--   0        0        0     2579 2023-03-29 02:52:09.742682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_reboot.py
--rw-r--r--   0        0        0     5238 2023-03-29 02:52:09.774682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_rebuild.py
--rw-r--r--   0        0        0     2870 2023-03-29 02:52:09.738682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_rename.py
--rw-r--r--   0        0        0    15950 2023-03-29 02:52:09.894683 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_resize.py
--rw-r--r--   0        0        0     3293 2023-03-29 02:52:09.758682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_resize_disk.py
--rw-r--r--   0        0        0     2907 2023-03-29 02:52:09.758682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_restore.py
--rw-r--r--   0        0        0     2599 2023-03-29 02:52:09.778682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_shutdown.py
--rw-r--r--   0        0        0     4148 2023-03-29 02:52:09.794682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_take_backup.py
--rw-r--r--   0        0        0     2599 2023-03-29 02:52:09.766682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_uncancel.py
--rw-r--r--   0        0        0     2579 2023-03-29 02:52:09.766682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_uptime.py
--rw-r--r--   0        0        0     3030 2023-03-29 03:05:42.879441 binarylane_cli-0.15.3/src/binarylane/console/commands/api/put_v2_account_keys_key_id.py
--rw-r--r--   0        0        0     5642 2023-03-29 02:52:09.574681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/put_v2_domains_domain_name_records_record_id.py
--rw-r--r--   0        0        0     3028 2023-03-29 02:52:09.538680 binarylane_cli-0.15.3/src/binarylane/console/commands/api/put_v2_images_image_id.py
--rw-r--r--   0        0        0     5267 2023-03-29 02:52:09.618681 binarylane_cli-0.15.3/src/binarylane/console/commands/api/put_v2_load_balancers_load_balancer_id.py
--rw-r--r--   0        0        0     3893 2023-03-29 02:52:09.882682 binarylane_cli-0.15.3/src/binarylane/console/commands/api/put_v2_vpcs_vpc_id.py
--rw-r--r--   0        0        0     1950 2023-03-21 04:41:01.420051 binarylane_cli-0.15.3/src/binarylane/console/commands/configure.py
--rw-r--r--   0        0        0      295 2023-03-15 04:49:44.262009 binarylane_cli-0.15.3/src/binarylane/console/commands/version.py
--rw-r--r--   0        0        0      476 2023-03-15 04:49:44.262009 binarylane_cli-0.15.3/src/binarylane/console/metadata.py
--rw-r--r--   0        0        0      529 2023-03-15 04:49:44.262009 binarylane_cli-0.15.3/src/binarylane/console/parser/__init__.py
--rw-r--r--   0        0        0     2592 2023-03-29 02:51:55.022597 binarylane_cli-0.15.3/src/binarylane/console/parser/attribute.py
--rw-r--r--   0        0        0     1439 2023-02-07 09:32:33.873646 binarylane_cli-0.15.3/src/binarylane/console/parser/help_formatter.py
--rw-r--r--   0        0        0     4785 2023-03-29 02:51:55.022597 binarylane_cli-0.15.3/src/binarylane/console/parser/list_attribute.py
--rw-r--r--   0        0        0     4935 2023-03-29 02:51:55.022597 binarylane_cli-0.15.3/src/binarylane/console/parser/object_attribute.py
--rw-r--r--   0        0        0     5765 2023-03-29 02:51:55.022597 binarylane_cli-0.15.3/src/binarylane/console/parser/parser.py
--rw-r--r--   0        0        0    10031 2023-03-21 04:41:01.420051 binarylane_cli-0.15.3/src/binarylane/console/parser/primitive_attribute.py
--rw-r--r--   0        0        0      888 2023-02-07 09:32:33.873646 binarylane_cli-0.15.3/src/binarylane/console/printers/__init__.py
--rw-r--r--   0        0        0     4638 2023-03-22 00:34:24.764386 binarylane_cli-0.15.3/src/binarylane/console/printers/formatter.py
--rw-r--r--   0        0        0      348 2023-02-17 22:36:19.051007 binarylane_cli-0.15.3/src/binarylane/console/printers/json_printer.py
--rw-r--r--   0        0        0      486 2023-02-17 22:36:19.051007 binarylane_cli-0.15.3/src/binarylane/console/printers/plain_printer.py
--rw-r--r--   0        0        0     1166 2023-02-17 22:36:19.051007 binarylane_cli-0.15.3/src/binarylane/console/printers/printer.py
--rw-r--r--   0        0        0      621 2023-02-17 22:36:19.051007 binarylane_cli-0.15.3/src/binarylane/console/printers/table_printer.py
--rw-r--r--   0        0        0      343 2023-02-17 22:36:19.051007 binarylane_cli-0.15.3/src/binarylane/console/printers/tsv_printer.py
--rw-r--r--   0        0        0       25 2023-02-07 09:32:33.873646 binarylane_cli-0.15.3/src/binarylane/console/py.typed
--rw-r--r--   0        0        0     3114 2023-03-21 04:41:01.420051 binarylane_cli-0.15.3/src/binarylane/console/runners/__init__.py
--rw-r--r--   0        0        0     3239 2023-03-21 04:41:01.420051 binarylane_cli-0.15.3/src/binarylane/console/runners/action.py
--rw-r--r--   0        0        0      861 2023-02-07 09:32:33.873646 binarylane_cli-0.15.3/src/binarylane/console/runners/actionlink.py
--rw-r--r--   0        0        0     5803 2023-03-21 05:56:18.130066 binarylane_cli-0.15.3/src/binarylane/console/runners/command.py
--rw-r--r--   0        0        0     2277 2023-03-15 04:49:44.262009 binarylane_cli-0.15.3/src/binarylane/console/runners/httpx_wrapper.py
--rw-r--r--   0        0        0     2633 2023-03-21 05:56:18.134066 binarylane_cli-0.15.3/src/binarylane/console/runners/list.py
--rw-r--r--   0        0        0      930 2023-03-15 04:49:44.262009 binarylane_cli-0.15.3/src/binarylane/console/util.py
--rw-r--r--   0        0        0      224 2023-02-07 09:32:33.873646 binarylane_cli-0.15.3/src/binarylane/pycompat/__init__.py
--rw-r--r--   0        0        0     1967 2023-03-15 04:49:44.262009 binarylane_cli-0.15.3/src/binarylane/pycompat/actions.py
--rw-r--r--   0        0        0      316 2023-02-07 09:32:33.873646 binarylane_cli-0.15.3/src/binarylane/pycompat/functools.py
--rw-r--r--   0        0        0      394 2023-02-07 09:32:33.873646 binarylane_cli-0.15.3/src/binarylane/pycompat/importlib.py
--rw-r--r--   0        0        0      474 2023-02-07 09:32:33.873646 binarylane_cli-0.15.3/src/binarylane/pycompat/shlex.py
--rw-r--r--   0        0        0      362 2023-03-15 04:49:44.262009 binarylane_cli-0.15.3/src/binarylane/pycompat/typing.py
--rw-r--r--   0        0        0    19865 1970-01-01 00:00:00.000000 binarylane_cli-0.15.3/setup.py
--rw-r--r--   0        0        0    17253 1970-01-01 00:00:00.000000 binarylane_cli-0.15.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-02-07 09:32:33.853646 binarylane_cli-0.16.0/LICENSE
+-rw-r--r--   0        0        0    16395 2023-02-17 22:36:19.031007 binarylane_cli-0.16.0/README.md
+-rw-r--r--   0        0        0       83 2023-03-29 02:52:04.102649 binarylane_cli-0.16.0/lib/binarylane/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.318645 binarylane_cli-0.16.0/lib/binarylane/api/accounts/__init__.py
+-rw-r--r--   0        0        0     3886 2023-03-29 02:52:06.690664 binarylane_cli-0.16.0/lib/binarylane/api/accounts/get_v2_account.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.342645 binarylane_cli-0.16.0/lib/binarylane/api/actions/__init__.py
+-rw-r--r--   0        0        0     5427 2023-03-29 02:52:06.774664 binarylane_cli-0.16.0/lib/binarylane/api/actions/get_v2_actions.py
+-rw-r--r--   0        0        0     4698 2023-03-29 02:52:06.774664 binarylane_cli-0.16.0/lib/binarylane/api/actions/get_v2_actions_action_id.py
+-rw-r--r--   0        0        0     5165 2023-03-29 02:52:06.778665 binarylane_cli-0.16.0/lib/binarylane/api/actions/post_v2_actions_action_id_proceed.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.342645 binarylane_cli-0.16.0/lib/binarylane/api/customers/__init__.py
+-rw-r--r--   0        0        0     3859 2023-03-29 02:52:06.826665 binarylane_cli-0.16.0/lib/binarylane/api/customers/get_v2_customers_my_balance.py
+-rw-r--r--   0        0        0     5446 2023-03-29 02:52:06.826665 binarylane_cli-0.16.0/lib/binarylane/api/customers/get_v2_customers_my_invoices.py
+-rw-r--r--   0        0        0     4717 2023-03-29 02:52:06.826665 binarylane_cli-0.16.0/lib/binarylane/api/customers/get_v2_customers_my_invoices_invoice_id.py
+-rw-r--r--   0        0        0     4605 2023-03-29 02:52:06.830665 binarylane_cli-0.16.0/lib/binarylane/api/customers/get_v2_customers_my_unpaid_payment_failed_invoices.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.346645 binarylane_cli-0.16.0/lib/binarylane/api/data_usages/__init__.py
+-rw-r--r--   0        0        0     5635 2023-03-29 02:52:06.750664 binarylane_cli-0.16.0/lib/binarylane/api/data_usages/get_v2_data_usages_current.py
+-rw-r--r--   0        0        0     4826 2023-03-29 02:52:06.750664 binarylane_cli-0.16.0/lib/binarylane/api/data_usages/get_v2_data_usages_server_id_current.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.350645 binarylane_cli-0.16.0/lib/binarylane/api/domains/__init__.py
+-rw-r--r--   0        0        0     4505 2023-03-29 02:52:06.770665 binarylane_cli-0.16.0/lib/binarylane/api/domains/delete_v2_domains_domain_name.py
+-rw-r--r--   0        0        0     5124 2023-03-29 02:52:06.766665 binarylane_cli-0.16.0/lib/binarylane/api/domains/delete_v2_domains_domain_name_records_record_id.py
+-rw-r--r--   0        0        0     6308 2023-03-29 02:52:06.770665 binarylane_cli-0.16.0/lib/binarylane/api/domains/get_v2_domains.py
+-rw-r--r--   0        0        0     4746 2023-03-29 02:52:06.762664 binarylane_cli-0.16.0/lib/binarylane/api/domains/get_v2_domains_domain_name.py
+-rw-r--r--   0        0        0    11108 2023-03-29 02:52:06.766665 binarylane_cli-0.16.0/lib/binarylane/api/domains/get_v2_domains_domain_name_records.py
+-rw-r--r--   0        0        0     5444 2023-03-29 02:52:06.770665 binarylane_cli-0.16.0/lib/binarylane/api/domains/get_v2_domains_domain_name_records_record_id.py
+-rw-r--r--   0        0        0     3952 2023-03-29 02:52:06.770665 binarylane_cli-0.16.0/lib/binarylane/api/domains/get_v2_domains_nameservers.py
+-rw-r--r--   0        0        0     4878 2023-03-29 02:52:06.762664 binarylane_cli-0.16.0/lib/binarylane/api/domains/post_v2_domains.py
+-rw-r--r--   0        0        0     6881 2023-03-29 02:52:06.762664 binarylane_cli-0.16.0/lib/binarylane/api/domains/post_v2_domains_domain_name_records.py
+-rw-r--r--   0        0        0     2886 2023-03-29 02:52:06.758664 binarylane_cli-0.16.0/lib/binarylane/api/domains/post_v2_domains_refresh_nameserver_cache.py
+-rw-r--r--   0        0        0     7399 2023-03-29 02:52:06.766665 binarylane_cli-0.16.0/lib/binarylane/api/domains/put_v2_domains_domain_name_records_record_id.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.362645 binarylane_cli-0.16.0/lib/binarylane/api/failover_ips/__init__.py
+-rw-r--r--   0        0        0     6382 2023-03-29 02:52:06.786665 binarylane_cli-0.16.0/lib/binarylane/api/failover_ips/get_v2_failover_ips_server_id.py
+-rw-r--r--   0        0        0     6564 2023-03-29 02:52:06.786665 binarylane_cli-0.16.0/lib/binarylane/api/failover_ips/get_v2_failover_ips_server_id_available.py
+-rw-r--r--   0        0        0     7465 2023-03-29 02:52:06.790665 binarylane_cli-0.16.0/lib/binarylane/api/failover_ips/post_v2_failover_ips_server_id.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.366645 binarylane_cli-0.16.0/lib/binarylane/api/images/__init__.py
+-rw-r--r--   0        0        0     7947 2023-03-29 02:52:06.834665 binarylane_cli-0.16.0/lib/binarylane/api/images/get_v2_images.py
+-rw-r--r--   0        0        0     5098 2023-03-29 02:52:06.830665 binarylane_cli-0.16.0/lib/binarylane/api/images/get_v2_images_image_id_download.py
+-rw-r--r--   0        0        0     5152 2023-03-29 03:05:42.875441 binarylane_cli-0.16.0/lib/binarylane/api/images/get_v2_images_image_id_or_slug.py
+-rw-r--r--   0        0        0     5969 2023-03-29 02:52:06.830665 binarylane_cli-0.16.0/lib/binarylane/api/images/put_v2_images_image_id.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.370645 binarylane_cli-0.16.0/lib/binarylane/api/keys/__init__.py
+-rw-r--r--   0        0        0     4874 2023-03-29 03:05:42.875441 binarylane_cli-0.16.0/lib/binarylane/api/keys/delete_v2_account_keys_key_id.py
+-rw-r--r--   0        0        0     5437 2023-03-29 02:52:06.758664 binarylane_cli-0.16.0/lib/binarylane/api/keys/get_v2_account_keys.py
+-rw-r--r--   0        0        0     5116 2023-03-29 03:05:42.875441 binarylane_cli-0.16.0/lib/binarylane/api/keys/get_v2_account_keys_key_id.py
+-rw-r--r--   0        0        0     4877 2023-03-29 02:52:06.754665 binarylane_cli-0.16.0/lib/binarylane/api/keys/post_v2_account_keys.py
+-rw-r--r--   0        0        0     6236 2023-03-29 03:05:42.875441 binarylane_cli-0.16.0/lib/binarylane/api/keys/put_v2_account_keys_key_id.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.374645 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/__init__.py
+-rw-r--r--   0        0        0     4660 2023-03-29 02:52:06.798665 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id.py
+-rw-r--r--   0        0        0     6123 2023-03-29 02:52:06.794665 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id_forwarding_rules.py
+-rw-r--r--   0        0        0     6072 2023-03-29 02:52:06.790665 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id_servers.py
+-rw-r--r--   0        0        0     5541 2023-03-29 02:52:06.794665 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/get_v2_load_balancers.py
+-rw-r--r--   0        0        0     4145 2023-03-29 02:52:06.790665 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/get_v2_load_balancers_availability.py
+-rw-r--r--   0        0        0     4980 2023-03-29 02:52:06.790665 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/get_v2_load_balancers_load_balancer_id.py
+-rw-r--r--   0        0        0     5584 2023-03-29 02:52:06.794665 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/post_v2_load_balancers.py
+-rw-r--r--   0        0        0     6089 2023-03-29 02:52:06.798665 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/post_v2_load_balancers_load_balancer_id_forwarding_rules.py
+-rw-r--r--   0        0        0     6038 2023-03-29 02:52:06.802665 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/post_v2_load_balancers_load_balancer_id_servers.py
+-rw-r--r--   0        0        0     6613 2023-03-29 02:52:06.798665 binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/put_v2_load_balancers_load_balancer_id.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.386645 binarylane_cli-0.16.0/lib/binarylane/api/regions/__init__.py
+-rw-r--r--   0        0        0     5178 2023-03-29 02:52:06.822665 binarylane_cli-0.16.0/lib/binarylane/api/regions/get_v2_regions.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.386645 binarylane_cli-0.16.0/lib/binarylane/api/reverse_names/__init__.py
+-rw-r--r--   0        0        0     7559 2023-03-29 02:52:06.682664 binarylane_cli-0.16.0/lib/binarylane/api/reverse_names/get_v2_reverse_names_ipv6.py
+-rw-r--r--   0        0        0     5530 2023-03-29 02:52:06.682664 binarylane_cli-0.16.0/lib/binarylane/api/reverse_names/post_v2_reverse_names_ipv6.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.390645 binarylane_cli-0.16.0/lib/binarylane/api/sample_sets/__init__.py
+-rw-r--r--   0        0        0    12650 2023-03-29 02:52:06.822665 binarylane_cli-0.16.0/lib/binarylane/api/sample_sets/get_v2_samplesets_server_id.py
+-rw-r--r--   0        0        0     7362 2023-03-29 02:52:06.822665 binarylane_cli-0.16.0/lib/binarylane/api/sample_sets/get_v2_samplesets_server_id_latest.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.394645 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/__init__.py
+-rw-r--r--   0        0        0     6448 2023-03-29 02:52:06.718664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/get_v2_servers_server_id_actions.py
+-rw-r--r--   0        0        0    22360 2023-03-29 02:52:06.742664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v2_servers_server_id_actions.py
+-rw-r--r--   0        0        0     7190 2023-03-29 02:52:06.706664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_add_disk.py
+-rw-r--r--   0        0        0     6826 2023-03-29 02:52:06.738664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_attach_backup.py
+-rw-r--r--   0        0        0     6967 2023-03-29 02:52:06.694664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_advanced_features.py
+-rw-r--r--   0        0        0     7044 2023-03-29 02:52:06.710664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_advanced_firewall_rules.py
+-rw-r--r--   0        0        0     6823 2023-03-29 02:52:06.702664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_backup_schedule.py
+-rw-r--r--   0        0        0     6643 2023-03-29 02:52:06.722664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_ipv_6.py
+-rw-r--r--   0        0        0     6997 2023-03-29 02:52:06.722664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_ipv_6_reverse_nameservers.py
+-rw-r--r--   0        0        0     6934 2023-03-29 02:52:06.714664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_kernel.py
+-rw-r--r--   0        0        0     7495 2023-03-29 02:52:06.694664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_manage_offsite_backup_copies.py
+-rw-r--r--   0        0        0     6946 2023-03-29 02:52:06.710664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_network.py
+-rw-r--r--   0        0        0     7316 2023-03-29 02:52:06.694664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_offsite_backup_location.py
+-rw-r--r--   0        0        0     6842 2023-03-29 02:52:06.702664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_partner.py
+-rw-r--r--   0        0        0     7967 2023-03-29 02:52:06.742664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_port_blocking.py
+-rw-r--r--   0        0        0     6859 2023-03-29 02:52:06.714664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_reverse_name.py
+-rw-r--r--   0        0        0     7567 2023-03-29 02:52:06.746664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_separate_private_network_interface.py
+-rw-r--r--   0        0        0    10443 2023-03-29 02:52:06.718664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_source_and_destination_check.py
+-rw-r--r--   0        0        0     6911 2023-03-29 02:52:06.722664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_threshold_alerts.py
+-rw-r--r--   0        0        0     6744 2023-03-29 02:52:06.690664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_vpc_ipv_4.py
+-rw-r--r--   0        0        0     8171 2023-03-29 02:52:06.698664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_clone_using_backup.py
+-rw-r--r--   0        0        0     6990 2023-03-29 02:52:06.718664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_delete_disk.py
+-rw-r--r--   0        0        0     6730 2023-03-29 02:52:06.726664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_detach_backup.py
+-rw-r--r--   0        0        0     8362 2023-03-29 02:52:06.734664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_disable_backups.py
+-rw-r--r--   0        0        0     7074 2023-03-29 02:52:06.738664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_disable_selinux.py
+-rw-r--r--   0        0        0     7574 2023-03-29 02:52:06.730664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_enable_backups.py
+-rw-r--r--   0        0        0     7031 2023-03-29 02:52:06.746664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_enable_ipv_6.py
+-rw-r--r--   0        0        0     6914 2023-03-29 02:52:06.714664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_is_running.py
+-rw-r--r--   0        0        0     7126 2023-03-29 02:52:06.730664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_password_reset.py
+-rw-r--r--   0        0        0     6881 2023-03-29 02:52:06.706664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_ping.py
+-rw-r--r--   0        0        0     7034 2023-03-29 02:52:06.726664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_cycle.py
+-rw-r--r--   0        0        0     6506 2023-03-29 02:52:06.706664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_off.py
+-rw-r--r--   0        0        0     6690 2023-03-29 02:52:06.730664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_on.py
+-rw-r--r--   0        0        0     7149 2023-03-29 02:52:06.734664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_reboot.py
+-rw-r--r--   0        0        0     6829 2023-03-29 02:52:06.706664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_rebuild.py
+-rw-r--r--   0        0        0     6645 2023-03-29 02:52:06.702664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_rename.py
+-rw-r--r--   0        0        0     7897 2023-03-29 02:52:06.738664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_resize.py
+-rw-r--r--   0        0        0     7446 2023-03-29 02:52:06.734664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_resize_disk.py
+-rw-r--r--   0        0        0     6929 2023-03-29 02:52:06.698664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_restore.py
+-rw-r--r--   0        0        0     7101 2023-03-29 02:52:06.746664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_shutdown.py
+-rw-r--r--   0        0        0     6454 2023-03-29 02:52:06.730664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_take_backup.py
+-rw-r--r--   0        0        0     6825 2023-03-29 02:52:06.710664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_uncancel.py
+-rw-r--r--   0        0        0     6545 2023-03-29 02:52:06.750664 binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_uptime.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.458645 binarylane_cli-0.16.0/lib/binarylane/api/servers/__init__.py
+-rw-r--r--   0        0        0     5309 2023-03-29 02:52:06.806665 binarylane_cli-0.16.0/lib/binarylane/api/servers/delete_v2_servers_server_id.py
+-rw-r--r--   0        0        0     6741 2023-03-29 02:52:06.818665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers.py
+-rw-r--r--   0        0        0     4698 2023-03-29 02:52:06.810665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id.py
+-rw-r--r--   0        0        0     5333 2023-03-29 02:52:06.814665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_actions_action_id.py
+-rw-r--r--   0        0        0     5139 2023-03-29 02:52:06.806665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_advanced_firewall_rules.py
+-rw-r--r--   0        0        0     5342 2023-03-29 02:52:06.802665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_available_advanced_features.py
+-rw-r--r--   0        0        0     6448 2023-03-29 02:52:06.810665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_backups.py
+-rw-r--r--   0        0        0     5384 2023-03-29 02:52:06.810665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_console.py
+-rw-r--r--   0        0        0     6828 2023-03-29 02:52:06.806665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_kernels.py
+-rw-r--r--   0        0        0     6808 2023-03-29 02:52:06.802665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_snapshots.py
+-rw-r--r--   0        0        0     6624 2023-03-29 02:52:06.814665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_software.py
+-rw-r--r--   0        0        0     5405 2023-03-29 02:52:06.818665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_threshold_alerts.py
+-rw-r--r--   0        0        0     4814 2023-03-29 02:52:06.814665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_user_data.py
+-rw-r--r--   0        0        0     4513 2023-03-29 02:52:06.806665 binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_threshold_alerts.py
+-rw-r--r--   0        0        0     5024 2023-03-29 02:52:06.814665 binarylane_cli-0.16.0/lib/binarylane/api/servers/post_v2_servers.py
+-rw-r--r--   0        0        0     6101 2023-03-29 02:52:06.818665 binarylane_cli-0.16.0/lib/binarylane/api/servers/post_v2_servers_server_id_backups.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.478646 binarylane_cli-0.16.0/lib/binarylane/api/sizes/__init__.py
+-rw-r--r--   0        0        0     9151 2023-03-29 03:05:42.879441 binarylane_cli-0.16.0/lib/binarylane/api/sizes/get_v2_sizes.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.478646 binarylane_cli-0.16.0/lib/binarylane/api/software/__init__.py
+-rw-r--r--   0        0        0     5249 2023-03-29 02:52:06.690664 binarylane_cli-0.16.0/lib/binarylane/api/software/get_v2_software.py
+-rw-r--r--   0        0        0     7624 2023-03-29 03:05:42.879441 binarylane_cli-0.16.0/lib/binarylane/api/software/get_v2_software_operating_system_operating_system_id_or_slug.py
+-rw-r--r--   0        0        0     4578 2023-03-29 02:52:06.686664 binarylane_cli-0.16.0/lib/binarylane/api/software/get_v2_software_software_id.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:03.482646 binarylane_cli-0.16.0/lib/binarylane/api/vpcs/__init__.py
+-rw-r--r--   0        0        0     4477 2023-03-29 02:52:06.778665 binarylane_cli-0.16.0/lib/binarylane/api/vpcs/delete_v2_vpcs_vpc_id.py
+-rw-r--r--   0        0        0     5409 2023-03-29 02:52:06.782665 binarylane_cli-0.16.0/lib/binarylane/api/vpcs/get_v2_vpcs.py
+-rw-r--r--   0        0        0     4524 2023-03-29 02:52:06.782665 binarylane_cli-0.16.0/lib/binarylane/api/vpcs/get_v2_vpcs_vpc_id.py
+-rw-r--r--   0        0        0     8911 2023-03-29 02:52:06.786665 binarylane_cli-0.16.0/lib/binarylane/api/vpcs/get_v2_vpcs_vpc_id_members.py
+-rw-r--r--   0        0        0     5833 2023-03-29 02:52:06.778665 binarylane_cli-0.16.0/lib/binarylane/api/vpcs/patch_v2_vpcs_vpc_id.py
+-rw-r--r--   0        0        0     4858 2023-03-29 02:52:06.778665 binarylane_cli-0.16.0/lib/binarylane/api/vpcs/post_v2_vpcs.py
+-rw-r--r--   0        0        0     6150 2023-03-29 02:52:06.782665 binarylane_cli-0.16.0/lib/binarylane/api/vpcs/put_v2_vpcs_vpc_id.py
+-rw-r--r--   0        0        0     2709 2023-03-29 02:52:05.590658 binarylane_cli-0.16.0/lib/binarylane/client.py
+-rw-r--r--   0        0        0      318 2023-03-29 02:52:05.558658 binarylane_cli-0.16.0/lib/binarylane/errors.py
+-rw-r--r--   0        0        0        0 2023-03-29 02:52:06.646664 binarylane_cli-0.16.0/lib/binarylane/models/__init__.py
+-rw-r--r--   0        0        0     3964 2023-03-29 02:52:06.922665 binarylane_cli-0.16.0/lib/binarylane/models/account.py
+-rw-r--r--   0        0        0     1524 2023-03-29 02:52:07.010666 binarylane_cli-0.16.0/lib/binarylane/models/account_response.py
+-rw-r--r--   0        0        0      252 2023-03-29 02:52:04.386651 binarylane_cli-0.16.0/lib/binarylane/models/account_status.py
+-rw-r--r--   0        0        0     8597 2023-03-29 02:52:07.006666 binarylane_cli-0.16.0/lib/binarylane/models/action.py
+-rw-r--r--   0        0        0     1639 2023-03-29 02:52:05.690658 binarylane_cli-0.16.0/lib/binarylane/models/action_link.py
+-rw-r--r--   0        0        0     2943 2023-03-29 02:52:06.994666 binarylane_cli-0.16.0/lib/binarylane/models/action_progress.py
+-rw-r--r--   0        0        0     1504 2023-03-29 02:52:06.990666 binarylane_cli-0.16.0/lib/binarylane/models/action_response.py
+-rw-r--r--   0        0        0      237 2023-03-29 02:52:04.470651 binarylane_cli-0.16.0/lib/binarylane/models/action_status.py
+-rw-r--r--   0        0        0     1813 2023-03-29 02:52:06.890665 binarylane_cli-0.16.0/lib/binarylane/models/actions_links.py
+-rw-r--r--   0        0        0     2809 2023-03-29 02:52:06.906665 binarylane_cli-0.16.0/lib/binarylane/models/actions_response.py
+-rw-r--r--   0        0        0     2390 2023-03-29 02:52:06.898665 binarylane_cli-0.16.0/lib/binarylane/models/add_disk.py
+-rw-r--r--   0        0        0      178 2023-03-29 02:52:04.454651 binarylane_cli-0.16.0/lib/binarylane/models/add_disk_type.py
+-rw-r--r--   0        0        0      494 2023-03-29 02:52:04.458651 binarylane_cli-0.16.0/lib/binarylane/models/advanced_feature.py
+-rw-r--r--   0        0        0     4296 2023-03-29 02:52:06.894665 binarylane_cli-0.16.0/lib/binarylane/models/advanced_firewall_rule.py
+-rw-r--r--   0        0        0      207 2023-03-29 02:52:04.298650 binarylane_cli-0.16.0/lib/binarylane/models/advanced_firewall_rule_action.py
+-rw-r--r--   0        0        0      235 2023-03-29 02:52:04.506651 binarylane_cli-0.16.0/lib/binarylane/models/advanced_firewall_rule_protocol.py
+-rw-r--r--   0        0        0     2325 2023-03-29 02:52:07.002666 binarylane_cli-0.16.0/lib/binarylane/models/advanced_firewall_rules_response.py
+-rw-r--r--   0        0        0     4703 2023-03-29 02:52:06.866665 binarylane_cli-0.16.0/lib/binarylane/models/advanced_server_features.py
+-rw-r--r--   0        0        0     1746 2023-03-29 02:52:06.962666 binarylane_cli-0.16.0/lib/binarylane/models/attach_backup.py
+-rw-r--r--   0        0        0      193 2023-03-29 02:52:04.370651 binarylane_cli-0.16.0/lib/binarylane/models/attach_backup_type.py
+-rw-r--r--   0        0        0     3782 2023-03-29 02:52:06.910665 binarylane_cli-0.16.0/lib/binarylane/models/attached_backup.py
+-rw-r--r--   0        0        0     3789 2023-03-29 02:52:06.890665 binarylane_cli-0.16.0/lib/binarylane/models/available_advanced_server_features.py
+-rw-r--r--   0        0        0     2068 2023-03-29 02:52:06.862665 binarylane_cli-0.16.0/lib/binarylane/models/available_advanced_server_features_response.py
+-rw-r--r--   0        0        0     2387 2023-03-29 02:52:06.874665 binarylane_cli-0.16.0/lib/binarylane/models/backup_disk.py
+-rw-r--r--   0        0        0     3714 2023-03-29 02:52:06.850665 binarylane_cli-0.16.0/lib/binarylane/models/backup_info.py
+-rw-r--r--   0        0        0      256 2023-03-29 02:52:04.338651 binarylane_cli-0.16.0/lib/binarylane/models/backup_replacement_strategy.py
+-rw-r--r--   0        0        0     3665 2023-03-29 02:52:06.918665 binarylane_cli-0.16.0/lib/binarylane/models/backup_settings.py
+-rw-r--r--   0        0        0      245 2023-03-29 02:52:04.358651 binarylane_cli-0.16.0/lib/binarylane/models/backup_slot.py
+-rw-r--r--   0        0        0     1984 2023-03-29 02:52:05.766659 binarylane_cli-0.16.0/lib/binarylane/models/backup_window.py
+-rw-r--r--   0        0        0     2804 2023-03-29 02:52:07.006666 binarylane_cli-0.16.0/lib/binarylane/models/backups_response.py
+-rw-r--r--   0        0        0     3413 2023-03-29 02:52:06.986666 binarylane_cli-0.16.0/lib/binarylane/models/balance.py
+-rw-r--r--   0        0        0     1524 2023-03-29 02:52:06.982666 binarylane_cli-0.16.0/lib/binarylane/models/balance_response.py
+-rw-r--r--   0        0        0     6741 2023-03-29 02:52:06.898665 binarylane_cli-0.16.0/lib/binarylane/models/change_advanced_features.py
+-rw-r--r--   0        0        0      225 2023-03-29 02:52:04.410651 binarylane_cli-0.16.0/lib/binarylane/models/change_advanced_features_type.py
+-rw-r--r--   0        0        0     2635 2023-03-29 02:52:06.970666 binarylane_cli-0.16.0/lib/binarylane/models/change_advanced_firewall_rules.py
+-rw-r--r--   0        0        0      242 2023-03-29 02:52:04.474651 binarylane_cli-0.16.0/lib/binarylane/models/change_advanced_firewall_rules_type.py
+-rw-r--r--   0        0        0     3061 2023-03-29 02:52:06.922665 binarylane_cli-0.16.0/lib/binarylane/models/change_backup_schedule.py
+-rw-r--r--   0        0        0      219 2023-03-29 02:52:04.542652 binarylane_cli-0.16.0/lib/binarylane/models/change_backup_schedule_type.py
+-rw-r--r--   0        0        0     2953 2023-03-29 02:52:06.926665 binarylane_cli-0.16.0/lib/binarylane/models/change_image.py
+-rw-r--r--   0        0        0     1743 2023-03-29 02:52:06.902665 binarylane_cli-0.16.0/lib/binarylane/models/change_ipv_6.py
+-rw-r--r--   0        0        0     2279 2023-03-29 02:52:06.950666 binarylane_cli-0.16.0/lib/binarylane/models/change_ipv_6_reverse_nameservers.py
+-rw-r--r--   0        0        0      245 2023-03-29 02:52:04.442651 binarylane_cli-0.16.0/lib/binarylane/models/change_ipv_6_reverse_nameservers_type.py
+-rw-r--r--   0        0        0      187 2023-03-29 02:52:04.294650 binarylane_cli-0.16.0/lib/binarylane/models/change_ipv_6_type.py
+-rw-r--r--   0        0        0     1734 2023-03-29 02:52:06.990666 binarylane_cli-0.16.0/lib/binarylane/models/change_kernel.py
+-rw-r--r--   0        0        0      193 2023-03-29 02:52:04.522652 binarylane_cli-0.16.0/lib/binarylane/models/change_kernel_type.py
+-rw-r--r--   0        0        0     1859 2023-03-29 02:52:06.894665 binarylane_cli-0.16.0/lib/binarylane/models/change_licenses.py
+-rw-r--r--   0        0        0     2560 2023-03-29 02:52:07.002666 binarylane_cli-0.16.0/lib/binarylane/models/change_manage_offsite_backup_copies.py
+-rw-r--r--   0        0        0      256 2023-03-29 02:52:04.526651 binarylane_cli-0.16.0/lib/binarylane/models/change_manage_offsite_backup_copies_type.py
+-rw-r--r--   0        0        0     1976 2023-03-29 02:52:06.898665 binarylane_cli-0.16.0/lib/binarylane/models/change_network.py
+-rw-r--r--   0        0        0      196 2023-03-29 02:52:04.338651 binarylane_cli-0.16.0/lib/binarylane/models/change_network_type.py
+-rw-r--r--   0        0        0     2470 2023-03-29 02:52:06.998666 binarylane_cli-0.16.0/lib/binarylane/models/change_offsite_backup_location.py
+-rw-r--r--   0        0        0      242 2023-03-29 02:52:04.490651 binarylane_cli-0.16.0/lib/binarylane/models/change_offsite_backup_location_type.py
+-rw-r--r--   0        0        0     2132 2023-03-29 02:52:06.902665 binarylane_cli-0.16.0/lib/binarylane/models/change_partner.py
+-rw-r--r--   0        0        0      196 2023-03-29 02:52:04.522652 binarylane_cli-0.16.0/lib/binarylane/models/change_partner_type.py
+-rw-r--r--   0        0        0     1835 2023-03-29 02:52:06.854665 binarylane_cli-0.16.0/lib/binarylane/models/change_port_blocking.py
+-rw-r--r--   0        0        0      213 2023-03-29 02:52:04.534652 binarylane_cli-0.16.0/lib/binarylane/models/change_port_blocking_type.py
+-rw-r--r--   0        0        0     2322 2023-03-29 02:52:06.966666 binarylane_cli-0.16.0/lib/binarylane/models/change_reverse_name.py
+-rw-r--r--   0        0        0      210 2023-03-29 02:52:04.538652 binarylane_cli-0.16.0/lib/binarylane/models/change_reverse_name_type.py
+-rw-r--r--   0        0        0     2095 2023-03-29 02:52:06.882665 binarylane_cli-0.16.0/lib/binarylane/models/change_separate_private_network_interface.py
+-rw-r--r--   0        0        0      274 2023-03-29 02:52:04.430651 binarylane_cli-0.16.0/lib/binarylane/models/change_separate_private_network_interface_type.py
+-rw-r--r--   0        0        0     7820 2023-03-29 02:52:06.870665 binarylane_cli-0.16.0/lib/binarylane/models/change_size_options_request.py
+-rw-r--r--   0        0        0     2052 2023-03-29 02:52:06.918665 binarylane_cli-0.16.0/lib/binarylane/models/change_source_and_destination_check.py
+-rw-r--r--   0        0        0      256 2023-03-29 02:52:04.386651 binarylane_cli-0.16.0/lib/binarylane/models/change_source_and_destination_check_type.py
+-rw-r--r--   0        0        0     2515 2023-03-29 02:52:07.010666 binarylane_cli-0.16.0/lib/binarylane/models/change_threshold_alerts.py
+-rw-r--r--   0        0        0      222 2023-03-29 02:52:04.494651 binarylane_cli-0.16.0/lib/binarylane/models/change_threshold_alerts_type.py
+-rw-r--r--   0        0        0     2281 2023-03-29 02:52:06.950666 binarylane_cli-0.16.0/lib/binarylane/models/change_vpc_ipv_4.py
+-rw-r--r--   0        0        0      198 2023-03-29 02:52:04.446651 binarylane_cli-0.16.0/lib/binarylane/models/change_vpc_ipv_4_type.py
+-rw-r--r--   0        0        0     2306 2023-03-29 02:52:05.862659 binarylane_cli-0.16.0/lib/binarylane/models/charge_information.py
+-rw-r--r--   0        0        0     2752 2023-03-29 02:52:06.846665 binarylane_cli-0.16.0/lib/binarylane/models/clone_using_backup.py
+-rw-r--r--   0        0        0      207 2023-03-29 02:52:04.350651 binarylane_cli-0.16.0/lib/binarylane/models/clone_using_backup_type.py
+-rw-r--r--   0        0        0     2354 2023-03-29 02:52:05.886659 binarylane_cli-0.16.0/lib/binarylane/models/console.py
+-rw-r--r--   0        0        0     1524 2023-03-29 02:52:06.998666 binarylane_cli-0.16.0/lib/binarylane/models/console_response.py
+-rw-r--r--   0        0        0     4825 2023-03-29 02:52:06.838665 binarylane_cli-0.16.0/lib/binarylane/models/create_load_balancer_request.py
+-rw-r--r--   0        0        0     1933 2023-03-29 02:52:06.946666 binarylane_cli-0.16.0/lib/binarylane/models/create_load_balancer_response.py
+-rw-r--r--   0        0        0     8213 2023-03-29 02:52:06.974666 binarylane_cli-0.16.0/lib/binarylane/models/create_server_request.py
+-rw-r--r--   0        0        0     1799 2023-03-29 02:52:06.966666 binarylane_cli-0.16.0/lib/binarylane/models/create_server_response.py
+-rw-r--r--   0        0        0     3204 2023-03-29 02:52:06.974666 binarylane_cli-0.16.0/lib/binarylane/models/create_vpc_request.py
+-rw-r--r--   0        0        0     1571 2023-03-29 02:52:05.914660 binarylane_cli-0.16.0/lib/binarylane/models/current_server_alerts_response.py
+-rw-r--r--   0        0        0      295 2023-03-29 02:52:04.366651 binarylane_cli-0.16.0/lib/binarylane/models/data_interval.py
+-rw-r--r--   0        0        0     3440 2023-03-29 02:52:05.910660 binarylane_cli-0.16.0/lib/binarylane/models/data_usage.py
+-rw-r--r--   0        0        0     1578 2023-03-29 02:52:06.978666 binarylane_cli-0.16.0/lib/binarylane/models/data_usage_response.py
+-rw-r--r--   0        0        0     2931 2023-03-29 02:52:06.950666 binarylane_cli-0.16.0/lib/binarylane/models/data_usages_response.py
+-rw-r--r--   0        0        0     1769 2023-03-29 02:52:06.898665 binarylane_cli-0.16.0/lib/binarylane/models/delete_disk.py
+-rw-r--r--   0        0        0      187 2023-03-29 02:52:04.442651 binarylane_cli-0.16.0/lib/binarylane/models/delete_disk_type.py
+-rw-r--r--   0        0        0     1553 2023-03-29 02:52:06.986666 binarylane_cli-0.16.0/lib/binarylane/models/detach_backup.py
+-rw-r--r--   0        0        0      193 2023-03-29 02:52:04.546652 binarylane_cli-0.16.0/lib/binarylane/models/detach_backup_type.py
+-rw-r--r--   0        0        0     1571 2023-03-29 02:52:06.862665 binarylane_cli-0.16.0/lib/binarylane/models/disable_backups.py
+-rw-r--r--   0        0        0      199 2023-03-29 02:52:04.366651 binarylane_cli-0.16.0/lib/binarylane/models/disable_backups_type.py
+-rw-r--r--   0        0        0     1562 2023-03-29 02:52:06.886665 binarylane_cli-0.16.0/lib/binarylane/models/disable_selinux.py
+-rw-r--r--   0        0        0      199 2023-03-29 02:52:04.522652 binarylane_cli-0.16.0/lib/binarylane/models/disable_selinux_type.py
+-rw-r--r--   0        0        0     2247 2023-03-29 02:52:06.878665 binarylane_cli-0.16.0/lib/binarylane/models/disk.py
+-rw-r--r--   0        0        0      242 2023-03-29 02:52:04.554652 binarylane_cli-0.16.0/lib/binarylane/models/distribution_feature.py
+-rw-r--r--   0        0        0     3740 2023-03-29 02:52:06.938665 binarylane_cli-0.16.0/lib/binarylane/models/distribution_info.py
+-rw-r--r--   0        0        0     4076 2023-03-29 02:52:07.002666 binarylane_cli-0.16.0/lib/binarylane/models/distribution_surcharges.py
+-rw-r--r--   0        0        0     2620 2023-03-29 02:52:06.946666 binarylane_cli-0.16.0/lib/binarylane/models/domain.py
+-rw-r--r--   0        0        0     4753 2023-03-29 02:52:07.010666 binarylane_cli-0.16.0/lib/binarylane/models/domain_record.py
+-rw-r--r--   0        0        0     4733 2023-03-29 02:52:06.934666 binarylane_cli-0.16.0/lib/binarylane/models/domain_record_request.py
+-rw-r--r--   0        0        0     1638 2023-03-29 02:52:06.878665 binarylane_cli-0.16.0/lib/binarylane/models/domain_record_response.py
+-rw-r--r--   0        0        0      299 2023-03-29 02:52:04.334650 binarylane_cli-0.16.0/lib/binarylane/models/domain_record_type.py
+-rw-r--r--   0        0        0     3027 2023-03-29 02:52:06.862665 binarylane_cli-0.16.0/lib/binarylane/models/domain_records_response.py
+-rw-r--r--   0        0        0     1902 2023-03-29 02:52:06.998666 binarylane_cli-0.16.0/lib/binarylane/models/domain_request.py
+-rw-r--r--   0        0        0     1504 2023-03-29 02:52:06.854665 binarylane_cli-0.16.0/lib/binarylane/models/domain_response.py
+-rw-r--r--   0        0        0     2809 2023-03-29 02:52:06.926665 binarylane_cli-0.16.0/lib/binarylane/models/domains_response.py
+-rw-r--r--   0        0        0     1570 2023-03-29 02:52:06.862665 binarylane_cli-0.16.0/lib/binarylane/models/enable_backups.py
+-rw-r--r--   0        0        0      196 2023-03-29 02:52:04.458651 binarylane_cli-0.16.0/lib/binarylane/models/enable_backups_type.py
+-rw-r--r--   0        0        0     1521 2023-03-29 02:52:06.954666 binarylane_cli-0.16.0/lib/binarylane/models/enable_ipv_6.py
+-rw-r--r--   0        0        0      187 2023-03-29 02:52:04.390651 binarylane_cli-0.16.0/lib/binarylane/models/enable_ipv_6_type.py
+-rw-r--r--   0        0        0     1736 2023-03-29 02:52:06.014660 binarylane_cli-0.16.0/lib/binarylane/models/failover_ips_request.py
+-rw-r--r--   0        0        0     2551 2023-03-29 02:52:06.838665 binarylane_cli-0.16.0/lib/binarylane/models/failover_ips_response.py
+-rw-r--r--   0        0        0     1778 2023-03-29 02:52:06.838665 binarylane_cli-0.16.0/lib/binarylane/models/forwarding_rule.py
+-rw-r--r--   0        0        0     2188 2023-03-29 02:52:06.886665 binarylane_cli-0.16.0/lib/binarylane/models/forwarding_rules_request.py
+-rw-r--r--   0        0        0     2366 2023-03-29 02:52:07.006666 binarylane_cli-0.16.0/lib/binarylane/models/health_check.py
+-rw-r--r--   0        0        0      216 2023-03-29 02:52:04.410651 binarylane_cli-0.16.0/lib/binarylane/models/health_check_protocol.py
+-rw-r--r--   0        0        0     2282 2023-03-29 02:52:06.938665 binarylane_cli-0.16.0/lib/binarylane/models/host.py
+-rw-r--r--   0        0        0    10687 2023-03-29 02:52:06.886665 binarylane_cli-0.16.0/lib/binarylane/models/image.py
+-rw-r--r--   0        0        0     2023 2023-03-29 02:52:06.086660 binarylane_cli-0.16.0/lib/binarylane/models/image_disk_download.py
+-rw-r--r--   0        0        0     2397 2023-03-29 02:52:06.878665 binarylane_cli-0.16.0/lib/binarylane/models/image_download.py
+-rw-r--r--   0        0        0     1558 2023-03-29 02:52:06.986666 binarylane_cli-0.16.0/lib/binarylane/models/image_download_response.py
+-rw-r--r--   0        0        0     3897 2023-03-29 02:52:06.930665 binarylane_cli-0.16.0/lib/binarylane/models/image_options.py
+-rw-r--r--   0        0        0      211 2023-03-29 02:52:04.294650 binarylane_cli-0.16.0/lib/binarylane/models/image_query_type.py
+-rw-r--r--   0        0        0     2106 2023-03-29 02:52:06.970666 binarylane_cli-0.16.0/lib/binarylane/models/image_request.py
+-rw-r--r--   0        0        0     1484 2023-03-29 02:52:06.942665 binarylane_cli-0.16.0/lib/binarylane/models/image_response.py
+-rw-r--r--   0        0        0      244 2023-03-29 02:52:04.526651 binarylane_cli-0.16.0/lib/binarylane/models/image_status.py
+-rw-r--r--   0        0        0      220 2023-03-29 02:52:04.506651 binarylane_cli-0.16.0/lib/binarylane/models/image_type.py
+-rw-r--r--   0        0        0     2777 2023-03-29 02:52:06.878665 binarylane_cli-0.16.0/lib/binarylane/models/images_response.py
+-rw-r--r--   0        0        0     6154 2023-03-29 02:52:06.966666 binarylane_cli-0.16.0/lib/binarylane/models/invoice.py
+-rw-r--r--   0        0        0     2398 2023-03-29 02:52:06.054660 binarylane_cli-0.16.0/lib/binarylane/models/invoice_line_item.py
+-rw-r--r--   0        0        0     1524 2023-03-29 02:52:06.890665 binarylane_cli-0.16.0/lib/binarylane/models/invoice_response.py
+-rw-r--r--   0        0        0     2841 2023-03-29 02:52:06.874665 binarylane_cli-0.16.0/lib/binarylane/models/invoices_response.py
+-rw-r--r--   0        0        0     1511 2023-03-29 02:52:06.966666 binarylane_cli-0.16.0/lib/binarylane/models/is_running.py
+-rw-r--r--   0        0        0      184 2023-03-29 02:52:04.454651 binarylane_cli-0.16.0/lib/binarylane/models/is_running_type.py
+-rw-r--r--   0        0        0     1981 2023-03-29 02:52:06.890665 binarylane_cli-0.16.0/lib/binarylane/models/kernel.py
+-rw-r--r--   0        0        0     2809 2023-03-29 02:52:06.914665 binarylane_cli-0.16.0/lib/binarylane/models/kernels_response.py
+-rw-r--r--   0        0        0     1651 2023-03-29 02:52:06.078661 binarylane_cli-0.16.0/lib/binarylane/models/license_.py
+-rw-r--r--   0        0        0     1854 2023-03-29 02:52:06.934666 binarylane_cli-0.16.0/lib/binarylane/models/licensed_software.py
+-rw-r--r--   0        0        0     3133 2023-03-29 02:52:06.990666 binarylane_cli-0.16.0/lib/binarylane/models/licensed_softwares_response.py
+-rw-r--r--   0        0        0     1554 2023-03-29 02:52:06.910665 binarylane_cli-0.16.0/lib/binarylane/models/links.py
+-rw-r--r--   0        0        0     5266 2023-03-29 02:52:06.914665 binarylane_cli-0.16.0/lib/binarylane/models/load_balancer.py
+-rw-r--r--   0        0        0     2768 2023-03-29 02:52:06.954666 binarylane_cli-0.16.0/lib/binarylane/models/load_balancer_availability_option.py
+-rw-r--r--   0        0        0     2645 2023-03-29 02:52:06.874665 binarylane_cli-0.16.0/lib/binarylane/models/load_balancer_availability_response.py
+-rw-r--r--   0        0        0     1638 2023-03-29 02:52:06.858665 binarylane_cli-0.16.0/lib/binarylane/models/load_balancer_response.py
+-rw-r--r--   0        0        0      203 2023-03-29 02:52:04.374651 binarylane_cli-0.16.0/lib/binarylane/models/load_balancer_rule_protocol.py
+-rw-r--r--   0        0        0      221 2023-03-29 02:52:04.550652 binarylane_cli-0.16.0/lib/binarylane/models/load_balancer_status.py
+-rw-r--r--   0        0        0     3027 2023-03-29 02:52:06.894665 binarylane_cli-0.16.0/lib/binarylane/models/load_balancers_response.py
+-rw-r--r--   0        0        0     1623 2023-03-29 02:52:06.122661 binarylane_cli-0.16.0/lib/binarylane/models/local_nameservers_response.py
+-rw-r--r--   0        0        0     1488 2023-03-29 02:52:06.126661 binarylane_cli-0.16.0/lib/binarylane/models/meta.py
+-rw-r--r--   0        0        0     3834 2023-03-29 02:52:06.962666 binarylane_cli-0.16.0/lib/binarylane/models/network.py
+-rw-r--r--   0        0        0      198 2023-03-29 02:52:04.534652 binarylane_cli-0.16.0/lib/binarylane/models/network_type.py
+-rw-r--r--   0        0        0     5171 2023-03-29 02:52:06.874665 binarylane_cli-0.16.0/lib/binarylane/models/networks.py
+-rw-r--r--   0        0        0     3058 2023-03-29 02:52:06.154661 binarylane_cli-0.16.0/lib/binarylane/models/offsite_backup_frequency_cost.py
+-rw-r--r--   0        0        0     3221 2023-03-29 02:52:06.930665 binarylane_cli-0.16.0/lib/binarylane/models/offsite_backup_settings.py
+-rw-r--r--   0        0        0     2550 2023-03-29 02:52:06.982666 binarylane_cli-0.16.0/lib/binarylane/models/pages.py
+-rw-r--r--   0        0        0      293 2023-03-29 02:52:04.550652 binarylane_cli-0.16.0/lib/binarylane/models/password_recovery_type.py
+-rw-r--r--   0        0        0     2987 2023-03-29 02:52:06.994666 binarylane_cli-0.16.0/lib/binarylane/models/password_reset.py
+-rw-r--r--   0        0        0      196 2023-03-29 02:52:04.358651 binarylane_cli-0.16.0/lib/binarylane/models/password_reset_type.py
+-rw-r--r--   0        0        0     2919 2023-03-29 02:52:06.854665 binarylane_cli-0.16.0/lib/binarylane/models/patch_vpc_request.py
+-rw-r--r--   0        0        0      208 2023-03-29 02:52:04.410651 binarylane_cli-0.16.0/lib/binarylane/models/payment_method.py
+-rw-r--r--   0        0        0     2463 2023-03-29 02:52:06.914665 binarylane_cli-0.16.0/lib/binarylane/models/period.py
+-rw-r--r--   0        0        0     1453 2023-03-29 02:52:06.978666 binarylane_cli-0.16.0/lib/binarylane/models/ping.py
+-rw-r--r--   0        0        0      167 2023-03-29 02:52:04.486651 binarylane_cli-0.16.0/lib/binarylane/models/ping_type.py
+-rw-r--r--   0        0        0     1523 2023-03-29 02:52:06.902665 binarylane_cli-0.16.0/lib/binarylane/models/power_cycle.py
+-rw-r--r--   0        0        0      187 2023-03-29 02:52:04.538652 binarylane_cli-0.16.0/lib/binarylane/models/power_cycle_type.py
+-rw-r--r--   0        0        0     1491 2023-03-29 02:52:06.918665 binarylane_cli-0.16.0/lib/binarylane/models/power_off.py
+-rw-r--r--   0        0        0      181 2023-03-29 02:52:04.326650 binarylane_cli-0.16.0/lib/binarylane/models/power_off_type.py
+-rw-r--r--   0        0        0     1480 2023-03-29 02:52:06.846665 binarylane_cli-0.16.0/lib/binarylane/models/power_on.py
+-rw-r--r--   0        0        0      178 2023-03-29 02:52:04.518652 binarylane_cli-0.16.0/lib/binarylane/models/power_on_type.py
+-rw-r--r--   0        0        0     2523 2023-03-29 02:52:06.914665 binarylane_cli-0.16.0/lib/binarylane/models/problem_details.py
+-rw-r--r--   0        0        0     1559 2023-03-29 02:52:06.194661 binarylane_cli-0.16.0/lib/binarylane/models/proceed_request.py
+-rw-r--r--   0        0        0     1994 2023-03-29 02:52:06.982666 binarylane_cli-0.16.0/lib/binarylane/models/processor_model.py
+-rw-r--r--   0        0        0     1482 2023-03-29 02:52:06.846665 binarylane_cli-0.16.0/lib/binarylane/models/reboot.py
+-rw-r--r--   0        0        0      173 2023-03-29 02:52:04.322651 binarylane_cli-0.16.0/lib/binarylane/models/reboot_type.py
+-rw-r--r--   0        0        0     3251 2023-03-29 02:52:06.994666 binarylane_cli-0.16.0/lib/binarylane/models/rebuild.py
+-rw-r--r--   0        0        0      176 2023-03-29 02:52:04.366651 binarylane_cli-0.16.0/lib/binarylane/models/rebuild_type.py
+-rw-r--r--   0        0        0     2647 2023-03-29 02:52:06.226661 binarylane_cli-0.16.0/lib/binarylane/models/region.py
+-rw-r--r--   0        0        0     2809 2023-03-29 02:52:06.970666 binarylane_cli-0.16.0/lib/binarylane/models/regions_response.py
+-rw-r--r--   0        0        0     1671 2023-03-29 02:52:06.938665 binarylane_cli-0.16.0/lib/binarylane/models/rename.py
+-rw-r--r--   0        0        0      173 2023-03-29 02:52:04.490651 binarylane_cli-0.16.0/lib/binarylane/models/rename_type.py
+-rw-r--r--   0        0        0     6138 2023-03-29 02:52:06.930665 binarylane_cli-0.16.0/lib/binarylane/models/resize.py
+-rw-r--r--   0        0        0     2158 2023-03-29 02:52:07.002666 binarylane_cli-0.16.0/lib/binarylane/models/resize_disk.py
+-rw-r--r--   0        0        0      187 2023-03-29 02:52:04.510651 binarylane_cli-0.16.0/lib/binarylane/models/resize_disk_type.py
+-rw-r--r--   0        0        0      173 2023-03-29 02:52:04.434651 binarylane_cli-0.16.0/lib/binarylane/models/resize_type.py
+-rw-r--r--   0        0        0      325 2023-03-29 02:52:04.410651 binarylane_cli-0.16.0/lib/binarylane/models/resource_type.py
+-rw-r--r--   0        0        0     1931 2023-03-29 02:52:06.986666 binarylane_cli-0.16.0/lib/binarylane/models/restore.py
+-rw-r--r--   0        0        0      176 2023-03-29 02:52:04.350651 binarylane_cli-0.16.0/lib/binarylane/models/restore_type.py
+-rw-r--r--   0        0        0     2659 2023-03-29 02:52:06.954666 binarylane_cli-0.16.0/lib/binarylane/models/reverse_name_servers_response.py
+-rw-r--r--   0        0        0     1815 2023-03-29 02:52:06.218661 binarylane_cli-0.16.0/lib/binarylane/models/reverse_nameservers_request.py
+-rw-r--r--   0        0        0     2175 2023-03-29 02:52:06.942665 binarylane_cli-0.16.0/lib/binarylane/models/route_entry.py
+-rw-r--r--   0        0        0     2213 2023-03-29 02:52:06.906665 binarylane_cli-0.16.0/lib/binarylane/models/route_entry_request.py
+-rw-r--r--   0        0        0     4965 2023-03-29 02:52:06.278662 binarylane_cli-0.16.0/lib/binarylane/models/sample.py
+-rw-r--r--   0        0        0     2938 2023-03-29 02:52:06.858665 binarylane_cli-0.16.0/lib/binarylane/models/sample_set.py
+-rw-r--r--   0        0        0     2078 2023-03-29 02:52:06.866665 binarylane_cli-0.16.0/lib/binarylane/models/sample_set_response.py
+-rw-r--r--   0        0        0     2931 2023-03-29 02:52:06.950666 binarylane_cli-0.16.0/lib/binarylane/models/sample_sets_response.py
+-rw-r--r--   0        0        0     3850 2023-03-29 02:52:06.286662 binarylane_cli-0.16.0/lib/binarylane/models/selected_size_options.py
+-rw-r--r--   0        0        0    13805 2023-03-29 02:52:06.958666 binarylane_cli-0.16.0/lib/binarylane/models/server.py
+-rw-r--r--   0        0        0     1535 2023-03-29 02:52:06.266662 binarylane_cli-0.16.0/lib/binarylane/models/server_ids_request.py
+-rw-r--r--   0        0        0     1504 2023-03-29 02:52:06.882665 binarylane_cli-0.16.0/lib/binarylane/models/server_response.py
+-rw-r--r--   0        0        0      231 2023-03-29 02:52:04.358651 binarylane_cli-0.16.0/lib/binarylane/models/server_status.py
+-rw-r--r--   0        0        0     2809 2023-03-29 02:52:06.978666 binarylane_cli-0.16.0/lib/binarylane/models/servers_response.py
+-rw-r--r--   0        0        0     1504 2023-03-29 02:52:06.982666 binarylane_cli-0.16.0/lib/binarylane/models/shutdown.py
+-rw-r--r--   0        0        0      179 2023-03-29 02:52:04.434651 binarylane_cli-0.16.0/lib/binarylane/models/shutdown_type.py
+-rw-r--r--   0        0        0     7284 2023-03-29 02:52:06.842665 binarylane_cli-0.16.0/lib/binarylane/models/size.py
+-rw-r--r--   0        0        0     9209 2023-03-29 02:52:06.866665 binarylane_cli-0.16.0/lib/binarylane/models/size_options.py
+-rw-r--r--   0        0        0     6754 2023-03-29 02:52:06.918665 binarylane_cli-0.16.0/lib/binarylane/models/size_options_request.py
+-rw-r--r--   0        0        0     2055 2023-03-29 02:52:06.982666 binarylane_cli-0.16.0/lib/binarylane/models/size_type.py
+-rw-r--r--   0        0        0     2745 2023-03-29 02:52:06.870665 binarylane_cli-0.16.0/lib/binarylane/models/sizes_response.py
+-rw-r--r--   0        0        0     2858 2023-03-29 02:52:06.986666 binarylane_cli-0.16.0/lib/binarylane/models/snapshots_response.py
+-rw-r--r--   0        0        0     4421 2023-03-29 02:52:06.922665 binarylane_cli-0.16.0/lib/binarylane/models/software.py
+-rw-r--r--   0        0        0     1544 2023-03-29 02:52:06.998666 binarylane_cli-0.16.0/lib/binarylane/models/software_response.py
+-rw-r--r--   0        0        0     2851 2023-03-29 02:52:06.994666 binarylane_cli-0.16.0/lib/binarylane/models/softwares_response.py
+-rw-r--r--   0        0        0     2548 2023-03-29 02:52:06.934666 binarylane_cli-0.16.0/lib/binarylane/models/ssh_key.py
+-rw-r--r--   0        0        0     2164 2023-03-29 02:52:06.842665 binarylane_cli-0.16.0/lib/binarylane/models/ssh_key_request.py
+-rw-r--r--   0        0        0     1518 2023-03-29 02:52:06.890665 binarylane_cli-0.16.0/lib/binarylane/models/ssh_key_response.py
+-rw-r--r--   0        0        0     2835 2023-03-29 02:52:06.838665 binarylane_cli-0.16.0/lib/binarylane/models/ssh_keys_response.py
+-rw-r--r--   0        0        0     3772 2023-03-29 02:52:06.878665 binarylane_cli-0.16.0/lib/binarylane/models/take_backup.py
+-rw-r--r--   0        0        0      187 2023-03-29 02:52:04.394651 binarylane_cli-0.16.0/lib/binarylane/models/take_backup_type.py
+-rw-r--r--   0        0        0     2538 2023-03-29 02:52:06.926665 binarylane_cli-0.16.0/lib/binarylane/models/tax_code.py
+-rw-r--r--   0        0        0      192 2023-03-29 02:52:04.410651 binarylane_cli-0.16.0/lib/binarylane/models/tax_code_type.py
+-rw-r--r--   0        0        0     6585 2023-03-29 02:52:06.946666 binarylane_cli-0.16.0/lib/binarylane/models/threshold_alert.py
+-rw-r--r--   0        0        0     4090 2023-03-29 02:52:06.842665 binarylane_cli-0.16.0/lib/binarylane/models/threshold_alert_request.py
+-rw-r--r--   0        0        0      413 2023-03-29 02:52:04.474651 binarylane_cli-0.16.0/lib/binarylane/models/threshold_alert_type.py
+-rw-r--r--   0        0        0     2089 2023-03-29 02:52:06.978666 binarylane_cli-0.16.0/lib/binarylane/models/threshold_alerts_response.py
+-rw-r--r--   0        0        0     1504 2023-03-29 02:52:06.882665 binarylane_cli-0.16.0/lib/binarylane/models/uncancel.py
+-rw-r--r--   0        0        0      179 2023-03-29 02:52:04.478651 binarylane_cli-0.16.0/lib/binarylane/models/uncancel_type.py
+-rw-r--r--   0        0        0     1905 2023-03-29 02:52:06.850665 binarylane_cli-0.16.0/lib/binarylane/models/unpaid_failed_invoices_response.py
+-rw-r--r--   0        0        0     4520 2023-03-29 02:52:06.946666 binarylane_cli-0.16.0/lib/binarylane/models/update_load_balancer_request.py
+-rw-r--r--   0        0        0     2416 2023-03-29 02:52:06.942665 binarylane_cli-0.16.0/lib/binarylane/models/update_load_balancer_response.py
+-rw-r--r--   0        0        0     2046 2023-03-29 02:52:06.990666 binarylane_cli-0.16.0/lib/binarylane/models/update_ssh_key_request.py
+-rw-r--r--   0        0        0     2751 2023-03-29 02:52:06.926665 binarylane_cli-0.16.0/lib/binarylane/models/update_vpc_request.py
+-rw-r--r--   0        0        0     3765 2023-03-29 02:52:06.902665 binarylane_cli-0.16.0/lib/binarylane/models/upload_image_request.py
+-rw-r--r--   0        0        0     1477 2023-03-29 02:52:06.882665 binarylane_cli-0.16.0/lib/binarylane/models/uptime.py
+-rw-r--r--   0        0        0      173 2023-03-29 02:52:04.498651 binarylane_cli-0.16.0/lib/binarylane/models/uptime_type.py
+-rw-r--r--   0        0        0     1596 2023-03-29 02:52:06.974666 binarylane_cli-0.16.0/lib/binarylane/models/user_data.py
+-rw-r--r--   0        0        0     2097 2023-03-29 02:52:06.946666 binarylane_cli-0.16.0/lib/binarylane/models/user_interaction_required.py
+-rw-r--r--   0        0        0      280 2023-03-29 02:52:04.402651 binarylane_cli-0.16.0/lib/binarylane/models/user_interaction_type.py
+-rw-r--r--   0        0        0     3139 2023-03-29 02:52:06.998666 binarylane_cli-0.16.0/lib/binarylane/models/validation_problem_details.py
+-rw-r--r--   0        0        0     1595 2023-04-21 00:20:59.977654 binarylane_cli-0.16.0/lib/binarylane/models/validation_problem_details_errors.py
+-rw-r--r--   0        0        0      266 2023-03-29 02:52:04.502652 binarylane_cli-0.16.0/lib/binarylane/models/video_device.py
+-rw-r--r--   0        0        0      420 2023-03-29 02:52:04.438651 binarylane_cli-0.16.0/lib/binarylane/models/vm_machine_type.py
+-rw-r--r--   0        0        0     2533 2023-03-29 02:52:06.846665 binarylane_cli-0.16.0/lib/binarylane/models/vpc.py
+-rw-r--r--   0        0        0     3260 2023-03-29 02:52:06.930665 binarylane_cli-0.16.0/lib/binarylane/models/vpc_member.py
+-rw-r--r--   0        0        0     2843 2023-03-29 02:52:06.962666 binarylane_cli-0.16.0/lib/binarylane/models/vpc_members_response.py
+-rw-r--r--   0        0        0     1444 2023-03-29 02:52:06.906665 binarylane_cli-0.16.0/lib/binarylane/models/vpc_response.py
+-rw-r--r--   0        0        0     2713 2023-03-29 02:52:06.910665 binarylane_cli-0.16.0/lib/binarylane/models/vpcs_response.py
+-rw-r--r--   0        0        0       25 2023-03-29 02:52:03.074643 binarylane_cli-0.16.0/lib/binarylane/py.typed
+-rw-r--r--   0        0        0     1028 2023-03-29 02:52:06.450663 binarylane_cli-0.16.0/lib/binarylane/types.py
+-rw-r--r--   0        0        0     3146 2023-04-21 00:28:52.078696 binarylane_cli-0.16.0/pyproject.toml
+-rw-r--r--   0        0        0     1933 2023-04-21 00:20:59.977654 binarylane_cli-0.16.0/src/binarylane/config/__init__.py
+-rw-r--r--   0        0        0     4083 2023-03-15 04:49:44.258009 binarylane_cli-0.16.0/src/binarylane/config/options.py
+-rw-r--r--   0        0        0     1539 2023-04-21 00:20:59.977654 binarylane_cli-0.16.0/src/binarylane/config/repository.py
+-rw-r--r--   0        0        0     4802 2023-03-15 04:49:44.258009 binarylane_cli-0.16.0/src/binarylane/config/sources.py
+-rw-r--r--   0        0        0        0 2023-02-07 09:32:33.869646 binarylane_cli-0.16.0/src/binarylane/console/__init__.py
+-rw-r--r--   0        0        0      619 2023-03-15 04:49:44.258009 binarylane_cli-0.16.0/src/binarylane/console/__main__.py
+-rw-r--r--   0        0        0     5831 2023-03-21 04:41:01.412051 binarylane_cli-0.16.0/src/binarylane/console/app.py
+-rw-r--r--   0        0        0      408 2023-03-15 04:49:44.258009 binarylane_cli-0.16.0/src/binarylane/console/commands/__init__.py
+-rw-r--r--   0        0        0    18051 2023-03-29 02:52:09.754682 binarylane_cli-0.16.0/src/binarylane/console/commands/api/__init__.py
+-rw-r--r--   0        0        0     1733 2023-03-29 03:05:42.879441 binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_account_keys_key_id.py
+-rw-r--r--   0        0        0     1723 2023-03-29 02:52:09.498680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_domains_domain_name.py
+-rw-r--r--   0        0        0     2159 2023-03-29 02:52:09.482680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_domains_domain_name_records_record_id.py
+-rw-r--r--   0        0        0     1800 2023-03-29 02:52:09.558681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id.py
+-rw-r--r--   0        0        0     3254 2023-03-29 02:52:09.574681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id_forwarding_rules.py
+-rw-r--r--   0        0        0     2605 2023-03-29 02:52:09.590681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id_servers.py
+-rw-r--r--   0        0        0     2410 2023-04-21 00:20:59.977654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_servers_server_id.py
+-rw-r--r--   0        0        0     1698 2023-03-29 02:52:09.822682 binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_vpcs_vpc_id.py
+-rw-r--r--   0        0        0     1231 2023-03-29 02:52:09.450680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_account.py
+-rw-r--r--   0        0        0     2992 2023-03-29 02:52:09.554681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_account_keys.py
+-rw-r--r--   0        0        0     1811 2023-03-29 03:05:42.879441 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_account_keys_key_id.py
+-rw-r--r--   0        0        0     4271 2023-03-29 02:52:09.486680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_actions.py
+-rw-r--r--   0        0        0     1780 2023-03-29 02:52:09.458680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_actions_action_id.py
+-rw-r--r--   0        0        0     1251 2023-03-29 02:52:09.446680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_customers_my_balance.py
+-rw-r--r--   0        0        0     4045 2023-03-29 02:52:09.486680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_customers_my_invoices.py
+-rw-r--r--   0        0        0     1829 2023-03-29 02:52:09.458680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_customers_my_invoices_invoice_id.py
+-rw-r--r--   0        0        0     3363 2023-03-29 02:52:09.482680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_customers_my_unpaid_payment_failed_invoices.py
+-rw-r--r--   0        0        0     3495 2023-03-29 02:52:09.486680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_data_usages_current.py
+-rw-r--r--   0        0        0     2112 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_data_usages_server_id_current.py
+-rw-r--r--   0        0        0     3332 2023-03-29 02:52:09.494680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_domains.py
+-rw-r--r--   0        0        0     1800 2023-03-29 02:52:09.466680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_domains_domain_name.py
+-rw-r--r--   0        0        0     6129 2023-03-29 02:52:09.566681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_domains_domain_name_records.py
+-rw-r--r--   0        0        0     2267 2023-03-29 02:52:09.486680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_domains_domain_name_records_record_id.py
+-rw-r--r--   0        0        0     1290 2023-03-29 02:52:09.470680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_domains_nameservers.py
+-rw-r--r--   0        0        0     2927 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_failover_ips_server_id.py
+-rw-r--r--   0        0        0     2948 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_failover_ips_server_id_available.py
+-rw-r--r--   0        0        0     6702 2023-03-29 02:52:09.578681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_images.py
+-rw-r--r--   0        0        0     1824 2023-03-29 02:52:09.530681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_images_image_id_download.py
+-rw-r--r--   0        0        0     1905 2023-03-29 03:05:42.879441 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_images_image_id_or_slug.py
+-rw-r--r--   0        0        0     3726 2023-03-29 02:52:09.582681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_load_balancers.py
+-rw-r--r--   0        0        0     2223 2023-03-29 02:52:09.566681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_load_balancers_availability.py
+-rw-r--r--   0        0        0     1908 2023-03-29 02:52:09.558681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_load_balancers_load_balancer_id.py
+-rw-r--r--   0        0        0     2908 2023-03-29 02:52:09.602681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_regions.py
+-rw-r--r--   0        0        0     2276 2023-03-29 02:52:09.590681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_reverse_names_ipv6.py
+-rw-r--r--   0        0        0     5936 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_samplesets_server_id.py
+-rw-r--r--   0        0        0     2772 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_samplesets_server_id_latest.py
+-rw-r--r--   0        0        0     6655 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers.py
+-rw-r--r--   0        0        0     2073 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id.py
+-rw-r--r--   0        0        0     5185 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_actions.py
+-rw-r--r--   0        0        0     2516 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_actions_action_id.py
+-rw-r--r--   0        0        0     3667 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_advanced_firewall_rules.py
+-rw-r--r--   0        0        0     2294 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_available_advanced_features.py
+-rw-r--r--   0        0        0     6506 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_backups.py
+-rw-r--r--   0        0        0     2292 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_console.py
+-rw-r--r--   0        0        0     3564 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_kernels.py
+-rw-r--r--   0        0        0     6556 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_snapshots.py
+-rw-r--r--   0        0        0     3613 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_software.py
+-rw-r--r--   0        0        0     5288 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_threshold_alerts.py
+-rw-r--r--   0        0        0     2116 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_user_data.py
+-rw-r--r--   0        0        0     1440 2023-03-29 02:52:09.798682 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_threshold_alerts.py
+-rw-r--r--   0        0        0     5807 2023-03-29 03:05:42.879441 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_sizes.py
+-rw-r--r--   0        0        0     3444 2023-03-29 02:52:09.858682 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_software.py
+-rw-r--r--   0        0        0     4469 2023-03-29 03:05:42.879441 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_software_operating_system_operating_system_id_or_slug.py
+-rw-r--r--   0        0        0     1775 2023-03-29 02:52:09.818682 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_software_software_id.py
+-rw-r--r--   0        0        0     2746 2023-03-29 02:52:09.850682 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_vpcs.py
+-rw-r--r--   0        0        0     1714 2023-03-29 02:52:09.834682 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_vpcs_vpc_id.py
+-rw-r--r--   0        0        0     4334 2023-03-29 02:52:09.886683 binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_vpcs_vpc_id_members.py
+-rw-r--r--   0        0        0     4070 2023-03-29 02:52:09.878682 binarylane_cli-0.16.0/src/binarylane/console/commands/api/patch_v2_vpcs_vpc_id.py
+-rw-r--r--   0        0        0     2666 2023-03-29 02:52:09.542681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_account_keys.py
+-rw-r--r--   0        0        0     2332 2023-03-29 02:52:09.466680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_actions_action_id_proceed.py
+-rw-r--r--   0        0        0     2337 2023-03-29 02:52:09.494680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_domains.py
+-rw-r--r--   0        0        0     5271 2023-03-29 02:52:09.538680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_domains_domain_name_records.py
+-rw-r--r--   0        0        0     1193 2023-03-29 02:52:09.490680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_domains_refresh_nameserver_cache.py
+-rw-r--r--   0        0        0     2996 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_failover_ips_server_id.py
+-rw-r--r--   0        0        0     5120 2023-03-29 02:52:09.602681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_load_balancers.py
+-rw-r--r--   0        0        0     3247 2023-03-29 02:52:09.586681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_load_balancers_load_balancer_id_forwarding_rules.py
+-rw-r--r--   0        0        0     2598 2023-03-29 02:52:09.578681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_load_balancers_load_balancer_id_servers.py
+-rw-r--r--   0        0        0     2316 2023-03-29 02:52:09.590681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_reverse_names_ipv6.py
+-rw-r--r--   0        0        0    12108 2023-03-29 02:52:09.918683 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_servers.py
+-rw-r--r--   0        0        0      827 2023-03-29 02:52:09.574681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_servers_server_id_actions.py
+-rw-r--r--   0        0        0     4462 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_servers_server_id_backups.py
+-rw-r--r--   0        0        0     3872 2023-03-29 02:52:09.874683 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_vpcs.py
+-rw-r--r--   0        0        0     3690 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_add_disk.py
+-rw-r--r--   0        0        0     3217 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_attach_backup.py
+-rw-r--r--   0        0        0     5656 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_advanced_features.py
+-rw-r--r--   0        0        0     6175 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_advanced_firewall_rules.py
+-rw-r--r--   0        0        0     4069 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_backup_schedule.py
+-rw-r--r--   0        0        0     3188 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_ipv_6.py
+-rw-r--r--   0        0        0     3547 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_ipv_6_reverse_nameservers.py
+-rw-r--r--   0        0        0     3195 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_kernel.py
+-rw-r--r--   0        0        0     3797 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_manage_offsite_backup_copies.py
+-rw-r--r--   0        0        0     3330 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_network.py
+-rw-r--r--   0        0        0     3656 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_offsite_backup_location.py
+-rw-r--r--   0        0        0     3372 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_partner.py
+-rw-r--r--   0        0        0     3278 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_port_blocking.py
+-rw-r--r--   0        0        0     3635 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_reverse_name.py
+-rw-r--r--   0        0        0     3506 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_separate_private_network_interface.py
+-rw-r--r--   0        0        0     3462 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_source_and_destination_check.py
+-rw-r--r--   0        0        0     6082 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_threshold_alerts.py
+-rw-r--r--   0        0        0     3601 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_vpc_ipv_4.py
+-rw-r--r--   0        0        0     4118 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_clone_using_backup.py
+-rw-r--r--   0        0        0     3213 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_delete_disk.py
+-rw-r--r--   0        0        0     2935 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_detach_backup.py
+-rw-r--r--   0        0        0     2955 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_disable_backups.py
+-rw-r--r--   0        0        0     2955 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_disable_selinux.py
+-rw-r--r--   0        0        0     2945 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_enable_backups.py
+-rw-r--r--   0        0        0     2918 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_enable_ipv_6.py
+-rw-r--r--   0        0        0     2905 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_is_running.py
+-rw-r--r--   0        0        0     4210 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_password_reset.py
+-rw-r--r--   0        0        0     2852 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_ping.py
+-rw-r--r--   0        0        0     2915 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_cycle.py
+-rw-r--r--   0        0        0     2895 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_off.py
+-rw-r--r--   0        0        0     2885 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_on.py
+-rw-r--r--   0        0        0     2872 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_reboot.py
+-rw-r--r--   0        0        0     5531 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_rebuild.py
+-rw-r--r--   0        0        0     3163 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_rename.py
+-rw-r--r--   0        0        0    16243 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_resize.py
+-rw-r--r--   0        0        0     3586 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_resize_disk.py
+-rw-r--r--   0        0        0     3200 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_restore.py
+-rw-r--r--   0        0        0     2892 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_shutdown.py
+-rw-r--r--   0        0        0     4441 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_take_backup.py
+-rw-r--r--   0        0        0     2892 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_uncancel.py
+-rw-r--r--   0        0        0     2872 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_uptime.py
+-rw-r--r--   0        0        0     3030 2023-03-29 03:05:42.879441 binarylane_cli-0.16.0/src/binarylane/console/commands/api/put_v2_account_keys_key_id.py
+-rw-r--r--   0        0        0     5642 2023-03-29 02:52:09.574681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/put_v2_domains_domain_name_records_record_id.py
+-rw-r--r--   0        0        0     3028 2023-03-29 02:52:09.538680 binarylane_cli-0.16.0/src/binarylane/console/commands/api/put_v2_images_image_id.py
+-rw-r--r--   0        0        0     5267 2023-03-29 02:52:09.618681 binarylane_cli-0.16.0/src/binarylane/console/commands/api/put_v2_load_balancers_load_balancer_id.py
+-rw-r--r--   0        0        0     3893 2023-03-29 02:52:09.882682 binarylane_cli-0.16.0/src/binarylane/console/commands/api/put_v2_vpcs_vpc_id.py
+-rw-r--r--   0        0        0     1987 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/commands/configure.py
+-rw-r--r--   0        0        0      295 2023-03-15 04:49:44.262009 binarylane_cli-0.16.0/src/binarylane/console/commands/version.py
+-rw-r--r--   0        0        0      476 2023-03-15 04:49:44.262009 binarylane_cli-0.16.0/src/binarylane/console/metadata.py
+-rw-r--r--   0        0        0      529 2023-03-15 04:49:44.262009 binarylane_cli-0.16.0/src/binarylane/console/parser/__init__.py
+-rw-r--r--   0        0        0     2592 2023-03-29 02:51:55.022597 binarylane_cli-0.16.0/src/binarylane/console/parser/attribute.py
+-rw-r--r--   0        0        0     1439 2023-02-07 09:32:33.873646 binarylane_cli-0.16.0/src/binarylane/console/parser/help_formatter.py
+-rw-r--r--   0        0        0     4785 2023-03-29 02:51:55.022597 binarylane_cli-0.16.0/src/binarylane/console/parser/list_attribute.py
+-rw-r--r--   0        0        0     4935 2023-03-29 02:51:55.022597 binarylane_cli-0.16.0/src/binarylane/console/parser/object_attribute.py
+-rw-r--r--   0        0        0     6131 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/parser/parser.py
+-rw-r--r--   0        0        0    11330 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/parser/primitive_attribute.py
+-rw-r--r--   0        0        0      940 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/printers/__init__.py
+-rw-r--r--   0        0        0     4406 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/printers/formatter.py
+-rw-r--r--   0        0        0      348 2023-02-17 22:36:19.051007 binarylane_cli-0.16.0/src/binarylane/console/printers/json_printer.py
+-rw-r--r--   0        0        0      486 2023-02-17 22:36:19.051007 binarylane_cli-0.16.0/src/binarylane/console/printers/plain_printer.py
+-rw-r--r--   0        0        0     1166 2023-02-17 22:36:19.051007 binarylane_cli-0.16.0/src/binarylane/console/printers/printer.py
+-rw-r--r--   0        0        0      621 2023-02-17 22:36:19.051007 binarylane_cli-0.16.0/src/binarylane/console/printers/table_printer.py
+-rw-r--r--   0        0        0      343 2023-02-17 22:36:19.051007 binarylane_cli-0.16.0/src/binarylane/console/printers/tsv_printer.py
+-rw-r--r--   0        0        0       25 2023-02-07 09:32:33.873646 binarylane_cli-0.16.0/src/binarylane/console/py.typed
+-rw-r--r--   0        0        0     3126 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/runners/__init__.py
+-rw-r--r--   0        0        0     3087 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/runners/action.py
+-rw-r--r--   0        0        0      765 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/runners/actionlink.py
+-rw-r--r--   0        0        0     5851 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/runners/command.py
+-rw-r--r--   0        0        0     2337 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/runners/httpx_wrapper.py
+-rw-r--r--   0        0        0     2671 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/runners/list.py
+-rw-r--r--   0        0        0      986 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/console/util.py
+-rw-r--r--   0        0        0      224 2023-02-07 09:32:33.873646 binarylane_cli-0.16.0/src/binarylane/pycompat/__init__.py
+-rw-r--r--   0        0        0     1966 2023-04-21 00:20:59.981654 binarylane_cli-0.16.0/src/binarylane/pycompat/actions.py
+-rw-r--r--   0        0        0      316 2023-02-07 09:32:33.873646 binarylane_cli-0.16.0/src/binarylane/pycompat/functools.py
+-rw-r--r--   0        0        0      394 2023-02-07 09:32:33.873646 binarylane_cli-0.16.0/src/binarylane/pycompat/importlib.py
+-rw-r--r--   0        0        0      474 2023-02-07 09:32:33.873646 binarylane_cli-0.16.0/src/binarylane/pycompat/shlex.py
+-rw-r--r--   0        0        0      362 2023-03-15 04:49:44.262009 binarylane_cli-0.16.0/src/binarylane/pycompat/typing.py
+-rw-r--r--   0        0        0    17253 1970-01-01 00:00:00.000000 binarylane_cli-0.16.0/PKG-INFO
```

### Comparing `binarylane_cli-0.15.3/LICENSE` & `binarylane_cli-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/README.md` & `binarylane_cli-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/accounts/get_v2_account.py` & `binarylane_cli-0.16.0/lib/binarylane/api/accounts/get_v2_account.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/actions/get_v2_actions.py` & `binarylane_cli-0.16.0/lib/binarylane/api/actions/get_v2_actions.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/actions/get_v2_actions_action_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/actions/get_v2_actions_action_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/actions/post_v2_actions_action_id_proceed.py` & `binarylane_cli-0.16.0/lib/binarylane/api/actions/post_v2_actions_action_id_proceed.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/customers/get_v2_customers_my_balance.py` & `binarylane_cli-0.16.0/lib/binarylane/api/customers/get_v2_customers_my_balance.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/customers/get_v2_customers_my_invoices.py` & `binarylane_cli-0.16.0/lib/binarylane/api/customers/get_v2_customers_my_invoices.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/customers/get_v2_customers_my_invoices_invoice_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/customers/get_v2_customers_my_invoices_invoice_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/customers/get_v2_customers_my_unpaid_payment_failed_invoices.py` & `binarylane_cli-0.16.0/lib/binarylane/api/customers/get_v2_customers_my_unpaid_payment_failed_invoices.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/data_usages/get_v2_data_usages_current.py` & `binarylane_cli-0.16.0/lib/binarylane/api/data_usages/get_v2_data_usages_current.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/data_usages/get_v2_data_usages_server_id_current.py` & `binarylane_cli-0.16.0/lib/binarylane/api/data_usages/get_v2_data_usages_server_id_current.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/delete_v2_domains_domain_name.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/delete_v2_domains_domain_name.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/delete_v2_domains_domain_name_records_record_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/delete_v2_domains_domain_name_records_record_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/get_v2_domains.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/get_v2_domains.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/get_v2_domains_domain_name.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/get_v2_domains_domain_name.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/get_v2_domains_domain_name_records.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/get_v2_domains_domain_name_records.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/get_v2_domains_domain_name_records_record_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/get_v2_domains_domain_name_records_record_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/get_v2_domains_nameservers.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/get_v2_domains_nameservers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/post_v2_domains.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/post_v2_domains.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/post_v2_domains_domain_name_records.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/post_v2_domains_domain_name_records.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/post_v2_domains_refresh_nameserver_cache.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/post_v2_domains_refresh_nameserver_cache.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/domains/put_v2_domains_domain_name_records_record_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/domains/put_v2_domains_domain_name_records_record_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/failover_ips/get_v2_failover_ips_server_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/failover_ips/get_v2_failover_ips_server_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/failover_ips/get_v2_failover_ips_server_id_available.py` & `binarylane_cli-0.16.0/lib/binarylane/api/failover_ips/get_v2_failover_ips_server_id_available.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/failover_ips/post_v2_failover_ips_server_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/failover_ips/post_v2_failover_ips_server_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/images/get_v2_images.py` & `binarylane_cli-0.16.0/lib/binarylane/api/images/get_v2_images.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/images/get_v2_images_image_id_download.py` & `binarylane_cli-0.16.0/lib/binarylane/api/images/get_v2_images_image_id_download.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/images/get_v2_images_image_id_or_slug.py` & `binarylane_cli-0.16.0/lib/binarylane/api/images/get_v2_images_image_id_or_slug.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/images/put_v2_images_image_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/images/put_v2_images_image_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/keys/delete_v2_account_keys_key_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/keys/delete_v2_account_keys_key_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/keys/get_v2_account_keys.py` & `binarylane_cli-0.16.0/lib/binarylane/api/keys/get_v2_account_keys.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/keys/get_v2_account_keys_key_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/keys/get_v2_account_keys_key_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/keys/post_v2_account_keys.py` & `binarylane_cli-0.16.0/lib/binarylane/api/keys/post_v2_account_keys.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/keys/put_v2_account_keys_key_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/keys/put_v2_account_keys_key_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id_forwarding_rules.py` & `binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id_servers.py` & `binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/delete_v2_load_balancers_load_balancer_id_servers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/get_v2_load_balancers.py` & `binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/get_v2_load_balancers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/get_v2_load_balancers_availability.py` & `binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/get_v2_load_balancers_availability.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/get_v2_load_balancers_load_balancer_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/get_v2_load_balancers_load_balancer_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/post_v2_load_balancers.py` & `binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/post_v2_load_balancers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/post_v2_load_balancers_load_balancer_id_forwarding_rules.py` & `binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/post_v2_load_balancers_load_balancer_id_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/post_v2_load_balancers_load_balancer_id_servers.py` & `binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/post_v2_load_balancers_load_balancer_id_servers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/load_balancers/put_v2_load_balancers_load_balancer_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/load_balancers/put_v2_load_balancers_load_balancer_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/regions/get_v2_regions.py` & `binarylane_cli-0.16.0/lib/binarylane/api/regions/get_v2_regions.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/reverse_names/get_v2_reverse_names_ipv6.py` & `binarylane_cli-0.16.0/lib/binarylane/api/reverse_names/get_v2_reverse_names_ipv6.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/reverse_names/post_v2_reverse_names_ipv6.py` & `binarylane_cli-0.16.0/lib/binarylane/api/reverse_names/post_v2_reverse_names_ipv6.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/sample_sets/get_v2_samplesets_server_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/sample_sets/get_v2_samplesets_server_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/sample_sets/get_v2_samplesets_server_id_latest.py` & `binarylane_cli-0.16.0/lib/binarylane/api/sample_sets/get_v2_samplesets_server_id_latest.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/get_v2_servers_server_id_actions.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/get_v2_servers_server_id_actions.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v2_servers_server_id_actions.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v2_servers_server_id_actions.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_add_disk.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_add_disk.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_attach_backup.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_attach_backup.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_advanced_features.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_advanced_features.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_advanced_firewall_rules.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_advanced_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_backup_schedule.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_backup_schedule.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_ipv_6.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_ipv_6.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_ipv_6_reverse_nameservers.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_ipv_6_reverse_nameservers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_kernel.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_kernel.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_manage_offsite_backup_copies.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_manage_offsite_backup_copies.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_network.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_network.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_offsite_backup_location.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_offsite_backup_location.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_partner.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_partner.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_port_blocking.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_port_blocking.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_reverse_name.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_reverse_name.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_separate_private_network_interface.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_separate_private_network_interface.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_source_and_destination_check.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_source_and_destination_check.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_threshold_alerts.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_threshold_alerts.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_vpc_ipv_4.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_change_vpc_ipv_4.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_clone_using_backup.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_clone_using_backup.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_delete_disk.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_delete_disk.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_detach_backup.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_detach_backup.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_disable_backups.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_disable_backups.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_disable_selinux.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_disable_selinux.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_enable_backups.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_enable_backups.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_enable_ipv_6.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_enable_ipv_6.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_is_running.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_is_running.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_password_reset.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_password_reset.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_ping.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_ping.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_cycle.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_cycle.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_off.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_off.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_on.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_power_on.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_reboot.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_reboot.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_rebuild.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_rebuild.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_rename.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_rename.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_resize.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_resize.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_resize_disk.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_resize_disk.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_restore.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_restore.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_shutdown.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_shutdown.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_take_backup.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_take_backup.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_uncancel.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_uncancel.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_uptime.py` & `binarylane_cli-0.16.0/lib/binarylane/api/server_actions/post_v_2_servers_server_id_actions_uptime.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/delete_v2_servers_server_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/delete_v2_servers_server_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_actions_action_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_actions_action_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_advanced_firewall_rules.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_advanced_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_available_advanced_features.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_available_advanced_features.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_backups.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_backups.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_console.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_console.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_kernels.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_kernels.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_snapshots.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_snapshots.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_software.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_software.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_threshold_alerts.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_threshold_alerts.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_server_id_user_data.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_server_id_user_data.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/get_v2_servers_threshold_alerts.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/get_v2_servers_threshold_alerts.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/post_v2_servers.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/post_v2_servers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/servers/post_v2_servers_server_id_backups.py` & `binarylane_cli-0.16.0/lib/binarylane/api/servers/post_v2_servers_server_id_backups.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/sizes/get_v2_sizes.py` & `binarylane_cli-0.16.0/lib/binarylane/api/sizes/get_v2_sizes.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/software/get_v2_software.py` & `binarylane_cli-0.16.0/lib/binarylane/api/software/get_v2_software.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/software/get_v2_software_operating_system_operating_system_id_or_slug.py` & `binarylane_cli-0.16.0/lib/binarylane/api/software/get_v2_software_operating_system_operating_system_id_or_slug.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/software/get_v2_software_software_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/software/get_v2_software_software_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/vpcs/delete_v2_vpcs_vpc_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/vpcs/delete_v2_vpcs_vpc_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/vpcs/get_v2_vpcs.py` & `binarylane_cli-0.16.0/lib/binarylane/api/vpcs/get_v2_vpcs.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/vpcs/get_v2_vpcs_vpc_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/vpcs/get_v2_vpcs_vpc_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/vpcs/get_v2_vpcs_vpc_id_members.py` & `binarylane_cli-0.16.0/lib/binarylane/api/vpcs/get_v2_vpcs_vpc_id_members.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/vpcs/patch_v2_vpcs_vpc_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/vpcs/patch_v2_vpcs_vpc_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/vpcs/post_v2_vpcs.py` & `binarylane_cli-0.16.0/lib/binarylane/api/vpcs/post_v2_vpcs.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/api/vpcs/put_v2_vpcs_vpc_id.py` & `binarylane_cli-0.16.0/lib/binarylane/api/vpcs/put_v2_vpcs_vpc_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/client.py` & `binarylane_cli-0.16.0/lib/binarylane/client.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/account.py` & `binarylane_cli-0.16.0/lib/binarylane/models/account.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/account_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/account_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/action.py` & `binarylane_cli-0.16.0/lib/binarylane/models/action.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/action_link.py` & `binarylane_cli-0.16.0/lib/binarylane/models/action_link.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/action_progress.py` & `binarylane_cli-0.16.0/lib/binarylane/models/action_progress.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/action_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/action_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/actions_links.py` & `binarylane_cli-0.16.0/lib/binarylane/models/actions_links.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/actions_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/actions_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/add_disk.py` & `binarylane_cli-0.16.0/lib/binarylane/models/add_disk.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/advanced_firewall_rule.py` & `binarylane_cli-0.16.0/lib/binarylane/models/advanced_firewall_rule.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/advanced_firewall_rules_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/advanced_firewall_rules_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/advanced_server_features.py` & `binarylane_cli-0.16.0/lib/binarylane/models/advanced_server_features.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/attach_backup.py` & `binarylane_cli-0.16.0/lib/binarylane/models/attach_backup.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/attached_backup.py` & `binarylane_cli-0.16.0/lib/binarylane/models/attached_backup.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/available_advanced_server_features.py` & `binarylane_cli-0.16.0/lib/binarylane/models/available_advanced_server_features.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/available_advanced_server_features_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/available_advanced_server_features_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/backup_disk.py` & `binarylane_cli-0.16.0/lib/binarylane/models/backup_disk.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/backup_info.py` & `binarylane_cli-0.16.0/lib/binarylane/models/backup_info.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/backup_settings.py` & `binarylane_cli-0.16.0/lib/binarylane/models/backup_settings.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/backup_window.py` & `binarylane_cli-0.16.0/lib/binarylane/models/backup_window.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/backups_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/backups_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/balance.py` & `binarylane_cli-0.16.0/lib/binarylane/models/balance.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/balance_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/balance_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_advanced_features.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_advanced_features.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_advanced_firewall_rules.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_advanced_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_backup_schedule.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_backup_schedule.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_image.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_image.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_ipv_6.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_ipv_6.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_ipv_6_reverse_nameservers.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_ipv_6_reverse_nameservers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_kernel.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_kernel.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_licenses.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_licenses.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_manage_offsite_backup_copies.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_manage_offsite_backup_copies.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_network.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_network.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_offsite_backup_location.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_offsite_backup_location.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_partner.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_partner.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_port_blocking.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_port_blocking.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_reverse_name.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_reverse_name.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_separate_private_network_interface.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_separate_private_network_interface.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_size_options_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_size_options_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_source_and_destination_check.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_source_and_destination_check.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_threshold_alerts.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_threshold_alerts.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/change_vpc_ipv_4.py` & `binarylane_cli-0.16.0/lib/binarylane/models/change_vpc_ipv_4.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/charge_information.py` & `binarylane_cli-0.16.0/lib/binarylane/models/charge_information.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/clone_using_backup.py` & `binarylane_cli-0.16.0/lib/binarylane/models/clone_using_backup.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/console.py` & `binarylane_cli-0.16.0/lib/binarylane/models/console.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/console_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/console_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/create_load_balancer_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/create_load_balancer_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/create_load_balancer_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/create_load_balancer_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/create_server_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/create_server_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/create_server_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/create_server_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/create_vpc_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/create_vpc_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/current_server_alerts_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/current_server_alerts_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/data_usage.py` & `binarylane_cli-0.16.0/lib/binarylane/models/data_usage.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/data_usage_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/data_usage_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/data_usages_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/data_usages_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/delete_disk.py` & `binarylane_cli-0.16.0/lib/binarylane/models/delete_disk.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/detach_backup.py` & `binarylane_cli-0.16.0/lib/binarylane/models/detach_backup.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/disable_backups.py` & `binarylane_cli-0.16.0/lib/binarylane/models/disable_backups.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/disable_selinux.py` & `binarylane_cli-0.16.0/lib/binarylane/models/disable_selinux.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/disk.py` & `binarylane_cli-0.16.0/lib/binarylane/models/disk.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/distribution_info.py` & `binarylane_cli-0.16.0/lib/binarylane/models/distribution_info.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/distribution_surcharges.py` & `binarylane_cli-0.16.0/lib/binarylane/models/distribution_surcharges.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/domain.py` & `binarylane_cli-0.16.0/lib/binarylane/models/domain.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/domain_record.py` & `binarylane_cli-0.16.0/lib/binarylane/models/domain_record.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/domain_record_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/domain_record_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/domain_record_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/domain_record_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/domain_records_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/domain_records_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/domain_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/domain_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/domain_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/domain_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/domains_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/domains_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/enable_backups.py` & `binarylane_cli-0.16.0/lib/binarylane/models/enable_backups.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/enable_ipv_6.py` & `binarylane_cli-0.16.0/lib/binarylane/models/enable_ipv_6.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/failover_ips_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/failover_ips_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/failover_ips_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/failover_ips_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/forwarding_rule.py` & `binarylane_cli-0.16.0/lib/binarylane/models/forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/forwarding_rules_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/forwarding_rules_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/health_check.py` & `binarylane_cli-0.16.0/lib/binarylane/models/health_check.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/host.py` & `binarylane_cli-0.16.0/lib/binarylane/models/host.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/image.py` & `binarylane_cli-0.16.0/lib/binarylane/models/image.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/image_disk_download.py` & `binarylane_cli-0.16.0/lib/binarylane/models/image_disk_download.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/image_download.py` & `binarylane_cli-0.16.0/lib/binarylane/models/image_download.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/image_download_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/image_download_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/image_options.py` & `binarylane_cli-0.16.0/lib/binarylane/models/image_options.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/image_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/image_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/image_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/image_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/images_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/images_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/invoice.py` & `binarylane_cli-0.16.0/lib/binarylane/models/invoice.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/invoice_line_item.py` & `binarylane_cli-0.16.0/lib/binarylane/models/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/invoice_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/invoice_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/invoices_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/invoices_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/is_running.py` & `binarylane_cli-0.16.0/lib/binarylane/models/is_running.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/kernel.py` & `binarylane_cli-0.16.0/lib/binarylane/models/kernel.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/kernels_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/kernels_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/license_.py` & `binarylane_cli-0.16.0/lib/binarylane/models/license_.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/licensed_software.py` & `binarylane_cli-0.16.0/lib/binarylane/models/licensed_software.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/licensed_softwares_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/licensed_softwares_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/links.py` & `binarylane_cli-0.16.0/lib/binarylane/models/links.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/load_balancer.py` & `binarylane_cli-0.16.0/lib/binarylane/models/load_balancer.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/load_balancer_availability_option.py` & `binarylane_cli-0.16.0/lib/binarylane/models/load_balancer_availability_option.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/load_balancer_availability_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/load_balancer_availability_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/load_balancer_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/load_balancer_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/load_balancers_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/load_balancers_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/local_nameservers_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/local_nameservers_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/meta.py` & `binarylane_cli-0.16.0/lib/binarylane/models/meta.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/network.py` & `binarylane_cli-0.16.0/lib/binarylane/models/network.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/networks.py` & `binarylane_cli-0.16.0/lib/binarylane/models/networks.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/offsite_backup_frequency_cost.py` & `binarylane_cli-0.16.0/lib/binarylane/models/offsite_backup_frequency_cost.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/offsite_backup_settings.py` & `binarylane_cli-0.16.0/lib/binarylane/models/offsite_backup_settings.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/pages.py` & `binarylane_cli-0.16.0/lib/binarylane/models/pages.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/password_reset.py` & `binarylane_cli-0.16.0/lib/binarylane/models/password_reset.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/patch_vpc_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/patch_vpc_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/period.py` & `binarylane_cli-0.16.0/lib/binarylane/models/period.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/ping.py` & `binarylane_cli-0.16.0/lib/binarylane/models/ping.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/power_cycle.py` & `binarylane_cli-0.16.0/lib/binarylane/models/power_cycle.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/power_off.py` & `binarylane_cli-0.16.0/lib/binarylane/models/power_off.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/power_on.py` & `binarylane_cli-0.16.0/lib/binarylane/models/power_on.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/problem_details.py` & `binarylane_cli-0.16.0/lib/binarylane/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/proceed_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/proceed_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/processor_model.py` & `binarylane_cli-0.16.0/lib/binarylane/models/processor_model.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/reboot.py` & `binarylane_cli-0.16.0/lib/binarylane/models/reboot.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/rebuild.py` & `binarylane_cli-0.16.0/lib/binarylane/models/rebuild.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/region.py` & `binarylane_cli-0.16.0/lib/binarylane/models/region.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/regions_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/regions_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/rename.py` & `binarylane_cli-0.16.0/lib/binarylane/models/rename.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/resize.py` & `binarylane_cli-0.16.0/lib/binarylane/models/resize.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/resize_disk.py` & `binarylane_cli-0.16.0/lib/binarylane/models/resize_disk.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/restore.py` & `binarylane_cli-0.16.0/lib/binarylane/models/restore.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/reverse_name_servers_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/reverse_name_servers_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/reverse_nameservers_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/reverse_nameservers_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/route_entry.py` & `binarylane_cli-0.16.0/lib/binarylane/models/route_entry.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/route_entry_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/route_entry_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/sample.py` & `binarylane_cli-0.16.0/lib/binarylane/models/sample.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/sample_set.py` & `binarylane_cli-0.16.0/lib/binarylane/models/sample_set.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/sample_set_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/sample_set_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/sample_sets_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/sample_sets_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/selected_size_options.py` & `binarylane_cli-0.16.0/lib/binarylane/models/selected_size_options.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/server.py` & `binarylane_cli-0.16.0/lib/binarylane/models/server.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/server_ids_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/server_ids_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/server_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/server_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/servers_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/servers_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/shutdown.py` & `binarylane_cli-0.16.0/lib/binarylane/models/shutdown.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/size.py` & `binarylane_cli-0.16.0/lib/binarylane/models/size.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/size_options.py` & `binarylane_cli-0.16.0/lib/binarylane/models/size_options.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/size_options_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/size_options_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/size_type.py` & `binarylane_cli-0.16.0/lib/binarylane/models/size_type.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/sizes_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/sizes_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/snapshots_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/snapshots_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/software.py` & `binarylane_cli-0.16.0/lib/binarylane/models/software.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/software_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/software_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/softwares_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/softwares_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/ssh_key.py` & `binarylane_cli-0.16.0/lib/binarylane/models/ssh_key.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/ssh_key_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/ssh_key_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/ssh_key_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/ssh_key_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/ssh_keys_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/ssh_keys_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/take_backup.py` & `binarylane_cli-0.16.0/lib/binarylane/models/take_backup.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/tax_code.py` & `binarylane_cli-0.16.0/lib/binarylane/models/tax_code.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/threshold_alert.py` & `binarylane_cli-0.16.0/lib/binarylane/models/threshold_alert.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/threshold_alert_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/threshold_alert_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/threshold_alerts_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/threshold_alerts_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/uncancel.py` & `binarylane_cli-0.16.0/lib/binarylane/models/uncancel.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/unpaid_failed_invoices_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/unpaid_failed_invoices_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/update_load_balancer_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/update_load_balancer_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/update_load_balancer_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/update_load_balancer_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/update_ssh_key_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/update_ssh_key_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/update_vpc_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/update_vpc_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/upload_image_request.py` & `binarylane_cli-0.16.0/lib/binarylane/models/upload_image_request.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/uptime.py` & `binarylane_cli-0.16.0/lib/binarylane/models/uptime.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/user_data.py` & `binarylane_cli-0.16.0/lib/binarylane/models/user_data.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/user_interaction_required.py` & `binarylane_cli-0.16.0/lib/binarylane/models/user_interaction_required.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/validation_problem_details.py` & `binarylane_cli-0.16.0/lib/binarylane/models/validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/validation_problem_details_errors.py` & `binarylane_cli-0.16.0/lib/binarylane/models/validation_problem_details_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 @attr.s(auto_attribs=True)
 class ValidationProblemDetailsErrors:
     """ """
 
     additional_properties: Dict[str, List[str]] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-
         field_dict: Dict[str, Any] = {}
         for prop_name, prop in self.additional_properties.items():
             field_dict[prop_name] = prop
 
         field_dict.update({})
 
         return field_dict
```

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/vpc.py` & `binarylane_cli-0.16.0/lib/binarylane/models/vpc.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/vpc_member.py` & `binarylane_cli-0.16.0/lib/binarylane/models/vpc_member.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/vpc_members_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/vpc_members_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/vpc_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/vpc_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/models/vpcs_response.py` & `binarylane_cli-0.16.0/lib/binarylane/models/vpcs_response.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/lib/binarylane/types.py` & `binarylane_cli-0.16.0/lib/binarylane/types.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/config/__init__.py` & `binarylane_cli-0.16.0/src/binarylane/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
-from argparse import Namespace
-from pathlib import Path
-from typing import Dict, Optional
+from typing import TYPE_CHECKING, Dict, Optional
 
 import binarylane.config.sources as src
 from binarylane.config.options import OptionAttributes, OptionName
 from binarylane.config.repository import Repository, Source
 
+if TYPE_CHECKING:
+    from argparse import Namespace
+    from pathlib import Path
+
 
 class _Config(Repository, OptionAttributes):
     def __init__(self) -> None:
         super().__init__(default_source=True)
 
 
 class DefaultConfig(_Config):
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/config/options.py` & `binarylane_cli-0.16.0/src/binarylane/config/options.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/config/repository.py` & `binarylane_cli-0.16.0/src/binarylane/config/repository.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
-from typing import List, Optional, Type, TypeVar
+from typing import TYPE_CHECKING, List, Optional, Type, TypeVar
 from binarylane.pycompat.typing import Protocol
 
 import binarylane.config.sources as src
-from binarylane.config.options import OptionName
+
+if TYPE_CHECKING:
+    from binarylane.config.options import OptionName
 
 
 class Source(Protocol):
     def get(self, name: str) -> Optional[str]:
         ...
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/config/sources.py` & `binarylane_cli-0.16.0/src/binarylane/config/sources.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/__main__.py` & `binarylane_cli-0.16.0/src/binarylane/console/__main__.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/app.py` & `binarylane_cli-0.16.0/src/binarylane/console/app.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/__init__.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/__init__.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_account_keys_key_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_account_keys_key_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_domains_domain_name.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_domains_domain_name.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_domains_domain_name_records_record_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_domains_domain_name_records_record_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id_forwarding_rules.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id_servers.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_load_balancers_load_balancer_id_servers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_servers_server_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_servers_server_id.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from binarylane.api.servers.delete_v2_servers_server_id import sync_detailed
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.types import UNSET, Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.command import CommandRunner
 
 
 class CommandRequest:
     server_id: int
     reason: Union[Unset, None, str] = UNSET
@@ -26,21 +27,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D/delete"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server to be cancelled.""",
+                metavar="server",
+                description="""The ID or name of the server to be cancelled.""",
+                lookup=lookup_server_id,
             )
         )
 
         mapping.add(
             PrimitiveAttribute(
                 "reason",
                 Union[Unset, None, str],
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/delete_v2_vpcs_vpc_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/delete_v2_vpcs_vpc_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_account.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_account.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_account_keys.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_account_keys.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_account_keys_key_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_account_keys_key_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_actions.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_actions.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_actions_action_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_actions_action_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_customers_my_balance.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_customers_my_balance.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_customers_my_invoices.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_customers_my_invoices.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_customers_my_invoices_invoice_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_customers_my_invoices_invoice_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_customers_my_unpaid_payment_failed_invoices.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_customers_my_unpaid_payment_failed_invoices.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_data_usages_current.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_data_usages_current.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_data_usages_server_id_current.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_user_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.data_usages.get_v2_data_usages_server_id_current import sync_detailed
-from binarylane.models.data_usage_response import DataUsageResponse
+from binarylane.api.servers.get_v2_servers_server_id_user_data import sync_detailed
 from binarylane.models.problem_details import ProblemDetails
+from binarylane.models.user_data import UserData
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.command import CommandRunner
 
 
 class CommandRequest:
     server_id: int
 
     def __init__(self, server_id: int) -> None:
         self.server_id = server_id
 
 
 class Command(CommandRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/DataUsages/paths/~1v2~1data_usages~1%7Bserver_id%7D~1current/get"
+        return (
+            "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1user_data/get"
+        )
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The target server id.""",
+                metavar="server",
+                description="""The ID or name of the server for which userdata should be fetched.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
-        return DataUsageResponse
+        return UserData
 
     def request(
         self,
         client: Client,
         request: object,
-    ) -> Tuple[HTTPStatus, Union[None, DataUsageResponse, ProblemDetails]]:
+    ) -> Tuple[HTTPStatus, Union[None, ProblemDetails, UserData]]:
         assert isinstance(request, CommandRequest)
 
-        # HTTPStatus.OK: DataUsageResponse
+        # HTTPStatus.OK: UserData
         # HTTPStatus.NOT_FOUND: ProblemDetails
         # HTTPStatus.UNAUTHORIZED: Any
         page_response = sync_detailed(
             server_id=request.server_id,
             client=client,
         )
         return page_response.status_code, page_response.parsed
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_domains.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_domains.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_domains_domain_name.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_domains_domain_name.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_domains_domain_name_records.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_domains_domain_name_records.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_domains_domain_name_records_record_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_domains_domain_name_records_record_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_domains_nameservers.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_domains_nameservers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_failover_ips_server_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_failover_ips_server_id_available.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Optional, Tuple, Union
 
-from binarylane.api.failover_ips.get_v2_failover_ips_server_id import sync_detailed
+from binarylane.api.failover_ips.get_v2_failover_ips_server_id_available import sync_detailed
 from binarylane.models.failover_ips_response import FailoverIpsResponse
 from binarylane.models.links import Links
 from binarylane.models.problem_details import ProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.command import CommandRunner
 
 
 class CommandRequest:
     server_id: int
 
     def __init__(self, server_id: int) -> None:
         self.server_id = server_id
 
 
 class Command(CommandRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/FailoverIps/paths/~1v2~1failover_ips~1%7Bserver_id%7D/get"
+        return "https://api.binarylane.com.au/reference/#tag/FailoverIps/paths/~1v2~1failover_ips~1%7Bserver_id%7D~1available/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The target server id.""",
+                metavar="server",
+                description="""The target server id or name.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_failover_ips_server_id_available.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_failover_ips_server_id.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 from __future__ import annotations
 
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Optional, Tuple, Union
+from typing import TYPE_CHECKING, List, Tuple, Union
 
-from binarylane.api.failover_ips.get_v2_failover_ips_server_id_available import sync_detailed
-from binarylane.models.failover_ips_response import FailoverIpsResponse
-from binarylane.models.links import Links
+from binarylane.api.failover_ips.post_v2_failover_ips_server_id import sync_detailed
+from binarylane.models.action_response import ActionResponse
+from binarylane.models.failover_ips_request import FailoverIpsRequest
 from binarylane.models.problem_details import ProblemDetails
+from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
-from binarylane.console.runners.command import CommandRunner
+from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
+    json_body: FailoverIpsRequest
 
-    def __init__(self, server_id: int) -> None:
+    def __init__(self, server_id: int, json_body: FailoverIpsRequest) -> None:
         self.server_id = server_id
+        self.json_body = json_body
 
 
-class Command(CommandRunner):
+class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/FailoverIps/paths/~1v2~1failover_ips~1%7Bserver_id%7D~1available/get"
+        return "https://api.binarylane.com.au/reference/#tag/FailoverIps/paths/~1v2~1failover_ips~1%7Bserver_id%7D/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The target server id.""",
+                metavar="server",
+                description="""The target server id or name.""",
+                lookup=lookup_server_id,
+            )
+        )
+
+        json_body = mapping.add_json_body(FailoverIpsRequest)
+
+        json_body.add(
+            PrimitiveAttribute(
+                "failover_ips",
+                List[str],
+                required=True,
+                option_name="failover-ips",
+                description="""The list of failover IP addresses to assign to this server. This overwrites the current list, so any current failover IP addresses that are omitted will be removed from the server.""",
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
-        return FailoverIpsResponse
+        return ActionResponse
 
     def request(
         self,
         client: Client,
         request: object,
-    ) -> Tuple[HTTPStatus, Union[None, FailoverIpsResponse, ProblemDetails]]:
+    ) -> Tuple[HTTPStatus, Union[ActionResponse, None, ProblemDetails, ValidationProblemDetails]]:
         assert isinstance(request, CommandRequest)
 
-        # HTTPStatus.OK: FailoverIpsResponse
+        # HTTPStatus.OK: ActionResponse
+        # HTTPStatus.NO_CONTENT: Any
+        # HTTPStatus.BAD_REQUEST: ValidationProblemDetails
         # HTTPStatus.NOT_FOUND: ProblemDetails
         # HTTPStatus.UNAUTHORIZED: Any
-        page = 0
-        per_page = 25
-        has_next = True
-        response: Optional[FailoverIpsResponse] = None
-
-        while has_next:
-            page += 1
-            page_response = sync_detailed(
-                server_id=request.server_id,
-                client=client,
-                page=page,
-                per_page=per_page,
-            )
-
-            status_code = page_response.status_code
-            if status_code != 200:
-                return status_code, page_response.parsed
-
-            assert isinstance(page_response.parsed, FailoverIpsResponse)
-            has_next = isinstance(page_response.parsed.links, Links) and isinstance(
-                page_response.parsed.links.pages.next_, str
-            )
-            if not response:
-                response = page_response.parsed
-            else:
-                response.failover_ips += page_response.parsed.failover_ips
-
-        return status_code, response
+        page_response = sync_detailed(
+            server_id=request.server_id,
+            client=client,
+            json_body=request.json_body,
+        )
+        return page_response.status_code, page_response.parsed
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_images.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_images.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_images_image_id_download.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_images_image_id_download.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_images_image_id_or_slug.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_images_image_id_or_slug.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_load_balancers.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_load_balancers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_load_balancers_availability.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_load_balancers_availability.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_load_balancers_load_balancer_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_load_balancers_load_balancer_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_regions.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_regions.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_reverse_names_ipv6.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_reverse_names_ipv6.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_samplesets_server_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_samplesets_server_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from binarylane.models.sample_sets_response import SampleSetsResponse
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import UNSET, Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.list import ListRunner
 
 
 class CommandRequest:
     server_id: int
     data_interval: Union[Unset, None, DataInterval] = UNSET
@@ -57,21 +58,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/SampleSets/paths/~1v2~1samplesets~1%7Bserver_id%7D/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The target server id.""",
+                metavar="server",
+                description="""The target server id or name.""",
+                lookup=lookup_server_id,
             )
         )
 
         mapping.add(
             PrimitiveAttribute(
                 "data_interval",
                 Union[Unset, None, DataInterval],
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_samplesets_server_id_latest.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_samplesets_server_id_latest.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.sample_set_response import SampleSetResponse
 from binarylane.types import UNSET, Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.command import CommandRunner
 
 
 class CommandRequest:
     server_id: int
     data_interval: Union[Unset, None, DataInterval] = UNSET
@@ -28,21 +29,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/SampleSets/paths/~1v2~1samplesets~1%7Bserver_id%7D~1latest/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The target server id.""",
+                metavar="server",
+                description="""The target server id or name.""",
+                lookup=lookup_server_id,
             )
         )
 
         mapping.add(
             PrimitiveAttribute(
                 "data_interval",
                 Union[Unset, None, DataInterval],
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 from binarylane.api.servers.get_v2_servers import sync_detailed
 from binarylane.models.links import Links
 from binarylane.models.servers_response import ServersResponse
 from binarylane.types import UNSET, Unset
 
+from binarylane.console.util import create_client
+
 if TYPE_CHECKING:
     from binarylane.client import Client
 
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.list import ListRunner
 
 
@@ -76,14 +78,26 @@
             "next_backup_window": """The details of the next scheduled backup, if any.""",
             "cancelled_at": """If the server has been cancelled, this is the date and time in ISO8601 format of that cancellation.""",
             "partner_id": """The server ID of the partner of this server, if one has been assigned.""",
             "permalink": """A randomly generated two-word identifier assigned to servers in regions that support this feature.""",
             "attached_backup": """An object that provides details of any backup image currently attached to the server..""",
         }
 
+    def lookup(self, ref: str) -> Optional[int]:
+        status_code, received = self.request(create_client(self._context), CommandRequest())
+        if status_code != 200:
+            super().response(status_code, received)
+
+        assert isinstance(received, ServersResponse)
+        for item in received.servers:
+            if item.name == ref:
+                return item.id
+        else:
+            return None
+
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from binarylane.api.servers.get_v2_servers_server_id import sync_detailed
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.server_response import ServerResponse
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.command import CommandRunner
 
 
 class CommandRequest:
     server_id: int
 
@@ -25,21 +26,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server to fetch.""",
+                metavar="server",
+                description="""The ID or name of the server to fetch.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_actions.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from binarylane.models.actions_response import ActionsResponse
 from binarylane.models.links import Links
 from binarylane.models.problem_details import ProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.list import ListRunner
 
 
 class CommandRequest:
     server_id: int
 
@@ -69,21 +70,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which actions should be listed.""",
+                metavar="server",
+                description="""The ID or name of the server for which actions should be listed.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_actions_action_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_actions_action_id.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from binarylane.api.servers.get_v2_servers_server_id_actions_action_id import sync_detailed
 from binarylane.models.action_response import ActionResponse
 from binarylane.models.problem_details import ProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.command import CommandRunner
 
 
 class CommandRequest:
     server_id: int
     action_id: int
@@ -27,21 +28,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1actions~1%7Baction_id%7D/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which the action should be fetched.""",
+                metavar="server",
+                description="""The ID or name of the server for which the action should be fetched.""",
+                lookup=lookup_server_id,
             )
         )
         mapping.add(
             PrimitiveAttribute(
                 "action_id",
                 int,
                 required=True,
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_advanced_firewall_rules.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_advanced_firewall_rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from binarylane.api.servers.get_v2_servers_server_id_advanced_firewall_rules import sync_detailed
 from binarylane.models.advanced_firewall_rules_response import AdvancedFirewallRulesResponse
 from binarylane.models.problem_details import ProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.list import ListRunner
 
 
 class CommandRequest:
     server_id: int
 
@@ -53,21 +54,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1advanced_firewall_rules/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which firewall rules should be listed.""",
+                metavar="server",
+                description="""The ID or name of the server for which firewall rules should be listed.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_available_advanced_features.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_available_advanced_features.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from binarylane.api.servers.get_v2_servers_server_id_available_advanced_features import sync_detailed
 from binarylane.models.available_advanced_server_features_response import AvailableAdvancedServerFeaturesResponse
 from binarylane.models.problem_details import ProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.command import CommandRunner
 
 
 class CommandRequest:
     server_id: int
 
@@ -25,21 +26,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1available_advanced_features/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which advanced features should be listed.""",
+                metavar="server",
+                description="""The ID or name of the server for which advanced features should be listed.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_backups.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_backups.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from binarylane.models.backups_response import BackupsResponse
 from binarylane.models.links import Links
 from binarylane.models.problem_details import ProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.list import ListRunner
 
 
 class CommandRequest:
     server_id: int
 
@@ -79,21 +80,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1backups/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which backups should be listed.""",
+                metavar="server",
+                description="""The ID or name of the server for which backups should be listed.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_console.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_console.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from binarylane.models.console_response import ConsoleResponse
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.command import CommandRunner
 
 
 class CommandRequest:
     server_id: int
 
@@ -26,21 +27,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1console/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which console URLs will be fetched.""",
+                metavar="server",
+                description="""The ID or name of the server for which console URLs will be fetched.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_kernels.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_kernels.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from binarylane.models.kernels_response import KernelsResponse
 from binarylane.models.links import Links
 from binarylane.models.problem_details import ProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.list import ListRunner
 
 
 class CommandRequest:
     server_id: int
 
@@ -48,21 +49,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1kernels/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which kernels should be listed.""",
+                metavar="server",
+                description="""The ID or name of the server for which kernels should be listed.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_snapshots.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_snapshots.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from binarylane.models.links import Links
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.snapshots_response import SnapshotsResponse
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.list import ListRunner
 
 
 class CommandRequest:
     server_id: int
 
@@ -81,21 +82,26 @@
         return (
             "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1snapshots/get"
         )
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which snapshots should be listed.""",
+                metavar="server",
+                description="""The ID or name of the server for which snapshots should be listed.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_software.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_software.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from binarylane.models.licensed_softwares_response import LicensedSoftwaresResponse
 from binarylane.models.links import Links
 from binarylane.models.problem_details import ProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.list import ListRunner
 
 
 class CommandRequest:
     server_id: int
 
@@ -45,21 +46,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1software/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which software should be fetched.""",
+                metavar="server",
+                description="""The ID or name of the server for which software should be fetched.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_threshold_alerts.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_server_id_threshold_alerts.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from binarylane.api.servers.get_v2_servers_server_id_threshold_alerts import sync_detailed
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.threshold_alerts_response import ThresholdAlertsResponse
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.list import ListRunner
 
 
 class CommandRequest:
     server_id: int
 
@@ -61,21 +62,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1threshold_alerts/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which threshold alerts should be fetched.""",
+                metavar="server",
+                description="""The ID or name of the server for which threshold alerts should be fetched.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_server_id_user_data.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_data_usages_server_id_current.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.servers.get_v2_servers_server_id_user_data import sync_detailed
+from binarylane.api.data_usages.get_v2_data_usages_server_id_current import sync_detailed
+from binarylane.models.data_usage_response import DataUsageResponse
 from binarylane.models.problem_details import ProblemDetails
-from binarylane.models.user_data import UserData
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.command import CommandRunner
 
 
 class CommandRequest:
     server_id: int
 
     def __init__(self, server_id: int) -> None:
         self.server_id = server_id
 
 
 class Command(CommandRunner):
     @property
     def reference_url(self) -> str:
-        return (
-            "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1user_data/get"
-        )
+        return "https://api.binarylane.com.au/reference/#tag/DataUsages/paths/~1v2~1data_usages~1%7Bserver_id%7D~1current/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which userdata should be fetched.""",
+                metavar="server",
+                description="""The target server id or name.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
-        return UserData
+        return DataUsageResponse
 
     def request(
         self,
         client: Client,
         request: object,
-    ) -> Tuple[HTTPStatus, Union[None, ProblemDetails, UserData]]:
+    ) -> Tuple[HTTPStatus, Union[None, DataUsageResponse, ProblemDetails]]:
         assert isinstance(request, CommandRequest)
 
-        # HTTPStatus.OK: UserData
+        # HTTPStatus.OK: DataUsageResponse
         # HTTPStatus.NOT_FOUND: ProblemDetails
         # HTTPStatus.UNAUTHORIZED: Any
         page_response = sync_detailed(
             server_id=request.server_id,
             client=client,
         )
         return page_response.status_code, page_response.parsed
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_servers_threshold_alerts.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_servers_threshold_alerts.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_sizes.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_sizes.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_software.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_software.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_software_operating_system_operating_system_id_or_slug.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_software_operating_system_operating_system_id_or_slug.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_software_software_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_software_software_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_vpcs.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_vpcs.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_vpcs_vpc_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_vpcs_vpc_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/get_v2_vpcs_vpc_id_members.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_vpcs_vpc_id_members.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/patch_v2_vpcs_vpc_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/patch_v2_vpcs_vpc_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_account_keys.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_account_keys.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_actions_action_id_proceed.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_actions_action_id_proceed.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_domains.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_domains.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_domains_domain_name_records.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_domains_domain_name_records.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_domains_refresh_nameserver_cache.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_domains_refresh_nameserver_cache.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_failover_ips_server_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_is_running.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 from __future__ import annotations
 
 from http import HTTPStatus
-from typing import TYPE_CHECKING, List, Tuple, Union
+from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.failover_ips.post_v2_failover_ips_server_id import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_is_running import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.failover_ips_request import FailoverIpsRequest
+from binarylane.models.is_running import IsRunning
+from binarylane.models.is_running_type import IsRunningType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: FailoverIpsRequest
+    json_body: IsRunning
 
-    def __init__(self, server_id: int, json_body: FailoverIpsRequest) -> None:
+    def __init__(self, server_id: int, json_body: IsRunning) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/FailoverIps/paths/~1v2~1failover_ips~1%7Bserver_id%7D/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#IsRunning/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The target server id.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(FailoverIpsRequest)
+        json_body = mapping.add_json_body(IsRunning)
 
         json_body.add(
             PrimitiveAttribute(
-                "failover_ips",
-                List[str],
+                "type",
+                IsRunningType,
                 required=True,
-                option_name="failover-ips",
-                description="""The list of failover IP addresses to assign to this server. This overwrites the current list, so any current failover IP addresses that are omitted will be removed from the server.""",
+                option_name="type",
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
@@ -65,17 +71,18 @@
         self,
         client: Client,
         request: object,
     ) -> Tuple[HTTPStatus, Union[ActionResponse, None, ProblemDetails, ValidationProblemDetails]]:
         assert isinstance(request, CommandRequest)
 
         # HTTPStatus.OK: ActionResponse
-        # HTTPStatus.NO_CONTENT: Any
+        # HTTPStatus.ACCEPTED: Any
         # HTTPStatus.BAD_REQUEST: ValidationProblemDetails
         # HTTPStatus.NOT_FOUND: ProblemDetails
+        # HTTPStatus.UNPROCESSABLE_ENTITY: ProblemDetails
         # HTTPStatus.UNAUTHORIZED: Any
         page_response = sync_detailed(
             server_id=request.server_id,
             client=client,
             json_body=request.json_body,
         )
         return page_response.status_code, page_response.parsed
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_load_balancers.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_load_balancers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_load_balancers_load_balancer_id_forwarding_rules.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_load_balancers_load_balancer_id_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_load_balancers_load_balancer_id_servers.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_load_balancers_load_balancer_id_servers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_reverse_names_ipv6.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_reverse_names_ipv6.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_servers.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_servers.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_servers_server_id_actions.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_servers_server_id_actions.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_servers_server_id_backups.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_servers_server_id_backups.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from binarylane.models.upload_image_request import UploadImageRequest
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: UploadImageRequest
@@ -32,21 +33,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/Servers/paths/~1v2~1servers~1%7Bserver_id%7D~1backups/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server for which the backup is to be uploaded.""",
+                metavar="server",
+                description="""The ID or name of the server for which the backup is to be uploaded.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(UploadImageRequest)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v2_vpcs.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v2_vpcs.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_add_disk.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_ping.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,70 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_add_disk import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_ping import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.add_disk import AddDisk
-from binarylane.models.add_disk_type import AddDiskType
+from binarylane.models.ping import Ping
+from binarylane.models.ping_type import PingType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
-from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: AddDisk
+    json_body: Ping
 
-    def __init__(self, server_id: int, json_body: AddDisk) -> None:
+    def __init__(self, server_id: int, json_body: Ping) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#AddDisk/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Ping/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(AddDisk)
+        json_body = mapping.add_json_body(Ping)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                AddDiskType,
+                PingType,
                 required=True,
                 option_name="type",
             )
         )
 
-        json_body.add(
-            PrimitiveAttribute(
-                "size_gigabytes",
-                int,
-                required=True,
-                option_name="size-gigabytes",
-                description="""The size of the new disk in GB. The server must have at least this much unallocated storage space.""",
-            )
-        )
-
-        json_body.add(
-            PrimitiveAttribute(
-                "description",
-                Union[Unset, None, str],
-                required=False,
-                option_name="description",
-                description="""An optional description for the disk. If this is null a default description will be added. Submit an empty string to prevent the default description being added.""",
-            )
-        )
-
         return mapping
 
     @property
     def ok_response_type(self) -> type:
         return ActionResponse
 
     def request(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_attach_backup.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_attach_backup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from binarylane.models.attach_backup_type import AttachBackupType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: AttachBackup
@@ -30,21 +31,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#AttachBackup/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(AttachBackup)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_advanced_features.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_advanced_features.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from binarylane.models.video_device import VideoDevice
 from binarylane.models.vm_machine_type import VmMachineType
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeAdvancedFeatures
@@ -34,21 +35,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeAdvancedFeatures/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeAdvancedFeatures)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_advanced_firewall_rules.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_advanced_firewall_rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import ListAttribute, Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeAdvancedFirewallRules
@@ -36,21 +37,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeAdvancedFirewallRules/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeAdvancedFirewallRules)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_backup_schedule.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_backup_schedule.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeBackupSchedule
@@ -31,21 +32,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeBackupSchedule/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeBackupSchedule)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_ipv_6.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_ipv_6.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from binarylane.models.change_ipv_6_type import ChangeIpv6Type
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeIpv6
@@ -30,21 +31,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeIpv6/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeIpv6)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_ipv_6_reverse_nameservers.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_ipv_6_reverse_nameservers.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from binarylane.models.change_ipv_6_reverse_nameservers_type import ChangeIpv6ReverseNameserversType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeIpv6ReverseNameservers
@@ -32,21 +33,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeIpv6ReverseNameservers/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeIpv6ReverseNameservers)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_kernel.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_uptime.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_change_kernel import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_uptime import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.change_kernel import ChangeKernel
-from binarylane.models.change_kernel_type import ChangeKernelType
 from binarylane.models.problem_details import ProblemDetails
+from binarylane.models.uptime import Uptime
+from binarylane.models.uptime_type import UptimeType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: ChangeKernel
+    json_body: Uptime
 
-    def __init__(self, server_id: int, json_body: ChangeKernel) -> None:
+    def __init__(self, server_id: int, json_body: Uptime) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeKernel/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Uptime/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(ChangeKernel)
+        json_body = mapping.add_json_body(Uptime)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                ChangeKernelType,
+                UptimeType,
                 required=True,
                 option_name="type",
             )
         )
 
-        json_body.add(
-            PrimitiveAttribute(
-                "kernel",
-                int,
-                required=True,
-                option_name="kernel",
-                description="""The ID of the kernel to use.""",
-            )
-        )
-
         return mapping
 
     @property
     def ok_response_type(self) -> type:
         return ActionResponse
 
     def request(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_manage_offsite_backup_copies.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_manage_offsite_backup_copies.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from binarylane.models.change_manage_offsite_backup_copies_type import ChangeManageOffsiteBackupCopiesType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeManageOffsiteBackupCopies
@@ -32,21 +33,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeManageOffsiteBackupCopies/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeManageOffsiteBackupCopies)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_network.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeNetwork
@@ -31,21 +32,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeNetwork/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeNetwork)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_offsite_backup_location.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_offsite_backup_location.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeOffsiteBackupLocation
@@ -33,21 +34,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeOffsiteBackupLocation/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeOffsiteBackupLocation)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_partner.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_partner.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangePartner
@@ -31,21 +32,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangePartner/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangePartner)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_port_blocking.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_reboot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_change_port_blocking import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_reboot import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.change_port_blocking import ChangePortBlocking
-from binarylane.models.change_port_blocking_type import ChangePortBlockingType
 from binarylane.models.problem_details import ProblemDetails
+from binarylane.models.reboot import Reboot
+from binarylane.models.reboot_type import RebootType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: ChangePortBlocking
+    json_body: Reboot
 
-    def __init__(self, server_id: int, json_body: ChangePortBlocking) -> None:
+    def __init__(self, server_id: int, json_body: Reboot) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangePortBlocking/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Reboot/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(ChangePortBlocking)
+        json_body = mapping.add_json_body(Reboot)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                ChangePortBlockingType,
+                RebootType,
                 required=True,
                 option_name="type",
             )
         )
 
-        json_body.add(
-            PrimitiveAttribute(
-                "enabled",
-                bool,
-                required=True,
-                option_name="enabled",
-                description="""The desired enabled status for port blocking.""",
-            )
-        )
-
         return mapping
 
     @property
     def ok_response_type(self) -> type:
         return ActionResponse
 
     def request(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_reverse_name.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_reverse_name.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeReverseName
@@ -31,21 +32,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeReverseName/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeReverseName)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_separate_private_network_interface.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_separate_private_network_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from binarylane.models.change_separate_private_network_interface_type import ChangeSeparatePrivateNetworkInterfaceType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeSeparatePrivateNetworkInterface
@@ -32,21 +33,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeSeparatePrivateNetworkInterface/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeSeparatePrivateNetworkInterface)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_source_and_destination_check.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_source_and_destination_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from binarylane.models.change_source_and_destination_check_type import ChangeSourceAndDestinationCheckType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeSourceAndDestinationCheck
@@ -32,21 +33,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeSourceAndDestinationCheck/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeSourceAndDestinationCheck)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_threshold_alerts.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_threshold_alerts.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from binarylane.models.threshold_alert_type import ThresholdAlertType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import ListAttribute, Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeThresholdAlerts
@@ -33,21 +34,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeThresholdAlerts/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeThresholdAlerts)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_vpc_ipv_4.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_vpc_ipv_4.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from binarylane.models.change_vpc_ipv_4_type import ChangeVpcIpv4Type
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: ChangeVpcIpv4
@@ -30,21 +31,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeVpcIpv4/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(ChangeVpcIpv4)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_clone_using_backup.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_clone_using_backup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: CloneUsingBackup
@@ -31,21 +32,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#CloneUsingBackup/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(CloneUsingBackup)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_delete_disk.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_disable_selinux.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_delete_disk import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_disable_selinux import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.delete_disk import DeleteDisk
-from binarylane.models.delete_disk_type import DeleteDiskType
+from binarylane.models.disable_selinux import DisableSelinux
+from binarylane.models.disable_selinux_type import DisableSelinuxType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: DeleteDisk
+    json_body: DisableSelinux
 
-    def __init__(self, server_id: int, json_body: DeleteDisk) -> None:
+    def __init__(self, server_id: int, json_body: DisableSelinux) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#DeleteDisk/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#DisableSelinux/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(DeleteDisk)
+        json_body = mapping.add_json_body(DisableSelinux)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                DeleteDiskType,
+                DisableSelinuxType,
                 required=True,
                 option_name="type",
             )
         )
 
-        json_body.add(
-            PrimitiveAttribute(
-                "disk_id",
-                int,
-                required=True,
-                option_name="disk-id",
-                description="""The ID of the existing disk. See server.disks for a list of IDs.""",
-            )
-        )
-
         return mapping
 
     @property
     def ok_response_type(self) -> type:
         return ActionResponse
 
     def request(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_detach_backup.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_detach_backup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from binarylane.models.detach_backup_type import DetachBackupType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: DetachBackup
@@ -30,21 +31,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#DetachBackup/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(DetachBackup)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_disable_backups.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_on.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_disable_backups import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_power_on import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.disable_backups import DisableBackups
-from binarylane.models.disable_backups_type import DisableBackupsType
+from binarylane.models.power_on import PowerOn
+from binarylane.models.power_on_type import PowerOnType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: DisableBackups
+    json_body: PowerOn
 
-    def __init__(self, server_id: int, json_body: DisableBackups) -> None:
+    def __init__(self, server_id: int, json_body: PowerOn) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#DisableBackups/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#PowerOn/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(DisableBackups)
+        json_body = mapping.add_json_body(PowerOn)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                DisableBackupsType,
+                PowerOnType,
                 required=True,
                 option_name="type",
             )
         )
 
         return mapping
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_disable_selinux.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_restore.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,80 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_disable_selinux import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_restore import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.disable_selinux import DisableSelinux
-from binarylane.models.disable_selinux_type import DisableSelinuxType
 from binarylane.models.problem_details import ProblemDetails
+from binarylane.models.restore import Restore
+from binarylane.models.restore_type import RestoreType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: DisableSelinux
+    json_body: Restore
 
-    def __init__(self, server_id: int, json_body: DisableSelinux) -> None:
+    def __init__(self, server_id: int, json_body: Restore) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#DisableSelinux/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Restore/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(DisableSelinux)
+        json_body = mapping.add_json_body(Restore)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                DisableSelinuxType,
+                RestoreType,
                 required=True,
                 option_name="type",
             )
         )
 
+        json_body.add(
+            PrimitiveAttribute(
+                "image",
+                Union[int, str],
+                required=True,
+                option_name="image",
+                description="""The ID of the specific backup to use. Snapshots are not currently supported.""",
+            )
+        )
+
         return mapping
 
     @property
     def ok_response_type(self) -> type:
         return ActionResponse
 
     def request(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_enable_backups.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_kernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,80 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_enable_backups import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_change_kernel import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.enable_backups import EnableBackups
-from binarylane.models.enable_backups_type import EnableBackupsType
+from binarylane.models.change_kernel import ChangeKernel
+from binarylane.models.change_kernel_type import ChangeKernelType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: EnableBackups
+    json_body: ChangeKernel
 
-    def __init__(self, server_id: int, json_body: EnableBackups) -> None:
+    def __init__(self, server_id: int, json_body: ChangeKernel) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#EnableBackups/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangeKernel/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(EnableBackups)
+        json_body = mapping.add_json_body(ChangeKernel)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                EnableBackupsType,
+                ChangeKernelType,
                 required=True,
                 option_name="type",
             )
         )
 
+        json_body.add(
+            PrimitiveAttribute(
+                "kernel",
+                int,
+                required=True,
+                option_name="kernel",
+                description="""The ID of the kernel to use.""",
+            )
+        )
+
         return mapping
 
     @property
     def ok_response_type(self) -> type:
         return ActionResponse
 
     def request(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_enable_ipv_6.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_enable_ipv_6.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from binarylane.models.enable_ipv_6_type import EnableIpv6Type
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: EnableIpv6
@@ -30,21 +31,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#EnableIpv6/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(EnableIpv6)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_is_running.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_off.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_is_running import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_power_off import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.is_running import IsRunning
-from binarylane.models.is_running_type import IsRunningType
+from binarylane.models.power_off import PowerOff
+from binarylane.models.power_off_type import PowerOffType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: IsRunning
+    json_body: PowerOff
 
-    def __init__(self, server_id: int, json_body: IsRunning) -> None:
+    def __init__(self, server_id: int, json_body: PowerOff) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#IsRunning/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#PowerOff/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(IsRunning)
+        json_body = mapping.add_json_body(PowerOff)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                IsRunningType,
+                PowerOffType,
                 required=True,
                 option_name="type",
             )
         )
 
         return mapping
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_password_reset.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_password_reset.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: PasswordReset
@@ -31,21 +32,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#PasswordReset/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(PasswordReset)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_ping.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_uncancel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_ping import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_uncancel import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.ping import Ping
-from binarylane.models.ping_type import PingType
 from binarylane.models.problem_details import ProblemDetails
+from binarylane.models.uncancel import Uncancel
+from binarylane.models.uncancel_type import UncancelType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: Ping
+    json_body: Uncancel
 
-    def __init__(self, server_id: int, json_body: Ping) -> None:
+    def __init__(self, server_id: int, json_body: Uncancel) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Ping/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Uncancel/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(Ping)
+        json_body = mapping.add_json_body(Uncancel)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                PingType,
+                UncancelType,
                 required=True,
                 option_name="type",
             )
         )
 
         return mapping
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_cycle.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_cycle.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from binarylane.models.power_cycle_type import PowerCycleType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: PowerCycle
@@ -30,21 +31,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#PowerCycle/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(PowerCycle)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_off.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_shutdown.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_power_off import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_shutdown import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.power_off import PowerOff
-from binarylane.models.power_off_type import PowerOffType
 from binarylane.models.problem_details import ProblemDetails
+from binarylane.models.shutdown import Shutdown
+from binarylane.models.shutdown_type import ShutdownType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: PowerOff
+    json_body: Shutdown
 
-    def __init__(self, server_id: int, json_body: PowerOff) -> None:
+    def __init__(self, server_id: int, json_body: Shutdown) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#PowerOff/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Shutdown/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(PowerOff)
+        json_body = mapping.add_json_body(Shutdown)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                PowerOffType,
+                ShutdownType,
                 required=True,
                 option_name="type",
             )
         )
 
         return mapping
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_power_on.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_delete_disk.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,80 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_power_on import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_delete_disk import sync_detailed
 from binarylane.models.action_response import ActionResponse
-from binarylane.models.power_on import PowerOn
-from binarylane.models.power_on_type import PowerOnType
+from binarylane.models.delete_disk import DeleteDisk
+from binarylane.models.delete_disk_type import DeleteDiskType
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: PowerOn
+    json_body: DeleteDisk
 
-    def __init__(self, server_id: int, json_body: PowerOn) -> None:
+    def __init__(self, server_id: int, json_body: DeleteDisk) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#PowerOn/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#DeleteDisk/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(PowerOn)
+        json_body = mapping.add_json_body(DeleteDisk)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                PowerOnType,
+                DeleteDiskType,
                 required=True,
                 option_name="type",
             )
         )
 
+        json_body.add(
+            PrimitiveAttribute(
+                "disk_id",
+                int,
+                required=True,
+                option_name="disk-id",
+                description="""The ID of the existing disk. See server.disks for a list of IDs.""",
+            )
+        )
+
         return mapping
 
     @property
     def ok_response_type(self) -> type:
         return ActionResponse
 
     def request(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_reboot.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_enable_backups.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_reboot import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_enable_backups import sync_detailed
 from binarylane.models.action_response import ActionResponse
+from binarylane.models.enable_backups import EnableBackups
+from binarylane.models.enable_backups_type import EnableBackupsType
 from binarylane.models.problem_details import ProblemDetails
-from binarylane.models.reboot import Reboot
-from binarylane.models.reboot_type import RebootType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: Reboot
+    json_body: EnableBackups
 
-    def __init__(self, server_id: int, json_body: Reboot) -> None:
+    def __init__(self, server_id: int, json_body: EnableBackups) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Reboot/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#EnableBackups/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(Reboot)
+        json_body = mapping.add_json_body(EnableBackups)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                RebootType,
+                EnableBackupsType,
                 required=True,
                 option_name="type",
             )
         )
 
         return mapping
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_rebuild.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_rebuild.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from binarylane.models.rebuild_type import RebuildType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, ObjectAttribute, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: Rebuild
@@ -32,21 +33,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Rebuild/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(Rebuild)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_rename.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_rename.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from binarylane.models.rename import Rename
 from binarylane.models.rename_type import RenameType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: Rename
@@ -30,21 +31,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Rename/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(Rename)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_resize.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_resize.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from binarylane.models.take_backup_type import TakeBackupType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import ListAttribute, Mapping, ObjectAttribute, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: Resize
@@ -40,21 +41,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Resize/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(Resize)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_resize_disk.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_add_disk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,88 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_resize_disk import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_add_disk import sync_detailed
 from binarylane.models.action_response import ActionResponse
+from binarylane.models.add_disk import AddDisk
+from binarylane.models.add_disk_type import AddDiskType
 from binarylane.models.problem_details import ProblemDetails
-from binarylane.models.resize_disk import ResizeDisk
-from binarylane.models.resize_disk_type import ResizeDiskType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
+from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: ResizeDisk
+    json_body: AddDisk
 
-    def __init__(self, server_id: int, json_body: ResizeDisk) -> None:
+    def __init__(self, server_id: int, json_body: AddDisk) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ResizeDisk/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#AddDisk/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(ResizeDisk)
+        json_body = mapping.add_json_body(AddDisk)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                ResizeDiskType,
+                AddDiskType,
                 required=True,
                 option_name="type",
             )
         )
 
         json_body.add(
             PrimitiveAttribute(
-                "disk_id",
+                "size_gigabytes",
                 int,
                 required=True,
-                option_name="disk-id",
-                description="""The ID of the existing disk. See server.disks for a list of IDs.""",
+                option_name="size-gigabytes",
+                description="""The size of the new disk in GB. The server must have at least this much unallocated storage space.""",
             )
         )
 
         json_body.add(
             PrimitiveAttribute(
-                "size_gigabytes",
-                int,
-                required=True,
-                option_name="size-gigabytes",
-                description="""The new size of the disk in GB. If increasing the size of the disk the server must have sufficient unallocated storage space.""",
+                "description",
+                Union[Unset, None, str],
+                required=False,
+                option_name="description",
+                description="""An optional description for the disk. If this is null a default description will be added. Submit an empty string to prevent the default description being added.""",
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_restore.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_change_port_blocking.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_restore import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_change_port_blocking import sync_detailed
 from binarylane.models.action_response import ActionResponse
+from binarylane.models.change_port_blocking import ChangePortBlocking
+from binarylane.models.change_port_blocking_type import ChangePortBlockingType
 from binarylane.models.problem_details import ProblemDetails
-from binarylane.models.restore import Restore
-from binarylane.models.restore_type import RestoreType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: Restore
+    json_body: ChangePortBlocking
 
-    def __init__(self, server_id: int, json_body: Restore) -> None:
+    def __init__(self, server_id: int, json_body: ChangePortBlocking) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Restore/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#ChangePortBlocking/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(Restore)
+        json_body = mapping.add_json_body(ChangePortBlocking)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                RestoreType,
+                ChangePortBlockingType,
                 required=True,
                 option_name="type",
             )
         )
 
         json_body.add(
             PrimitiveAttribute(
-                "image",
-                Union[int, str],
+                "enabled",
+                bool,
                 required=True,
-                option_name="image",
-                description="""The ID of the specific backup to use. Snapshots are not currently supported.""",
+                option_name="enabled",
+                description="""The desired enabled status for port blocking.""",
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_shutdown.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_disable_backups.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_shutdown import sync_detailed
+from binarylane.api.server_actions.post_v_2_servers_server_id_actions_disable_backups import sync_detailed
 from binarylane.models.action_response import ActionResponse
+from binarylane.models.disable_backups import DisableBackups
+from binarylane.models.disable_backups_type import DisableBackupsType
 from binarylane.models.problem_details import ProblemDetails
-from binarylane.models.shutdown import Shutdown
-from binarylane.models.shutdown_type import ShutdownType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: Shutdown
+    json_body: DisableBackups
 
-    def __init__(self, server_id: int, json_body: Shutdown) -> None:
+    def __init__(self, server_id: int, json_body: DisableBackups) -> None:
         self.server_id = server_id
         self.json_body = json_body
 
 
 class Command(ActionRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Shutdown/post"
+        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#DisableBackups/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
-        json_body = mapping.add_json_body(Shutdown)
+        json_body = mapping.add_json_body(DisableBackups)
 
         json_body.add(
             PrimitiveAttribute(
                 "type",
-                ShutdownType,
+                DisableBackupsType,
                 required=True,
                 option_name="type",
             )
         )
 
         return mapping
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_take_backup.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_take_backup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from binarylane.models.take_backup_type import TakeBackupType
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 from binarylane.types import Unset
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
 from binarylane.console.runners.action import ActionRunner
 
 
 class CommandRequest:
     server_id: int
     json_body: TakeBackup
@@ -33,21 +34,26 @@
     @property
     def reference_url(self) -> str:
         return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#TakeBackup/post"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
+                metavar="server",
+                description="""The ID or name of the server on which the action should be performed.""",
+                lookup=lookup_server_id,
             )
         )
 
         json_body = mapping.add_json_body(TakeBackup)
 
         json_body.add(
             PrimitiveAttribute(
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/post_v_2_servers_server_id_actions_uptime.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/get_v2_failover_ips_server_id.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,92 @@
 from __future__ import annotations
 
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Tuple, Union
+from typing import TYPE_CHECKING, Optional, Tuple, Union
 
-from binarylane.api.server_actions.post_v_2_servers_server_id_actions_uptime import sync_detailed
-from binarylane.models.action_response import ActionResponse
+from binarylane.api.failover_ips.get_v2_failover_ips_server_id import sync_detailed
+from binarylane.models.failover_ips_response import FailoverIpsResponse
+from binarylane.models.links import Links
 from binarylane.models.problem_details import ProblemDetails
-from binarylane.models.uptime import Uptime
-from binarylane.models.uptime_type import UptimeType
-from binarylane.models.validation_problem_details import ValidationProblemDetails
 
 if TYPE_CHECKING:
     from binarylane.client import Client
 
+import binarylane.console.commands.api.get_v2_servers as api_get_v2_servers
 from binarylane.console.parser import Mapping, PrimitiveAttribute
-from binarylane.console.runners.action import ActionRunner
+from binarylane.console.runners.command import CommandRunner
 
 
 class CommandRequest:
     server_id: int
-    json_body: Uptime
 
-    def __init__(self, server_id: int, json_body: Uptime) -> None:
+    def __init__(self, server_id: int) -> None:
         self.server_id = server_id
-        self.json_body = json_body
 
 
-class Command(ActionRunner):
+class Command(CommandRunner):
     @property
     def reference_url(self) -> str:
-        return "https://api.binarylane.com.au/reference/#tag/ServerActions/paths/~1v2~1servers~1%7Bserver_id%7D~1actions#Uptime/post"
+        return "https://api.binarylane.com.au/reference/#tag/FailoverIps/paths/~1v2~1failover_ips~1%7Bserver_id%7D/get"
 
     def create_mapping(self) -> Mapping:
         mapping = Mapping(CommandRequest)
 
+        def lookup_server_id(ref: str) -> Union[None, int]:
+            return api_get_v2_servers.Command(self._context).lookup(ref)
+
         mapping.add(
             PrimitiveAttribute(
                 "server_id",
                 int,
                 required=True,
                 option_name=None,
-                description="""The ID of the server on which the action should be performed.""",
-            )
-        )
-
-        json_body = mapping.add_json_body(Uptime)
-
-        json_body.add(
-            PrimitiveAttribute(
-                "type",
-                UptimeType,
-                required=True,
-                option_name="type",
+                metavar="server",
+                description="""The target server id or name.""",
+                lookup=lookup_server_id,
             )
         )
 
         return mapping
 
     @property
     def ok_response_type(self) -> type:
-        return ActionResponse
+        return FailoverIpsResponse
 
     def request(
         self,
         client: Client,
         request: object,
-    ) -> Tuple[HTTPStatus, Union[ActionResponse, None, ProblemDetails, ValidationProblemDetails]]:
+    ) -> Tuple[HTTPStatus, Union[None, FailoverIpsResponse, ProblemDetails]]:
         assert isinstance(request, CommandRequest)
 
-        # HTTPStatus.OK: ActionResponse
-        # HTTPStatus.ACCEPTED: Any
-        # HTTPStatus.BAD_REQUEST: ValidationProblemDetails
+        # HTTPStatus.OK: FailoverIpsResponse
         # HTTPStatus.NOT_FOUND: ProblemDetails
-        # HTTPStatus.UNPROCESSABLE_ENTITY: ProblemDetails
         # HTTPStatus.UNAUTHORIZED: Any
-        page_response = sync_detailed(
-            server_id=request.server_id,
-            client=client,
-            json_body=request.json_body,
-        )
-        return page_response.status_code, page_response.parsed
+        page = 0
+        per_page = 25
+        has_next = True
+        response: Optional[FailoverIpsResponse] = None
+
+        while has_next:
+            page += 1
+            page_response = sync_detailed(
+                server_id=request.server_id,
+                client=client,
+                page=page,
+                per_page=per_page,
+            )
+
+            status_code = page_response.status_code
+            if status_code != 200:
+                return status_code, page_response.parsed
+
+            assert isinstance(page_response.parsed, FailoverIpsResponse)
+            has_next = isinstance(page_response.parsed.links, Links) and isinstance(
+                page_response.parsed.links.pages.next_, str
+            )
+            if not response:
+                response = page_response.parsed
+            else:
+                response.failover_ips += page_response.parsed.failover_ips
+
+        return status_code, response
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/put_v2_account_keys_key_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/put_v2_account_keys_key_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/put_v2_domains_domain_name_records_record_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/put_v2_domains_domain_name_records_record_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/put_v2_images_image_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/put_v2_images_image_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/put_v2_load_balancers_load_balancer_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/put_v2_load_balancers_load_balancer_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/api/put_v2_vpcs_vpc_id.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/api/put_v2_vpcs_vpc_id.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/commands/configure.py` & `binarylane_cli-0.16.0/src/binarylane/console/commands/configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import logging
-from typing import List
-
-from binarylane.config import UserConfig
+from typing import TYPE_CHECKING, List
 
 from binarylane.console.runners import ExitCode, Runner
 from binarylane.console.util import create_client
 
+if TYPE_CHECKING:
+    from binarylane.config import UserConfig
+
 logger = logging.getLogger(__name__)
 
 
 class Command(Runner):
     """Interactive runner to request, verify, and store API token to configuration file"""
 
     def run(self, args: List[str]) -> None:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/parser/__init__.py` & `binarylane_cli-0.16.0/src/binarylane/console/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/parser/attribute.py` & `binarylane_cli-0.16.0/src/binarylane/console/parser/attribute.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/parser/help_formatter.py` & `binarylane_cli-0.16.0/src/binarylane/console/parser/help_formatter.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/parser/list_attribute.py` & `binarylane_cli-0.16.0/src/binarylane/console/parser/list_attribute.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/parser/object_attribute.py` & `binarylane_cli-0.16.0/src/binarylane/console/parser/object_attribute.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/parser/parser.py` & `binarylane_cli-0.16.0/src/binarylane/console/parser/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from __future__ import annotations
 
 import argparse
 import logging
 import shutil
-from argparse import HelpFormatter
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Sequence, Union
 
 from binarylane.console.parser.help_formatter import CommandHelpFormatter
-from binarylane.console.parser.object_attribute import Mapping
 
 if TYPE_CHECKING:
+    from argparse import HelpFormatter
+
     from typing_extensions import TypeAlias
 
+    from binarylane.console.parser.object_attribute import Mapping
+
     ArgumentGroup: TypeAlias = argparse._ArgumentGroup  # pylint: disable=protected-access
 
 logger = logging.getLogger(__name__)
 
 
 class Namespace(argparse.Namespace):
     mapped_object: Any
 
 
 # FIXME: Wrap ArgumentParser instead of subclassing it
 class Parser(argparse.ArgumentParser):
-
     _argument_names: List[str]
     _mapping: Optional[Mapping] = None
     _parsed: Optional[argparse.Namespace] = None
     _configured: bool = False
     _keywords: List[str]
     _groups: Dict[str, ArgumentGroup]
     _dest_counter: int = 0
 
+    # Optional callback on completion of argument parsing, but prior to constructing mapped_object
+    on_parse_args: Callable[[Namespace], None] = staticmethod(lambda _: None)  # type: ignore
+
     def __init__(self, prog: str, description: Optional[str] = None, epilog: Optional[str] = None) -> None:
         super().__init__(prog=prog, description=description, epilog=epilog, add_help=False, allow_abbrev=False)
 
         self._groups = {
             "required=True": self.add_argument_group(title="Arguments"),
             "required=False": self.add_argument_group(title="Parameters"),
         }
@@ -100,16 +104,21 @@
         return f"{self.prog} [OPTIONS] {' '.join(mapping_usage)}"
 
     def parse(self, args: Sequence[str]) -> Namespace:
         self.configure()
         self.usage = self._format_usage()
 
         self._parsed = self.parse_args(args, Namespace())
+        self.on_parse_args(self._parsed)
+
         if self._mapping:
-            self._parsed.mapped_object = self._mapping.construct(self, self._parsed)
+            try:
+                self._parsed.mapped_object = self._mapping.construct(self, self._parsed)
+            except argparse.ArgumentError as exc:
+                self.error(exc.message)
 
         return self._parsed
 
     def set_mapping(self, mapping: Mapping) -> Mapping:
         self._mapping = mapping
         return mapping
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/parser/primitive_attribute.py` & `binarylane_cli-0.16.0/src/binarylane/console/parser/primitive_attribute.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,45 +10,54 @@
 from binarylane.types import UNSET, Unset
 
 from binarylane.console.parser.attribute import Attribute
 
 NoneType = type(None)
 
 if TYPE_CHECKING:
-    from binarylane.console.parser.object_attribute import ObjectAttribute
     from binarylane.console.parser.parser import Parser
 
 logger = logging.getLogger(__name__)
 
 PRIMITIVE_TYPES = {int, str, bool, float, datetime, Enum}
 
 
 def is_primitive_type(type_: type) -> bool:
     return any(issubclass(type_, t) for t in PRIMITIVE_TYPES)
 
 
+class Lookup(typing.Protocol):
+    """Lookup is a function that accepts an entity reference (e.g. its name) and returns that entity's ID"""
+
+    def __call__(self, ref: str) -> Optional[int]:
+        ...
+
+
 class PrimitiveAttribute(Attribute):
     """Represents a strongly typed, command parameter"""
 
     _alternate_types: List[type]
     _dest: str
     _action: Optional[Type[argparse.Action]]
+    _lookup: Optional[Lookup]
     _metavar: str
     _default_value: object = UNSET
     _nargs: Optional[str]
 
     def __init__(
         self,
         attribute_name: str,
         attribute_type_hint: object,
         *,
         option_name: Optional[str],
         required: bool,
         description: Optional[str] = None,
+        metavar: Optional[str] = None,
         action: Optional[Type[argparse.Action]] = None,
+        lookup: Optional[Lookup] = None,
     ) -> None:
         # Partial construction needed to perform unboxing:
         self._nargs = None
         self._alternate_types = []
         self.required = required
         attribute_type = self._unbox_type(attribute_type_hint)
 
@@ -59,15 +68,16 @@
             required=required,
             option_name=option_name,
             description=description,
         )
 
         self._dest = attribute_name
         self._action = action
-        self._metavar = (option_name or attribute_name).replace("-", "_").upper()
+        self._lookup = lookup
+        self._metavar = (metavar or option_name or attribute_name).replace("-", "_").upper()
 
     @property
     def usage(self) -> Optional[str]:
         if self.has_default_value:
             return None
 
         if not self.option_name:
@@ -112,15 +122,20 @@
             self._unsupported("missing metavar")
             kwargs["metavar"] = self.option_name.upper()
 
         # This argument is going to be displayed, warn if a description is not available
         if self.description is None:
             self._unsupported("missing help", False)
 
-        parser.add_to_group(self.group_name or bool(self.required), self.name_or_flag, self.attribute_type, **kwargs)
+        # parser input type is changed to string if lookup is permitted
+        attribute_type = self.attribute_type
+        if self._lookup:
+            attribute_type = str
+
+        parser.add_to_group(self.group_name or bool(self.required), self.name_or_flag, attribute_type, **kwargs)
 
     def construct(self, _parser: Parser, parsed: argparse.Namespace) -> object:
         value: object = getattr(parsed, self._dest, self._default_value)
         if value in (None, UNSET):
             if not self.required:
                 return UNSET
             raise ValueError(f"{self.option_name} is a required value")
@@ -136,19 +151,38 @@
                     result += [self._construct(nested) for nested in item]
                 else:
                     result.append(self._construct(item))
             return result
 
         return self._construct(value)
 
+    def lookup(self, value: str) -> object:
+        assert self._lookup is not None
+        try:
+            # See if provided value is already of correct type
+            return self.attribute_type(value)
+        except ValueError:
+            # If not, perform a lookup using the provided value
+            result = self._lookup(value)
+            if result is None:
+                # pylint: disable=raise-missing-from
+                raise argparse.ArgumentError(None, f"{self.attribute_name.upper()}: could not find '{value}'")
+            return result
+
     def _construct(self, value: object) -> object:
         if self.attribute_type is None:
             logger.warning("%s does not have a primitive type, assuming str", self.option_name)
             return value
 
+        # Perform lookup or convert to native type when required
+        if self._lookup:
+            # if we have a lookup, the parser was given attribute_type = str but type analyzer does not know that
+            assert isinstance(value, str)
+            value = self.lookup(value)
+
         # Ensure value is of correct type
         if not isinstance(value, self.attribute_type):
             raise TypeError(f"{self.option_name} has {type(value)} instead of {self.attribute_type}")
 
         # If we have alternative types, see if any are valid:
         for type_ in self._alternate_types:
             try:
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/printers/__init__.py` & `binarylane_cli-0.16.0/src/binarylane/console/printers/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 
 from binarylane.console.printers.json_printer import JsonPrinter
 from binarylane.console.printers.plain_printer import PlainPrinter
 from binarylane.console.printers.printer import Printer
 from binarylane.console.printers.table_printer import TablePrinter
 from binarylane.console.printers.tsv_printer import TsvPrinter
 
+__all__ = [
+    "Printer",
+    "create_printer",
+]
+
 
 class PrinterType(Enum):
     """Enum of available printer implementations"""
 
     PLAIN = PlainPrinter
     TABLE = TablePrinter
     TSV = TsvPrinter
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/printers/formatter.py` & `binarylane_cli-0.16.0/src/binarylane/console/printers/formatter.py`

 * *Files 15% similar despite different names*

```diff
@@ -81,43 +81,37 @@
         item_type = type(item)
         if item_type is list:
             if len(item) > max_list:
                 item = item[:max_list] + [trunc]
             if not single_object:
                 item = ", ".join(map(str, item))
             else:
-                item = (
-                    "- "
-                    + "\n- ".join(
-                        [
-                            (
-                                "  ".join(f"{key}: {value}\n" for key, value in i.items())
-                                if isinstance(i, dict)
-                                else str(i)
-                            )
-                            for i in item
-                        ]
-                    )
-                    if item
-                    else ""
-                )
+                item = _flatten_list(item) if item else ""
         if item_type is dict:
             item = _flatten_dict(item, single_object)
 
         if item_type is bool:
             item = "Yes" if item else "No"
 
         item = str(item) if item is not None else NULL_STR
         if len(item) > max_str + len(trunc):
             item = item[:max_str] + trunc
         result.append(item)
 
     return result
 
 
+def _flatten_list(item: List[Any]) -> str:
+    result = "- "
+    result += "\n- ".join(
+        [("  ".join(f"{key}: {value}\n" for key, value in i.items()) if isinstance(i, dict) else str(i)) for i in item]
+    )
+    return result
+
+
 def _flatten_dict(item: Dict[str, Any], single_object: bool) -> str:
     # FIXME: openapi spec should provide these directions
 
     # - use display_name for host
     # - use full_name for image (preferred over name)
     # - of the remainder generic columns we prefer name > slug > id
     for key in ("display_name", "full_name", "name", "slug", "id"):
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/printers/printer.py` & `binarylane_cli-0.16.0/src/binarylane/console/printers/printer.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/printers/table_printer.py` & `binarylane_cli-0.16.0/src/binarylane/console/printers/table_printer.py`

 * *Files identical despite different names*

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/runners/__init__.py` & `binarylane_cli-0.16.0/src/binarylane/console/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import importlib
 import sys
 from abc import ABC, abstractmethod
 from argparse import SUPPRESS
 from dataclasses import dataclass
 from enum import Enum
-from typing import ClassVar, List, NoReturn, Optional, Sequence, Type
+from typing import ClassVar, List, NoReturn, Sequence, Type
 from binarylane.pycompat.actions import BooleanOptionalAction
 
 from binarylane.config import DefaultConfig, UserConfig
 
 from binarylane.console.metadata import program_name
 from binarylane.console.parser import Namespace, Parser
 
@@ -72,20 +72,21 @@
         self._parser = Parser(context.prog, context.description)
         self._parser.add_argument("--help", help=self.HELP_DESCRIPTION, action="help")
 
         self._context = context
         self._context.configure(self._parser)
         self.configure(self._parser)
 
+        self._parser.on_parse_args = self._context.add_commandline
+
     def configure(self, parser: Parser) -> None:
         """Subclasses add arguments to parser here"""
 
     def parse(self, args: Sequence[str]) -> Namespace:
         parsed = self._parser.parse(args)
-        self._context.add_commandline(parsed)
         return parsed
 
     @abstractmethod
     def run(self, args: List[str]) -> None:
         """Subclasses implement their primary behaviour here"""
 
     @staticmethod
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/runners/action.py` & `binarylane_cli-0.16.0/src/binarylane/console/runners/action.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 
 import logging
 import shutil
 import sys
 import time
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any
 
-from binarylane.console.parser import Namespace, Parser
 from binarylane.console.runners.command import CommandRunner
 
 if TYPE_CHECKING:
-    from binarylane.api.actions.get_v2_actions_action_id import sync_detailed
-    from binarylane.models.action_response import ActionResponse
+    from binarylane.console.parser import Namespace, Parser
+
 
 logger = logging.getLogger(__name__)
 
 
 class ActionRunner(CommandRunner):
     """ActionRunner handles API commands that return ActionResponse, showing progress until the Action completes"""
 
-    _async: Optional[bool]
-    _quiet: Optional[bool]
+    _async: bool = False
+    _quiet: bool = False
 
     def configure(self, parser: Parser) -> None:
         super().configure(parser)
 
         parser.add_argument(
             "--async", action="store_true", dest="runner_async", help="Do not wait for requested action to complete"
         )
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/runners/command.py` & `binarylane_cli-0.16.0/src/binarylane/console/runners/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from __future__ import annotations
 
 import logging
 from abc import abstractmethod
-from http import HTTPStatus
-from typing import Any, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, List, Optional, Tuple
 
-from binarylane.client import AuthenticatedClient, Client
 from binarylane.models.problem_details import ProblemDetails
 from binarylane.models.validation_problem_details import ValidationProblemDetails
 
-from binarylane.console.parser import Mapping, Namespace, Parser
 from binarylane.console.printers import Printer, PrinterType, create_printer
 from binarylane.console.runners import ExitCode, Runner
 from binarylane.console.runners.httpx_wrapper import CurlCommand
 from binarylane.console.util import create_client
 
+if TYPE_CHECKING:
+    from http import HTTPStatus
+
+    from binarylane.client import AuthenticatedClient, Client
+
+    from binarylane.console.parser import Mapping, Namespace, Parser
+
 logger = logging.getLogger(__name__)
 
 _DEFAULT_OUTPUT = "table"
 _DEFAULT_HEADER = True
 
 
 class CommandRunner(Runner):
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/runners/httpx_wrapper.py` & `binarylane_cli-0.16.0/src/binarylane/console/runners/httpx_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import json
 import urllib.parse
 from abc import ABC, abstractmethod
-from types import TracebackType
 from typing import TYPE_CHECKING, Any, Callable, Optional, TypeVar
 from binarylane.pycompat import shlex
 
 if TYPE_CHECKING:
-    import httpx
+    from types import TracebackType
+
+    import httpx  # noqa: TC004 - lazy import in HttpxWrapper.__init__()
 
 
 WrapperT = TypeVar("WrapperT", bound="HttpxWrapper")
 
 
 class HttpxWrapper(ABC):
     """Hook httpx.request to enable displaying additional information from API calls"""
@@ -22,15 +23,14 @@
         import httpx
 
         globals()["httpx"] = httpx
 
     _httpx_request: Optional[Callable[..., httpx.Response]]
 
     def __enter__(self: WrapperT) -> WrapperT:
-
         self._httpx_request = httpx.request
         httpx.request = self.request
         return self
 
     @abstractmethod
     def request(self, *args: Any, **kwargs: Any) -> httpx.Response:
         """Perform HTTP request - child classes can override to modify and/or replace request"""
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/runners/list.py` & `binarylane_cli-0.16.0/src/binarylane/console/runners/list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import fnmatch
 import re
 from abc import abstractmethod
-from typing import Dict, List
+from typing import TYPE_CHECKING, Dict, List
 
-from binarylane.console.parser import Namespace, Parser
 from binarylane.console.runners.command import CommandRunner
 
+if TYPE_CHECKING:
+    from binarylane.console.parser import Namespace, Parser
+
 
 class ListRunner(CommandRunner):
     """ListRunner displays a received list with user-customisable field list"""
 
     _format: List[str]
     output: str
     header: bool
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/console/util.py` & `binarylane_cli-0.16.0/src/binarylane/console/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 from platform import machine, python_implementation, python_version, system
+from typing import TYPE_CHECKING
 
 from binarylane.client import AuthenticatedClient
-from binarylane.config import UserConfig
 
 from binarylane.console.metadata import distribution_name, distribution_version
 
+if TYPE_CHECKING:
+    from binarylane.config import UserConfig
+
 
 def create_client(config: UserConfig) -> AuthenticatedClient:
     return AuthenticatedClient(
         base_url=config.api_url,
         token=config.api_token,
         verify_ssl=not config.api_development,
         timeout=5.0,
```

### Comparing `binarylane_cli-0.15.3/src/binarylane/pycompat/actions.py` & `binarylane_cli-0.16.0/src/binarylane/pycompat/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         default: Union[object, str, None] = None,
         type: Union[Callable[[str], object], argparse.FileType, None] = None,  # pylint: disable=redefined-builtin
         choices: Union[Iterable[object], None] = None,
         required: bool = False,
         help: Union[str, None] = None,  # pylint: disable=redefined-builtin
         metavar: Union[str, Tuple[str, ...], None] = None,
     ) -> None:
-
         _option_strings = []
         for option_string in option_strings:
             _option_strings.append(option_string)
 
             if option_string.startswith("--"):
                 option_string = "--no-" + option_string[2:]
                 _option_strings.append(option_string)
```

### Comparing `binarylane_cli-0.15.3/setup.py` & `binarylane_cli-0.16.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,94 +1,425 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: binarylane-cli
+Version: 0.16.0
+Summary: 
+Author: Nathan O'Sullivan
+Author-email: nathan.osullivan@mammoth.com.au
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: backports.cached-property (>=1.0.2,<2.0.0) ; python_version < "3.8"
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: importlib-metadata ; python_version < "3.8"
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: terminaltables (>=3.1.10,<4.0.0)
+Requires-Dist: typing-extensions (>=4.0.0,<5.0.0) ; python_version < "3.8"
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src',
- 'binarylane': 'lib/binarylane',
- 'binarylane.api': 'lib/binarylane/api',
- 'binarylane.api.accounts': 'lib/binarylane/api/accounts',
- 'binarylane.api.actions': 'lib/binarylane/api/actions',
- 'binarylane.api.customers': 'lib/binarylane/api/customers',
- 'binarylane.api.data_usages': 'lib/binarylane/api/data_usages',
- 'binarylane.api.domains': 'lib/binarylane/api/domains',
- 'binarylane.api.failover_ips': 'lib/binarylane/api/failover_ips',
- 'binarylane.api.images': 'lib/binarylane/api/images',
- 'binarylane.api.keys': 'lib/binarylane/api/keys',
- 'binarylane.api.load_balancers': 'lib/binarylane/api/load_balancers',
- 'binarylane.api.regions': 'lib/binarylane/api/regions',
- 'binarylane.api.reverse_names': 'lib/binarylane/api/reverse_names',
- 'binarylane.api.sample_sets': 'lib/binarylane/api/sample_sets',
- 'binarylane.api.server_actions': 'lib/binarylane/api/server_actions',
- 'binarylane.api.servers': 'lib/binarylane/api/servers',
- 'binarylane.api.sizes': 'lib/binarylane/api/sizes',
- 'binarylane.api.software': 'lib/binarylane/api/software',
- 'binarylane.api.vpcs': 'lib/binarylane/api/vpcs',
- 'binarylane.models': 'lib/binarylane/models'}
-
-packages = \
-['binarylane',
- 'binarylane.api',
- 'binarylane.api.accounts',
- 'binarylane.api.actions',
- 'binarylane.api.customers',
- 'binarylane.api.data_usages',
- 'binarylane.api.domains',
- 'binarylane.api.failover_ips',
- 'binarylane.api.images',
- 'binarylane.api.keys',
- 'binarylane.api.load_balancers',
- 'binarylane.api.regions',
- 'binarylane.api.reverse_names',
- 'binarylane.api.sample_sets',
- 'binarylane.api.server_actions',
- 'binarylane.api.servers',
- 'binarylane.api.sizes',
- 'binarylane.api.software',
- 'binarylane.api.vpcs',
- 'binarylane.config',
- 'binarylane.console',
- 'binarylane.console.commands',
- 'binarylane.console.commands.api',
- 'binarylane.console.parser',
- 'binarylane.console.printers',
- 'binarylane.console.runners',
- 'binarylane.models',
- 'binarylane.pycompat']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=22.2.0,<23.0.0',
- 'httpx>=0.23.0,<0.24.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'terminaltables>=3.1.10,<4.0.0']
-
-extras_require = \
-{':python_version < "3.8"': ['backports.cached-property>=1.0.2,<2.0.0',
-                             'typing-extensions>=4.0.0,<5.0.0',
-                             'importlib-metadata']}
-
-entry_points = \
-{'console_scripts': ['bl = binarylane.console.__main__:main']}
-
-setup_kwargs = {
-    'name': 'binarylane-cli',
-    'version': '0.15.3',
-    'description': '',
-    'long_description': '# `bl`: BinaryLane command-line interface\n\n```\n$ bl --help\nusage: bl [OPTIONS] COMMAND\n\nbl is a command-line interface for the BinaryLane API\n\nOptions:\n  --help                Display available commands and descriptions\n\nAvailable Commands:\n    account             Access account commands\n    action              Access action commands\n    configure           Configure access to BinaryLane API\n    domain              Access domain commands\n    image               Access image commands\n    load-balancer       Access load-balancer commands\n    region              Access region commands\n    server              Access server commands\n    size                Access size commands\n    software            Access software commands\n    ssh-key             Access ssh-key commands\n    version             Show the current version\n    vpc                 Access vpc commands\n```\n\n## Installation\n\n`bl` requires Python 3.7 or later and has been tested on a variety of Linux\ndistributions, Windows and Mac OSX. To install:\n\n```\npip install binarylane-cli\n```\n\n### Portable install (without Python)\n\nThe [releases page](https://github.com/binarylane/binarylane-cli/releases) has\na standalone `bl.exe` for use on Windows.\n\n\n## Getting Started\n\nThe BinaryLane CLI program is invoked by running `bl` (or `bl.exe` on Windows).\nTo use `bl` you must configure the program with a BinaryLane customer access\ntoken.\n\n 1. To start the configuration process, run:\n```\nbl configure\n```\n\n 2. A prompt will be shown requesting access token. Go to [Developer API](https://home.binarylane.com.au/api-info) section of BinaryLane website and select **+ Create Token**, enter a name such as *CLI* and **Create**. \n\n 3. Copy the displayed token and paste at the `bl` *Enter your API access token:*\nprompt.\n\n 4. To confirm token is working correctly, use `bl` to display BinaryLane account details:\n```\nbl account get\n``` \n\n## Usage\n\n`bl` provides commands to access all functionality provided by the [BinaryLane\nAPI](https://api.binarylane.com.au/reference/), organised into a *command\ntree*. The general form for invoking an command is `bl NOUN [NOUN] VERB`.\nFor example:\n\n - `bl server list`: Displays list of servers\n - `bl domain record create`: Create a DNS record\n\nThe available commands at each level of the tree are displayed by running `bl`\nwith no arguments:\n\n```\n$ bl\n\nusage: bl [OPTIONS] COMMAND\n\nbl is a command-line interface for the binaryLane API\n\nOptions:\n  --help                Display available commands and descriptions\n\nAvailable Commands:\n    account             Access account commands\n    action              Access action commands\n    configure           Configure access to binaryLane API\n    domain              Access domain commands\n    image               Access image commands\n    load-balancer       Access load-balancer commands\n    region              Access region commands\n    server              Access server commands\n    size                Access size commands\n    software            Access software commands\n    ssh-key             Access ssh-key commands\n    version             Show the current version\n    vpc                 Access vpc commands\n```\n\nTo see the available commands within the tree:\n\n```\nbl NOUN [NOUN]\n```\n\nFor example:\n\n```\n$ bl domain\nusage: bl domain [OPTIONS] COMMAND\n\nAccess domain commands\n\nOptions:\n  --help                Display available commands and descriptions\n\nAvailable Commands:\n    create              Create a new domain\n    delete              Delete an existing domain\n    get                 Fetch an existing domain\n    list                List all domains\n    nameservers         Access domain nameservers commands\n    record              Access domain record commands\n```\n\nTo see the required arguments and optional parameters for a command:\n\n```\nbl NOUN [NOUN] VERB --help\n```\n\nFor example:\n\n```\n$ bl domain create --help\nusage: bl domain create [OPTIONS] --name NAME [PARAMETERS]\n\nCreate a New Domain\n\nOptions:\n  --help                Display command options and descriptions\n  --curl                Display API request as a \'curl\' command-line\n  --no-header           Display columns without field labels\n  --output OUTPUT       Desired output format [plain, table, tsv, json] (Default: "table")\n\nArguments:\n  --name NAME           The domain name to add to the DNS management system.\n\nParameters:\n  --ip-address IP_ADDRESS\n                        An optional IPv4 address that will be used to create an A record for the root domain.\n```\n\n### Walkthrough: Creating a server\n\nServer creation is provided by the `bl server create` command. Use `--help` to\nview all arguments and parameters:\n\n```\n$ bl server list --help\nusage: bl server create [OPTIONS] --size SIZE --image IMAGE --region REGION [PARAMETERS]\n\nCreate a new server.\n\nOptions:\n  --help                Display command options and descriptions\n  --curl                Display API request as a \'curl\' command-line\n  --no-header           Display columns without field labels\n  --output OUTPUT       Desired output format [plain, table, tsv, json] (Default: "table")\n  --async               Do not wait for requested action to complete\n  --quiet               Do not show progress while waiting for requested action to complete\n\nArguments:\n  --size SIZE           The slug of the selected size.\n  --image IMAGE         The slug or id of the selected operating system.\n  --region REGION       The slug of the selected region.\n\nParameters:\n  --name NAME           The hostname of your server, such as vps01.yourcompany.com. If not\n                        provided, the server will be created with a random name.\n  --backups, --no-backups\n                        If true this will enable two daily backups for the server.\n                        Options.daily_backups will override this value if provided. Setting\n                        this to false has no effect.\n  --ipv6, --no-ipv6     If true this will enable IPv6 for this server.\n  --ssh-keys [SSH_KEYS [SSH_KEYS ...]]\n                        This may be either the SSH keys Ids or fingerprints. If this is null\n                        or not provided any SSH keys that have been marked as default will be\n                        deployed (if the operating system supports SSH keys). Submit an empty\n                        array to disable deployment of default keys.\n  --password PASSWORD   If this is provided the default remote user account\'s password will be\n                        set to this value. If this is null a random password will be generated\n                        and emailed to the account email address.\n  <additional parameters omitted for brevity>\n```\n\nIn the help displayed by `bl`, **Arguments** are required and **Parameters**\nare optional. For the `bl server list` command `--size SIZE`, `--image IMAGE`,\nand `--region REGION` are required. A list of available choices for each can be\ndisplayed by running:\n\n```\nbl size list\nbl image list\nbl region list\n```\n\nFor example, to create a minimum-sized Ubuntu 22.04 LTS server in Sydney using\nSSH public key authentication:\n\n```\n$ bl server create --size std-min --image ubuntu-22.04-lts --region syd\ncompleted.\n┌───────────────────────────┬─────────────────────────────────────────────────────────────────────────────────────┐\n│ name                      │ value                                                                               │\n├───────────────────────────┼─────────────────────────────────────────────────────────────────────────────────────┤\n│ id                        │ 210658                                                                              │\n│ name                      │ giant-rudolf.bnr.la                                                                 │\n│ memory                    │ 1024                                                                                │\n│ vcpus                     │ 1                                                                                   │\n│ disk                      │ 20                                                                                  │\n│ created_at                │ 2023-01-20T02:02:32+00:00                                                           │\n│ status                    │ new                                                                                 │\n│ region                    │ Sydney                                                                              │\n│ image                     │ 20.04 LTS                                                                           │\n│ size                      │ std-min                                                                             │\n│ size_slug                 │ std-min                                                                             │\n│ networks                  │ v4: [{\'ip_address\': \'175.45.180.1\',  \'type\': \'public\', \'netmask\': \'255.255.255.0... │\n  <additional rows omitted for brevity>\n└───────────────────────────┴─────────────────────────────────────────────────────────────────────────────────────┘\n```\n\n### Server passwords\n\nThe use of SSH public key authentication is strongly recommended where\npossible. When public key authentication is not suitable or the image being\ndeployed does not support SSH public key authentication (e.g. Windows Server),\ncommands such as `bl server create` and `bl server action password-reset` have\nan optional `--password PASSWORD` parameter that specifies the password to use.\n\nFor example, to create a server per the previous example with password\nauthentication:\n\n```\n$ bl server create --size std-min --image ubuntu-22.04-lts --region syd --password \'qq7s6GYZgbiVG3\'\n```\n\nUpon completion, the root password for the server in this example would be `qq7s6GYZgbiVG3`.\n\n:warning: **Internet-connected servers with password-based authentication enabled\nmust have a strong, randomly generated password.** Brute-force login attempts\nare pervasive on the public internet: if a server password is not randomly\ngenerated, unauthorised access is likely to occur.\n\n### Server actions\n\n`bl` can be used to perform any action that the BinaryLane website can perform,\nincluding:\n\n - Take and restore backups\n - Change plan, operating system, or reinstall\n - Restart and power cycle\n - and many more...\n\nA list of available commands is displayed by running `bl server action`:\n\n```\n$ bl server action\n\nAvailable Commands:\n    add-disk            Create an additional disk for a server\n    attach-backup       Attach a backup to a server\n    change-advanced-features\n                        Change the advanced features of a server\n    change-advanced-firewall-rules\n                        Change the advanced firewall rules for a server\n    change-backup-schedule\n                        Change the backup schedule of a server\n    change-ipv6         Enable or disable IPv6 for a server\n    change-ipv6-reverse-nameservers\n                        Update the IPv6 reverse name servers for a server\n    change-kernel       Change the kernel of a server\n  <additional actions omitted for brevity>\n    ping                Attempt to ping a server\n    power-cycle         Power a server off and then on\n    power-off           Power a server off\n    power-on            Power a server on\n    reboot              Request a server perform a reboot\n    rebuild             Rebuild an existing server\n    rename              Rename a server\n    resize              Update the size and related options for a server\n    resize-disk         Alter the size of an existing disk for a server\n    restore             Restore a backup to a server\n    shutdown            Request a server perform a shutdown\n    take-backup         Take a backup of a server\n    uncancel            Revert the cancellation of a server\n    uptime              Check the uptime of a server\n```\n\nEach server action has a mandatory `SERVER_ID` argument  which can be obtained\nfrom `bl server list`.\n\nMany actions have additional *action-specific* arguments and parameters. Run\n`bl server action COMMAND --help` to see what a particular action supports.\n\n#### Example: password reset\n\n 1. Use `--help` to see the available arguments and parameters:\n\n\n```\n$ bl server action password-reset --help\nusage: bl server action password-reset [OPTIONS] SERVER_ID [PARAMETERS]\n\nReset the Password of a Server\n\n<options omitted for brevity>\n\nArguments:\n  SERVER_ID            The ID of the server on which the action should be performed.\n\nParameters:\n  --username USERNAME  The username of the user to change the password.\n  --password PASSWORD  If this is provided the specified or default remote user\'s account\n                       password will be set to this value.\n```\n\n 2. Use `bl server list` to obtain the numeric server ID. In this example, the\nserver requiring a password reset is ID 123456.\n\n 3. Provide the server ID and desired password to the `password-reset` command:\n\n```\nbl server action password-reset 123456 --password \'qq7s6GYZgbiVG3\'\n```\n\n### Asynchronous actions\n\n`bl` commands that perform an action - `bl create server`, `bl server\naction restore-backup`, and many others - default to *synchronous* handling\nwhere `bl` will display progress information to the console and not exit until\nthe command finishes.\n\nIn some scenarios such as when creating multiple servers, it may be desirable\nrun the command with *asynchronous* handling where `bl` will exit as\nsoon as the BinaryLane API accepts the requested command. To do so, include the\n`--async` option in the command invocation. For example:\n\n```\n$ bl server create --size std-min --image ubuntu-22.04-lts --region syd --async\n```\n\n### Configuration file\n\n`bl configure` creates a configuration file containing the API token, and reads\nthat configuration file on subsequent invocations. The configuration file is\nstored at:\n\n * `$XDG_CONFIG_HOME/binarylane/config.ini`\n\nTypically the environment variable `$XDG_CONFIG_HOME` is not set, in which case\nthe configuration file stored at:\n\n - **Linux/Mac/etc**: `$HOME/.config` - typical file location is\n   `/home/username/.config/binarylane/config.ini`\n - **Windows**: `$APPDATA` - typical file location is\n   `C:\\Users\\UserName\\AppData\\Roaming\\binarylane\\config.ini`\n\n\n### Environment variables\n\nFor environments where the use of `bl configure` and a permanent configuration\nfile are not suitable, environment variables may be utilised instead.\n\nThe environment variable `BL_API_TOKEN` may be used to provide the API token\nrequired to perform `bl` commands.\n\n## Versioning\n\n`bl` uses [semantic versioning](https://semver.org/spec/v2.0.0.html) to version\n[releases](https://github.com/binarylane/binarylane-cli/releases).\n\nSemantic versions are in the form of `MAJOR.MINOR.PATCH`. The value of `MAJOR`\nis currently **0**, which indicates that each new release of the `bl` program may\ncontain changes to its interface that are not backwards-compatible with\nprevious releases such as:\n\n - Command names may change, or moved within the command tree\n - Parameter names may change, or be removed entirely\n - Available field names may change, or be removed entirely\n - Default set of displayed fields displayed in output may change\n\nSuch changes in a new release are not likely to impact interactive use of `bl`,\nbut may cause problems for customers who integrate `bl` into non-interactive\nenvironments such as automation.\n\nIn non-interactive environments, customers should review the release\nChangelog prior to deploying an updated `0.x.y` release, and  ensure that any\nrequired adjustments to the non-interactive environment are made prior to\nupgrading the `bl` program itself.\n',
-    'author': "Nathan O'Sullivan",
-    'author_email': 'nathan.osullivan@mammoth.com.au',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+# `bl`: BinaryLane command-line interface
 
+```
+$ bl --help
+usage: bl [OPTIONS] COMMAND
+
+bl is a command-line interface for the BinaryLane API
+
+Options:
+  --help                Display available commands and descriptions
+
+Available Commands:
+    account             Access account commands
+    action              Access action commands
+    configure           Configure access to BinaryLane API
+    domain              Access domain commands
+    image               Access image commands
+    load-balancer       Access load-balancer commands
+    region              Access region commands
+    server              Access server commands
+    size                Access size commands
+    software            Access software commands
+    ssh-key             Access ssh-key commands
+    version             Show the current version
+    vpc                 Access vpc commands
+```
+
+## Installation
+
+`bl` requires Python 3.7 or later and has been tested on a variety of Linux
+distributions, Windows and Mac OSX. To install:
+
+```
+pip install binarylane-cli
+```
+
+### Portable install (without Python)
+
+The [releases page](https://github.com/binarylane/binarylane-cli/releases) has
+a standalone `bl.exe` for use on Windows.
+
+
+## Getting Started
+
+The BinaryLane CLI program is invoked by running `bl` (or `bl.exe` on Windows).
+To use `bl` you must configure the program with a BinaryLane customer access
+token.
+
+ 1. To start the configuration process, run:
+```
+bl configure
+```
+
+ 2. A prompt will be shown requesting access token. Go to [Developer API](https://home.binarylane.com.au/api-info) section of BinaryLane website and select **+ Create Token**, enter a name such as *CLI* and **Create**. 
+
+ 3. Copy the displayed token and paste at the `bl` *Enter your API access token:*
+prompt.
+
+ 4. To confirm token is working correctly, use `bl` to display BinaryLane account details:
+```
+bl account get
+``` 
+
+## Usage
+
+`bl` provides commands to access all functionality provided by the [BinaryLane
+API](https://api.binarylane.com.au/reference/), organised into a *command
+tree*. The general form for invoking an command is `bl NOUN [NOUN] VERB`.
+For example:
+
+ - `bl server list`: Displays list of servers
+ - `bl domain record create`: Create a DNS record
+
+The available commands at each level of the tree are displayed by running `bl`
+with no arguments:
+
+```
+$ bl
+
+usage: bl [OPTIONS] COMMAND
+
+bl is a command-line interface for the binaryLane API
+
+Options:
+  --help                Display available commands and descriptions
+
+Available Commands:
+    account             Access account commands
+    action              Access action commands
+    configure           Configure access to binaryLane API
+    domain              Access domain commands
+    image               Access image commands
+    load-balancer       Access load-balancer commands
+    region              Access region commands
+    server              Access server commands
+    size                Access size commands
+    software            Access software commands
+    ssh-key             Access ssh-key commands
+    version             Show the current version
+    vpc                 Access vpc commands
+```
+
+To see the available commands within the tree:
+
+```
+bl NOUN [NOUN]
+```
+
+For example:
+
+```
+$ bl domain
+usage: bl domain [OPTIONS] COMMAND
+
+Access domain commands
+
+Options:
+  --help                Display available commands and descriptions
+
+Available Commands:
+    create              Create a new domain
+    delete              Delete an existing domain
+    get                 Fetch an existing domain
+    list                List all domains
+    nameservers         Access domain nameservers commands
+    record              Access domain record commands
+```
+
+To see the required arguments and optional parameters for a command:
+
+```
+bl NOUN [NOUN] VERB --help
+```
+
+For example:
+
+```
+$ bl domain create --help
+usage: bl domain create [OPTIONS] --name NAME [PARAMETERS]
+
+Create a New Domain
+
+Options:
+  --help                Display command options and descriptions
+  --curl                Display API request as a 'curl' command-line
+  --no-header           Display columns without field labels
+  --output OUTPUT       Desired output format [plain, table, tsv, json] (Default: "table")
+
+Arguments:
+  --name NAME           The domain name to add to the DNS management system.
+
+Parameters:
+  --ip-address IP_ADDRESS
+                        An optional IPv4 address that will be used to create an A record for the root domain.
+```
+
+### Walkthrough: Creating a server
+
+Server creation is provided by the `bl server create` command. Use `--help` to
+view all arguments and parameters:
+
+```
+$ bl server list --help
+usage: bl server create [OPTIONS] --size SIZE --image IMAGE --region REGION [PARAMETERS]
+
+Create a new server.
+
+Options:
+  --help                Display command options and descriptions
+  --curl                Display API request as a 'curl' command-line
+  --no-header           Display columns without field labels
+  --output OUTPUT       Desired output format [plain, table, tsv, json] (Default: "table")
+  --async               Do not wait for requested action to complete
+  --quiet               Do not show progress while waiting for requested action to complete
+
+Arguments:
+  --size SIZE           The slug of the selected size.
+  --image IMAGE         The slug or id of the selected operating system.
+  --region REGION       The slug of the selected region.
+
+Parameters:
+  --name NAME           The hostname of your server, such as vps01.yourcompany.com. If not
+                        provided, the server will be created with a random name.
+  --backups, --no-backups
+                        If true this will enable two daily backups for the server.
+                        Options.daily_backups will override this value if provided. Setting
+                        this to false has no effect.
+  --ipv6, --no-ipv6     If true this will enable IPv6 for this server.
+  --ssh-keys [SSH_KEYS [SSH_KEYS ...]]
+                        This may be either the SSH keys Ids or fingerprints. If this is null
+                        or not provided any SSH keys that have been marked as default will be
+                        deployed (if the operating system supports SSH keys). Submit an empty
+                        array to disable deployment of default keys.
+  --password PASSWORD   If this is provided the default remote user account's password will be
+                        set to this value. If this is null a random password will be generated
+                        and emailed to the account email address.
+  <additional parameters omitted for brevity>
+```
+
+In the help displayed by `bl`, **Arguments** are required and **Parameters**
+are optional. For the `bl server list` command `--size SIZE`, `--image IMAGE`,
+and `--region REGION` are required. A list of available choices for each can be
+displayed by running:
+
+```
+bl size list
+bl image list
+bl region list
+```
+
+For example, to create a minimum-sized Ubuntu 22.04 LTS server in Sydney using
+SSH public key authentication:
+
+```
+$ bl server create --size std-min --image ubuntu-22.04-lts --region syd
+completed.
+┌───────────────────────────┬─────────────────────────────────────────────────────────────────────────────────────┐
+│ name                      │ value                                                                               │
+├───────────────────────────┼─────────────────────────────────────────────────────────────────────────────────────┤
+│ id                        │ 210658                                                                              │
+│ name                      │ giant-rudolf.bnr.la                                                                 │
+│ memory                    │ 1024                                                                                │
+│ vcpus                     │ 1                                                                                   │
+│ disk                      │ 20                                                                                  │
+│ created_at                │ 2023-01-20T02:02:32+00:00                                                           │
+│ status                    │ new                                                                                 │
+│ region                    │ Sydney                                                                              │
+│ image                     │ 20.04 LTS                                                                           │
+│ size                      │ std-min                                                                             │
+│ size_slug                 │ std-min                                                                             │
+│ networks                  │ v4: [{'ip_address': '175.45.180.1',  'type': 'public', 'netmask': '255.255.255.0... │
+  <additional rows omitted for brevity>
+└───────────────────────────┴─────────────────────────────────────────────────────────────────────────────────────┘
+```
+
+### Server passwords
+
+The use of SSH public key authentication is strongly recommended where
+possible. When public key authentication is not suitable or the image being
+deployed does not support SSH public key authentication (e.g. Windows Server),
+commands such as `bl server create` and `bl server action password-reset` have
+an optional `--password PASSWORD` parameter that specifies the password to use.
+
+For example, to create a server per the previous example with password
+authentication:
+
+```
+$ bl server create --size std-min --image ubuntu-22.04-lts --region syd --password 'qq7s6GYZgbiVG3'
+```
+
+Upon completion, the root password for the server in this example would be `qq7s6GYZgbiVG3`.
+
+:warning: **Internet-connected servers with password-based authentication enabled
+must have a strong, randomly generated password.** Brute-force login attempts
+are pervasive on the public internet: if a server password is not randomly
+generated, unauthorised access is likely to occur.
+
+### Server actions
+
+`bl` can be used to perform any action that the BinaryLane website can perform,
+including:
+
+ - Take and restore backups
+ - Change plan, operating system, or reinstall
+ - Restart and power cycle
+ - and many more...
+
+A list of available commands is displayed by running `bl server action`:
+
+```
+$ bl server action
+
+Available Commands:
+    add-disk            Create an additional disk for a server
+    attach-backup       Attach a backup to a server
+    change-advanced-features
+                        Change the advanced features of a server
+    change-advanced-firewall-rules
+                        Change the advanced firewall rules for a server
+    change-backup-schedule
+                        Change the backup schedule of a server
+    change-ipv6         Enable or disable IPv6 for a server
+    change-ipv6-reverse-nameservers
+                        Update the IPv6 reverse name servers for a server
+    change-kernel       Change the kernel of a server
+  <additional actions omitted for brevity>
+    ping                Attempt to ping a server
+    power-cycle         Power a server off and then on
+    power-off           Power a server off
+    power-on            Power a server on
+    reboot              Request a server perform a reboot
+    rebuild             Rebuild an existing server
+    rename              Rename a server
+    resize              Update the size and related options for a server
+    resize-disk         Alter the size of an existing disk for a server
+    restore             Restore a backup to a server
+    shutdown            Request a server perform a shutdown
+    take-backup         Take a backup of a server
+    uncancel            Revert the cancellation of a server
+    uptime              Check the uptime of a server
+```
+
+Each server action has a mandatory `SERVER_ID` argument  which can be obtained
+from `bl server list`.
+
+Many actions have additional *action-specific* arguments and parameters. Run
+`bl server action COMMAND --help` to see what a particular action supports.
+
+#### Example: password reset
+
+ 1. Use `--help` to see the available arguments and parameters:
+
+
+```
+$ bl server action password-reset --help
+usage: bl server action password-reset [OPTIONS] SERVER_ID [PARAMETERS]
+
+Reset the Password of a Server
+
+<options omitted for brevity>
+
+Arguments:
+  SERVER_ID            The ID of the server on which the action should be performed.
+
+Parameters:
+  --username USERNAME  The username of the user to change the password.
+  --password PASSWORD  If this is provided the specified or default remote user's account
+                       password will be set to this value.
+```
+
+ 2. Use `bl server list` to obtain the numeric server ID. In this example, the
+server requiring a password reset is ID 123456.
+
+ 3. Provide the server ID and desired password to the `password-reset` command:
+
+```
+bl server action password-reset 123456 --password 'qq7s6GYZgbiVG3'
+```
+
+### Asynchronous actions
+
+`bl` commands that perform an action - `bl create server`, `bl server
+action restore-backup`, and many others - default to *synchronous* handling
+where `bl` will display progress information to the console and not exit until
+the command finishes.
+
+In some scenarios such as when creating multiple servers, it may be desirable
+run the command with *asynchronous* handling where `bl` will exit as
+soon as the BinaryLane API accepts the requested command. To do so, include the
+`--async` option in the command invocation. For example:
+
+```
+$ bl server create --size std-min --image ubuntu-22.04-lts --region syd --async
+```
+
+### Configuration file
+
+`bl configure` creates a configuration file containing the API token, and reads
+that configuration file on subsequent invocations. The configuration file is
+stored at:
+
+ * `$XDG_CONFIG_HOME/binarylane/config.ini`
+
+Typically the environment variable `$XDG_CONFIG_HOME` is not set, in which case
+the configuration file stored at:
+
+ - **Linux/Mac/etc**: `$HOME/.config` - typical file location is
+   `/home/username/.config/binarylane/config.ini`
+ - **Windows**: `$APPDATA` - typical file location is
+   `C:\Users\UserName\AppData\Roaming\binarylane\config.ini`
+
+
+### Environment variables
+
+For environments where the use of `bl configure` and a permanent configuration
+file are not suitable, environment variables may be utilised instead.
+
+The environment variable `BL_API_TOKEN` may be used to provide the API token
+required to perform `bl` commands.
+
+## Versioning
+
+`bl` uses [semantic versioning](https://semver.org/spec/v2.0.0.html) to version
+[releases](https://github.com/binarylane/binarylane-cli/releases).
+
+Semantic versions are in the form of `MAJOR.MINOR.PATCH`. The value of `MAJOR`
+is currently **0**, which indicates that each new release of the `bl` program may
+contain changes to its interface that are not backwards-compatible with
+previous releases such as:
+
+ - Command names may change, or moved within the command tree
+ - Parameter names may change, or be removed entirely
+ - Available field names may change, or be removed entirely
+ - Default set of displayed fields displayed in output may change
+
+Such changes in a new release are not likely to impact interactive use of `bl`,
+but may cause problems for customers who integrate `bl` into non-interactive
+environments such as automation.
+
+In non-interactive environments, customers should review the release
+Changelog prior to deploying an updated `0.x.y` release, and  ensure that any
+required adjustments to the non-interactive environment are made prior to
+upgrading the `bl` program itself.
 
-setup(**setup_kwargs)
```

