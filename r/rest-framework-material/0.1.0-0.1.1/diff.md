# Comparing `tmp/rest_framework_material-0.1.0.tar.gz` & `tmp/rest_framework_material-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_material-0.1.0.tar", max compression
+gzip compressed data, was "rest_framework_material-0.1.1.tar", max compression
```

## Comparing `rest_framework_material-0.1.0.tar` & `rest_framework_material-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-21 17:36:10.988103 rest_framework_material-0.1.0/LICENSE
--rw-r--r--   0        0        0      589 2023-04-21 17:39:31.096785 rest_framework_material-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      749 2023-04-21 17:40:45.269789 rest_framework_material-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_material-0.1.0/rest_framework_material/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_material-0.1.0/rest_framework_material/admin.py
--rw-r--r--   0        0        0      248 2023-04-21 17:38:09.789518 rest_framework_material-0.1.0/rest_framework_material/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_material-0.1.0/rest_framework_material/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_material-0.1.0/rest_framework_material/models.py
--rw-r--r--   0        0        0    23750 2023-04-20 09:09:17.444650 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1085 2023-04-20 09:11:06.989223 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4375 2023-04-18 08:11:26.812363 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_material-0.1.0/rest_framework_material/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_material-0.1.0/rest_framework_material/views.py
--rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 rest_framework_material-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-21 17:36:10.988103 rest_framework_material-0.1.1/LICENSE
+-rw-r--r--   0        0        0      589 2023-04-21 17:51:54.543587 rest_framework_material-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      749 2023-04-21 17:40:45.269789 rest_framework_material-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_material-0.1.1/rest_framework_material/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_material-0.1.1/rest_framework_material/admin.py
+-rw-r--r--   0        0        0      248 2023-04-21 17:38:09.789518 rest_framework_material-0.1.1/rest_framework_material/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_material-0.1.1/rest_framework_material/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_material-0.1.1/rest_framework_material/models.py
+-rw-r--r--   0        0        0    23552 2023-04-21 17:30:40.413795 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1181 2023-04-21 17:25:31.881402 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     4252 2023-04-21 17:33:58.678317 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_material-0.1.1/rest_framework_material/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_material-0.1.1/rest_framework_material/views.py
+-rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 rest_framework_material-0.1.1/PKG-INFO
```

### Comparing `rest_framework_material-0.1.0/LICENSE` & `rest_framework_material-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/pyproject.toml` & `rest_framework_material-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-material"
-version = "0.1.0"
+version = "0.1.1"
 description = "Redesign of the browsable api of Django REST Framework using MD Bootstrap"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_material"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
```

### Comparing `rest_framework_material-0.1.0/README.md` & `rest_framework_material-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/api.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/api.html`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 {% block meta %}
   {{ block.super }}
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
 {% endblock %}
 
 {% block style %}
   {% block bootstrap_theme %}
-    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet"
-      integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
+    <link href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap"rel="stylesheet"/>
+    <link href="https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.2.0/mdb.min.css" rel="stylesheet" />
+
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.4/font/bootstrap-icons.css">
     <link rel="stylesheet" href="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.7.0/build/styles/default.min.css">
   {% endblock %}
 
   <style>
     {% if code_style %}
       {{ code_style }}
@@ -31,22 +32,24 @@
   <header class="fixed-top">
     <div class="bg-danger py-2 shadow">
       <nav class="navbar navbar-expand-lg navbar-dark bg-dark {% block bootstrap_navbar_variant %}{% endblock %}"
         role="navigation" aria-label="{% translate 'navbar' %}">
         <div class="container">
           {% block branding %}
             <a class="navbar-brand" rel="nofollow" href="https://www.django-rest-framework.org/">
-                <strong>{% translate 'Django REST Framework' %}</strong>
+              <strong>{% translate 'Django REST Framework' %}</strong>
             </a>
           {% endblock %}
 
-          <button type="button" class="navbar-toggler" data-bs-toggle="collapse"
-            data-bs-target="#navbar" aria-controls="navbar" aria-expanded="false"
+          <button type="button" class="navbar-toggler" data-mdb-toggle="collapse"
+            data-mdb-target="#navbar" aria-controls="navbar" aria-expanded="false"
             aria-label="Toggle navigation">
-            <span class="navbar-toggler-icon"></span>
+            <span class="navbar-toggler-icon d-flex align-items-center justify-content-center">
+              <i class="bi bi-three-dots-vertical fs-3"></i>
+            </span>
           </button>
 
           <div class="collapse navbar-collapse" id="navbar">
             <ul class="navbar-nav me-auto">
               <li class="nav-item">
                 <a href="https://www.django-rest-framework.org/" class="nav-link">
                   <strong class="d-flex align-items-center gap-3">
@@ -78,26 +81,31 @@
                     {% translate "Redesign" %}
                   </strong>
                 </a>
               </li>
             </ul>
             <ul class="navbar-nav">
               <li class="nav-item dropdown">
-                <a href="#" class="nav-link" data-bs-toggle="dropdown">
+                <a href="#" class="nav-link" data-mdb-toggle="dropdown">
                   <strong class="d-flex align-items-center gap-3">
                     <i class="bi bi-person-fill"></i>
                     {% if user.is_authenticated %}
                       {{ request.user|capfirst }}
                     {% else %}
                       {% translate "Account" %}
                     {% endif %}
                     <i class="bi bi-chevron-down"></i>
                   </strong>
                 </a>
-                <ul class="dropdown-menu dropdown-menu-dark dropdown-menu-end rounded-3 shadow">
+                <ul class="dropdown-menu dropdown-menu-end rounded-3 shadow">
+                  <li>
+                    <h5 class="dropdown-header">
+                      {% translate 'Account' %}
+                    </h5>
+                  </li>
                   <li>
                     {% if user.is_authenticated %}
                       <a class="dropdown-item" href="{% url 'rest_framework:logout' %}">
                         <strong class="d-flex align-items-center gap-3">
                           <i class="bi bi-box-arrow-right"></i>
                           {% translate 'Logout' %}
                         </strong>
@@ -174,15 +182,15 @@
                     title="Make a GET request on the {{ name }} resource">
                     <strong class="d-flex align-items-center justify-content-center gap-3">
                       <i class="bi bi-arrow-clockwise"></i>
                       {% translate "GET" %}
                     </strong>
                   </a>
                   <button class="btn btn-lg btn-outline-primary dropdown-toggle" type="button" id="dropdownMenuButton"
-                    data-bs-toggle="dropdown" aria-expanded="false">
+                    data-mdb-toggle="dropdown" aria-expanded="false">
                     <i class="bi bi-chevron-down"></i>
                   </button>
                   <div class="dropdown">
                     <ul class="dropdown-menu dropdown-menu-end rounded-3 shadow" aria-labelledby="dropdownMenuButton">
                       <li>
                         <h6 class="dropdown-header">
                           {% translate 'Select a format' %}
@@ -211,26 +219,26 @@
               {% endif %}
             </fieldset>
           </form>
         {% endif %}
 
         {% if options_form %}
           <form class="button-form" action="{{ request.get_full_path }}" data-method="OPTIONS">
-            <button type="submit" class="btn btn-lg btn-secondary w-100" title="Make an OPTIONS request on the {{ name }} resource">
+            <button type="submit" class="btn btn-lg btn-warning w-100" title="Make an OPTIONS request on the {{ name }} resource">
               <strong class="d-flex align-items-center justify-content-center gap-3">
                 <i class="bi bi-info-square"></i>
                 {% translate "OPTIONS" %}
               </strong>
             </button>
           </form>
         {% endif %}
 
         {% if delete_form %}
           <div>
-            <button type="button" class="btn btn-lg btn-danger w-100" data-bs-toggle="modal" data-bs-target="#deleteModal"
+            <button type="button" class="btn btn-lg btn-danger w-100" data-mdb-toggle="modal" data-mdb-target="#deleteModal"
               title="Make a DELETE request on the {{ name }} resource">
               <strong class="d-flex align-items-center justify-content-center gap-3">
                 <i class="bi bi-trash"></i>
                 {% translate "DELETE" %}
               </strong>
             </button>
           </div>
@@ -238,45 +246,45 @@
           <div class="modal fade" id="deleteModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
             <div class="modal-dialog modal-dialog-centered">
               <div class="modal-content p-md-3 p-lg-4 rounded-4 shadow">
                 <div class="modal-header border-bottom-0">
                   <h3 class="modal-title" id="exampleModalLabel">
                     {% translate 'Delete' %} {{ name }}
                   </h3>
-                  <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
+                  <button type="button" class="btn-close" data-mdb-dismiss="modal" aria-label="Close"></button>
                 </div>
                 <div class="modal-body">
                   <p class="mb-4">
                     {% translate "Are you sure you want to delete this" %} {{ name }}?
                   </p>
                   <div class="d-grid d-lg-flex align-items-lg-center gap-4">
                     <form class="button-form w-100" action="{{ request.get_full_path }}" data-method="DELETE">
                       <button class="btn btn-lg btn-danger w-100">
                         <strong class="d-flex align-item-center justify-content-center gap-3">
                           <i class="bi bi-trash"></i>
                           {% translate "Delete" %}
                         </strong>
                       </button>
                     </form>
-                    <button type="button" class="btn btn-lg btn-outline-secondary w-100" data-bs-dismiss="modal">
+                    <button type="button" class="btn btn-lg btn-secondary w-100" data-mdb-dismiss="modal">
                       <strong class="d-flex align-item-center justify-content-center gap-3">
                         <i class="bi bi-x-lg"></i>
                         {% translate "Cancel" %}
                       </strong>
                     </button>
                   </div>
                 </div>
               </div>
             </div>
           </div>
         {% endif %}
 
         {% if extra_actions %}
           <div class="dropdown">
-            <button class="btn btn-lg btn-info w-100" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
+            <button class="btn btn-lg btn-info w-100" id="extra-actions-menu" data-mdb-toggle="dropdown" aria-haspopup="true"
               aria-expanded="true">
               <strong class="d-flex align-items-center justify-content-center gap-3">
                 {% translate "Extra Actions" %}
                 <i class="bi bi-chevron-down"></i>
               </strong>
             </button>
             <ul class="dropdown-menu" aria-labelledby="extra-actions-menu">
@@ -288,15 +296,15 @@
                 </li>
               {% endfor %}
             </ul>
           </div>
         {% endif %}
 
         {% if filter_form %}
-          <button data-bs-toggle="modal" data-bs-target="#filtersModal" class="btn btn-lg btn-success">
+          <button data-mdb-toggle="modal" data-mdb-target="#filtersModal" class="btn btn-lg btn-success">
             <strong class="d-flex align-items-center justify-content-center gap-3">
               <i class="bi bi-filter"></i>
               {% translate "Filters" %}
             </strong>
           </button>
         {% endif %}
       </section>
@@ -314,29 +322,28 @@
           </div>
         </div>
       </section>
 
       <section class="col-12 col-lg-4">
         {% if display_edit_forms %}
           {% if post_form or raw_data_post_form %}
-            <div {% if post_form %}class="card card-body rounded-3" {% endif %}>
+            <div {% if post_form %}class="card card-body rounded-3"{% endif %}>
               {% if post_form %}
-                <ul class="nav nav-pills nav-fill gap-2 p-1 small bg-dark rounded-5 shadow mb-4" role="tablist"
-                  style="--bs-nav-link-color: var(--bs-danger); --bs-nav-pills-link-active-color: var(--bs-white); --bs-nav-pills-link-active-bg: var(--bs-danger);">
+                <ul class="nav nav-pills gap-4 nav-fill mb-4" role="tablist">
                   <li class="nav-item" role="presentation">
-                    <button class="nav-link active rounded-5" id="form-tab" data-bs-toggle="tab" data-bs-target="#form"
+                    <button class="nav-link active rounded-5 w-100 m-0" id="form-tab" data-mdb-toggle="tab" data-mdb-target="#form"
                       type="button" role="tab" aria-controls="form" aria-selected="true">
                       <strong class="d-flex align-items-center justify-content-center gap-3">
                         <i class="bi bi-filetype-html"></i>
                         {% translate 'HTML form' %}
                       </strong>
                     </button>
                   </li>
                   <li class="nav-item" role="presentation">
-                    <button class="nav-link rounded-5" id="raw-tab" data-bs-toggle="tab" data-bs-target="#raw"
+                    <button class="nav-link rounded-5 w-100 m-0" id="raw-tab" data-mdb-toggle="tab" data-mdb-target="#raw"
                       type="button" role="tab" aria-controls="raw" aria-selected="false">
                       <strong class="d-flex align-items-center justify-content-center gap-3">
                         <i class="bi bi-filetype-json"></i>
                         {% translate 'Raw data' %}
                       </strong>
                     </button>
                   </li>
@@ -386,27 +393,26 @@
               </div>
             </div>
           {% endif %}
 
           {% if put_form or raw_data_put_form or raw_data_patch_form %}
             <div {% if put_form %}class="card card-body rounded-3"{% endif %}>
               {% if put_form %}
-                <ul class="nav nav-pills nav-fill gap-2 p-1 small bg-dark rounded-5 shadow mb-4" role="tablist"
-                  style="--bs-nav-link-color: var(--bs-danger); --bs-nav-pills-link-active-color: var(--bs-white); --bs-nav-pills-link-active-bg: var(--bs-danger);">
+                <ul class="nav nav-pills gap-4 nav-fill mb-4" role="tablist">
                   <li class="nav-item" role="presentation">
-                    <button class="nav-link active rounded-5" id="form-tab" data-bs-toggle="tab" data-bs-target="#put-object-form"
+                    <button class="nav-link active rounded-5 w-100 m-0" id="form-tab" data-mdb-toggle="tab" data-mdb-target="#put-object-form"
                       type="button" role="tab" aria-controls="form" aria-selected="true">
                       <strong class="d-flex align-items-center justify-content-center gap-3">
                         <i class="bi bi-filetype-html"></i>
                         {% translate 'HTML form' %}
                       </strong>
                     </button>
                   </li>
                   <li class="nav-item" role="presentation">
-                    <button class="nav-link rounded-5" id="raw-tab" data-bs-toggle="tab" data-bs-target="#put-generic-content-form"
+                    <button class="nav-link rounded-5 w-100 m-0" id="raw-tab" data-mdb-toggle="tab" data-mdb-target="#put-generic-content-form"
                       type="button" role="tab" aria-controls="raw" aria-selected="false">
                       <strong class="d-flex align-items-center justify-content-center gap-3">
                         <i class="bi bi-filetype-json"></i>
                         {% translate 'Raw data' %}
                       </strong>
                     </button>
                   </li>
@@ -487,13 +493,11 @@
   <script src="{% static "rest_framework/js/prettify-min.js" %}"></script>
   <script src="{% static "rest_framework/js/default.js" %}"></script>
   <script>
     $(document).ready(function() {
       $('form').ajaxForm();
     });
   </script>
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
-    integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe"
-    crossorigin="anonymous"></script>
+  <script type="text/javascript"src="https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.2.0/mdb.min.js"></script>
   <script src="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.7.0/build/highlight.min.js"></script>
   <script>hljs.highlightAll()</script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
 {% extends "rest_framework/base.html" %} {% load i18n static rest_framework %}
 {% block meta %} {{ block.super }}
  {% endblock %} {% block style %} {% block bootstrap_theme %}
 
 
+
  {% endblock %}
  {% endblock %} {% block navbar %}
 {% block branding %} {%_translate_'Django_REST_Framework'_%} {% endblock %}
     *  {%_translate_"Home"_%}
     *  {%_translate_"Tutorial"_%}
     *  {%_translate_"Github"_%}
     *  {%_translate_"Redesign"_%}
     *  {%_if_user.is_authenticated_%}_{{_request.user|capfirst_}}_{%_else_%}_{%
       translate_"Account"_%}_{%_endif_%}
+          o ** {% translate 'Account' %} **
           o {% if user.is_authenticated %}
              {%_translate_'Logout'_%}
              {% else %}
              {%_translate_'Login'_%}
              {% endif %}
  {% endblock %} {% block breadcrumbs %}
    1. {% for breadcrumb_name, breadcrumb_url in breadcrumblist %} {% if
@@ -71,15 +73,15 @@
 {{ request.method }} {{ request.get_full_path }}
 HTTP {{ response.status_code }} {{ response.status_text }}
 {% for key, val in response_headers|items %}
 {{ key }}: {{ val|break_long_headers|urlize }}
 {% endfor %}
 {{ content|urlize }}
   {% if display_edit_forms %} {% if post_form or raw_data_post_form %}
-% if post_form %}class="card card-body rounded-3" {% endif %}> {% if post_form
+% if post_form %}class="card card-body rounded-3"{% endif %}> {% if post_form
 %}
     *
        {% translate 'HTML form' %}
 
     *
        {% translate 'Raw data' %}
```

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/filters/ordering.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/filters/search.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/input.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/radio.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/select.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/horizontal/textarea.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/login.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/login.html`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 {% block meta %}
   {{ block.super }}
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
 {% endblock %}
 
 {% block style %}
   {% block bootstrap_theme %}
-    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet"
-      integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
+    <link href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap"rel="stylesheet"/>
+    <link href="https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.2.0/mdb.min.css" rel="stylesheet" />
+
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.4/font/bootstrap-icons.css">
   {% endblock %}
 
   {% if code_style %}<style>{{ code_style }}</style>{% endif %}
 {% endblock %}
 
 {% block body %}
@@ -91,11 +92,9 @@
   <script src="{% static "rest_framework/js/prettify-min.js" %}"></script>
   <script src="{% static "rest_framework/js/default.js" %}"></script>
   <script>
     $(document).ready(function() {
       $('form').ajaxForm();
     });
   </script>
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
-    integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe"
-    crossorigin="anonymous"></script>
+  <script type="text/javascript"src="https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.2.0/mdb.min.js"></script>
 {% endblock %}
```

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/pagination/numbers.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_material-0.1.1/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.0/PKG-INFO` & `rest_framework_material-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-material
-Version: 0.1.0
+Version: 0.1.1
 Summary: Redesign of the browsable api of Django REST Framework using MD Bootstrap
 Home-page: https://github.com/youzarsiph/rest-framework-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

