# Comparing `tmp/easy_mvp-0.1.2.tar.gz` & `tmp/easy_mvp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_mvp-0.1.2.tar", last modified: Mon Apr 17 19:25:21 2023, max compression
+gzip compressed data, was "easy_mvp-0.2.0.tar", last modified: Fri Apr 21 20:36:14 2023, max compression
```

## Comparing `easy_mvp-0.1.2.tar` & `easy_mvp-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:25:21.921742 easy_mvp-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-17 19:25:21.921742 easy_mvp-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 19:25:21.925742 easy_mvp-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:25:21.921742 easy_mvp-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:25:21.921742 easy_mvp-0.1.2/src/easy_mvp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/abstract_presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/application_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:25:21.921742 easy_mvp-0.1.2/src/easy_mvp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-17 19:25:21.000000 easy_mvp-0.1.2/src/easy_mvp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-17 19:25:21.000000 easy_mvp-0.1.2/src/easy_mvp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:25:21.000000 easy_mvp-0.1.2/src/easy_mvp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 19:25:21.000000 easy_mvp-0.1.2/src/easy_mvp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 19:25:21.000000 easy_mvp-0.1.2/src/easy_mvp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:36:14.347905 easy_mvp-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-21 20:36:03.000000 easy_mvp-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-21 20:36:14.347905 easy_mvp-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-04-21 20:36:03.000000 easy_mvp-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-21 20:36:03.000000 easy_mvp-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-21 20:36:14.347905 easy_mvp-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:36:14.343905 easy_mvp-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:36:14.343905 easy_mvp-0.2.0/src/easy_mvp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:36:03.000000 easy_mvp-0.2.0/src/easy_mvp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-21 20:36:03.000000 easy_mvp-0.2.0/src/easy_mvp/abstract_presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-21 20:36:03.000000 easy_mvp-0.2.0/src/easy_mvp/application_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-21 20:36:03.000000 easy_mvp-0.2.0/src/easy_mvp/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-21 20:36:03.000000 easy_mvp-0.2.0/src/easy_mvp/intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-04-21 20:36:03.000000 easy_mvp-0.2.0/src/easy_mvp/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:36:14.347905 easy_mvp-0.2.0/src/easy_mvp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-21 20:36:14.000000 easy_mvp-0.2.0/src/easy_mvp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-21 20:36:14.000000 easy_mvp-0.2.0/src/easy_mvp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:36:14.000000 easy_mvp-0.2.0/src/easy_mvp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 20:36:14.000000 easy_mvp-0.2.0/src/easy_mvp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 20:36:14.000000 easy_mvp-0.2.0/src/easy_mvp.egg-info/top_level.txt
```

### Comparing `easy_mvp-0.1.2/LICENSE` & `easy_mvp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_mvp-0.1.2/PKG-INFO` & `easy_mvp-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_mvp
-Version: 0.1.2
+Version: 0.2.0
 Summary: Construct MVP PyQt5 application easily
 Home-page: https://github.com/R0land013/easy-mvp
 Author: Rolando Rio Garaboa
 Author-email: rolandorio06@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,14 @@
 To install this package you need to have **Python** installed in your system.
 Then you can run this command to install this package:
 
 ````shell script
 pip install easy_mvp
 ````
 
-
 ## Explaining the mechanism
 
 The following explanations are reflected in ``demo.py`` program.
 
 ### The application model created by **easy_mvp** is like this:
 
 ![App Manager and windows](https://github.com/R0land013/easy-mvp/blob/master/readme_img/app_manager_and_windows.png?raw=true)
@@ -68,25 +67,24 @@
 classes must **inherit from the AbstractPresenter** class.
 
 **AbstractPresenter** has several methods to open new presenters,
 close the current presenter and to handle certain flows within the
 application, such as when a presenter is going to be initialized, hidden,
 or closed.
 
-
 ### The flow of events in a class that inherits from AbstractPresenter is like this:
 
 ![flow_of_calls_on_presenter](https://github.com/R0land013/easy-mvp/blob/b2c8ba51e5315679848925967611e1e5931871dd/readme_img/flow_of_calls_on_presenter.png?raw=true)
 
 The **_on_initialize** method is the first method called in the **AbstractPresenter** class.
 Here the instance variables of the presenter must be initialized. Also, you must
 create the instance of the view that corresponds to the presenter. Once created,
 the view instance must be set with the **_set_view(view)** method, from
 this way the view is made accessible to the rest of the classes in **easy_mvp environment**.
-The view can be obtained with the **get_view** method of **AbstractPresenter**, if it was set
+The view can be obtained with the **view** property or **get_view** method of **AbstractPresenter**, if it was set
 by **_set_view(view)** first.
 
 The **on_view_shown** method is called just after the presenter view
 is displayed in the graphical interface. In this method the data should be loaded,
 and the tables and forms filled.
 
 If on the presenter whose view is visible, **_open_other_presenter** is called
@@ -108,52 +106,48 @@
 removed, and it will happen what it has been explained previously.
 It should be noted that if the presenter who closes is the
 only one that exists in the entire application, that is, there is only one
 window, and it owns only a presenter then the application will close with
 the **status code 0**. To close the program with different code, use the **exit_app**
 method of AbstractPresenter.
 
-
 ### Receiving data from presenters
 
 A presenter can receive data from another presenter that it has created,
 if the second one is closed using the **_close_this_presenter_with_result(result_data: dict, result: str = Intent.NO_RESULT)**
 method. In this way, the presenter that is below in the stack receives control of the
 program via **on_view_discovered_with_result(action: str, data: dict, result: str)** instead of
 **on_view_discovered**. The action parameter is the action that was passed to the **Intent** when
 it was ordered to open the new presenter. The result_data is a **Python dictionary** that the
 presenter who was on top can pass through
 **_close_this_presenter_with_result(result_data: dict, result: str = Intent.NO_RESULT)**. The result string can be used
 to tell the below presenter what happened on top presenter. In this way the below presenter can take different decisions
 depending on the result returned by top presenter.
 
-
 ### Managing global data
 
 Data can be created to be accessible throughout the entire application. This is
 accomplished with the **set_global_data(key: str, data)** and **get_global_data(key: str)**
 methods of **AbstractPresenter**. You can also check if a global data exists with the method
 **has_global_data(key: str)**, which returns True if it exists and False otherwise.
 
-
 ## Knowing Intent in depth
 
 As explained **Intent** is what makes it possible to open new presenters. You can specify
 that the new presenter must be opened on a new window using
 **use_new_window(use_new_window: bool = False)**. You can also specify that
 if a new window is to be opened, then make it modal or not with the method
 **use_modal(self, modal: bool = False)**.
 
 An intent can be specified with an action with **set_action(action: str)**, like so
 the new presenter may behave differently depending on the action received.
 
 **Intent** also allows data to be passed to a new presenter via **set_data(data: dict)**.
 To see examples of how **Intent** is used, check out the ``demo.py`` program.
 
-
 ## Acting when user closes window
 
 If the user clicks the close window button then all presenters in the
 presenter stack of the window will receive the **on_window_closing(self)**
 call. The first presenter to receive the call will be the one which is
 on the stack top, the next to receive the call will be the below presenter.
 This flow of calls will occur all the way down through the window stack.
@@ -161,28 +155,39 @@
 window will be closed. If the window that is being closing has child
 windows, then all its children will receive the **on_window_closing(self)**
 calls in the same way the parent window received it.
 
 This method is useful to close database connections, close files and
 stop threads. All you must close goes here.
 
-
-
 ## Customize window title
 
 Every presenter can change the window title. This is useful because each presenter will do
 a different task, and therefore you would like to change the title of the window depending
 on it.
 
 You can reimplement the method **get_default_window_title(self)** to set a custom
 window title. You only have to set **return 'My custom window title'** in the method's
 body. This method will be called before the presenter receives the
 ***on_view_show***, ***on_view_discovered*** and ***on_view_discovered_with_result*** calls.
 By default, this method returns the *'No Title, reimplement get_default_window_title'* string.
 
-
 But if you want more power on changing the window title you can use the
 **_set_window_title(self, window_title: str)** to immediately change it. After calling
 this method the window title can be replaced automatically if the presenter who set it is popped,
 or if a new presenter is added on top. This will happen because of the calls to
 **get_default_window_title(self)** on below presenter or on the new presenter respectively,
 during the **easy-mvp** event flow.
+
+## Setting application name and window Icon
+
+You can set the application name and Window Icon by passing this information to
+ApplicationManager constructor:
+
+````python
+manager = ApplicationManager(
+    app_name='easy_mvp demo',
+    window_icon_path='./demo/view/ui/assets/icon.png'
+)
+````
+
+This way the operating system will know the name of your app and its window icon.
```

### Comparing `easy_mvp-0.1.2/README.md` & `easy_mvp-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 To install this package you need to have **Python** installed in your system.
 Then you can run this command to install this package:
 
 ````shell script
 pip install easy_mvp
 ````
 
-
 ## Explaining the mechanism
 
 The following explanations are reflected in ``demo.py`` program.
 
 ### The application model created by **easy_mvp** is like this:
 
 ![App Manager and windows](https://github.com/R0land013/easy-mvp/blob/master/readme_img/app_manager_and_windows.png?raw=true)
@@ -55,25 +54,24 @@
 classes must **inherit from the AbstractPresenter** class.
 
 **AbstractPresenter** has several methods to open new presenters,
 close the current presenter and to handle certain flows within the
 application, such as when a presenter is going to be initialized, hidden,
 or closed.
 
-
 ### The flow of events in a class that inherits from AbstractPresenter is like this:
 
 ![flow_of_calls_on_presenter](https://github.com/R0land013/easy-mvp/blob/b2c8ba51e5315679848925967611e1e5931871dd/readme_img/flow_of_calls_on_presenter.png?raw=true)
 
 The **_on_initialize** method is the first method called in the **AbstractPresenter** class.
 Here the instance variables of the presenter must be initialized. Also, you must
 create the instance of the view that corresponds to the presenter. Once created,
 the view instance must be set with the **_set_view(view)** method, from
 this way the view is made accessible to the rest of the classes in **easy_mvp environment**.
-The view can be obtained with the **get_view** method of **AbstractPresenter**, if it was set
+The view can be obtained with the **view** property or **get_view** method of **AbstractPresenter**, if it was set
 by **_set_view(view)** first.
 
 The **on_view_shown** method is called just after the presenter view
 is displayed in the graphical interface. In this method the data should be loaded,
 and the tables and forms filled.
 
 If on the presenter whose view is visible, **_open_other_presenter** is called
@@ -95,52 +93,48 @@
 removed, and it will happen what it has been explained previously.
 It should be noted that if the presenter who closes is the
 only one that exists in the entire application, that is, there is only one
 window, and it owns only a presenter then the application will close with
 the **status code 0**. To close the program with different code, use the **exit_app**
 method of AbstractPresenter.
 
-
 ### Receiving data from presenters
 
 A presenter can receive data from another presenter that it has created,
 if the second one is closed using the **_close_this_presenter_with_result(result_data: dict, result: str = Intent.NO_RESULT)**
 method. In this way, the presenter that is below in the stack receives control of the
 program via **on_view_discovered_with_result(action: str, data: dict, result: str)** instead of
 **on_view_discovered**. The action parameter is the action that was passed to the **Intent** when
 it was ordered to open the new presenter. The result_data is a **Python dictionary** that the
 presenter who was on top can pass through
 **_close_this_presenter_with_result(result_data: dict, result: str = Intent.NO_RESULT)**. The result string can be used
 to tell the below presenter what happened on top presenter. In this way the below presenter can take different decisions
 depending on the result returned by top presenter.
 
-
 ### Managing global data
 
 Data can be created to be accessible throughout the entire application. This is
 accomplished with the **set_global_data(key: str, data)** and **get_global_data(key: str)**
 methods of **AbstractPresenter**. You can also check if a global data exists with the method
 **has_global_data(key: str)**, which returns True if it exists and False otherwise.
 
-
 ## Knowing Intent in depth
 
 As explained **Intent** is what makes it possible to open new presenters. You can specify
 that the new presenter must be opened on a new window using
 **use_new_window(use_new_window: bool = False)**. You can also specify that
 if a new window is to be opened, then make it modal or not with the method
 **use_modal(self, modal: bool = False)**.
 
 An intent can be specified with an action with **set_action(action: str)**, like so
 the new presenter may behave differently depending on the action received.
 
 **Intent** also allows data to be passed to a new presenter via **set_data(data: dict)**.
 To see examples of how **Intent** is used, check out the ``demo.py`` program.
 
-
 ## Acting when user closes window
 
 If the user clicks the close window button then all presenters in the
 presenter stack of the window will receive the **on_window_closing(self)**
 call. The first presenter to receive the call will be the one which is
 on the stack top, the next to receive the call will be the below presenter.
 This flow of calls will occur all the way down through the window stack.
@@ -148,28 +142,39 @@
 window will be closed. If the window that is being closing has child
 windows, then all its children will receive the **on_window_closing(self)**
 calls in the same way the parent window received it.
 
 This method is useful to close database connections, close files and
 stop threads. All you must close goes here.
 
-
-
 ## Customize window title
 
 Every presenter can change the window title. This is useful because each presenter will do
 a different task, and therefore you would like to change the title of the window depending
 on it.
 
 You can reimplement the method **get_default_window_title(self)** to set a custom
 window title. You only have to set **return 'My custom window title'** in the method's
 body. This method will be called before the presenter receives the
 ***on_view_show***, ***on_view_discovered*** and ***on_view_discovered_with_result*** calls.
 By default, this method returns the *'No Title, reimplement get_default_window_title'* string.
 
-
 But if you want more power on changing the window title you can use the
 **_set_window_title(self, window_title: str)** to immediately change it. After calling
 this method the window title can be replaced automatically if the presenter who set it is popped,
 or if a new presenter is added on top. This will happen because of the calls to
 **get_default_window_title(self)** on below presenter or on the new presenter respectively,
-during the **easy-mvp** event flow.
+during the **easy-mvp** event flow.
+
+## Setting application name and window Icon
+
+You can set the application name and Window Icon by passing this information to
+ApplicationManager constructor:
+
+````python
+manager = ApplicationManager(
+    app_name='easy_mvp demo',
+    window_icon_path='./demo/view/ui/assets/icon.png'
+)
+````
+
+This way the operating system will know the name of your app and its window icon.
```

### Comparing `easy_mvp-0.1.2/setup.cfg` & `easy_mvp-0.2.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easy_mvp
-version = 0.1.2
+version = 0.2.0
 author = Rolando Rio Garaboa
 author_email = rolandorio06@gmail.com
 description = Construct MVP PyQt5 application easily
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/R0land013/easy-mvp
 classifiers =
```

### Comparing `easy_mvp-0.1.2/src/easy_mvp/abstract_presenter.py` & `easy_mvp-0.2.0/src/easy_mvp/abstract_presenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,18 @@
     def __init__(self, intent: Intent, window, app_manager):
         self.__intent = intent
         self.__window_handler = window
         self.__app_manager = app_manager
         self.__view = None
         self._on_initialize()
 
+    @property
+    def view(self):
+        return self.__view
+
     def get_view(self):
         return self.__view
 
     def _set_view(self, view):
         self.__view = view
 
     def _open_other_presenter(self, intent: Intent):
```

### Comparing `easy_mvp-0.1.2/src/easy_mvp/application_manager.py` & `easy_mvp-0.2.0/src/easy_mvp/application_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from PyQt5.QtWidgets import QApplication
 from easy_mvp.abstract_presenter import AbstractPresenter
 from easy_mvp.exception import NoGlobalDataWithKeyException
 from easy_mvp.intent import Intent
 from easy_mvp.window import WindowHandler
-
+import sys
 
 class ApplicationManager:
 
-    def __init__(self):
+    def __init__(self, app_name: str = 'No Name', window_icon_path: str = None):
         self.__window_stack = []
-        self.__app = QApplication([])
+        self.__app = QApplication(sys.argv)
         self.__global_data = {}
+        self.__window_icon_path = window_icon_path
+
+        self.__app.setApplicationName(app_name)
 
     def add_new_window(self, intent: Intent, parent_window: WindowHandler, calling_presenter: AbstractPresenter):
         window = WindowHandler(self, parent_window)
         window.add_presenter(intent, calling_presenter)
         self.__window_stack.append(window)
         window.show()
 
     def remove_window(self, window: WindowHandler):
         self.__window_stack.remove(window)
 
     def execute_app(self, initial_intent: Intent):
-        window = WindowHandler(self)
+        window = WindowHandler(self, window_icon_path=self.__window_icon_path)
         window.add_presenter(initial_intent)
 
         self.__window_stack.append(window)
         window.show()
         self.__app.exec()
 
     def exit(self, code: int = 0):
```

### Comparing `easy_mvp-0.1.2/src/easy_mvp/exception.py` & `easy_mvp-0.2.0/src/easy_mvp/exception.py`

 * *Files identical despite different names*

### Comparing `easy_mvp-0.1.2/src/easy_mvp/intent.py` & `easy_mvp-0.2.0/src/easy_mvp/intent.py`

 * *Files identical despite different names*

### Comparing `easy_mvp-0.1.2/src/easy_mvp/window.py` & `easy_mvp-0.2.0/src/easy_mvp/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtGui import QCloseEvent
+from PyQt5.QtGui import QCloseEvent, QIcon
 from PyQt5.QtWidgets import QStackedWidget
 from PyQt5.QtCore import Qt
 from easy_mvp.abstract_presenter import AbstractPresenter
 from easy_mvp.exception import BelowPresenterDoingCommandsException, NoBelowPresenterToBeNotifiedWithResultException
 from easy_mvp.intent import Intent
 
 
@@ -20,21 +20,22 @@
             self.__already_notified_on_closing = True
             self.__window_handler.close_handler_and_send_all_notifications()
 
 
 
 class WindowHandler:
 
-    def __init__(self, application_manager, parent_window=None):
+    def __init__(self, application_manager, parent_window=None, window_icon_path: str = None):
         self.__presenter_stack = []
         self.__parent_window = None
         self.__link_to_parent_window(parent_window)
         self.__stacked_widget = StackWindow(self)
         self.__app_manager = application_manager
         self.__child_windows = []
+        self.__window_icon_path = window_icon_path
 
     def __link_to_parent_window(self, parent_window):
         if parent_window is not None:
             parent_window.add_child_window(self)
         self.__parent_window = parent_window
 
     def get_base_widget(self) -> QStackedWidget:
@@ -72,16 +73,16 @@
         if calling_presenter is not None:
             calling_presenter.on_view_covered()
 
     def __add_presenter_and_its_view(self, intent: Intent):
         presenter_class = intent.get_presenter_class()
         new_presenter = presenter_class(intent, self, self.__app_manager)
         self.__presenter_stack.append(new_presenter)
-        self.__stacked_widget.addWidget(new_presenter.get_view())
-        self.__stacked_widget.setCurrentWidget(new_presenter.get_view())
+        self.__stacked_widget.addWidget(new_presenter.view)
+        self.__stacked_widget.setCurrentWidget(new_presenter.view)
 
     def update_window_title(self):
         top_presenter_title = self.get_top_presenter().get_default_window_title()
         self.__stacked_widget.setWindowTitle(top_presenter_title)
 
     def __notify_top_presenter_on_view_shown(self):
         self.get_top_presenter().on_view_shown()
@@ -90,15 +91,15 @@
         return self.__presenter_stack[-1]
 
     def pop_presenter(self, calling_presenter: AbstractPresenter) -> AbstractPresenter:
         self.__check_is_top_presenter(calling_presenter)
 
         top_presenter = self.__pop_presenter_and_its_view()
         top_presenter.on_closing_presenter()
-        top_presenter.get_view().deleteLater()
+        top_presenter.view.deleteLater()
 
         was_window_closed = self.__close_window_if_no_presenter_remains()
         if was_window_closed and self.has_parent_window():
             self.__parent_window.update_window_title()
             presenter_of_parent_window = self.__parent_window.get_top_presenter()
             presenter_of_parent_window.on_view_discovered()
         elif self.presenter_count() >= 1:
@@ -108,15 +109,15 @@
         else:
             self.__app_manager.exit()
 
         return top_presenter
 
     def __pop_presenter_and_its_view(self) -> AbstractPresenter:
         top_presenter = self.__presenter_stack.pop(-1)
-        self.__stacked_widget.removeWidget(top_presenter.get_view())
+        self.__stacked_widget.removeWidget(top_presenter.view)
         return top_presenter
 
     def __notify_presenter_on_view_discovered(self):
         if len(self.__presenter_stack) >= 1:
             below_presenter = self.get_top_presenter()
             below_presenter.on_view_discovered()
 
@@ -153,15 +154,15 @@
 
     def pop_presenter_with_result(self, intent: Intent, calling_presenter: AbstractPresenter, result_data: dict, result: str):
         self.__check_is_top_presenter(calling_presenter)
         self.__check_there_is_below_presenter_to_be_notified_with_result()
 
         top_presenter = self.__pop_presenter_and_its_view()
         top_presenter.on_closing_presenter()
-        top_presenter.get_view().deleteLater()
+        top_presenter.view.deleteLater()
 
         was_window_closed = self.__close_window_if_no_presenter_remains()
         if was_window_closed:
             self.__parent_window.update_window_title()
             self.__notify_presenter_on_discovered_with_result_on_parent_window(intent, result_data, result)
         else:
             self.update_window_title()
@@ -179,14 +180,16 @@
         parent_window_presenter.on_view_discovered_with_result(intent.get_action(), result_data, result)
 
     def __notify_below_presenter_on_discovered_with_result(self, intent: Intent, result_data: dict, result: str):
         below_presenter = self.get_top_presenter()
         below_presenter.on_view_discovered_with_result(intent.get_action(), result_data, result)
 
     def show(self):
+        if self.__window_icon_path:
+            self.__stacked_widget.setWindowIcon(QIcon(self.__window_icon_path))
         self.__stacked_widget.show()
 
     def exit_app(self, code: int = 0):
         self.__app_manager.exit(code)
 
     def close_all_child_windows(self):
         while len(self.__child_windows) > 0:
```

### Comparing `easy_mvp-0.1.2/src/easy_mvp.egg-info/PKG-INFO` & `easy_mvp-0.2.0/src/easy_mvp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-mvp
-Version: 0.1.2
+Version: 0.2.0
 Summary: Construct MVP PyQt5 application easily
 Home-page: https://github.com/R0land013/easy-mvp
 Author: Rolando Rio Garaboa
 Author-email: rolandorio06@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,14 @@
 To install this package you need to have **Python** installed in your system.
 Then you can run this command to install this package:
 
 ````shell script
 pip install easy_mvp
 ````
 
-
 ## Explaining the mechanism
 
 The following explanations are reflected in ``demo.py`` program.
 
 ### The application model created by **easy_mvp** is like this:
 
 ![App Manager and windows](https://github.com/R0land013/easy-mvp/blob/master/readme_img/app_manager_and_windows.png?raw=true)
@@ -68,25 +67,24 @@
 classes must **inherit from the AbstractPresenter** class.
 
 **AbstractPresenter** has several methods to open new presenters,
 close the current presenter and to handle certain flows within the
 application, such as when a presenter is going to be initialized, hidden,
 or closed.
 
-
 ### The flow of events in a class that inherits from AbstractPresenter is like this:
 
 ![flow_of_calls_on_presenter](https://github.com/R0land013/easy-mvp/blob/b2c8ba51e5315679848925967611e1e5931871dd/readme_img/flow_of_calls_on_presenter.png?raw=true)
 
 The **_on_initialize** method is the first method called in the **AbstractPresenter** class.
 Here the instance variables of the presenter must be initialized. Also, you must
 create the instance of the view that corresponds to the presenter. Once created,
 the view instance must be set with the **_set_view(view)** method, from
 this way the view is made accessible to the rest of the classes in **easy_mvp environment**.
-The view can be obtained with the **get_view** method of **AbstractPresenter**, if it was set
+The view can be obtained with the **view** property or **get_view** method of **AbstractPresenter**, if it was set
 by **_set_view(view)** first.
 
 The **on_view_shown** method is called just after the presenter view
 is displayed in the graphical interface. In this method the data should be loaded,
 and the tables and forms filled.
 
 If on the presenter whose view is visible, **_open_other_presenter** is called
@@ -108,52 +106,48 @@
 removed, and it will happen what it has been explained previously.
 It should be noted that if the presenter who closes is the
 only one that exists in the entire application, that is, there is only one
 window, and it owns only a presenter then the application will close with
 the **status code 0**. To close the program with different code, use the **exit_app**
 method of AbstractPresenter.
 
-
 ### Receiving data from presenters
 
 A presenter can receive data from another presenter that it has created,
 if the second one is closed using the **_close_this_presenter_with_result(result_data: dict, result: str = Intent.NO_RESULT)**
 method. In this way, the presenter that is below in the stack receives control of the
 program via **on_view_discovered_with_result(action: str, data: dict, result: str)** instead of
 **on_view_discovered**. The action parameter is the action that was passed to the **Intent** when
 it was ordered to open the new presenter. The result_data is a **Python dictionary** that the
 presenter who was on top can pass through
 **_close_this_presenter_with_result(result_data: dict, result: str = Intent.NO_RESULT)**. The result string can be used
 to tell the below presenter what happened on top presenter. In this way the below presenter can take different decisions
 depending on the result returned by top presenter.
 
-
 ### Managing global data
 
 Data can be created to be accessible throughout the entire application. This is
 accomplished with the **set_global_data(key: str, data)** and **get_global_data(key: str)**
 methods of **AbstractPresenter**. You can also check if a global data exists with the method
 **has_global_data(key: str)**, which returns True if it exists and False otherwise.
 
-
 ## Knowing Intent in depth
 
 As explained **Intent** is what makes it possible to open new presenters. You can specify
 that the new presenter must be opened on a new window using
 **use_new_window(use_new_window: bool = False)**. You can also specify that
 if a new window is to be opened, then make it modal or not with the method
 **use_modal(self, modal: bool = False)**.
 
 An intent can be specified with an action with **set_action(action: str)**, like so
 the new presenter may behave differently depending on the action received.
 
 **Intent** also allows data to be passed to a new presenter via **set_data(data: dict)**.
 To see examples of how **Intent** is used, check out the ``demo.py`` program.
 
-
 ## Acting when user closes window
 
 If the user clicks the close window button then all presenters in the
 presenter stack of the window will receive the **on_window_closing(self)**
 call. The first presenter to receive the call will be the one which is
 on the stack top, the next to receive the call will be the below presenter.
 This flow of calls will occur all the way down through the window stack.
@@ -161,28 +155,39 @@
 window will be closed. If the window that is being closing has child
 windows, then all its children will receive the **on_window_closing(self)**
 calls in the same way the parent window received it.
 
 This method is useful to close database connections, close files and
 stop threads. All you must close goes here.
 
-
-
 ## Customize window title
 
 Every presenter can change the window title. This is useful because each presenter will do
 a different task, and therefore you would like to change the title of the window depending
 on it.
 
 You can reimplement the method **get_default_window_title(self)** to set a custom
 window title. You only have to set **return 'My custom window title'** in the method's
 body. This method will be called before the presenter receives the
 ***on_view_show***, ***on_view_discovered*** and ***on_view_discovered_with_result*** calls.
 By default, this method returns the *'No Title, reimplement get_default_window_title'* string.
 
-
 But if you want more power on changing the window title you can use the
 **_set_window_title(self, window_title: str)** to immediately change it. After calling
 this method the window title can be replaced automatically if the presenter who set it is popped,
 or if a new presenter is added on top. This will happen because of the calls to
 **get_default_window_title(self)** on below presenter or on the new presenter respectively,
 during the **easy-mvp** event flow.
+
+## Setting application name and window Icon
+
+You can set the application name and Window Icon by passing this information to
+ApplicationManager constructor:
+
+````python
+manager = ApplicationManager(
+    app_name='easy_mvp demo',
+    window_icon_path='./demo/view/ui/assets/icon.png'
+)
+````
+
+This way the operating system will know the name of your app and its window icon.
```

