# Comparing `tmp/mpserializer-1.0.1-py3-none-any.whl.zip` & `tmp/mpserializer-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -4,12 +4,12 @@
 -rw-rw-rw-  2.0 fat     1815 b- defN 23-Apr-19 22:52 serializers/serializer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-07 18:47 serializers/parsers/__init__.py
 -rw-rw-rw-  2.0 fat     3767 b- defN 23-Apr-07 18:47 serializers/parsers/json_parser.py
 -rw-rw-rw-  2.0 fat      447 b- defN 23-Apr-14 08:43 serializers/parsers/parser_factory_method.py
 -rw-rw-rw-  2.0 fat      273 b- defN 23-Apr-07 18:47 serializers/parsers/pickle_parser.py
 -rw-rw-rw-  2.0 fat     2823 b- defN 23-Apr-19 22:26 serializers/parsers/toml_parser.py
 -rw-rw-rw-  2.0 fat     4862 b- defN 23-Apr-07 18:47 serializers/parsers/yaml_parser.py
--rw-rw-rw-  2.0 fat      274 b- defN 23-Apr-20 19:13 mpserializer-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 19:13 mpserializer-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       32 b- defN 23-Apr-20 19:13 mpserializer-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1111 b- defN 23-Apr-20 19:13 mpserializer-1.0.1.dist-info/RECORD
+-rw-rw-rw-  2.0 fat      274 b- defN 23-Apr-20 19:27 mpserializer-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 19:27 mpserializer-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       32 b- defN 23-Apr-20 19:27 mpserializer-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1111 b- defN 23-Apr-20 19:27 mpserializer-1.0.2.dist-info/RECORD
 13 files, 19798 bytes uncompressed, 5408 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: serializers/parsers/toml_parser.py
 Comment: 
 
 Filename: serializers/parsers/yaml_parser.py
 Comment: 
 
-Filename: mpserializer-1.0.1.dist-info/METADATA
+Filename: mpserializer-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: mpserializer-1.0.1.dist-info/WHEEL
+Filename: mpserializer-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: mpserializer-1.0.1.dist-info/top_level.txt
+Filename: mpserializer-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mpserializer-1.0.1.dist-info/RECORD
+Filename: mpserializer-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mpserializer-1.0.1.dist-info/RECORD` & `mpserializer-1.0.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 serializers/serializer.py,sha256=GVk64ZSmFsNg1QhB-XHCcwEn9Uyw4ZLiU-OEbfnuL94,1815
 serializers/parsers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 serializers/parsers/json_parser.py,sha256=UucE2M1SKYr6a0H3JFEfQS4s2MkRvgLYGukebmto39A,3767
 serializers/parsers/parser_factory_method.py,sha256=5bXQgYnAakDvGknORX9OpbHIY_pX1gjE0TJz0MkYYDM,447
 serializers/parsers/pickle_parser.py,sha256=BqthoPcNPCvIRZz-ig4GymUAGJygotdvYY4dfmvDBfI,273
 serializers/parsers/toml_parser.py,sha256=CMRT8SnEYwtTEfBK97PKnLdTVrTb2eZ4mUHmnoxFudk,2823
 serializers/parsers/yaml_parser.py,sha256=y5gKAyZbd6oLgidCnOkZCAkRMAghQjVH5XTah35vmns,4862
-mpserializer-1.0.1.dist-info/METADATA,sha256=S8Iq8CYyofa6GdP-8S1pUxulIDrld5i1s0lGWBRkLQI,274
-mpserializer-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mpserializer-1.0.1.dist-info/top_level.txt,sha256=TYwEAa24xBPItbKqqw25hW6z8gEGmN2yEcioxSye9LM,32
-mpserializer-1.0.1.dist-info/RECORD,,
+mpserializer-1.0.2.dist-info/METADATA,sha256=fVOWLhAvaUuPvushPs9N1DQuO87b5KYb-BiK2vqpJtU,274
+mpserializer-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mpserializer-1.0.2.dist-info/top_level.txt,sha256=TYwEAa24xBPItbKqqw25hW6z8gEGmN2yEcioxSye9LM,32
+mpserializer-1.0.2.dist-info/RECORD,,
```

