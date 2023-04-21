# Comparing `tmp/xia_scw_instance-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_instance-0.0.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 103389 bytes, number of entries: 12
--rw-r--r--  2.0 unx      107 b- defN 23-Apr-21 11:31 xia_scw_instance/__init__.py
--rw-r--r--  2.0 unx   241152 b- defN 23-Apr-21 13:47 xia_scw_instance/instance.cp39-win_amd64.pyd
+Zip file size: 103412 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      107 b- defN 23-Apr-21 16:02 xia_scw_instance/__init__.py
+-rw-r--r--  2.0 unx   241152 b- defN 23-Apr-21 16:12 xia_scw_instance/instance.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/backend.tf
 -rw-rw-rw-  2.0 unx      125 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/main.tf
 -rw-rw-rw-  2.0 unx      393 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/output.tf
 -rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/provider.tf
--rw-rw-rw-  2.0 unx      954 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-21 13:47 xia_scw_instance-0.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      699 b- defN 23-Apr-21 13:47 xia_scw_instance-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-21 13:47 xia_scw_instance-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-21 13:47 xia_scw_instance-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1143 b- defN 23-Apr-21 13:47 xia_scw_instance-0.0.5.dist-info/RECORD
-12 files, 245253 bytes uncompressed, 101407 bytes compressed:  58.7%
+-rw-rw-rw-  2.0 unx     1063 b- defN 23-Apr-21 16:02 xia_scw_instance/templates/ScwInstance/variables.tf
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-21 16:12 xia_scw_instance-0.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-21 16:12 xia_scw_instance-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-21 16:12 xia_scw_instance-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-21 16:12 xia_scw_instance-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1144 b- defN 23-Apr-21 16:12 xia_scw_instance-0.0.6.dist-info/RECORD
+12 files, 245363 bytes uncompressed, 101430 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xia_scw_instance/templates/ScwInstance/provider.tf
 Comment: 
 
 Filename: xia_scw_instance/templates/ScwInstance/variables.tf
 Comment: 
 
-Filename: xia_scw_instance-0.0.5.dist-info/LICENSE.txt
+Filename: xia_scw_instance-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.5.dist-info/METADATA
+Filename: xia_scw_instance-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_instance-0.0.5.dist-info/WHEEL
+Filename: xia_scw_instance-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_instance-0.0.5.dist-info/top_level.txt
+Filename: xia_scw_instance-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.5.dist-info/RECORD
+Filename: xia_scw_instance-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_instance/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_instance.instance import ScwInstance
 
 
 __all__ = [
     "ScwInstance"
 ]
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## xia_scw_instance/templates/ScwInstance/variables.tf

```diff
@@ -1,40 +1,40 @@
-variable "project_id" {
+variable "state" {
   type = string
   default = null  #xia#
-  #xia# default = {% if project_id is not none %}"{{ project_id }}"{% else %}null{% endif %}
+  #xia# default = {% if state is defined and state is not none %}"{{ state }}"{% else %}null{% endif %}
 
 }
 
-variable "name" {
+variable "project_id" {
   type = string
   default = null  #xia#
-  #xia# default = {% if name is not none %}"{{ name }}"{% else %}null{% endif %}
+  #xia# default = {% if project_id is defined and project_id is not none %}"{{ project_id }}"{% else %}null{% endif %}
 
 }
 
-variable "type" {
+variable "name" {
   type = string
   default = null  #xia#
-  #xia# default = {% if type is not none %}"{{ type }}"{% else %}null{% endif %}
+  #xia# default = {% if name is defined and name is not none %}"{{ name }}"{% else %}null{% endif %}
 
 }
 
-variable "image" {
+variable "type" {
   type = string
   default = null  #xia#
-  #xia# default = {% if image is not none %}"{{ image }}"{% else %}null{% endif %}
+  #xia# default = {% if type is defined and type is not none %}"{{ type }}"{% else %}null{% endif %}
 
 }
 
-variable "state" {
+variable "image" {
   type = string
   default = null  #xia#
-  #xia# default = {% if state is not none %}"{{ state }}"{% else %}null{% endif %}
+  #xia# default = {% if image is defined and image is not none %}"{{ image }}"{% else %}null{% endif %}
 
 }
 
 variable "tags" {
     type = list(string)
     default = null  #xia#
     #xia# default = [{% for v in tags %}{% if loop.index > 1 %}, {% endif %}{% if v is not none %}"{{ v }}"{% else %}null{% endif %}{% endfor %}]
-}
+}
```

## Comparing `xia_scw_instance-0.0.5.dist-info/METADATA` & `xia_scw_instance-0.0.6.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-scw-instance
-Version: 0.0.5
+Version: 0.0.6
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.5/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.6/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_scw_instance-0.0.5.dist-info/RECORD` & `xia_scw_instance-0.0.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_scw_instance/__init__.py,sha256=x8GIV4H7RkQWjahnoO3wjrK35kFMceBAY1yHj_GMcR8,107
-xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=5USFdzZr2ryWrhmLSw2qs_gtKDdrR5wHFW-HhysEp8w,241152
+xia_scw_instance/__init__.py,sha256=p_ZHqzr1KIOCdNcGj0z0GiP6hRV-asHhgqEjx1pdJVQ,107
+xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=HdZwnFOlL9dwiFoQiV-7MzIltDdeWh0PsO4ch_Csm6g,241152
 xia_scw_instance/templates/ScwInstance/backend.tf,sha256=E6fgAX-nMcTt9oErRKvK67uJPdB-O77YJpzAvf06zgs,69
 xia_scw_instance/templates/ScwInstance/main.tf,sha256=JEF3C2keRHR4Yf1jq-1InkD_1cltym9iVQiwMuDGOL4,125
 xia_scw_instance/templates/ScwInstance/output.tf,sha256=zYgmsP0Q8ibCaLmRYDM7BJl6n39qURGPhcS_DhQUvJU,393
 xia_scw_instance/templates/ScwInstance/provider.tf,sha256=h_zFGas7QtYJPGvufLGuPHtgDhoZa28Qa5t--1dpheI,343
-xia_scw_instance/templates/ScwInstance/variables.tf,sha256=EYYhTpbQeOfZoGHVFSkhun-d13iUYTmybW-yvSwiN1Y,954
-xia_scw_instance-0.0.5.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
-xia_scw_instance-0.0.5.dist-info/METADATA,sha256=cvlScs8RDREJgLzaXf0TscHWY6LbGBLtW3GD2Fqn-94,699
-xia_scw_instance-0.0.5.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_instance-0.0.5.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
-xia_scw_instance-0.0.5.dist-info/RECORD,,
+xia_scw_instance/templates/ScwInstance/variables.tf,sha256=tjh2NHOT-v9dTpc0c4FTaGrE8y9Gfm4ME8eVbI2To1g,1063
+xia_scw_instance-0.0.6.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
+xia_scw_instance-0.0.6.dist-info/METADATA,sha256=wghaLDFEyszPvMF2EpyGfwz_L3T4a4uFFLJJGCwZYvg,699
+xia_scw_instance-0.0.6.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_scw_instance-0.0.6.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
+xia_scw_instance-0.0.6.dist-info/RECORD,,
```

