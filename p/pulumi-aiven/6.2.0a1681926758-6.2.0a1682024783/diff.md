# Comparing `tmp/pulumi_aiven-6.2.0a1681926758.tar.gz` & `tmp/pulumi_aiven-6.2.0a1682024783.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aiven-6.2.0a1681926758.tar", last modified: Wed Apr 19 18:14:25 2023, max compression
+gzip compressed data, was "pulumi_aiven-6.2.0a1682024783.tar", last modified: Thu Apr 20 21:10:32 2023, max compression
```

## Comparing `pulumi_aiven-6.2.0a1681926758.tar` & `pulumi_aiven-6.2.0a1682024783.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:14:25.677051 pulumi_aiven-6.2.0a1681926758/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-19 18:14:25.677051 pulumi_aiven-6.2.0a1681926758/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:14:25.673051 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   599198 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/azure_privatelink_connection_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    73507 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26602 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/clickhouse_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/clickhouse_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/clickhouse_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:14:25.677051 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    73192 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/flink.py
--rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_cassanda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_clickhouse_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_flink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22261 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_pg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_service_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_transit_gateway_vpc_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    74761 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    73222 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    78050 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    76154 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    76710 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    75554 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    74440 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    75063 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    74183 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16700 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)   892539 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71601 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/pg.py
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    74559 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29938 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    53402 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/static_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    22097 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven/transit_gateway_vpc_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:14:25.677051 pulumi_aiven-6.2.0a1681926758/pulumi_aiven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/pulumi_aiven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:14:25.677051 pulumi_aiven-6.2.0a1681926758/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-19 18:14:25.000000 pulumi_aiven-6.2.0a1681926758/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:10:32.486400 pulumi_aiven-6.2.0a1682024783/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-20 21:10:32.486400 pulumi_aiven-6.2.0a1682024783/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:10:32.482400 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/
+-rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   596286 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/azure_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73507 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26602 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/clickhouse_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/clickhouse_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/clickhouse_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:10:32.486400 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73192 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_cassanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_clickhouse_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22261 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_service_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_transit_gateway_vpc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74761 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73222 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78050 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76154 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76710 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75554 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74440 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75063 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74183 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16700 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)   892539 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71601 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    74559 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29938 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53402 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22097 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven/transit_gateway_vpc_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:10:32.486400 pulumi_aiven-6.2.0a1682024783/pulumi_aiven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/pulumi_aiven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:10:32.486400 pulumi_aiven-6.2.0a1682024783/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-20 21:10:32.000000 pulumi_aiven-6.2.0a1682024783/setup.py
```

### Comparing `pulumi_aiven-6.2.0a1681926758/PKG-INFO` & `pulumi_aiven-6.2.0a1682024783/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_aiven
-Version: 6.2.0a1681926758
+Version: 6.2.0a1682024783
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-aiven/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-aiven/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Faiven.svg)](https://www.npmjs.com/package/@pulumi/aiven)
 [![Python version](https://badge.fury.io/py/pulumi-aiven.svg)](https://pypi.org/project/pulumi-aiven)
 [![NuGet version](https://badge.fury.io/nu/pulumi.aiven.svg)](https://badge.fury.io/nu/pulumi.aiven)
```

### Comparing `pulumi_aiven-6.2.0a1681926758/README.md` & `pulumi_aiven-6.2.0a1682024783/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/__init__.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/_inputs.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,16 +338,16 @@
         if cassandra_version is not None:
             pulumi.set(__self__, "cassandra_version", cassandra_version)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if migrate_sstableloader is not None:
             pulumi.set(__self__, "migrate_sstableloader", migrate_sstableloader)
         if private_access is not None:
             pulumi.set(__self__, "private_access", private_access)
         if project_to_fork_from is not None:
@@ -810,16 +810,16 @@
         if additional_backup_regions is not None:
             pulumi.set(__self__, "additional_backup_regions", additional_backup_regions)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if project_to_fork_from is not None:
             pulumi.set(__self__, "project_to_fork_from", project_to_fork_from)
         if service_to_fork_from is not None:
             pulumi.set(__self__, "service_to_fork_from", service_to_fork_from)
 
@@ -1404,16 +1404,16 @@
         if flink_version is not None:
             pulumi.set(__self__, "flink_version", flink_version)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if number_of_task_slots is not None:
             pulumi.set(__self__, "number_of_task_slots", number_of_task_slots)
         if privatelink_access is not None:
             pulumi.set(__self__, "privatelink_access", privatelink_access)
 
@@ -1813,16 +1813,16 @@
         if google_analytics_ua_id is not None:
             pulumi.set(__self__, "google_analytics_ua_id", google_analytics_ua_id)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if metrics_enabled is not None:
             pulumi.set(__self__, "metrics_enabled", metrics_enabled)
         if private_access is not None:
             pulumi.set(__self__, "private_access", private_access)
         if privatelink_access is not None:
@@ -3129,16 +3129,16 @@
         if influxdb is not None:
             pulumi.set(__self__, "influxdb", influxdb)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if private_access is not None:
             pulumi.set(__self__, "private_access", private_access)
         if privatelink_access is not None:
             pulumi.set(__self__, "privatelink_access", privatelink_access)
         if project_to_fork_from is not None:
@@ -3756,16 +3756,16 @@
         if additional_backup_regions is not None:
             pulumi.set(__self__, "additional_backup_regions", additional_backup_regions)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if kafka_connect is not None:
             pulumi.set(__self__, "kafka_connect", kafka_connect)
         if private_access is not None:
             pulumi.set(__self__, "private_access", private_access)
         if privatelink_access is not None:
@@ -4393,16 +4393,16 @@
         if custom_domain is not None:
             pulumi.set(__self__, "custom_domain", custom_domain)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if kafka is not None:
             pulumi.set(__self__, "kafka", kafka)
         if kafka_authentication_methods is not None:
             pulumi.set(__self__, "kafka_authentication_methods", kafka_authentication_methods)
         if kafka_connect is not None:
@@ -5824,16 +5824,16 @@
         if additional_backup_regions is not None:
             pulumi.set(__self__, "additional_backup_regions", additional_backup_regions)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if kafka_mirrormaker is not None:
             pulumi.set(__self__, "kafka_mirrormaker", kafka_mirrormaker)
         if static_ips is not None:
             pulumi.set(__self__, "static_ips", static_ips)
 
@@ -6710,16 +6710,16 @@
         if custom_domain is not None:
             pulumi.set(__self__, "custom_domain", custom_domain)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if m3_version is not None:
             warnings.warn("""Usage of this field is discouraged.""", DeprecationWarning)
             pulumi.log.warn("""m3_version is deprecated: Usage of this field is discouraged.""")
         if m3_version is not None:
             pulumi.set(__self__, "m3_version", m3_version)
@@ -6994,16 +6994,16 @@
         if custom_domain is not None:
             pulumi.set(__self__, "custom_domain", custom_domain)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if limits is not None:
             pulumi.set(__self__, "limits", limits)
         if m3 is not None:
             pulumi.set(__self__, "m3", m3)
         if m3_version is not None:
@@ -7558,16 +7558,16 @@
         if aggregations is not None:
             pulumi.set(__self__, "aggregations", aggregations)
         if drop is not None:
             pulumi.set(__self__, "drop", drop)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespaces is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with namespaces_string instead. When switching to namespaces_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""namespaces is deprecated: This will be removed in v5.0.0 and replaced with namespaces_string instead. When switching to namespaces_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with namespaces_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""namespaces is deprecated: This will be removed in v5.0.0 and replaced with namespaces_string instead.""")
         if namespaces is not None:
             pulumi.set(__self__, "namespaces", namespaces)
         if namespaces_objects is not None:
             pulumi.set(__self__, "namespaces_objects", namespaces_objects)
         if namespaces_strings is not None:
             pulumi.set(__self__, "namespaces_strings", namespaces_strings)
         if tags is not None:
@@ -7886,16 +7886,16 @@
         if binlog_retention_period is not None:
             pulumi.set(__self__, "binlog_retention_period", binlog_retention_period)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if migration is not None:
             pulumi.set(__self__, "migration", migration)
         if mysql is not None:
             pulumi.set(__self__, "mysql", mysql)
         if mysql_version is not None:
@@ -8921,16 +8921,16 @@
         if index_template is not None:
             pulumi.set(__self__, "index_template", index_template)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if keep_index_refresh_interval is not None:
             pulumi.set(__self__, "keep_index_refresh_interval", keep_index_refresh_interval)
         if max_index_count is not None:
             warnings.warn("""Usage of this field is discouraged.""", DeprecationWarning)
             pulumi.log.warn("""max_index_count is deprecated: Usage of this field is discouraged.""")
@@ -10255,16 +10255,16 @@
         if enable_ipv6 is not None:
             pulumi.set(__self__, "enable_ipv6", enable_ipv6)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if migration is not None:
             pulumi.set(__self__, "migration", migration)
         if pg is not None:
             pulumi.set(__self__, "pg", pg)
         if pg_read_replica is not None:
@@ -11902,16 +11902,16 @@
         if additional_backup_regions is not None:
             pulumi.set(__self__, "additional_backup_regions", additional_backup_regions)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
-            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""", DeprecationWarning)
-            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead. When switching to ip_filter_string, please apply the changes twice due to technical limitations.""")
+            warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
+            pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
         if migration is not None:
             pulumi.set(__self__, "migration", migration)
         if private_access is not None:
             pulumi.set(__self__, "private_access", private_access)
         if privatelink_access is not None:
```

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/_utilities.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/account.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/account_authentication.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/account_team.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/account_team_member.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/account_team_project.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/aws_privatelink.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/aws_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/azure_privatelink.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/azure_privatelink_connection_approval.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/azure_privatelink_connection_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/azure_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/billing_group.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/cassandra.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/cassandra_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/clickhouse.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/clickhouse_database.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/clickhouse_grant.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/clickhouse_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/clickhouse_role.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/clickhouse_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/clickhouse_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/config/vars.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/connection_pool.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/flink.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/flink_application.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/flink_application_version.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/gcp_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_account.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_account_authentication.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_account_team.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_account_team_member.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_account_team_project.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_aws_privatelink.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_aws_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_azure_privatelink.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_azure_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_billing_group.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_cassanda.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_cassanda.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_cassandra.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_cassandra_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_clickhouse.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_clickhouse_database.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_clickhouse_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_connection_pool.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_flink.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_flink_application.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_flink_application_version.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_gcp_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_grafana.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_influx_db.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_influxdb_database.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_influxdb_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_acl.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_connect.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_connector.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_mirror_maker.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_schema.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_schema_configuration.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_schema_registry_acl.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_topic.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_kafka_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_m3_aggregator.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_m3_db.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_m3db_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_mirror_maker_replication_flow.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_my_sql.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_mysql_database.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_mysql_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_open_search.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_open_search_acl_config.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_open_search_acl_rule.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_opensearch_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_pg.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_pg_database.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_pg_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_project.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_project_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_project_vpc.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_redis.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_redis_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_service_component.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_service_component.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_service_integration.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_service_integration_endpoint.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/get_transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/get_transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/grafana.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/influx_db.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/influxdb_database.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/influxdb_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_acl.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_connect.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_connector.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_mirror_maker.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_schema.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_schema_configuration.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_schema_registry_acl.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_topic.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/kafka_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/m3_aggregator.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/m3_db.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/m3db_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/mirror_maker_replication_flow.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/my_sql.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/mysql_database.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/mysql_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/open_search.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/open_search_acl_config.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/open_search_acl_rule.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/opensearch_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/outputs.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/pg.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/pg_database.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/pg_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/project.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/project_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/project_vpc.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/provider.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/redis.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/redis_user.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/service_integration.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/service_integration_endpoint.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/static_ip.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/static_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven/transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven.egg-info/PKG-INFO` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-aiven
-Version: 6.2.0a1681926758
+Version: 6.2.0a1682024783
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-aiven/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-aiven/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Faiven.svg)](https://www.npmjs.com/package/@pulumi/aiven)
 [![Python version](https://badge.fury.io/py/pulumi-aiven.svg)](https://pypi.org/project/pulumi-aiven)
 [![NuGet version](https://badge.fury.io/nu/pulumi.aiven.svg)](https://badge.fury.io/nu/pulumi.aiven)
```

### Comparing `pulumi_aiven-6.2.0a1681926758/pulumi_aiven.egg-info/SOURCES.txt` & `pulumi_aiven-6.2.0a1682024783/pulumi_aiven.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1681926758/setup.py` & `pulumi_aiven-6.2.0a1682024783/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.2.0a1681926758"
-PLUGIN_VERSION = "6.2.0-alpha.1681926758+48bf0ecf"
+VERSION = "6.2.0a1682024783"
+PLUGIN_VERSION = "6.2.0-alpha.1682024783+4dbd7e68"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aiven', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "aiven Pulumi Package - Development Version"
 
 
 setup(name='pulumi_aiven',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing Aiven cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

