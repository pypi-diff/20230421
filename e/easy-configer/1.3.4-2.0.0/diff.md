# Comparing `tmp/easy_configer-1.3.4.tar.gz` & `tmp/easy_configer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_configer-1.3.4.tar", last modified: Mon Feb 20 02:16:45 2023, max compression
+gzip compressed data, was "easy_configer-2.0.0.tar", last modified: Fri Apr 21 06:56:32 2023, max compression
```

## Comparing `easy_configer-1.3.4.tar` & `easy_configer-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 02:16:45.875495 easy_configer-1.3.4/
--rw-rw-rw-   0        0        0     9658 2023-02-20 02:16:45.874343 easy_configer-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     7399 2022-09-02 14:40:08.000000 easy_configer-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-20 02:16:45.828023 easy_configer-1.3.4/easy_configer/
--rw-rw-rw-   0        0        0     1228 2023-02-08 14:15:35.000000 easy_configer-1.3.4/easy_configer/Argparser.py
--rw-rw-rw-   0        0        0     7407 2023-02-20 02:09:16.000000 easy_configer-1.3.4/easy_configer/Configer.py
--rw-rw-rw-   0        0        0     2023 2023-02-17 13:46:28.000000 easy_configer-1.3.4/easy_configer/IO_Converter.py
-drwxrwxrwx   0        0        0        0 2023-02-20 02:16:45.854305 easy_configer-1.3.4/easy_configer/utils/
--rw-rw-rw-   0        0        0      807 2021-12-30 00:08:34.000000 easy_configer-1.3.4/easy_configer/utils/Flag.py
--rw-rw-rw-   0        0        0     3160 2023-02-05 12:11:55.000000 easy_configer-1.3.4/easy_configer/utils/Type_Convertor.py
-drwxrwxrwx   0        0        0        0 2023-02-20 02:16:45.837158 easy_configer-1.3.4/easy_configer.egg-info/
--rw-rw-rw-   0        0        0     9658 2023-02-20 02:16:44.000000 easy_configer-1.3.4/easy_configer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-02-20 02:16:44.000000 easy_configer-1.3.4/easy_configer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 02:16:44.000000 easy_configer-1.3.4/easy_configer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-02-20 02:16:44.000000 easy_configer-1.3.4/easy_configer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-20 02:16:45.875495 easy_configer-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1056 2023-02-20 02:16:38.000000 easy_configer-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-20 02:16:45.871894 easy_configer-1.3.4/test/
--rw-rw-rw-   0        0        0     3033 2023-02-17 14:05:39.000000 easy_configer-1.3.4/test/test_Configer.py
--rw-rw-rw-   0        0        0     1294 2023-02-17 13:46:35.000000 easy_configer-1.3.4/test/test_IO_Converter.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:56:32.187587 easy_configer-2.0.0/
+-rw-rw-rw-   0        0        0    17635 2023-04-21 06:56:32.186614 easy_configer-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13903 2023-04-21 05:47:34.000000 easy_configer-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 06:56:32.112543 easy_configer-2.0.0/easy_configer/
+-rw-rw-rw-   0        0        0     1456 2023-04-21 05:47:25.000000 easy_configer-2.0.0/easy_configer/Argparser.py
+-rw-rw-rw-   0        0        0     9359 2023-04-12 14:02:36.000000 easy_configer-2.0.0/easy_configer/Configer.py
+-rw-rw-rw-   0        0        0     2023 2023-04-21 05:47:25.000000 easy_configer-2.0.0/easy_configer/IO_Converter.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:56:32.154513 easy_configer-2.0.0/easy_configer/utils/
+-rw-rw-rw-   0        0        0      807 2023-04-21 05:47:25.000000 easy_configer-2.0.0/easy_configer/utils/Flag.py
+-rw-rw-rw-   0        0        0     3160 2023-04-21 05:47:25.000000 easy_configer-2.0.0/easy_configer/utils/Type_Convertor.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:56:32.137911 easy_configer-2.0.0/easy_configer.egg-info/
+-rw-rw-rw-   0        0        0    17635 2023-04-21 06:56:31.000000 easy_configer-2.0.0/easy_configer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-21 06:56:31.000000 easy_configer-2.0.0/easy_configer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 06:56:31.000000 easy_configer-2.0.0/easy_configer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-21 06:56:31.000000 easy_configer-2.0.0/easy_configer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 06:56:32.188588 easy_configer-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-04-21 05:53:21.000000 easy_configer-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:56:32.176076 easy_configer-2.0.0/test/
+-rw-rw-rw-   0        0        0     3033 2023-04-21 05:47:25.000000 easy_configer-2.0.0/test/test_Configer.py
+-rw-rw-rw-   0        0        0     1294 2023-04-21 05:47:25.000000 easy_configer-2.0.0/test/test_IO_Converter.py
```

### Comparing `easy_configer-1.3.4/easy_configer/Argparser.py` & `easy_configer-2.0.0/easy_configer/Argparser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import sys
+from .utils.Type_Convertor import Type_Convertor
 
 class Argparser:
 
     # Update the namespace value via commend-line input 
     @staticmethod
-    def args_from_cmd(cfg_dict):
-
-        def is_long_flag(flag_str):
-            prefix = flag_str[0:2]
-            return True if prefix == "--" else False
-            
+    def args_from_cmd(idx_sec_by_dot):   
         '''
             Update the arguments by commend line input string
         '''
+        # Note that argument key should begin with - symbol for increasing read-ability!
+        def is_arg_key(cmd_str):
+            if cmd_str[0] == '-':
+                return True
+            else:
+                return False
+
+        typ_cnvt = Type_Convertor()
+
         # remove file name from args
         cmd_arg_lst = sys.argv[1:]
-
+        
         # print out helper document string
         if "-h" in cmd_arg_lst:
             cmd_arg_lst.remove("-h")
             print(cfg_dict['_doc_str'])
 
+        sec_ptr, sec_key = None, None
         for idx, item in enumerate(cmd_arg_lst):
-            if idx % 2 == 0:  # argument flag 
-                if is_long_flag(item):
-                    flag = item[2:]
-                    flag_lst = flag.split('-')
-                    sec_key, arg = flag_lst[0], flag_lst[1]
-                else:
-                    arg = item[1:]
-                    sec_key = ""
-                    
-            else:     # argument value 
-                val = item
-                if sec_key == "":
-                    cfg_dict[arg] = val
-                else:
-                    cfg_dict[sec_key][arg] = val
+            if is_arg_key(item):  # argument flag 
+                sec_keys_str = item.split('-')[-1]   # strip - symbol, and get argument key
+                sec_ptr, sec_key = idx_sec_by_dot(sec_keys_str)       
+            else:                # argument value 
+                if idx % 2 == 0:
+                    raise RuntimeError('Commendline argument missing the argument key, note that argument key should begin with - symbol!')
+                val_str = item
+                sec_ptr[sec_key] = typ_cnvt.convert(val_str)
+
```

### Comparing `easy_configer-1.3.4/easy_configer/Configer.py` & `easy_configer-2.0.0/easy_configer/Configer.py`

 * *Files 16% similar despite different names*

```diff
@@ -80,36 +80,58 @@
     # return an absl style flag to store all of the args.
     def get_cfg_flag(self):
         return self.__flag
 
     def get_doc_str(self):
         return self.__doc_str
 
-    def merge_conf(self, cfg, override=False):
-        cfg_dict = cfg.__dict__
-        for sec_key, sec_val in cfg_dict.items():
-            if not override:
-                # prevent checking private vars
-                if ('_' != sec_key[0]) and (sec_key in self.__dict__):
-                    raise RuntimeError(f"Key '{sec_key}' in input config already exists in merged config!!")
-            
-            # same section exists, just update kv pair
-            if isinstance(sec_val, dict) and sec_key in self.__dict__ :    
-                self.__dict__[sec_key].update(sec_val)
-            # else, directly feed new val or sec_dict to container
-            self.__dict__[sec_key] = sec_val
+    # merge conf suppose 2 config have overlap section, otherwise use 'concate' method!
+    def merge_conf(self, cfg, override=True):
+        
+        def hier_merge(sf_dict, cfg_dict):
+            for sec_key, sec_val in cfg_dict.items():
+                # same section exists
+                if sec_key in sf_dict.keys():
+                    if not override:
+                        raise RuntimeError(f"Key '{sec_key}' in input config already exists in merged config!!")
+                    
+                    # if both self-dict and cfg_dict are dict, merge it hierachically!
+                    if isinstance(sec_val, dict) and isinstance(sf_dict[sec_key], dict):
+                        hier_merge(sf_dict[sec_key], sec_val)
+                    else:
+                        sf_dict[sec_key] = sec_val
+
+                # directly feed new val
+                else:
+                    sf_dict[sec_key] = sec_val
+
+        # prevent checking private vars
+        cfg_dict = { k:v for k, v in cfg.__dict__.copy().items() \
+                                    if '_' != k[0] }
+        hier_merge(self.__dict__, cfg_dict)
+    
+    # concate just means merge2conf "without" any override!!
+    def concate_cfg(self, cfg):
+        cp_cfg = deepcopy(self)
+        cp_cfg.merge_conf(cfg, override=False)
+        return cp_cfg
 
-    def concate_cfg(self, cfg, override=False):
+    ## Configuration operator support :
+    #  all of operator will be forced to return value!!
+    # 1. merge operator, force to override!
+    def __or__(self, cfg):
         cp_cfg = deepcopy(self)
-        cp_cfg.merge_conf(cfg, override)
+        cp_cfg.merge_conf(cfg, override=True)
         return cp_cfg
-    # operator support..
+
+    # 2. concate operator 
     def __add__(self, cfg):
         return self.concate_cfg(cfg, override=False)
 
+
     # utils of config parser
     def __preproc_cfgstr(self, cfg_str:str) -> str:
         # eliminate the line full of white-space without any text
         cfg_str = cfg_str.strip() 
         # skip empty line and comment line 
         if len(cfg_str) == 0 or cfg_str[0] == '#': 
             return ''
@@ -119,16 +141,34 @@
     def __get_sec(self, cfg_str:str) -> str:
         if '[' != cfg_str[0]:
             return ''
         # more robust with Indented section
         beg, end = cfg_str.find('['), cfg_str.rfind(']')
         if end == -1:
             raise RuntimeError("Configuration Error : Invalid section notation, missing ']' at end of line")
-        sec_key = cfg_str[beg+1 : end].strip()
-        return sec_key
+        sec_key_str = cfg_str[beg+1 : end].strip()
+        return sec_key_str
+    
+    def __idx_sec_by_dot(self, sec_keys_str:str) -> [dict, str]:
+        sec_name_lst = sec_keys_str.split('.')
+        # Before easy_configer 1.3.4 ver, all section is builded upon this level
+        if len(sec_name_lst) == 1:
+            return self.__dict__, sec_keys_str
+
+        ## Support toml like 'hierachical' format!!
+        #  dynamically search the hierachical section begin from the 'next layer' of self.__dict__
+        idx_sec = self.__dict__[ sec_name_lst.pop(0) ]
+        #  keep the index point to the node "parent", since the child node will be init as dict!
+        try:
+            for sec in sec_name_lst[:-1]:
+                idx_sec = idx_sec[sec]
+        except:
+            raise RuntimeError(f"The parent node of {sec} is not defined yet, it's invalid for directly made the child node")
+
+        return idx_sec, sec_name_lst[-1]
 
     def __get_declr_dict(self, cfg_str:str) -> dict : 
         if self.__split_chr not in cfg_str:
             raise RuntimeError(f"Configuration Error : Split character '{self.__split_chr}' not found in '{cfg_str}'")
         
         try:
             var_name, val_str = cfg_str.split(self.__split_chr)
@@ -141,38 +181,42 @@
         return { var_name : var_val }
 
     def __cfg_parser(self, raw_cfg_text:str):
         '''
             raw_cfg_text :
                 The string which declare the arguments with the same syntax used in config file.
         '''
-        cur_sec_key = ''
+        cur_sec_keys = ''
         for lin in raw_cfg_text.splitlines():
             # strip empty space and 'skip' empty line in cfgstr
             cfg_str = self.__preproc_cfgstr(lin)
             if not cfg_str:
                 continue
 
             # get the section key of config string (if there exists)
-            sec_key = self.__get_sec(cfg_str)
-            if sec_key:
-                self.__dict__[sec_key] = {}
-                cur_sec_key = sec_key
+            sec_keys_str = self.__get_sec(cfg_str)
+            if sec_keys_str:
+                idx_sec, idx_sec_key = self.__idx_sec_by_dot(sec_keys_str)
+                if idx_sec_key in idx_sec.keys():
+                    raise RuntimeError(f'Re-defined config, {sec_keys_str} section will be overrided!!')
+                idx_sec[idx_sec_key] = {}
+                cur_sec_keys = sec_keys_str
                 
             # parse variable assignment string
             else:
                 val_dict = self.__get_declr_dict(cfg_str)
-                if cur_sec_key != '':
-                    self.__dict__[cur_sec_key].update( val_dict )
+                if cur_sec_keys != '':
+                    idx_sec, idx_sec_key = self.__idx_sec_by_dot(cur_sec_keys)
+                    idx_sec[idx_sec_key].update( val_dict )
                 else:
                     self.__dict__.update( val_dict )
 
         # Update the namespace value via commend-line input 
         if self.__cmd_args:
-            Argparser.args_from_cmd(self.__dict__)
+            Argparser.args_from_cmd(self.__idx_sec_by_dot)
 
     # Display the namespace which record all of the declared arguments
     #   for the inner-node structure, iter-call __str__ wrapper !!
     def __str__(self):
         key_str = [ str(key) for key in self.__dict__.keys() if key[0] != '_' ] 
         return "Namespace : \n" + ", ".join(key_str)
```

### Comparing `easy_configer-1.3.4/easy_configer/IO_Converter.py` & `easy_configer-2.0.0/easy_configer/IO_Converter.py`

 * *Files identical despite different names*

### Comparing `easy_configer-1.3.4/easy_configer/utils/Flag.py` & `easy_configer-2.0.0/easy_configer/utils/Flag.py`

 * *Files identical despite different names*

### Comparing `easy_configer-1.3.4/easy_configer/utils/Type_Convertor.py` & `easy_configer-2.0.0/easy_configer/utils/Type_Convertor.py`

 * *Files identical despite different names*

### Comparing `easy_configer-1.3.4/setup.py` & `easy_configer-2.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # read the contents of your README file
 this_directory = abspath(dirname(__file__))
 with open(join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='easy_configer',
-    version='1.3.4',
-    description='An easy-way for configurating pyhon program by the given config file or config str',
+    version='2.0.0',
+    description='An easy way for configurating python program by the given config file or config str',
     author='JosefHuang',
     author_email='a3285556aa@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/HuangChiEn/easy_config',
     packages=['easy_configer', 'easy_configer/utils'],
```

### Comparing `easy_configer-1.3.4/test/test_Configer.py` & `easy_configer-2.0.0/test/test_Configer.py`

 * *Files identical despite different names*

### Comparing `easy_configer-1.3.4/test/test_IO_Converter.py` & `easy_configer-2.0.0/test/test_IO_Converter.py`

 * *Files identical despite different names*

