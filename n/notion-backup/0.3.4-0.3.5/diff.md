# Comparing `tmp/notion_backup-0.3.4.tar.gz` & `tmp/notion_backup-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion_backup-0.3.4.tar", max compression
+gzip compressed data, was "notion_backup-0.3.5.tar", max compression
```

## Comparing `notion_backup-0.3.4.tar` & `notion_backup-0.3.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      523 2022-12-27 18:28:30.869399 notion_backup-0.3.4/README.md
--rw-r--r--   0        0        0     4647 2022-12-27 23:51:19.315271 notion_backup-0.3.4/notion_backup/backup_service.py
--rw-r--r--   0        0        0     1299 2022-12-27 22:59:19.457798 notion_backup-0.3.4/notion_backup/configuration_service.py
--rw-r--r--   0        0        0     2520 2022-12-27 23:51:19.315456 notion_backup-0.3.4/notion_backup/notion_client.py
--rw-r--r--   0        0        0      592 2022-12-27 23:53:36.504782 notion_backup-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 notion_backup-0.3.4/setup.py
--rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 notion_backup-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      523 2022-12-27 18:28:30.869399 notion_backup-0.3.5/README.md
+-rw-r--r--   0        0        0     4758 2023-04-21 19:39:18.234743 notion_backup-0.3.5/notion_backup/backup_service.py
+-rw-r--r--   0        0        0     1299 2022-12-27 22:59:19.457798 notion_backup-0.3.5/notion_backup/configuration_service.py
+-rw-r--r--   0        0        0     2782 2023-04-21 19:39:18.235103 notion_backup-0.3.5/notion_backup/notion_client.py
+-rw-r--r--   0        0        0      592 2023-04-21 19:39:18.235330 notion_backup-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 notion_backup-0.3.5/setup.py
+-rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 notion_backup-0.3.5/PKG-INFO
```

### Comparing `notion_backup-0.3.4/README.md` & `notion_backup-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `notion_backup-0.3.4/notion_backup/backup_service.py` & `notion_backup-0.3.5/notion_backup/backup_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class BackupService:
     def __init__(self, output_dir_path, space_id):
         self.output_dir_path = output_dir_path
         self.space_id = space_id
         if not self.output_dir_path.exists():
-            raise Exception(f'Output directory {self.output_dir_path.resolve()} does not exit')
+            raise Exception(f"Output directory {self.output_dir_path.resolve()} does not exit")
         self.configuration_service = ConfigurationService()
         self.notion_client = NotionClient(self.configuration_service)
 
     def _login(self):
         email = self.configuration_service.get_key("email")
         if email:
             email = prompt("Email address: ", default=email)
@@ -36,17 +36,19 @@
         print(f"A one temporary password has been sent to your email address {email}")
         otp = prompt("Temporary password: ")
 
         token = self.notion_client.get_token(csrf_values, otp)
         self.configuration_service.write_key("token", token)
         print("Congratulations, you have been successfully authenticated")
 
-    def _download_file(self, url, export_file):
-        with requests.get(url, stream=True, allow_redirects=True) as response:
-            total_size = int(response.headers.get("content-length", 0))
+    def _download_file(self, url, export_file, file_token):
+        with requests.get(
+            url, stream=True, allow_redirects=True, cookies={"file_token": file_token}
+        ) as response:
+            total_size = int(response.headers.get("Content-Length", 0))
             tqdm_bar = tqdm(total=total_size, unit="iB", unit_scale=True)
             with export_file.open("wb") as export_file_handle:
                 for data in response.iter_content(block_size):
                     tqdm_bar.update(len(data))
                     export_file_handle.write(data)
             tqdm_bar.close()
 
@@ -55,34 +57,34 @@
         if not token:
             print("First time login")
             self._login()
 
         try:
             self.notion_client.get_user_content()
         except requests.exceptions.HTTPError as err:
-            if err.response.status_code==401:
+            if err.response.status_code == 401:
                 print("Credentials have expired, login again")
                 self._login()
 
         user_content = self.notion_client.get_user_content()
 
         user_id = list(user_content["notion_user"].keys())[0]
         print(f"User id: {user_id}")
 
         spaces = [
             (space_id, space_details["value"]["name"])
             for (space_id, space_details) in user_content["space"].items()
         ]
         print("Available spaces:")
-        for (space_id, space_name) in spaces:
+        for space_id, space_name in spaces:
             print(f"\t- {space_name}: {space_id}")
 
         if self.space_id:
             print(f"Selecting space {self.space_id}")
-            space_id=self.space_id
+            space_id = self.space_id
         else:
             space_id = self.configuration_service.get_key("space_id")
             space_id = prompt("Select space id: ", default=(space_id or spaces[0][0]))
 
         if space_id not in map(itemgetter(0), spaces):
             raise Exception("Selected space id not in list")
 
@@ -90,35 +92,34 @@
 
         print("Launching export task")
         task_id = self.notion_client.launch_export_task(space_id)
         print(f"Export task {task_id} has been launched")
 
         while True:
             task_status = self.notion_client.get_user_task_status(task_id)
-            if 'status' in task_status and task_status["status"]["type"] == "complete":
+            if "status" in task_status and task_status["status"]["type"] == "complete":
                 break
-            print(
-                f"...Export still in progress, waiting for {STATUS_WAIT_TIME} seconds"
-            )
+            print(f"...Export still in progress, waiting for {STATUS_WAIT_TIME} seconds")
             sleep(STATUS_WAIT_TIME)
         print("Export task is finished")
 
         export_link = task_status["status"]["exportURL"]
         print(f"Downloading zip export from {export_link}")
 
         export_file_name = f'export_{space_id}_{datetime.now().strftime("%Y%m%d")}.zip'
 
-        self._download_file(export_link, self.output_dir_path / export_file_name)
+        file_token = self.notion_client.get_file_token()
+        self._download_file(export_link, self.output_dir_path / export_file_name, file_token)
 
 
 @click.command()
 @click.option("--output-dir", default=".", help="Where the zip export will be saved")
 @click.option("--space-id", help="Id of Notion workspace")
 def main(output_dir, space_id):
     output_dir_path = Path(output_dir)
     print(f"Backup Notion workspace into directory {output_dir_path.resolve()}")
     backup_service = BackupService(output_dir_path, space_id)
     backup_service.backup()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `notion_backup-0.3.4/notion_backup/configuration_service.py` & `notion_backup-0.3.5/notion_backup/configuration_service.py`

 * *Files identical despite different names*

### Comparing `notion_backup-0.3.4/notion_backup/notion_client.py` & `notion_backup-0.3.5/notion_backup/notion_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,23 @@
             f"{NOTION_API_ROOT}/loginWithEmail",
             json={"state": csrf_values["csrf_state"], "password": otp},
             cookies={"csrf": csrf_values["csrf_cookie"]},
         )
         response.raise_for_status()
         return response.cookies["token_v2"]
 
+    def get_file_token(self):
+        response = requests.request(
+            "GET",
+            f"https://www.notion.so/f/refresh",
+            cookies={"token_v2": self.configuration_service.get_key("token")},
+        )
+        response.raise_for_status()
+        return response.cookies["file_token"]
+
     def _send_post_request(self, path, body):
         response = requests.request(
             "POST",
             f"{NOTION_API_ROOT}/{path}",
             json=body,
             cookies={"token_v2": self.configuration_service.get_key("token")},
         )
@@ -65,14 +74,10 @@
                         },
                     },
                 }
             },
         )["taskId"]
 
     def get_user_task_status(self, task_id):
-        task_statuses = self._send_post_request("getTasks", {"taskIds": [task_id]})[
-            "results"
-        ]
-
-        return list(
-            filter(lambda task_status: task_status["id"] == task_id, task_statuses)
-        )[0]
+        task_statuses = self._send_post_request("getTasks", {"taskIds": [task_id]})["results"]
+
+        return list(filter(lambda task_status: task_status["id"] == task_id, task_statuses))[0]
```

### Comparing `notion_backup-0.3.4/pyproject.toml` & `notion_backup-0.3.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notion-backup"
-version = "0.3.4"
+version = "0.3.5"
 description = "Notion workspace export automation tool"
 authors = ["Ligohu <ligohu@outlook.fr>"]
 readme = "README.md"
 repository = "https://github.com/HugoLime/notion-backup"
 
 [tool.poetry.dependencies]
 python = ">=3.8.5"
```

### Comparing `notion_backup-0.3.4/setup.py` & `notion_backup-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'tqdm>=4.46.0']
 
 entry_points = \
 {'console_scripts': ['backup_notion = notion_backup.backup_service:main']}
 
 setup_kwargs = {
     'name': 'notion-backup',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'Notion workspace export automation tool',
     'long_description': "# notion-backup\n\nAutomate export of Notion workspace\n\n## Deprecation\n\nThe login system does not work anymore. Its seems to be blocked by a browser integrity check\n\n## Installation\n\n```\npip install --upgrade notion-backup\n```\n\n## Usage\n\n```\nbackup_notion --output-dir='.'\n```\n\n## How it works\n\nThe script obtains an API token by requesting a temporary password to be sent to your email address.\n\nLogin information are stored in `~/.notion_backup.conf`\n\nThe export zip is generated and downloaded to the specified directory.\n",
     'author': 'Ligohu',
     'author_email': 'ligohu@outlook.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/HugoLime/notion-backup',
```

### Comparing `notion_backup-0.3.4/PKG-INFO` & `notion_backup-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-backup
-Version: 0.3.4
+Version: 0.3.5
 Summary: Notion workspace export automation tool
 Home-page: https://github.com/HugoLime/notion-backup
 Author: Ligohu
 Author-email: ligohu@outlook.fr
 Requires-Python: >=3.8.5
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

