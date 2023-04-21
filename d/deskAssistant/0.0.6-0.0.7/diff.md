# Comparing `tmp/deskAssistant-0.0.6.tar.gz` & `tmp/deskAssistant-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\deskAssistant-0.0.6.tar", last modified: Sat Feb 18 11:54:32 2023, max compression
+gzip compressed data, was "dist\deskAssistant-0.0.7.tar", last modified: Fri Apr 21 19:49:40 2023, max compression
```

## Comparing `deskAssistant-0.0.6.tar` & `deskAssistant-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-02-18 11:54:32.353065 deskAssistant-0.0.6/
--rw-rw-rw-   0        0        0      609 2023-02-18 11:54:32.353065 deskAssistant-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-18 11:54:32.279262 deskAssistant-0.0.6/deskAssistant/
--rw-rw-rw-   0        0        0      349 2023-02-18 11:51:19.000000 deskAssistant-0.0.6/deskAssistant/__init__.py
--rw-rw-rw-   0        0        0     1620 2023-02-18 11:48:32.000000 deskAssistant-0.0.6/deskAssistant/deskAssistant.py
-drwxrwxrwx   0        0        0        0 2023-02-18 11:54:32.351071 deskAssistant-0.0.6/deskAssistant.egg-info/
--rw-rw-rw-   0        0        0      609 2023-02-18 11:54:32.000000 deskAssistant-0.0.6/deskAssistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-02-18 11:54:32.000000 deskAssistant-0.0.6/deskAssistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-18 11:54:32.000000 deskAssistant-0.0.6/deskAssistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-02-18 11:54:32.000000 deskAssistant-0.0.6/deskAssistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-18 11:54:32.000000 deskAssistant-0.0.6/deskAssistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-18 11:54:32.353065 deskAssistant-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-02-18 11:52:30.000000 deskAssistant-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:49:40.764917 deskAssistant-0.0.7/
+-rw-rw-rw-   0        0        0      539 2023-04-21 19:49:40.759930 deskAssistant-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 19:49:40.738475 deskAssistant-0.0.7/deskAssistant/
+-rw-rw-rw-   0        0        0       49 2023-04-21 18:44:38.000000 deskAssistant-0.0.7/deskAssistant/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-04-21 18:03:48.000000 deskAssistant-0.0.7/deskAssistant/deskAssistant.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:49:40.758934 deskAssistant-0.0.7/deskAssistant.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-04-21 19:49:40.000000 deskAssistant-0.0.7/deskAssistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-21 19:49:40.000000 deskAssistant-0.0.7/deskAssistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 19:49:40.000000 deskAssistant-0.0.7/deskAssistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 19:49:40.000000 deskAssistant-0.0.7/deskAssistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-21 19:49:40.000000 deskAssistant-0.0.7/deskAssistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 19:49:40.767908 deskAssistant-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-04-21 18:05:00.000000 deskAssistant-0.0.7/setup.py
```

### Comparing `deskAssistant-0.0.6/PKG-INFO` & `deskAssistant-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 Metadata-Version: 2.1
 Name: deskAssistant
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to help with making a virtual assistant
-Home-page: UNKNOWN
 Author: Blinken77YT
 Author-email: theonilsson2012@icloud.com
-License: UNKNOWN
 Keywords: python,virtual,assistant,assistant virtual,virtual assistant
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-
-UNKNOWN
-
```

### Comparing `deskAssistant-0.0.6/deskAssistant/deskAssistant.py` & `deskAssistant-0.0.7/deskAssistant/deskAssistant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 import speech_recognition as sr
 import pyttsx3 as tts
 import datetime as dt
 import webbrowser
 
-engine = tts.init()
-r = sr.Recognizer()
+class Assistant:
+    def __init__(self):
+        self.engine = tts.init()
+        self.r = sr.Recognizer()
+
+    def takeCommand(self):
+        with sr.Microphone() as source:
+            print("Listening...")
+            self.r.pause_threshold = 0.7
+            audio = self.r.listen(source)
+            try:
+                print("Recongizing...")
+                Query = self.r.recognize_google(audio, language="en-US")
+            except Exception as e:
+                print(e)
+                print("Say that again please")
+                return "None"
+            
+            return Query
+
+    def speak(self, audio):
+        self.engine.say(audio)
+        self.engine.runAndWait()
+
+    def tellDay(self):
+        day = dt.datetime.today().weekday() +1
+
+        Day_dict = {
+            1: 'Monday', 2: 'Tuesday', 3: 'Wednesday', 4: 'Thursday', 5: 'Friday', 6: 'Saturday', 7: 'Sunday'
+        }
+
+        if day in Day_dict.keys():
+            day_of_the_week = Day_dict[day]
+            print(day_of_the_week)
+            self.speak(f"It is {day_of_the_week} today!")
+
+
+    def tellTime(self):
+        time = str(dt.datetime.now())
+        print(time)
+        
+        hour = time[11:13]
+        if "0" in hour:
+            hour = hour.split("0")
+        min = time[14:16]
+        self.speak(f"The time is {hour} hours and {min} minutes")
+
+    def openMail(self):
+        webbrowser.open('mailto:', new=1)
+        self.speak("I opened your mail for you.")
 
-def takeCommand():
-    with sr.Microphone() as source:
-        print("Listening...")
-        r.pause_threshold = 0.7
-        audio = r.listen(source)
+    def calculate(self, expression):
         try:
-            print("Recongizing...")
-            Query = r.recognize_google(audio, language="en-US")
-        except Exception as e:
-            print(e)
-            print("Say that again please")
-            return "None"
-        
-        return Query
+            result = eval(expression)
+            return str(result)
+        except:
+            return "Sorry, I couldn't perform that calculation"
+
 
-def speak(audio):
-    engine.say(audio)
-    engine.runAndWait()
-
-def tellDay():
-    day = dt.datetime.today().weekday() +1
-
-    Day_dict = {
-        1: 'Monday', 2: 'Tuesday', 3: 'Wednesday', 4: 'Thursday', 5: 'Friday', 6: 'Saturday', 7: 'Sunday'
-    }
-
-    if day in Day_dict.keys():
-        day_of_the_week = Day_dict[day]
-        print(day_of_the_week)
-        speak(f"It is {day_of_the_week} today!")
-
-
-def tellTime():
-    time = str(dt.datetime.now())
-    print(time)
-    
-    hour = time[11:13]
-    if "0" in hour:
-        hour = hour.split("0")
-    min = time[14:16]
-    speak(f"The time is {hour} hours and {min} minutes")
-
-def openMail():
-    webbrowser.open('mailto:', new=1)
-    speak("I opened your mail for you.")
-
-def calculate(expression):
-    try:
-        result = eval(expression)
-        return str(result)
-    except:
-        return "Sorry, I couldn't perform that calculation"
-
-
-def voiceCalc():
-    expression = takeCommand()
-    result = calculate(expression)
-    speak(f"{result}")
+    def voiceCalc(self):
+        expression = self.takeCommand()
+        result = self.calculate(expression)
+        self.speak(f"{result}")
```

### Comparing `deskAssistant-0.0.6/deskAssistant.egg-info/PKG-INFO` & `deskAssistant-0.0.7/deskAssistant.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 Metadata-Version: 2.1
 Name: deskAssistant
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to help with making a virtual assistant
-Home-page: UNKNOWN
 Author: Blinken77YT
 Author-email: theonilsson2012@icloud.com
-License: UNKNOWN
 Keywords: python,virtual,assistant,assistant virtual,virtual assistant
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-
-UNKNOWN
-
```

### Comparing `deskAssistant-0.0.6/setup.py` & `deskAssistant-0.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from setuptools import setup, find_packages
-import codecs
-import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'A package to help with making a virtual assistant'
 
 # Setting up
 setup(
     name="deskAssistant",
     version=VERSION,
     author="Blinken77YT",
```

