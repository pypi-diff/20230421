# Comparing `tmp/chatgpt4-cli-1.5.1.tar.gz` & `tmp/chatgpt4-cli-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.5.1.tar", last modified: Wed Apr 19 13:16:25 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.5.2.tar", last modified: Fri Apr 21 07:05:03 2023, max compression
```

## Comparing `chatgpt4-cli-1.5.1.tar` & `chatgpt4-cli-1.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:25.770380 chatgpt4-cli-1.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:25.770380 chatgpt4-cli-1.5.1/GPTCLI/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/emage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31039 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/gptcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-19 13:16:25.770380 chatgpt4-cli-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:25.770380 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:16:25.770380 chatgpt4-cli-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:05:03.425552 chatgpt4-cli-1.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:05:03.425552 chatgpt4-cli-1.5.2/GPTCLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/emage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31397 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/gptcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-04-21 07:05:03.425552 chatgpt4-cli-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:05:03.425552 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 07:05:03.425552 chatgpt4-cli-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/setup.py
```

### Comparing `chatgpt4-cli-1.5.1/GPTCLI/__init__.py` & `chatgpt4-cli-1.5.2/GPTCLI/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-__version__ = "1.5.1"
+__version__ = "1.5.2"
 __author__ = "Smartwa Caleb"
 __repo__ = "https://github.com/Simatwa/gpt-cli"
 
 import logging
 
 logging.basicConfig(
-    format="%(levelname)s - %(message)s - (%(asctime)s) ",#[%(module)s,%(lineno)s]",
+    format="%(levelname)s - %(message)s - (%(asctime)s) ",  # [%(module)s,%(lineno)s]",
     datefmt="%d-%b-%Y %H:%M:%S",
     level=logging.INFO,
 )
 
 getExc = lambda e: e.args[1] if isinstance(e.args, list) else str(e)
```

### Comparing `chatgpt4-cli-1.5.1/GPTCLI/addons.py` & `chatgpt4-cli-1.5.2/GPTCLI/addons.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.1/GPTCLI/bard.py` & `chatgpt4-cli-1.5.2/GPTCLI/bard.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from Bard import Chatbot
-from . import logging, error_handler
+from . import logging, error_handler,getExc
 from sys import exit
 from os import environ
 from json import load
 from time import sleep
 
 
 class Bard:
     def __init__(self, args: object):
         self.args = args
         self.session = environ.get("BARD_SESSION") or self.__get_sess()
-        self.active_link = Chatbot(self.session)
+        try:
+            self.active_link = Chatbot(self.session)
+        except Exception as e:
+            exit(logging.critical(getExc(e)))
 
     @error_handler(exit)
     def __get_sess(self):
         """Gets Bard's session"""
         if any([self.args.bkey, self.args.bkey_path, self.args.bcookie_file]):
             if self.args.bkey:
                 resp = self.args.bkey
```

### Comparing `chatgpt4-cli-1.5.1/GPTCLI/emage.py` & `chatgpt4-cli-1.5.2/GPTCLI/emage.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.1/GPTCLI/gptcli.py` & `chatgpt4-cli-1.5.2/GPTCLI/gptcli.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,15 @@
 from datetime import datetime
 from os import system, remove, path, environ, makedirs
 from threading import Thread as thr
 from appdirs import AppDirs
 from rich.markdown import Markdown
 from .addons import file_parser, system_control
 from .bard import Bard
+from time import sleep
 
 app_dir = AppDirs(
     "smartwa",
     "gpt-cli",
 ).user_data_dir
 
 first_time_run = False
@@ -564,15 +565,16 @@
     )
     prompt = time_now_format(prompt_disp)
     config_handler = config_handler()
     color_dict = config_handler.color_dict
     bcolor_dict = config_handler.bcolor_dict
     interactive = local_interactor()
     parser = lambda self, line: file_parser(line).parse()
-    bard = Bard(args)
+    if not args.update:
+        bard = Bard(args)
 
     def apply_color(self):
         print(
             self.bcolor_dict[args.background_color] + self.color_dict[args.input_color]
         )
 
     def prompt_is_error_free(self, prompt, resp=True) -> bool:
@@ -643,48 +645,54 @@
         if not chat:
             record_keeper.main(info)
         print(self.color_dict[args.input_color])
         self.do__prompt(self.prompt_disp)
         if return_fb:
             return info
 
-    @error_handler()
+    @error_handler(False)
     def do__botchat(self, line):
         rich_print("Let the bots talk:")
 
         def get_value(msg: str, type1: object = str) -> str:
             while True:
-                val = input(f"[*] " + msg + f" >>")
+                val = input(f"[*] " + msg + " >>")
                 if val:
                     if type1 == int:
                         if val.isdigit():
                             return int(val)
                     else:
                         return val
 
         def gpt_chat(msg):
-            print("[ChatGPT]")
+            print(">>[ChatGPT]")
             return self.default(msg, return_fb=True)
 
         def bard_chat(msg):
-            print("[Bard]")
-            return self.do_bard(bard, return_fb=True, chat=True)
+            print("\n<<[Bard]")
+            return self.do_bard(msg, return_fb=True, chat=True)
 
-        gpt = get_value("Enter prompt for ChatGPT")
-        bard = get_value("Enter prompt for Bard")
+        gpt_ = get_value("Enter prompt for ChatGPT")
+        bard_ = get_value("Enter prompt for Bard")
         amount = get_value("Enter amount of chat cycles [0 - infinity]", int)
-        for x in range(amount if amount else 1000000):
-            if x == 0:
-                gpt = gpt_chat(gpt)
-                bard = bard_chat(bard)
-            else:
-                if x % 2 == 0:
-                    bard = bard_chat(gpt)
-                else:
-                    gpt = gpt_chat(bard)
+        interval = get_value("Enter sleep interval in each chat (s) - preferred 0", int)
+        gpt = gpt_chat(gpt_)
+        bard = bard_chat(bard_)
+        while amount if amount else True:
+            args.message = gpt
+            record_keeper.main(bard)
+            gpt = gpt_chat(bard)
+            bard = bard_chat(gpt)
+            if interval:
+                sleep_duration = 0
+                print()
+                while sleep_duration != interval:
+                    sleep_duration += 1
+                    print(f">[{interval}]<{sleep_duration}", end="\r")
+                    sleep(1)
 
     def do_txt2img(self, line):
         """Generate images based on GPT description"""
         line = self.parser(line)
         if not line:
             self.do__prompt(self.prompt_disp)
             return
@@ -957,13 +965,13 @@
                 run.do_bard(prompt)
             else:
                 run.default(prompt)
         run.cmdloop()
     except (KeyboardInterrupt, EOFError):
         exit(logging.info("Stopping program"))
     except Exception as e:
-        logging.exception(e)
+        # logging.exception(e)
         logging.error(getExc(e))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chatgpt4-cli-1.5.1/GPTCLI/helper.py` & `chatgpt4-cli-1.5.2/GPTCLI/helper.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.1/GPTCLI/image.py` & `chatgpt4-cli-1.5.2/GPTCLI/image.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.1/LICENSE` & `chatgpt4-cli-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.1/PKG-INFO` & `chatgpt4-cli-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.1
+Version: 1.5.2
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,24 +24,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.9&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.2&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
-CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com). 
+CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com).
 > Generate images with Bing and ChatGPT's DALL-E model.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
 ## [Independencies](requirements.txt)
 
 * [Openai](https://github.com/openai/openai-python)
@@ -49,28 +49,28 @@
 * [Colorama](https://github.com/tartley/colorama)
 * [revChatGPT](https://github.com/acheong08/ChatGPT)
 
 ### Features
 
 - Chat with ChatGPT and Bard conversationally.
 - Let **ChatGPT** and **Bard** chat to each other.
-- Generate Images - Based on your prompt or GPT generated description.
+- Generate Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated description.
 - Stream or Non-stream responses.
 - Maintain record of the chats.
 - Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily.
 - Fully customizable Commandline Interface.
 - Interact with system commands on the fly.
 
 ### Prerequisites
 
 - [x] [OPENAI_API_KEY](https://platform.openai.com/account/api-keys)
 
 - [x] [Bard Cookies](https://bard.google.com)
 
-- [x] [Bing cookies](https://bing.com)
+- [x] [Bing cookies](https://bing.com) - *optional*
 
 ## Installation
 
 Either of the following ways will get you ready.
 
 1. Using pip
 - From pypi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.1 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.2 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
@@ -19,42 +19,43 @@
 bard.google.com). > Generate images with Bing and ChatGPT's DALL-E model. !
 [screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
 Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
 github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
 [Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
 github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
 conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
-Images - Based on your prompt or GPT generated description. - Stream or Non-
-stream responses. - Maintain record of the chats. - Parse [awesome-chatgpt-
-prompts](https://github.com/f/awesome-chatgpt-prompts) easily. - Fully
-customizable Commandline Interface. - Interact with system commands on the fly.
-### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
-api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
-(https://bing.com) ## Installation Either of the following ways will get you
-ready. 1. Using pip - From pypi ```sh $ sudo pip install chatgpt4-cli ``` -
-Installing from source ```sh $ sudo pip install git+https://github.com/Simatwa/
-gpt-cli.git ``` 2. Cloning locally and install ```sh $ git clone https://
-github.com/Simatwa/gpt-cli.git $ cd gpt-cli $ sudo python3 setup.py install #or
-$ python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
-variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
-or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
-prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
-OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
-For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
-vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
-f/awesome-chatgpt-prompts) can be parsed to the script through the following
-ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
-Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
-cli --dump show` to view the act,prompt and their **indexes** You can as well
-generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
-uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
-``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
-learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
-environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
-or `$gpt-cli-emage -h`. ## Highlight
+Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated
+description. - Stream or Non-stream responses. - Maintain record of the chats.
+- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
+easily. - Fully customizable Commandline Interface. - Interact with system
+commands on the fly. ### Prerequisites - [x] [OPENAI_API_KEY](https://
+platform.openai.com/account/api-keys) - [x] [Bard Cookies](https://
+bard.google.com) - [x] [Bing cookies](https://bing.com) - *optional* ##
+Installation Either of the following ways will get you ready. 1. Using pip -
+From pypi ```sh $ sudo pip install chatgpt4-cli ``` - Installing from source
+```sh $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git ``` 2.
+Cloning locally and install ```sh $ git clone https://github.com/Simatwa/gpt-
+cli.git $ cd gpt-cli $ sudo python3 setup.py install #or $ python3 setup.py
+install ``` ## Usage - Make OPENAI_API_KEY an environment variable. `$ export
+OPENAI_API_KEY=` After that you can launch the script with or without a prompt
+> For instance : ```sh #Without a prompt $ gpt-cli # With a prompt $ gpt-cli
+Write a conversation between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as
+one of the arguments Run `$ gpt-cli -k  ` at the terminal. > For instance :
+```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using
+NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-
+prompts) can be parsed to the script through the following ways: - Specifying
+the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the
+index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
+act,prompt and their **indexes** You can as well generate images using EdgeGPT
+(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
+1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
+github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
+cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
+image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
+Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
```

### Comparing `chatgpt4-cli-1.5.1/README.md` & `chatgpt4-cli-1.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.9&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.2&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
-CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com). 
+CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com).
 > Generate images with Bing and ChatGPT's DALL-E model.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
 ## [Independencies](requirements.txt)
 
 * [Openai](https://github.com/openai/openai-python)
@@ -22,28 +22,28 @@
 * [Colorama](https://github.com/tartley/colorama)
 * [revChatGPT](https://github.com/acheong08/ChatGPT)
 
 ### Features
 
 - Chat with ChatGPT and Bard conversationally.
 - Let **ChatGPT** and **Bard** chat to each other.
-- Generate Images - Based on your prompt or GPT generated description.
+- Generate Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated description.
 - Stream or Non-stream responses.
 - Maintain record of the chats.
 - Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily.
 - Fully customizable Commandline Interface.
 - Interact with system commands on the fly.
 
 ### Prerequisites
 
 - [x] [OPENAI_API_KEY](https://platform.openai.com/account/api-keys)
 
 - [x] [Bard Cookies](https://bard.google.com)
 
-- [x] [Bing cookies](https://bing.com)
+- [x] [Bing cookies](https://bing.com) - *optional*
 
 ## Installation
 
 Either of the following ways will get you ready.
 
 1. Using pip
 - From pypi
```

#### html2text {}

```diff
@@ -5,42 +5,43 @@
 bard.google.com). > Generate images with Bing and ChatGPT's DALL-E model. !
 [screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
 Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
 github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
 [Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
 github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
 conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
-Images - Based on your prompt or GPT generated description. - Stream or Non-
-stream responses. - Maintain record of the chats. - Parse [awesome-chatgpt-
-prompts](https://github.com/f/awesome-chatgpt-prompts) easily. - Fully
-customizable Commandline Interface. - Interact with system commands on the fly.
-### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
-api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
-(https://bing.com) ## Installation Either of the following ways will get you
-ready. 1. Using pip - From pypi ```sh $ sudo pip install chatgpt4-cli ``` -
-Installing from source ```sh $ sudo pip install git+https://github.com/Simatwa/
-gpt-cli.git ``` 2. Cloning locally and install ```sh $ git clone https://
-github.com/Simatwa/gpt-cli.git $ cd gpt-cli $ sudo python3 setup.py install #or
-$ python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
-variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
-or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
-prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
-OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
-For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
-vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
-f/awesome-chatgpt-prompts) can be parsed to the script through the following
-ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
-Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
-cli --dump show` to view the act,prompt and their **indexes** You can as well
-generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
-uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
-``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
-learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
-environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
-or `$gpt-cli-emage -h`. ## Highlight
+Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated
+description. - Stream or Non-stream responses. - Maintain record of the chats.
+- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
+easily. - Fully customizable Commandline Interface. - Interact with system
+commands on the fly. ### Prerequisites - [x] [OPENAI_API_KEY](https://
+platform.openai.com/account/api-keys) - [x] [Bard Cookies](https://
+bard.google.com) - [x] [Bing cookies](https://bing.com) - *optional* ##
+Installation Either of the following ways will get you ready. 1. Using pip -
+From pypi ```sh $ sudo pip install chatgpt4-cli ``` - Installing from source
+```sh $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git ``` 2.
+Cloning locally and install ```sh $ git clone https://github.com/Simatwa/gpt-
+cli.git $ cd gpt-cli $ sudo python3 setup.py install #or $ python3 setup.py
+install ``` ## Usage - Make OPENAI_API_KEY an environment variable. `$ export
+OPENAI_API_KEY=` After that you can launch the script with or without a prompt
+> For instance : ```sh #Without a prompt $ gpt-cli # With a prompt $ gpt-cli
+Write a conversation between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as
+one of the arguments Run `$ gpt-cli -k  ` at the terminal. > For instance :
+```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using
+NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-
+prompts) can be parsed to the script through the following ways: - Specifying
+the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the
+index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
+act,prompt and their **indexes** You can as well generate images using EdgeGPT
+(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
+1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
+github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
+cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
+image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
+Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
```

### Comparing `chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.1
+Version: 1.5.2
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,24 +24,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.9&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.2&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
-CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com). 
+CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com).
 > Generate images with Bing and ChatGPT's DALL-E model.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
 ## [Independencies](requirements.txt)
 
 * [Openai](https://github.com/openai/openai-python)
@@ -49,28 +49,28 @@
 * [Colorama](https://github.com/tartley/colorama)
 * [revChatGPT](https://github.com/acheong08/ChatGPT)
 
 ### Features
 
 - Chat with ChatGPT and Bard conversationally.
 - Let **ChatGPT** and **Bard** chat to each other.
-- Generate Images - Based on your prompt or GPT generated description.
+- Generate Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated description.
 - Stream or Non-stream responses.
 - Maintain record of the chats.
 - Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily.
 - Fully customizable Commandline Interface.
 - Interact with system commands on the fly.
 
 ### Prerequisites
 
 - [x] [OPENAI_API_KEY](https://platform.openai.com/account/api-keys)
 
 - [x] [Bard Cookies](https://bard.google.com)
 
-- [x] [Bing cookies](https://bing.com)
+- [x] [Bing cookies](https://bing.com) - *optional*
 
 ## Installation
 
 Either of the following ways will get you ready.
 
 1. Using pip
 - From pypi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.1 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.2 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
@@ -19,42 +19,43 @@
 bard.google.com). > Generate images with Bing and ChatGPT's DALL-E model. !
 [screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
 Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
 github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
 [Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
 github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
 conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
-Images - Based on your prompt or GPT generated description. - Stream or Non-
-stream responses. - Maintain record of the chats. - Parse [awesome-chatgpt-
-prompts](https://github.com/f/awesome-chatgpt-prompts) easily. - Fully
-customizable Commandline Interface. - Interact with system commands on the fly.
-### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
-api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
-(https://bing.com) ## Installation Either of the following ways will get you
-ready. 1. Using pip - From pypi ```sh $ sudo pip install chatgpt4-cli ``` -
-Installing from source ```sh $ sudo pip install git+https://github.com/Simatwa/
-gpt-cli.git ``` 2. Cloning locally and install ```sh $ git clone https://
-github.com/Simatwa/gpt-cli.git $ cd gpt-cli $ sudo python3 setup.py install #or
-$ python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
-variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
-or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
-prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
-OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
-For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
-vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
-f/awesome-chatgpt-prompts) can be parsed to the script through the following
-ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
-Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
-cli --dump show` to view the act,prompt and their **indexes** You can as well
-generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
-uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
-``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
-learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
-environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
-or `$gpt-cli-emage -h`. ## Highlight
+Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated
+description. - Stream or Non-stream responses. - Maintain record of the chats.
+- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
+easily. - Fully customizable Commandline Interface. - Interact with system
+commands on the fly. ### Prerequisites - [x] [OPENAI_API_KEY](https://
+platform.openai.com/account/api-keys) - [x] [Bard Cookies](https://
+bard.google.com) - [x] [Bing cookies](https://bing.com) - *optional* ##
+Installation Either of the following ways will get you ready. 1. Using pip -
+From pypi ```sh $ sudo pip install chatgpt4-cli ``` - Installing from source
+```sh $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git ``` 2.
+Cloning locally and install ```sh $ git clone https://github.com/Simatwa/gpt-
+cli.git $ cd gpt-cli $ sudo python3 setup.py install #or $ python3 setup.py
+install ``` ## Usage - Make OPENAI_API_KEY an environment variable. `$ export
+OPENAI_API_KEY=` After that you can launch the script with or without a prompt
+> For instance : ```sh #Without a prompt $ gpt-cli # With a prompt $ gpt-cli
+Write a conversation between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as
+one of the arguments Run `$ gpt-cli -k  ` at the terminal. > For instance :
+```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using
+NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-
+prompts) can be parsed to the script through the following ways: - Specifying
+the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the
+index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
+act,prompt and their **indexes** You can as well generate images using EdgeGPT
+(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
+1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
+github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
+cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
+image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
+Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
```

### Comparing `chatgpt4-cli-1.5.1/setup.py` & `chatgpt4-cli-1.5.2/setup.py`

 * *Files identical despite different names*

