# Comparing `tmp/py_yprinciple_gen-0.2.7.tar.gz` & `tmp/py_yprinciple_gen-0.2.8.tar.gz`

## Comparing `py_yprinciple_gen-0.2.7.tar` & `py_yprinciple_gen-0.2.8.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/.pydevproject
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/.github/workflows/upload-to-pypi.yml
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/scripts/install
--rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/basemwtest.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/basesmwtest.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/basetest.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/test_editor.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/test_python.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/test_smw.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/test_smw_generate.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/__init__.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/editor.py
--rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/genapi.py
--rw-r--r--   0        0        0    13170 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/gengrid.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/profiler.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/push.py
--rw-r--r--   0        0        0    22523 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/smw_targets.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/target.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/version.py
--rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/ypcell.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/ypgen.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/ypgenapp.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/resources/static/css/md_style_indigo.css
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/LICENSE
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/README.md
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/.pydevproject
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/.github/workflows/upload-to-pypi.yml
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/scripts/install
+-rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/__init__.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/basemwtest.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/basesmwtest.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/basetest.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/test_editor.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/test_python.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/test_smw.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/test_smw_generate.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/__init__.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/editor.py
+-rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/genapi.py
+-rw-r--r--   0        0        0    13170 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/gengrid.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/profiler.py
+-rw-r--r--   0        0        0    22523 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/smw_targets.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/target.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/version.py
+-rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/ypcell.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/ypgen.py
+-rw-r--r--   0        0        0    11743 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/ypgenapp.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/resources/static/css/md_style_indigo.css
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/README.md
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/PKG-INFO
```

### Comparing `py_yprinciple_gen-0.2.7/.github/workflows/build.yml` & `py_yprinciple_gen-0.2.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/.github/workflows/upload-to-pypi.yml` & `py_yprinciple_gen-0.2.8/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/scripts/test` & `py_yprinciple_gen-0.2.8/scripts/test`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/tests/basemwtest.py` & `py_yprinciple_gen-0.2.8/tests/basemwtest.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/tests/basesmwtest.py` & `py_yprinciple_gen-0.2.8/tests/basesmwtest.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/tests/basetest.py` & `py_yprinciple_gen-0.2.8/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/tests/test_editor.py` & `py_yprinciple_gen-0.2.8/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/tests/test_smw.py` & `py_yprinciple_gen-0.2.8/tests/test_smw.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/tests/test_smw_generate.py` & `py_yprinciple_gen-0.2.8/tests/test_smw_generate.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/editor.py` & `py_yprinciple_gen-0.2.8/yprinciple/editor.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/genapi.py` & `py_yprinciple_gen-0.2.8/yprinciple/genapi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 '''
 Created on 2023-01-30
 
 @author: wf
 '''
+import traceback
+import sys
 from pathlib import Path
 from meta.mw import SMWAccess
 from meta.metamodel import Context
 from yprinciple.smw_targets import SMWTarget
 from yprinciple.ypcell import YpCell
+from wikibot3rd.wikipush import WikiPush
 
 class GeneratorAPI:
     """
     
     generator API e.g. to be used as a
     
     command line generator 
@@ -23,41 +26,50 @@
         
         Args:
             verbose(bool): if True show verbose messages
             debug(bool): if True switch debugging on
         """
         self.verbose=verbose
         self.debug=debug
+        self.args=None
         
     @classmethod
     def fromArgs(cls,args)->"GeneratorAPI":
         """
         create a GeneratorAPI for the given command line arguments
         
         Args:
             args: command line arguments
             
         Returns:
             GeneratorAPI:
         """
         gen=GeneratorAPI(verbose=not args.quiet,debug=args.debug)
-        gen.setWikiAndGetContexts(args.wikiId)
+        gen.setWikiAndGetContexts(args)
         if args.sidif:
             gen.context,gen.error,gen.errMsg=Context.fromSiDIF_input(args.sidif, debug=args.debug)
         else:
-            gen.readContext(args.wikiId,args.context)
+            wikiId=args.source if args.push else args.wikiId
+            gen.readContext(wikiId,args.context)
+        # remember complete arguments (e.g. for push)
+        gen.args=args
         return gen
     
-    def setWikiAndGetContexts(self,wikiId):
+    def setWikiAndGetContexts(self,args):
         """
-        set my wiki and get Contexts
+        set my wiki and get Contexts for the given args
+        
+        Args:
+            args: command line arguments
         """
-        self.wikiId=wikiId
-        self.smwAccess=SMWAccess(wikiId)
-        self.mw_contexts=self.smwAccess.getMwContexts()
+        self.wikiId=args.wikiId
+        self.smwAccess=SMWAccess(args.wikiId)
+        self.smwSourceAccess=SMWAccess(args.source) if args.push else None
+        self.smwContextAccess=self.smwSourceAccess if args.push else self.smwAccess
+        self.mw_contexts=self.smwContextAccess.getMwContexts()
        
     def readContext(self,wikiId:str,context_name:str):
         """
         Args:
             wikiId(str): the wikiId of the wiki to read the context from
             context_name: the name of the context to read
         """
@@ -126,14 +138,21 @@
                             for subCell in ypCell.subCells.values():
                                 showMsg(topic_name,subCell)
                                 yield subCell
                     else:
                         showMsg(topic_name,ypCell)
                         yield ypCell
                         
+    def handleFailure(self,ypCell,ex):
+        """
+        handle the given failure
+        """
+        print(f"Warning ⚠️: generating {ypCell.target} for {ypCell.modelElement} failed with {str(ex)}",file=sys.stderr,flush=True)
+        if self.debug:
+            print(traceback.format_exc())
           
     def generateViaMwApi(self,target_names:list=None,topic_names:list=None,dryRun:bool=True,withEditor:bool=False):
         """
         start the generation via MediaWiki API
         
         Args:
             target_names(list): an optional list of target names
@@ -143,21 +162,24 @@
             
         Return:
             list(MwGenResult): a list of Mediawiki Generator Results
         """
         self.smwAccess.wikiClient.login()
         genResults=[]
         for ypCell in self.yieldYpCells("via Mediawiki Api", target_names, topic_names):
-            genResult=ypCell.generateViaMwApi(smwAccess=self.smwAccess,dryRun=dryRun,withEditor=withEditor)
-            if self.debug or self.verbose:
-                diff_url=genResult.getDiffUrl()
-                diff_info="" if diff_url is None else diff_url
-                diff_info+=f"({len(genResult.markup_diff)})"
-                print(f"diff: {diff_info}")
-            genResults.append(genResult)
+            try:
+                genResult=ypCell.generateViaMwApi(smwAccess=self.smwAccess,dryRun=dryRun,withEditor=withEditor)
+                if self.debug or self.verbose:
+                    diff_url=genResult.getDiffUrl()
+                    diff_info="" if diff_url is None else diff_url
+                    diff_info+=f"({len(genResult.markup_diff)})"
+                    print(f"diff: {diff_info}")
+                genResults.append(genResult)
+            except Exception as ex:
+                self.handleFailure(ypCell, ex)
         return genResults
  
     def generateToFile(self,target_dir=None,target_names:list=None,topic_names:list=None,dryRun:bool=True,withEditor:bool=False):
         """
         start the generation via MediaWiki Backup Directory
         
         Args:
@@ -172,11 +194,50 @@
             list(FileGenResult): a list of File Generator Results
         """
         genResults=[]
         if target_dir is None:
             home = Path.home()
             target_dir=f"{home}/wikibackup/{self.wikiId}"
         for ypCell in self.yieldYpCells(f" to file in {target_dir}", target_names, topic_names):
-            genResult=ypCell.generateToFile(target_dir=target_dir,dryRun=dryRun,withEditor=withEditor)
-            genResults.append(genResult)
+            try:
+                genResult=ypCell.generateToFile(target_dir=target_dir,dryRun=dryRun,withEditor=withEditor)
+                genResults.append(genResult)
+            except Exception as ex:
+                self.handleFailure(ypCell,ex)
         return genResults
- 
+    
+    def push(self):
+        """
+        push according to my command line args
+        """
+        if not self.args.source:
+            raise "missing source wiki"
+        if self.args.topics:
+            topic_names=self.args.topics
+        else:
+            topic_names=self.context.topics.keys()
+        login=self.args.login
+        force=self.args.force
+        ignore=True
+        fromWikiId=self.args.source
+        wikiPush=WikiPush(fromWikiId=fromWikiId,toWikiId=self.smwAccess.wikiId,login=login,verbose=not self.args.quiet,debug=self.args.debug)
+        if not self.args.quiet:
+            print(f"pushing concept {self.args.context} from {self.args.source} to {self.wikiId} ...")
+        all_page_titles=[]
+        for topic_name in topic_names:
+            topic=self.context.topics[topic_name]
+            for page_titles,page_query,query_field in [
+                    ([f"Concept:{topic_name}"],None,None),
+                    ([f"Category:{topic_name}"],None,None),
+                    ([f"Template:{topic_name}"],None,None),
+                    ([f"Form:{topic_name}"],None,None),
+                    ([f"Help:{topic_name}"],None,None),
+                    ([f"List of {topic.pluralName}"],None,None),
+                    (None,f"{{{{#ask: [[Property topic::Concept:{topic_name}]]|?#=page}}}}","page"),
+                    (None,f"{{{{#ask: [[Topic name::{topic_name}]]|?Topic context=context}}}}","context")     
+                ]:   
+                if not page_titles:
+                    page_titles=wikiPush.query(page_query, wiki=self.smwSourceAccess.wikiClient, queryField=query_field)
+                all_page_titles.extend(page_title for page_title in page_titles if page_title not in all_page_titles)    
+        failed=wikiPush.push(pageTitles=all_page_titles,force=force,ignore=ignore,withImages=True)
+        if len(failed)>0:
+            print(f"Warning {len(failed)} push attempts failed")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/gengrid.py` & `py_yprinciple_gen-0.2.8/yprinciple/gengrid.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/profiler.py` & `py_yprinciple_gen-0.2.8/yprinciple/profiler.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/smw_targets.py` & `py_yprinciple_gen-0.2.8/yprinciple/smw_targets.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/target.py` & `py_yprinciple_gen-0.2.8/yprinciple/target.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/version.py` & `py_yprinciple_gen-0.2.8/yprinciple/version.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/ypcell.py` & `py_yprinciple_gen-0.2.8/yprinciple/ypcell.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/ypgen.py` & `py_yprinciple_gen-0.2.8/yprinciple/ypgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 '''
 
 from argparse import ArgumentParser
 from argparse import RawDescriptionHelpFormatter
 from yprinciple.version import Version
 from yprinciple.ypgenapp import YPGenApp
 from yprinciple.genapi import GeneratorAPI
-from yprinciple.push import Push
 import os
 import sys
 import traceback
 import webbrowser
 # import after app!
 from jpcore.justpy_app import JustpyServer
 
@@ -48,14 +47,16 @@
         parser.add_argument("--editor", action="store_true", help="open editor for results [default: %(default)s]")       
         parser.add_argument('--host',default=JustpyServer.getDefaultHost(),help="the host to serve / listen from [default: %(default)s]")
         parser.add_argument('--port',type=int,default=8778,help="the port to serve from [default: %(default)s]")
         parser.add_argument("--push", action="store_true", help="push from source to target [default: %(default)s]")       
         parser.add_argument("--serve",help="start webserver",action="store_true")
         parser.add_argument('--wikiId',"-t","--target", default="wiki",help='id of the wiki to generate for [default: %(default)s]')
         parser.add_argument('--source',"-s", default="profiwiki",help='id of the wiki to get concept and contexts (schemas) from [default: %(default)s]')
+        parser.add_argument("-l", "--login", dest="login", action='store_true', help="login to source wiki for access permission")
+        parser.add_argument("-f", "--force", dest="force", action='store_true', help="force to overwrite existing pages")
         parser.add_argument('-q', '--quiet', help="not verbose [default: %(default)s]" )
         parser.add_argument('-V', '--version', action='version', version=version_msg)
         return parser
     
 __version__ = Version.version
 __date__ = Version.date
 __updated__ = Version.updated
@@ -100,27 +101,26 @@
             webbrowser.open(Version.doc_url)
         elif args.serve:
             ypGenApp=YPGenApp(version=Version, title="Y-Principle generator",args=args)
             url=f"http://{args.host}:{args.port}"
             webbrowser.open(url)
             ypGenApp.start(host=args.host, port=args.port,debug=args.debug)
             pass
-        elif args.genToFile or args.genViaMwApi:
+        elif args.genToFile or args.genViaMwApi or args.push:
             gen=GeneratorAPI.fromArgs(args)
             if gen.error:
                 print(f"{gen.errmsg}", file=sys.stderr)
                 return 3
             dryRun=not args.noDry
             if args.genViaMwApi:
                 gen.generateViaMwApi(target_names=args.targets,topic_names=args.topics, dryRun=dryRun, withEditor=args.editor)
             if args.genToFile:
                 gen.generateToFile(target_dir=args.targetPath,target_names=args.targets,topic_names=args.topics, dryRun=dryRun, withEditor=args.editor) 
-        elif args.push:
-            push=Push(args)
-            push.push()       
+            if args.push:
+                gen.push()       
         pass
     except KeyboardInterrupt:
         ### handle keyboard interrupt ###
         return 1
     except Exception as e:
         if DEBUG:
             raise(e)
```

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/ypgenapp.py` & `py_yprinciple_gen-0.2.8/yprinciple/ypgenapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self.explainDepth=0
         
     def setGenApiFromArgs(self,args):
         """
         set the semantic MediaWiki
         """
         self.genapi=GeneratorAPI.fromArgs(args)
-        self.genapi.setWikiAndGetContexts(args.wikiId)
+        self.genapi.setWikiAndGetContexts(args)
         self.smwAccess=self.genapi.smwAccess
         if self.wikiLink is not None:
             self.wikiLink.text=args.wikiId
             self.wikiLink.title=args.wikiId
             wikiUser=self.smwAccess.wikiClient.wikiUser
             if wikiUser:
                 self.wikiLink.href=wikiUser.getWikiUrl()
```

### Comparing `py_yprinciple_gen-0.2.7/yprinciple/resources/static/css/md_style_indigo.css` & `py_yprinciple_gen-0.2.8/yprinciple/resources/static/css/md_style_indigo.css`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/.gitignore` & `py_yprinciple_gen-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/LICENSE` & `py_yprinciple_gen-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/README.md` & `py_yprinciple_gen-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.7/pyproject.toml` & `py_yprinciple_gen-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 		# https://github.com/justpy-org/justpy
         'justpy>=0.12.1',
         # https://pypi.org/project/pyJustpyWidgets/
         'pyJustpyWidgets>=0.1.13',
         # https://pypi.org/project/search-engine-parser/
         'search-engine-parser>=0.6.8',
         # https://pypi.org/project/py-3rdparty-mediawiki/
-        'py-3rdparty-mediawiki>=0.8.0',
+        'py-3rdparty-mediawiki>=0.9.5',
         # https://pypi.org/project/pyMetaModel/
-        'pyMetaModel>=0.3.0',
+        'pyMetaModel>=0.3.1',
         # https://pypi.org/project/beautifulsoup4/
         'beautifulsoup4',
         # https://github.com/borisbabic/browser_cookie3
         # 'browser_cookie>=0.16.2'
      ]
 
 requires-python = ">=3.8"
```

### Comparing `py_yprinciple_gen-0.2.7/PKG-INFO` & `py_yprinciple_gen-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-yprinciple-gen
-Version: 0.2.7
+Version: 0.2.8
 Project-URL: Home, https://github.com/WolfgangFahl/py-yprinciple-gen
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/Py-yprinciple-gen
 Project-URL: Source, https://github.com/WolfgangFahl/py-yprinciple-gen
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -20,17 +20,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Requires-Dist: beautifulsoup4
 Requires-Dist: justpy>=0.12.1
-Requires-Dist: py-3rdparty-mediawiki>=0.8.0
+Requires-Dist: py-3rdparty-mediawiki>=0.9.5
 Requires-Dist: pyjustpywidgets>=0.1.13
-Requires-Dist: pymetamodel>=0.3.0
+Requires-Dist: pymetamodel>=0.3.1
 Requires-Dist: search-engine-parser>=0.6.8
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
 
 # py-yprinciple-gen
 python Library for code generation according to the Y-Principle
```

