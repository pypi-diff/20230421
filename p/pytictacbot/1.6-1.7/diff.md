# Comparing `tmp/pytictacbot-1.6.tar.gz` & `tmp/pytictacbot-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytictacbot-1.6.tar", last modified: Fri Apr 21 11:06:09 2023, max compression
+gzip compressed data, was "pytictacbot-1.7.tar", last modified: Fri Apr 21 15:48:18 2023, max compression
```

## Comparing `pytictacbot-1.6.tar` & `pytictacbot-1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 11:06:09.459816 pytictacbot-1.6/
--rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.6/MANIFEST.in
--rw-r--r--   0 edgarcresson   (501) staff       (20)     3973 2023-04-21 11:06:09.459632 pytictacbot-1.6/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)     3820 2023-04-21 11:01:50.000000 pytictacbot-1.6/README.md
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 11:06:09.455778 pytictacbot-1.6/pytictacbot.egg-info/
--rw-r--r--   0 edgarcresson   (501) staff       (20)     3973 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/SOURCES.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/dependency_links.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/entry_points.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/requires.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/top_level.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-21 11:06:09.459864 pytictacbot-1.6/setup.cfg
--rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-21 10:53:13.000000 pytictacbot-1.6/setup.py
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 11:06:09.459303 pytictacbot-1.6/tictacbot/
--rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-21 10:51:49.000000 pytictacbot-1.6/tictacbot/gutenberg.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)     6697 2023-04-21 10:52:43.000000 pytictacbot-1.6/tictacbot/listen.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 15:48:18.175886 pytictacbot-1.7/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.7/MANIFEST.in
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     4150 2023-04-21 15:48:18.175713 pytictacbot-1.7/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     3997 2023-04-21 15:46:37.000000 pytictacbot-1.7/README.md
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 15:48:18.171332 pytictacbot-1.7/pytictacbot.egg-info/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     4150 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/SOURCES.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/dependency_links.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/entry_points.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/requires.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/top_level.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-21 15:48:18.175926 pytictacbot-1.7/setup.cfg
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-21 15:46:56.000000 pytictacbot-1.7/setup.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 15:48:18.175462 pytictacbot-1.7/tictacbot/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-21 10:51:49.000000 pytictacbot-1.7/tictacbot/gutenberg.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     7589 2023-04-21 15:44:11.000000 pytictacbot-1.7/tictacbot/listen.py
```

### Comparing `pytictacbot-1.6/PKG-INFO` & `pytictacbot-1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.6
+Version: 1.7
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
@@ -25,57 +25,58 @@
 Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip* (it is included with python):
 ```zsh
 pip install pytictacbot
 ```
 
 ## Usage
 
-*Note: this program will only work on MacOS since it uses "Command + V" keys to paste. You can edit the code yourself if you want to adapt it to your environment.*
-
-In order for this program to work, you must allow "Accessibility" settings to the application that will run the script. Indeed, you need access to the input monitoring to listen to the keys you type.
+In order for this program to work, you must grant access to *Accessibility* and *Input Monitoring* to the application that will run the script. Indeed, the program need access to listen to the keys you type.
 
 On Mac:
 - Open *System settings*,
 - Navigate into the *Privacy & Security* section,
 - Click on *Accessibility*,
-- Allow the application(s) in which you will run the script (ex: iTerm, Visual Studio Code...),
+- Allow the application(s) in which you will run the script (ex: Terminal, iTerm...),
 - Go back, then do the same thing for *Input Monitoring*.
 
 Once this is done, it is ready to use !
 
 In your terminal, run:
 ```zsh
 tictacbot
 ```
 
-An interface will be displayed. It will listen to the keys you type. A history of these keys will be displayed in the interface.
+An interface will be displayed. It will listen to the keys you type. A history of these keys will be displayed on the interface.
 
 - To launch the search, **press the space bar**.
-- To cancel the keys you typed, **press the escape key**. 
+- To cancel the keys you typed, **press the escape key**.
+- To quit, **press control+c**.
 
-After a successful search, the found word will be automatically pasted. The "remaining letters" list will be updated accordingly.
+After a successful search, the found word will be automatically pasted. The *remaining letters* list will be updated accordingly.
 
 ## Rules
 
 Before understanding how does it work, let's remember the rules of the [jklm.fun's BombParty](https://jklm.fun/) :
-1. The player will be given a series of letters. He will then have to find (as quickly as possible) a word that contains this series of letters *(ex: "iso" -> "ma**iso**n")*
+1. The player will be given a series of letters. He have to find (as quickly as possible) a word that contains this series of letters *(ex: "**iso**" -> "ma**iso**n")*
 2. The player can't reuse a word that has already been used during the game.
 3. The player starts with a list of all the letters in the alphabet, except "k", "w", "x", "y" and "z". If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
 
 Finally, the goal in each round would be to find a word containing the sequence of letters, that has not been used already, but also the one that will unlock the most letters at once!
 
 ## How does it work ?
 
 Once the script is launched, it will run in the background, listening to the keys that are typed on the keyboard.
 
 It will display everything on the interface to make it easier for the user to understand what is happening in the background.
 
 When the user will press escape to search the best word including the sequence of letters he/she typed, *Tictacbot* will crawl a file containing all the words of the French language.
 
 It will first determine a list of all words containing the given sequence of letters.
-Then, it will crawl this list and, for each word, calculate a score using the letters to discover (cf. 3rd rule). It will finally return the word with the highest possible score.
+Then, it will crawl this list and, for each word, calculate a score using the letters to discover (cf. 3rd rule). At the end, it will return the word with the highest possible score.
 
 Finally, it will erase the sequence of letters that has ben typed by the user and paste the word instead.
 
 ## TODO's
 
-- [ ] **Correct this issue**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
+- [ ] **Handling this case**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
+- [ ] **Refining the source**: In rare cases, a word retrieved by *Tictacbot* may not be accepted in the game. In this case, manually remove the word from [the source file](tictacbot/gutenberg.txt).
+- [x] **Manage all environments**: Adapt the keyboard shortcuts to the user's operating system and keyboard layout.
```

### Comparing `pytictacbot-1.6/README.md` & `pytictacbot-1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,57 +19,58 @@
 Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip* (it is included with python):
 ```zsh
 pip install pytictacbot
 ```
 
 ## Usage
 
-*Note: this program will only work on MacOS since it uses "Command + V" keys to paste. You can edit the code yourself if you want to adapt it to your environment.*
-
-In order for this program to work, you must allow "Accessibility" settings to the application that will run the script. Indeed, you need access to the input monitoring to listen to the keys you type.
+In order for this program to work, you must grant access to *Accessibility* and *Input Monitoring* to the application that will run the script. Indeed, the program need access to listen to the keys you type.
 
 On Mac:
 - Open *System settings*,
 - Navigate into the *Privacy & Security* section,
 - Click on *Accessibility*,
-- Allow the application(s) in which you will run the script (ex: iTerm, Visual Studio Code...),
+- Allow the application(s) in which you will run the script (ex: Terminal, iTerm...),
 - Go back, then do the same thing for *Input Monitoring*.
 
 Once this is done, it is ready to use !
 
 In your terminal, run:
 ```zsh
 tictacbot
 ```
 
-An interface will be displayed. It will listen to the keys you type. A history of these keys will be displayed in the interface.
+An interface will be displayed. It will listen to the keys you type. A history of these keys will be displayed on the interface.
 
 - To launch the search, **press the space bar**.
-- To cancel the keys you typed, **press the escape key**. 
+- To cancel the keys you typed, **press the escape key**.
+- To quit, **press control+c**.
 
-After a successful search, the found word will be automatically pasted. The "remaining letters" list will be updated accordingly.
+After a successful search, the found word will be automatically pasted. The *remaining letters* list will be updated accordingly.
 
 ## Rules
 
 Before understanding how does it work, let's remember the rules of the [jklm.fun's BombParty](https://jklm.fun/) :
-1. The player will be given a series of letters. He will then have to find (as quickly as possible) a word that contains this series of letters *(ex: "iso" -> "ma**iso**n")*
+1. The player will be given a series of letters. He have to find (as quickly as possible) a word that contains this series of letters *(ex: "**iso**" -> "ma**iso**n")*
 2. The player can't reuse a word that has already been used during the game.
 3. The player starts with a list of all the letters in the alphabet, except "k", "w", "x", "y" and "z". If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
 
 Finally, the goal in each round would be to find a word containing the sequence of letters, that has not been used already, but also the one that will unlock the most letters at once!
 
 ## How does it work ?
 
 Once the script is launched, it will run in the background, listening to the keys that are typed on the keyboard.
 
 It will display everything on the interface to make it easier for the user to understand what is happening in the background.
 
 When the user will press escape to search the best word including the sequence of letters he/she typed, *Tictacbot* will crawl a file containing all the words of the French language.
 
 It will first determine a list of all words containing the given sequence of letters.
-Then, it will crawl this list and, for each word, calculate a score using the letters to discover (cf. 3rd rule). It will finally return the word with the highest possible score.
+Then, it will crawl this list and, for each word, calculate a score using the letters to discover (cf. 3rd rule). At the end, it will return the word with the highest possible score.
 
 Finally, it will erase the sequence of letters that has ben typed by the user and paste the word instead.
 
 ## TODO's
 
-- [ ] **Correct this issue**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
+- [ ] **Handling this case**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
+- [ ] **Refining the source**: In rare cases, a word retrieved by *Tictacbot* may not be accepted in the game. In this case, manually remove the word from [the source file](tictacbot/gutenberg.txt).
+- [x] **Manage all environments**: Adapt the keyboard shortcuts to the user's operating system and keyboard layout.
```

### Comparing `pytictacbot-1.6/pytictacbot.egg-info/PKG-INFO` & `pytictacbot-1.7/pytictacbot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.6
+Version: 1.7
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
@@ -25,57 +25,58 @@
 Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip* (it is included with python):
 ```zsh
 pip install pytictacbot
 ```
 
 ## Usage
 
-*Note: this program will only work on MacOS since it uses "Command + V" keys to paste. You can edit the code yourself if you want to adapt it to your environment.*
-
-In order for this program to work, you must allow "Accessibility" settings to the application that will run the script. Indeed, you need access to the input monitoring to listen to the keys you type.
+In order for this program to work, you must grant access to *Accessibility* and *Input Monitoring* to the application that will run the script. Indeed, the program need access to listen to the keys you type.
 
 On Mac:
 - Open *System settings*,
 - Navigate into the *Privacy & Security* section,
 - Click on *Accessibility*,
-- Allow the application(s) in which you will run the script (ex: iTerm, Visual Studio Code...),
+- Allow the application(s) in which you will run the script (ex: Terminal, iTerm...),
 - Go back, then do the same thing for *Input Monitoring*.
 
 Once this is done, it is ready to use !
 
 In your terminal, run:
 ```zsh
 tictacbot
 ```
 
-An interface will be displayed. It will listen to the keys you type. A history of these keys will be displayed in the interface.
+An interface will be displayed. It will listen to the keys you type. A history of these keys will be displayed on the interface.
 
 - To launch the search, **press the space bar**.
-- To cancel the keys you typed, **press the escape key**. 
+- To cancel the keys you typed, **press the escape key**.
+- To quit, **press control+c**.
 
-After a successful search, the found word will be automatically pasted. The "remaining letters" list will be updated accordingly.
+After a successful search, the found word will be automatically pasted. The *remaining letters* list will be updated accordingly.
 
 ## Rules
 
 Before understanding how does it work, let's remember the rules of the [jklm.fun's BombParty](https://jklm.fun/) :
-1. The player will be given a series of letters. He will then have to find (as quickly as possible) a word that contains this series of letters *(ex: "iso" -> "ma**iso**n")*
+1. The player will be given a series of letters. He have to find (as quickly as possible) a word that contains this series of letters *(ex: "**iso**" -> "ma**iso**n")*
 2. The player can't reuse a word that has already been used during the game.
 3. The player starts with a list of all the letters in the alphabet, except "k", "w", "x", "y" and "z". If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
 
 Finally, the goal in each round would be to find a word containing the sequence of letters, that has not been used already, but also the one that will unlock the most letters at once!
 
 ## How does it work ?
 
 Once the script is launched, it will run in the background, listening to the keys that are typed on the keyboard.
 
 It will display everything on the interface to make it easier for the user to understand what is happening in the background.
 
 When the user will press escape to search the best word including the sequence of letters he/she typed, *Tictacbot* will crawl a file containing all the words of the French language.
 
 It will first determine a list of all words containing the given sequence of letters.
-Then, it will crawl this list and, for each word, calculate a score using the letters to discover (cf. 3rd rule). It will finally return the word with the highest possible score.
+Then, it will crawl this list and, for each word, calculate a score using the letters to discover (cf. 3rd rule). At the end, it will return the word with the highest possible score.
 
 Finally, it will erase the sequence of letters that has ben typed by the user and paste the word instead.
 
 ## TODO's
 
-- [ ] **Correct this issue**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
+- [ ] **Handling this case**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
+- [ ] **Refining the source**: In rare cases, a word retrieved by *Tictacbot* may not be accepted in the game. In this case, manually remove the word from [the source file](tictacbot/gutenberg.txt).
+- [x] **Manage all environments**: Adapt the keyboard shortcuts to the user's operating system and keyboard layout.
```

### Comparing `pytictacbot-1.6/setup.py` & `pytictacbot-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pytictacbot",
-    version="1.6",
+    version="1.7",
     packages=["tictacbot"],
     include_package_data=True,
     description="A program that makes you unbeatable at BombParty",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "pynput",
```

### Comparing `pytictacbot-1.6/tictacbot/gutenberg.txt` & `pytictacbot-1.7/tictacbot/gutenberg.txt`

 * *Files identical despite different names*

### Comparing `pytictacbot-1.6/tictacbot/listen.py` & `pytictacbot-1.7/tictacbot/listen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 import os
+import platform
+import locale
 import unicodedata
 from pynput import keyboard
 import pyperclip
 import pyautogui
 from art import text2art
 from colorama import init, Fore, Style
 
 init()
 
-letters_to_discover = list("abcdefghijlmnopqrstuv")
+platform_system = platform.system()
+
+keyboard_layout = None
+lang, encoding = locale.getlocale()
+locale.setlocale(locale.LC_ALL, lang)
+if (
+    locale.nl_langinfo(locale.CODESET) == "UTF-8"
+    and locale.nl_langinfo(locale.YESEXPR) == "^[oOyY]"
+):
+    keyboard_layout = "qwerty"
+else:
+    keyboard_layout = "azerty"
 
+letters_to_discover = list("abcdefghijlmnopqrstuv")
 keys_pressed: list[str] = []
 words_already_used: list[str] = []
 remaining_letters = letters_to_discover.copy()
 
 
 def remove_accent(word: str) -> str:
     return unicodedata.normalize("NFD", word).encode("ascii", "ignore").decode("utf-8")
@@ -89,18 +103,31 @@
     ]
     if len(remaining_letters) == 0:
         print_success_message()
         remaining_letters = letters_to_discover.copy()
 
 
 def paste_word(word: str):
+    global keyboard_layout
     print("\n" + Fore.YELLOW + "Pasting..." + Style.RESET_ALL)
     pyperclip.copy(word)
-    pyautogui.press("backspace", presses=len(keys_pressed) + 1)
-    pyautogui.hotkey("command", "v")
+    if platform_system == "Darwin":  # macOS
+        pyautogui.hotkey("command")  # init command key
+        if keyboard_layout == "azerty":
+            pyautogui.hotkey("command", "q")  # means command + a on azerty keyboard
+        else:
+            pyautogui.hotkey("command", "a")
+        pyautogui.hotkey("command", "v")
+    else:  # Windows, Linux...
+        pyautogui.hotkey("ctrl")  # init ctrl key
+        if keyboard_layout == "azerty":
+            pyautogui.hotkey("ctrl", "q")  # means ctrl + a on azerty keyboard
+        else:
+            pyautogui.hotkey("ctrl", "a")
+        pyautogui.hotkey("ctrl", "v")
     print(Fore.GREEN + "Pasted !" + Style.RESET_ALL)
 
 
 def escape():
     print(Fore.YELLOW + "Escaping..." + Style.RESET_ALL)
     keys_pressed.clear()
     print_new_section(init=False)
```

