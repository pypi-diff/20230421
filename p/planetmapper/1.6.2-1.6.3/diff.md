# Comparing `tmp/planetmapper-1.6.2.tar.gz` & `tmp/planetmapper-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.6.2.tar", last modified: Fri Apr 14 13:18:35 2023, max compression
+gzip compressed data, was "planetmapper-1.6.3.tar", last modified: Fri Apr 21 10:33:40 2023, max compression
```

## Comparing `planetmapper-1.6.2.tar` & `planetmapper-1.6.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:35.173646 planetmapper-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-14 13:18:35.173646 planetmapper-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-14 13:18:24.000000 planetmapper-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:35.169646 planetmapper-1.6.2/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    72134 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)    99198 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:35.173646 planetmapper-1.6.2/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   109295 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    43334 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:35.169646 planetmapper-1.6.2/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 13:18:24.000000 planetmapper-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:18:35.173646 planetmapper-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-14 13:18:24.000000 planetmapper-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:35.173646 planetmapper-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:33:40.125534 planetmapper-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-21 10:33:40.125534 planetmapper-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-21 10:33:26.000000 planetmapper-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:33:40.121534 planetmapper-1.6.3/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72134 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99198 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:33:40.125534 planetmapper-1.6.3/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114930 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43334 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:33:40.125534 planetmapper-1.6.3/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 10:33:26.000000 planetmapper-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:33:40.125534 planetmapper-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-21 10:33:26.000000 planetmapper-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:33:40.125534 planetmapper-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_utils.py
```

### Comparing `planetmapper-1.6.2/PKG-INFO` & `planetmapper-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.6.2
+Version: 1.6.3
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
```

### Comparing `planetmapper-1.6.2/README.md` & `planetmapper-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/__init__.py` & `planetmapper-1.6.3/planetmapper/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/base.py` & `planetmapper-1.6.3/planetmapper/base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/basic_body.py` & `planetmapper-1.6.3/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/body.py` & `planetmapper-1.6.3/planetmapper/body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/body_xy.py` & `planetmapper-1.6.3/planetmapper/body_xy.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/data/rings.json` & `planetmapper-1.6.3/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/data_loader.py` & `planetmapper-1.6.3/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/gui.py` & `planetmapper-1.6.3/planetmapper/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                 ],
                 'plate_scale_km': [
                     lambda f: self.get_observation().set_plate_scale_km(f)
                 ],
             },
         )
         self.ui_callbacks: defaultdict[
-            SETTER_KEY, set[Callable[[], Any]]
+            SETTER_KEY | None, set[Callable[[], Any]]
         ] = defaultdict(set)
 
         self.getters: dict[SETTER_KEY, Callable[[], float]] = {
             'x0': lambda: self.get_observation().get_x0(),
             'y0': lambda: self.get_observation().get_y0(),
             'r0': lambda: self.get_observation().get_r0(),
             'rotation': lambda: self.get_observation().get_rotation(),
@@ -245,14 +245,16 @@
         }
 
         self.kernels: list[str] = [
             os.path.join(base.get_kernel_path(), pattern)
             for pattern in base._KERNEL_DATA['kernel_patterns']
         ]
 
+        self.delayed_actions: dict[str, tuple[Callable[[], Any], str]] = {}
+
         self.event_time_to_ignore = None
         self.gui_built = False
 
     def __repr__(self) -> str:
         return f'InteractiveObservation()'
 
     def run(self) -> None:
@@ -311,14 +313,21 @@
         if n_wavl == 1:
             self.plot_settings['_']['image_mode'] = 'single'
         elif n_wavl == 3 and not self.gui_built:
             self.plot_settings['_']['image_mode'] = 'rgb'
         else:
             self.plot_settings['_']['image_mode'] = 'sum'
 
+        self.plot_settings['_'].update(
+            image_idx_single=0,
+            image_idx_r=0,
+            image_idx_g=1,
+            image_idx_b=2,
+        )
+
         if self.gui_built:
             self.run_all_ui_callbacks()
             self.rebuild_plot()
             self.root.title(self.get_observation().get_description(multiline=False))
             self.reset_help_hint()
 
         self.click_locations = []
@@ -365,14 +374,16 @@
                 foreground='black',
                 insertcolor='black',
                 fieldbackground='white',
                 selectbackground='#bdf',
                 selectforeground='black',
             )
 
+        self.style.map('TScale', troughcolor=[('disabled', '#d9d9d9')])
+
     def build_controls(self) -> None:
         self.notebook = ttk.Notebook(self.controls_frame)
         self.notebook.pack(fill='both', expand=True)
         self.build_main_controls_tab()
         self.build_disc_finding_controls_tab()
         self.build_plot_settings_controls_tab()
         self.build_coords_tab()
@@ -518,22 +529,23 @@
         menu.pack()
         self.notebook.add(menu, text='Settings')
 
         # Image
         frame = ttk.LabelFrame(menu, text='Observation')
         frame.pack(fill='x', pady=5)
         frame.grid_columnconfigure(0, weight=1)
-        PlotImageSetting(
+        self.image_setting = PlotImageSetting(
             self,
             frame,
             'image',
             label='Observed image',
             hint='the image of your observation',
             callbacks=[self.replot_image],
         )
+        self.ui_callbacks[None].add(self.image_setting.update_tool_ui_state)
 
         # Plot features
         frame = ttk.LabelFrame(menu, text='Plotted features')
         frame.pack(fill='x', pady=5)
         frame.grid_columnconfigure(0, weight=1)
         PlotLineSetting(self, frame, 'limb', label='Limb', hint='the target\'s limb')
         PlotLineSetting(
@@ -956,14 +968,18 @@
 
     # Plotting
     def update_plot(self, print_coords: bool = False) -> None:
         self.get_observation().update_transform()
         self.canvas.draw()
         self.update_coords(print_coords=print_coords)
 
+    def update_only_image(self) -> None:
+        self.replot_image()
+        self.canvas.draw()
+
     def build_plot(self) -> None:
         self.fig = plt.figure()
         self.ax = self.fig.add_axes([0.06, 0.03, 0.93, 0.96])
         self.transform = (
             self.get_observation().matplotlib_radec2xy_transform() + self.ax.transData
         )
 
@@ -1025,19 +1041,19 @@
         self.remove_artists('image')
 
         mode = self.plot_settings['_'].setdefault('image_mode', 'single')
         vmin = self.plot_settings['_'].setdefault('image_vmin', 0)
         vmax = self.plot_settings['_'].setdefault('image_vmax', 1)
         limit_type = self.plot_settings['_'].setdefault('image_limit_type', 'absolute')
 
-        image = self.image_modes[mode][0]()  # type: ignore
-
-        if limit_type == 'percentile':
-            vmin = np.nanpercentile(image, vmin)
-            vmax = np.nanpercentile(image, vmax)
+        with utils.ignore_warnings('All-NaN slice encountered'):
+            image = self.image_modes[mode][0]()  # type: ignore
+            if limit_type == 'percentile':
+                vmin = np.nanpercentile(image, vmin)
+                vmax = np.nanpercentile(image, vmax)
 
         self.plot_handles['image'].append(
             self.ax.imshow(
                 image,
                 origin='lower',
                 vmin=vmin,
                 vmax=vmax,
@@ -1193,14 +1209,31 @@
                 self.ax.axhline(y, **self.plot_settings['marked_coord'])
             )
 
     def remove_artists(self, key: PLOT_KEY) -> None:
         while self.plot_handles[key]:
             self.plot_handles[key].pop().remove()
 
+    # Delayed actions
+    def add_delayed_action(self, name: str, ms: int, func: Callable[[], Any]) -> None:
+        self.cancel_delayed_action(name)
+        self.delayed_actions[name] = (
+            func,
+            self.root.after(ms, lambda: self.run_delayed_action(name)),
+        )
+
+    def cancel_delayed_action(self, name: str) -> None:
+        action = self.delayed_actions.pop(name, None)
+        if action:
+            self.root.after_cancel(action[1])
+
+    def run_delayed_action(self, name: str) -> None:
+        func, _ = self.delayed_actions.pop(name)
+        func()
+
     # Image
     def image_sum(self) -> np.ndarray:
         return 100 * utils.normalise(
             np.nansum(self.get_observation().data, axis=0)
         ) ** self.plot_settings['_'].setdefault('image_gamma', 1)
 
     def image_single(self) -> np.ndarray:
@@ -2330,14 +2363,128 @@
             widget.grid(row=row, column=1, sticky='w')
 
     def get_window_size(self) -> str:
         return '350x350'
 
 
 class PlotImageSetting(ArtistSetting):
+    REPLOT_DELAY_MS = 100
+
+    def __init__(
+        self,
+        gui: GUI,
+        parent: tk.Widget,
+        key: PLOT_KEY,
+        label: str | None = None,
+        hint: str | None = None,
+        callbacks: list[Callable[[], None]] | None = None,
+        row: int | None = None,
+    ):
+        super().__init__(gui, parent, key, label, hint, callbacks, row)
+
+        row = parent.grid_size()[1]
+
+        self.tools_frame = ttk.Frame(parent)
+        self.tools_frame.grid(
+            row=row, column=0, columnspan=2, padx=5, pady=5, sticky='nsew'
+        )
+
+        general_settings = self.gui.plot_settings['_']
+        self.single_wavelength_enabled = tk.IntVar(
+            value=int(general_settings.setdefault('image_mode', 'single') == 'single')
+        )
+        self.wavelength_variable = tk.IntVar(
+            value=int(general_settings.setdefault('image_idx_single', 0))
+        )
+
+        self.single_wavelength_checkbutton = ttk.Checkbutton(
+            self.tools_frame,
+            text='Single wavelength',
+            variable=self.single_wavelength_enabled,
+        )
+        self.single_wavelength_checkbutton.pack()
+
+        self.wavelength_slider = ttk.Scale(
+            self.tools_frame,
+            variable=self.wavelength_variable,
+            from_=0,
+            to=self.gui.get_observation().data.shape[0],
+        )
+        self.wavelength_slider.pack(fill='x')
+
+        self.enabled.trace_add('write', self.update_tool_ui_state)
+        self.single_wavelength_enabled.trace_add(
+            'write', self.on_single_wavelength_checkbutton_change
+        )
+        self.wavelength_variable.trace_add('write', self.on_wavelength_slider_change)
+
+        self.gui.add_tooltip(
+            self.single_wavelength_checkbutton,
+            'Toggle displaying single wavelength or average of all wavelengths (click Edit for more options)',
+        )
+        self.gui.add_tooltip(
+            self.wavelength_slider,
+            'Change displayed wavelength (click Edit for more options)',
+        )
+
+        self.in_tool_updating_state = False
+        self.update_tool_ui_state()
+
+    def on_single_wavelength_checkbutton_change(self, *_) -> None:
+        if self.in_tool_updating_state or self.gui.get_observation().data.shape[0] < 2:
+            return
+        is_single = bool(self.single_wavelength_enabled.get())
+        self.gui.plot_settings['_']['image_mode'] = 'single' if is_single else 'sum'
+        self.schedule_replot(skip_full_delay=True)
+
+    def on_wavelength_slider_change(self, *_) -> None:
+        if self.in_tool_updating_state or self.gui.get_observation().data.shape[0] < 2:
+            return
+
+        wavelength_idx = self.wavelength_variable.get()
+        if not self.single_wavelength_enabled.get():
+            # tick the checkbox if user changes the slider value
+            if wavelength_idx != self.gui.plot_settings['_']['image_idx_single']:
+                self.single_wavelength_enabled.set(1)
+
+        self.gui.plot_settings['_']['image_idx_single'] = wavelength_idx
+        self.schedule_replot()
+
+    def schedule_replot(self, skip_full_delay: bool = False) -> None:
+        self.gui.add_delayed_action(
+            'update_only_image',
+            1 if skip_full_delay else self.REPLOT_DELAY_MS,
+            self.gui.update_only_image,
+        )
+
+    def update_tool_ui_state(self, *_) -> None:
+        self.in_tool_updating_state = True
+        try:
+            general_settings = self.gui.plot_settings['_']
+            n_wavelengths = self.gui.get_observation().data.shape[0]
+
+            enable = self.enabled.get() and n_wavelengths > 1
+            is_single_wavelength = bool(
+                general_settings.setdefault('image_mode', 'single') == 'single'
+            )
+            wavelength_idx = int(general_settings.setdefault('image_idx_single', 0))
+
+            self.single_wavelength_enabled.set(int(is_single_wavelength))
+            self.wavelength_variable.set(wavelength_idx)
+
+            self.single_wavelength_checkbutton.configure(
+                state='normal' if enable else 'disable',
+            )
+            self.wavelength_slider.configure(
+                to=n_wavelengths - 1,
+                state='normal' if enable else 'disable',
+            )
+        finally:
+            self.in_tool_updating_state = False
+
     def make_menu(self) -> None:
         settings = self.gui.plot_settings[self.key]
         general_settings = self.gui.plot_settings['_']
 
         self.cmap = tk.StringVar(value=settings.setdefault('cmap', 'gray'))
 
         self.image_vmin = tk.StringVar(
@@ -2488,15 +2635,15 @@
                 'so set vmin=0 and vmax=100 to show the',
                 'entire dynamic range.',
                 '',
                 'Set vmin/vmax type to "percentile" to',
                 'calculate the limits as percentiles of the',
                 'data in the image. This can be useful if',
                 'your data has extreme outliers (e.g. try',
-                'vmin=1, vmax=99, type=percentile).',
+                'vmin=1, vmax=99 & type=percentile).',
             ]
         )
         ttk.Label(self.grid_frame, text=msg).pack()
 
         self.image_mode.trace_add('write', self.change_image_mode_radio)
         self.change_image_mode_radio()  # run initial setup
 
@@ -2506,17 +2653,20 @@
             if mode in modes:
                 widget['state'] = 'readonly' if '_readonly' in modes else 'normal'
             else:
                 widget['state'] = 'disable'
 
     def get_idx(self, stirng_variable: tk.StringVar, name: str) -> int:
         sz = self.gui.get_observation().data.shape[0]
-        return self.get_int(
+        value = self.get_int(
             stirng_variable, name=name, positive=False, minimum=-sz, maximum=sz - 1
         )
+        if value < 0:
+            value = sz - value
+        return value
 
     def apply_settings(self) -> bool:
         settings = {}
         general_settings = {}
         try:
             image_mode = self.image_mode.get()
             general_settings['image_mode'] = image_mode
@@ -2565,14 +2715,15 @@
                     message=f'Unrecognised matplotlib colormap {self.cmap.get()!r}',
                 )
                 return False
             settings['cmap'] = cmap
 
         self.gui.plot_settings[self.key].update(settings)
         self.gui.plot_settings['_'].update(general_settings)
+        self.update_tool_ui_state()
         return True
 
     def get_window_size(self) -> str:
         return '350x600'
 
 
 class PlotLineSetting(ArtistSetting):
@@ -3081,19 +3232,19 @@
             ('Pan', None, 'move', 'pan'),
             ('Zoom', None, 'zoom_to_rect', 'zoom'),
             (None, None, None, None),
             ('Save', None, 'filesave', 'save_figure'),
         )
         super().__init__(canvas, window, pack_toolbar=pack_toolbar)
         try:
-            self._message_label.configure(foreground='#666666')
+            self._message_label.configure(foreground='#666666')  # type: ignore
         except:
             pass
         try:
-            for name, button in self._buttons.items():
+            for name, button in self._buttons.items():  # type: ignore
                 # Get default tooltips from super() and use them
                 for text, tooltip_text, image_file, callback in super().toolitems:
                     if text == name:
                         hint = tooltip_text.replace('\n', ', ')
                         gui.add_tooltip(button, hint)
                         break
         except:
```

### Comparing `planetmapper-1.6.2/planetmapper/kernel_downloader.py` & `planetmapper-1.6.3/planetmapper/kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/observation.py` & `planetmapper-1.6.3/planetmapper/observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/progress.py` & `planetmapper-1.6.3/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/planetmapper/utils.py` & `planetmapper-1.6.3/planetmapper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,30 @@
     Returns:
         String representting the degress, minutes, seconds of the angle.
     """
     d, m, s = decimal_degrees_to_dms(decimal_degrees)
     return f'{d}°{m}′{s:{seconds_fmt}}″'
 
 
+class ignore_warnings(warnings.catch_warnings):
+    """
+    Context manager to ignore general warnings using warnings.filterwarnings.
+    """
+
+    def __init__(self, *warining_strings: str, **kwargs):
+        super().__init__(**kwargs)
+        self.warning_strings = warining_strings
+
+    def __enter__(self):
+        out = super().__enter__()
+        for ws in self.warning_strings:
+            warnings.filterwarnings('ignore', ws)
+        return out
+
+
 class filter_fits_comment_warning(warnings.catch_warnings):
     """
     Context manager to hide FITS `Card is too long, comment will be truncated` warnings.
     """
 
     def __enter__(self):
         out = super().__enter__()
```

### Comparing `planetmapper-1.6.2/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.6.3/planetmapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.6.2
+Version: 1.6.3
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
```

### Comparing `planetmapper-1.6.2/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.6.3/planetmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/setup.py` & `planetmapper-1.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/tests/test_base.py` & `planetmapper-1.6.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/tests/test_basic_body.py` & `planetmapper-1.6.3/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/tests/test_body.py` & `planetmapper-1.6.3/tests/test_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/tests/test_body_xy.py` & `planetmapper-1.6.3/tests/test_body_xy.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/tests/test_init.py` & `planetmapper-1.6.3/tests/test_init.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,12 +4,18 @@
 from packaging import version
 
 
 class TestInit(unittest.TestCase):
     def test_init(self):
         self.assertEqual(planetmapper.__author__, 'Oliver King')
         self.assertEqual(planetmapper.__url__, 'https://github.com/ortk95/planetmapper')
-        self.assertTrue(
-            version.Version(planetmapper.__version__) > version.Version('1.0')
-        )
+
+    def test_version(self):
         self.assertEqual(planetmapper.__version__.count('.'), 2)
         self.assertEqual(planetmapper.__version__.strip(), planetmapper.__version__)
+
+        self.assertGreater(
+            version.Version(planetmapper.__version__), version.Version('1.6.2')
+        )
+        self.assertEqual(
+            str(version.Version(planetmapper.__version__)), planetmapper.__version__
+        )
```

### Comparing `planetmapper-1.6.2/tests/test_observation.py` & `planetmapper-1.6.3/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.2/tests/test_utils.py` & `planetmapper-1.6.3/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -50,14 +50,37 @@
                 self.assertEqual(
                     utils.decimal_degrees_to_dms_str(
                         decimal_degrees, seconds_fmt='.4f'
                     ),
                     dms_str,
                 )
 
+    def test_ignore_warnings(self):
+        warning_string1 = 'test warning string'
+        warning_string2 = 'test warning string 2'
+
+        with warnings.catch_warnings():
+            warnings.simplefilter('always')
+            with self.assertWarns(UserWarning):
+                warnings.warn(warning_string1, UserWarning)
+
+        with warnings.catch_warnings():
+            warnings.simplefilter('error')
+            with utils.ignore_warnings(warning_string1):
+                warnings.warn(warning_string1, UserWarning)
+
+            with utils.ignore_warnings(warning_string1, warning_string2):
+                warnings.warn(warning_string1, UserWarning)
+                warnings.warn(warning_string1, UserWarning)
+
+        with warnings.catch_warnings():
+            warnings.simplefilter('always')
+            with self.assertWarns(UserWarning):
+                warnings.warn(warning_string1, UserWarning)
+
     def test_filter_fits_comment_warning(self):
         card = (
             'KEY',
             'value',
             'A very very long comment that will create a warning because the card is too long',
         )
         with warnings.catch_warnings():
@@ -70,14 +93,21 @@
         with warnings.catch_warnings():
             warnings.simplefilter('error')
             with utils.filter_fits_comment_warning():
                 header = fits.Header()
                 header.append(card)
                 header.tostring()
 
+        with warnings.catch_warnings():
+            warnings.simplefilter('always')
+            with self.assertWarns(UserWarning):
+                header = fits.Header()
+                header.append(card)
+                header.tostring()
+
     def test_normalise(self):
         pairs = [
             [[1, 2, 3], array([0.0, 0.5, 1.0])],
             [[[nan, -99], [1.23, 45.6]], array([[nan, 0.0], [0.69315353, 1.0]])],
             [[1, 1, 1], array([0, 0, 0])],
         ]
         for a, b in pairs:
```

