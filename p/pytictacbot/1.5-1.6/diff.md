# Comparing `tmp/pytictacbot-1.5.tar.gz` & `tmp/pytictacbot-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytictacbot-1.5.tar", last modified: Thu Apr 20 12:26:23 2023, max compression
+gzip compressed data, was "pytictacbot-1.6.tar", last modified: Fri Apr 21 11:06:09 2023, max compression
```

## Comparing `pytictacbot-1.5.tar` & `pytictacbot-1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 12:26:23.582573 pytictacbot-1.5/
--rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.5/MANIFEST.in
--rw-r--r--   0 edgarcresson   (501) staff       (20)     3151 2023-04-20 12:26:23.582442 pytictacbot-1.5/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)     2998 2023-04-20 12:25:02.000000 pytictacbot-1.5/README.md
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 12:26:23.578920 pytictacbot-1.5/pytictacbot.egg-info/
--rw-r--r--   0 edgarcresson   (501) staff       (20)     3151 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/SOURCES.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/dependency_links.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/entry_points.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/requires.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-20 12:26:23.000000 pytictacbot-1.5/pytictacbot.egg-info/top_level.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-20 12:26:23.582610 pytictacbot-1.5/setup.cfg
--rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-20 12:25:36.000000 pytictacbot-1.5/setup.py
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 12:26:23.582258 pytictacbot-1.5/tictacbot/
--rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-14 12:45:16.000000 pytictacbot-1.5/tictacbot/gutenberg.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)     6531 2023-04-20 12:19:46.000000 pytictacbot-1.5/tictacbot/listen.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 11:06:09.459816 pytictacbot-1.6/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.6/MANIFEST.in
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     3973 2023-04-21 11:06:09.459632 pytictacbot-1.6/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     3820 2023-04-21 11:01:50.000000 pytictacbot-1.6/README.md
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 11:06:09.455778 pytictacbot-1.6/pytictacbot.egg-info/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     3973 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/SOURCES.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/dependency_links.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/entry_points.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/requires.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-21 11:06:09.000000 pytictacbot-1.6/pytictacbot.egg-info/top_level.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-21 11:06:09.459864 pytictacbot-1.6/setup.cfg
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-21 10:53:13.000000 pytictacbot-1.6/setup.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-21 11:06:09.459303 pytictacbot-1.6/tictacbot/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-21 10:51:49.000000 pytictacbot-1.6/tictacbot/gutenberg.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     6697 2023-04-21 10:52:43.000000 pytictacbot-1.6/tictacbot/listen.py
```

### Comparing `pytictacbot-1.5/PKG-INFO` & `pytictacbot-1.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.5
+Version: 1.6
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
 ![Demo](tictacbot-demo.gif)
 
+## Disclaimer
+
+I developed this program because I wanted to challenge myself with code and found it fun to try to create a bot that could follow the rules of the game perfectly.
+
+It's not meant to be used to ruin other players' games: for my part, I used it to amaze and make my friends laugh during our private games.
+
+Anyway, I doubt that many people find much interest in cheating on a simple board game without much at stake.
+
 ## Installation
 
 ⚠️ This program requires a version of [python](https://www.python.org/) >= 3 installed on your machine.
 
 Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip* (it is included with python):
 ```zsh
 pip install pytictacbot
@@ -44,25 +52,30 @@
 - To launch the search, **press the space bar**.
 - To cancel the keys you typed, **press the escape key**. 
 
 After a successful search, the found word will be automatically pasted. The "remaining letters" list will be updated accordingly.
 
 ## Rules
 
-Before understanding how does it work, let's remember the rules of the bomb party :
-- The player will be given a series of letters. He will then have to find (as quickly as possible) a word that contains this series of letters *(ex: "iso" -> "ma**iso**n")*
-- The player starts with a list of all the letters in the alphabet, except "k", "w", "x", "y" and "z". If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
+Before understanding how does it work, let's remember the rules of the [jklm.fun's BombParty](https://jklm.fun/) :
+1. The player will be given a series of letters. He will then have to find (as quickly as possible) a word that contains this series of letters *(ex: "iso" -> "ma**iso**n")*
+2. The player can't reuse a word that has already been used during the game.
+3. The player starts with a list of all the letters in the alphabet, except "k", "w", "x", "y" and "z". If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
 
-Finally, the goal in each round would be to find a word containing the sequence of letters, but also the one that will unlock the most letters at once!
+Finally, the goal in each round would be to find a word containing the sequence of letters, that has not been used already, but also the one that will unlock the most letters at once!
 
 ## How does it work ?
 
 Once the script is launched, it will run in the background, listening to the keys that are typed on the keyboard.
 
 It will display everything on the interface to make it easier for the user to understand what is happening in the background.
 
-When the user will press escape to search the best word including the sequence of letters he/she typed, the *Tictacbot* will crawl a file containing all the words of the French language.
+When the user will press escape to search the best word including the sequence of letters he/she typed, *Tictacbot* will crawl a file containing all the words of the French language.
 
 It will first determine a list of all words containing the given sequence of letters.
-Then, it will crawl this list and, for each word, calculate a score using the letters to discover (cf. 2nd rule). It will finally return the word with the highest possible score.
+Then, it will crawl this list and, for each word, calculate a score using the letters to discover (cf. 3rd rule). It will finally return the word with the highest possible score.
 
 Finally, it will erase the sequence of letters that has ben typed by the user and paste the word instead.
+
+## TODO's
+
+- [ ] **Correct this issue**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
```

### Comparing `pytictacbot-1.5/README.md` & `pytictacbot-1.6/pytictacbot.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,27 @@
+Metadata-Version: 2.1
+Name: pytictacbot
+Version: 1.6
+Summary: A program that makes you unbeatable at BombParty
+Description-Content-Type: text/markdown
+
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
 ![Demo](tictacbot-demo.gif)
 
+## Disclaimer
+
+I developed this program because I wanted to challenge myself with code and found it fun to try to create a bot that could follow the rules of the game perfectly.
+
+It's not meant to be used to ruin other players' games: for my part, I used it to amaze and make my friends laugh during our private games.
+
+Anyway, I doubt that many people find much interest in cheating on a simple board game without much at stake.
+
 ## Installation
 
 ⚠️ This program requires a version of [python](https://www.python.org/) >= 3 installed on your machine.
 
 Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip* (it is included with python):
 ```zsh
 pip install pytictacbot
@@ -38,25 +52,30 @@
 - To launch the search, **press the space bar**.
 - To cancel the keys you typed, **press the escape key**. 
 
 After a successful search, the found word will be automatically pasted. The "remaining letters" list will be updated accordingly.
 
 ## Rules
 
-Before understanding how does it work, let's remember the rules of the bomb party :
-- The player will be given a series of letters. He will then have to find (as quickly as possible) a word that contains this series of letters *(ex: "iso" -> "ma**iso**n")*
-- The player starts with a list of all the letters in the alphabet, except "k", "w", "x", "y" and "z". If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
+Before understanding how does it work, let's remember the rules of the [jklm.fun's BombParty](https://jklm.fun/) :
+1. The player will be given a series of letters. He will then have to find (as quickly as possible) a word that contains this series of letters *(ex: "iso" -> "ma**iso**n")*
+2. The player can't reuse a word that has already been used during the game.
+3. The player starts with a list of all the letters in the alphabet, except "k", "w", "x", "y" and "z". If, with the words he/she types during the game, the player manages to use all these letters at least once, then the player will gain an extra life.
 
-Finally, the goal in each round would be to find a word containing the sequence of letters, but also the one that will unlock the most letters at once!
+Finally, the goal in each round would be to find a word containing the sequence of letters, that has not been used already, but also the one that will unlock the most letters at once!
 
 ## How does it work ?
 
 Once the script is launched, it will run in the background, listening to the keys that are typed on the keyboard.
 
 It will display everything on the interface to make it easier for the user to understand what is happening in the background.
 
-When the user will press escape to search the best word including the sequence of letters he/she typed, the *Tictacbot* will crawl a file containing all the words of the French language.
+When the user will press escape to search the best word including the sequence of letters he/she typed, *Tictacbot* will crawl a file containing all the words of the French language.
 
 It will first determine a list of all words containing the given sequence of letters.
-Then, it will crawl this list and, for each word, calculate a score using the letters to discover (cf. 2nd rule). It will finally return the word with the highest possible score.
+Then, it will crawl this list and, for each word, calculate a score using the letters to discover (cf. 3rd rule). It will finally return the word with the highest possible score.
+
+Finally, it will erase the sequence of letters that has ben typed by the user and paste the word instead.
+
+## TODO's
 
-Finally, it will erase the sequence of letters that has ben typed by the user and paste the word instead.
+- [ ] **Correct this issue**: Currently, the program does not remain the words that has been used by the other players (only those that the player himself used). This can sometimes result in the reuse of an already used word (cf. 2nd rule).
```

### Comparing `pytictacbot-1.5/setup.py` & `pytictacbot-1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pytictacbot",
-    version="1.5",
+    version="1.6",
     packages=["tictacbot"],
     include_package_data=True,
     description="A program that makes you unbeatable at BombParty",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "pynput",
```

### Comparing `pytictacbot-1.5/tictacbot/gutenberg.txt` & `pytictacbot-1.6/tictacbot/gutenberg.txt`

 * *Files identical despite different names*

### Comparing `pytictacbot-1.5/tictacbot/listen.py` & `pytictacbot-1.6/tictacbot/listen.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from art import text2art
 from colorama import init, Fore, Style
 
 init()
 
 letters_to_discover = list("abcdefghijlmnopqrstuv")
 
-keys_pressed = []
+keys_pressed: list[str] = []
+words_already_used: list[str] = []
 remaining_letters = letters_to_discover.copy()
 
 
 def remove_accent(word: str) -> str:
     return unicodedata.normalize("NFD", word).encode("ascii", "ignore").decode("utf-8")
 
 
@@ -26,19 +27,21 @@
 
         this_file_path = os.path.dirname(os.path.abspath(__file__))
         gutenberg = os.path.join(this_file_path, "gutenberg.txt")
 
         best_word = {"word": None, "score": -1}
         with open(gutenberg, "r", encoding="utf-8") as f:
             for word in f:
-                if str_to_search in word:
+                word = word.strip()
+                if str_to_search in word and word not in words_already_used:
                     score = len(set(remove_accent(word)) & set(remaining_letters))
-                    word_found = {"word": word.strip(), "score": score}
+                    word_found = {"word": word, "score": score}
                     if best_word["score"] < word_found["score"]:
                         best_word = word_found
+            words_already_used.append(best_word["word"])
             return best_word
 
 
 def print_new_section(init: bool):
     global remaining_letters
     if not init:
         print("\n")
```

