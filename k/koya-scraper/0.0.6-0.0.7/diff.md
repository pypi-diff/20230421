# Comparing `tmp/koya_scraper-0.0.6-py2.py3-none-any.whl.zip` & `tmp/koya_scraper-0.0.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4658 bytes, number of entries: 7
+Zip file size: 4628 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       28 b- defN 23-Jan-26 20:08 koya_scraper/__init__.py
--rw-r--r--  2.0 unx    11667 b- defN 23-Feb-23 00:50 koya_scraper/koya_scraper.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 00:55 koya_scraper-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      270 b- defN 23-Feb-23 00:55 koya_scraper-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-23 00:55 koya_scraper-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Feb-23 00:55 koya_scraper-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      573 b- defN 23-Feb-23 00:55 koya_scraper-0.0.6.dist-info/RECORD
-7 files, 12661 bytes uncompressed, 3632 bytes compressed:  71.3%
+-rw-r--r--  2.0 unx    11441 b- defN 23-Apr-21 03:03 koya_scraper/koya_scraper.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 03:04 koya_scraper-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      270 b- defN 23-Apr-21 03:04 koya_scraper-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-21 03:04 koya_scraper-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-21 03:04 koya_scraper-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      573 b- defN 23-Apr-21 03:04 koya_scraper-0.0.7.dist-info/RECORD
+7 files, 12435 bytes uncompressed, 3602 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: koya_scraper/__init__.py
 Comment: 
 
 Filename: koya_scraper/koya_scraper.py
 Comment: 
 
-Filename: koya_scraper-0.0.6.dist-info/LICENSE
+Filename: koya_scraper-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: koya_scraper-0.0.6.dist-info/METADATA
+Filename: koya_scraper-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: koya_scraper-0.0.6.dist-info/WHEEL
+Filename: koya_scraper-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: koya_scraper-0.0.6.dist-info/top_level.txt
+Filename: koya_scraper-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: koya_scraper-0.0.6.dist-info/RECORD
+Filename: koya_scraper-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## koya_scraper/koya_scraper.py

```diff
@@ -3,23 +3,24 @@
 import sys
 import boto3
 import pandas as pd
 
 from scrapy.crawler import CrawlerProcess
 from scrapy.utils.project import get_project_settings
 
-from koya_aws import get_file_from_s3, config_aws_env, create_bucket
+# from koya_aws import config_aws_env, create_bucket
 from koya_utilities import send_email_to
 
 import socket
 import platform
 import psutil
 import subprocess
 import sqlalchemy
 import json
+import awswrangler as wr
 
 def get_engine(host='koya-internal.cr4gqvnvc2y8.us-east-1.rds.amazonaws.com', port='3306', db_user=None, db_password=None):
     
     if db_user is None or db_password is None:
         db_user = os.getenv('KOYA_DB_SCRAPER_LOGS_USER')
         db_password = os.getenv('KOYA_DB_SCRAPER_LOGS_PASSWORD')
     return sqlalchemy.create_engine(f'mysql+pymysql://{db_user}:{db_password}@{host}')
@@ -263,21 +264,18 @@
                           , email_to=email_to)
 
         return 1
 
 
     if return_data:
         try:
-            aws_session = config_aws_env(profile_name=profile_name)
-            koya_s3_obj = get_file_from_s3(client_project_name=client_project_name
-                                       ,session=aws_session
-                                       ,input_file_path=stage+'/ingestion/data/'
-                                       ,aws_filename=filename)
-        
-            data = pd.read_csv(koya_s3_obj['Body'])
+
+            file_path = f"s3://{client_project_name}/{stage}/ingestion/data/"+filename
+            print(f"reading: {file_path}")
+            data = wr.s3.read_csv(path=file_path)
             return data
         except Exception as e:
             print(str(e))
             if send_email:
                 send_email_to(body=f'error on scraper for \n client_project_name: {client_project_name} \n scrape_project_name: {scrape_project_name} \n error: {str(e)}'
                               , project_name=scrape_project_name
                               , subject=f'error on scraper for client_project_name {client_project_name} and scrape_project_name {scrape_project_name}'
```

## Comparing `koya_scraper-0.0.6.dist-info/RECORD` & `koya_scraper-0.0.7.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 koya_scraper/__init__.py,sha256=-cHVaaFc5xS_xDRg0jfT0La_7CCWj_eJuNpM6BU-AHI,28
-koya_scraper/koya_scraper.py,sha256=9xHg5O5TLmkMMBjg1vSoxMmZ3ExvuJEMXz5V1Q1faF0,11667
-koya_scraper-0.0.6.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-koya_scraper-0.0.6.dist-info/METADATA,sha256=jtNFudn73VEroi8YL-1aRZugz3luJzD1BW4WEc7Cf7k,270
-koya_scraper-0.0.6.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-koya_scraper-0.0.6.dist-info/top_level.txt,sha256=Q2LMJ7yQq7V7XSzX6f31GN5WjW_eghMuSMv3U4O1Q1A,13
-koya_scraper-0.0.6.dist-info/RECORD,,
+koya_scraper/koya_scraper.py,sha256=tffrfy6E6MagRnPfrEldqQncT5ygwlYw8HyYK_T5OoU,11441
+koya_scraper-0.0.7.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+koya_scraper-0.0.7.dist-info/METADATA,sha256=9wmPPW5PSVsZQOymrgM-bQJV6mTAnkxqqjpYXMURMzM,270
+koya_scraper-0.0.7.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+koya_scraper-0.0.7.dist-info/top_level.txt,sha256=Q2LMJ7yQq7V7XSzX6f31GN5WjW_eghMuSMv3U4O1Q1A,13
+koya_scraper-0.0.7.dist-info/RECORD,,
```

