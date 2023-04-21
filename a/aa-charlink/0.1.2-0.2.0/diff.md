# Comparing `tmp/aa-charlink-0.1.2.tar.gz` & `tmp/aa-charlink-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-charlink-0.1.2.tar", last modified: Tue Apr 18 07:34:50 2023, max compression
+gzip compressed data, was "aa-charlink-0.2.0.tar", last modified: Fri Apr 21 13:07:54 2023, max compression
```

## Comparing `aa-charlink-0.1.2.tar` & `aa-charlink-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.746011 aa-charlink-0.1.2/aa_charlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/charlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/app_imports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/charlink/imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/imports/corptools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/imports/memberaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/imports/miningtaxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/charlink/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.746011 aa-charlink-0.1.2/charlink/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/charlink/templates/charlink/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/templates/charlink/charlink.html
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/aa_charlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/charlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/app_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/app_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/charlink/imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/corptools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/memberaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/miningtaxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/moonmining.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/moonstuff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/charlink/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.594582 aa-charlink-0.2.0/charlink/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/charlink/templates/charlink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/templates/charlink/charlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/setup.cfg
```

### Comparing `aa-charlink-0.1.2/LICENSE` & `aa-charlink-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.2/PKG-INFO` & `aa-charlink-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 0.1.2
+Version: 0.2.0
 Summary: Character Linker for Alliance Auth
 Home-page: https://github.com/Maestro-Zacht/aa-charlink
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,allianceauth_charlink,charlink,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -50,7 +50,13 @@
    ```
 
 2. Add `'charlink',` to your `INSTALLED_APPS` in `local.py`
 
 ## Current apps
 
 I've opened an [issue](https://github.com/Maestro-Zacht/aa-charlink/issues/1) to track the current apps that are implemented in CharLink and the WIPs. If you want another app to be supported, please comment on the issue or reach me on the [AllianceAuth discord server](https://discord.gg/fjnHAmk).
+
+## Settings
+
+| Name                   | Description                                                                         | Default |
+| ---------------------- | ----------------------------------------------------------------------------------- | ------- |
+| `CHARLINK_IGNORE_APPS` | List of apps to ignore. Use the name of the app as it is called in `INSTALLED_APPS` | `[]`    |
```

### Comparing `aa-charlink-0.1.2/aa_charlink.egg-info/PKG-INFO` & `aa-charlink-0.2.0/aa_charlink.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 0.1.2
+Version: 0.2.0
 Summary: Character Linker for Alliance Auth
 Home-page: https://github.com/Maestro-Zacht/aa-charlink
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,allianceauth_charlink,charlink,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -50,7 +50,13 @@
    ```
 
 2. Add `'charlink',` to your `INSTALLED_APPS` in `local.py`
 
 ## Current apps
 
 I've opened an [issue](https://github.com/Maestro-Zacht/aa-charlink/issues/1) to track the current apps that are implemented in CharLink and the WIPs. If you want another app to be supported, please comment on the issue or reach me on the [AllianceAuth discord server](https://discord.gg/fjnHAmk).
+
+## Settings
+
+| Name                   | Description                                                                         | Default |
+| ---------------------- | ----------------------------------------------------------------------------------- | ------- |
+| `CHARLINK_IGNORE_APPS` | List of apps to ignore. Use the name of the app as it is called in `INSTALLED_APPS` | `[]`    |
```

### Comparing `aa-charlink-0.1.2/aa_charlink.egg-info/SOURCES.txt` & `aa-charlink-0.2.0/aa_charlink.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 aa_charlink.egg-info/SOURCES.txt
 aa_charlink.egg-info/dependency_links.txt
 aa_charlink.egg-info/not-zip-safe
 aa_charlink.egg-info/requires.txt
 aa_charlink.egg-info/top_level.txt
 charlink/__init__.py
 charlink/app_imports.py
+charlink/app_settings.py
 charlink/apps.py
 charlink/auth_hooks.py
 charlink/decorators.py
 charlink/forms.py
 charlink/models.py
 charlink/urls.py
 charlink/views.py
 charlink/imports/__init__.py
 charlink/imports/corptools.py
 charlink/imports/memberaudit.py
 charlink/imports/miningtaxes.py
+charlink/imports/moonmining.py
+charlink/imports/moonstuff.py
+charlink/imports/structures.py
 charlink/migrations/__init__.py
 charlink/templates/charlink/charlink.html
```

### Comparing `aa-charlink-0.1.2/charlink/app_imports.py` & `aa-charlink-0.2.0/charlink/app_imports.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.2/charlink/forms.py` & `aa-charlink-0.2.0/charlink/forms.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from django import forms
 
 from .app_imports import import_apps
+from .app_settings import CHARLINK_IGNORE_APPS
 
 
 class LinkForm(forms.Form):
     add_character = forms.BooleanField(
         required=False,
         initial=True,
         disabled=True,
         label='Add Character (default)'
     )
 
     def __init__(self, user, *args, **kwargs):
         super().__init__(*args, **kwargs)
         for app, data in import_apps().items():
-            if app != 'add_character' and user.has_perms(data['permissions']):
+            if app != 'add_character' and app not in CHARLINK_IGNORE_APPS and user.has_perms(data['permissions']):
                 self.fields[app] = forms.BooleanField(
                     required=False,
                     initial=True,
                     label=data.get('field_label', app)
                 )
```

### Comparing `aa-charlink-0.1.2/charlink/imports/corptools.py` & `aa-charlink-0.2.0/charlink/imports/corptools.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.2/charlink/imports/memberaudit.py` & `aa-charlink-0.2.0/charlink/imports/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.2/charlink/imports/miningtaxes.py` & `aa-charlink-0.2.0/charlink/imports/miningtaxes.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.2/charlink/views.py` & `aa-charlink-0.2.0/charlink/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 from django.contrib import messages
 
 from allianceauth.services.hooks import get_extension_logger
 
 from .forms import LinkForm
 from .app_imports import import_apps
 from .decorators import charlink
+from .app_settings import CHARLINK_IGNORE_APPS
 
 logger = get_extension_logger(__name__)
 
 
 @login_required
 def index(request):
+    imported_apps = import_apps()
+
     if request.method == 'POST':
         form = LinkForm(request.user, request.POST)
         if form.is_valid():
-            imported_apps = import_apps()
+
             scopes = set()
             selected_apps = []
 
             for app, to_import in form.cleaned_data.items():
                 if to_import:
                     scopes.update(imported_apps[app].get('scopes', []))
                     selected_apps.append(app)
@@ -35,28 +38,29 @@
             return redirect('charlink:login')
 
     else:
         form = LinkForm(request.user)
 
     context = {
         'form': form,
+        'apps': [data for app, data in imported_apps.items() if app != 'add_character' and app not in CHARLINK_IGNORE_APPS and request.user.has_perms(data['permissions'])],
     }
 
     return render(request, 'charlink/charlink.html', context=context)
 
 
 @login_required
 @charlink
 def login_view(request, token):
     imported_apps = import_apps()
 
     charlink_data = request.session.pop('charlink')
 
     for app in charlink_data['apps']:
-        if app != 'add_character' and request.user.has_perms(imported_apps[app]['permissions']):
+        if app != 'add_character' and app not in CHARLINK_IGNORE_APPS and request.user.has_perms(imported_apps[app]['permissions']):
             try:
                 imported_apps[app]['add_character'](request, token)
             except Exception as e:
                 logger.exception(e)
                 messages.error(request, f"Failed to add character to {imported_apps[app]['field_label']}")
             else:
                 messages.success(request, f"Character successfully added to {imported_apps[app]['field_label']}")
```

### Comparing `aa-charlink-0.1.2/setup.cfg` & `aa-charlink-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.2
+current_version = 0.2.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(b(?P<beta>\d+))?
 serialize = 
 	{major}.{minor}.{patch}b{beta}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 sign_tags = True
```

