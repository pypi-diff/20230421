# Comparing `tmp/apache-airflow-providers-amazon-7.4.1rc1.tar.gz` & `tmp/apache-airflow-providers-amazon-8.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-amazon-7.4.1rc1.tar", last modified: Sun Apr  9 13:48:06 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-amazon-8.0.0rc1.tar", last modified: Fri Apr 21 19:47:52 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-7.4.1rc1.tar` & `apache-airflow-providers-amazon-8.0.0rc1.tar`

### file list

```diff
@@ -1,169 +1,168 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:06.000000 apache-airflow-providers-amazon-7.4.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-7.4.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-04-09 13:48:01.000000 apache-airflow-providers-amazon-7.4.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-7.4.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    53299 2023-04-09 13:48:06.000000 apache-airflow-providers-amazon-7.4.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    51478 2023-04-09 13:48:01.000000 apache-airflow-providers-amazon-7.4.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12935 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    44515 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    19189 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)     9644 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7641 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    22191 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    13816 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13561 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    42450 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    57278 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     6826 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)     1217 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/aws_lambda.py
--rw-r--r--   0 root         (0) root         (0)    13603 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    30225 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    31781 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    46887 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     8343 2023-02-24 21:43:25.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    29868 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    28218 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8052 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    49835 2023-03-01 07:06:45.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16132 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     9198 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    18537 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2768 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     5857 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8639 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5036 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9198 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4569 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6185 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     7690 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20348 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/waiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)     1378 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)    36812 2023-04-09 13:48:01.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:06.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    53299 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7266 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      777 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-amazon-7.4.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-04-09 13:48:06.000000 apache-airflow-providers-amazon-7.4.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2356 2023-04-09 13:48:00.000000 apache-airflow-providers-amazon-7.4.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-04-21 19:47:47.000000 apache-airflow-providers-amazon-8.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    56663 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    54842 2023-04-21 19:47:47.000000 apache-airflow-providers-amazon-8.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12240 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    42181 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    20629 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)     9644 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7641 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    18990 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    13816 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13108 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    42450 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)    15828 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    29018 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    31753 2023-04-14 11:39:41.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    49023 2023-04-20 13:52:20.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    29868 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    28218 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    49835 2023-03-01 07:06:45.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15533 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    18505 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     5857 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     7676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8475 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20348 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/waiter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)    36826 2023-04-21 19:47:47.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    56663 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7207 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      777 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-amazon-8.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-04-21 19:47:47.000000 apache-airflow-providers-amazon-8.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/LICENSE` & `apache-airflow-providers-amazon-8.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/MANIFEST.in` & `apache-airflow-providers-amazon-8.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/PKG-INFO` & `apache-airflow-providers-amazon-8.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 7.4.1rc1
+Version: 8.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -60,28 +60,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``7.4.1rc1``
+Release: ``8.0.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -158,14 +158,84 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+8.0.0
+......
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  In this version of the provider, deprecated GCS hook's parameter ``delegate_to`` is removed from the following operators: ``GCSToS3Operator``, ``GlacierToGCSOperator`` and ``GoogleApiToS3Operator``.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+  Removed deprecated parameter ``google_cloud_storage_conn_id`` from ``GCSToS3Operator``, ``gcp_conn_id`` should be used instead.
+
+  Removed deprecated parameter ``max_tries`` from the Athena & EMR hook & operators in favor of ``max_polling_attempts``.
+
+  Disabled deprecated behavior of switching to an empty aws connection ID on error. You can set it to None explicitly.
+
+  Removed deprecated method ``waiter`` from emr hook in favor of the more generic ``airflow.providers.amazon.aws.utils.waiter.waiter``
+
+  Removed deprecated unused parameter ``cluster_identifier`` from Redshift Cluster's hook method ``get_cluster_snapshot_status``
+
+  Removed deprecated method ``find_processing_job_by_name`` from Sagemaker hook, use ``count_processing_jobs_by_name`` instead.
+
+  Removed deprecated module ``airflow.providers.amazon.aws.operators.aws_lambda`` in favor of ``airflow.providers.amazon.aws.operators.lambda_function``
+
+  Removed EcsOperator in favor of EcsRunTaskOperator.
+  EcsTaskLogFetcher and EcsProtocol should be imported from the hook.
+
+  Removed AwsLambdaInvokeFunctionOperator in favor of LambdaInvokeFunctionOperator.
+
+  Removed deprecated param ``await_result`` from RedshiftDataOperator in favor of ``wait_for_completion``.
+  Some methods from this operator should be imported from the hook instead.
+
+  Removed deprecated ``RedshiftSQLOperator`` in favor of the generic ``SQLExecuteQueryOperator``.
+  The parameter that was passed as ``redshift_conn_id`` needs to be changed to ``conn_id``, and the behavior should stay the same.
+
+  Removed deprecated method ``get_conn_uri`` from secrets manager in favor of ``get_conn_value``
+  Also removed deprecated method ``get_conn_uri`` from systems manager. ``deserialize_connection(...).get_uri()`` should be used instead.
+
+  Removed deprecated and unused param ``s3_conn_id`` from ``ImapAttachmentToS3Operator``, ``MongoToS3Operator`` and ``S3ToSFTPOperator``.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+* ``Remove deprecated code from Amazon provider (#30755)``
+
+Features
+~~~~~~~~
+
+* ``add a stop operator to emr serverless (#30720)``
+* ``SqlToS3Operator - Add feature to partition SQL table (#30460)``
+* ``New AWS sensor — DynamoDBValueSensor (#28338)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fixed logging issue (#30703)``
+* ``DynamoDBHook - waiter_path() to consider 'resource_type' or 'client_type' (#30595)``
+* ``Add ability to override waiter delay in EcsRunTaskOperator (#30586)``
+* ``Add support in AWS Batch Operator for multinode jobs (#29522)``
+* ``AWS logs. Exit fast when 3 consecutive responses are returned from AWS Cloudwatch logs (#30756)``
+
+Misc
+~~~~
+
+* ``Remove @poke_mode_only from EmrStepSensor (#30774)``
+* ``Organize Amazon providers docs index (#30541)``
+* ``Remove duplicate param docstring in EksPodOperator (#30634)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+
 7.4.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fix 'RedshiftResumeClusterOperator' deferrable implementation (#30370)``
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/README.rst` & `apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,52 @@
+Metadata-Version: 2.1
+Name: apache-airflow-providers-amazon
+Version: 8.0.0rc1
+Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
+Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
+Author: Apache Software Foundation
+Author-email: dev@airflow.apache.org
+License: Apache License 2.0
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
+Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
+Project-URL: Source Code, https://github.com/apache/airflow
+Project-URL: Slack Chat, https://s.apache.org/airflow-slack
+Project-URL: Twitter, https://twitter.com/ApacheAirflow
+Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Framework :: Apache Airflow
+Classifier: Framework :: Apache Airflow :: Provider
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: System :: Monitoring
+Requires-Python: ~=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: apache.hive
+Provides-Extra: cncf.kubernetes
+Provides-Extra: common.sql
+Provides-Extra: exasol
+Provides-Extra: ftp
+Provides-Extra: google
+Provides-Extra: imap
+Provides-Extra: mongo
+Provides-Extra: salesforce
+Provides-Extra: ssh
+Provides-Extra: pandas
+Provides-Extra: aiobotocore
+License-File: LICENSE
+License-File: NOTICE
+
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
@@ -15,28 +60,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``7.4.1rc1``
+Release: ``8.0.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -113,14 +158,84 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+8.0.0
+......
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  In this version of the provider, deprecated GCS hook's parameter ``delegate_to`` is removed from the following operators: ``GCSToS3Operator``, ``GlacierToGCSOperator`` and ``GoogleApiToS3Operator``.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+  Removed deprecated parameter ``google_cloud_storage_conn_id`` from ``GCSToS3Operator``, ``gcp_conn_id`` should be used instead.
+
+  Removed deprecated parameter ``max_tries`` from the Athena & EMR hook & operators in favor of ``max_polling_attempts``.
+
+  Disabled deprecated behavior of switching to an empty aws connection ID on error. You can set it to None explicitly.
+
+  Removed deprecated method ``waiter`` from emr hook in favor of the more generic ``airflow.providers.amazon.aws.utils.waiter.waiter``
+
+  Removed deprecated unused parameter ``cluster_identifier`` from Redshift Cluster's hook method ``get_cluster_snapshot_status``
+
+  Removed deprecated method ``find_processing_job_by_name`` from Sagemaker hook, use ``count_processing_jobs_by_name`` instead.
+
+  Removed deprecated module ``airflow.providers.amazon.aws.operators.aws_lambda`` in favor of ``airflow.providers.amazon.aws.operators.lambda_function``
+
+  Removed EcsOperator in favor of EcsRunTaskOperator.
+  EcsTaskLogFetcher and EcsProtocol should be imported from the hook.
+
+  Removed AwsLambdaInvokeFunctionOperator in favor of LambdaInvokeFunctionOperator.
+
+  Removed deprecated param ``await_result`` from RedshiftDataOperator in favor of ``wait_for_completion``.
+  Some methods from this operator should be imported from the hook instead.
+
+  Removed deprecated ``RedshiftSQLOperator`` in favor of the generic ``SQLExecuteQueryOperator``.
+  The parameter that was passed as ``redshift_conn_id`` needs to be changed to ``conn_id``, and the behavior should stay the same.
+
+  Removed deprecated method ``get_conn_uri`` from secrets manager in favor of ``get_conn_value``
+  Also removed deprecated method ``get_conn_uri`` from systems manager. ``deserialize_connection(...).get_uri()`` should be used instead.
+
+  Removed deprecated and unused param ``s3_conn_id`` from ``ImapAttachmentToS3Operator``, ``MongoToS3Operator`` and ``S3ToSFTPOperator``.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+* ``Remove deprecated code from Amazon provider (#30755)``
+
+Features
+~~~~~~~~
+
+* ``add a stop operator to emr serverless (#30720)``
+* ``SqlToS3Operator - Add feature to partition SQL table (#30460)``
+* ``New AWS sensor — DynamoDBValueSensor (#28338)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fixed logging issue (#30703)``
+* ``DynamoDBHook - waiter_path() to consider 'resource_type' or 'client_type' (#30595)``
+* ``Add ability to override waiter delay in EcsRunTaskOperator (#30586)``
+* ``Add support in AWS Batch Operator for multinode jobs (#29522)``
+* ``AWS logs. Exit fast when 3 consecutive responses are returned from AWS Cloudwatch logs (#30756)``
+
+Misc
+~~~~
+
+* ``Remove @poke_mode_only from EmrStepSensor (#30774)``
+* ``Organize Amazon providers docs index (#30541)``
+* ``Remove duplicate param docstring in EksPodOperator (#30634)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+
 7.4.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fix 'RedshiftResumeClusterOperator' deferrable implementation (#30370)``
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 .. spelling::
 
     PageIterator
 """
 from __future__ import annotations
 
-import warnings
 from time import sleep
 from typing import Any
 
 from botocore.paginate import PageIterator
 
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
@@ -220,37 +219,23 @@
         }
         paginator = self.get_conn().get_paginator("get_query_results")
         return paginator.paginate(**result_params)
 
     def poll_query_status(
         self,
         query_execution_id: str,
-        max_tries: int | None = None,
         max_polling_attempts: int | None = None,
     ) -> str | None:
         """
         Poll the status of submitted athena query until query state reaches final state.
         Returns one of the final states
 
         :param query_execution_id: Id of submitted athena query
-        :param max_tries: Deprecated - Use max_polling_attempts instead
         :param max_polling_attempts: Number of times to poll for query state before function exits
         """
-        if max_tries:
-            warnings.warn(
-                f"Passing 'max_tries' to {self.__class__.__name__}.poll_query_status is deprecated "
-                f"and will be removed in a future release. Please use 'max_polling_attempts' instead.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-            if max_polling_attempts and max_polling_attempts != max_tries:
-                raise Exception("max_polling_attempts must be the same value as max_tries")
-            else:
-                max_polling_attempts = max_tries
-
         try_number = 1
         final_query_state = None  # Query state when query reaches final state or max_polling_attempts reached
         while True:
             query_state = self.check_query_status(query_execution_id)
             if query_state is None:
                 self.log.info(
                     "Query execution id: %s, trial %s: Invalid query state. Retrying again",
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 import datetime
 import inspect
 import json
 import logging
 import os
 import uuid
-import warnings
 from copy import deepcopy
 from functools import wraps
 from os import PathLike
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Generic, TypeVar, Union
 
 import boto3
@@ -50,15 +49,14 @@
 from dateutil.tz import tzlocal
 from slugify import slugify
 
 from airflow.compat.functools import cached_property
 from airflow.configuration import conf
 from airflow.exceptions import (
     AirflowException,
-    AirflowNotFoundException,
 )
 from airflow.hooks.base import BaseHook
 from airflow.providers.amazon.aws.utils.connection_wrapper import AwsConnectionWrapper
 from airflow.providers.amazon.aws.waiters.base_waiter import BaseBotoWaiter
 from airflow.providers_manager import ProvidersManager
 from airflow.utils.helpers import exactly_one
 from airflow.utils.log.logging_mixin import LoggingMixin
@@ -358,42 +356,14 @@
             return google_id_token_credentials.token
 
         return web_identity_token_loader
 
     def _strip_invalid_session_name_characters(self, role_session_name: str) -> str:
         return slugify(role_session_name, regex_pattern=r"[^\w+=,.@-]+")
 
-    def _get_region_name(self) -> str | None:
-        warnings.warn(
-            "`BaseSessionFactory._get_region_name` method deprecated and will be removed "
-            "in a future releases. Please use `BaseSessionFactory.region_name` property instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.region_name
-
-    def _read_role_arn_from_extra_config(self) -> str | None:
-        warnings.warn(
-            "`BaseSessionFactory._read_role_arn_from_extra_config` method deprecated and will be removed "
-            "in a future releases. Please use `BaseSessionFactory.role_arn` property instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.role_arn
-
-    def _read_credentials_from_connection(self) -> tuple[str | None, str | None]:
-        warnings.warn(
-            "`BaseSessionFactory._read_credentials_from_connection` method deprecated and will be removed "
-            "in a future releases. Please use `BaseSessionFactory.conn.aws_access_key_id` and "
-            "`BaseSessionFactory.aws_secret_access_key` properties instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.conn.aws_access_key_id, self.conn.aws_secret_access_key
-
 
 class AwsGenericHook(BaseHook, Generic[BaseAwsConnection]):
     """
     Generic class for interact with AWS.
     This class provide a thin wrapper around the boto3 python library.
 
     :param aws_conn_id: The Airflow connection used for AWS credentials.
@@ -524,25 +494,15 @@
         return " ".join(user_agent_extra_values).strip()
 
     @cached_property
     def conn_config(self) -> AwsConnectionWrapper:
         """Get the Airflow Connection object and wrap it in helper (cached)."""
         connection = None
         if self.aws_conn_id:
-            try:
-                connection = self.get_connection(self.aws_conn_id)
-            except AirflowNotFoundException:
-                warnings.warn(
-                    f"Unable to find AWS Connection ID '{self.aws_conn_id}', switching to empty. "
-                    "This behaviour is deprecated and will be removed in a future releases. "
-                    "Please provide existed AWS connection ID or if required boto3 credential strategy "
-                    "explicit set AWS Connection ID to None.",
-                    DeprecationWarning,
-                    stacklevel=2,
-                )
+            connection = self.get_connection(self.aws_conn_id)
 
         return AwsConnectionWrapper(
             conn=connection, region_name=self._region_name, botocore_config=self._config, verify=self._verify
         )
 
     @property
     def service_config(self) -> dict:
@@ -726,25 +686,14 @@
                 }
                 return tenacity.retry(**default_kwargs)(fun)(self, *args, **kwargs)
 
             return decorator_f
 
         return retry_decorator
 
-    def _get_credentials(self, region_name: str | None) -> tuple[boto3.session.Session, str | None]:
-        warnings.warn(
-            "`AwsGenericHook._get_credentials` method deprecated and will be removed in a future releases. "
-            "Please use `AwsGenericHook.get_session` method and "
-            "`AwsGenericHook.conn_config.endpoint_url` property instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-        return self.get_session(region_name=region_name), self.conn_config.endpoint_url
-
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
         """Returns custom UI field behaviour for AWS Connection."""
         return {
             "hidden_fields": ["host", "schema", "port"],
             "relabeling": {
                 "login": "AWS Access Key ID",
@@ -790,15 +739,16 @@
             return True, ", ".join(f"{k}={v!r}" for k, v in conn_info.items())
 
         except Exception as e:
             return False, str(f"{type(e).__name__!r} error occurred while testing connection: {e}")
 
     @cached_property
     def waiter_path(self) -> PathLike[str] | None:
-        path = Path(__file__).parents[1].joinpath(f"waiters/{self.client_type}.json").resolve()
+        filename = self.client_type if self.client_type else self.resource_type
+        path = Path(__file__).parents[1].joinpath(f"waiters/{filename}.json").resolve()
         return path if path.exists() else None
 
     def get_waiter(self, waiter_name: str, parameters: dict[str, str] | None = None) -> Waiter:
         """
         First checks if there is a custom waiter with the provided waiter_name and
         uses that if it exists, otherwise it will check the service client for a
         waiter that matches the name and pass that through.
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -410,51 +410,84 @@
         matching_jobs = [job for job in jobs if job.get("jobId") == job_id]
         if len(matching_jobs) != 1:
             raise AirflowException(f"AWS Batch job ({job_id}) description error: response: {response}")
 
         return matching_jobs[0]
 
     def get_job_awslogs_info(self, job_id: str) -> dict[str, str] | None:
+        all_info = self.get_job_all_awslogs_info(job_id)
+        if not all_info:
+            return None
+        if len(all_info) > 1:
+            self.log.warning(
+                f"AWS Batch job ({job_id}) has more than one log stream, " f"only returning the first one."
+            )
+        return all_info[0]
+
+    def get_job_all_awslogs_info(self, job_id: str) -> list[dict[str, str]]:
         """
         Parse job description to extract AWS CloudWatch information.
 
         :param job_id: AWS Batch Job ID
         """
-        job_container_desc = self.get_job_description(job_id=job_id).get("container", {})
-        log_configuration = job_container_desc.get("logConfiguration", {})
+        job_desc = self.get_job_description(job_id=job_id)
+
+        job_node_properties = job_desc.get("nodeProperties", {})
+        job_container_desc = job_desc.get("container", {})
 
-        # In case if user select other "logDriver" rather than "awslogs"
-        # than CloudWatch logging should be disabled.
-        # If user not specify anything than expected that "awslogs" will use
-        # with default settings:
-        #   awslogs-group = /aws/batch/job
-        #   awslogs-region = `same as AWS Batch Job region`
-        log_driver = log_configuration.get("logDriver", "awslogs")
-        if log_driver != "awslogs":
+        if job_node_properties:
+            # one log config per node
+            log_configs = [
+                p.get("container", {}).get("logConfiguration", {})
+                for p in job_node_properties.get("nodeRangeProperties", {})
+            ]
+            # one stream name per attempt
+            stream_names = [a.get("container", {}).get("logStreamName") for a in job_desc.get("attempts", [])]
+        elif job_container_desc:
+            log_configs = [job_container_desc.get("logConfiguration", {})]
+            stream_name = job_container_desc.get("logStreamName")
+            stream_names = [stream_name] if stream_name is not None else []
+        else:
+            raise AirflowException(
+                f"AWS Batch job ({job_id}) is not a supported job type. "
+                "Supported job types: container, array, multinode."
+            )
+
+        # If the user selected another logDriver than "awslogs", then CloudWatch logging is disabled.
+        if any([c.get("logDriver", "awslogs") != "awslogs" for c in log_configs]):
             self.log.warning(
-                "AWS Batch job (%s) uses logDriver (%s). AWS CloudWatch logging disabled.", job_id, log_driver
+                f"AWS Batch job ({job_id}) uses non-aws log drivers. AWS CloudWatch logging disabled."
             )
-            return None
+            return []
 
-        awslogs_stream_name = job_container_desc.get("logStreamName")
-        if not awslogs_stream_name:
-            # In case of call this method on very early stage of running AWS Batch
-            # there is possibility than AWS CloudWatch Stream Name not exists yet.
-            # AWS CloudWatch Stream Name also not created in case of misconfiguration.
-            self.log.warning("AWS Batch job (%s) doesn't create AWS CloudWatch Stream.", job_id)
-            return None
+        if not stream_names:
+            # If this method is called very early after starting the AWS Batch job,
+            # there is a possibility that the AWS CloudWatch Stream Name would not exist yet.
+            # This can also happen in case of misconfiguration.
+            self.log.warning(f"AWS Batch job ({job_id}) doesn't have any AWS CloudWatch Stream.")
+            return []
 
         # Try to get user-defined log configuration options
-        log_options = log_configuration.get("options", {})
+        log_options = [c.get("options", {}) for c in log_configs]
 
-        return {
-            "awslogs_stream_name": awslogs_stream_name,
-            "awslogs_group": log_options.get("awslogs-group", "/aws/batch/job"),
-            "awslogs_region": log_options.get("awslogs-region", self.conn_region_name),
-        }
+        # cross stream names with options (i.e. attempts X nodes) to generate all log infos
+        result = []
+        for stream in stream_names:
+            for option in log_options:
+                result.append(
+                    {
+                        "awslogs_stream_name": stream,
+                        # If the user did not specify anything, the default settings are:
+                        #   awslogs-group = /aws/batch/job
+                        #   awslogs-region = `same as AWS Batch Job region`
+                        "awslogs_group": option.get("awslogs-group", "/aws/batch/job"),
+                        "awslogs_region": option.get("awslogs-region", self.conn_region_name),
+                    }
+                )
+        return result
 
     @staticmethod
     def add_jitter(delay: int | float, width: int | float = 1, minima: int | float = 0) -> float:
         """
         Use delay +/- width for random jitter
 
         Adding jitter to status polling can help to avoid
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,22 +16,21 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
 import warnings
 from time import sleep
-from typing import Any, Callable
+from typing import Any
 
 from botocore.exceptions import ClientError
 
 from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowNotFoundException
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
-from airflow.providers.amazon.aws.utils.waiter import get_state, waiter
 from airflow.utils.helpers import prune_dict
 
 
 class EmrHook(AwsBaseHook):
     """
     Interact with Amazon Elastic MapReduce Service (EMR).
     Provide thick wrapper around :external+boto3:py:class:`boto3.client("emr") <EMR.Client>`.
@@ -255,70 +254,14 @@
         super().__init__(*args, **kwargs)
 
     @cached_property
     def conn(self):
         """Get the underlying boto3 EmrServerlessAPIService client (cached)"""
         return super().conn
 
-    # This method should be replaced with boto waiters which would implement timeouts and backoff nicely.
-    def waiter(
-        self,
-        get_state_callable: Callable,
-        get_state_args: dict,
-        parse_response: list,
-        desired_state: set,
-        failure_states: set,
-        object_type: str,
-        action: str,
-        countdown: int = 25 * 60,
-        check_interval_seconds: int = 60,
-    ) -> None:
-        """
-        Will run the sensor until it turns True.
-
-        :param get_state_callable: A callable to run until it returns True
-        :param get_state_args: Arguments to pass to get_state_callable
-        :param parse_response: Dictionary keys to extract state from response of get_state_callable
-        :param desired_state: Wait until the getter returns this value
-        :param failure_states: A set of states which indicate failure and should throw an
-            exception if any are reached before the desired_state
-        :param object_type: Used for the reporting string. What are you waiting for? (application, job, etc)
-        :param action: Used for the reporting string. What action are you waiting for? (created, deleted, etc)
-        :param countdown: Total amount of time the waiter should wait for the desired state
-            before timing out (in seconds). Defaults to 25 * 60 seconds.
-        :param check_interval_seconds: Number of seconds waiter should wait before attempting
-            to retry get_state_callable. Defaults to 60 seconds.
-        """
-        warnings.warn(
-            """This method is deprecated.
-            Please use `airflow.providers.amazon.aws.utils.waiter.waiter`.""",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        waiter(
-            get_state_callable=get_state_callable,
-            get_state_args=get_state_args,
-            parse_response=parse_response,
-            desired_state=desired_state,
-            failure_states=failure_states,
-            object_type=object_type,
-            action=action,
-            countdown=countdown,
-            check_interval_seconds=check_interval_seconds,
-        )
-
-    def get_state(self, response, keys) -> str:
-        warnings.warn(
-            """This method is deprecated.
-            Please use `airflow.providers.amazon.aws.utils.waiter.get_state`.""",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return get_state(response=response, keys=keys)
-
 
 class EmrContainerHook(AwsBaseHook):
     """
     Interact with Amazon EMR Containers (Amazon EMR on EKS).
     Provide thick wrapper around :py:class:`boto3.client("emr-containers") <EMRContainers.Client>`.
 
     :param virtual_cluster_id: Cluster ID of the EMR on EKS virtual cluster
@@ -479,39 +422,25 @@
             # If we receive a generic ClientError, we swallow the exception so that the
             self.log.error("AWS request failed, check logs for more info: %s", ex)
             return None
 
     def poll_query_status(
         self,
         job_id: str,
-        max_tries: int | None = None,
         poll_interval: int = 30,
         max_polling_attempts: int | None = None,
     ) -> str | None:
         """
         Poll the status of submitted job run until query state reaches final state.
         Returns one of the final states.
 
         :param job_id: The ID of the job run request.
-        :param max_tries: Deprecated - Use max_polling_attempts instead
         :param poll_interval: Time (in seconds) to wait between calls to check query status on EMR
         :param max_polling_attempts: Number of times to poll for query state before function exits
         """
-        if max_tries:
-            warnings.warn(
-                f"Method `{self.__class__.__name__}.max_tries` is deprecated and will be removed "
-                "in a future release.  Please use method `max_polling_attempts` instead.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-            if max_polling_attempts and max_polling_attempts != max_tries:
-                raise Exception("max_polling_attempts must be the same value as max_tries")
-            else:
-                max_polling_attempts = max_tries
-
         try_number = 1
         final_query_state = None  # Query state when query reaches final state or max_polling_attempts reached
 
         while True:
             query_state = self.check_query_status(job_id)
             if query_state is None:
                 self.log.info("Try %s: Invalid query state. Retrying again", try_number)
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,92 +11,93 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""
-This module contains a hook (AwsLogsHook) with some very basic
-functionality for interacting with AWS CloudWatch.
-"""
 from __future__ import annotations
 
-from typing import Generator
+from enum import Enum
+from typing import TYPE_CHECKING, Any, Sequence
 
-from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
+from airflow.compat.functools import cached_property
+from airflow.exceptions import AirflowException
+from airflow.providers.amazon.aws.hooks.glacier import GlacierHook
+from airflow.sensors.base import BaseSensorOperator
 
+if TYPE_CHECKING:
+    from airflow.utils.context import Context
+
+
+class JobStatus(Enum):
+    """Glacier jobs description"""
+
+    IN_PROGRESS = "InProgress"
+    SUCCEEDED = "Succeeded"
 
-class AwsLogsHook(AwsBaseHook):
-    """
-    Interact with Amazon CloudWatch Logs.
-    Provide thin wrapper around :external+boto3:py:class:`boto3.client("logs") <CloudWatchLogs.Client>`.
 
-    Additional arguments (such as ``aws_conn_id``) may be specified and
-    are passed down to the underlying AwsBaseHook.
+class GlacierJobOperationSensor(BaseSensorOperator):
+    """
+    Glacier sensor for checking job state. This operator runs only in reschedule mode.
 
     .. seealso::
-        - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
+        For more information on how to use this sensor, take a look at the guide:
+        :ref:`howto/sensor:GlacierJobOperationSensor`
+
+    :param aws_conn_id: The reference to the AWS connection details
+    :param vault_name: name of Glacier vault on which job is executed
+    :param job_id: the job ID was returned by retrieve_inventory()
+    :param poke_interval: Time in seconds that the job should wait in
+        between each tries
+    :param mode: How the sensor operates.
+        Options are: ``{ poke | reschedule }``, default is ``poke``.
+        When set to ``poke`` the sensor is taking up a worker slot for its
+        whole execution time and sleeps between pokes. Use this mode if the
+        expected runtime of the sensor is short or if a short poke interval
+        is required. Note that the sensor will hold onto a worker slot and
+        a pool slot for the duration of the sensor's runtime in this mode.
+        When set to ``reschedule`` the sensor task frees the worker slot when
+        the criteria is not yet met and it's rescheduled at a later time. Use
+        this mode if the time before the criteria is met is expected to be
+        quite long. The poke interval should be more than one minute to
+        prevent too much load on the scheduler.
     """
 
-    def __init__(self, *args, **kwargs) -> None:
-        kwargs["client_type"] = "logs"
-        super().__init__(*args, **kwargs)
+    template_fields: Sequence[str] = ("vault_name", "job_id")
 
-    def get_log_events(
+    def __init__(
         self,
-        log_group: str,
-        log_stream_name: str,
-        start_time: int = 0,
-        skip: int = 0,
-        start_from_head: bool = True,
-    ) -> Generator:
-        """
-        A generator for log items in a single stream. This will yield all the
-        items that are available at the current moment.
-
-        .. seealso::
-            - :external+boto3:py:meth:`CloudWatchLogs.Client.get_log_events`
-
-        :param log_group: The name of the log group.
-        :param log_stream_name: The name of the specific stream.
-        :param start_time: The time stamp value to start reading the logs from (default: 0).
-        :param skip: The number of log entries to skip at the start (default: 0).
-            This is for when there are multiple entries at the same timestamp.
-        :param start_from_head: whether to start from the beginning (True) of the log or
-            at the end of the log (False).
-        :return: | A CloudWatch log event with the following key-value pairs:
-                 |   'timestamp' (int): The time in milliseconds of the event.
-                 |   'message' (str): The log event data.
-                 |   'ingestionTime' (int): The time in milliseconds the event was ingested.
-        """
-        next_token = None
-        while True:
-            if next_token is not None:
-                token_arg: dict[str, str] | None = {"nextToken": next_token}
-            else:
-                token_arg = {}
-
-            response = self.get_conn().get_log_events(
-                logGroupName=log_group,
-                logStreamName=log_stream_name,
-                startTime=start_time,
-                startFromHead=start_from_head,
-                **token_arg,
+        *,
+        aws_conn_id: str = "aws_default",
+        vault_name: str,
+        job_id: str,
+        poke_interval: int = 60 * 20,
+        mode: str = "reschedule",
+        **kwargs: Any,
+    ) -> None:
+        super().__init__(**kwargs)
+        self.aws_conn_id = aws_conn_id
+        self.vault_name = vault_name
+        self.job_id = job_id
+        self.poke_interval = poke_interval
+        self.mode = mode
+
+    @cached_property
+    def hook(self):
+        return GlacierHook(aws_conn_id=self.aws_conn_id)
+
+    def poke(self, context: Context) -> bool:
+        response = self.hook.describe_job(vault_name=self.vault_name, job_id=self.job_id)
+
+        if response["StatusCode"] == JobStatus.SUCCEEDED.value:
+            self.log.info("Job status: %s, code status: %s", response["Action"], response["StatusCode"])
+            self.log.info("Job finished successfully")
+            return True
+        elif response["StatusCode"] == JobStatus.IN_PROGRESS.value:
+            self.log.info("Processing...")
+            self.log.warning("Code status: %s", response["StatusCode"])
+            return False
+        else:
+            raise AirflowException(
+                f'Sensor failed. Job status: {response["Action"]}, code status: {response["StatusCode"]}'
             )
-
-            events = response["events"]
-            event_count = len(events)
-
-            if event_count > skip:
-                events = events[skip:]
-                skip = 0
-            else:
-                skip -= event_count
-                events = []
-
-            yield from events
-
-            if next_token != response["nextForwardToken"]:
-                next_token = response["nextForwardToken"]
-            else:
-                return
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import asyncio
-import warnings
 from typing import Any, Sequence
 
 import botocore.exceptions
 from botocore.exceptions import ClientError
 
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseAsyncHook, AwsBaseHook
 
@@ -173,30 +172,20 @@
         response = self.get_conn().create_cluster_snapshot(
             SnapshotIdentifier=snapshot_identifier,
             ClusterIdentifier=cluster_identifier,
             ManualSnapshotRetentionPeriod=retention_period,
         )
         return response["Snapshot"] if response["Snapshot"] else None
 
-    def get_cluster_snapshot_status(self, snapshot_identifier: str, cluster_identifier: str | None = None):
+    def get_cluster_snapshot_status(self, snapshot_identifier: str):
         """
         Return Redshift cluster snapshot status. If cluster snapshot not found return ``None``
 
         :param snapshot_identifier: A unique identifier for the snapshot that you are requesting
-        :param cluster_identifier: (deprecated) The unique identifier of the cluster
-            the snapshot was created from
         """
-        if cluster_identifier:
-            warnings.warn(
-                "Parameter `cluster_identifier` is deprecated."
-                "This option will be removed in a future version.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-
         try:
             response = self.get_conn().describe_cluster_snapshots(
                 SnapshotIdentifier=snapshot_identifier,
             )
             snapshot = response.get("Snapshots")[0]
             snapshot_status: str = snapshot.get("Status")
             return snapshot_status
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 import collections
 import os
 import re
 import tarfile
 import tempfile
 import time
-import warnings
 from collections import Counter
 from datetime import datetime
 from functools import partial
 from typing import Any, Callable, Generator, cast
 
 from botocore.exceptions import ClientError
 
@@ -973,29 +972,14 @@
 
             if "NextToken" not in response or (max_results is not None and len(results) == max_results):
                 # Return when there are no results left (no NextToken) or when we've reached max_results.
                 return results
             else:
                 next_token = response["NextToken"]
 
-    def find_processing_job_by_name(self, processing_job_name: str) -> bool:
-        """
-        Query processing job by name
-
-        This method is deprecated.
-        Please use `airflow.providers.amazon.aws.hooks.sagemaker.count_processing_jobs_by_name`.
-        """
-        warnings.warn(
-            "This method is deprecated. "
-            "Please use `airflow.providers.amazon.aws.hooks.sagemaker.count_processing_jobs_by_name`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return bool(self.count_processing_jobs_by_name(processing_job_name))
-
     @staticmethod
     def _name_matches_pattern(
         processing_job_name: str,
         found_name: str,
         job_name_suffix: str | None = None,
     ) -> bool:
         pattern = re.compile(f"^{processing_job_name}({job_name_suffix})?$")
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/athena.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-import warnings
 from typing import TYPE_CHECKING, Any, Sequence
 
 from airflow.compat.functools import cached_property
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.athena import AthenaHook
 
 if TYPE_CHECKING:
@@ -41,15 +40,14 @@
     :param output_location: s3 path to write the query results into. (templated)
     :param aws_conn_id: aws connection to use
     :param client_request_token: Unique token created by user to avoid multiple executions of same query
     :param workgroup: Athena workgroup in which query will be run
     :param query_execution_context: Context in which query need to be run
     :param result_configuration: Dict with path to store results in and config related to encryption
     :param sleep_time: Time (in seconds) to wait between two consecutive calls to check query status on Athena
-    :param max_tries: Deprecated - use max_polling_attempts instead.
     :param max_polling_attempts: Number of times to poll for query state before function exits
         To limit task execution time, use execution_timeout.
     :param log_query: Whether to log athena query and other execution params when it's executed.
         Defaults to *True*.
     """
 
     ui_color = "#44b5e2"
@@ -65,15 +63,14 @@
         output_location: str,
         aws_conn_id: str = "aws_default",
         client_request_token: str | None = None,
         workgroup: str = "primary",
         query_execution_context: dict[str, str] | None = None,
         result_configuration: dict[str, Any] | None = None,
         sleep_time: int = 30,
-        max_tries: int | None = None,
         max_polling_attempts: int | None = None,
         log_query: bool = True,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         self.query = query
         self.database = database
@@ -84,26 +81,14 @@
         self.query_execution_context = query_execution_context or {}
         self.result_configuration = result_configuration or {}
         self.sleep_time = sleep_time
         self.max_polling_attempts = max_polling_attempts
         self.query_execution_id: str | None = None
         self.log_query: bool = log_query
 
-        if max_tries:
-            warnings.warn(
-                f"Parameter `{self.__class__.__name__}.max_tries` is deprecated and will be removed "
-                "in a future release.  Please use method `max_polling_attempts` instead.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-            if max_polling_attempts and max_polling_attempts != max_tries:
-                raise Exception("max_polling_attempts must be the same value as max_tries")
-            else:
-                self.max_polling_attempts = max_tries
-
     @cached_property
     def hook(self) -> AthenaHook:
         """Create and return an AthenaHook."""
         return AthenaHook(self.aws_conn_id, sleep_time=self.sleep_time, log_query=self.log_query)
 
     def execute(self, context: Context) -> str | None:
         """Run Presto Query on Athena"""
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/aws_lambda.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -11,19 +10,19 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""This module is deprecated. Please use :mod:`airflow.providers.amazon.aws.operators.lambda_function`."""
+
 from __future__ import annotations
 
-import warnings
+from enum import Enum
+
 
-from airflow.providers.amazon.aws.operators.lambda_function import AwsLambdaInvokeFunctionOperator  # noqa
+class ApprovalStatus(Enum):
+    """Approval statuses for a Sagemaker Model Package."""
 
-warnings.warn(
-    "This module is deprecated. Please use `airflow.providers.amazon.aws.operators.lambda_function`.",
-    DeprecationWarning,
-    stacklevel=2,
-)
+    APPROVED = "Approved"
+    REJECTED = "Rejected"
+    PENDING_MANUAL_APPROVAL = "PendingManualApproval"
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     - https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
     - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html
     - https://docs.aws.amazon.com/batch/latest/APIReference/Welcome.html
 """
 from __future__ import annotations
 
+import warnings
 from typing import TYPE_CHECKING, Any, Sequence
 
 from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.batch_client import BatchClientHook
 from airflow.providers.amazon.aws.links.batch import (
@@ -50,15 +51,17 @@
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:BatchOperator`
 
     :param job_name: the name for the job that will run on AWS Batch (templated)
     :param job_definition: the job definition name on AWS Batch
     :param job_queue: the queue name on AWS Batch
-    :param overrides: the `containerOverrides` parameter for boto3 (templated)
+    :param overrides: DEPRECATED, use container_overrides instead with the same value.
+    :param container_overrides: the `containerOverrides` parameter for boto3 (templated)
+    :param node_overrides: the `nodeOverrides` parameter for boto3 (templated)
     :param array_properties: the `arrayProperties` parameter for boto3
     :param parameters: the `parameters` for boto3 (templated)
     :param job_id: the job ID, usually unknown (None) until the
         submit_job operation gets the jobId defined by AWS Batch
     :param waiters: an :py:class:`.BatchWaiters` object (see note below);
         if None, polling is used with max_retries and status_retries.
     :param max_retries: exponential back-off retries, 4200 = 48 hours;
@@ -84,22 +87,27 @@
     ui_color = "#c3dae0"
     arn: str | None = None
     template_fields: Sequence[str] = (
         "job_id",
         "job_name",
         "job_definition",
         "job_queue",
-        "overrides",
+        "container_overrides",
         "array_properties",
+        "node_overrides",
         "parameters",
         "waiters",
         "tags",
         "wait_for_completion",
     )
-    template_fields_renderers = {"overrides": "json", "parameters": "json"}
+    template_fields_renderers = {
+        "container_overrides": "json",
+        "parameters": "json",
+        "node_overrides": "json",
+    }
 
     @property
     def operator_extra_links(self):
         op_extra_links = [BatchJobDetailsLink()]
         if self.wait_for_completion:
             op_extra_links.extend([BatchJobDefinitionLink(), BatchJobQueueLink()])
         if not self.array_properties:
@@ -110,16 +118,18 @@
 
     def __init__(
         self,
         *,
         job_name: str,
         job_definition: str,
         job_queue: str,
-        overrides: dict,
+        overrides: dict | None = None,  # deprecated
+        container_overrides: dict | None = None,
         array_properties: dict | None = None,
+        node_overrides: dict | None = None,
         parameters: dict | None = None,
         job_id: str | None = None,
         waiters: Any | None = None,
         max_retries: int | None = None,
         status_retries: int | None = None,
         aws_conn_id: str | None = None,
         region_name: str | None = None,
@@ -129,25 +139,51 @@
     ):
 
         BaseOperator.__init__(self, **kwargs)
         self.job_id = job_id
         self.job_name = job_name
         self.job_definition = job_definition
         self.job_queue = job_queue
-        self.overrides = overrides or {}
-        self.array_properties = array_properties or {}
+
+        self.container_overrides = container_overrides
+        # handle `overrides` deprecation in favor of `container_overrides`
+        if overrides:
+            if container_overrides:
+                # disallow setting both old and new params
+                raise AirflowException(
+                    "'container_overrides' replaces the 'overrides' parameter. "
+                    "You cannot specify both. Please remove assignation to the deprecated 'overrides'."
+                )
+            self.container_overrides = overrides
+            warnings.warn(
+                "Parameter `overrides` is deprecated, Please use `container_overrides` instead.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
+        self.node_overrides = node_overrides
+        self.array_properties = array_properties
         self.parameters = parameters or {}
         self.waiters = waiters
         self.tags = tags or {}
         self.wait_for_completion = wait_for_completion
-        self.hook = BatchClientHook(
-            max_retries=max_retries,
-            status_retries=status_retries,
-            aws_conn_id=aws_conn_id,
-            region_name=region_name,
+
+        # params for hook
+        self.max_retries = max_retries
+        self.status_retries = status_retries
+        self.aws_conn_id = aws_conn_id
+        self.region_name = region_name
+
+    @cached_property
+    def hook(self) -> BatchClientHook:
+        return BatchClientHook(
+            max_retries=self.max_retries,
+            status_retries=self.status_retries,
+            aws_conn_id=self.aws_conn_id,
+            region_name=self.region_name,
         )
 
     def execute(self, context: Context):
         """
         Submit and monitor an AWS Batch job
 
         :raises: AirflowException
@@ -170,26 +206,35 @@
         :raises: AirflowException
         """
         self.log.info(
             "Running AWS Batch job - job definition: %s - on queue %s",
             self.job_definition,
             self.job_queue,
         )
-        self.log.info("AWS Batch job - container overrides: %s", self.overrides)
+
+        if self.container_overrides:
+            self.log.info("AWS Batch job - container overrides: %s", self.container_overrides)
+        if self.array_properties:
+            self.log.info("AWS Batch job - array properties: %s", self.array_properties)
+        if self.node_overrides:
+            self.log.info("AWS Batch job - node properties: %s", self.node_overrides)
+
+        args = {
+            "jobName": self.job_name,
+            "jobQueue": self.job_queue,
+            "jobDefinition": self.job_definition,
+            "arrayProperties": self.array_properties,
+            "parameters": self.parameters,
+            "tags": self.tags,
+            "containerOverrides": self.container_overrides,
+            "nodeOverrides": self.node_overrides,
+        }
 
         try:
-            response = self.hook.client.submit_job(
-                jobName=self.job_name,
-                jobQueue=self.job_queue,
-                jobDefinition=self.job_definition,
-                arrayProperties=self.array_properties,
-                parameters=self.parameters,
-                containerOverrides=self.overrides,
-                tags=self.tags,
-            )
+            response = self.hook.client.submit_job(**trim_none_values(args))
         except Exception as e:
             self.log.error(
                 "AWS Batch job failed submission - job definition: %s - on queue %s",
                 self.job_definition,
                 self.job_queue,
             )
             raise AirflowException(e)
@@ -245,23 +290,32 @@
             )
 
         if self.waiters:
             self.waiters.wait_for_job(self.job_id)
         else:
             self.hook.wait_for_job(self.job_id)
 
-        awslogs = self.hook.get_job_awslogs_info(self.job_id)
+        awslogs = self.hook.get_job_all_awslogs_info(self.job_id)
         if awslogs:
-            self.log.info("AWS Batch job (%s) CloudWatch Events details found: %s", self.job_id, awslogs)
+            self.log.info("AWS Batch job (%s) CloudWatch Events details found. Links to logs:", self.job_id)
+            link_builder = CloudWatchEventsLink()
+            for log in awslogs:
+                self.log.info(link_builder.format_link(**log))
+            if len(awslogs) > 1:
+                # there can be several log streams on multi-node jobs
+                self.log.warning(
+                    "out of all those logs, we can only link to one in the UI. " "Using the first one."
+                )
+
             CloudWatchEventsLink.persist(
                 context=context,
                 operator=self,
                 region_name=self.hook.conn_region_name,
                 aws_partition=self.hook.conn_partition,
-                **awslogs,
+                **awslogs[0],
             )
 
         self.hook.check_job_success(self.job_id)
         self.log.info("AWS Batch job (%s) succeeded", self.job_id)
 
 
 class BatchCreateComputeEnvironmentOperator(BaseOperator):
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,32 +15,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import re
 import sys
-import warnings
 from datetime import timedelta
 from typing import TYPE_CHECKING, Sequence
 
 import boto3
 
 from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator, XCom
 from airflow.providers.amazon.aws.exceptions import EcsOperatorError, EcsTaskFailToStart
-
-# TODO: Remove the following import when EcsProtocol and EcsTaskLogFetcher deprecations are removed.
-from airflow.providers.amazon.aws.hooks import ecs
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.hooks.ecs import (
     EcsClusterStates,
     EcsHook,
     EcsTaskDefinitionStates,
+    EcsTaskLogFetcher,
     should_retry_eni,
 )
 from airflow.utils.helpers import prune_dict
 from airflow.utils.session import provide_session
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -384,14 +381,18 @@
         is already running. If so, the operator will attach to it instead of starting a new task.
         This is to avoid relaunching a new task when the connection drops between Airflow and ECS while
         the task is running (when the Airflow worker is restarted for example).
     :param number_logs_exception: Number of lines from the last Cloudwatch logs to return in the
         AirflowException if an ECS task is stopped (to receive Airflow alerts with the logs of what
         failed in the code running in ECS).
     :param wait_for_completion: If True, waits for creation of the cluster to complete. (default: True)
+    :param waiter_delay: The amount of time in seconds to wait between attempts,
+        if not set then the default waiter value will be used.
+    :param waiter_max_attempts: The maximum number of attempts to be made,
+        if not set then the default waiter value will be used.
     """
 
     ui_color = "#f0ede4"
     template_fields: Sequence[str] = (
         "task_definition",
         "cluster",
         "overrides",
@@ -439,14 +440,16 @@
         awslogs_stream_prefix: str | None = None,
         awslogs_fetch_interval: timedelta = timedelta(seconds=30),
         propagate_tags: str | None = None,
         quota_retry: dict | None = None,
         reattach: bool = False,
         number_logs_exception: int = 10,
         wait_for_completion: bool = True,
+        waiter_delay: int | None = None,
+        waiter_max_attempts: int | None = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.task_definition = task_definition
         self.cluster = cluster
         self.overrides = overrides
@@ -470,14 +473,16 @@
         if self.awslogs_region is None:
             self.awslogs_region = self.region
 
         self.arn: str | None = None
         self.retry_args = quota_retry
         self.task_log_fetcher: EcsTaskLogFetcher | None = None
         self.wait_for_completion = wait_for_completion
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
 
     @provide_session
     def execute(self, context, session=None):
         self.log.info(
             "Running ECS Task - Task definition: %s - on cluster %s", self.task_definition, self.cluster
         )
         self.log.info("EcsOperator overrides: %s", self.overrides)
@@ -592,28 +597,36 @@
 
     def _wait_for_task_ended(self) -> None:
         if not self.client or not self.arn:
             return
 
         waiter = self.client.get_waiter("tasks_stopped")
         waiter.config.max_attempts = sys.maxsize  # timeout is managed by airflow
-        waiter.wait(cluster=self.cluster, tasks=[self.arn])
+        waiter.wait(
+            cluster=self.cluster,
+            tasks=[self.arn],
+            WaiterConfig=prune_dict(
+                {
+                    "Delay": self.waiter_delay,
+                    "MaxAttempts": self.waiter_max_attempts,
+                }
+            ),
+        )
 
         return
 
     def _aws_logs_enabled(self):
         return self.awslogs_group and self.awslogs_stream_prefix
 
-    # TODO: When the deprecation wrapper below is removed, please fix the following return type hint.
-    def _get_task_log_fetcher(self) -> ecs.EcsTaskLogFetcher:
+    def _get_task_log_fetcher(self) -> EcsTaskLogFetcher:
         if not self.awslogs_group:
             raise ValueError("must specify awslogs_group to fetch task logs")
         log_stream_name = f"{self.awslogs_stream_prefix}/{self.ecs_task_id}"
 
-        return ecs.EcsTaskLogFetcher(
+        return EcsTaskLogFetcher(
             aws_conn_id=self.aws_conn_id,
             region_name=self.awslogs_region,
             log_group=self.awslogs_group,
             log_stream_name=log_stream_name,
             fetch_interval=self.awslogs_fetch_interval,
             logger=self.log,
         )
@@ -675,57 +688,7 @@
         if self.task_log_fetcher:
             self.task_log_fetcher.stop()
 
         response = self.client.stop_task(
             cluster=self.cluster, task=self.arn, reason="Task killed by the user"
         )
         self.log.info(response)
-
-
-class EcsOperator(EcsRunTaskOperator):
-    """
-    This operator is deprecated.
-    Please use :class:`airflow.providers.amazon.aws.operators.ecs.EcsRunTaskOperator`.
-    """
-
-    def __init__(self, *args, **kwargs):
-        warnings.warn(
-            "This operator is deprecated. "
-            "Please use `airflow.providers.amazon.aws.operators.ecs.EcsRunTaskOperator`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        super().__init__(*args, **kwargs)
-
-
-class EcsTaskLogFetcher(ecs.EcsTaskLogFetcher):
-    """
-    This class is deprecated.
-    Please use :class:`airflow.providers.amazon.aws.hooks.ecs.EcsTaskLogFetcher`.
-    """
-
-    # TODO: Note to deprecator, Be sure to fix the use of `ecs.EcsTaskLogFetcher`
-    #       in the Operators above when you remove this wrapper class.
-    def __init__(self, *args, **kwargs):
-        warnings.warn(
-            "This class is deprecated. "
-            "Please use `airflow.providers.amazon.aws.hooks.ecs.EcsTaskLogFetcher`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        super().__init__(*args, **kwargs)
-
-
-class EcsProtocol(ecs.EcsProtocol):
-    """
-    This class is deprecated.
-    Please use :class:`airflow.providers.amazon.aws.hooks.ecs.EcsProtocol`.
-    """
-
-    # TODO: Note to deprecator, Be sure to fix the use of `ecs.EcsProtocol`
-    #       in the Operators above when you remove this wrapper class.
-    def __init__(self):
-        warnings.warn(
-            "This class is deprecated.  Please use `airflow.providers.amazon.aws.hooks.ecs.EcsProtocol`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/eks.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,15 +640,14 @@
     :param cluster_name: The name of the Amazon EKS Cluster to execute the task on. (templated)
     :param cluster_role_arn: The Amazon Resource Name (ARN) of the IAM role that provides permissions
          for the Kubernetes control plane to make calls to AWS API operations on your behalf. (templated)
     :param in_cluster: If True, look for config inside the cluster; if False look for a local file path.
     :param namespace: The namespace in which to execute the pod. (templated)
     :param pod_name: The unique name to give the pod. (templated)
     :param aws_profile: The named profile containing the credentials for the AWS CLI tool to use.
-    :param aws_profile: str
     :param region: Which AWS region the connection should use. (templated)
          If this is None or empty then the default boto3 behaviour is used.
     :param aws_conn_id: The Airflow connection used for AWS credentials. (templated)
          If this is None or empty then the default boto3 behaviour is used. If
          running Airflow in a distributed manner and aws_conn_id is None or
          empty, then the default boto3 configuration would be used (and must be
          maintained on each worker node).
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/emr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1006,40 +1006,40 @@
                 action="run",
                 countdown=self.waiter_countdown,
                 check_interval_seconds=self.waiter_check_interval_seconds,
             )
         return response["jobRunId"]
 
 
-class EmrServerlessDeleteApplicationOperator(BaseOperator):
+class EmrServerlessStopApplicationOperator(BaseOperator):
     """
-    Operator to delete EMR Serverless application
+    Operator to stop an EMR Serverless application
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
-        :ref:`howto/operator:EmrServerlessDeleteApplicationOperator`
+        :ref:`howto/operator:EmrServerlessStopApplicationOperator`
 
-    :param application_id: ID of the EMR Serverless application to delete.
-    :param wait_for_completion: If true, wait for the Application to start before returning. Default to True
+    :param application_id: ID of the EMR Serverless application to stop.
+    :param wait_for_completion: If true, wait for the Application to stop before returning. Default to True
     :param aws_conn_id: AWS connection to use
     :param waiter_countdown: Total amount of time, in seconds, the operator will wait for
-        the application be deleted. Defaults to 25 minutes.
+        the application be stopped. Defaults to 5 minutes.
     :param waiter_check_interval_seconds: Number of seconds between polling the state of the application.
-        Defaults to 60 seconds.
+        Defaults to 30 seconds.
     """
 
     template_fields: Sequence[str] = ("application_id",)
 
     def __init__(
         self,
         application_id: str,
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
-        waiter_countdown: int = 25 * 60,
-        waiter_check_interval_seconds: int = 60,
+        waiter_countdown: int = 5 * 60,
+        waiter_check_interval_seconds: int = 30,
         **kwargs,
     ):
         self.aws_conn_id = aws_conn_id
         self.application_id = application_id
         self.wait_for_completion = wait_for_completion
         self.waiter_countdown = waiter_countdown
         self.waiter_check_interval_seconds = waiter_check_interval_seconds
@@ -1050,36 +1050,84 @@
         """Create and return an EmrServerlessHook."""
         return EmrServerlessHook(aws_conn_id=self.aws_conn_id)
 
     def execute(self, context: Context) -> None:
         self.log.info("Stopping application: %s", self.application_id)
         self.hook.conn.stop_application(applicationId=self.application_id)
 
-        # This should be replaced with a boto waiter when available.
-        waiter(
-            get_state_callable=self.hook.conn.get_application,
-            get_state_args={
-                "applicationId": self.application_id,
-            },
-            parse_response=["application", "state"],
-            desired_state=EmrServerlessHook.APPLICATION_FAILURE_STATES,
-            failure_states=set(),
-            object_type="application",
-            action="stopped",
-            countdown=self.waiter_countdown,
-            check_interval_seconds=self.waiter_check_interval_seconds,
+        if self.wait_for_completion:
+            # This should be replaced with a boto waiter when available.
+            waiter(
+                get_state_callable=self.hook.conn.get_application,
+                get_state_args={
+                    "applicationId": self.application_id,
+                },
+                parse_response=["application", "state"],
+                desired_state=EmrServerlessHook.APPLICATION_FAILURE_STATES,
+                failure_states=set(),
+                object_type="application",
+                action="stopped",
+                countdown=self.waiter_countdown,
+                check_interval_seconds=self.waiter_check_interval_seconds,
+            )
+            self.log.info("EMR serverless application %s stopped successfully", self.application_id)
+
+
+class EmrServerlessDeleteApplicationOperator(EmrServerlessStopApplicationOperator):
+    """
+    Operator to delete EMR Serverless application
+
+    .. seealso::
+        For more information on how to use this operator, take a look at the guide:
+        :ref:`howto/operator:EmrServerlessDeleteApplicationOperator`
+
+    :param application_id: ID of the EMR Serverless application to delete.
+    :param wait_for_completion: If true, wait for the Application to be deleted before returning.
+        Defaults to True. Note that this operator will always wait for the application to be STOPPED first.
+    :param aws_conn_id: AWS connection to use
+    :param waiter_countdown: Total amount of time, in seconds, the operator will wait for each step of first,
+        the application to be stopped, and then deleted. Defaults to 25 minutes.
+    :param waiter_check_interval_seconds: Number of seconds between polling the state of the application.
+        Defaults to 60 seconds.
+    """
+
+    template_fields: Sequence[str] = ("application_id",)
+
+    def __init__(
+        self,
+        application_id: str,
+        wait_for_completion: bool = True,
+        aws_conn_id: str = "aws_default",
+        waiter_countdown: int = 25 * 60,
+        waiter_check_interval_seconds: int = 60,
+        **kwargs,
+    ):
+        self.wait_for_delete_completion = wait_for_completion
+        # super stops the app
+        super().__init__(
+            application_id=application_id,
+            # when deleting an app, we always need to wait for it to stop before we can call delete()
+            wait_for_completion=True,
+            aws_conn_id=aws_conn_id,
+            waiter_countdown=waiter_countdown,
+            waiter_check_interval_seconds=waiter_check_interval_seconds,
+            **kwargs,
         )
 
-        self.log.info("Deleting application: %s", self.application_id)
+    def execute(self, context: Context) -> None:
+        # super stops the app (or makes sure it's already stopped)
+        super().execute(context)
+
+        self.log.info("Now deleting application: %s", self.application_id)
         response = self.hook.conn.delete_application(applicationId=self.application_id)
 
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"Application deletion failed: {response}")
 
-        if self.wait_for_completion:
+        if self.wait_for_delete_completion:
             # This should be replaced with a boto waiter when available.
             waiter(
                 get_state_callable=self.hook.conn.get_application,
                 get_state_args={"applicationId": self.application_id},
                 parse_response=["application", "state"],
                 desired_state={"TERMINATED"},
                 failure_states=EmrServerlessHook.APPLICATION_FAILURE_STATES,
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
-import warnings
 from typing import TYPE_CHECKING, Sequence
 
 from airflow.compat.functools import cached_property
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.lambda_function import LambdaHook
 
 if TYPE_CHECKING:
@@ -191,25 +190,7 @@
         if "FunctionError" in response:
             raise ValueError(
                 "Lambda function execution resulted in error",
                 {"ResponseMetadata": response.get("ResponseMetadata"), "Payload": payload},
             )
         self.log.info("Lambda function invocation succeeded: %r", response.get("ResponseMetadata"))
         return payload
-
-
-class AwsLambdaInvokeFunctionOperator(LambdaInvokeFunctionOperator):
-    """
-    This class is deprecated.
-    Please use
-    :class:`airflow.providers.amazon.aws.operators.lambda_function.LambdaInvokeFunctionOperator`.
-    """
-
-    def __init__(self, *args, **kwargs):
-        warnings.warn(
-            "This class is deprecated."
-            "Please use"
-            "`airflow.providers.amazon.aws.operators.lambda_function.LambdaInvokeFunctionOperator`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        super().__init__(*args, **kwargs)
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-import warnings
 from typing import TYPE_CHECKING
 
 from airflow.compat.functools import cached_property
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.redshift_data import RedshiftDataHook
 
 if TYPE_CHECKING:
@@ -79,36 +78,26 @@
         statement_name: str | None = None,
         with_event: bool = False,
         wait_for_completion: bool = True,
         poll_interval: int = 10,
         return_sql_result: bool = False,
         aws_conn_id: str = "aws_default",
         region: str | None = None,
-        await_result: bool | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.database = database
         self.sql = sql
         self.cluster_identifier = cluster_identifier
         self.db_user = db_user
         self.parameters = parameters
         self.secret_arn = secret_arn
         self.statement_name = statement_name
         self.with_event = with_event
-        self.await_result = await_result
         self.wait_for_completion = wait_for_completion
-        if await_result:
-            warnings.warn(
-                f"Parameter `{self.__class__.__name__}.await_result` is deprecated and will be removed "
-                "in a future release. Please use method `wait_for_completion` instead.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-            self.wait_for_completion = await_result
         if poll_interval > 0:
             self.poll_interval = poll_interval
         else:
             self.log.warning(
                 "Invalid poll_interval:",
                 poll_interval,
             )
@@ -118,65 +107,14 @@
         self.statement_id: str | None = None
 
     @cached_property
     def hook(self) -> RedshiftDataHook:
         """Create and return an RedshiftDataHook."""
         return RedshiftDataHook(aws_conn_id=self.aws_conn_id, region_name=self.region)
 
-    def execute_query(self) -> str:
-        warnings.warn(
-            "This method is deprecated and has been moved to the hook "
-            "`airflow.providers.amazon.aws.hooks.redshift_data.RedshiftDataHook`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self.statement_id = self.hook.execute_query(
-            database=self.database,
-            sql=self.sql,
-            cluster_identifier=self.cluster_identifier,
-            db_user=self.db_user,
-            parameters=self.parameters,
-            secret_arn=self.secret_arn,
-            statement_name=self.statement_name,
-            with_event=self.with_event,
-            wait_for_completion=self.wait_for_completion,
-            poll_interval=self.poll_interval,
-        )
-        return self.statement_id
-
-    def execute_batch_query(self) -> str:
-        warnings.warn(
-            "This method is deprecated and has been moved to the hook "
-            "`airflow.providers.amazon.aws.hooks.redshift_data.RedshiftDataHook`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self.statement_id = self.hook.execute_query(
-            database=self.database,
-            sql=self.sql,
-            cluster_identifier=self.cluster_identifier,
-            db_user=self.db_user,
-            parameters=self.parameters,
-            secret_arn=self.secret_arn,
-            statement_name=self.statement_name,
-            with_event=self.with_event,
-            wait_for_completion=self.wait_for_completion,
-            poll_interval=self.poll_interval,
-        )
-        return self.statement_id
-
-    def wait_for_results(self, statement_id: str):
-        warnings.warn(
-            "This method is deprecated and has been moved to the hook "
-            "`airflow.providers.amazon.aws.hooks.redshift_data.RedshiftDataHook`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.hook.wait_for_results(statement_id=statement_id, poll_interval=self.poll_interval)
-
     def execute(self, context: Context) -> GetStatementResultResponseTypeDef | str:
         """Execute a statement against Amazon Redshift"""
         self.log.info("Executing statement: %s", self.sql)
 
         self.statement_id = self.hook.execute_query(
             database=self.database,
             sql=self.sql,
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -263,31 +263,14 @@
             if self.are_secret_values_urlencoded:
                 standardized_secret_dict = self._remove_escaping_in_secret_dict(standardized_secret_dict)
             standardized_secret = json.dumps(standardized_secret_dict)
             return standardized_secret
         else:
             return secret
 
-    def get_conn_uri(self, conn_id: str) -> str | None:
-        """
-        Return URI representation of Connection conn_id.
-
-        As of Airflow version 2.3.0 this method is deprecated.
-
-        :param conn_id: the connection id
-        :return: deserialized Connection
-        """
-        warnings.warn(
-            f"Method `{self.__class__.__name__}.get_conn_uri` is deprecated and will be removed "
-            "in a future release. Please use method `get_conn_value` instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.get_conn_value(conn_id)
-
     def get_variable(self, key: str) -> str | None:
         """
         Get Airflow Variable
         :param key: Variable Key
         :return: Variable Value
         """
         if self.variables_prefix is None:
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Objects relating to sourcing connections from AWS SSM Parameter Store"""
 from __future__ import annotations
 
 import re
-import warnings
 
 from airflow.compat.functools import cached_property
 from airflow.providers.amazon.aws.utils import trim_none_values
 from airflow.secrets import BaseSecretsBackend
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 
@@ -139,34 +138,14 @@
         :param conn_id: connection id
         """
         if self.connections_prefix is None:
             return None
 
         return self._get_secret(self.connections_prefix, conn_id, self.connections_lookup_pattern)
 
-    def get_conn_uri(self, conn_id: str) -> str | None:
-        """
-        Return URI representation of Connection conn_id.
-
-        As of Airflow version 2.3.0 this method is deprecated.
-
-        :param conn_id: the connection id
-        """
-        warnings.warn(
-            f"Method `{self.__class__.__name__}.get_conn_uri` is deprecated and will be removed "
-            "in a future release. Please use method `get_conn_value` instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        value = self.get_conn_value(conn_id)
-        if value is None:
-            return None
-
-        return self.deserialize_connection(conn_id, value).get_uri()
-
     def get_variable(self, key: str) -> str | None:
         """
         Get Airflow Variable
 
         :param key: Variable Key
         :return: Variable Value
         """
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from deprecated import deprecated
 
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.emr import EmrContainerHook, EmrHook, EmrServerlessHook
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.amazon.aws.links.emr import EmrLogsLink
-from airflow.sensors.base import BaseSensorOperator, poke_mode_only
+from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 from airflow.compat.functools import cached_property
 
 
@@ -447,15 +447,14 @@
             return (
                 f"for code: {state_change_reason.get('Code', 'No code')} "
                 f"with message {state_change_reason.get('Message', 'Unknown')}"
             )
         return None
 
 
-@poke_mode_only
 class EmrStepSensor(EmrBaseSensor):
     """
     Asks for the state of the step until it reaches any of the target states.
     If it fails the sensor errors, failing the task.
 
     With the default target states, sensor waits step to be completed.
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -13,91 +12,117 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-from enum import Enum
-from typing import TYPE_CHECKING, Any, Sequence
+from tempfile import NamedTemporaryFile
+from typing import TYPE_CHECKING, Callable, Iterable, Sequence
 
 from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
-from airflow.providers.amazon.aws.hooks.glacier import GlacierHook
-from airflow.sensors.base import BaseSensorOperator
+from airflow.hooks.base import BaseHook
+from airflow.models import BaseOperator
+from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
-class JobStatus(Enum):
-    """Glacier jobs description"""
+class S3ToSqlOperator(BaseOperator):
+    """
+        Loads Data from S3 into a SQL Database.
+        You need to provide a parser function that takes a filename as an input
+        and returns an iterable of rows
 
-    IN_PROGRESS = "InProgress"
-    SUCCEEDED = "Succeeded"
+    .. seealso::
+        For more information on how to use this operator, take a look at the guide:
+        :ref:`howto/operator:S3ToSqlOperator`
 
+    :param schema: reference to a specific schema in SQL database
+    :param table: reference to a specific table in SQL database
+    :param s3_bucket: reference to a specific S3 bucket
+    :param s3_key: reference to a specific S3 key
+    :param sql_conn_id: reference to a specific SQL database. Must be of type DBApiHook
+    :param aws_conn_id: reference to a specific S3 / AWS connection
+    :param column_list: list of column names to use in the insert SQL.
+    :param commit_every: The maximum number of rows to insert in one
+        transaction. Set to `0` to insert all rows in one transaction.
+    :param parser: parser function that takes a filepath as input and returns an iterable.
+        e.g. to use a CSV parser that yields rows line-by-line, pass the following
+        function:
 
-class GlacierJobOperationSensor(BaseSensorOperator):
-    """
-    Glacier sensor for checking job state. This operator runs only in reschedule mode.
+        def parse_csv(filepath):
+            import csv
 
-    .. seealso::
-        For more information on how to use this sensor, take a look at the guide:
-        :ref:`howto/sensor:GlacierJobOperationSensor`
+            with open(filepath, newline="") as file:
+                yield from csv.reader(file)
 
-    :param aws_conn_id: The reference to the AWS connection details
-    :param vault_name: name of Glacier vault on which job is executed
-    :param job_id: the job ID was returned by retrieve_inventory()
-    :param poke_interval: Time in seconds that the job should wait in
-        between each tries
-    :param mode: How the sensor operates.
-        Options are: ``{ poke | reschedule }``, default is ``poke``.
-        When set to ``poke`` the sensor is taking up a worker slot for its
-        whole execution time and sleeps between pokes. Use this mode if the
-        expected runtime of the sensor is short or if a short poke interval
-        is required. Note that the sensor will hold onto a worker slot and
-        a pool slot for the duration of the sensor's runtime in this mode.
-        When set to ``reschedule`` the sensor task frees the worker slot when
-        the criteria is not yet met and it's rescheduled at a later time. Use
-        this mode if the time before the criteria is met is expected to be
-        quite long. The poke interval should be more than one minute to
-        prevent too much load on the scheduler.
     """
 
-    template_fields: Sequence[str] = ("vault_name", "job_id")
+    template_fields: Sequence[str] = (
+        "s3_bucket",
+        "s3_key",
+        "schema",
+        "table",
+        "column_list",
+        "sql_conn_id",
+    )
+    template_ext: Sequence[str] = ()
+    ui_color = "#f4a460"
 
     def __init__(
         self,
         *,
+        s3_key: str,
+        s3_bucket: str,
+        table: str,
+        parser: Callable[[str], Iterable[Iterable]],
+        column_list: list[str] | None = None,
+        commit_every: int = 1000,
+        schema: str | None = None,
+        sql_conn_id: str = "sql_default",
         aws_conn_id: str = "aws_default",
-        vault_name: str,
-        job_id: str,
-        poke_interval: int = 60 * 20,
-        mode: str = "reschedule",
-        **kwargs: Any,
+        **kwargs,
     ) -> None:
         super().__init__(**kwargs)
+        self.s3_bucket = s3_bucket
+        self.s3_key = s3_key
+        self.table = table
+        self.schema = schema
         self.aws_conn_id = aws_conn_id
-        self.vault_name = vault_name
-        self.job_id = job_id
-        self.poke_interval = poke_interval
-        self.mode = mode
+        self.sql_conn_id = sql_conn_id
+        self.column_list = column_list
+        self.commit_every = commit_every
+        self.parser = parser
+
+    def execute(self, context: Context) -> None:
+
+        self.log.info("Loading %s to SQL table %s...", self.s3_key, self.table)
+
+        s3_hook = S3Hook(aws_conn_id=self.aws_conn_id)
+        s3_obj = s3_hook.get_key(key=self.s3_key, bucket_name=self.s3_bucket)
+
+        with NamedTemporaryFile() as local_tempfile:
+
+            s3_obj.download_fileobj(local_tempfile)
+            local_tempfile.flush()
+            local_tempfile.seek(0)
+
+            self.db_hook.insert_rows(
+                table=self.table,
+                schema=self.schema,
+                target_fields=self.column_list,
+                rows=self.parser(local_tempfile.name),
+                commit_every=self.commit_every,
+            )
 
     @cached_property
-    def hook(self):
-        return GlacierHook(aws_conn_id=self.aws_conn_id)
-
-    def poke(self, context: Context) -> bool:
-        response = self.hook.describe_job(vault_name=self.vault_name, job_id=self.job_id)
-
-        if response["StatusCode"] == JobStatus.SUCCEEDED.value:
-            self.log.info("Job status: %s, code status: %s", response["Action"], response["StatusCode"])
-            self.log.info("Job finished successfully")
-            return True
-        elif response["StatusCode"] == JobStatus.IN_PROGRESS.value:
-            self.log.info("Processing...")
-            self.log.warning("Code status: %s", response["StatusCode"])
-            return False
-        else:
+    def db_hook(self):
+        self.log.debug("Get connection for %s", self.sql_conn_id)
+        hook = BaseHook.get_hook(self.sql_conn_id)
+        if not callable(getattr(hook, "insert_rows", None)):
             raise AirflowException(
-                f'Sensor failed. Job status: {response["Action"]}, code status: {response["StatusCode"]}'
+                "This hook is not supported. The hook class must have an `insert_rows` method."
             )
+        return hook
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Google Cloud Storage to S3 operator."""
 from __future__ import annotations
 
 import os
-import warnings
 from typing import TYPE_CHECKING, Sequence
 
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.google.cloud.hooks.gcs import GCSHook
 
 if TYPE_CHECKING:
@@ -41,19 +40,14 @@
     :param bucket: The Google Cloud Storage bucket to find the objects. (templated)
     :param prefix: Prefix string which filters objects whose name begin with
         this prefix. (templated)
     :param delimiter: The delimiter by which you want to filter the objects. (templated)
         For e.g to lists the CSV files from in a directory in GCS you would use
         delimiter='.csv'.
     :param gcp_conn_id: (Optional) The connection ID used to connect to Google Cloud.
-    :param google_cloud_storage_conn_id: (Deprecated) The connection ID used to connect to Google Cloud.
-        This parameter has been deprecated. You should pass the gcp_conn_id parameter instead.
-    :param delegate_to: Google account to impersonate using domain-wide delegation of authority,
-        if any. For this to work, the service account making the request must have
-        domain-wide delegation enabled.
     :param dest_aws_conn_id: The destination S3 connection
     :param dest_s3_key: The base S3 key to be used to store the files. (templated)
     :param dest_verify: Whether or not to verify SSL certificates for S3 connection.
         By default SSL certificates are verified.
         You can provide the following values:
 
         - ``False``: do not validate SSL certificates. SSL will still be used
@@ -96,56 +90,43 @@
     def __init__(
         self,
         *,
         bucket: str,
         prefix: str | None = None,
         delimiter: str | None = None,
         gcp_conn_id: str = "google_cloud_default",
-        google_cloud_storage_conn_id: str | None = None,
-        delegate_to: str | None = None,
         dest_aws_conn_id: str = "aws_default",
         dest_s3_key: str,
         dest_verify: str | bool | None = None,
         replace: bool = False,
         google_impersonation_chain: str | Sequence[str] | None = None,
         dest_s3_extra_args: dict | None = None,
         s3_acl_policy: str | None = None,
         keep_directory_structure: bool = True,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
 
-        if google_cloud_storage_conn_id:
-            warnings.warn(
-                "The google_cloud_storage_conn_id parameter has been deprecated. You should pass "
-                "the gcp_conn_id parameter.",
-                DeprecationWarning,
-                stacklevel=3,
-            )
-            gcp_conn_id = google_cloud_storage_conn_id
-
         self.bucket = bucket
         self.prefix = prefix
         self.delimiter = delimiter
         self.gcp_conn_id = gcp_conn_id
-        self.delegate_to = delegate_to
         self.dest_aws_conn_id = dest_aws_conn_id
         self.dest_s3_key = dest_s3_key
         self.dest_verify = dest_verify
         self.replace = replace
         self.google_impersonation_chain = google_impersonation_chain
         self.dest_s3_extra_args = dest_s3_extra_args or {}
         self.s3_acl_policy = s3_acl_policy
         self.keep_directory_structure = keep_directory_structure
 
     def execute(self, context: Context) -> list[str]:
         # list all files in an Google Cloud Storage bucket
         hook = GCSHook(
             gcp_conn_id=self.gcp_conn_id,
-            delegate_to=self.delegate_to,
             impersonation_chain=self.google_impersonation_chain,
         )
 
         self.log.info(
             "Getting list of the files. Bucket: %s; Delimiter: %s; Prefix: %s",
             self.bucket,
             self.delimiter,
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,18 +43,15 @@
     :param aws_conn_id: The reference to the AWS connection details
     :param gcp_conn_id: The reference to the GCP connection details
     :param vault_name: the Glacier vault on which job is executed
     :param bucket_name: the Google Cloud Storage bucket where the data will be transferred
     :param object_name: the name of the object to check in the Google cloud
         storage bucket.
     :param gzip: option to compress local file or file data for upload
-    :param chunk_size: size of chunk in bytes the that will downloaded from Glacier vault
-    :param delegate_to: The account to impersonate using domain-wide delegation of authority,
-        if any. For this to work, the service account making the request must have
-        domain-wide delegation enabled.
+    :param chunk_size: size of chunk in bytes the that will be downloaded from Glacier vault
     :param google_impersonation_chain: Optional Google service account to impersonate using
         short-term credentials, or chained list of accounts required to get the access_token
         of the last account in the list, which will be impersonated in the request.
         If set as a string, the account must grant the originating account
         the Service Account Token Creator IAM role.
         If set as a sequence, the identities from the list must grant
         Service Account Token Creator IAM role to the directly preceding identity, with first
@@ -69,34 +66,31 @@
         aws_conn_id: str = "aws_default",
         gcp_conn_id: str = "google_cloud_default",
         vault_name: str,
         bucket_name: str,
         object_name: str,
         gzip: bool,
         chunk_size: int = 1024,
-        delegate_to: str | None = None,
         google_impersonation_chain: str | Sequence[str] | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.aws_conn_id = aws_conn_id
         self.gcp_conn_id = gcp_conn_id
         self.vault_name = vault_name
         self.bucket_name = bucket_name
         self.object_name = object_name
         self.gzip = gzip
         self.chunk_size = chunk_size
-        self.delegate_to = delegate_to
         self.impersonation_chain = google_impersonation_chain
 
     def execute(self, context: Context) -> str:
         glacier_hook = GlacierHook(aws_conn_id=self.aws_conn_id)
         gcs_hook = GCSHook(
             gcp_conn_id=self.gcp_conn_id,
-            delegate_to=self.delegate_to,
             impersonation_chain=self.impersonation_chain,
         )
         job_id = glacier_hook.retrieve_inventory(vault_name=self.vault_name)
 
         with tempfile.NamedTemporaryFile() as temp_file:
             glacier_data = glacier_hook.retrieve_inventory_results(
                 vault_name=self.vault_name, job_id=job_id["jobId"]
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 """This module allows you to transfer data from any Google API endpoint into a S3 Bucket."""
 from __future__ import annotations
 
 import json
 import sys
 from typing import TYPE_CHECKING, Sequence
 
-from airflow.models import BaseOperator, TaskInstance
+from airflow.models import BaseOperator
 from airflow.models.xcom import MAX_XCOM_SIZE, XCOM_RETURN_KEY
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.google.common.hooks.discovery_api import GoogleDiscoveryApiHook
 
 if TYPE_CHECKING:
+    from airflow.models import TaskInstance
+    from airflow.serialization.pydantic.taskinstance import TaskInstancePydantic
     from airflow.utils.context import Context
 
 
 class GoogleApiToS3Operator(BaseOperator):
     """
     Basic class for transferring data from a Google API endpoint into a S3 Bucket.
 
@@ -67,21 +69,18 @@
         for pulling from xcom and updating the google api endpoint params.
     :param google_api_endpoint_params_via_xcom_task_ids: Task ids to filter xcom by.
     :param google_api_pagination: If set to True Pagination will be enabled for this request
         to retrieve all data.
 
         .. note:: This means the response will be a list of responses.
 
-    :param google_api_num_retries: Define the number of retries for the google api requests being made
+    :param google_api_num_retries: Define the number of retries for the Google API requests being made
         if it fails.
     :param s3_overwrite: Specifies whether the s3 file will be overwritten if exists.
     :param gcp_conn_id: The connection ID to use when fetching connection info.
-    :param delegate_to: Google account to impersonate using domain-wide delegation of authority,
-        if any. For this to work, the service account making the request must have
-        domain-wide delegation enabled.
     :param aws_conn_id: The connection id specifying the authentication information for the S3 Bucket.
     :param google_impersonation_chain: Optional Google service account to impersonate using
         short-term credentials, or chained list of accounts required to get the access_token
         of the last account in the list, which will be impersonated in the request.
         If set as a string, the account must grant the originating account
         the Service Account Token Creator IAM role.
         If set as a sequence, the identities from the list must grant
@@ -109,15 +108,14 @@
         google_api_response_via_xcom: str | None = None,
         google_api_endpoint_params_via_xcom: str | None = None,
         google_api_endpoint_params_via_xcom_task_ids: str | None = None,
         google_api_pagination: bool = False,
         google_api_num_retries: int = 0,
         s3_overwrite: bool = False,
         gcp_conn_id: str = "google_cloud_default",
-        delegate_to: str | None = None,
         aws_conn_id: str = "aws_default",
         google_impersonation_chain: str | Sequence[str] | None = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.google_api_service_name = google_api_service_name
         self.google_api_service_version = google_api_service_version
@@ -127,15 +125,14 @@
         self.google_api_response_via_xcom = google_api_response_via_xcom
         self.google_api_endpoint_params_via_xcom = google_api_endpoint_params_via_xcom
         self.google_api_endpoint_params_via_xcom_task_ids = google_api_endpoint_params_via_xcom_task_ids
         self.google_api_pagination = google_api_pagination
         self.google_api_num_retries = google_api_num_retries
         self.s3_overwrite = s3_overwrite
         self.gcp_conn_id = gcp_conn_id
-        self.delegate_to = delegate_to
         self.aws_conn_id = aws_conn_id
         self.google_impersonation_chain = google_impersonation_chain
 
     def execute(self, context: Context) -> None:
         """
         Transfers Google APIs json data to S3.
 
@@ -152,15 +149,14 @@
 
         if self.google_api_response_via_xcom:
             self._expose_google_api_response_via_xcom(context["task_instance"], data)
 
     def _retrieve_data_from_google_api(self) -> dict:
         google_discovery_api_hook = GoogleDiscoveryApiHook(
             gcp_conn_id=self.gcp_conn_id,
-            delegate_to=self.delegate_to,
             api_service_name=self.google_api_service_name,
             api_version=self.google_api_service_version,
             impersonation_chain=self.google_impersonation_chain,
         )
         return google_discovery_api_hook.query(
             endpoint=self.google_api_endpoint_path,
             data=self.google_api_endpoint_params,
@@ -173,21 +169,25 @@
         s3_hook.load_string(
             string_data=json.dumps(data),
             bucket_name=S3Hook.parse_s3_url(self.s3_destination_key)[0],
             key=S3Hook.parse_s3_url(self.s3_destination_key)[1],
             replace=self.s3_overwrite,
         )
 
-    def _update_google_api_endpoint_params_via_xcom(self, task_instance: TaskInstance) -> None:
+    def _update_google_api_endpoint_params_via_xcom(
+        self, task_instance: TaskInstance | TaskInstancePydantic
+    ) -> None:
 
         if self.google_api_endpoint_params_via_xcom:
             google_api_endpoint_params = task_instance.xcom_pull(
                 task_ids=self.google_api_endpoint_params_via_xcom_task_ids,
                 key=self.google_api_endpoint_params_via_xcom,
             )
             self.google_api_endpoint_params.update(google_api_endpoint_params)
 
-    def _expose_google_api_response_via_xcom(self, task_instance: TaskInstance, data: dict) -> None:
+    def _expose_google_api_response_via_xcom(
+        self, task_instance: TaskInstance | TaskInstancePydantic, data: dict
+    ) -> None:
         if sys.getsizeof(data) < MAX_XCOM_SIZE:
             task_instance.xcom_push(key=self.google_api_response_via_xcom or XCOM_RETURN_KEY, value=data)
         else:
             raise RuntimeError("The size of the downloaded data is too large to push to XCom!")
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,28 +14,23 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module allows you to transfer mail attachments from a mail server into s3 bucket."""
 from __future__ import annotations
 
-import warnings
 from typing import TYPE_CHECKING, Sequence
 
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.imap.hooks.imap import ImapHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
-_DEPRECATION_MSG = (
-    "The s3_conn_id parameter has been deprecated. You should pass instead the aws_conn_id parameter."
-)
-
 
 class ImapAttachmentToS3Operator(BaseOperator):
     """
     Transfers a mail attachment from a mail server into s3 bucket.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
@@ -62,23 +57,18 @@
         s3_bucket: str,
         s3_key: str,
         imap_check_regex: bool = False,
         imap_mail_folder: str = "INBOX",
         imap_mail_filter: str = "All",
         s3_overwrite: bool = False,
         imap_conn_id: str = "imap_default",
-        s3_conn_id: str | None = None,
         aws_conn_id: str = "aws_default",
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
-        if s3_conn_id:
-            warnings.warn(_DEPRECATION_MSG, DeprecationWarning, stacklevel=3)
-            aws_conn_id = s3_conn_id
-
         self.imap_attachment_name = imap_attachment_name
         self.s3_bucket = s3_bucket
         self.s3_key = s3_key
         self.imap_check_regex = imap_check_regex
         self.imap_mail_folder = imap_mail_folder
         self.imap_mail_filter = imap_mail_filter
         self.s3_overwrite = s3_overwrite
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,32 +14,26 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
-import warnings
 from typing import TYPE_CHECKING, Any, Iterable, Sequence, cast
 
 from bson import json_util
 
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.mongo.hooks.mongo import MongoHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
-_DEPRECATION_MSG = (
-    "The s3_conn_id parameter has been deprecated. You should pass instead the aws_conn_id parameter."
-)
-
-
 class MongoToS3Operator(BaseOperator):
     """Operator meant to move data from mongo via pymongo to s3 via boto.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:MongoToS3Operator`
 
@@ -62,33 +56,28 @@
     template_fields: Sequence[str] = ("s3_bucket", "s3_key", "mongo_query", "mongo_collection")
     ui_color = "#589636"
     template_fields_renderers = {"mongo_query": "json"}
 
     def __init__(
         self,
         *,
-        s3_conn_id: str | None = None,
         mongo_conn_id: str = "mongo_default",
         aws_conn_id: str = "aws_default",
         mongo_collection: str,
         mongo_query: list | dict,
         s3_bucket: str,
         s3_key: str,
         mongo_db: str | None = None,
         mongo_projection: list | dict | None = None,
         replace: bool = False,
         allow_disk_use: bool = False,
         compression: str | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
-        if s3_conn_id:
-            warnings.warn(_DEPRECATION_MSG, DeprecationWarning, stacklevel=3)
-            aws_conn_id = s3_conn_id
-
         self.mongo_conn_id = mongo_conn_id
         self.aws_conn_id = aws_conn_id
         self.mongo_db = mongo_db
         self.mongo_collection = mongo_collection
 
         # Grab query and determine if we need to run an aggregate pipeline
         self.mongo_query = mongo_query
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,30 +13,25 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-import warnings
 from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING, Sequence
 from urllib.parse import urlsplit
 
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.ssh.hooks.ssh import SSHHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
-_DEPRECATION_MSG = (
-    "The s3_conn_id parameter has been deprecated. You should pass instead the aws_conn_id parameter."
-)
-
 
 class S3ToSFTPOperator(BaseOperator):
     """
     This operator enables the transferring of files from S3 to a SFTP server.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
@@ -58,23 +53,18 @@
     def __init__(
         self,
         *,
         s3_bucket: str,
         s3_key: str,
         sftp_path: str,
         sftp_conn_id: str = "ssh_default",
-        s3_conn_id: str | None = None,
         aws_conn_id: str = "aws_default",
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
-        if s3_conn_id:
-            warnings.warn(_DEPRECATION_MSG, DeprecationWarning, stacklevel=3)
-            aws_conn_id = s3_conn_id
-
         self.sftp_conn_id = sftp_conn_id
         self.sftp_path = sftp_path
         self.s3_bucket = s3_bucket
         self.s3_key = s3_key
         self.aws_conn_id = aws_conn_id
 
     @staticmethod
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         - ``False``: do not validate SSL certificates. SSL will still be used
                 (unless use_ssl is False), but SSL certificates will not be verified.
         - ``path/to/cert/bundle.pem``: A filename of the CA cert bundle to uses.
                 You can specify this argument if you want to use a different
                 CA cert bundle than the one used by botocore.
     :param file_format: the destination file format, only string 'csv', 'json' or 'parquet' is accepted.
     :param pd_kwargs: arguments to include in DataFrame ``.to_parquet()``, ``.to_json()`` or ``.to_csv()``.
+    :param groupby_kwargs: argument to include in DataFrame ``groupby()``.
     """
 
     template_fields: Sequence[str] = (
         "s3_bucket",
         "s3_key",
         "query",
         "sql_conn_id",
@@ -103,26 +104,28 @@
         sql_conn_id: str,
         parameters: None | Mapping | Iterable = None,
         replace: bool = False,
         aws_conn_id: str = "aws_default",
         verify: bool | str | None = None,
         file_format: Literal["csv", "json", "parquet"] = "csv",
         pd_kwargs: dict | None = None,
+        groupby_kwargs: dict | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.query = query
         self.s3_bucket = s3_bucket
         self.s3_key = s3_key
         self.sql_conn_id = sql_conn_id
         self.aws_conn_id = aws_conn_id
         self.verify = verify
         self.replace = replace
         self.pd_kwargs = pd_kwargs or {}
         self.parameters = parameters
+        self.groupby_kwargs = groupby_kwargs or {}
 
         if "path_or_buf" in self.pd_kwargs:
             raise AirflowException("The argument path_or_buf is not allowed, please remove it")
 
         try:
             self.file_format = FILE_FORMAT[file_format.upper()]
         except KeyError:
@@ -166,23 +169,34 @@
         s3_conn = S3Hook(aws_conn_id=self.aws_conn_id, verify=self.verify)
         data_df = sql_hook.get_pandas_df(sql=self.query, parameters=self.parameters)
         self.log.info("Data from SQL obtained")
 
         self._fix_dtypes(data_df, self.file_format)
         file_options = FILE_OPTIONS_MAP[self.file_format]
 
-        with NamedTemporaryFile(mode=file_options.mode, suffix=file_options.suffix) as tmp_file:
+        for group_name, df in self._partition_dataframe(df=data_df):
+            with NamedTemporaryFile(mode=file_options.mode, suffix=file_options.suffix) as tmp_file:
 
-            self.log.info("Writing data to temp file")
-            getattr(data_df, file_options.function)(tmp_file.name, **self.pd_kwargs)
+                self.log.info("Writing data to temp file")
+                getattr(df, file_options.function)(tmp_file.name, **self.pd_kwargs)
 
-            self.log.info("Uploading data to S3")
-            s3_conn.load_file(
-                filename=tmp_file.name, key=self.s3_key, bucket_name=self.s3_bucket, replace=self.replace
-            )
+                self.log.info("Uploading data to S3")
+                object_key = f"{self.s3_key}_{group_name}" if group_name else self.s3_key
+                s3_conn.load_file(
+                    filename=tmp_file.name, key=object_key, bucket_name=self.s3_bucket, replace=self.replace
+                )
+
+    def _partition_dataframe(self, df: DataFrame) -> Iterable[tuple[str, DataFrame]]:
+        """Partition dataframe using pandas groupby() method"""
+        if not self.groupby_kwargs:
+            yield "", df
+        else:
+            grouped_df = df.groupby(**self.groupby_kwargs)
+            for group_label in grouped_df.groups.keys():
+                yield group_label, grouped_df.get_group(group_label).reset_index(drop=True)
 
     def _get_hook(self) -> DbApiHook:
         self.log.debug("Get connection for %s", self.sql_conn_id)
         conn = BaseHook.get_connection(self.sql_conn_id)
         hook = conn.get_hook()
         if not callable(getattr(hook, "get_pandas_df", None)):
             raise AirflowException(
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-amazon",
         "name": "Amazon",
         "description": "Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).\n",
         "suspended": False,
         "versions": [
+            "8.0.0",
             "7.4.1",
             "7.4.0",
             "7.3.0",
             "7.2.1",
             "7.2.0",
             "7.1.0",
             "7.0.0",
@@ -101,14 +102,15 @@
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/datasync.rst"],
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon DynamoDB",
                 "external-doc-url": "https://aws.amazon.com/dynamodb/",
                 "logo": "/integration-logos/aws/Amazon-DynamoDB_light-bg@4x.png",
+                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/dynamodb.rst"],
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon EC2",
                 "external-doc-url": "https://aws.amazon.com/ec2/",
                 "logo": "/integration-logos/aws/Amazon-EC2_light-bg@4x.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/ec2.rst"],
@@ -138,37 +140,37 @@
                 "external-doc-url": "https://aws.amazon.com/elasticache/redis//",
                 "logo": "/integration-logos/aws/Amazon-ElastiCache_light-bg@4x.png",
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon EMR",
                 "external-doc-url": "https://aws.amazon.com/emr/",
-                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/emr.rst"],
+                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/emr/emr.rst"],
                 "logo": "/integration-logos/aws/Amazon-EMR_light-bg@4x.png",
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon EMR on EKS",
                 "external-doc-url": "https://docs.aws.amazon.com/emr/latest/EMR-on-EKS-DevelopmentGuide/emr-eks.html",
-                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/emr_eks.rst"],
+                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/emr/emr_eks.rst"],
                 "logo": "/integration-logos/aws/Amazon-EMR_light-bg@4x.png",
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon EMR Serverless",
                 "external-doc-url": "https://docs.aws.amazon.com/emr/latest/EMR-Serverless-UserGuide/emr-serverless.html",
-                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/emr_serverless.rst"],
+                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/emr/emr_serverless.rst"],
                 "logo": "/integration-logos/aws/Amazon-EMR_light-bg@4x.png",
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon Glacier",
                 "external-doc-url": "https://aws.amazon.com/glacier/",
                 "logo": "/integration-logos/aws/Amazon-S3-Glacier_light-bg@4x.png",
-                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/glacier.rst"],
+                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/s3/glacier.rst"],
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon Kinesis Data Firehose",
                 "external-doc-url": "https://aws.amazon.com/kinesis/data-firehose/",
                 "logo": "/integration-logos/aws/Amazon-Kinesis-Data-Firehose_light-bg@4x.png",
                 "tags": ["aws"],
@@ -181,24 +183,26 @@
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon Redshift",
                 "external-doc-url": "https://aws.amazon.com/redshift/",
                 "logo": "/integration-logos/aws/Amazon-Redshift_light-bg@4x.png",
                 "how-to-guide": [
-                    "/docs/apache-airflow-providers-amazon/operators/redshift_sql.rst",
-                    "/docs/apache-airflow-providers-amazon/operators/redshift_cluster.rst",
+                    "/docs/apache-airflow-providers-amazon/operators/redshift/redshift_sql.rst",
+                    "/docs/apache-airflow-providers-amazon/operators/redshift/redshift_cluster.rst",
                 ],
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon Redshift Data",
                 "external-doc-url": "https://aws.amazon.com/redshift/",
                 "logo": "/integration-logos/aws/Amazon-Redshift_light-bg@4x.png",
-                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/redshift_data.rst"],
+                "how-to-guide": [
+                    "/docs/apache-airflow-providers-amazon/operators/redshift/redshift_data.rst"
+                ],
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon SageMaker",
                 "external-doc-url": "https://aws.amazon.com/sagemaker/",
                 "logo": "/integration-logos/aws/Amazon-SageMaker_light-bg@4x.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/sagemaker.rst"],
@@ -231,15 +235,15 @@
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/sqs.rst"],
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon Simple Storage Service (S3)",
                 "external-doc-url": "https://aws.amazon.com/s3/",
                 "logo": "/integration-logos/aws/Amazon-Simple-Storage-Service-S3_light-bg@4x.png",
-                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/s3.rst"],
+                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/s3/s3.rst"],
                 "tags": ["aws"],
             },
             {
                 "integration-name": "Amazon Systems Manager (SSM)",
                 "external-doc-url": "https://aws.amazon.com/systems-manager/",
                 "logo": "/integration-logos/aws/AWS-Systems-Manager_light-bg@4x.png",
                 "tags": ["aws"],
@@ -362,18 +366,15 @@
                 "python-modules": [
                     "airflow.providers.amazon.aws.operators.glue",
                     "airflow.providers.amazon.aws.operators.glue_crawler",
                 ],
             },
             {
                 "integration-name": "AWS Lambda",
-                "python-modules": [
-                    "airflow.providers.amazon.aws.operators.aws_lambda",
-                    "airflow.providers.amazon.aws.operators.lambda_function",
-                ],
+                "python-modules": ["airflow.providers.amazon.aws.operators.lambda_function"],
             },
             {
                 "integration-name": "Amazon Simple Storage Service (S3)",
                 "python-modules": ["airflow.providers.amazon.aws.operators.s3"],
             },
             {
                 "integration-name": "Amazon SageMaker",
@@ -394,15 +395,14 @@
             {
                 "integration-name": "Amazon RDS",
                 "python-modules": ["airflow.providers.amazon.aws.operators.rds"],
             },
             {
                 "integration-name": "Amazon Redshift",
                 "python-modules": [
-                    "airflow.providers.amazon.aws.operators.redshift_sql",
                     "airflow.providers.amazon.aws.operators.redshift_cluster",
                     "airflow.providers.amazon.aws.operators.redshift_data",
                 ],
             },
             {
                 "integration-name": "Amazon QuickSight",
                 "python-modules": ["airflow.providers.amazon.aws.operators.quicksight"],
@@ -426,14 +426,18 @@
                 "python-modules": ["airflow.providers.amazon.aws.sensors.cloud_formation"],
             },
             {
                 "integration-name": "AWS Database Migration Service",
                 "python-modules": ["airflow.providers.amazon.aws.sensors.dms"],
             },
             {
+                "integration-name": "Amazon DynamoDB",
+                "python-modules": ["airflow.providers.amazon.aws.sensors.dynamodb"],
+            },
+            {
                 "integration-name": "Amazon EC2",
                 "python-modules": ["airflow.providers.amazon.aws.sensors.ec2"],
             },
             {
                 "integration-name": "Amazon ECS",
                 "python-modules": ["airflow.providers.amazon.aws.sensors.ecs"],
             },
@@ -623,116 +627,116 @@
                 "python-modules": ["airflow.providers.amazon.aws.hooks.appflow"],
             },
         ],
         "transfers": [
             {
                 "source-integration-name": "Amazon DynamoDB",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/dynamodb_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/dynamodb_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.dynamodb_to_s3",
             },
             {
                 "source-integration-name": "Google Cloud Storage (GCS)",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/gcs_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/gcs_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.gcs_to_s3",
             },
             {
                 "source-integration-name": "Amazon Glacier",
                 "target-integration-name": "Google Cloud Storage (GCS)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/glacier_to_gcs.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/glacier_to_gcs.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.glacier_to_gcs",
             },
             {
                 "source-integration-name": "Google",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/google_api_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/google_api_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.google_api_to_s3",
             },
             {
                 "source-integration-name": "Apache Hive",
                 "target-integration-name": "Amazon DynamoDB",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/hive_to_dynamodb.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/hive_to_dynamodb.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.hive_to_dynamodb",
             },
             {
                 "source-integration-name": "Internet Message Access Protocol (IMAP)",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/imap_attachment_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/imap_attachment_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.imap_attachment_to_s3",
             },
             {
                 "source-integration-name": "MongoDB",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/mongo_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/mongo_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.mongo_to_s3",
             },
             {
                 "source-integration-name": "Amazon Redshift",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/redshift_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/redshift_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.redshift_to_s3",
             },
             {
                 "source-integration-name": "Amazon Simple Storage Service (S3)",
                 "target-integration-name": "Amazon Redshift",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/s3_to_redshift.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/s3_to_redshift.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.s3_to_redshift",
             },
             {
                 "source-integration-name": "Amazon Simple Storage Service (S3)",
                 "target-integration-name": "SSH File Transfer Protocol (SFTP)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/s3_to_sftp.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/s3_to_sftp.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.s3_to_sftp",
             },
             {
                 "source-integration-name": "SSH File Transfer Protocol (SFTP)",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/sftp_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/sftp_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.sftp_to_s3",
             },
             {
                 "source-integration-name": "Amazon Simple Storage Service (S3)",
                 "target-integration-name": "File Transfer Protocol (FTP)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/s3_to_ftp.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/s3_to_ftp.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.s3_to_ftp",
             },
             {
                 "source-integration-name": "Exasol",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
                 "python-module": "airflow.providers.amazon.aws.transfers.exasol_to_s3",
             },
             {
                 "source-integration-name": "File Transfer Protocol (FTP)",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/ftp_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/ftp_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.ftp_to_s3",
             },
             {
                 "source-integration-name": "Salesforce",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/salesforce_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/salesforce_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.salesforce_to_s3",
             },
             {
                 "source-integration-name": "Local",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/local_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/local_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.local_to_s3",
             },
             {
                 "source-integration-name": "Common SQL",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/sql_to_s3.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/sql_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.sql_to_s3",
             },
             {
                 "source-integration-name": "Amazon Simple Storage Service (S3)",
                 "target-integration-name": "Common SQL",
-                "how-to-guide": "/docs/apache-airflow-providers-amazon/operators/transfer/s3_to_sql.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/s3_to_sql.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.s3_to_sql",
             },
             {
                 "source-integration-name": "Amazon Web Services",
                 "target-integration-name": "Amazon Web Services",
                 "python-module": "airflow.providers.amazon.aws.transfers.base",
             },
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-8.0.0rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,7 @@
-Metadata-Version: 2.1
-Name: apache-airflow-providers-amazon
-Version: 7.4.1rc1
-Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
-Home-page: https://airflow.apache.org/
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Author: Apache Software Foundation
-Author-email: dev@airflow.apache.org
-License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/
-Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Source Code, https://github.com/apache/airflow
-Project-URL: Slack Chat, https://s.apache.org/airflow-slack
-Project-URL: Twitter, https://twitter.com/ApacheAirflow
-Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Framework :: Apache Airflow
-Classifier: Framework :: Apache Airflow :: Provider
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: apache.hive
-Provides-Extra: cncf.kubernetes
-Provides-Extra: common.sql
-Provides-Extra: exasol
-Provides-Extra: ftp
-Provides-Extra: google
-Provides-Extra: imap
-Provides-Extra: mongo
-Provides-Extra: salesforce
-Provides-Extra: ssh
-Provides-Extra: pandas
-Provides-Extra: aiobotocore
-License-File: LICENSE
-License-File: NOTICE
-
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
@@ -60,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``7.4.1rc1``
+Release: ``8.0.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -158,14 +113,84 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+8.0.0
+......
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  In this version of the provider, deprecated GCS hook's parameter ``delegate_to`` is removed from the following operators: ``GCSToS3Operator``, ``GlacierToGCSOperator`` and ``GoogleApiToS3Operator``.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+  Removed deprecated parameter ``google_cloud_storage_conn_id`` from ``GCSToS3Operator``, ``gcp_conn_id`` should be used instead.
+
+  Removed deprecated parameter ``max_tries`` from the Athena & EMR hook & operators in favor of ``max_polling_attempts``.
+
+  Disabled deprecated behavior of switching to an empty aws connection ID on error. You can set it to None explicitly.
+
+  Removed deprecated method ``waiter`` from emr hook in favor of the more generic ``airflow.providers.amazon.aws.utils.waiter.waiter``
+
+  Removed deprecated unused parameter ``cluster_identifier`` from Redshift Cluster's hook method ``get_cluster_snapshot_status``
+
+  Removed deprecated method ``find_processing_job_by_name`` from Sagemaker hook, use ``count_processing_jobs_by_name`` instead.
+
+  Removed deprecated module ``airflow.providers.amazon.aws.operators.aws_lambda`` in favor of ``airflow.providers.amazon.aws.operators.lambda_function``
+
+  Removed EcsOperator in favor of EcsRunTaskOperator.
+  EcsTaskLogFetcher and EcsProtocol should be imported from the hook.
+
+  Removed AwsLambdaInvokeFunctionOperator in favor of LambdaInvokeFunctionOperator.
+
+  Removed deprecated param ``await_result`` from RedshiftDataOperator in favor of ``wait_for_completion``.
+  Some methods from this operator should be imported from the hook instead.
+
+  Removed deprecated ``RedshiftSQLOperator`` in favor of the generic ``SQLExecuteQueryOperator``.
+  The parameter that was passed as ``redshift_conn_id`` needs to be changed to ``conn_id``, and the behavior should stay the same.
+
+  Removed deprecated method ``get_conn_uri`` from secrets manager in favor of ``get_conn_value``
+  Also removed deprecated method ``get_conn_uri`` from systems manager. ``deserialize_connection(...).get_uri()`` should be used instead.
+
+  Removed deprecated and unused param ``s3_conn_id`` from ``ImapAttachmentToS3Operator``, ``MongoToS3Operator`` and ``S3ToSFTPOperator``.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+* ``Remove deprecated code from Amazon provider (#30755)``
+
+Features
+~~~~~~~~
+
+* ``add a stop operator to emr serverless (#30720)``
+* ``SqlToS3Operator - Add feature to partition SQL table (#30460)``
+* ``New AWS sensor — DynamoDBValueSensor (#28338)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fixed logging issue (#30703)``
+* ``DynamoDBHook - waiter_path() to consider 'resource_type' or 'client_type' (#30595)``
+* ``Add ability to override waiter delay in EcsRunTaskOperator (#30586)``
+* ``Add support in AWS Batch Operator for multinode jobs (#29522)``
+* ``AWS logs. Exit fast when 3 consecutive responses are returned from AWS Cloudwatch logs (#30756)``
+
+Misc
+~~~~
+
+* ``Remove @poke_mode_only from EmrStepSensor (#30774)``
+* ``Organize Amazon providers docs index (#30541)``
+* ``Remove duplicate param docstring in EksPodOperator (#30634)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+
 7.4.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fix 'RedshiftResumeClusterOperator' deferrable implementation (#30370)``
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 airflow/providers/amazon/aws/links/logs.py
 airflow/providers/amazon/aws/log/__init__.py
 airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
 airflow/providers/amazon/aws/log/s3_task_handler.py
 airflow/providers/amazon/aws/operators/__init__.py
 airflow/providers/amazon/aws/operators/appflow.py
 airflow/providers/amazon/aws/operators/athena.py
-airflow/providers/amazon/aws/operators/aws_lambda.py
 airflow/providers/amazon/aws/operators/batch.py
 airflow/providers/amazon/aws/operators/cloud_formation.py
 airflow/providers/amazon/aws/operators/datasync.py
 airflow/providers/amazon/aws/operators/dms.py
 airflow/providers/amazon/aws/operators/ec2.py
 airflow/providers/amazon/aws/operators/ecs.py
 airflow/providers/amazon/aws/operators/eks.py
@@ -72,28 +71,28 @@
 airflow/providers/amazon/aws/operators/glue.py
 airflow/providers/amazon/aws/operators/glue_crawler.py
 airflow/providers/amazon/aws/operators/lambda_function.py
 airflow/providers/amazon/aws/operators/quicksight.py
 airflow/providers/amazon/aws/operators/rds.py
 airflow/providers/amazon/aws/operators/redshift_cluster.py
 airflow/providers/amazon/aws/operators/redshift_data.py
-airflow/providers/amazon/aws/operators/redshift_sql.py
 airflow/providers/amazon/aws/operators/s3.py
 airflow/providers/amazon/aws/operators/sagemaker.py
 airflow/providers/amazon/aws/operators/sns.py
 airflow/providers/amazon/aws/operators/sqs.py
 airflow/providers/amazon/aws/operators/step_function.py
 airflow/providers/amazon/aws/secrets/__init__.py
 airflow/providers/amazon/aws/secrets/secrets_manager.py
 airflow/providers/amazon/aws/secrets/systems_manager.py
 airflow/providers/amazon/aws/sensors/__init__.py
 airflow/providers/amazon/aws/sensors/athena.py
 airflow/providers/amazon/aws/sensors/batch.py
 airflow/providers/amazon/aws/sensors/cloud_formation.py
 airflow/providers/amazon/aws/sensors/dms.py
+airflow/providers/amazon/aws/sensors/dynamodb.py
 airflow/providers/amazon/aws/sensors/ec2.py
 airflow/providers/amazon/aws/sensors/ecs.py
 airflow/providers/amazon/aws/sensors/eks.py
 airflow/providers/amazon/aws/sensors/emr.py
 airflow/providers/amazon/aws/sensors/glacier.py
 airflow/providers/amazon/aws/sensors/glue.py
 airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/pyproject.toml` & `apache-airflow-providers-amazon-8.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/setup.cfg` & `apache-airflow-providers-amazon-8.0.0rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-amazon-7.4.1rc1/setup.py` & `apache-airflow-providers-amazon-8.0.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-amazon package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "7.4.1"
+version = "8.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-amazon setup."""
     setup(
         version=version,
         extras_require={
```

