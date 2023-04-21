# Comparing `tmp/likeprocessing-0.1.7.2.4.tar.gz` & `tmp/likeprocessing-0.1.7.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "likeprocessing-0.1.7.2.4.tar", max compression
+gzip compressed data, was "likeprocessing-0.1.7.2.5.tar", max compression
```

## Comparing `likeprocessing-0.1.7.2.4.tar` & `likeprocessing-0.1.7.2.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     6615 2022-12-28 17:02:23.278570 likeprocessing-0.1.7.2.4/likeprocessing/affichage.py
--rw-r--r--   0        0        0    28492 2023-03-13 18:39:09.473700 likeprocessing-0.1.7.2.4/likeprocessing/bloc2D.py
--rw-r--r--   0        0        0     1322 2022-12-28 17:02:23.280566 likeprocessing-0.1.7.2.4/likeprocessing/error.png
--rw-r--r--   0        0        0       38 2022-12-28 17:02:23.281566 likeprocessing-0.1.7.2.4/likeprocessing/exceptions.py
--rw-r--r--   0        0        0    26713 2023-04-14 19:30:22.656752 likeprocessing-0.1.7.2.4/likeprocessing/formes.py
--rw-r--r--   0        0        0    14488 2022-12-28 17:02:23.285565 likeprocessing-0.1.7.2.4/likeprocessing/images/image1.png
--rw-r--r--   0        0        0     6467 2023-04-03 18:49:11.495979 likeprocessing-0.1.7.2.4/likeprocessing/images/image10.png
--rw-r--r--   0        0        0     4165 2022-12-28 17:02:23.286568 likeprocessing-0.1.7.2.4/likeprocessing/images/image2.png
--rw-r--r--   0        0        0     8127 2023-04-03 18:30:37.712411 likeprocessing-0.1.7.2.4/likeprocessing/images/image3.png
--rw-r--r--   0        0        0     7330 2023-04-03 18:34:03.727970 likeprocessing-0.1.7.2.4/likeprocessing/images/image4.png
--rw-r--r--   0        0        0     7973 2023-04-03 18:38:30.742802 likeprocessing-0.1.7.2.4/likeprocessing/images/image5.png
--rw-r--r--   0        0        0     4547 2023-04-03 18:39:47.603042 likeprocessing-0.1.7.2.4/likeprocessing/images/image6.png
--rw-r--r--   0        0        0     4446 2023-04-03 18:40:53.103385 likeprocessing-0.1.7.2.4/likeprocessing/images/image7.png
--rw-r--r--   0        0        0     5664 2023-04-03 18:41:25.752657 likeprocessing-0.1.7.2.4/likeprocessing/images/image8.png
--rw-r--r--   0        0        0     6670 2023-04-03 18:42:48.561996 likeprocessing-0.1.7.2.4/likeprocessing/images/image9.png
--rw-r--r--   0        0        0     2712 2023-04-02 13:03:30.812517 likeprocessing-0.1.7.2.4/likeprocessing/images.py
--rw-r--r--   0        0        0     1407 2022-12-28 17:02:23.289572 likeprocessing-0.1.7.2.4/likeprocessing/info.png
--rw-r--r--   0        0        0     1553 2023-01-31 15:21:36.320000 likeprocessing-0.1.7.2.4/likeprocessing/jauge.py
--rw-r--r--   0        0        0      617 2022-12-28 17:02:23.291567 likeprocessing-0.1.7.2.4/likeprocessing/list_tools.py
--rw-r--r--   0        0        0     2972 2022-12-28 17:02:23.292567 likeprocessing-0.1.7.2.4/likeprocessing/print_vars.py
--rw-r--r--   0        0        0    16165 2023-04-03 17:56:31.860717 likeprocessing-0.1.7.2.4/likeprocessing/processing.py
--rw-r--r--   0        0        0   106987 2023-04-15 09:56:32.995869 likeprocessing-0.1.7.2.4/likeprocessing/pyDialog.py
--rw-r--r--   0        0        0    12642 2023-04-02 15:15:57.364975 likeprocessing-0.1.7.2.4/likeprocessing/pygame_textinput.py
--rw-r--r--   0        0        0     1399 2022-12-28 17:02:23.296567 likeprocessing-0.1.7.2.4/likeprocessing/question.png
--rw-r--r--   0        0        0    32847 2023-04-10 20:17:08.347239 likeprocessing-0.1.7.2.4/likeprocessing/README.md
--rw-r--r--   0        0        0     4005 2023-04-03 18:18:51.538032 likeprocessing-0.1.7.2.4/likeprocessing/tempos.py
--rw-r--r--   0        0        0     4702 2023-03-11 18:15:23.243113 likeprocessing-0.1.7.2.4/likeprocessing/texte.py
--rw-r--r--   0        0        0     1768 2023-03-22 16:49:01.809515 likeprocessing-0.1.7.2.4/likeprocessing/tor.py
--rw-r--r--   0        0        0     4351 2023-04-05 17:28:13.480285 likeprocessing-0.1.7.2.4/likeprocessing/transformation.py
--rw-r--r--   0        0        0     4065 2022-12-28 17:02:23.303567 likeprocessing-0.1.7.2.4/likeprocessing/trigo.py
--rw-r--r--   0        0        0      720 2022-12-28 17:02:23.304568 likeprocessing-0.1.7.2.4/likeprocessing/warning.png
--rw-r--r--   0        0        0      399 2023-04-15 10:26:35.272439 likeprocessing-0.1.7.2.4/pyproject.toml
--rw-r--r--   0        0        0    33653 2023-04-15 10:26:57.744090 likeprocessing-0.1.7.2.4/setup.py
--rw-r--r--   0        0        0    31967 2023-04-15 10:26:57.745089 likeprocessing-0.1.7.2.4/PKG-INFO
+-rw-r--r--   0        0        0     6615 2022-12-28 17:02:23.278570 likeprocessing-0.1.7.2.5/likeprocessing/affichage.py
+-rw-r--r--   0        0        0    28492 2023-04-21 06:47:40.260173 likeprocessing-0.1.7.2.5/likeprocessing/bloc2D.py
+-rw-r--r--   0        0        0     1322 2022-12-28 17:02:23.280566 likeprocessing-0.1.7.2.5/likeprocessing/error.png
+-rw-r--r--   0        0        0       38 2022-12-28 17:02:23.281566 likeprocessing-0.1.7.2.5/likeprocessing/exceptions.py
+-rw-r--r--   0        0        0    27812 2023-04-21 07:29:27.522481 likeprocessing-0.1.7.2.5/likeprocessing/formes.py
+-rw-r--r--   0        0        0    14488 2023-04-21 06:47:40.263169 likeprocessing-0.1.7.2.5/likeprocessing/images/image1.png
+-rw-r--r--   0        0        0     6467 2023-04-21 06:47:40.264159 likeprocessing-0.1.7.2.5/likeprocessing/images/image10.png
+-rw-r--r--   0        0        0     4165 2023-04-21 06:47:40.264159 likeprocessing-0.1.7.2.5/likeprocessing/images/image2.png
+-rw-r--r--   0        0        0     8127 2023-04-21 06:47:40.265157 likeprocessing-0.1.7.2.5/likeprocessing/images/image3.png
+-rw-r--r--   0        0        0     7330 2023-04-21 06:47:40.265157 likeprocessing-0.1.7.2.5/likeprocessing/images/image4.png
+-rw-r--r--   0        0        0     7973 2023-04-21 06:47:40.266157 likeprocessing-0.1.7.2.5/likeprocessing/images/image5.png
+-rw-r--r--   0        0        0     4547 2023-04-21 06:47:40.266157 likeprocessing-0.1.7.2.5/likeprocessing/images/image6.png
+-rw-r--r--   0        0        0     4446 2023-04-21 06:47:40.267159 likeprocessing-0.1.7.2.5/likeprocessing/images/image7.png
+-rw-r--r--   0        0        0     5664 2023-04-21 06:47:40.267159 likeprocessing-0.1.7.2.5/likeprocessing/images/image8.png
+-rw-r--r--   0        0        0     6670 2023-04-21 06:47:40.268156 likeprocessing-0.1.7.2.5/likeprocessing/images/image9.png
+-rw-r--r--   0        0        0     2712 2023-04-21 06:47:40.262158 likeprocessing-0.1.7.2.5/likeprocessing/images.py
+-rw-r--r--   0        0        0     1407 2022-12-28 17:02:23.289572 likeprocessing-0.1.7.2.5/likeprocessing/info.png
+-rw-r--r--   0        0        0     1553 2023-04-21 06:47:40.268156 likeprocessing-0.1.7.2.5/likeprocessing/jauge.py
+-rw-r--r--   0        0        0      617 2022-12-28 17:02:23.291567 likeprocessing-0.1.7.2.5/likeprocessing/list_tools.py
+-rw-r--r--   0        0        0     2972 2022-12-28 17:02:23.292567 likeprocessing-0.1.7.2.5/likeprocessing/print_vars.py
+-rw-r--r--   0        0        0    16165 2023-04-21 06:47:40.270183 likeprocessing-0.1.7.2.5/likeprocessing/processing.py
+-rw-r--r--   0        0        0   108082 2023-04-21 08:31:02.131734 likeprocessing-0.1.7.2.5/likeprocessing/pyDialog.py
+-rw-r--r--   0        0        0    12642 2023-04-21 06:47:40.273407 likeprocessing-0.1.7.2.5/likeprocessing/pygame_textinput.py
+-rw-r--r--   0        0        0     1399 2022-12-28 17:02:23.296567 likeprocessing-0.1.7.2.5/likeprocessing/question.png
+-rw-r--r--   0        0        0    33151 2023-04-21 07:46:12.574983 likeprocessing-0.1.7.2.5/likeprocessing/README.md
+-rw-r--r--   0        0        0     4005 2023-04-21 06:47:40.273407 likeprocessing-0.1.7.2.5/likeprocessing/tempos.py
+-rw-r--r--   0        0        0     4702 2023-04-21 06:47:40.274429 likeprocessing-0.1.7.2.5/likeprocessing/texte.py
+-rw-r--r--   0        0        0     1768 2023-04-21 06:47:40.274429 likeprocessing-0.1.7.2.5/likeprocessing/tor.py
+-rw-r--r--   0        0        0     4351 2023-04-21 06:47:40.275419 likeprocessing-0.1.7.2.5/likeprocessing/transformation.py
+-rw-r--r--   0        0        0     4065 2022-12-28 17:02:23.303567 likeprocessing-0.1.7.2.5/likeprocessing/trigo.py
+-rw-r--r--   0        0        0      720 2022-12-28 17:02:23.304568 likeprocessing-0.1.7.2.5/likeprocessing/warning.png
+-rw-r--r--   0        0        0      429 2023-04-21 08:19:24.098274 likeprocessing-0.1.7.2.5/pyproject.toml
+-rw-r--r--   0        0        0    33992 2023-04-21 08:31:09.895585 likeprocessing-0.1.7.2.5/setup.py
+-rw-r--r--   0        0        0    32317 2023-04-21 08:31:09.897584 likeprocessing-0.1.7.2.5/PKG-INFO
```

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/affichage.py` & `likeprocessing-0.1.7.2.5/likeprocessing/affichage.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/bloc2D.py` & `likeprocessing-0.1.7.2.5/likeprocessing/bloc2D.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/error.png` & `likeprocessing-0.1.7.2.5/likeprocessing/error.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/formes.py` & `likeprocessing-0.1.7.2.5/likeprocessing/formes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import math
 
 import likeprocessing.processing as processing
 import likeprocessing.trigo as trigo
 import pygame
 
 
-def in_polygone(x, y, points: list) -> bool:
-    """retourne True si le point (x,y) est dans le polygone"""
-    segment = []
-    for i in range(0, len(points) - 1):
-        if (points[i][0] >= x or points[i + 1][0] >= x) and (
-                points[i][1] < y < points[i + 1][1] or points[i][1] > y > points[i + 1][1]):
-            segment.append((points[i], points[i + 1]))
-    if (points[0][0] >= x or points[-1][0] >= x) and (
-            points[0][1] < y < points[-1][1] or points[0][1] > y > points[-1][1]):
-        segment.append((points[0], points[-1]))
-    if len(segment) % 2 == 1:
-        return True
-    else:
-        nb = 0
-        for s in segment:
-            if (s[1][0] - s[0][0]) != 0:
-                a = (s[1][1] - s[0][1]) / (s[1][0] - s[0][0])
-                b = s[1][1] - a * s[1][0]
-                if (y - b) / a >= x:
-                    nb += 1
-            else:
-                nb += 1
-        return nb % 2 == 1
+def in_polygone(x, y, points:list):
+    """
+    Vérifie si un point donné se trouve à l'intérieur d'un polygone donné.
+
+    Args:
+        point (tuple): Les coordonnées du point à tester sous la forme (x, y).
+        points (list): Une liste de tuples contenant les coordonnées des sommets du polygone.
+
+    Returns:
+        bool: True si le point se trouve à l'intérieur du polygone, False sinon.
+    """
+
+    n = len(points)
+    inside = False
+
+    p1x, p1y = points[0]
+    for i in range(1, n+1):
+        p2x, p2y = points[i % n]
+        if y > min(p1y, p2y):
+            if y <= max(p1y, p2y):
+                if x <= max(p1x, p2x):
+                    if p1y != p2y:
+                        x_intersect = (y - p1y) * (p2x - p1x) / (p2y - p1y) + p1x
+                    if p1x == p2x or x <= x_intersect:
+                        inside = not inside
+        p1x, p1y = p2x, p2y
+
+    return inside
 
 
 def in_line(x, y, x1, y1, x2, y2) -> bool:
     """retourne True si la souris est sur le trait"""
     d1 = dist(x, y, x1, y1)
     d2 = dist(x, y, x2, y2)
     d = dist(x1, y1, x2, y2)
@@ -152,14 +157,16 @@
         x, y = processing.transformation([[x + dx, y + dy]])[0]
         processing.screen.blit(img,
                                (x - img.get_width() / 2, y - img.get_height() / 2),
                                (0, 0, img.get_width(), img.get_height()))
         if processing.in_polygone(*processing.mouseXY(), points):
             fill_mouse_on = kwargs.get("fill_mouse_on", processing.__fill_color_mouse_on)
             if fill_mouse_on is not None:
+                if isinstance(fill_mouse_on, str):
+                    fill_mouse_on = processing.rgb_color(fill_mouse_on)
                 fill_mouse_on = list(fill_mouse_on)[:3] + [127]
                 lx, ly = zip(*points)
                 min_x, min_y, max_x, max_y = min(lx), min(ly), max(lx), max(ly)
                 target_rect = pygame.Rect(min_x, min_y, max_x - min_x, max_y - min_y)
                 shape_surf = pygame.Surface(target_rect.size, pygame.SRCALPHA)
                 pygame.draw.polygon(shape_surf, fill_mouse_on, [(x - min_x, y - min_y) for x, y in points])
                 processing.screen.blit(shape_surf, target_rect)
@@ -207,21 +214,27 @@
     points = [(x1, y1), (x2, y2)]
     points = processing.transformation(points)
     stroke_weight = kwargs.get("stroke_weight", processing.__border_width)
     fill_mouse_on = kwargs.get("fill_mouse_on", processing.__fill_color_mouse_on)
     arrow_start = kwargs.get("arrow_start", False)
     arrow_end = kwargs.get("arrow_end", False)
     command = kwargs.get("command", None)
+    command_mouse_over = kwargs.get("command_mouse_over", None)
     name = kwargs.get("name", None)
     if fill_mouse_on is not None and in_line(*processing.mouseXY(), *points[0], *points[1]):
         if processing.mouse_click_down() and command is not None:
             if name is not None:
                 command(name)
             else:
                 command()
+        if command_mouse_over is not None:
+            if name is not None:
+                command_mouse_over(name)
+            else:
+                command_mouse_over()
         stroke = fill_mouse_on
     pygame.draw.line(processing.screen, stroke, *points, stroke_weight)
     if arrow_start:
         angle = trigo.atan2(y2 - y1, x2 - x1)
         r = processing.rotate(-angle, (x1, y1))
         triangle(x1, y1, x1 + 5, y1 - 3, x1 + 5, y1 + 3, fill=stroke, no_fill=False, no_stroke=False)
         processing.rotate(*r)
@@ -269,14 +282,15 @@
     fill = kwargs.get("fill", processing.get_fill_color())
     no_fill = kwargs.get("no_fill", processing.__no_fill)
     stroke = kwargs.get("stroke", processing.__border_color)
     stroke_weight = kwargs.get("stroke_weight", processing.__border_width)
     fill_mouse_on = kwargs.get("fill_mouse_on", processing.__fill_color_mouse_on)
     no_stoke = kwargs.get("no_stroke", False)
     command = kwargs.get("command", None)
+    command_mouse_over = kwargs.get("command_mouse_over", None)
     name = kwargs.get("name", None)
     if processing.__scale != 1:
         largeur *= processing.__scale
         hauteur *= processing.__scale
     if no_stoke is True:
         stroke_weight = 0
     if isinstance(fill, str):
@@ -291,14 +305,19 @@
             if fill_mouse_on is not None and in_ellipse(*processing.mouseXY(), x + largeur / 2,
                                                         y + hauteur / 2, largeur, hauteur):
                 if processing.mouse_click_down() and command is not None:
                     if name is not None:
                         command(name)
                     else:
                         command()
+                if command_mouse_over is not None:
+                    if name is not None:
+                        command_mouse_over(name)
+                    else:
+                        command_mouse_over()
                 pygame.draw.ellipse(processing.screen, fill_mouse_on,
                                     (x + processing.__dx, y + processing.__dy, largeur, hauteur),
                                     0)
             else:
                 pygame.draw.ellipse(processing.screen, fill,
                                     (x + processing.__dx, y + processing.__dy, largeur, hauteur),
                                     0)
@@ -328,14 +347,15 @@
     fill = kwargs.get("fill", processing.get_fill_color())
     no_fill = kwargs.get("no_fill", processing.__no_fill)
     stroke = kwargs.get("stroke", processing.__border_color)
     stroke_weight = kwargs.get("stroke_weight", processing.__border_width)
     fill_mouse_on = kwargs.get("fill_mouse_on", processing.__fill_color_mouse_on)
     no_stoke = kwargs.get("no_stroke", False)
     command = kwargs.get("command", None)
+    command_mouse_over = kwargs.get("command_mouse_over", None)
     name = kwargs.get("name", None)
     if processing.__scale != 1:
         diametre *= processing.__scale
     if no_stoke is True:
         stroke_weight = 0
     if isinstance(fill, str):
         fill = processing.rgb_color(fill)
@@ -356,14 +376,19 @@
         if fill_mouse_on is not None and in_circle(*processing.mouseXY(), x + diametre / 2,
                                                    y + diametre / 2, diametre):
             if processing.mouse_click_down() and command is not None:
                 if name is not None:
                     command(name)
                 else:
                     command()
+            if command_mouse_over is not None:
+                if name is not None:
+                    command_mouse_over(name)
+                else:
+                    command_mouse_over()
             pygame.draw.ellipse(processing.screen, fill_mouse_on,
                                 (x, y, diametre, diametre),
                                 0)
         else:
             pygame.draw.ellipse(processing.screen, fill,
                                 (x, y, diametre, diametre),
                                 0)
@@ -407,14 +432,15 @@
     fill = kwargs.get("fill", processing.get_fill_color())
     no_fill = kwargs.get("no_fill", processing.__no_fill)
     stroke = kwargs.get("stroke", processing.__border_color)
     stroke_weight = kwargs.get("stroke_weight", processing.__border_width)
     fill_mouse_on = kwargs.get("fill_mouse_on", processing.__fill_color_mouse_on)
     no_stroke = kwargs.get("no_stroke", False)
     command = kwargs.get("command", None)
+    command_mouse_over = kwargs.get("command_mouse_over", None)
     name = kwargs.get("name", None)
     click_up = kwargs.get("click_up", False)
     if no_stroke is True:
         stroke_weight = 0
     if isinstance(fill, str):
         fill = processing.rgb_color(fill)
     if no_fill is True:
@@ -431,14 +457,18 @@
                     command()
             if fill_mouse_on is None:
                 pygame.draw.polygon(processing.screen, fill,
                                     points)
             else:
                 pygame.draw.polygon(processing.screen, fill_mouse_on,
                                     points)
+                if name is not None:
+                    command_mouse_over(name)
+                else:
+                    command_mouse_over()
         else:
             pygame.draw.polygon(processing.screen, fill,
                                 points)
         if stroke_weight != 0:
             pygame.draw.polygon(processing.screen, stroke,
                                 points, width=stroke_weight)
```

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images/image1.png` & `likeprocessing-0.1.7.2.5/likeprocessing/images/image1.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images/image10.png` & `likeprocessing-0.1.7.2.5/likeprocessing/images/image10.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images/image2.png` & `likeprocessing-0.1.7.2.5/likeprocessing/images/image2.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images/image3.png` & `likeprocessing-0.1.7.2.5/likeprocessing/images/image3.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images/image4.png` & `likeprocessing-0.1.7.2.5/likeprocessing/images/image4.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images/image5.png` & `likeprocessing-0.1.7.2.5/likeprocessing/images/image5.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images/image6.png` & `likeprocessing-0.1.7.2.5/likeprocessing/images/image6.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images/image7.png` & `likeprocessing-0.1.7.2.5/likeprocessing/images/image7.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images/image8.png` & `likeprocessing-0.1.7.2.5/likeprocessing/images/image8.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images/image9.png` & `likeprocessing-0.1.7.2.5/likeprocessing/images/image9.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/images.py` & `likeprocessing-0.1.7.2.5/likeprocessing/images.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/info.png` & `likeprocessing-0.1.7.2.5/likeprocessing/info.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/jauge.py` & `likeprocessing-0.1.7.2.5/likeprocessing/jauge.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/list_tools.py` & `likeprocessing-0.1.7.2.5/likeprocessing/list_tools.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/print_vars.py` & `likeprocessing-0.1.7.2.5/likeprocessing/print_vars.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/processing.py` & `likeprocessing-0.1.7.2.5/likeprocessing/processing.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/pyDialog.py` & `likeprocessing-0.1.7.2.5/likeprocessing/pyDialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         self._focus = False
         self.name = kwargs.get('name', None)
         self.border_rounded = kwargs.get('border_rounded', 0)
         if kwargs.get('no_fill', False):
             self.fill = None
         if kwargs.get('no_stroke', False):
             self.stroke_weight = 0
-        self._visible = True
+        self._visible = kwargs.get('visible', True)
         # if isinstance(self.parent, Dialog) and self.parent.cadre:
         # if not isinstance(self.parent, pygame.Rect):
         try:
             self.top += self.parent.decy
             pass
         except:
             pass
@@ -1013,14 +1013,17 @@
     def set_text(self, texte: str):
         self.texte.value = str(texte)
         self.texte.update([])
         self.texte.cursor_visible = False
 
 
 class Bouton(Boite):
+    """ TODO Bouton
+    docstring
+    compléter le readme """
     BOUTON_FOND = affichage.rgb_color("white")
     BOUTON_FOND_MOUSE_ON = (200, 241, 251)
     BOUTON_BORD = affichage.rgb_color("gray68")
     BOUTON_BORD_MOUSE_ON = (0, 120, 215)
     BOUTON_FOND_DISABLED = affichage.rgb_color("grey")
     BOUTON_TEXT_COLOR = affichage.rgb_color("black")
     BOUTON_TEXT_COLOR_DISABLED = affichage.rgb_color("grey90")
@@ -1035,14 +1038,18 @@
         elif len(rect) == 3:
             rect = (rect[0], rect[1], rect[2], 0)
         kwargs["align_v"] = kwargs.get("align_v", "center")
         kwargs["align_h"] = kwargs.get("align_h", "center")
         self.filled = kwargs.get("fill", None)
         super().__init__(parent, rect, **kwargs)
         self.fonction = kwargs.get("command", None)
+        cmo = kwargs.get("command_mouse_over", None)
+        if not isinstance(cmo, tuple):
+            cmo = (cmo, None)
+        self.fonction_mouse_over, self.fonction_mouse_over_off = cmo
         self.mouseOn = False
         self.mouseClick = False
         self.texte = MultiLineText(self, (2, 2, self.width - 4, self.height - 4), texte, **kwargs)
         self.height = max(self.height, self.texte.height + 4)
         self.width = max(self.width, self.texte.width + 2 * self.border_rounded + 4)
         self.forced = False
         self.texte.left = self.left + 2
@@ -1065,14 +1072,23 @@
         return self.disabled
 
     @disabled.setter
     def disabled(self, value: bool):
         self.is_disabled = value
         self.texte.disabled = value
 
+    @property
+    def visible(self):
+        return self._visible
+
+    @visible.setter
+    def visible(self, value: bool):
+        self._visible = value
+        self.texte._visible = value
+
     def setX(self, value: int):
         self.x = value
         self.texte.left = self.left + (self.width - self.texte.width) // 2
 
     def setY(self, value: int):
         self.y = value
         self.texte.top = self.top + (self.height - self.texte.height) // 2
@@ -1156,14 +1172,26 @@
             if self.collidepoint(x, y):
                 self.parent.lostFocus()
                 self.mouseOn = True
                 self.focus = True
             else:
                 self.mouseOn = False
                 self.focus = False
+            if self.fonction_mouse_over is not None:
+                if self.mouseOn is True:
+                    if self.name is None:
+                        self.fonction_mouse_over()
+                    else:
+                        self.fonction_mouse_over(self.name)
+                else:
+                    if self.fonction_mouse_over_off is not None:
+                        if self.name is None:
+                            self.fonction_mouse_over_off()
+                        else:
+                            self.fonction_mouse_over_off(self.name)
             if click is False and self.mouseClick is True:
                 self.mouseClick = False
                 if self.mouseOn is True and self.fonction is not None:
                     if self.name is None:
                         self.fonction()
                     else:
                         self.fonction(self.name)
@@ -1201,15 +1229,16 @@
         if self.frame:
             self.cadre = False
             # dialogue type frame
             # self.fill = kwargs["fill"]
             # self.stroke_weight = 0
             kwargs["no_stroke"] = True
             titre = Label(self, (7, 1, 0, 0), kwargs["title"], **kwargs)
-            self.addObjet(Boite(self, (0, titre.height//2, self.width, self.height - titre.h//2), fill=self.fill), "frame_cadre")
+            self.addObjet(Boite(self, (0, titre.height // 2, self.width, self.height - titre.h // 2), fill=self.fill),
+                          "frame_cadre")
             self.addObjet(titre, "frame_title")
             self.decy = self.objet_by_name("frame_title").height + 1
 
         elif self.cadre:
             self.addObjet(
                 Boite(self, (2, 2, self.width - 19, 22), stroke=Dialog.BORD, stroke_weight=1,
                       fill="lightblue"),
@@ -1289,15 +1318,15 @@
             self.objet['frame_cadre'].width = self.width
         self.repack()
 
     def setHeight(self, value: int):
         """modifie la hauteur de la boite de dialogue"""
         self.height = value
         if self.frame:
-            self.objet['frame_cadre'].height = self.height - self.objet["frame_title"].height//2
+            self.objet['frame_cadre'].height = self.height - self.objet["frame_title"].height // 2
         self.repack()
 
     def repack(self):
         """réordonne les objets d'une boite de dialogue
         après un redimensionnement par exemple"""
         if len(self.pack_list) == 1:
             self.pack(self.pack_list[0])
@@ -1515,15 +1544,15 @@
             if not is_ihm:
                 # gestion boite de dialogue
                 if click:
                     self.lostFocus()
                     self.objet_focus = False
                 else:
                     self.start_drop = None
-            #t
+            # t
             mouse_on_dialog = False
             for o in self.objet.values():
                 if o.visible:
                     # gestion de boite de dialogue enfant de ihm
                     if isinstance(self, IhmScreen) and isinstance(o, Dialog):
 
                         if o.collidepoint(x, y) or o.start_drop is not None:
@@ -1538,20 +1567,20 @@
                             o.focus = False
                         if o.modale:
                             modale = True
                             break
             if not self.modale and mouse_on_dialog is False:
                 # try:
                 objets = list(self.objet.keys())
-                #test
+                # test
                 # fin test
                 for k in objets:
                     o: Boite = self.objet.get(k)
                     if o is not None and o.visible:
-                        if isinstance(o,Dialog) and o.collidepoint(x,y):
+                        if isinstance(o, Dialog) and o.collidepoint(x, y):
                             mouse_on_dialog = True
                         if o == self.objet.get('title_box') and (
                                 o.collidepoint(x, y) or self.start_drop is not None) and click:
                             # déplacement de la boite de dialogue
                             if self.start_drop is None:
                                 self.start_drop = (self.x - x, self.y - y)
                             else:
@@ -1749,14 +1778,15 @@
         self.lostFocus()
         self.objet_by_name(object_name).focus = True
 
     def close_modale(self, object_name):
         self.modale = False
         self.objet_by_name(object_name).visible = False
 
+
 class Painter(Boite):
     """Crée une boite de dessin qui pourra se placer dans un boite de dialogue
     afin de pouvoir utiliser les fonctions forme de likeprocessing en surchargeant la méthode
     draw_paint de Paint.
     Exemple d'utilisation:
     ihm = IhmScreen()
 
@@ -1783,21 +1813,22 @@
 
     def __init__(self, parent, rect):
         super().__init__(parent, rect)
 
     def draw(self):
         super().draw()
         pos = processing.translate(self.absolute().x, self.absolute().y)
-        self.draw_paint(self)
+        self.draw_paint()
         processing.init_translate(*pos)
 
     @staticmethod
     def draw_paint(self):
         pass
 
+
 class ListRadio(Dialog):
     def __init__(self, parent, rect, list_items: list, **kwargs):
         """cette classe permet de créer une frame avec des boutons radios.
         parent: IhmScreen ou dialog
         rect: taille de la boite : tuple(int,int,int,int)
         list_items : list[str] liste des noms des boutons radios
         paramètres facultatifs:
```

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/pygame_textinput.py` & `likeprocessing-0.1.7.2.5/likeprocessing/pygame_textinput.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/question.png` & `likeprocessing-0.1.7.2.5/likeprocessing/question.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/README.md` & `likeprocessing-0.1.7.2.5/likeprocessing/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -436,26 +436,29 @@
 ```
 triangle(20, 10, 50, 15, 40, 70, fill = "green", fill_mouse_on="yellow", stroke_weight=3)
 rect(10,100,100,50,fill = "red", image=loadImage("image.jpg")) # rectangle avec une image
 rect(150,100,100,60,fill= "blue",border_rounded = 10) # rectangle au coins arrondis avec un rayon de 10px 
 ```
 
 
-l'ajout de **command = ma_fonction** au paramètre **fill_mouse_on="couleur"** permet d'exécuter la fonction **ma_fonction()**. Si l'on veut attribuer **ma_fonction** à plusieurs formes il est possible d'ajouter le paramètre **name = valeur**. Dans ce cas, la fonction **ma_fonction(name)** sera exécutée . Il faudra créer impérativement soit : 
+l'ajout de **command = ma_fonction** ou **command_mouse_over = ma_fonction** au paramètre **fill_mouse_on="couleur"** permet d'exécuter la fonction **ma_fonction()**. Si l'on veut attribuer **ma_fonction** à plusieurs formes il est possible d'ajouter le paramètre **name = valeur**. Dans ce cas, la fonction **ma_fonction(name)** sera exécutée . Il faudra créer impérativement soit : 
 
 def ma_fonction():
 
     pass
 
 ou
 
 def ma_fonction(nom):
 
     pass
 
+Remarque:<br>
+avec le paramètre command exécute la fonction si la forme est cliquée alors qu'avec command_mous_over elle sera exécutée simplement si la souris est sur la forme.<br>
+Si les deux paramètres sont présents les deux fonctions sont exécutées.
 
 ## Textes
 
 
 <table>
   <tr>
    <td><strong>fonctions</strong>
@@ -1291,10 +1294,10 @@
 ihm.addObjet(Bouton(ihm, (0, 0, 100, 0), "Quitter",
                    font_size=20, command=bp_quitter), "bp_quitter")
 ```
 
 
  
 
-**Remarque **: on peut rendre si nécessaire la croix de la fenêtre likeprocessing inactive avec la fonction  **disabled_quit_cross(). **La fonction** enabled_quit_cross()** permet de la réactivée.
+**Remarque**: on peut rendre si nécessaire la croix de la fenêtre likeprocessing inactive avec la fonction  **disabled_quit_cross(). **La fonction** enabled_quit_cross()** permet de la réactivée.
```

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/tempos.py` & `likeprocessing-0.1.7.2.5/likeprocessing/tempos.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/texte.py` & `likeprocessing-0.1.7.2.5/likeprocessing/texte.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/tor.py` & `likeprocessing-0.1.7.2.5/likeprocessing/tor.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/transformation.py` & `likeprocessing-0.1.7.2.5/likeprocessing/transformation.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/trigo.py` & `likeprocessing-0.1.7.2.5/likeprocessing/trigo.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/likeprocessing/warning.png` & `likeprocessing-0.1.7.2.5/likeprocessing/warning.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.2.4/setup.py` & `likeprocessing-0.1.7.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['likeprocessing']
 
 package_data = \
 {'': ['*'], 'likeprocessing': ['images/*']}
 
 install_requires = \
-['pygame>=2.1.2,<3.0.0']
+['pygame>=2.1.2,<3.0.0', 'pygame_textinput>=1.0.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'likeprocessing',
-    'version': '0.1.7.2.4',
+    'version': '0.1.7.2.5',
     'description': 'Like processing library with pygame',
-    'long_description': '\n## Structure du programme \n\n\n### Installation:\n\n**Dans pycharm :** \\\nCTRL+ALT+s, puis choisir project -> python interpreter et + puis likeprocessing\n\n**dans le terminal :** \\\npip install likeprocessing\n\n\n### Les fonctions setup(), draw() et run(globals())\n\nLe programme doit contenir deux fonctions, setup() et draw(), et l\'exécution est lancée à l\'aide de l\'instruction run(globals()).\n\nLorsque l\'on exécute l\'instruction run(globals()), la fonction setup() est exécutée une fois :\n\n\n```\nfrom likeprocessing.processing import *\ndef setup():\n    createCanvas(800,600)\n    # instructions de paramétrage de l\'affichage\n```\n\n\nCette fonction permet de définir les dimensions de la fenêtre de tracé, et quelques paramètres initiaux. Les valeurs données aux paramètres de la fonction **createCanvas() ** sont affectées automatiquement à deux variables systèmes : **width** pour le premier paramètre et **height** pour le second. Un troisième paramètre **resizable** optionnel permet d\'offrir la possibilité de redimensionner la fenêtre avec la souris  On peut récupérer les valeurs de **width** et **height** grâce au fonction **width()** et **height()**\n\nPuis la fonction **draw()** est ensuite exécutée en boucle, après l\'exécution de **setup()**:\n\n\n```\ndef draw():\n    # instructions de dessin\n```\n\n\nElle contient des instructions qui seront exécutées avec une fréquence réglable, permettant de modifier le contenu de la fenêtre et de créer des contenus statiques ou des animations.\n\nL\'instruction **stop()** met fin à l\'exécution de la boucle :\n\n\n```\ndef compute():\n    # instructions de calcul\n```\n\n\nCette fonction n\'est pas obligatoire. Elle permet d\'éviter de trop surcharger la fonction **draw()** en réservant celle-ci aux instructions de dessins. La fonction **compute()** si elle existe est insérée dans la boucle et est exécutée avant la fonction **draw()** \n\n\n## Structure de base :\n\n\n```\nfrom likeprocessing.processing import *\n\ndef setup():\n   createCanvas(400,200)\n   background("grey")\n\ndef draw():\n   pass\n\nrun(globals())\n```\n\n\n\n## Fonctions système\n\n\n<table>\n  <tr>\n   <td><strong>Fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>width(), height()\n   </td>\n   <td>Dimensions de la zone de dessin. Les valeurs de width et height sont définies par les paramètres de la fonction createCanvas().\n   </td>\n  </tr>\n  <tr>\n   <td>createCanvas()\n   </td>\n   <td> La fonction createCanvas(largeur,hauteur) permet de dimensionner la fenêtre de l\'application. En plus de la largeur et de la hauteur on peut ajouter un troisieme paramètre à True pour que la fenêtre puisse être redimensionnée. (ex createCanvas(400,300,True).\n     <BR>On peut aussi changer l\'icone de la fenêtre avec le paramètre facultatif icone :<br>\n     createCanvas(400,300,True,icone="image.png")  \n   </td>\n  </tr>\n  <tr>\n   <td>title("mon titre")\n   </td>\n   <td> La fonction title("mon titre") permet de changer le titre de la fenêtre par mon titre\n   </td>\n  </tr>\n  <tr>\n   <td>set_icone("icone.jpg")\n   </td>\n   <td> La fonction set_icone() permet de changer l\'icône de la fenêtre\n   </td>\n  </tr>\n</table>\n\n\n\n## Rafraîchissement\n\n\n<table>\n  <tr>\n   <td><strong>Fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>frameCount()\n   </td>\n   <td>Nombre d\'images affichées depuis le démarrage du programme.\n   </td>\n  </tr>\n  <tr>\n   <td>frameRate() \\\ngetFrameRate()\n   </td>\n   <td>Renvoie le nombre d\'images affichées chaque seconde.\n   </td>\n  </tr>\n  <tr>\n   <td>frameRate(valeur) \\\nsetFrameRate(valeur)\n   </td>\n   <td>Spécifie le nombre d\'images à afficher chaque seconde.\n   </td>\n  </tr>\n  <tr>\n   <td>noLoop()\n   </td>\n   <td>Si cette instruction est présente dans la fonction setup la fonction draw sera exécutée une seule fois. Si cette instruction est présente dans la fonction draw, les instructions de la fonction draw en cours sont exécutées (il n\'y a pas d\'interruption) mais celle-ci ne sera pas appelée à nouveau.\n   </td>\n  </tr>\n  <tr>\n   <td>loop()\n   </td>\n   <td>Relance l\'exécution en boucle de draw().\n   </td>\n  </tr>\n</table>\n\n\n\n## Couleurs\n\n\n## Désigner une couleur\n\n\n<table>\n  <tr>\n   <td><strong>syntaxe</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>\'red\'\n   </td>\n   <td>nom de couleur\n   </td>\n  </tr>\n  <tr>\n   <td>120\n   </td>\n   <td>niveau de gris : 0 - 255\n   </td>\n  </tr>\n  <tr>\n   <td>(100, 125, 255)\n   </td>\n   <td>couleur r, v, b (décimal) : 0 - 255\n   </td>\n  </tr>\n  <tr>\n   <td>\'#2aff95\'\n   </td>\n   <td>couleur r, v, b (hexadécimal) : 00 - ff\n   </td>\n  </tr>\n</table>\n\n\n\n## Dessiner en couleur\n\n\n<table>\n  <tr>\n   <td><strong>Fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>background(couleur)\n   </td>\n   <td>Définit la couleur d\'arrière-plan de la zone de dessin (255 par défaut).\n   </td>\n  </tr>\n  <tr>\n   <td>set_background_image(image: Image)\n   </td>\n   <td>Définit l\'image d\'arrière-plan de la zone de dessin.\n   </td>\n  </tr>\n  <tr>\n   <td>get_background_image()\n   </td>\n   <td>Récupère l\'image d\'arrière-plan de la zone de dessin.\n   </td>\n  </tr>\n  <tr>\n   <td>save_background():\n   </td>\n   <td>fait une copie du contenu de la fenêtre et le sauvegarde dans l\'image d\'arrière plan.\n   </td>\n  </tr>\n  <tr>\n   <td>fill(couleur=None)\n   </td>\n   <td>Définit la couleur de remplissage des formes (255 par défaut) et réactive le remplissage des formes. Sans paramètre seul le remplissage est activé (utile après un noFill()). Retourne la valeur précédente du remplissage.\n   </td>\n  </tr>\n  <tr>\n   <td>fill_mouse_on(couleur: any):\n   </td>\n   <td>initialise la couleur de fond des figures qui affichera quand la souris est dessus.\n   </td>\n  </tr>\n  <tr>\n   <td>get_fill()\n   </td>\n   <td>Retourne la couleur de fond actuelle\n   </td>\n  </tr>\n  <tr>\n   <td>noFill()\n   </td>\n   <td>Désactive la couleur de remplissage.\n   </td>\n  </tr>\n  <tr>\n   <td>stroke(couleur)\n   </td>\n   <td>Définit la couleur du tracé des bords des formes et des lignes("black" par défaut). Retourne la valeur précédente de la couleur.\n   </td>\n  </tr>\n  <tr>\n   <td>get_stroke()\n   </td>\n   <td>retourne la couleur des bords actuelle\n   </td>\n  </tr>\n  <tr>\n   <td>noStroke()\n   </td>\n   <td>Désactive le tracé du contour des figures. Retourne la valeur précédente de la couleur.\n   </td>\n  </tr>\n  <tr>\n   <td>save_fill_stroke()\n   </td>\n   <td>Sauvegarde les paramètres fill et stroke\n   </td>\n  </tr>\n  <tr>\n   <td>restore_fill_stroke()\n   </td>\n   <td>recharge les paramètres fill et stroke précédemment sauvegardé avec <strong>save_fill_stroke</strong>\n   </td>\n  </tr>\n</table>\n\n\nSi **noFill()** et **noStroke() **sont exécutées en même temps, rien n\'est tracé dans la zone de dessin.\n\n\n## Formes\n\n\n### Primitives 2d\n\nL\'origine du repère est située en haut à gauche. Les abscisses augmentent de gauche à droite, les ordonnées augmentent de haut en bas.\n\n\n\n![](./images/image1.png)\n\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>point(x, y)\n   </td>\n   <td>Trace un point de coordonnées (x, y). carré de 2x2 pixels\n   </td>\n  </tr>\n  <tr>\n   <td>line(x1, y1, x2, y2)\n   </td>\n   <td>Trace un segment reliant les deux points de coordonnées (x1, y1) et (x2, y2).\n   </td>\n  </tr>\n  <tr>\n   <td>ellipse(x, y, largeur, hauteur)\n   </td>\n   <td>Tracer une ellipse dont le centre a pour coordonnées (x, y) et dont la largeur et la hauteur prennent les valeurs fixées.\n   </td>\n  </tr>\n  <tr>\n   <td>circle(x, y, diametre)\n   </td>\n   <td>Trace un cercle dont le centre a pour coordonnées (x, y) et dont le diamètre prend la valeur fixée. Idem ellipse((x, y, diametre, diametre)\n   </td>\n  </tr>\n  <tr>\n   <td>arc(x,y,largeur,hauteur,,angleDebut, angleFin)\n   </td>\n   <td>Créer une portion d\'ellipse type part de tarte qui pourra être rempli entre les points repérés par les angles angleDébut et angleFin (unité courante). x et y sont les coordonnées du centre du cercle.  \n   </td>\n  </tr>\n  <tr>\n   <td>circle_arc(x,y,rayon,angleDebut, angleFin)\n   </td>\n   <td>idem arc mais à partir d\'un disque\n   </td>\n  </tr>\n  <tr>\n   <td>ellipseMode(corners_center: str)\n   </td>\n   <td>Définie la position des points x et y des fonctions basées sur ellipse. par défaut : "corners" x et y sont les coordonnées du point en haut à gauche du rectangle dans lequel est inscrit l\'ellipse. si les paramètre est "center" x et y représente le centre du rectangle. Retourne la valeur précédente du mode.\n   </td>\n  </tr>\n  <tr>\n   <td>rect(x, y, largeur, hauteur)\n   </td>\n   <td>Créer un rectangle aux coordonnées x,y de largeur largeur et de hauteur. Si rectMode(\'center\') x et y sont les coordonnées du centre du rectangle. Si rectMode(\'corners\') x,y sont les coordonnées du coin haut gauche. Le rectangle est rempli par la couleur définie par fill(couleur). Si le paramètre image est renseigné (image= ...) le fond du rectangle sera occupé pas l\'image retaillée aux dimensions du rectangle sauf si largeur et/ou hauteur sont nulles (ou non renseignées). largeur et/ou hauteur seront alors celles de l\'image. Les paramètres <strong>allign_h </strong>(left, center et right) et  <strong>allign_v</strong> (top,center et bottom) permettent d\'aligner l\'image dans un cadre plus grand qu\'elle.\n   </td>\n  </tr>\n  <tr>\n   <td>square(x, y, cote)\n   </td>\n   <td>Trace un carré dont le sommet en haut à gauche a pour coordonnées (x, y) et dont le côté prend la valeur fixée. fonctionnement idem rectangle\n   </td>\n  </tr>\n  <tr>\n   <td>rectMode(corners_center: str)\n   </td>\n   <td>Définie la position des points x et y des fonctions basées sur rect. par défaut : "corners" x et y sont les coordonnées du point en haut à gauche du rectangle. si les paramètre est "center" x et y représente le centre du rectangle. Retourne la valeur précédente du mode.\n   </td>\n  </tr>\n  <tr>\n   <td>triangle(x1, y1, x2, y2, x3, y3)\n   </td>\n   <td>Trace un triangle dont les trois sommets ont pour coordonnées (x1, y1), (x2, y2), et (x3, y3).\n   </td>\n  </tr>\n  <tr>\n   <td>quad(x1, y1, x2, y2, x3, y3, x4, y4)\n   </td>\n   <td>Trace un quadrilatère dont les quatre sommets ont pour coordonnées (x1, y1), (x2, y2), (x3, y3) et (x4, y4).\n   </td>\n  </tr>\n  <tr>\n   <td>k_line(points)\n   </td>\n   <td>trace un ligne brisée à partir d\'une liste de points [[1,2],[5,6],[8,3],.....]. (nb_point = nb_segments + 1)\n   </td>\n  </tr>\n</table>\n\n\n\n### Tracés\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>strokeWeight(epaisseur)\n   </td>\n   <td>Définit l\'épaisseur du tracé en pixels (par défaut : 1 pixel). Retourne la valeur précédente de la largeur du trait\n   </td>\n  </tr>\n  <tr>\n   <td>noStroke()\n   </td>\n   <td>Désactive le tracé du contour des figures en mettant la largeur du bord à 0. Retourne la valeur précédente de la largeur.\n   </td>\n  </tr>\n  <tr>\n   <td>stroke(couleur)\n   </td>\n   <td>Définit la couleur du tracé des bords des formes et des lignes ("black" par défaut). Si aucune valeur n\'est passée, celle-ci retourne la couleur actuelle. Retourne la valeur précédente de la couleur.\n   </td>\n  </tr>\n</table>\n\n\n\n## Paramètres optionnels:\n\nLes paramètres optionnels sont passés directement dans la fonction et ne concernent que celle-ci: \n\nfill, no_fill, fill_mouse_on, stroke, stroke_weight, command, fill_mousse_on, name. Pour les rectangles nous avons en plus image et border_rounded \n\nexemple :\n\n\n```\ntriangle(20, 10, 50, 15, 40, 70, fill = "green", fill_mouse_on="yellow", stroke_weight=3)\nrect(10,100,100,50,fill = "red", image=loadImage("image.jpg")) # rectangle avec une image\nrect(150,100,100,60,fill= "blue",border_rounded = 10) # rectangle au coins arrondis avec un rayon de 10px \n```\n\n\nl\'ajout de **command = ma_fonction** au paramètre **fill_mouse_on="couleur"** permet d\'exécuter la fonction **ma_fonction()**. Si l\'on veut attribuer **ma_fonction** à plusieurs formes il est possible d\'ajouter le paramètre **name = valeur**. Dans ce cas, la fonction **ma_fonction(name)** sera exécutée . Il faudra créer impérativement soit : \n\ndef ma_fonction():\n\n    pass\n\nou\n\ndef ma_fonction(nom):\n\n    pass\n\n\n## Textes\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>text(chaine, x, y)\n   </td>\n   <td>Affiche la chaîne à la position (x, y) dans une boite ajustée. couleur, largeur bord et couleur bord de la boite idem formes. Accepte les paramètres optionnels\n   </td>\n  </tr>\n  <tr>\n   <td>text(chaine, x, y, largeur, hauteur)\n   </td>\n   <td>Affiche la chaîne à la position (x, y) dans une boite de dimensions largeur x hauteur. couleur, largeur bord et couleur bord de la boite idem formes. largeur et hauteur sont optionnels\n   </td>\n  </tr>\n  <tr>\n   <td>textAlign(alignement_horizontal)\n<p>\ntextAlign(alignement_horizontal, alignement_vertical)\n   </td>\n   <td>Spécifie l\'alignement horizontal parmi LEFT, CENTER, et RIGHT et l\'alignement vertical parmi TOP, BOTTOM, CENTER, et BASELINE\n   </td>\n  </tr>\n  <tr>\n   <td>textFont(police)\n<p>\ntextFont(police, taille)\n   </td>\n   <td>Spécifie la police de caractères et éventuellement sa taille. Retourne la police et la taille précédente \n   </td>\n  </tr>\n  <tr>\n   <td>textSize(taille)\n   </td>\n   <td>Spécifie la taille de la police de caractères. Retourne la taille précédente de la police\n   </td>\n  </tr>\n  <tr>\n   <td>textStyle(style)\n   </td>\n   <td>Spécifie le style parmi NORMAL, ITALIC, BOLD et BOLDITALIC\n   </td>\n  </tr>\n  <tr>\n   <td>textWidth(chaine)\n   </td>\n   <td>Largeur en pixels de l\'affichage de chaîne, dans la police et taille actuelles\n   </td>\n  </tr>\n</table>\n\n\n\n## Paramètres optionnels spécifique à text:\n\nLes paramètres optionnels sont passés directement dans la fonction et ne concernent que celle-ci: \n\nla fonction text possèdes elle aussi des paramètres optionnels qui ne concernent que la fonction en cours : \\\n**font, font_size, font_color** qui permettent  de définir la police, la taille des caractères ainsi que la couleur de ceux-ci. \n\n**allign_h et allign_v** permettent de positionner le texte dans la boîte de texte comme **textAllign()**.\n\n**padx et pady** permettent de créer une marge autour du texte (valeur en pixels)  \\\nexemple : \n\n\n```\ntext("salut les amis",20,30,300,allign_h="center",font="arial",font_size=48,fontTools="green",pady=10)\n```\n\n\nCe code va afficher "salut les amis" dans un cadre de longueur 300 à la position x=20 et y=30. La hauteur du cadre est calculée en fonction de la hauteur du texte (font_size). **pady=10** ajoute 10 pixels au dessus et en dessous du texte. **Si la hauteur du cadre est donnée, si celle-ci est trop petite le texte sortira du cadre.**\n\n\n## Événements\n\n\n### Touches du clavier\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>key()\n   </td>\n   <td>état des touches du clavier (list)\n   </td>\n  </tr>\n  <tr>\n   <td>keyCode()\n   </td>\n   <td>Code de la dernière touche appuyée.\n   </td>\n  </tr>\n  <tr>\n   <td>keyIsPressed()\n<p>\nisKeyPressed()\n   </td>\n   <td>Vaut True lorsqu\'une touche du clavier est appuyée et False sinon.\n   </td>\n  </tr>\n  <tr>\n   <td>keyIsDown(code)\n<p>\nkeyIsDown(touche)\n   </td>\n   <td>Vaut True si la touche concernée est appuyée et False sinon.\n   </td>\n  </tr>\n</table>\n\n\n\n### Souris\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>mouseX(), mouseY()\n   </td>\n   <td>Coordonnées du pointeur de la souris\n   </td>\n  </tr>\n  <tr>\n   <td>mouseXY()\n   </td>\n   <td>Coordonnées du pointeur de la souris sous forme de tuple\n   </td>\n  </tr>\n  <tr>\n   <td>mouseIsPressed()\n   </td>\n   <td>Vaut True si la souris est cliquée, et False sinon.\n   </td>\n  </tr>\n  <tr>\n   <td>fill_mouse_on(couleur:str)\n   </td>\n   <td>Change la couleur des formes quand on passe la souris dessus. Non actif par défaut.\n   </td>\n  </tr>\n  <tr>\n   <td>noFill_mouse_on()\n   </td>\n   <td>annule l\'effet de fill_mouse_on()\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_click_down()\n   </td>\n   <td>renvoie True lors du passage de relâché à appuyé du bouton de la souris.\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_click_up()\n   </td>\n   <td>renvoie True lors du passage de appuyé à relâché du bouton de la souris.\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_click()\n   </td>\n   <td>idem mouseIsPressed()\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_wheel_state()\n   </td>\n   <td>retourne 1 si la roulette de la souris est tournée vers l\'avant, -1 vers l\'arrière et 0 si elle est immobile.\n   </td>\n  </tr>\n</table>\n\n\n\n## Mathématiques\n\n\n### Angles\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>angleMode(mode_angle:str)\n   </td>\n   <td>Définit l\'unité de mesure des angles. \\\n \'rad\' les angles des fonctions trigonométriques seront pris comme des radians (défaut) \\\n \'deg\' les angles des fonctions trigonométriques seront pris comme des degrés \\\n\'grd\' les angles des fonctions trigonométriques seront pris comme des grades \\\nUne exception est levée en cas d\'erreur de paramètre\n<p>\nsi mode_angle == "" la valeur de mode est retournée (str)\n   </td>\n  </tr>\n  <tr>\n   <td>cos(), sin(), tan(), acos(),asin(),atan(),atan2()\n   </td>\n   <td>Fonctions trigonométriques usuelles l\'unité considérée sera celle choisie avec angleMode(). atan2 : même fonctionnement que la fonction math.atan2 mais l\'unité de l\'angle retourné dépend  de angleMode()  \n   </td>\n  </tr>\n  <tr>\n   <td>degrees(mesure) \\\nradians(mesure) \\\ngrades(mesure)\n   </td>\n   <td>Convertit une mesure d\'angle en degrés, en radians ou en grades. l\'unité de mesure dépend de angleMode(). \n   </td>\n  </tr>\n  <tr>\n   <td>HALF_PI, PI, QUARTER_PI, TWO_PI\n   </td>\n   <td>Constantes permettant respectivement d\'approcher les valeurs de π/2, π, π/4, 2π\n   </td>\n  </tr>\n</table>\n\n\n\n### Géométrie\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>dist(x1,y1,x2,y2)\n   </td>\n   <td>retourne la distance entre deux points\n   </td>\n  </tr>\n  <tr>\n   <td>midPoint(x1, y1, x2, y2)\n   </td>\n   <td>retourne le milieu d\'un segment défini par deux points\n   </td>\n  </tr>\n</table>\n\n\n\n## Images\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>loadImage(chemin)\n   </td>\n   <td>Charge une image à partir d\'un chemin et crée un objet Image. Si nécessaire, l\'image peut être préchargée en plaçant l\'appel à la fonction loadImage en debut de programme.\n   </td>\n  </tr>\n  <tr>\n   <td>loadImages((liste_images:list[str],sens=0) ->Image:\n   </td>\n   <td>Retourne une surface qui est l\'assemblage de toutes les images\n    de la liste. Si sens = 1 les images sont assemblées verticalement\n    et horizontalement si sens =0. Ex: loadImages(["image1.png","image2.jpg"])\n   </td>\n  </tr>\n  <tr>\n   <td>background(Image)\n   </td>\n   <td>Affiche une Image en fond d\'écran\n   </td>\n  </tr>\n  <tr>\n   <td>image(image, x, y)\n   </td>\n   <td>Affiche une Image en plaçant le pixel en haut à gauche au point de coordonnées (x, y) dans la zone de dessin.\n   </td>\n  </tr>\n  <tr>\n   <td>copy_image(picture: Image, rect=None) -> Image\n   </td>\n   <td>retourne une copie de picture ou une partie de picture au dimensions de rect\n   </td>\n  </tr>\n  <tr>\n   <td>get_pixel_color(picture: Image, pos: tuple) -> tuple\n   </td>\n   <td>retourne la valeur de la couleur d\'un pixel d\'une image (picture)\n<p>\nsous la forme d\'un tuple\n   </td>\n  </tr>\n  <tr>\n   <td>resize_image(picture:Image,size : tuple\n   </td>\n   <td>retourne une image redimensionné en fonction de size : (largeur,hauteur) \n   </td>\n  </tr>\n</table>\n\n\n\n## Transformations\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>translate(x,y)\n   </td>\n   <td>applique une translation à toutes les fonctions de dessin et d\'image. x et y sont des valeurs relatives qui s\'ajoutent aux translations précédentes.\n<p>\nLa translation est remise à zéro avant chaque exécution de la fonction draw().\n   </td>\n  </tr>\n  <tr>\n   <td>get_translate()\n   </td>\n   <td>retourne la valeur de la translation sous la forme d\'un tuple (x,y)\n   </td>\n  </tr>\n  <tr>\n   <td>init_translate()\n   </td>\n   <td>Force la remise à zéro de la translation. (A utiliser dans la fonction draw() en cas de besoin \n   </td>\n  </tr>\n  <tr>\n   <td>rotate(angle,axis)\n   </td>\n   <td>applique une rotation &lt;angle> par rapport à &lt;axis>. à toutes les fonctions de dessin et d\'image. angle est une valeur absolue. Par défaut axis vaut (0,0). Cette fonction retourne la valeur précédente prise par la fonction sous la forme d\'un tuple.\n   </td>\n  </tr>\n  <tr>\n   <td>flip_h(axe_h)\n   </td>\n   <td>entraîne une symétrie horizontale par rapport à la droite y = axe_h\n   </td>\n  </tr>\n  <tr>\n   <td>flip_v(axe_v)\n   </td>\n   <td>entraîne une symétrie verticale par rapport à la droite x = axe_v\n   </td>\n  </tr>\n</table>\n\n\n\n## Temporisations\n\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>t=Tempo(duree_ms)\n   </td>\n   <td>t=Tempo(1000) créer un objet de temporisation t de durée 1000 ms qui se relance indéfiniment. \n    <img src="./images/image2.png">\n   </td>\n  </tr>\n  <tr>\n   <td>t.fin()\n   </td>\n   <td>renvoie True lorsque la temporisation est terminée. Pour notre exemple au bout de 500 ms.\n   </td>\n  </tr>\n  <tr>\n   <td>t.is_on()\n   </td>\n   <td>renvoie True si la temporisation est à on.\n   </td>\n  </tr>\n  <tr>\n   <td>t.is_off()\n   </td>\n   <td>renvoie True si la temporisation est à off.\n   </td>\n  </tr>\n  <tr>\n   <td>t.set_tempo(duree_ms)\n   </td>\n   <td>permet de réinitialiser la temporisation avec une nouvelle valeur.\n   </td>\n  </tr>\n  <tr>\n   <td>t.reset()\n   </td>\n   <td>force le redémarrage de la temporisation.\n   </td>\n  </tr>\n   <td>t=Monostable(duree_ms)\n   </td>\n   <td>t=Monostable(500) créer un objet de temporisation t de durée 500 ms qui ne se relance qu\'après execution de la methode reset() \n   </td>\n<tr>\n   <td>t=Pwm(500,25) \n    </td>\n    <td>\n    créer un objet générateur de signaux carré de période 500 ms et de rapport cyclique 25% \n   </td>\n  </tr>\n</table>\n\nComme les objets Monostable et Pwm héritent de Tempo ils en possèdent les méthodes.\n\n# Tutoriel Interface homme Machine\n\n\nl’IHM d’un programme permet à l’utilisateur d’interagir avec celui-ci.\n\nEn mode console les instructions print et input permettent de réaliser une interaction sommaire entre le programme et l’utilisateur.\n\nEn mode graphique l’interaction sera plus poussée.\n\n\n## IHM en python avec LikeProcessing\n\n\n### à faire vous même 1\n\nTaper le code suivant dans un nouveau fichier dans votre ide préféré :\n\n\n```\nfrom likeprocessing.processing import *\n\nihm = IhmScreen()\n\ndef setup():\n   createCanvas(400, 200)\n   ihm.init()\n   background("grey")\ndef compute():\nihm.scan_events()\n\n\ndef draw():\nihm.draw()\n\n\nrun(globals())\n```\n\n\nQuand vous exécutez ce code une fenêtre fonctionnelle vide apparaît.\n\n\n## Ajouter des Widgets à l’intérieur de la fenêtre.\n\nNous allons ajouter du texte dans la fenêtre.\n\n\n### à faire vous même 2\n\nAjouter le code suivant :\n\n\n```\netiquette1 = Label(ihm, (10, 10, 0, 0), "notre premier texte")\n```\n\n\n et lancer le programme. Que se passe-t-il ?\n\nMaintenant ajouter\n\n\n```\nihm.addObjet(etiquette1)\n```\n\n\n et lancer le programme. Que se passe-t-il ?\n\nAjouter : \n\n\n```\nihm.pack(["obj_1"])\n\n```\n\n\nQue se passe-t-il ?\n\nEssayer pack(margin_left=10) , pack(margin_right=10)\n\nAjouter une étiquette2 à la fenêtre.\n\n\n```\netiquette2 = Label(ihm, (10, 10, 0, 0), "etiquette2")\nihm.addObjet(etiquette2)\n```\n\n\nOù se place-t-elle sans utiliser **pack** ?\n\nEssayer avec la méthode pack et conclure.\n\nRemarque :\n\non peut utiliser la méthode addObjet en lui passant une liste d\'objet  \n\n\n```\nihm.addObjet([texte,entry, bouton])\n```\n\n\n\n## Interaction des éléments (widget) avec l’utilisateur.\n\nOn souhaite réaliser interface suivante qui contient :\n\n\n\n![](./images/image3.png)\n\nune étiquette (Label) donnant une explication à l’utilisateur, une zone de texte modifiable (LineEdit) et un bouton (Bouton) qui permettra de changer le titre de la fenêtre par le texte entré par l’utilisateur.\n\n\n```\netiquette = Label(ihm, (10, 10, 0, 0), "Modifier le texte et appuyer sur le bouton")\ntexte = LineEdit(ihm,(10,30,100,30),"")\nbouton = Bouton(ihm, (10, 60, 100, 30), "Changer le titre")\nihm.addObjet([etiquette,texte, bouton])\nihm.pack(["obj_1","obj_2","obj_3"])\n```\n\n\nn’oubliez pas d’utiliser les méthode addObjet() et pack()\n\nLorsque vous lancez le programme, que se passe-t-il ?\n\nModifier votre programme en complétant la création du bouton avec :\n\n\n```\ncommand=lambda : title(texte.text())\n```\n\n\ntexte.text() permet de récupérer le texte écrit par l’utilisateur.\n\nlambda permet de définir une fonction sur une ligne (le paramètre **command** à besoin d’une fonction comme valeur). On peut aussi donner le nom d\'une fonction que l\'on aura déjà créé.\n\nTester votre programme et modifier les paramètres de pack() en utilisant expand="x",pady=10,padx=10 pour obtenir la fenêtre ci-dessus (vous pouvez changer la hauteur de la fenêtre).\n\n\n## Précision sur l\'objet IhmScreen\n\nL\'objet IhmScreen possède plusieurs méthodes pour gérer l\'interface graphique:\n\naddObjet permet d\'ajouter des widgets à l\'interface. Si les objets n\'ont pas de nom (paramètre nom non renseigné) la méthode les nomme "obj_1", "obj_2",... \n\nobjet_by_name(nom_objet) permet de récupérer l\'objet de l\'interface pour par exemple changer sa couleur, récupérer la valeur du texte d\'un LineEdit ou changer le **text()** d\'un Label...\n\nEx : \n\n\n```\nihm.addObjet(LineEdit(ihm,(10,30,100,30),""),"texte")\n```\n\n\nCette commande ajoute à l\'interface un champ modifiable qui sera appelé "texte" \n\nprint(ihm.objet_by_name("texte").text()) affichera sur le console la valeur du champ.\n\nOn peut si on le souhaite supprimer un objet : ihm.delObjet(nom_objet) ou simplement le rendre invisible avec ihm.objet_by_name(nom_objet).visible = False\n\n\n## Création d’une calculatrice\n\nOn désire réaliser l’interface suivante :\n\nIl faut créer des boutons pour chaque touche ainsi qu’une étiquette pour simuler l’écran de la calculatrice.\n\n\n```\ntouche = [["1","2","3","*"],\n         ["4","5","6","/"],\n         ["7","8","9","+"],\n         ["0",".","²","-"],\n         ["(",")","=","AC"]]\n\nfor i in range(5):\n   for j in range(4):\n       ihm.addObjet(Bouton(None, (10+.....*40, 50+.....*40, 40, 40), touche[i][j], command=lambda v=touche[i][j]: calcule(v)))\n```\n\n\nla dernière ligne peut être remplacer par :\n\n\n```\nihm.addObjet(Bouton(None, (10+.....*40, 50+.....*40, 40, 40), touche[i][j], command=calcule, name = touche[i][j])) \n```\n\n\nce qui évite d\'utiliser la fonction lambda.\n\nLe paramètre **name** sera envoyé à la fonction **calcule**.\n\n\n### à faire vous même 3\n\ncréer l’IHM de la calculatrice.\n\n\n\n\n\n![](./images/image4.png)\n\n\n### à faire vous même 4\n\nRéalisation de l’interface graphique d\'un logiciel de dessin\n\nOn veut créer l’IHM du logiciel de dessin my_paint dont le code est le suivant:\n\n\n```\nfrom likeprocessing.processing import *\n\nforme = "cercle"\ncouleur = "blue"\npoint1 = None\nfigure = []\n\n\ndef draw_figure():\n   for f in figure:\n       largeur = abs(f[1][0] - f[2][0])\n       hauteur = abs(f[1][1] - f[2][1])\n       if f[0] == "rectangle":\n           rect(*f[1],largeur,hauteur,fill=f[3])\n       elif f[0] == "ligne":\n           line(*f[1],*f[2],stroke=f[3])\n       elif f[0] == "cercle":\n           circle(*f[1],dist(*f[1],*f[2]),fill=f[3],center_mode="center")\n\n\ndef setup():\n   createCanvas(400, 200,True)\n   background("grey")\n   title("my_paint")\n\n\ndef compute():\n   global point1\n   if mouse_click_down():\n       if point1 is None:\n           point1 = mouseXY()\n           figure.append([forme, point1, point1, couleur])\n   if len(figure)>0 and mouseIsPressed():\n       figure[-1][2] = mouseXY()\n   if mouse_click_up():\n       figure[-1][2] = mouseXY()\n       point1 = None\n\n\n\ndef draw():\n   draw_figure()\n\n\nrun(globals())\n```\n\n\nforme peut prendre les valeurs suivantes : "rectangle","cercle","ligne" et couleur les couleurs acceptés par likeprocessing.\n\nl\'interface doit permettre :\n\n- afficher le type de forme en cours\n\n- de changer le type de forme,\n\n- couleur des figures,\n\n- la couleur du fond,\n\n- effacer la dernière forme,\n\n- effacer le dessin,\n\n\n## Utilisation des boîtes de dialogues d\'information (Show)  et des boîtes de dialogues de questionnement (Ask…)\n\nCes boîtes ont un comportement bloquant c\'est à dire que seule l\'interaction avec avec la boite est prise en compte : les fonctions compute(), draw(), exit() ne sont plus appelées.\n\n\n```\nShowInfo(ihm, "Ceci est une \\ninformation").response()\n```\n\n\n\n![](./images/image5.png)\n\n\n```\nShowWarning(ihm, "Ceci est un \\navertissement").response()\n```\n\n\n![](./images/image6.png)\n\n\n\n```\nShowError(ihm, "Ceci est une \\nerreur").response()\n```\n\n\n![](./images/image7.png)\n\n\n\n```\nAskYesNo(ihm, "Voulez-vous Vraiment\\nquitter le jeu").response()\n```\n\n\n\n![](./images/image8.png)\n\n\n\n```\nAskOkCancel(ihm, "Voulez-vous Vraiment\\nquitter le jeu").response()\n```\n\n\n\n![](images/image9.png)\n\n\n\n```\nAskRetriyCancel(ihm, "Voulez-vous tenter\\nà nouveau\\nvotre chance").response()\n```\n\n\n![](./images/image10.png)\n\n\n\n### Utilisation: \n\nles bouton sont numéroté de la gauche vers la droite (0,1) .Le clique sur croix de la boîte retourne la valeur 4 \n\n\n```\nif AskYesNo(ihm, "Voulez-vous tenter\\nà nouveau\\nvotre chance").response() == 0:\n```\n\n\nAvec le code ci-dessus, la condition sera vraie si le bouton de gauche est cliqué. \n\nExemple d\'utilisation d\'une boîte et de la fonction exit().\n\nLa fonction exit() est une fonction facultative (comme compute) destinée à simplifier la sortie du programme que ce soit par l\'intermédiaire d\'un bouton dédié ou par l\'utilisation de la croix de fermeture de la fenêtre.\n\nSans cette fonction lorsque que l\'on appuie sur la croix la fonction **set_quit(True)** est exécutée ce qui à pour effet de fermer immédiatement l\'application.\n\n le code suivant qui utilise la fonction exit() permet de faire les choses avec plus d\'élégance : \n\n\n```\ndef exit():\n   set_quit(False)\n   if AskYesNo(ihm, "Voulez-vous Vraiment\\nquitter le jeu").response() == 0:\n       set_quit(True)\n```\n\n\najout d\'un bouton dédié à la fermeture du programme : \n\n\n```\nihm.addObjet(Bouton(ihm, (0, 0, 100, 0), "Quitter",\n                   font_size=20, command=lambda : set_quit(True) ), bp_quitter")\n```\n\n\nOn peut aussi passer par une fonction intermédiaire:\n\n\n```\ndef bp_quitter():\n   set_quit(True)\n\nihm.addObjet(Bouton(ihm, (0, 0, 100, 0), "Quitter",\n                   font_size=20, command=bp_quitter), "bp_quitter")\n```\n\n\n \n\n**Remarque **: on peut rendre si nécessaire la croix de la fenêtre likeprocessing inactive avec la fonction  **disabled_quit_cross(). **La fonction** enabled_quit_cross()** permet de la réactivée.\n\n \n',
+    'long_description': '\n## Structure du programme \n\n\n### Installation:\n\n**Dans pycharm :** \\\nCTRL+ALT+s, puis choisir project -> python interpreter et + puis likeprocessing\n\n**dans le terminal :** \\\npip install likeprocessing\n\n\n### Les fonctions setup(), draw() et run(globals())\n\nLe programme doit contenir deux fonctions, setup() et draw(), et l\'exécution est lancée à l\'aide de l\'instruction run(globals()).\n\nLorsque l\'on exécute l\'instruction run(globals()), la fonction setup() est exécutée une fois :\n\n\n```\nfrom likeprocessing.processing import *\ndef setup():\n    createCanvas(800,600)\n    # instructions de paramétrage de l\'affichage\n```\n\n\nCette fonction permet de définir les dimensions de la fenêtre de tracé, et quelques paramètres initiaux. Les valeurs données aux paramètres de la fonction **createCanvas() ** sont affectées automatiquement à deux variables systèmes : **width** pour le premier paramètre et **height** pour le second. Un troisième paramètre **resizable** optionnel permet d\'offrir la possibilité de redimensionner la fenêtre avec la souris  On peut récupérer les valeurs de **width** et **height** grâce au fonction **width()** et **height()**\n\nPuis la fonction **draw()** est ensuite exécutée en boucle, après l\'exécution de **setup()**:\n\n\n```\ndef draw():\n    # instructions de dessin\n```\n\n\nElle contient des instructions qui seront exécutées avec une fréquence réglable, permettant de modifier le contenu de la fenêtre et de créer des contenus statiques ou des animations.\n\nL\'instruction **stop()** met fin à l\'exécution de la boucle :\n\n\n```\ndef compute():\n    # instructions de calcul\n```\n\n\nCette fonction n\'est pas obligatoire. Elle permet d\'éviter de trop surcharger la fonction **draw()** en réservant celle-ci aux instructions de dessins. La fonction **compute()** si elle existe est insérée dans la boucle et est exécutée avant la fonction **draw()** \n\n\n## Structure de base :\n\n\n```\nfrom likeprocessing.processing import *\n\ndef setup():\n   createCanvas(400,200)\n   background("grey")\n\ndef draw():\n   pass\n\nrun(globals())\n```\n\n\n\n## Fonctions système\n\n\n<table>\n  <tr>\n   <td><strong>Fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>width(), height()\n   </td>\n   <td>Dimensions de la zone de dessin. Les valeurs de width et height sont définies par les paramètres de la fonction createCanvas().\n   </td>\n  </tr>\n  <tr>\n   <td>createCanvas()\n   </td>\n   <td> La fonction createCanvas(largeur,hauteur) permet de dimensionner la fenêtre de l\'application. En plus de la largeur et de la hauteur on peut ajouter un troisieme paramètre à True pour que la fenêtre puisse être redimensionnée. (ex createCanvas(400,300,True).\n     <BR>On peut aussi changer l\'icone de la fenêtre avec le paramètre facultatif icone :<br>\n     createCanvas(400,300,True,icone="image.png")  \n   </td>\n  </tr>\n  <tr>\n   <td>title("mon titre")\n   </td>\n   <td> La fonction title("mon titre") permet de changer le titre de la fenêtre par mon titre\n   </td>\n  </tr>\n  <tr>\n   <td>set_icone("icone.jpg")\n   </td>\n   <td> La fonction set_icone() permet de changer l\'icône de la fenêtre\n   </td>\n  </tr>\n</table>\n\n\n\n## Rafraîchissement\n\n\n<table>\n  <tr>\n   <td><strong>Fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>frameCount()\n   </td>\n   <td>Nombre d\'images affichées depuis le démarrage du programme.\n   </td>\n  </tr>\n  <tr>\n   <td>frameRate() \\\ngetFrameRate()\n   </td>\n   <td>Renvoie le nombre d\'images affichées chaque seconde.\n   </td>\n  </tr>\n  <tr>\n   <td>frameRate(valeur) \\\nsetFrameRate(valeur)\n   </td>\n   <td>Spécifie le nombre d\'images à afficher chaque seconde.\n   </td>\n  </tr>\n  <tr>\n   <td>noLoop()\n   </td>\n   <td>Si cette instruction est présente dans la fonction setup la fonction draw sera exécutée une seule fois. Si cette instruction est présente dans la fonction draw, les instructions de la fonction draw en cours sont exécutées (il n\'y a pas d\'interruption) mais celle-ci ne sera pas appelée à nouveau.\n   </td>\n  </tr>\n  <tr>\n   <td>loop()\n   </td>\n   <td>Relance l\'exécution en boucle de draw().\n   </td>\n  </tr>\n</table>\n\n\n\n## Couleurs\n\n\n## Désigner une couleur\n\n\n<table>\n  <tr>\n   <td><strong>syntaxe</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>\'red\'\n   </td>\n   <td>nom de couleur\n   </td>\n  </tr>\n  <tr>\n   <td>120\n   </td>\n   <td>niveau de gris : 0 - 255\n   </td>\n  </tr>\n  <tr>\n   <td>(100, 125, 255)\n   </td>\n   <td>couleur r, v, b (décimal) : 0 - 255\n   </td>\n  </tr>\n  <tr>\n   <td>\'#2aff95\'\n   </td>\n   <td>couleur r, v, b (hexadécimal) : 00 - ff\n   </td>\n  </tr>\n</table>\n\n\n\n## Dessiner en couleur\n\n\n<table>\n  <tr>\n   <td><strong>Fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>background(couleur)\n   </td>\n   <td>Définit la couleur d\'arrière-plan de la zone de dessin (255 par défaut).\n   </td>\n  </tr>\n  <tr>\n   <td>set_background_image(image: Image)\n   </td>\n   <td>Définit l\'image d\'arrière-plan de la zone de dessin.\n   </td>\n  </tr>\n  <tr>\n   <td>get_background_image()\n   </td>\n   <td>Récupère l\'image d\'arrière-plan de la zone de dessin.\n   </td>\n  </tr>\n  <tr>\n   <td>save_background():\n   </td>\n   <td>fait une copie du contenu de la fenêtre et le sauvegarde dans l\'image d\'arrière plan.\n   </td>\n  </tr>\n  <tr>\n   <td>fill(couleur=None)\n   </td>\n   <td>Définit la couleur de remplissage des formes (255 par défaut) et réactive le remplissage des formes. Sans paramètre seul le remplissage est activé (utile après un noFill()). Retourne la valeur précédente du remplissage.\n   </td>\n  </tr>\n  <tr>\n   <td>fill_mouse_on(couleur: any):\n   </td>\n   <td>initialise la couleur de fond des figures qui affichera quand la souris est dessus.\n   </td>\n  </tr>\n  <tr>\n   <td>get_fill()\n   </td>\n   <td>Retourne la couleur de fond actuelle\n   </td>\n  </tr>\n  <tr>\n   <td>noFill()\n   </td>\n   <td>Désactive la couleur de remplissage.\n   </td>\n  </tr>\n  <tr>\n   <td>stroke(couleur)\n   </td>\n   <td>Définit la couleur du tracé des bords des formes et des lignes("black" par défaut). Retourne la valeur précédente de la couleur.\n   </td>\n  </tr>\n  <tr>\n   <td>get_stroke()\n   </td>\n   <td>retourne la couleur des bords actuelle\n   </td>\n  </tr>\n  <tr>\n   <td>noStroke()\n   </td>\n   <td>Désactive le tracé du contour des figures. Retourne la valeur précédente de la couleur.\n   </td>\n  </tr>\n  <tr>\n   <td>save_fill_stroke()\n   </td>\n   <td>Sauvegarde les paramètres fill et stroke\n   </td>\n  </tr>\n  <tr>\n   <td>restore_fill_stroke()\n   </td>\n   <td>recharge les paramètres fill et stroke précédemment sauvegardé avec <strong>save_fill_stroke</strong>\n   </td>\n  </tr>\n</table>\n\n\nSi **noFill()** et **noStroke() **sont exécutées en même temps, rien n\'est tracé dans la zone de dessin.\n\n\n## Formes\n\n\n### Primitives 2d\n\nL\'origine du repère est située en haut à gauche. Les abscisses augmentent de gauche à droite, les ordonnées augmentent de haut en bas.\n\n\n\n![](./images/image1.png)\n\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>point(x, y)\n   </td>\n   <td>Trace un point de coordonnées (x, y). carré de 2x2 pixels\n   </td>\n  </tr>\n  <tr>\n   <td>line(x1, y1, x2, y2)\n   </td>\n   <td>Trace un segment reliant les deux points de coordonnées (x1, y1) et (x2, y2).\n   </td>\n  </tr>\n  <tr>\n   <td>ellipse(x, y, largeur, hauteur)\n   </td>\n   <td>Tracer une ellipse dont le centre a pour coordonnées (x, y) et dont la largeur et la hauteur prennent les valeurs fixées.\n   </td>\n  </tr>\n  <tr>\n   <td>circle(x, y, diametre)\n   </td>\n   <td>Trace un cercle dont le centre a pour coordonnées (x, y) et dont le diamètre prend la valeur fixée. Idem ellipse((x, y, diametre, diametre)\n   </td>\n  </tr>\n  <tr>\n   <td>arc(x,y,largeur,hauteur,,angleDebut, angleFin)\n   </td>\n   <td>Créer une portion d\'ellipse type part de tarte qui pourra être rempli entre les points repérés par les angles angleDébut et angleFin (unité courante). x et y sont les coordonnées du centre du cercle.  \n   </td>\n  </tr>\n  <tr>\n   <td>circle_arc(x,y,rayon,angleDebut, angleFin)\n   </td>\n   <td>idem arc mais à partir d\'un disque\n   </td>\n  </tr>\n  <tr>\n   <td>ellipseMode(corners_center: str)\n   </td>\n   <td>Définie la position des points x et y des fonctions basées sur ellipse. par défaut : "corners" x et y sont les coordonnées du point en haut à gauche du rectangle dans lequel est inscrit l\'ellipse. si les paramètre est "center" x et y représente le centre du rectangle. Retourne la valeur précédente du mode.\n   </td>\n  </tr>\n  <tr>\n   <td>rect(x, y, largeur, hauteur)\n   </td>\n   <td>Créer un rectangle aux coordonnées x,y de largeur largeur et de hauteur. Si rectMode(\'center\') x et y sont les coordonnées du centre du rectangle. Si rectMode(\'corners\') x,y sont les coordonnées du coin haut gauche. Le rectangle est rempli par la couleur définie par fill(couleur). Si le paramètre image est renseigné (image= ...) le fond du rectangle sera occupé pas l\'image retaillée aux dimensions du rectangle sauf si largeur et/ou hauteur sont nulles (ou non renseignées). largeur et/ou hauteur seront alors celles de l\'image. Les paramètres <strong>allign_h </strong>(left, center et right) et  <strong>allign_v</strong> (top,center et bottom) permettent d\'aligner l\'image dans un cadre plus grand qu\'elle.\n   </td>\n  </tr>\n  <tr>\n   <td>square(x, y, cote)\n   </td>\n   <td>Trace un carré dont le sommet en haut à gauche a pour coordonnées (x, y) et dont le côté prend la valeur fixée. fonctionnement idem rectangle\n   </td>\n  </tr>\n  <tr>\n   <td>rectMode(corners_center: str)\n   </td>\n   <td>Définie la position des points x et y des fonctions basées sur rect. par défaut : "corners" x et y sont les coordonnées du point en haut à gauche du rectangle. si les paramètre est "center" x et y représente le centre du rectangle. Retourne la valeur précédente du mode.\n   </td>\n  </tr>\n  <tr>\n   <td>triangle(x1, y1, x2, y2, x3, y3)\n   </td>\n   <td>Trace un triangle dont les trois sommets ont pour coordonnées (x1, y1), (x2, y2), et (x3, y3).\n   </td>\n  </tr>\n  <tr>\n   <td>quad(x1, y1, x2, y2, x3, y3, x4, y4)\n   </td>\n   <td>Trace un quadrilatère dont les quatre sommets ont pour coordonnées (x1, y1), (x2, y2), (x3, y3) et (x4, y4).\n   </td>\n  </tr>\n  <tr>\n   <td>k_line(points)\n   </td>\n   <td>trace un ligne brisée à partir d\'une liste de points [[1,2],[5,6],[8,3],.....]. (nb_point = nb_segments + 1)\n   </td>\n  </tr>\n</table>\n\n\n\n### Tracés\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>strokeWeight(epaisseur)\n   </td>\n   <td>Définit l\'épaisseur du tracé en pixels (par défaut : 1 pixel). Retourne la valeur précédente de la largeur du trait\n   </td>\n  </tr>\n  <tr>\n   <td>noStroke()\n   </td>\n   <td>Désactive le tracé du contour des figures en mettant la largeur du bord à 0. Retourne la valeur précédente de la largeur.\n   </td>\n  </tr>\n  <tr>\n   <td>stroke(couleur)\n   </td>\n   <td>Définit la couleur du tracé des bords des formes et des lignes ("black" par défaut). Si aucune valeur n\'est passée, celle-ci retourne la couleur actuelle. Retourne la valeur précédente de la couleur.\n   </td>\n  </tr>\n</table>\n\n\n\n## Paramètres optionnels:\n\nLes paramètres optionnels sont passés directement dans la fonction et ne concernent que celle-ci: \n\nfill, no_fill, fill_mouse_on, stroke, stroke_weight, command, fill_mousse_on, name. Pour les rectangles nous avons en plus image et border_rounded \n\nexemple :\n\n\n```\ntriangle(20, 10, 50, 15, 40, 70, fill = "green", fill_mouse_on="yellow", stroke_weight=3)\nrect(10,100,100,50,fill = "red", image=loadImage("image.jpg")) # rectangle avec une image\nrect(150,100,100,60,fill= "blue",border_rounded = 10) # rectangle au coins arrondis avec un rayon de 10px \n```\n\n\nl\'ajout de **command = ma_fonction** ou **command_mouse_over = ma_fonction** au paramètre **fill_mouse_on="couleur"** permet d\'exécuter la fonction **ma_fonction()**. Si l\'on veut attribuer **ma_fonction** à plusieurs formes il est possible d\'ajouter le paramètre **name = valeur**. Dans ce cas, la fonction **ma_fonction(name)** sera exécutée . Il faudra créer impérativement soit : \n\ndef ma_fonction():\n\n    pass\n\nou\n\ndef ma_fonction(nom):\n\n    pass\n\nRemarque:<br>\navec le paramètre command exécute la fonction si la forme est cliquée alors qu\'avec command_mous_over elle sera exécutée simplement si la souris est sur la forme.<br>\nSi les deux paramètres sont présents les deux fonctions sont exécutées.\n\n## Textes\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>text(chaine, x, y)\n   </td>\n   <td>Affiche la chaîne à la position (x, y) dans une boite ajustée. couleur, largeur bord et couleur bord de la boite idem formes. Accepte les paramètres optionnels\n   </td>\n  </tr>\n  <tr>\n   <td>text(chaine, x, y, largeur, hauteur)\n   </td>\n   <td>Affiche la chaîne à la position (x, y) dans une boite de dimensions largeur x hauteur. couleur, largeur bord et couleur bord de la boite idem formes. largeur et hauteur sont optionnels\n   </td>\n  </tr>\n  <tr>\n   <td>textAlign(alignement_horizontal)\n<p>\ntextAlign(alignement_horizontal, alignement_vertical)\n   </td>\n   <td>Spécifie l\'alignement horizontal parmi LEFT, CENTER, et RIGHT et l\'alignement vertical parmi TOP, BOTTOM, CENTER, et BASELINE\n   </td>\n  </tr>\n  <tr>\n   <td>textFont(police)\n<p>\ntextFont(police, taille)\n   </td>\n   <td>Spécifie la police de caractères et éventuellement sa taille. Retourne la police et la taille précédente \n   </td>\n  </tr>\n  <tr>\n   <td>textSize(taille)\n   </td>\n   <td>Spécifie la taille de la police de caractères. Retourne la taille précédente de la police\n   </td>\n  </tr>\n  <tr>\n   <td>textStyle(style)\n   </td>\n   <td>Spécifie le style parmi NORMAL, ITALIC, BOLD et BOLDITALIC\n   </td>\n  </tr>\n  <tr>\n   <td>textWidth(chaine)\n   </td>\n   <td>Largeur en pixels de l\'affichage de chaîne, dans la police et taille actuelles\n   </td>\n  </tr>\n</table>\n\n\n\n## Paramètres optionnels spécifique à text:\n\nLes paramètres optionnels sont passés directement dans la fonction et ne concernent que celle-ci: \n\nla fonction text possèdes elle aussi des paramètres optionnels qui ne concernent que la fonction en cours : \\\n**font, font_size, font_color** qui permettent  de définir la police, la taille des caractères ainsi que la couleur de ceux-ci. \n\n**allign_h et allign_v** permettent de positionner le texte dans la boîte de texte comme **textAllign()**.\n\n**padx et pady** permettent de créer une marge autour du texte (valeur en pixels)  \\\nexemple : \n\n\n```\ntext("salut les amis",20,30,300,allign_h="center",font="arial",font_size=48,fontTools="green",pady=10)\n```\n\n\nCe code va afficher "salut les amis" dans un cadre de longueur 300 à la position x=20 et y=30. La hauteur du cadre est calculée en fonction de la hauteur du texte (font_size). **pady=10** ajoute 10 pixels au dessus et en dessous du texte. **Si la hauteur du cadre est donnée, si celle-ci est trop petite le texte sortira du cadre.**\n\n\n## Événements\n\n\n### Touches du clavier\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>key()\n   </td>\n   <td>état des touches du clavier (list)\n   </td>\n  </tr>\n  <tr>\n   <td>keyCode()\n   </td>\n   <td>Code de la dernière touche appuyée.\n   </td>\n  </tr>\n  <tr>\n   <td>keyIsPressed()\n<p>\nisKeyPressed()\n   </td>\n   <td>Vaut True lorsqu\'une touche du clavier est appuyée et False sinon.\n   </td>\n  </tr>\n  <tr>\n   <td>keyIsDown(code)\n<p>\nkeyIsDown(touche)\n   </td>\n   <td>Vaut True si la touche concernée est appuyée et False sinon.\n   </td>\n  </tr>\n</table>\n\n\n\n### Souris\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>mouseX(), mouseY()\n   </td>\n   <td>Coordonnées du pointeur de la souris\n   </td>\n  </tr>\n  <tr>\n   <td>mouseXY()\n   </td>\n   <td>Coordonnées du pointeur de la souris sous forme de tuple\n   </td>\n  </tr>\n  <tr>\n   <td>mouseIsPressed()\n   </td>\n   <td>Vaut True si la souris est cliquée, et False sinon.\n   </td>\n  </tr>\n  <tr>\n   <td>fill_mouse_on(couleur:str)\n   </td>\n   <td>Change la couleur des formes quand on passe la souris dessus. Non actif par défaut.\n   </td>\n  </tr>\n  <tr>\n   <td>noFill_mouse_on()\n   </td>\n   <td>annule l\'effet de fill_mouse_on()\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_click_down()\n   </td>\n   <td>renvoie True lors du passage de relâché à appuyé du bouton de la souris.\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_click_up()\n   </td>\n   <td>renvoie True lors du passage de appuyé à relâché du bouton de la souris.\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_click()\n   </td>\n   <td>idem mouseIsPressed()\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_wheel_state()\n   </td>\n   <td>retourne 1 si la roulette de la souris est tournée vers l\'avant, -1 vers l\'arrière et 0 si elle est immobile.\n   </td>\n  </tr>\n</table>\n\n\n\n## Mathématiques\n\n\n### Angles\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>angleMode(mode_angle:str)\n   </td>\n   <td>Définit l\'unité de mesure des angles. \\\n \'rad\' les angles des fonctions trigonométriques seront pris comme des radians (défaut) \\\n \'deg\' les angles des fonctions trigonométriques seront pris comme des degrés \\\n\'grd\' les angles des fonctions trigonométriques seront pris comme des grades \\\nUne exception est levée en cas d\'erreur de paramètre\n<p>\nsi mode_angle == "" la valeur de mode est retournée (str)\n   </td>\n  </tr>\n  <tr>\n   <td>cos(), sin(), tan(), acos(),asin(),atan(),atan2()\n   </td>\n   <td>Fonctions trigonométriques usuelles l\'unité considérée sera celle choisie avec angleMode(). atan2 : même fonctionnement que la fonction math.atan2 mais l\'unité de l\'angle retourné dépend  de angleMode()  \n   </td>\n  </tr>\n  <tr>\n   <td>degrees(mesure) \\\nradians(mesure) \\\ngrades(mesure)\n   </td>\n   <td>Convertit une mesure d\'angle en degrés, en radians ou en grades. l\'unité de mesure dépend de angleMode(). \n   </td>\n  </tr>\n  <tr>\n   <td>HALF_PI, PI, QUARTER_PI, TWO_PI\n   </td>\n   <td>Constantes permettant respectivement d\'approcher les valeurs de π/2, π, π/4, 2π\n   </td>\n  </tr>\n</table>\n\n\n\n### Géométrie\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>dist(x1,y1,x2,y2)\n   </td>\n   <td>retourne la distance entre deux points\n   </td>\n  </tr>\n  <tr>\n   <td>midPoint(x1, y1, x2, y2)\n   </td>\n   <td>retourne le milieu d\'un segment défini par deux points\n   </td>\n  </tr>\n</table>\n\n\n\n## Images\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>loadImage(chemin)\n   </td>\n   <td>Charge une image à partir d\'un chemin et crée un objet Image. Si nécessaire, l\'image peut être préchargée en plaçant l\'appel à la fonction loadImage en debut de programme.\n   </td>\n  </tr>\n  <tr>\n   <td>loadImages((liste_images:list[str],sens=0) ->Image:\n   </td>\n   <td>Retourne une surface qui est l\'assemblage de toutes les images\n    de la liste. Si sens = 1 les images sont assemblées verticalement\n    et horizontalement si sens =0. Ex: loadImages(["image1.png","image2.jpg"])\n   </td>\n  </tr>\n  <tr>\n   <td>background(Image)\n   </td>\n   <td>Affiche une Image en fond d\'écran\n   </td>\n  </tr>\n  <tr>\n   <td>image(image, x, y)\n   </td>\n   <td>Affiche une Image en plaçant le pixel en haut à gauche au point de coordonnées (x, y) dans la zone de dessin.\n   </td>\n  </tr>\n  <tr>\n   <td>copy_image(picture: Image, rect=None) -> Image\n   </td>\n   <td>retourne une copie de picture ou une partie de picture au dimensions de rect\n   </td>\n  </tr>\n  <tr>\n   <td>get_pixel_color(picture: Image, pos: tuple) -> tuple\n   </td>\n   <td>retourne la valeur de la couleur d\'un pixel d\'une image (picture)\n<p>\nsous la forme d\'un tuple\n   </td>\n  </tr>\n  <tr>\n   <td>resize_image(picture:Image,size : tuple\n   </td>\n   <td>retourne une image redimensionné en fonction de size : (largeur,hauteur) \n   </td>\n  </tr>\n</table>\n\n\n\n## Transformations\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>translate(x,y)\n   </td>\n   <td>applique une translation à toutes les fonctions de dessin et d\'image. x et y sont des valeurs relatives qui s\'ajoutent aux translations précédentes.\n<p>\nLa translation est remise à zéro avant chaque exécution de la fonction draw().\n   </td>\n  </tr>\n  <tr>\n   <td>get_translate()\n   </td>\n   <td>retourne la valeur de la translation sous la forme d\'un tuple (x,y)\n   </td>\n  </tr>\n  <tr>\n   <td>init_translate()\n   </td>\n   <td>Force la remise à zéro de la translation. (A utiliser dans la fonction draw() en cas de besoin \n   </td>\n  </tr>\n  <tr>\n   <td>rotate(angle,axis)\n   </td>\n   <td>applique une rotation &lt;angle> par rapport à &lt;axis>. à toutes les fonctions de dessin et d\'image. angle est une valeur absolue. Par défaut axis vaut (0,0). Cette fonction retourne la valeur précédente prise par la fonction sous la forme d\'un tuple.\n   </td>\n  </tr>\n  <tr>\n   <td>flip_h(axe_h)\n   </td>\n   <td>entraîne une symétrie horizontale par rapport à la droite y = axe_h\n   </td>\n  </tr>\n  <tr>\n   <td>flip_v(axe_v)\n   </td>\n   <td>entraîne une symétrie verticale par rapport à la droite x = axe_v\n   </td>\n  </tr>\n</table>\n\n\n\n## Temporisations\n\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>t=Tempo(duree_ms)\n   </td>\n   <td>t=Tempo(1000) créer un objet de temporisation t de durée 1000 ms qui se relance indéfiniment. \n    <img src="./images/image2.png">\n   </td>\n  </tr>\n  <tr>\n   <td>t.fin()\n   </td>\n   <td>renvoie True lorsque la temporisation est terminée. Pour notre exemple au bout de 500 ms.\n   </td>\n  </tr>\n  <tr>\n   <td>t.is_on()\n   </td>\n   <td>renvoie True si la temporisation est à on.\n   </td>\n  </tr>\n  <tr>\n   <td>t.is_off()\n   </td>\n   <td>renvoie True si la temporisation est à off.\n   </td>\n  </tr>\n  <tr>\n   <td>t.set_tempo(duree_ms)\n   </td>\n   <td>permet de réinitialiser la temporisation avec une nouvelle valeur.\n   </td>\n  </tr>\n  <tr>\n   <td>t.reset()\n   </td>\n   <td>force le redémarrage de la temporisation.\n   </td>\n  </tr>\n   <td>t=Monostable(duree_ms)\n   </td>\n   <td>t=Monostable(500) créer un objet de temporisation t de durée 500 ms qui ne se relance qu\'après execution de la methode reset() \n   </td>\n<tr>\n   <td>t=Pwm(500,25) \n    </td>\n    <td>\n    créer un objet générateur de signaux carré de période 500 ms et de rapport cyclique 25% \n   </td>\n  </tr>\n</table>\n\nComme les objets Monostable et Pwm héritent de Tempo ils en possèdent les méthodes.\n\n# Tutoriel Interface homme Machine\n\n\nl’IHM d’un programme permet à l’utilisateur d’interagir avec celui-ci.\n\nEn mode console les instructions print et input permettent de réaliser une interaction sommaire entre le programme et l’utilisateur.\n\nEn mode graphique l’interaction sera plus poussée.\n\n\n## IHM en python avec LikeProcessing\n\n\n### à faire vous même 1\n\nTaper le code suivant dans un nouveau fichier dans votre ide préféré :\n\n\n```\nfrom likeprocessing.processing import *\n\nihm = IhmScreen()\n\ndef setup():\n   createCanvas(400, 200)\n   ihm.init()\n   background("grey")\ndef compute():\nihm.scan_events()\n\n\ndef draw():\nihm.draw()\n\n\nrun(globals())\n```\n\n\nQuand vous exécutez ce code une fenêtre fonctionnelle vide apparaît.\n\n\n## Ajouter des Widgets à l’intérieur de la fenêtre.\n\nNous allons ajouter du texte dans la fenêtre.\n\n\n### à faire vous même 2\n\nAjouter le code suivant :\n\n\n```\netiquette1 = Label(ihm, (10, 10, 0, 0), "notre premier texte")\n```\n\n\n et lancer le programme. Que se passe-t-il ?\n\nMaintenant ajouter\n\n\n```\nihm.addObjet(etiquette1)\n```\n\n\n et lancer le programme. Que se passe-t-il ?\n\nAjouter : \n\n\n```\nihm.pack(["obj_1"])\n\n```\n\n\nQue se passe-t-il ?\n\nEssayer pack(margin_left=10) , pack(margin_right=10)\n\nAjouter une étiquette2 à la fenêtre.\n\n\n```\netiquette2 = Label(ihm, (10, 10, 0, 0), "etiquette2")\nihm.addObjet(etiquette2)\n```\n\n\nOù se place-t-elle sans utiliser **pack** ?\n\nEssayer avec la méthode pack et conclure.\n\nRemarque :\n\non peut utiliser la méthode addObjet en lui passant une liste d\'objet  \n\n\n```\nihm.addObjet([texte,entry, bouton])\n```\n\n\n\n## Interaction des éléments (widget) avec l’utilisateur.\n\nOn souhaite réaliser interface suivante qui contient :\n\n\n\n![](./images/image3.png)\n\nune étiquette (Label) donnant une explication à l’utilisateur, une zone de texte modifiable (LineEdit) et un bouton (Bouton) qui permettra de changer le titre de la fenêtre par le texte entré par l’utilisateur.\n\n\n```\netiquette = Label(ihm, (10, 10, 0, 0), "Modifier le texte et appuyer sur le bouton")\ntexte = LineEdit(ihm,(10,30,100,30),"")\nbouton = Bouton(ihm, (10, 60, 100, 30), "Changer le titre")\nihm.addObjet([etiquette,texte, bouton])\nihm.pack(["obj_1","obj_2","obj_3"])\n```\n\n\nn’oubliez pas d’utiliser les méthode addObjet() et pack()\n\nLorsque vous lancez le programme, que se passe-t-il ?\n\nModifier votre programme en complétant la création du bouton avec :\n\n\n```\ncommand=lambda : title(texte.text())\n```\n\n\ntexte.text() permet de récupérer le texte écrit par l’utilisateur.\n\nlambda permet de définir une fonction sur une ligne (le paramètre **command** à besoin d’une fonction comme valeur). On peut aussi donner le nom d\'une fonction que l\'on aura déjà créé.\n\nTester votre programme et modifier les paramètres de pack() en utilisant expand="x",pady=10,padx=10 pour obtenir la fenêtre ci-dessus (vous pouvez changer la hauteur de la fenêtre).\n\n\n## Précision sur l\'objet IhmScreen\n\nL\'objet IhmScreen possède plusieurs méthodes pour gérer l\'interface graphique:\n\naddObjet permet d\'ajouter des widgets à l\'interface. Si les objets n\'ont pas de nom (paramètre nom non renseigné) la méthode les nomme "obj_1", "obj_2",... \n\nobjet_by_name(nom_objet) permet de récupérer l\'objet de l\'interface pour par exemple changer sa couleur, récupérer la valeur du texte d\'un LineEdit ou changer le **text()** d\'un Label...\n\nEx : \n\n\n```\nihm.addObjet(LineEdit(ihm,(10,30,100,30),""),"texte")\n```\n\n\nCette commande ajoute à l\'interface un champ modifiable qui sera appelé "texte" \n\nprint(ihm.objet_by_name("texte").text()) affichera sur le console la valeur du champ.\n\nOn peut si on le souhaite supprimer un objet : ihm.delObjet(nom_objet) ou simplement le rendre invisible avec ihm.objet_by_name(nom_objet).visible = False\n\n\n## Création d’une calculatrice\n\nOn désire réaliser l’interface suivante :\n\nIl faut créer des boutons pour chaque touche ainsi qu’une étiquette pour simuler l’écran de la calculatrice.\n\n\n```\ntouche = [["1","2","3","*"],\n         ["4","5","6","/"],\n         ["7","8","9","+"],\n         ["0",".","²","-"],\n         ["(",")","=","AC"]]\n\nfor i in range(5):\n   for j in range(4):\n       ihm.addObjet(Bouton(None, (10+.....*40, 50+.....*40, 40, 40), touche[i][j], command=lambda v=touche[i][j]: calcule(v)))\n```\n\n\nla dernière ligne peut être remplacer par :\n\n\n```\nihm.addObjet(Bouton(None, (10+.....*40, 50+.....*40, 40, 40), touche[i][j], command=calcule, name = touche[i][j])) \n```\n\n\nce qui évite d\'utiliser la fonction lambda.\n\nLe paramètre **name** sera envoyé à la fonction **calcule**.\n\n\n### à faire vous même 3\n\ncréer l’IHM de la calculatrice.\n\n\n\n\n\n![](./images/image4.png)\n\n\n### à faire vous même 4\n\nRéalisation de l’interface graphique d\'un logiciel de dessin\n\nOn veut créer l’IHM du logiciel de dessin my_paint dont le code est le suivant:\n\n\n```\nfrom likeprocessing.processing import *\n\nforme = "cercle"\ncouleur = "blue"\npoint1 = None\nfigure = []\n\n\ndef draw_figure():\n   for f in figure:\n       largeur = abs(f[1][0] - f[2][0])\n       hauteur = abs(f[1][1] - f[2][1])\n       if f[0] == "rectangle":\n           rect(*f[1],largeur,hauteur,fill=f[3])\n       elif f[0] == "ligne":\n           line(*f[1],*f[2],stroke=f[3])\n       elif f[0] == "cercle":\n           circle(*f[1],dist(*f[1],*f[2]),fill=f[3],center_mode="center")\n\n\ndef setup():\n   createCanvas(400, 200,True)\n   background("grey")\n   title("my_paint")\n\n\ndef compute():\n   global point1\n   if mouse_click_down():\n       if point1 is None:\n           point1 = mouseXY()\n           figure.append([forme, point1, point1, couleur])\n   if len(figure)>0 and mouseIsPressed():\n       figure[-1][2] = mouseXY()\n   if mouse_click_up():\n       figure[-1][2] = mouseXY()\n       point1 = None\n\n\n\ndef draw():\n   draw_figure()\n\n\nrun(globals())\n```\n\n\nforme peut prendre les valeurs suivantes : "rectangle","cercle","ligne" et couleur les couleurs acceptés par likeprocessing.\n\nl\'interface doit permettre :\n\n- afficher le type de forme en cours\n\n- de changer le type de forme,\n\n- couleur des figures,\n\n- la couleur du fond,\n\n- effacer la dernière forme,\n\n- effacer le dessin,\n\n\n## Utilisation des boîtes de dialogues d\'information (Show)  et des boîtes de dialogues de questionnement (Ask…)\n\nCes boîtes ont un comportement bloquant c\'est à dire que seule l\'interaction avec avec la boite est prise en compte : les fonctions compute(), draw(), exit() ne sont plus appelées.\n\n\n```\nShowInfo(ihm, "Ceci est une \\ninformation").response()\n```\n\n\n\n![](./images/image5.png)\n\n\n```\nShowWarning(ihm, "Ceci est un \\navertissement").response()\n```\n\n\n![](./images/image6.png)\n\n\n\n```\nShowError(ihm, "Ceci est une \\nerreur").response()\n```\n\n\n![](./images/image7.png)\n\n\n\n```\nAskYesNo(ihm, "Voulez-vous Vraiment\\nquitter le jeu").response()\n```\n\n\n\n![](./images/image8.png)\n\n\n\n```\nAskOkCancel(ihm, "Voulez-vous Vraiment\\nquitter le jeu").response()\n```\n\n\n\n![](images/image9.png)\n\n\n\n```\nAskRetriyCancel(ihm, "Voulez-vous tenter\\nà nouveau\\nvotre chance").response()\n```\n\n\n![](./images/image10.png)\n\n\n\n### Utilisation: \n\nles bouton sont numéroté de la gauche vers la droite (0,1) .Le clique sur croix de la boîte retourne la valeur 4 \n\n\n```\nif AskYesNo(ihm, "Voulez-vous tenter\\nà nouveau\\nvotre chance").response() == 0:\n```\n\n\nAvec le code ci-dessus, la condition sera vraie si le bouton de gauche est cliqué. \n\nExemple d\'utilisation d\'une boîte et de la fonction exit().\n\nLa fonction exit() est une fonction facultative (comme compute) destinée à simplifier la sortie du programme que ce soit par l\'intermédiaire d\'un bouton dédié ou par l\'utilisation de la croix de fermeture de la fenêtre.\n\nSans cette fonction lorsque que l\'on appuie sur la croix la fonction **set_quit(True)** est exécutée ce qui à pour effet de fermer immédiatement l\'application.\n\n le code suivant qui utilise la fonction exit() permet de faire les choses avec plus d\'élégance : \n\n\n```\ndef exit():\n   set_quit(False)\n   if AskYesNo(ihm, "Voulez-vous Vraiment\\nquitter le jeu").response() == 0:\n       set_quit(True)\n```\n\n\najout d\'un bouton dédié à la fermeture du programme : \n\n\n```\nihm.addObjet(Bouton(ihm, (0, 0, 100, 0), "Quitter",\n                   font_size=20, command=lambda : set_quit(True) ), bp_quitter")\n```\n\n\nOn peut aussi passer par une fonction intermédiaire:\n\n\n```\ndef bp_quitter():\n   set_quit(True)\n\nihm.addObjet(Bouton(ihm, (0, 0, 100, 0), "Quitter",\n                   font_size=20, command=bp_quitter), "bp_quitter")\n```\n\n\n \n\n**Remarque**: on peut rendre si nécessaire la croix de la fenêtre likeprocessing inactive avec la fonction  **disabled_quit_cross(). **La fonction** enabled_quit_cross()** permet de la réactivée.\n\n \n',
     'author': 'Pierre Lemaitre',
     'author_email': 'oultetman@sfr.fr',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `likeprocessing-0.1.7.2.4/PKG-INFO` & `likeprocessing-0.1.7.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: likeprocessing
-Version: 0.1.7.2.4
+Version: 0.1.7.2.5
 Summary: Like processing library with pygame
 Author: Pierre Lemaitre
 Author-email: oultetman@sfr.fr
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: pygame (>=2.1.2,<3.0.0)
+Requires-Dist: pygame_textinput (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 
 ## Structure du programme 
 
 
 ### Installation:
@@ -449,26 +450,29 @@
 ```
 triangle(20, 10, 50, 15, 40, 70, fill = "green", fill_mouse_on="yellow", stroke_weight=3)
 rect(10,100,100,50,fill = "red", image=loadImage("image.jpg")) # rectangle avec une image
 rect(150,100,100,60,fill= "blue",border_rounded = 10) # rectangle au coins arrondis avec un rayon de 10px 
 ```
 
 
-l'ajout de **command = ma_fonction** au paramètre **fill_mouse_on="couleur"** permet d'exécuter la fonction **ma_fonction()**. Si l'on veut attribuer **ma_fonction** à plusieurs formes il est possible d'ajouter le paramètre **name = valeur**. Dans ce cas, la fonction **ma_fonction(name)** sera exécutée . Il faudra créer impérativement soit : 
+l'ajout de **command = ma_fonction** ou **command_mouse_over = ma_fonction** au paramètre **fill_mouse_on="couleur"** permet d'exécuter la fonction **ma_fonction()**. Si l'on veut attribuer **ma_fonction** à plusieurs formes il est possible d'ajouter le paramètre **name = valeur**. Dans ce cas, la fonction **ma_fonction(name)** sera exécutée . Il faudra créer impérativement soit : 
 
 def ma_fonction():
 
     pass
 
 ou
 
 def ma_fonction(nom):
 
     pass
 
+Remarque:<br>
+avec le paramètre command exécute la fonction si la forme est cliquée alors qu'avec command_mous_over elle sera exécutée simplement si la souris est sur la forme.<br>
+Si les deux paramètres sont présents les deux fonctions sont exécutées.
 
 ## Textes
 
 
 <table>
   <tr>
    <td><strong>fonctions</strong>
@@ -1304,11 +1308,11 @@
 ihm.addObjet(Bouton(ihm, (0, 0, 100, 0), "Quitter",
                    font_size=20, command=bp_quitter), "bp_quitter")
 ```
 
 
  
 
-**Remarque **: on peut rendre si nécessaire la croix de la fenêtre likeprocessing inactive avec la fonction  **disabled_quit_cross(). **La fonction** enabled_quit_cross()** permet de la réactivée.
+**Remarque**: on peut rendre si nécessaire la croix de la fenêtre likeprocessing inactive avec la fonction  **disabled_quit_cross(). **La fonction** enabled_quit_cross()** permet de la réactivée.
```

