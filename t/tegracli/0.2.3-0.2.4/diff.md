# Comparing `tmp/tegracli-0.2.3.tar.gz` & `tmp/tegracli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tegracli-0.2.3.tar", max compression
+gzip compressed data, was "tegracli-0.2.4.tar", max compression
```

## Comparing `tegracli-0.2.3.tar` & `tegracli-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.3/LICENSE
--rw-r--r--   0        0        0     8456 2023-04-12 14:05:59.583449 tegracli-0.2.3/README.md
--rw-r--r--   0        0        0     1322 2023-04-21 13:27:30.097101 tegracli-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       65 2023-04-11 13:51:38.330956 tegracli-0.2.3/tegracli/__init__.py
--rw-r--r--   0        0        0     5448 2023-04-21 13:26:56.213016 tegracli-0.2.3/tegracli/dispatch.py
--rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.3/tegracli/group.py
--rw-r--r--   0        0        0    12773 2023-04-13 10:33:21.255171 tegracli-0.2.3/tegracli/main.py
--rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.3/tegracli/types.py
--rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.3/tegracli/utilities.py
--rw-r--r--   0        0        0     9568 2023-04-21 13:28:04.845759 tegracli-0.2.3/setup.py
--rw-r--r--   0        0        0     9430 2023-04-21 13:28:04.846476 tegracli-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.4/LICENSE
+-rw-r--r--   0        0        0     8456 2023-04-12 14:05:59.583449 tegracli-0.2.4/README.md
+-rw-r--r--   0        0        0     1322 2023-04-21 13:31:19.817693 tegracli-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-04-11 13:51:38.330956 tegracli-0.2.4/tegracli/__init__.py
+-rw-r--r--   0        0        0     5419 2023-04-21 13:31:33.705730 tegracli-0.2.4/tegracli/dispatch.py
+-rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.4/tegracli/group.py
+-rw-r--r--   0        0        0    12773 2023-04-13 10:33:21.255171 tegracli-0.2.4/tegracli/main.py
+-rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.4/tegracli/types.py
+-rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.4/tegracli/utilities.py
+-rw-r--r--   0        0        0     9568 2023-04-21 13:32:11.917433 tegracli-0.2.4/setup.py
+-rw-r--r--   0        0        0     9430 2023-04-21 13:32:11.918090 tegracli-0.2.4/PKG-INFO
```

### Comparing `tegracli-0.2.3/LICENSE` & `tegracli-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.3/README.md` & `tegracli-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.3/pyproject.toml` & `tegracli-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tegracli"
-version = "0.2.3"
+version = "0.2.4"
 description = "A research-focused Telegram CLI application"
 authors = ["Philipp Kessling <p.kessling@leibniz-hbi.de>", "Felix Münch <f.muench@lebniz-hbi.de>"]
 readme  = "README.md"
 license = "MIT"
 repository  = "https://github.com/Leibniz-HBI/tegracli"
 homepage = "https://pypi.org/project/tegracli/"
 classifiers = [
```

### Comparing `tegracli-0.2.3/tegracli/dispatch.py` & `tegracli-0.2.4/tegracli/dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Dispatch functions that request data from Telethon and MTProto."""
 import datetime
 import sys
 import time
 from functools import partial
 from io import TextIOWrapper
 from pathlib import Path
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional
 
 import telethon
 import ujson
 from loguru import logger as log
 from telethon import TelegramClient
 from telethon.errors import ChannelPrivateError, FloodWaitError, UserDeactivatedError
 
@@ -28,15 +28,15 @@
     Args:
         client: the client to use.
         params: the parameters to pass to the method.
         callback: the callback to pass data to.
     """
     try:
         async for message in client.iter_messages(wait_time=10, **params):
-            await callback(message or params)
+            await callback(message)
     except UserDeactivatedError:
         log.error("User account has been deactivated by Telegram. Stopping now.")
         sys.exit(127)
     except ChannelPrivateError:
         log.error(f"Entity {params['entity']} is private. Skipping.")
 
 
@@ -99,33 +99,34 @@
                     file.write("\n")
         except ValueError as error:
             log.error(f"No dice for {query}, because {error}")
             continue
 
 
 async def handle_message(
-    message: Union[telethon.types.Message, Dict],
+    message: Optional[telethon.types.Message],
     file: TextIOWrapper,
     injects: Optional[Dict],
 ):
     """Accept incoming messages and log them to disk.
 
     Args:
         message: incoming single message.
         file: opened file to dump the message's json into.
         injects: additional data to inject into the message.
     """
     if message is None:
         log.error("Message is None. Skipping.")
+        return
 
     m_dict = str_dict(message.to_dict())
     if injects is not None:
         for key, value in injects.items():
             m_dict[key] = value
-    # print(str(m_dict))
+
     ujson.dump(m_dict, file, ensure_ascii=True)
     file.write("\n")
 
 
 async def get_input_entity(
     client: TelegramClient, member_id: int
 ) -> Optional[telethon.types.TypeInputPeer]:
```

### Comparing `tegracli-0.2.3/tegracli/group.py` & `tegracli-0.2.4/tegracli/group.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.3/tegracli/main.py` & `tegracli-0.2.4/tegracli/main.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.3/tegracli/utilities.py` & `tegracli-0.2.4/tegracli/utilities.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.3/setup.py` & `tegracli-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'ujson>=5.4.0,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['tegracli = tegracli.main:cli']}
 
 setup_kwargs = {
     'name': 'tegracli',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'A research-focused Telegram CLI application',
     'long_description': '# tegracli\n\n![The TEGRACLI logo](https://github.com/Leibniz-HBI/tegracli/blob/trunk/tegracli.png?raw=true)\n\nA convenience wrapper around Telethon and the Telegram Client API for research purposes.\n\n# Installation Instructions\n\n`tegracli` uses Poetry and python >= 3.9 and < 4.0 for building and installing.\n\nTo install using pipx, run the following command `pipx install tegracli`.\n\n## How to get API keys\n\nIf you don\'t have API keys for Telegram, head over to [my.telegram.org](https://my.telegram.org).\nClick on [API development tools](https://my.telegram.org/apps), fill the form to create yourself an app and pluck the keys into `tegracli.conf.yml`. The session name can be arbitrary.\n\n```yaml\napi_id: 1234567\napi_hash : some12321hashthatmustbehere123\nsession_name: somesessionyo\n```\n\nThis template file is provided with the repository.\n\n# Usage\n\n`tegracli` is a terminal application to access the Telegram API for research purposes.\nIn order to retrieve messages the configuration-file from the section before must be present in the directory you start `tegracli`.\n\nThe following commands are available:\n\n## CONFIGURE\n\nOpens an interactive prompt for configuring API-access. Aks you to input your API id, API hash and session name and requests\na 2FA code from Telegram.\n\n```text\nUsage: tegracli configure [OPTIONS]\n\n  Configure tegracli.\n\nOptions:\n  --help  Show this message and exit.\n```\n\n## GET\n\nTo _get_ messages from a number of channels, use this command.\n\n```text\nUsage: tegracli get [OPTIONS] [CHANNELS]...\n\n  Get messages for the specified channels by either ID or username.\n\nOptions:\n  -l, --limit INTEGER           Number of messages to retrieve.\n  -O, --offset_date [%Y-%m-%d]  Offset retrieval to specific date in YYYY-MM-\n                                DD format.\n  -o, --offset_id INTEGER       Offset retrieval to a specific post number.\n  -m, --min_id INTEGER          Minimal post number.\n  -M, --max_id INTEGER          Maximal post number\n  -a, --add_offset INTEGER      Add an offset to the post numbers to be\n                                retrieved.\n  -f, --from_user TEXT          Only messages from this user.\n  --reverse / --forward         Should post numbers count upward or downward.\n                                Defaults to forward.\n  -r, --reply_to TEXT           Only messages replied to specific post id.\n  --help                        Show this message and exit.\n```\n\n| **parameter**       | **description**                                                                                                              |\n|---------------------|------------------------------------------------------------------------------------------------------------------------------|\n| **channels**        | a list of of either telegram usernames, channel or group URLs or user IDs.                                                   |\n| **limit**           | number of messages to retrieve, positive integer. If set to `-1` , retrieves all messages in the channel. defaults to `-1`.  |\n| **offset_date**     | specify start point of retrieval by date, retrieval direction is controlled by `reverse/forward`. Format must be YYYY-MM-DD. |\n| **offset_id**       | specify start point of retrieval by post number, retrieval direction is controlled by `reverse/forward`.                     |\n| **min_id**          | sets the minimum post number                                                                                                 |\n| **max_id**          | sets the maximum post number                                                                                                 |\n| **add_offset**      | add a offset to the post numbers to be retrieved                                                                             |\n| **from_user**       | limit messages to posts *from* a specific user                                                                               |\n| **reply_to**        | limit messages to replies *to* a specific user                                                                               |\n| **reverse/forward** | flag to indicate whether messages should be retrieved in chronological or reverse chronological order.                       |\n\n### Basic Examples\n\nTo retrieve the last fifty messages from a Telegram channel:\n\n```bash\ntegracli get --limit 50 corona_infokanal_bmg\n```\n\nTo retrieve the entire history starting with post #1 of a channel, set `limit` to `-1`.\n\n```bash\ntegracli get --reverse --limit -1 corona_infokanal_bmg\n```\nTo retrieve messages sent after January, 1st 2022:\n\n```bash\ntegracli get --offset_date 2022-01-01 corona_infokanal_bmg\n```\n\nTo retrieve message sent before January, 1st 2022:\n\n```bash\ntegracli get --reverse --offset_date 2022-01-01 corona_infokanal_bmg\n```\n## SEARCH\n\nTo _search_ messages of your chats and groups and channels you are subscribed to, use this command.\n\n```text\nUsage: tegracli search [OPTIONS] [QUERIES]...\n\n  This function searches Telegram content that is available to your account for the specified search term(s).\n\nOptions:\n  --help  Show this message and exit.\n```\n\n## HYDRATE\n\nTo rehydrate messages from the API this command accepts a file with message IDs in the format of `$channel_name/$post_number`.\nBoth input and output file are optional, if not given, `stdin` and `stdout` are used.\n\nOutput data is JSONL, one message per line.\n\n```text\nUsage: tegracli hydrate [OPTIONS] [INPUT_FILE] [OUTPUT_FILE]\n\n  Hydrate a file with messages-ids.\n\nOptions:\n  --help  Show this message and exit.\n```\n\nFor example, to rehydrate message IDs:\n\n```bash\necho test_channel/1234 | tegracli hydrate\n>> {"_":"Message","id": 1234, ... , "restriction_reason":[],"ttl_period":null}\n```\n\n## GROUP INIT and GROUP RUN\n\nIn order to support updatable  and long-running collections `tegracli` sports an *account group* feature which retrieves\nthe history of a given set of accounts and is able to retrieve updates on each of these accounts.\n\nGroups are initialized by calling `teracli group init`, where accounts to track are stated by either stating them as arguments\nor by reading in a file.\n\n### Account Group File Format\n\nAccount files are expected to follow these requirements:\n\n- UTF8 text document,\n- per line one account, given as either username, channel-URL or ID,\n- there shall be no header and  no additional columns\n\n```text\nUsage: tegracli group init [OPTIONS] NAME [ACCOUNTS]...\n\n  initialize a new account group\n\nOptions:\n  -f, --read_file PATH         read an account list from a file, one\n                               handle/id/url per line.\n  -s, --start_date [%Y-%m-%d]  Start date for the collection. Must be in YYYY-\n                               MM-DD format.\n  -l, --limit INTEGER          number of posts fo retrieve in one run\n  --help                       Show this message and exit.\n```\n\nA group is essentially a directory in your tegracli project folder which holdes\na group configuration file, a `profiles.jsonl` file which will collect all user objects returned\nby Telegram (these will be recycled to save API requests), as well as the jsonl-files containing the messages.\nThe messages-files are structured in a way that one file holds the messages of one account and is named by the\naccount\'s ID.\n\nAn exemplary project could look this:\n\n```text\ntegracli-project/\n |- tegracli.conf.yml\n |- mysession.session\n |- my_group/\n    |- tegracli_group.conf.yml\n    |- profiles.jsonl\n    |- 10000001.jsonl\n    |- 10000002.jsonl\n```\nTo run the project command your terminal to `tegracli group run my_group` to collect the latest post of the accounts you want to track.\n\n```text\nUsage: tegracli group run [OPTIONS] [GROUPS]...\n\n  load a group configuration and run the groups operations\n```\n\n## Result File Format\n\nMessages are stored in `jsonl`-files per channel or query. For channels filename is the channel\'s or user\'s id, for searches the query.\n**BEWARE:** how directories and files are structured is subject to active development and prone to changes in the near future.\n\n# Developer Installation\n\n1. Install [poetry](https://python-poetry.org/docs/#installation),\n2. Clone repository and unzip, if necessary,\n3. In the directory run `poetry install`,\n4. Run `poetry shell` to start the development virtualenv,\n5. Run `pytest` to run tests, run `pytest --run_api` to include tests against the Telegram API (**these do require a valid configuration**), coverage report can be found under `tests/coverage`.\n',
     'author': 'Philipp Kessling',
     'author_email': 'p.kessling@leibniz-hbi.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://pypi.org/project/tegracli/',
```

### Comparing `tegracli-0.2.3/PKG-INFO` & `tegracli-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tegracli
-Version: 0.2.3
+Version: 0.2.4
 Summary: A research-focused Telegram CLI application
 Home-page: https://pypi.org/project/tegracli/
 License: MIT
 Author: Philipp Kessling
 Author-email: p.kessling@leibniz-hbi.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

