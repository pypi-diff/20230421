# Comparing `tmp/pytictacbot-1.4.tar.gz` & `tmp/pytictacbot-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytictacbot-1.4.tar", last modified: Thu Apr 20 09:46:22 2023, max compression
+gzip compressed data, was "pytictacbot-1.5.tar", last modified: Thu Apr 20 12:26:23 2023, max compression
```

## Comparing `pytictacbot-1.4.tar` & `pytictacbot-1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 09:46:22.630764 pytictacbot-1.4/
--rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.4/MANIFEST.in
--rw-r--r--   0 edgarcresson   (501) staff       (20)     3116 2023-04-20 09:46:22.630622 pytictacbot-1.4/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)     2963 2023-04-20 09:45:54.000000 pytictacbot-1.4/README.md
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 09:46:22.626617 pytictacbot-1.4/pytictacbot.egg-info/
--rw-r--r--   0 edgarcresson   (501) staff       (20)     3116 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/SOURCES.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/dependency_links.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/entry_points.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/requires.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/top_level.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-20 09:46:22.630814 pytictacbot-1.4/setup.cfg
--rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-20 09:46:00.000000 pytictacbot-1.4/setup.py
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 09:46:22.630276 pytictacbot-1.4/tictacbot/
--rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-14 12:45:16.000000 pytictacbot-1.4/tictacbot/gutenberg.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)     6477 2023-04-20 08:47:39.000000 pytictacbot-1.4/tictacbot/listen.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 12:26:23.582573 pytictacbot-1.5/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.5/MANIFEST.in
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     3151 2023-04-20 12:26:23.582442 pytictacbot-1.5/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     2998 2023-04-20 12:25:02.000000 pytictacbot-1.5/README.md
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 12:26:23.578920 pytictacbot-1.5/pytictacbot.egg-info/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     3151 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/SOURCES.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/dependency_links.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/entry_points.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/requires.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/top_level.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-20 12:26:23.582610 pytictacbot-1.5/setup.cfg
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-20 12:25:36.000000 pytictacbot-1.5/setup.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 12:26:23.582258 pytictacbot-1.5/tictacbot/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-14 12:45:16.000000 pytictacbot-1.5/tictacbot/gutenberg.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     6531 2023-04-20 12:19:46.000000 pytictacbot-1.5/tictacbot/listen.py
```

### Comparing `pytictacbot-1.4/PKG-INFO` & `pytictacbot-1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.4
+Version: 1.5
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
@@ -46,15 +46,15 @@
 
 After a successful search, the found word will be automatically pasted. The "remaining letters" list will be updated accordingly.
 
 ## Rules
 
 Before understanding how does it work, let's remember the rules of the bomb party :
 - The player will be given a series of letters. He will then have to find (as quickly as possible) a word that contains this series of letters *(ex: "iso" -> "ma**iso**n")*
-- The player starts with a list of all the letters in the alphabet. If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
+- The player starts with a list of all the letters in the alphabet, except "k", "w", "x", "y" and "z". If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
 
 Finally, the goal in each round would be to find a word containing the sequence of letters, but also the one that will unlock the most letters at once!
 
 ## How does it work ?
 
 Once the script is launched, it will run in the background, listening to the keys that are typed on the keyboard.
```

### Comparing `pytictacbot-1.4/README.md` & `pytictacbot-1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 After a successful search, the found word will be automatically pasted. The "remaining letters" list will be updated accordingly.
 
 ## Rules
 
 Before understanding how does it work, let's remember the rules of the bomb party :
 - The player will be given a series of letters. He will then have to find (as quickly as possible) a word that contains this series of letters *(ex: "iso" -> "ma**iso**n")*
-- The player starts with a list of all the letters in the alphabet. If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
+- The player starts with a list of all the letters in the alphabet, except "k", "w", "x", "y" and "z". If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
 
 Finally, the goal in each round would be to find a word containing the sequence of letters, but also the one that will unlock the most letters at once!
 
 ## How does it work ?
 
 Once the script is launched, it will run in the background, listening to the keys that are typed on the keyboard.
```

### Comparing `pytictacbot-1.4/pytictacbot.egg-info/PKG-INFO` & `pytictacbot-1.5/pytictacbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.4
+Version: 1.5
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
@@ -46,15 +46,15 @@
 
 After a successful search, the found word will be automatically pasted. The "remaining letters" list will be updated accordingly.
 
 ## Rules
 
 Before understanding how does it work, let's remember the rules of the bomb party :
 - The player will be given a series of letters. He will then have to find (as quickly as possible) a word that contains this series of letters *(ex: "iso" -> "ma**iso**n")*
-- The player starts with a list of all the letters in the alphabet. If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
+- The player starts with a list of all the letters in the alphabet, except "k", "w", "x", "y" and "z". If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
 
 Finally, the goal in each round would be to find a word containing the sequence of letters, but also the one that will unlock the most letters at once!
 
 ## How does it work ?
 
 Once the script is launched, it will run in the background, listening to the keys that are typed on the keyboard.
```

### Comparing `pytictacbot-1.4/setup.py` & `pytictacbot-1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pytictacbot",
-    version="1.4",
+    version="1.5",
     packages=["tictacbot"],
     include_package_data=True,
     description="A program that makes you unbeatable at BombParty",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "pynput",
```

### Comparing `pytictacbot-1.4/tictacbot/gutenberg.txt` & `pytictacbot-1.5/tictacbot/gutenberg.txt`

 * *Files identical despite different names*

### Comparing `pytictacbot-1.4/tictacbot/listen.py` & `pytictacbot-1.5/tictacbot/listen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import os
+import unicodedata
 from pynput import keyboard
 import pyperclip
 import pyautogui
 from art import text2art
 from colorama import init, Fore, Style
-import unicodedata
 
 init()
 
+letters_to_discover = list("abcdefghijlmnopqrstuv")
+
 keys_pressed = []
-remaining_letters = list("abcdefghijklmnopqrstuvwxyz")
+remaining_letters = letters_to_discover.copy()
+
 
 def remove_accent(word: str) -> str:
-    return unicodedata.normalize('NFD', word).encode('ascii', 'ignore').decode('utf-8')
+    return unicodedata.normalize("NFD", word).encode("ascii", "ignore").decode("utf-8")
+
 
 def retrieve_best_word(
     str_to_search: str, remaining_letters: list[str]
 ) -> dict["word":str, "score":int] | None:
     if str_to_search.isalpha():
         str_to_search = str_to_search.lower()
 
         this_file_path = os.path.dirname(os.path.abspath(__file__))
         gutenberg = os.path.join(this_file_path, "gutenberg.txt")
 
         best_word = {"word": None, "score": -1}
         with open(gutenberg, "r", encoding="utf-8") as f:
             for word in f:
-                if str_to_search in word: 
+                if str_to_search in word:
                     score = len(set(remove_accent(word)) & set(remaining_letters))
                     word_found = {"word": word.strip(), "score": score}
                     if best_word["score"] < word_found["score"]:
                         best_word = word_found
             return best_word
 
 
@@ -72,19 +76,21 @@
 
     print(Style.RESET_ALL)
 
 
 def update_remaining_letters(word_found: str):
     global remaining_letters
     remaining_letters = [
-        letter for letter in remaining_letters if letter not in remove_accent(word_found)
+        letter
+        for letter in remaining_letters
+        if letter not in remove_accent(word_found)
     ]
     if len(remaining_letters) == 0:
         print_success_message()
-        remaining_letters = list("abcdefghijklmnopqrstuvwxyz")
+        remaining_letters = letters_to_discover.copy()
 
 
 def paste_word(word: str):
     print("\n" + Fore.YELLOW + "Pasting..." + Style.RESET_ALL)
     pyperclip.copy(word)
     pyautogui.press("backspace", presses=len(keys_pressed) + 1)
     pyautogui.hotkey("command", "v")
```

