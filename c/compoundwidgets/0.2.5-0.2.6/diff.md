# Comparing `tmp/compoundwidgets-0.2.5.tar.gz` & `tmp/compoundwidgets-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compoundwidgets-0.2.5.tar", last modified: Fri Apr 21 14:36:55 2023, max compression
+gzip compressed data, was "compoundwidgets-0.2.6.tar", last modified: Fri Apr 21 14:46:26 2023, max compression
```

## Comparing `compoundwidgets-0.2.5.tar` & `compoundwidgets-0.2.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:36:55.140961 compoundwidgets-0.2.5/
--rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      332 2023-04-21 14:36:55.139992 compoundwidgets-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1161 2023-04-21 13:55:20.000000 compoundwidgets-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 14:36:55.034132 compoundwidgets-0.2.5/compoundwidgets/
--rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.5/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
--rw-rw-rw-   0        0        0    54397 2023-04-21 14:35:17.000000 compoundwidgets-0.2.5/compoundwidgets/COMPOUND_WIDGETS.py
--rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.5/compoundwidgets/CUSTOM_BUTTONS.py
--rw-rw-rw-   0        0        0    16474 2023-04-17 20:34:54.000000 compoundwidgets-0.2.5/compoundwidgets/CUSTOM_FRAMES.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:36:55.077597 compoundwidgets-0.2.5/compoundwidgets/IMAGES/
--rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/__init__.py
--rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/add_new.png
--rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/add_to_form.png
--rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/back.png
--rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/calculate.png
--rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/clear.png
--rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/edit_form.png
--rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/help.png
--rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/no.png
--rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/quit.png
--rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/remove_from_form.png
--rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/save.png
--rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/trash_can.png
--rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.5/compoundwidgets/IMAGES/yes.png
--rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.5/compoundwidgets/LED_BUTTONS.py
--rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.5/compoundwidgets/MESSAGE_BOX_WIDGETS.py
--rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.5/compoundwidgets/SCRIPTS.py
--rw-rw-rw-   0        0        0     1843 2023-04-21 14:36:52.000000 compoundwidgets-0.2.5/compoundwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:36:55.050299 compoundwidgets-0.2.5/compoundwidgets.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-21 14:36:54.000000 compoundwidgets-0.2.5/compoundwidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2023-04-21 14:36:54.000000 compoundwidgets-0.2.5/compoundwidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:36:54.000000 compoundwidgets-0.2.5/compoundwidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-21 14:36:54.000000 compoundwidgets-0.2.5/compoundwidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-21 14:36:54.000000 compoundwidgets-0.2.5/compoundwidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:36:55.140961 compoundwidgets-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      576 2023-04-21 14:36:52.000000 compoundwidgets-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:36:55.137950 compoundwidgets-0.2.5/test/
--rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.5/test/autocomplete_widget_test.py
--rw-rw-rw-   0        0        0    10106 2023-04-17 13:00:19.000000 compoundwidgets-0.2.5/test/compound_widgets_test_1.py
--rw-rw-rw-   0        0        0     7306 2023-04-17 12:42:39.000000 compoundwidgets-0.2.5/test/compound_widgets_test_2.py
--rw-rw-rw-   0        0        0      981 2023-04-07 20:22:34.000000 compoundwidgets-0.2.5/test/custom_buttons_test.py
--rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.5/test/custom_frames_test_1.py
--rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.5/test/custom_frames_test_2.py
--rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.5/test/custom_frames_test_3.py
--rw-rw-rw-   0        0        0     2745 2023-04-17 20:15:42.000000 compoundwidgets-0.2.5/test/custom_frames_test_4.py
--rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.5/test/led_buttons_test.py
--rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.5/test/message_box_test.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:46:26.899505 compoundwidgets-0.2.6/
+-rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      332 2023-04-21 14:46:26.898505 compoundwidgets-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2023-04-21 13:55:20.000000 compoundwidgets-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:46:26.781096 compoundwidgets-0.2.6/compoundwidgets/
+-rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.6/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
+-rw-rw-rw-   0        0        0    54563 2023-04-21 14:44:57.000000 compoundwidgets-0.2.6/compoundwidgets/COMPOUND_WIDGETS.py
+-rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.6/compoundwidgets/CUSTOM_BUTTONS.py
+-rw-rw-rw-   0        0        0    16474 2023-04-17 20:34:54.000000 compoundwidgets-0.2.6/compoundwidgets/CUSTOM_FRAMES.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:46:26.830821 compoundwidgets-0.2.6/compoundwidgets/IMAGES/
+-rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/__init__.py
+-rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/add_new.png
+-rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/add_to_form.png
+-rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/back.png
+-rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/calculate.png
+-rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/clear.png
+-rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/edit_form.png
+-rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/help.png
+-rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/no.png
+-rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/quit.png
+-rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/remove_from_form.png
+-rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/save.png
+-rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/trash_can.png
+-rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/yes.png
+-rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.6/compoundwidgets/LED_BUTTONS.py
+-rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.6/compoundwidgets/MESSAGE_BOX_WIDGETS.py
+-rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.6/compoundwidgets/SCRIPTS.py
+-rw-rw-rw-   0        0        0     1843 2023-04-21 14:46:23.000000 compoundwidgets-0.2.6/compoundwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:46:26.798107 compoundwidgets-0.2.6/compoundwidgets.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-21 14:46:26.000000 compoundwidgets-0.2.6/compoundwidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-04-21 14:46:26.000000 compoundwidgets-0.2.6/compoundwidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:46:26.000000 compoundwidgets-0.2.6/compoundwidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-21 14:46:26.000000 compoundwidgets-0.2.6/compoundwidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-21 14:46:26.000000 compoundwidgets-0.2.6/compoundwidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:46:26.900504 compoundwidgets-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      576 2023-04-21 14:46:23.000000 compoundwidgets-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:46:26.897490 compoundwidgets-0.2.6/test/
+-rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.6/test/autocomplete_widget_test.py
+-rw-rw-rw-   0        0        0    10106 2023-04-17 13:00:19.000000 compoundwidgets-0.2.6/test/compound_widgets_test_1.py
+-rw-rw-rw-   0        0        0     7306 2023-04-17 12:42:39.000000 compoundwidgets-0.2.6/test/compound_widgets_test_2.py
+-rw-rw-rw-   0        0        0      981 2023-04-07 20:22:34.000000 compoundwidgets-0.2.6/test/custom_buttons_test.py
+-rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.6/test/custom_frames_test_1.py
+-rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.6/test/custom_frames_test_2.py
+-rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.6/test/custom_frames_test_3.py
+-rw-rw-rw-   0        0        0     2745 2023-04-17 20:15:42.000000 compoundwidgets-0.2.6/test/custom_frames_test_4.py
+-rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.6/test/led_buttons_test.py
+-rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.6/test/message_box_test.py
```

### Comparing `compoundwidgets-0.2.5/LICENSE.txt` & `compoundwidgets-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/MANIFEST.in` & `compoundwidgets-0.2.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/README.md` & `compoundwidgets-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/AUTOCOMPLETE_WIDGETS.py` & `compoundwidgets-0.2.6/compoundwidgets/AUTOCOMPLETE_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/COMPOUND_WIDGETS.py` & `compoundwidgets-0.2.6/compoundwidgets/COMPOUND_WIDGETS.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,16 @@
         if True:
             self.entry_method = entry_method
             self.variable.trace_add(["read", "write", "unset"], self._update_value)
             self.entry.bind("<Return>", entry_method)
             self.entry.bind("<FocusOut>", entry_method)
 
     def _update_value(self, name, index, mode):
-        self.entry_method()
+        if self.entry_method:
+            self.entry.event_generate("<Return>")
 
     def enable(self):
         self.label.config(style='TLabel')
         self.entry.config(state='normal')
 
     def disable(self):
         self.variable.set('')
@@ -429,15 +430,16 @@
             self.spin.bind("<FocusOut>", entry_method, add='+')
             self.spin.bind("<FocusOut>", self._check_user_value, add='+')
             self.spin.bind("<<Increment>>", self._do_on_increment)
             self.spin.bind("<<Decrement>>", self._do_on_decrement)
             self.spin.bind("<ButtonRelease-1>", self._spin_selected, add='+')
 
     def _update_value(self, name, index, mode):
-        self.entry_method()
+        if self.entry_method:
+            self.entry.event_generate("<Return>")
 
     def _spin_selected(self, event=None):
         self._check_user_value()
         self.spin.event_generate('<Return>')
 
     def _do_on_increment(self):
         self._do_upon_clicking_arrows("up")
@@ -837,25 +839,25 @@
             self.combobox_variable = self.unit_combo.variable
             self.is_locked = False
 
         # Bind methods
         if True:
             self.entry_method = entry_method
             self.entry_variable.trace_add(["read", "write", "unset"], self._update_value)
-            self.entry_method = entry_method
             self.entry.bind("<Return>", entry_method)
             self.entry.bind("<FocusOut>", entry_method)
 
             if not self.combobox_unit_conversion:
                 self.unit_combo.bind("<<ComboboxSelected>>", entry_method)
             else:
                 self.unit_combo.bind("<<ComboboxSelected>>", self._convert_to_selected_unit)
 
     def _update_value(self, name, index, mode):
-        self.entry_method()
+        if self.entry_method:
+            self.entry.event_generate("<Return>")
 
     # Widget state methods ---------------------------------------------------------------------------------------------
     def enable(self):
         self.unlock_unit()
         self.label.config(style='TLabel')
         self.entry.config(state='normal')
         self.unit_combo.config(state='readonly', values=self.unit_combo.values)
@@ -1249,15 +1251,16 @@
             self.variable.trace_add(["read", "write", "unset"], self._update_value)
             self.entry_method = entry_method
             if entry_method:
                 self.entry.bind("<Return>", entry_method)
                 self.entry.bind("<FocusOut>", entry_method)
 
     def _update_value(self, name, index, mode):
-        self.entry_method()
+        if self.entry_method:
+            self.entry.event_generate("<Return>")
 
     def enable(self):
         self.label.config(style='TLabel')
         self.entry.config(state='normal')
         self.button.state(["!disabled"])
 
     def disable(self):
```

### Comparing `compoundwidgets-0.2.5/compoundwidgets/CUSTOM_BUTTONS.py` & `compoundwidgets-0.2.6/compoundwidgets/CUSTOM_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/CUSTOM_FRAMES.py` & `compoundwidgets-0.2.6/compoundwidgets/CUSTOM_FRAMES.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/add_new.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/add_new.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/add_to_form.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/add_to_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/back.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/back.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/calculate.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/calculate.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/clear.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/clear.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/edit_form.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/edit_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/help.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/help.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/no.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/no.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/quit.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/quit.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/remove_from_form.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/remove_from_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/save.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/save.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/trash_can.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/trash_can.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/IMAGES/yes.png` & `compoundwidgets-0.2.6/compoundwidgets/IMAGES/yes.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/LED_BUTTONS.py` & `compoundwidgets-0.2.6/compoundwidgets/LED_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/MESSAGE_BOX_WIDGETS.py` & `compoundwidgets-0.2.6/compoundwidgets/MESSAGE_BOX_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/SCRIPTS.py` & `compoundwidgets-0.2.6/compoundwidgets/SCRIPTS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/compoundwidgets/__init__.py` & `compoundwidgets-0.2.6/compoundwidgets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.05"
+__version__ = "0.2.06"
 __author__ = 'Andre Mariano'
 __all__ = ['AUTOCOMPLETE_WIDGETS',
            'COMPOUND_WIDGETS',
            'CUSTOM_BUTTONS',
            'CUSTOM_FRAMES',
            'MESSAGE_BOX_WIDGETS',
            'IMAGES',
```

### Comparing `compoundwidgets-0.2.5/compoundwidgets.egg-info/SOURCES.txt` & `compoundwidgets-0.2.6/compoundwidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/setup.py` & `compoundwidgets-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='compoundwidgets',
-    version='0.2.05',
+    version='0.2.06',
     author='Andre Mariano',
     license="MIT",
     url='https://github.com/AndreMariano100/CompoundWidgets.git',
     description='Compound TTK Widgets with ttkbootstrap',
     author_email='andremariano100@gmail.com',
     packages=['compoundwidgets', 'compoundwidgets.IMAGES'],
     install_requires=['ttkbootstrap', 'Pillow'],
```

### Comparing `compoundwidgets-0.2.5/test/autocomplete_widget_test.py` & `compoundwidgets-0.2.6/test/autocomplete_widget_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/test/compound_widgets_test_1.py` & `compoundwidgets-0.2.6/test/compound_widgets_test_1.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/test/compound_widgets_test_2.py` & `compoundwidgets-0.2.6/test/compound_widgets_test_2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/test/custom_buttons_test.py` & `compoundwidgets-0.2.6/test/custom_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/test/custom_frames_test_1.py` & `compoundwidgets-0.2.6/test/custom_frames_test_1.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/test/custom_frames_test_2.py` & `compoundwidgets-0.2.6/test/custom_frames_test_2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/test/custom_frames_test_3.py` & `compoundwidgets-0.2.6/test/custom_frames_test_3.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/test/custom_frames_test_4.py` & `compoundwidgets-0.2.6/test/custom_frames_test_4.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/test/led_buttons_test.py` & `compoundwidgets-0.2.6/test/led_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.5/test/message_box_test.py` & `compoundwidgets-0.2.6/test/message_box_test.py`

 * *Files identical despite different names*

