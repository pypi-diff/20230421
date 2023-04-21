# Comparing `tmp/Turk_game-1.0.1.tar.gz` & `tmp/Turk_game-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Turk_game-1.0.1.tar", last modified: Sun Apr 16 11:19:40 2023, max compression
+gzip compressed data, was "Turk_game-1.0.2.tar", last modified: Fri Apr 21 10:30:15 2023, max compression
```

## Comparing `Turk_game-1.0.1.tar` & `Turk_game-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 11:19:40.000000 Turk_game-1.0.1/
--rw-rw-rw-   0        0        0     1066 2019-06-03 23:39:34.000000 Turk_game-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      278 2023-04-16 11:19:42.000000 Turk_game-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2033 2019-06-03 23:39:34.000000 Turk_game-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 11:19:40.000000 Turk_game-1.0.1/Turk_game.egg-info/
--rw-rw-rw-   0        0        0      278 2023-04-16 11:19:40.000000 Turk_game-1.0.1/Turk_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-04-16 11:19:40.000000 Turk_game-1.0.1/Turk_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 11:19:40.000000 Turk_game-1.0.1/Turk_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 11:19:40.000000 Turk_game-1.0.1/Turk_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2553 2023-04-16 11:14:42.000000 Turk_game-1.0.1/Turk_game.py
--rw-rw-rw-   0        0        0       10 2023-04-11 06:37:16.000000 Turk_game-1.0.1/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-16 11:19:42.000000 Turk_game-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-04-16 11:19:32.000000 Turk_game-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 10:30:14.000000 Turk_game-1.0.2/
+-rw-rw-rw-   0        0        0     1066 2019-06-03 23:39:34.000000 Turk_game-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      278 2023-04-21 10:30:16.000000 Turk_game-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2033 2019-06-03 23:39:34.000000 Turk_game-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 10:30:14.000000 Turk_game-1.0.2/Turk_game.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-04-21 10:30:14.000000 Turk_game-1.0.2/Turk_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-04-21 10:30:14.000000 Turk_game-1.0.2/Turk_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 10:30:14.000000 Turk_game-1.0.2/Turk_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 10:30:14.000000 Turk_game-1.0.2/Turk_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2698 2023-04-21 10:17:56.000000 Turk_game-1.0.2/Turk_game.py
+-rw-rw-rw-   0        0        0       10 2023-04-11 06:37:16.000000 Turk_game-1.0.2/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 10:30:16.000000 Turk_game-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      425 2023-04-21 10:30:08.000000 Turk_game-1.0.2/setup.py
```

### Comparing `Turk_game-1.0.1/LICENSE` & `Turk_game-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Turk_game-1.0.1/README.md` & `Turk_game-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Turk_game-1.0.1/Turk_game.py` & `Turk_game-1.0.2/Turk_game.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 import pygame as pg
 import threading as th
-import sys, os
+import keyboard as ky
+import sys, os , time
+
+def bekle(sure):
+    time.sleep(sure)
+
+def basildi(tus:str):
+    return ky.is_pressed(tus)
+
+
 
 
 def carpma_listesi(nesne,diger):
+
     x = nesne.collidelist(diger)
     if x != -1:
         return 1
-    else:
-        return 0 
+    else:    
+        return 0
+
 
 
 
 def dikdortgen_carp(nesne,diger):
+    
     return pg.Rect.colliderect(nesne,diger)
 
 
 def ses_yukle(ses):
     pg.mixer.music.load(ses)
 
 
 
-def ses_cal(ses):
+def ses_cal():
     pg.mixer.music.play()
 
 
 def s_duraklat():
     pg.mixer.music.pause()
 
 
@@ -54,58 +66,53 @@
         self.rect = pg.rect.Rect(ozellik[0:2],ozellik[2:])
 
 
 
 class Turk_resim:
     def __init__(self,resim,boyut:list):
         self.resim = pg.transform.scale(pg.image.load(resim),boyut)
+    def guncelle(self,resim,boyut:list):
+        self.resim = pg.transform.scale(pg.image.load(resim),boyut)
         
 
     
 class EKRAN:
-    def __init__(self,x:int,y:int,baslik:str,ikon:str,normal_islem,event_islem,kapandi_islem,yenileme_cesidi):
+    def __init__(self,x:int,y:int,baslik:str,ikon:str):
         if not ikon == "":
             self.ikon = pg.transform.scale(pg.image.load(ikon),(320,320))
             pg.display.set_icon(self.ikon)
         pg.display.set_caption(str(baslik))
         self.___ekran___ = pg.display.set_mode((x,y))
         self.running = True  # running özelliğini tanımla
-        self.dongu(normal_islem,event_islem,kapandi_islem)
+        #self.dongu(normal_islem,event_islem,kapandi_islem,yenileme_cesidi)
 
     def yerlestir(self,nesne):
         if type(nesne[0]) == Turk_resim:
             self.___ekran___.blit(nesne[0].resim,(nesne[1],nesne[2]))
         else:
             self.___ekran___.blit(nesne[0],(nesne[1],nesne[2]))
 
     def ciz(self,nesne:Turk_rect,renk):
-        pg.draw.rect(self.ekran,renk,nesne.rect)
+        pg.draw.rect(self.___ekran___,renk,nesne.rect)
 
     def update(self):
         pg.display.update()
 
     def flip(self):
         pg.display.flip()
         
     def dongu(self,normal_islem,event_islem,kapandi_islem,yenileme_cesidi):
-        global i
+        self.running = True
         while self.running:  # self.running özelliğini kullan
             self.events = pg.event.get()
             for self.event in self.events:
                 if self.event.type == pg.QUIT:
                     kapandi_islem()
                     self.running = False
 
                 event_islem()
             
             normal_islem()
             yenileme_cesidi()
 
         pg.quit()
-        sys.exit()
-
-
-"""
-a = EKRAN(200,200,"","",False)
-a.dongu([],[],[],pg.display.update)
-"""
-
+        sys.exit()
```

