# Comparing `tmp/hardwario-chester-1.8.6.tar.gz` & `tmp/hardwario-chester-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardwario-chester-1.8.6.tar", max compression
+gzip compressed data, was "hardwario-chester-1.9.0.tar", max compression
```

## Comparing `hardwario-chester-1.8.6.tar` & `hardwario-chester-1.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2022-05-04 10:34:17.486948 hardwario-chester-1.8.6/LICENSE
--rw-r--r--   0        0        0     1253 2022-05-04 10:34:17.486948 hardwario-chester-1.8.6/README.md
--rw-r--r--   0        0        0     1507 2022-05-04 10:35:00.915391 hardwario-chester-1.8.6/pyproject.toml
--rw-r--r--   0        0        0       57 2022-05-04 10:35:00.919391 hardwario-chester-1.8.6/src/hardwario/chester/__init__.py
--rw-r--r--   0        0        0      249 2022-05-04 10:34:17.486948 hardwario-chester-1.8.6/src/hardwario/chester/cli/__init__.py
--rw-r--r--   0        0        0     6814 2022-05-04 10:34:17.486948 hardwario-chester-1.8.6/src/hardwario/chester/cli/app.py
--rw-r--r--   0        0        0     2131 2022-05-04 10:34:17.486948 hardwario-chester-1.8.6/src/hardwario/chester/cli/lte.py
--rw-r--r--   0        0        0     6747 2022-05-04 10:34:17.486948 hardwario-chester-1.8.6/src/hardwario/chester/console.py
--rw-r--r--   0        0        0     9962 2022-05-04 10:34:17.486948 hardwario-chester-1.8.6/src/hardwario/chester/nrfjprog.py
--rw-r--r--   0        0        0     1706 2022-05-04 10:34:17.486948 hardwario-chester-1.8.6/src/hardwario/chester/pib.py
--rw-r--r--   0        0        0     2359 2022-05-04 10:35:01.531747 hardwario-chester-1.8.6/setup.py
--rw-r--r--   0        0        0     2552 2022-05-04 10:35:01.532201 hardwario-chester-1.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-05-17 13:16:34.378337 hardwario-chester-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1253 2022-05-17 13:16:34.378337 hardwario-chester-1.9.0/README.md
+-rw-r--r--   0        0        0     1507 2022-05-17 13:17:17.926592 hardwario-chester-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       57 2022-05-17 13:17:17.926592 hardwario-chester-1.9.0/src/hardwario/chester/__init__.py
+-rw-r--r--   0        0        0      249 2022-05-17 13:16:34.378337 hardwario-chester-1.9.0/src/hardwario/chester/cli/__init__.py
+-rw-r--r--   0        0        0     6947 2022-05-17 13:16:34.378337 hardwario-chester-1.9.0/src/hardwario/chester/cli/app.py
+-rw-r--r--   0        0        0     2131 2022-05-17 13:16:34.378337 hardwario-chester-1.9.0/src/hardwario/chester/cli/lte.py
+-rw-r--r--   0        0        0     7092 2022-05-17 13:16:34.378337 hardwario-chester-1.9.0/src/hardwario/chester/console.py
+-rw-r--r--   0        0        0     9962 2022-05-17 13:16:34.378337 hardwario-chester-1.9.0/src/hardwario/chester/nrfjprog.py
+-rw-r--r--   0        0        0     1706 2022-05-17 13:16:34.378337 hardwario-chester-1.9.0/src/hardwario/chester/pib.py
+-rw-r--r--   0        0        0     2359 2022-05-17 13:17:18.496513 hardwario-chester-1.9.0/setup.py
+-rw-r--r--   0        0        0     2552 2022-05-17 13:17:18.496931 hardwario-chester-1.9.0/PKG-INFO
```

### Comparing `hardwario-chester-1.8.6/LICENSE` & `hardwario-chester-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hardwario-chester-1.8.6/README.md` & `hardwario-chester-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hardwario-chester-1.8.6/pyproject.toml` & `hardwario-chester-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hardwario-chester"
-version = "v1.8.6"
+version = "v1.9.0"
 description = "HARDWARIO CHESTER"
 authors = ["Karel Blavka <karel.blavka@hardwario.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/hardwario/py-hardwario-chester"
 repository = "https://github.com/hardwario/py-hardwario-chester"
 classifiers = [
```

### Comparing `hardwario-chester-1.8.6/src/hardwario/chester/cli/app.py` & `hardwario-chester-1.9.0/src/hardwario/chester/cli/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,27 +59,28 @@
 
 default_history_file = os.path.expanduser("~/.chester_history")
 default_console_file = os.path.expanduser("~/.chester_console")
 
 
 @cli.command('console')
 @click.option('--reset', is_flag=True, help='Reset application firmware.')
+@click.option('--latency', type=int, help='Latency for RTT readout in ms.', show_default=True, default=50)
 @click.option('--history-file', type=click.Path(writable=True), show_default=True, default=default_history_file)
 @click.option('--console-file', type=click.File('a', 'utf-8'), show_default=True, default=default_console_file)
 @click.pass_context
-def command_console(ctx, reset, history_file, console_file):
+def command_console(ctx, reset, latency, history_file, console_file):
     '''Start interactive console for shell and logging.'''
     logger.remove(2)  # Remove stderr logger
 
     console = Console(history_file=history_file)
     with ctx.obj['prog'] as prog:
         if reset:
             prog.reset()
             prog.go()
-        console.run(prog, console_file)
+        console.run(prog, console_file, latency=latency)
 
 
 def validate_pib_param(ctx, param, value):
     # print('validate_pib_param', ctx.obj, param.name, value)
     try:
         getattr(ctx.obj['pib'], f'set_{param.name}')(value)
     except PIBException as e:
```

### Comparing `hardwario-chester-1.8.6/src/hardwario/chester/cli/lte.py` & `hardwario-chester-1.9.0/src/hardwario/chester/cli/lte.py`

 * *Files identical despite different names*

### Comparing `hardwario-chester-1.8.6/src/hardwario/chester/console.py` & `hardwario-chester-1.9.0/src/hardwario/chester/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,23 +132,25 @@
             key_bindings=bindings,
             mouse_support=True,
             full_screen=True,
             enable_page_navigation_bindings=True,
             clipboard=PyperclipClipboard()
         )
 
-    def run(self, prog: NRFJProg, console_file):
+    def run(self, prog: NRFJProg, console_file, latency=50):
         channels = prog.rtt_start()
 
         if 'Logger' not in channels:
             raise Exception('Not found RTT Logger channel')
 
         if 'Terminal' not in channels:
             raise Exception('Not found RTT Terminal channel')
 
+        rtt_read_delay = latency / 1000.0
+
         async def task_rtt_read(channel, buffer):
             while prog.rtt_is_running:
                 with logger.catch(message='task_rtt_read', reraise=True):
                     try:
                         line = prog.rtt_read(channel)
                     except NRFJProgRTTNoChannels:
                         return
@@ -158,28 +160,35 @@
                             console_file.write(getTime() + (' # ' if channel == 'Logger' else ' > '))
                             console_file.write(sline)
                             console_file.write('\n')
                         console_file.flush()
 
                         line = line.replace('\r', '')
                         buffer.set_document(Document(buffer.text + line, None), True)
-                    await asyncio.sleep(0.05)
+                    await asyncio.sleep(rtt_read_delay)
 
         console_file.write(f'{ "*" * 80 }\n')
 
         async def task_rtt_read_logger():
             await task_rtt_read('Logger', self.logger_buffer)
 
         async def task_rtt_read_terminal():
             await task_rtt_read('Terminal', self.shell_buffer)
 
         loop = get_event_loop()
         loop.create_task(task_rtt_read_logger())
         loop.create_task(task_rtt_read_terminal())
 
+        # t1 = threading.Thread(target=task_rtt_read, args=('Logger', self.logger_buffer))
+        # t2 = threading.Thread(target=task_rtt_read, args=('Terminal', self.shell_buffer))
+        # t1.daemon = True
+        # t2.daemon = True
+        # t1.start()
+        # t2.start()
+
         def accept(buff):
             line = f'{buff.text}\n'.replace('\r', '')
             # self.shell_buffer.insert_text(line)
             console_file.write(f'{getTime()} < {line}')
             text = self.shell_buffer.text + line
             self.shell_buffer.set_document(Document(text, None), True)
```

### Comparing `hardwario-chester-1.8.6/src/hardwario/chester/nrfjprog.py` & `hardwario-chester-1.9.0/src/hardwario/chester/nrfjprog.py`

 * *Files identical despite different names*

### Comparing `hardwario-chester-1.8.6/src/hardwario/chester/pib.py` & `hardwario-chester-1.9.0/src/hardwario/chester/pib.py`

 * *Files identical despite different names*

### Comparing `hardwario-chester-1.8.6/setup.py` & `hardwario-chester-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'pyperclip>=1.8.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['chester = hardwario.chester.cli:main']}
 
 setup_kwargs = {
     'name': 'hardwario-chester',
-    'version': '1.8.6',
+    'version': '1.9.0',
     'description': 'HARDWARIO CHESTER',
     'long_description': '<a href="https://www.hardwario.com/"><img src="https://www.hardwario.com/ci/assets/hw-logo.svg" width="200" alt="HARDWARIO Logo" align="right"></a>\n\n# HARDWARIO CHESTER\n\n[![Main](https://github.com/hardwario/py-hardwario-chester/actions/workflows/main.yaml/badge.svg)](https://github.com/hardwario/py-hardwario-chester/actions/workflows/main.yaml)\n[![Release](https://img.shields.io/github/release/hardwario/py-hardwario-chester.svg)](https://github.com/hardwario/py-hardwario-chester/releases)\n[![PyPI](https://img.shields.io/pypi/v/hardwario-chester.svg)](https://pypi.org/project/hardwario-chester/)\n[![License](https://img.shields.io/github/license/hardwario/py-hardwario-chester.svg)](https://github.com/hardwario/py-hardwario-chester/blob/master/LICENSE)\n[![Twitter](https://img.shields.io/twitter/follow/hardwario_en.svg?style=social&label=Follow)](https://twitter.com/hardwario_en)\n\nThis repository contains Python package [hardwario-chester](https://pypi.org/project/hardwario-chester/)\n\n\n## License\n\nThis project is licensed under the [MIT License](https://opensource.org/licenses/MIT/) - see the [LICENSE](LICENSE) file for details.\n\n---\n\nMade with &#x2764;&nbsp; by [**HARDWARIO s.r.o.**](https://www.hardwario.com/) in the heart of Europe.\n',
     'author': 'Karel Blavka',
     'author_email': 'karel.blavka@hardwario.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/hardwario/py-hardwario-chester',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['hardwario', 'hardwario.chester', 'hardwario.chester.cli']
 package_data = \ {'': ['*']} install_requires = \ ['click>=8.0.3,<9.0.0',
 'docker>=5.0.3,<6.0.0', 'hardwario-common>=1.6.1,<2.0.0',
 'loguru>=0.6.0,<0.7.0', 'prompt-toolkit>=3.0.28,<4.0.0', 'pylink-
 square>=0.12.0,<0.13.0', 'pynrfjprog==10.15.2', 'pyperclip>=1.8.2,<2.0.0']
 entry_points = \ {'console_scripts': ['chester = hardwario.chester.cli:main']}
-setup_kwargs = { 'name': 'hardwario-chester', 'version': '1.8.6',
+setup_kwargs = { 'name': 'hardwario-chester', 'version': '1.9.0',
 'description': 'HARDWARIO CHESTER', 'long_description': '[HARDWARIO_Logo]\n\n#
 HARDWARIO CHESTER\n\n[![Main](https://github.com/hardwario/py-hardwario-
 chester/actions/workflows/main.yaml/badge.svg)](https://github.com/hardwario/
 py-hardwario-chester/actions/workflows/main.yaml)\n[![Release](https://
 img.shields.io/github/release/hardwario/py-hardwario-chester.svg)](https://
 github.com/hardwario/py-hardwario-chester/releases)\n[![PyPI](https://
 img.shields.io/pypi/v/hardwario-chester.svg)](https://pypi.org/project/
```

### Comparing `hardwario-chester-1.8.6/PKG-INFO` & `hardwario-chester-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardwario-chester
-Version: 1.8.6
+Version: 1.9.0
 Summary: HARDWARIO CHESTER
 Home-page: https://github.com/hardwario/py-hardwario-chester
 License: MIT
 Author: Karel Blavka
 Author-email: karel.blavka@hardwario.com
 Requires-Python: >=3.6.2
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hardwario-chester Version: 1.8.6 Summary: HARDWARIO
+Metadata-Version: 2.1 Name: hardwario-chester Version: 1.9.0 Summary: HARDWARIO
 CHESTER Home-page: https://github.com/hardwario/py-hardwario-chester License:
 MIT Author: Karel Blavka Author-email: karel.blavka@hardwario.com Requires-
 Python: >=3.6.2 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

