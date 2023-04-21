# Comparing `tmp/compoundwidgets-0.2.3.tar.gz` & `tmp/compoundwidgets-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compoundwidgets-0.2.3.tar", last modified: Mon Apr 17 20:37:05 2023, max compression
+gzip compressed data, was "compoundwidgets-0.2.4.tar", last modified: Fri Apr 21 14:04:49 2023, max compression
```

## Comparing `compoundwidgets-0.2.3.tar` & `compoundwidgets-0.2.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:37:05.088102 compoundwidgets-0.2.3/
--rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      332 2023-04-17 20:37:05.088102 compoundwidgets-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      673 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 20:37:04.931118 compoundwidgets-0.2.3/compoundwidgets/
--rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.3/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
--rw-rw-rw-   0        0        0    53695 2023-04-17 13:08:22.000000 compoundwidgets-0.2.3/compoundwidgets/COMPOUND_WIDGETS.py
--rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.3/compoundwidgets/CUSTOM_BUTTONS.py
--rw-rw-rw-   0        0        0    16474 2023-04-17 20:34:54.000000 compoundwidgets-0.2.3/compoundwidgets/CUSTOM_FRAMES.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:37:05.010161 compoundwidgets-0.2.3/compoundwidgets/IMAGES/
--rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/__init__.py
--rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/add_new.png
--rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/add_to_form.png
--rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/back.png
--rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/calculate.png
--rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/clear.png
--rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/edit_form.png
--rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/help.png
--rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/no.png
--rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/quit.png
--rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/remove_from_form.png
--rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/save.png
--rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/trash_can.png
--rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.3/compoundwidgets/IMAGES/yes.png
--rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.3/compoundwidgets/LED_BUTTONS.py
--rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.3/compoundwidgets/MESSAGE_BOX_WIDGETS.py
--rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.3/compoundwidgets/SCRIPTS.py
--rw-rw-rw-   0        0        0     1843 2023-04-17 20:36:58.000000 compoundwidgets-0.2.3/compoundwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:37:04.962369 compoundwidgets-0.2.3/compoundwidgets.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-17 20:37:04.000000 compoundwidgets-0.2.3/compoundwidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2023-04-17 20:37:04.000000 compoundwidgets-0.2.3/compoundwidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:37:04.000000 compoundwidgets-0.2.3/compoundwidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-17 20:37:04.000000 compoundwidgets-0.2.3/compoundwidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-17 20:37:04.000000 compoundwidgets-0.2.3/compoundwidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 20:37:05.088102 compoundwidgets-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      576 2023-04-17 20:36:58.000000 compoundwidgets-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:37:05.088102 compoundwidgets-0.2.3/test/
--rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.3/test/autocomplete_widget_test.py
--rw-rw-rw-   0        0        0    10106 2023-04-17 13:00:19.000000 compoundwidgets-0.2.3/test/compound_widgets_test_1.py
--rw-rw-rw-   0        0        0     7306 2023-04-17 12:42:39.000000 compoundwidgets-0.2.3/test/compound_widgets_test_2.py
--rw-rw-rw-   0        0        0      981 2023-04-07 20:22:34.000000 compoundwidgets-0.2.3/test/custom_buttons_test.py
--rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.3/test/custom_frames_test_1.py
--rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.3/test/custom_frames_test_2.py
--rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.3/test/custom_frames_test_3.py
--rw-rw-rw-   0        0        0     2745 2023-04-17 20:15:42.000000 compoundwidgets-0.2.3/test/custom_frames_test_4.py
--rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.3/test/led_buttons_test.py
--rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.3/test/message_box_test.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:04:49.556913 compoundwidgets-0.2.4/
+-rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      332 2023-04-21 14:04:49.556913 compoundwidgets-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2023-04-21 13:55:20.000000 compoundwidgets-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:04:49.409552 compoundwidgets-0.2.4/compoundwidgets/
+-rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.4/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
+-rw-rw-rw-   0        0        0    54153 2023-04-21 14:04:42.000000 compoundwidgets-0.2.4/compoundwidgets/COMPOUND_WIDGETS.py
+-rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.4/compoundwidgets/CUSTOM_BUTTONS.py
+-rw-rw-rw-   0        0        0    16474 2023-04-17 20:34:54.000000 compoundwidgets-0.2.4/compoundwidgets/CUSTOM_FRAMES.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:04:49.475056 compoundwidgets-0.2.4/compoundwidgets/IMAGES/
+-rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/__init__.py
+-rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/add_new.png
+-rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/add_to_form.png
+-rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/back.png
+-rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/calculate.png
+-rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/clear.png
+-rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/edit_form.png
+-rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/help.png
+-rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/no.png
+-rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/quit.png
+-rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/remove_from_form.png
+-rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/save.png
+-rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/trash_can.png
+-rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.4/compoundwidgets/IMAGES/yes.png
+-rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.4/compoundwidgets/LED_BUTTONS.py
+-rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.4/compoundwidgets/MESSAGE_BOX_WIDGETS.py
+-rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.4/compoundwidgets/SCRIPTS.py
+-rw-rw-rw-   0        0        0     1843 2023-04-21 13:55:20.000000 compoundwidgets-0.2.4/compoundwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:04:49.441024 compoundwidgets-0.2.4/compoundwidgets.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-21 14:04:49.000000 compoundwidgets-0.2.4/compoundwidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-04-21 14:04:49.000000 compoundwidgets-0.2.4/compoundwidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:04:49.000000 compoundwidgets-0.2.4/compoundwidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-21 14:04:49.000000 compoundwidgets-0.2.4/compoundwidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-21 14:04:49.000000 compoundwidgets-0.2.4/compoundwidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:04:49.556913 compoundwidgets-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      576 2023-04-21 14:04:42.000000 compoundwidgets-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:04:49.556913 compoundwidgets-0.2.4/test/
+-rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.4/test/autocomplete_widget_test.py
+-rw-rw-rw-   0        0        0    10106 2023-04-17 13:00:19.000000 compoundwidgets-0.2.4/test/compound_widgets_test_1.py
+-rw-rw-rw-   0        0        0     7306 2023-04-17 12:42:39.000000 compoundwidgets-0.2.4/test/compound_widgets_test_2.py
+-rw-rw-rw-   0        0        0      981 2023-04-07 20:22:34.000000 compoundwidgets-0.2.4/test/custom_buttons_test.py
+-rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.4/test/custom_frames_test_1.py
+-rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.4/test/custom_frames_test_2.py
+-rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.4/test/custom_frames_test_3.py
+-rw-rw-rw-   0        0        0     2745 2023-04-17 20:15:42.000000 compoundwidgets-0.2.4/test/custom_frames_test_4.py
+-rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.4/test/led_buttons_test.py
+-rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.4/test/message_box_test.py
```

### Comparing `compoundwidgets-0.2.3/LICENSE.txt` & `compoundwidgets-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/MANIFEST.in` & `compoundwidgets-0.2.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/AUTOCOMPLETE_WIDGETS.py` & `compoundwidgets-0.2.4/compoundwidgets/AUTOCOMPLETE_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/COMPOUND_WIDGETS.py` & `compoundwidgets-0.2.4/compoundwidgets/COMPOUND_WIDGETS.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,24 +574,24 @@
         (almost) Static Methods: return (Value, Unit)
         convert_data_to_metric(value, unit): converts the given pair to the equivalent metric unit
         convert_data_to_imperial(value, unit): converts the given pair to the equivalent imperial unit
         convert_to_given_unit((old_value, old_unit), new_unit): converts the given pair to the given unit
     Internal Classes:
         NoUnitCombo: ('-')
         TemperatureCombo: ('°C', '°F')
-        LengthCombo: ('mm', 'cm', 'in')
-        AreaCombo: ('mm²', 'cm²', 'in²')
+        LengthCombo: ('mm', 'cm', 'm', 'in')
+        AreaCombo: ('mm²', 'cm²', 'm²', 'in²')
         PressureCombo: ('kPa', 'bar', 'kgf/cm²', 'MPa', 'atmosphere', 'ksi', 'psi')
         StressCombo: ('MPa', 'GPa', 'x10³ ksi', 'psi', 'ksi')
         ForceCombo: ('N', 'kN', 'kgf', 'lbf')
         MomentCombo: ('N.m', 'kN.m', 'kgf.m', 'lbf.ft')
         EnergyCombo: ('joule', 'ft-lbf')
         ToughnessCombo: ('MPa.√m', 'N/mm^(3/2)', 'ksi.√in')
         JIntegralCombo: ('joule/m²', 'ft-lbf/ft²')
-        ThermalExpansionCombo: ('10e-6 mm/mm.°C', '10e-6 in/in.°F')
+        ThermalExpansionCombo: ('10e-6/°C', '10e-6/°F')
     """
 
     class NoUnitCombo(ttk.Combobox):
         def __init__(self, parent, width):
             super().__init__(parent)
 
             self.values = ('-',)
@@ -608,27 +608,27 @@
             self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
                            state='readonly')
 
     class LengthCombo(ttk.Combobox):
         def __init__(self, parent, width):
             super().__init__(parent)
 
-            self.values = ('mm', 'cm', 'in')
-            self.conversion_values = (1, 10, 25.4)
+            self.values = ('mm', 'cm', 'm', 'in')
+            self.conversion_values = (1, 10, 1000, 25.4)
 
             self.variable = tk.StringVar(value=self.values[0])
             self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
                            state='readonly')
 
     class AreaCombo(ttk.Combobox):
         def __init__(self, parent, width):
             super().__init__(parent)
 
-            self.values = ('mm²', 'cm²', 'in²')
-            self.conversion_values = (1, 100, 645.16)
+            self.values = ('mm²', 'cm²', 'm²', 'in²')
+            self.conversion_values = (1, 100, 1000000, 645.16)
 
             self.variable = tk.StringVar(value=self.values[0])
             self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
                            state='readonly')
 
     class PressureCombo(ttk.Combobox):
         def __init__(self, parent, width):
@@ -707,60 +707,65 @@
 
             self.values = ('10e-6/°C', '10e-6/°F')
             self.conversion_values = (1, 0.55556)
             self.variable = tk.StringVar(value=self.values[0])
             self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
                            state='readonly')
 
+    # Dictionary that correlates the desired unit to the appropriate class
     unit_dict = {
         'none': NoUnitCombo,
         'temperature': TemperatureCombo,
         'length': LengthCombo,
         'area': AreaCombo,
         'pressure': PressureCombo,
         'stress': StressCombo,
         'force': ForceCombo,
         'moment': MomentCombo,
         'energy': EnergyCombo,
         'toughness': ToughnessCombo,
         'j-integral': JIntegralCombo,
         'thermal expansion': ThermalExpansionCombo
     }
+
+    # List which identifies unit as SI or Custom. Their position in list guides its conversion units.
     metric_unit_list = \
-        ('mm', 'cm',  # LengthCombo
-         'mm²', 'cm²',  # AreaCombo
+        ('mm', 'cm',  'm',          # LengthCombo
+         'mm²', 'cm²', 'm²',        # AreaCombo
          'kPa', 'kPa', 'bar', 'kgf/cm²', 'MPa', 'atmosphere',  # PressureCombo
-         'kPa', 'GPa',  # StressCombo
-         'N', 'kgf',  # ForceCombo
-         'N.m', 'kgf.m',  # MomentCombo
-         '-',  # NoUnitCombo
-         'N/mm^(3/2)', 'MPa.√m',  # ToughnessCombo
-         'joule',  # EnergyCombo
-         'joule/m²',  # JIntegralCombo
-         '10e-6/°C'  # Thermal Expansion
+         'GPa',                     # StressCombo
+         'N', 'kN', 'kgf',          # ForceCombo
+         'N.m', 'kN.m', 'kgf.m',    # MomentCombo
+         '-',                       # NoUnitCombo
+         'N/mm^(3/2)', 'MPa.√m',    # ToughnessCombo
+         'joule',                   # EnergyCombo
+         'joule/m²',                # JIntegralCombo
+         '10e-6/°C',                # Thermal Expansion
          )
     imperial_unit_list = \
-        ('in', 'in',
-         'in²', 'in²',
+        ('in', 'in', 'in',
+         'in²', 'in²', 'in²',
          'psi', 'ksi', 'ksi', 'ksi', 'ksi', 'psi',
-         'x10³ ksi', 'x10³ ksi',
-         'lbf', 'lbf',
-         'lbf.ft', 'lbf.ft',
+         'x10³ ksi',
+         'lbf', 'lbf', 'lbf',
+         'lbf.ft', 'lbf.ft', 'lbf.ft',
          '-',
          'ksi.√in', 'ksi.√in',
          'ft-lbf',
          'ft-lbf/ft²',
          '10e-6/°F')
+
+    # List with the conversion values from imperial to metric
     conversion = \
-        (25.4, 2.54,
-         645.16, 6.4516,
+        (25.4, 2.54, 0.0254,
+         645.16, 6.4516, 0.00064516,
          6.894757, 6894.757, 68.94757, 70.30696, 6.894757, 0.06804596,
-         6.894757e6, 6.894757,
-         4.448222, 0.4535924,
-         1.35582, 0.1382552,
+         6.894757e6,
+         4.448222, 0.004448222, 0.4535924,
+         1.35582, 0.00135582, 0.1382552,
          1,
          34.7485, 1.0988,
          1.355818,
          14.5939,
          0.55556)
 
     # imperial_unit_list[index] * conversion[index] => metric_unit_list[index]
```

### Comparing `compoundwidgets-0.2.3/compoundwidgets/CUSTOM_BUTTONS.py` & `compoundwidgets-0.2.4/compoundwidgets/CUSTOM_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/CUSTOM_FRAMES.py` & `compoundwidgets-0.2.4/compoundwidgets/CUSTOM_FRAMES.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/add_new.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/add_new.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/add_to_form.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/add_to_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/back.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/back.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/calculate.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/calculate.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/clear.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/clear.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/edit_form.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/edit_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/help.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/help.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/no.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/no.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/quit.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/quit.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/remove_from_form.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/remove_from_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/save.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/save.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/trash_can.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/trash_can.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/IMAGES/yes.png` & `compoundwidgets-0.2.4/compoundwidgets/IMAGES/yes.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/LED_BUTTONS.py` & `compoundwidgets-0.2.4/compoundwidgets/LED_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/MESSAGE_BOX_WIDGETS.py` & `compoundwidgets-0.2.4/compoundwidgets/MESSAGE_BOX_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/SCRIPTS.py` & `compoundwidgets-0.2.4/compoundwidgets/SCRIPTS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/compoundwidgets/__init__.py` & `compoundwidgets-0.2.4/compoundwidgets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.03"
+__version__ = "0.2.04"
 __author__ = 'Andre Mariano'
 __all__ = ['AUTOCOMPLETE_WIDGETS',
            'COMPOUND_WIDGETS',
            'CUSTOM_BUTTONS',
            'CUSTOM_FRAMES',
            'MESSAGE_BOX_WIDGETS',
            'IMAGES',
```

### Comparing `compoundwidgets-0.2.3/compoundwidgets.egg-info/SOURCES.txt` & `compoundwidgets-0.2.4/compoundwidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/setup.py` & `compoundwidgets-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='compoundwidgets',
-    version='0.2.03',
+    version='0.2.04',
     author='Andre Mariano',
     license="MIT",
     url='https://github.com/AndreMariano100/CompoundWidgets.git',
     description='Compound TTK Widgets with ttkbootstrap',
     author_email='andremariano100@gmail.com',
     packages=['compoundwidgets', 'compoundwidgets.IMAGES'],
     install_requires=['ttkbootstrap', 'Pillow'],
```

### Comparing `compoundwidgets-0.2.3/test/autocomplete_widget_test.py` & `compoundwidgets-0.2.4/test/autocomplete_widget_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/test/compound_widgets_test_1.py` & `compoundwidgets-0.2.4/test/compound_widgets_test_1.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/test/compound_widgets_test_2.py` & `compoundwidgets-0.2.4/test/compound_widgets_test_2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/test/custom_buttons_test.py` & `compoundwidgets-0.2.4/test/custom_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/test/custom_frames_test_1.py` & `compoundwidgets-0.2.4/test/custom_frames_test_1.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/test/custom_frames_test_2.py` & `compoundwidgets-0.2.4/test/custom_frames_test_2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/test/custom_frames_test_3.py` & `compoundwidgets-0.2.4/test/custom_frames_test_3.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/test/custom_frames_test_4.py` & `compoundwidgets-0.2.4/test/custom_frames_test_4.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/test/led_buttons_test.py` & `compoundwidgets-0.2.4/test/led_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.3/test/message_box_test.py` & `compoundwidgets-0.2.4/test/message_box_test.py`

 * *Files identical despite different names*

