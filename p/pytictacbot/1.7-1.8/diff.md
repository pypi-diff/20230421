# Comparing `tmp/pytictacbot-1.7.tar.gz` & `tmp/pytictacbot-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytictacbot-1.7.tar", last modified: Fri Apr 21 15:48:18 2023, max compression
+gzip compressed data, was "pytictacbot-1.8.tar", last modified: Fri Apr 21 16:37:54 2023, max compression
```

## Comparing `pytictacbot-1.7.tar` & `pytictacbot-1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 15:48:18.175886 pytictacbot-1.7/
--rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.7/MANIFEST.in
--rw-r--r--   0 edgarcresson   (501) staff       (20)     4150 2023-04-21 15:48:18.175713 pytictacbot-1.7/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)     3997 2023-04-21 15:46:37.000000 pytictacbot-1.7/README.md
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 15:48:18.171332 pytictacbot-1.7/pytictacbot.egg-info/
--rw-r--r--   0 edgarcresson   (501) staff       (20)     4150 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/SOURCES.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/dependency_links.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/entry_points.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/requires.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-21 15:48:18.000000 pytictacbot-1.7/pytictacbot.egg-info/top_level.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-21 15:48:18.175926 pytictacbot-1.7/setup.cfg
--rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-21 15:46:56.000000 pytictacbot-1.7/setup.py
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 15:48:18.175462 pytictacbot-1.7/tictacbot/
--rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-21 10:51:49.000000 pytictacbot-1.7/tictacbot/gutenberg.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)     7589 2023-04-21 15:44:11.000000 pytictacbot-1.7/tictacbot/listen.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 16:37:54.946737 pytictacbot-1.8/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.8/MANIFEST.in
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     4130 2023-04-21 16:37:54.946608 pytictacbot-1.8/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     3977 2023-04-21 15:58:01.000000 pytictacbot-1.8/README.md
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 16:37:54.942786 pytictacbot-1.8/pytictacbot.egg-info/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     4130 2023-04-21 16:37:54.000000 pytictacbot-1.8/pytictacbot.egg-info/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-21 16:37:54.000000 pytictacbot-1.8/pytictacbot.egg-info/SOURCES.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-21 16:37:54.000000 pytictacbot-1.8/pytictacbot.egg-info/dependency_links.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-21 16:37:54.000000 pytictacbot-1.8/pytictacbot.egg-info/entry_points.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-21 16:37:54.000000 pytictacbot-1.8/pytictacbot.egg-info/requires.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-21 16:37:54.000000 pytictacbot-1.8/pytictacbot.egg-info/top_level.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-21 16:37:54.946774 pytictacbot-1.8/setup.cfg
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-21 16:37:30.000000 pytictacbot-1.8/setup.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 16:37:54.946420 pytictacbot-1.8/tictacbot/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-21 10:51:49.000000 pytictacbot-1.8/tictacbot/gutenberg.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     7331 2023-04-21 16:28:37.000000 pytictacbot-1.8/tictacbot/listen.py
```

### Comparing `pytictacbot-1.7/PKG-INFO` & `pytictacbot-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.7
+Version: 1.8
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
@@ -75,8 +75,8 @@
 
 Finally, it will erase the sequence of letters that has ben typed by the user and paste the word instead.
 
 ## TODO's
 
 - [ ] **Handling this case**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
 - [ ] **Refining the source**: In rare cases, a word retrieved by *Tictacbot* may not be accepted in the game. In this case, manually remove the word from [the source file](tictacbot/gutenberg.txt).
-- [x] **Manage all environments**: Adapt the keyboard shortcuts to the user's operating system and keyboard layout.
+- [x] **Manage all environments**: Adapt the keyboard shortcuts to the user's operating system.
```

### Comparing `pytictacbot-1.7/README.md` & `pytictacbot-1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,8 +69,8 @@
 
 Finally, it will erase the sequence of letters that has ben typed by the user and paste the word instead.
 
 ## TODO's
 
 - [ ] **Handling this case**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
 - [ ] **Refining the source**: In rare cases, a word retrieved by *Tictacbot* may not be accepted in the game. In this case, manually remove the word from [the source file](tictacbot/gutenberg.txt).
-- [x] **Manage all environments**: Adapt the keyboard shortcuts to the user's operating system and keyboard layout.
+- [x] **Manage all environments**: Adapt the keyboard shortcuts to the user's operating system.
```

### Comparing `pytictacbot-1.7/pytictacbot.egg-info/PKG-INFO` & `pytictacbot-1.8/pytictacbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.7
+Version: 1.8
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
@@ -75,8 +75,8 @@
 
 Finally, it will erase the sequence of letters that has ben typed by the user and paste the word instead.
 
 ## TODO's
 
 - [ ] **Handling this case**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
 - [ ] **Refining the source**: In rare cases, a word retrieved by *Tictacbot* may not be accepted in the game. In this case, manually remove the word from [the source file](tictacbot/gutenberg.txt).
-- [x] **Manage all environments**: Adapt the keyboard shortcuts to the user's operating system and keyboard layout.
+- [x] **Manage all environments**: Adapt the keyboard shortcuts to the user's operating system.
```

### Comparing `pytictacbot-1.7/setup.py` & `pytictacbot-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pytictacbot",
-    version="1.7",
+    version="1.8",
     packages=["tictacbot"],
     include_package_data=True,
     description="A program that makes you unbeatable at BombParty",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "pynput",
```

### Comparing `pytictacbot-1.7/tictacbot/gutenberg.txt` & `pytictacbot-1.8/tictacbot/gutenberg.txt`

 * *Files identical despite different names*

### Comparing `pytictacbot-1.7/tictacbot/listen.py` & `pytictacbot-1.8/tictacbot/listen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 import os
 import platform
-import locale
 import unicodedata
 from pynput import keyboard
 import pyperclip
 import pyautogui
 from art import text2art
 from colorama import init, Fore, Style
 
 init()
 
 platform_system = platform.system()
-
-keyboard_layout = None
-lang, encoding = locale.getlocale()
-locale.setlocale(locale.LC_ALL, lang)
-if (
-    locale.nl_langinfo(locale.CODESET) == "UTF-8"
-    and locale.nl_langinfo(locale.YESEXPR) == "^[oOyY]"
-):
-    keyboard_layout = "qwerty"
-else:
-    keyboard_layout = "azerty"
+control_key = "control"
+if platform_system == "Darwin":  # macOS
+    control_key = "command"
 
 letters_to_discover = list("abcdefghijlmnopqrstuv")
-keys_pressed: list[str] = []
+letters_pressed: list[str] = []
 words_already_used: list[str] = []
 remaining_letters = letters_to_discover.copy()
 
 
 def remove_accent(word: str) -> str:
     return unicodedata.normalize("NFD", word).encode("ascii", "ignore").decode("utf-8")
 
@@ -59,18 +50,18 @@
     global remaining_letters
     if not init:
         print("\n")
         print("_" * 50)
     label_colored = Fore.YELLOW + "Remaining letters: \n" + Style.RESET_ALL
     remaining_letters_beautified = ""
     for letter in remaining_letters:
-        letter_colored = Fore.LIGHTBLUE_EX + letter + Style.RESET_ALL
+        letter_colored = Fore.LIGHTBLUE_EX + letter.upper() + Style.RESET_ALL
         remaining_letters_beautified += "[" + letter_colored + "] "
     print(label_colored + remaining_letters_beautified + "\n")
-    print(Fore.YELLOW + "Keys pressed: " + Style.RESET_ALL)
+    print(Fore.YELLOW + "Letters pressed: " + Style.RESET_ALL)
 
 
 def print_success_message():
     text = "Alphabet completed !"
     width = len(text) + 4
     border = "-" * width
     content = f"| {text} |"
@@ -102,45 +93,39 @@
         if letter not in remove_accent(word_found)
     ]
     if len(remaining_letters) == 0:
         print_success_message()
         remaining_letters = letters_to_discover.copy()
 
 
-def paste_word(word: str):
-    global keyboard_layout
+def paste_word_and_press_enter(word: str):
+    global control_key
     print("\n" + Fore.YELLOW + "Pasting..." + Style.RESET_ALL)
+
     pyperclip.copy(word)
-    if platform_system == "Darwin":  # macOS
-        pyautogui.hotkey("command")  # init command key
-        if keyboard_layout == "azerty":
-            pyautogui.hotkey("command", "q")  # means command + a on azerty keyboard
-        else:
-            pyautogui.hotkey("command", "a")
-        pyautogui.hotkey("command", "v")
-    else:  # Windows, Linux...
-        pyautogui.hotkey("ctrl")  # init ctrl key
-        if keyboard_layout == "azerty":
-            pyautogui.hotkey("ctrl", "q")  # means ctrl + a on azerty keyboard
-        else:
-            pyautogui.hotkey("ctrl", "a")
-        pyautogui.hotkey("ctrl", "v")
+
+    pyautogui.hotkey(control_key)  # init control key
+    pyautogui.hotkey(control_key, "backspace")
+    pyautogui.hotkey(control_key, "v")
+    pyautogui.hotkey("enter")
+
     print(Fore.GREEN + "Pasted !" + Style.RESET_ALL)
 
 
 def escape():
     print(Fore.YELLOW + "Escaping..." + Style.RESET_ALL)
-    keys_pressed.clear()
+    letters_pressed.clear()
     print_new_section(init=False)
 
 
 def search():
-    print("\n" + Fore.YELLOW + "Searching..." + Style.RESET_ALL)
+    print("\n")
+    print(Fore.YELLOW + "Searching..." + Style.RESET_ALL)
     global remaining_letters
-    str_to_search = "".join(keys_pressed)
+    str_to_search = "".join(letters_pressed)
     best_word = retrieve_best_word(str_to_search, remaining_letters)
 
     if best_word and best_word["word"] and len(best_word["word"]):
         word_found: str = best_word["word"]
         word_score: int = best_word["score"]
 
         # Colorization start (really annoying to read)
@@ -197,35 +182,39 @@
             word_found_label_colored
             + word_found_colored
             + " - "
             + score_label_colored
             + score
         )
         update_remaining_letters(word_found.lower())
-        paste_word(word_found.lower())
+        paste_word_and_press_enter(word_found.lower())
     else:
         print(Fore.RED + "Not found" + Style.RESET_ALL)
-    keys_pressed.clear()
+        pyautogui.hotkey(control_key)  # init control key
+        pyautogui.hotkey(control_key, "backspace")
+    letters_pressed.clear()
     print_new_section(init=False)
 
 
 def on_press(key):
     try:
         key_char = key.char
         if not key_char.isalpha():
             return
-        keys_pressed.append(key_char)
+        letters_pressed.append(key_char)
     except AttributeError:
-        if key == keyboard.Key.esc:
+        if key == keyboard.Key.esc and len(letters_pressed):
             escape()
-        if key == keyboard.Key.space:
+        if key == keyboard.Key.space and len(letters_pressed):
             search()
+        if key == keyboard.Key.backspace and len(letters_pressed):
+            letters_pressed.pop(-1)
 
-    if len(keys_pressed):
-        print("".join(keys_pressed))
+    print("\r\033[K", end="", flush=True) # erase previous line
+    print("".join(letters_pressed).upper(), end="", flush=True)
 
 
 listener = keyboard.Listener(on_press=on_press)
 
 listener.start()
 
 print(text2art("Tictacbot"))
```

