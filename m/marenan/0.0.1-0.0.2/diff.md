# Comparing `tmp/marenan-0.0.1-py3-none-any.whl.zip` & `tmp/marenan-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 2231 bytes, number of entries: 10
--rw-rw-r--  2.0 unx       26 b- defN 23-Apr-20 17:30 marenan/__init__.py
--rw-rw-r--  2.0 unx       59 b- defN 23-Apr-20 17:53 marenan/__main__.py
--rw-rw-r--  2.0 unx       71 b- defN 23-Apr-20 17:21 marenan/marenanDay.py
+Zip file size: 3098 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx       26 b- defN 23-Apr-20 20:07 marenan/__init__.py
+-rw-rw-r--  2.0 unx       61 b- defN 23-Apr-20 20:13 marenan/__main__.py
+-rw-rw-r--  2.0 unx       74 b- defN 23-Apr-20 23:42 marenan/marenanDay.py
 -rw-rw-r--  2.0 unx       19 b- defN 23-Apr-20 17:51 marenan/cli/__init__.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Apr-20 17:47 marenan/cli/main.py
--rw-rw-r--  2.0 unx       52 b- defN 23-Apr-20 17:58 marenan-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 17:58 marenan-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       45 b- defN 23-Apr-20 17:58 marenan-0.0.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-20 17:58 marenan-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      766 b- defN 23-Apr-20 17:58 marenan-0.0.1.dist-info/RECORD
-10 files, 1236 bytes uncompressed, 911 bytes compressed:  26.3%
+-rw-rw-r--  2.0 unx     1948 b- defN 23-Apr-21 00:01 marenan-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-21 00:01 marenan-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       45 b- defN 23-Apr-21 00:01 marenan-0.0.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-21 00:01 marenan-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      768 b- defN 23-Apr-21 00:01 marenan-0.0.2.dist-info/RECORD
+10 files, 3139 bytes uncompressed, 1778 bytes compressed:  43.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: marenan/cli/__init__.py
 Comment: 
 
 Filename: marenan/cli/main.py
 Comment: 
 
-Filename: marenan-0.0.1.dist-info/METADATA
+Filename: marenan-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: marenan-0.0.1.dist-info/WHEEL
+Filename: marenan-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: marenan-0.0.1.dist-info/entry_points.txt
+Filename: marenan-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: marenan-0.0.1.dist-info/top_level.txt
+Filename: marenan-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: marenan-0.0.1.dist-info/RECORD
+Filename: marenan-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## marenan/__main__.py

```diff
@@ -1,4 +1,4 @@
 from .cli import main
 
-if __name__ == '__main__':
-  main()
+if __name__ == "__main__":
+    main()
```

## marenan/marenanDay.py

```diff
@@ -1,4 +1,5 @@
 import datetime
 
+
 def marenanDay():
-  return datetime.date(2022, 6, 24)
+    return datetime.date(2022, 6, 24)
```

## Comparing `marenan-0.0.1.dist-info/RECORD` & `marenan-0.0.2.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 marenan/__init__.py,sha256=hsTqpnMNsguVjxZQinao32IDvwIASXdpmD4bIYJPHH0,26
-marenan/__main__.py,sha256=_ynNFJI9KysRKvgIHOjrC8pkwjc-7aUmDb0PBIkYDHs,59
-marenan/marenanDay.py,sha256=Z2lj9D90MliDax-hdeRKQr2d6wAWJRvZm51rzrtDHIU,71
+marenan/__main__.py,sha256=MSmt_5Xg84uHqzTN38JwgseJK8rsJn_11A8WD99VtEo,61
+marenan/marenanDay.py,sha256=Br9w-EcBY_FthiY2DMuRobTV8m2SCXlWWjTGkKyL8jo,74
 marenan/cli/__init__.py,sha256=zDr350exO14Ii8Pj3TXwPuRxIDrEjrg43CpjYABDqh4,19
 marenan/cli/main.py,sha256=6LgFinDmkI1f-LXxgHe__gCFD0MeykYxC1mAPRPRshY,98
-marenan-0.0.1.dist-info/METADATA,sha256=WLREn8Iob91_Kikj2s4k9HnbGZON_Uw99X4CEt0Logs,52
-marenan-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-marenan-0.0.1.dist-info/entry_points.txt,sha256=QtPRLIDoBjjYj_xYiYu_gREtYjpidM3kIkRgiuTRC1k,45
-marenan-0.0.1.dist-info/top_level.txt,sha256=PSlGSVsUOqQozUV-_CI3SDRqjuMLxtEccej6_KqAwAg,8
-marenan-0.0.1.dist-info/RECORD,,
+marenan-0.0.2.dist-info/METADATA,sha256=V1VMitWEprzy1BdOTuIIx0PTuuOuAs6fsrMVrmpfYZs,1948
+marenan-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+marenan-0.0.2.dist-info/entry_points.txt,sha256=QtPRLIDoBjjYj_xYiYu_gREtYjpidM3kIkRgiuTRC1k,45
+marenan-0.0.2.dist-info/top_level.txt,sha256=PSlGSVsUOqQozUV-_CI3SDRqjuMLxtEccej6_KqAwAg,8
+marenan-0.0.2.dist-info/RECORD,,
```

