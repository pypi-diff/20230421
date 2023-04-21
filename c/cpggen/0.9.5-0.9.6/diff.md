# Comparing `tmp/cpggen-0.9.5.tar.gz` & `tmp/cpggen-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-0.9.5.tar", max compression
+gzip compressed data, was "cpggen-0.9.6.tar", max compression
```

## Comparing `cpggen-0.9.5.tar` & `cpggen-0.9.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-19 05:29:23.478079 cpggen-0.9.5/LICENSE
--rw-r--r--   0        0        0     7201 2023-04-19 05:29:23.478079 cpggen-0.9.5/README.md
--rw-r--r--   0        0        0        0 2023-04-19 05:29:23.478079 cpggen-0.9.5/cpggen/__init__.py
--rw-r--r--   0        0        0    13069 2023-04-19 05:29:23.478079 cpggen-0.9.5/cpggen/cli.py
--rw-r--r--   0        0        0    32803 2023-04-19 05:29:23.478079 cpggen-0.9.5/cpggen/executor.py
--rw-r--r--   0        0        0      746 2023-04-19 05:29:23.478079 cpggen-0.9.5/cpggen/logger.py
--rw-r--r--   0        0        0    11089 2023-04-19 05:29:23.478079 cpggen-0.9.5/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-19 05:29:23.482079 cpggen-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     8529 1970-01-01 00:00:00.000000 cpggen-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-21 12:22:08.046902 cpggen-0.9.6/LICENSE
+-rw-r--r--   0        0        0     7487 2023-04-21 12:22:08.046902 cpggen-0.9.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 12:22:08.046902 cpggen-0.9.6/cpggen/__init__.py
+-rw-r--r--   0        0        0    13069 2023-04-21 12:22:08.046902 cpggen-0.9.6/cpggen/cli.py
+-rw-r--r--   0        0        0    33093 2023-04-21 12:22:08.050902 cpggen-0.9.6/cpggen/executor.py
+-rw-r--r--   0        0        0      746 2023-04-21 12:22:08.050902 cpggen-0.9.6/cpggen/logger.py
+-rw-r--r--   0        0        0    11219 2023-04-21 12:22:08.050902 cpggen-0.9.6/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-21 12:22:08.050902 cpggen-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     8815 1970-01-01 00:00:00.000000 cpggen-0.9.6/PKG-INFO
```

### Comparing `cpggen-0.9.5/LICENSE` & `cpggen-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.5/README.md` & `cpggen-0.9.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,38 +52,46 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.4/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.6/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.4/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.6/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
-Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
+Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary.
 
 ```bash
 oras pull ghcr.io/appthreat/cpggen-bin:v1
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
+On Windows
+
+```powershell
+Invoke-WebRequest -Uri https://github.com/oras-project/oras/releases/download/v1.0.0/oras_1.0.0_windows_amd64.zip -UseBasicParsing -OutFile oras_1.0.0_windows_amd64.zip
+Expand-Archive -Path oras_1.0.0_windows_amd64.zip -DestinationPath .
+oras.exe pull ghcr.io/appthreat/cpggen-windows-bin:v1
+```
+
 ## Usage
 
 To auto detect the language from the current directory and generate CPG.
 
 ```
 cpggen
 ```
@@ -118,21 +126,21 @@
 ### Export graphs
 
 By passing `--export`, cpggen can export the various graphs to many formats using [joern-export](https://docs.joern.io/exporting/)
 
 Example to export `cpg14` graphs in `dot` format
 
 ```bash
-cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/export_out
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export
 ```
 
 To export `pdg` in `neo4jcsv` format
 
 ```bash
-cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/export_out --export-repr pdg --export-format neo4jcsv
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export --export-repr pdg --export-format neo4jcsv
 ```
 
 ### Artifacts produced
 
 Upon successful completion, cpggen would produce the following artifacts in the directory specified under `out_dir`
 
 - {name}-{lang}-cpg.bin.zip - Code Property Graph for the given language type
```

### Comparing `cpggen-0.9.5/cpggen/cli.py` & `cpggen-0.9.6/cpggen/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         src = str(PurePath(args.src))
         if not cpg_out_dir and src:
             if os.path.isfile(src):
                 cpg_out_dir = os.path.join(os.path.dirname(src), "cpg_out")
             else:
                 cpg_out_dir = os.path.join(src, "cpg_out")
         if not export_out_dir and src:
-            export_out_dir = os.path.join(src, "export_out")
+            export_out_dir = os.path.join(src, "cpg_export")
     if cpg_out_dir:
         cpg_out_dir = str(PurePath(cpg_out_dir))
     if export_out_dir:
         export_out_dir = str(PurePath(export_out_dir))
     languages = args.language
     joern_home = args.joern_home
     use_container = args.use_container
```

### Comparing `cpggen-0.9.5/cpggen/executor.py` & `cpggen-0.9.6/cpggen/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,18 @@
     joern_bundled = resource_path(os.path.join("local_bin", "joern-cli.zip"))
     if os.path.exists(csharp2cpg_bundled) and not os.path.exists(
         os.path.join(local_bin_dir, "bin", "csharp2cpg")
     ):
         try:
             with zipfile.ZipFile(csharp2cpg_bundled, "r") as zip_ref:
                 zip_ref.extractall(local_bin_dir)
-                if not os.path.exists(
+                # Create symlinks only when the binary exists
+                if os.path.exists(
+                    os.path.join(local_bin_dir, "bin", "csharp2cpg")
+                ) and not os.path.exists(
                     os.path.join(local_bin_dir, "joern-cli", "csharp2cpg")
                 ):
                     os.symlink(
                         os.path.join(local_bin_dir, "bin", "csharp2cpg"),
                         os.path.join(local_bin_dir, "joern-cli", "csharp2cpg"),
                     )
         except Exception as e:
@@ -145,22 +148,14 @@
     "export": "%(joern_home)sjoern-export --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
     "qwiet": "sl analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
     "dot2png": "dot -Tpng %(dot_file)s -o %(png_out)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
-    "java": {
-        "maven": [
-            get("MVN_CMD", "%(maven_cmd)s"),
-            "compile",
-        ],
-        "gradle": [get("GRADLE_CMD", "%(gradle_cmd)s"), "build"],
-        "sbt": ["sbt", "compile"],
-    },
     "jar": {
         "maven": [
             get("MVN_CMD", "%(maven_cmd)s"),
             "compile",
             "package",
             "-Dmaven.test.skip=true",
         ],
@@ -193,14 +188,29 @@
         "install": ["composer", "install", "-n", "--ignore-platform-reqs"],
         "update": ["composer", "update", "-n", "--ignore-platform-reqs"],
         "autoload": ["composer", "dump-autoload", "-o"],
     },
     "make": ["make"],
 }
 
+qwiet_lang_map = {
+    "jar": "java",
+    "jsp": "java",
+    "scala": "java",
+    "java": "javasrc",
+    "python": "pythonsrc",
+    "js": "javascriptsrc",
+    "ts": "javascriptsrc",
+    "javascript": "javascriptsrc",
+    "typescript": "javascriptsrc",
+    "go": "go",
+    "csharp": "csharp",
+    "dotnet": "csharp",
+}
+
 
 def qwiet_analysis(app_manifest, cwd, env):
     try:
         LOG.info(f"Submitting {app_manifest['app']} for Qwiet.AI analysis")
         build_args = cpg_tools_map["qwiet"]
         policy = ""
         vcs_correction = ""
@@ -682,16 +692,16 @@
                         # In case of github action, we need to convert this to relative path
                         if os.getenv("GITHUB_PATH"):
                             cpg_out = cpg_out.replace("/github/workspace/", "")
                             sbom_out = sbom_out.replace("/github/workspace/", "")
                             amodule = amodule.replace("/github/workspace/", "")
                         language = tool_lang.split("-")[0]
                         # Override the language for jvm
-                        if language in ("jar", "scala"):
-                            language = "java"
+                        if qwiet_lang_map.get(language):
+                            language = qwiet_lang_map.get(language)
                         app_base_name = os.path.basename(amodule)
                         # Let's improve the name for github action
                         if app_base_name == "workspace" and os.getenv(
                             "GITHUB_REPOSITORY"
                         ):
                             app_base_name = os.getenv("GITHUB_REPOSITORY").split("/")[
                                 -1
```

### Comparing `cpggen-0.9.5/cpggen/logger.py` & `cpggen-0.9.6/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.5/cpggen/utils.py` & `cpggen-0.9.6/cpggen/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 import re
 import shutil
 import tempfile
 import zipfile
 from pathlib import Path
 from sys import platform
 
-import git
+GIT_AVAILABLE = False
+try:
+    import git
+
+    GIT_AVAILABLE = True
+except Exception:
+    pass
 
 # Default ignore list
 ignore_directories = [
     ".git",
     ".svn",
     ".mvn",
     ".idea",
@@ -382,9 +388,11 @@
         project_types.append("llvm")
     if is_exe(src_dir):
         project_types.append("binary")
     return project_types
 
 
 def clone_repo(repo_url, clone_dir, depth=1):
+    if not GIT_AVAILABLE:
+        return None
     git.Repo.clone_from(repo_url, clone_dir, depth=depth)
     return clone_dir
```

### Comparing `cpggen-0.9.5/pyproject.toml` & `cpggen-0.9.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "0.9.5"
+version = "0.9.6"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-0.9.5/PKG-INFO` & `cpggen-0.9.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 0.9.5
+Version: 0.9.6
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -84,38 +84,46 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.4/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.6/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.4/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.6/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
-Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
+Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary.
 
 ```bash
 oras pull ghcr.io/appthreat/cpggen-bin:v1
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
+On Windows
+
+```powershell
+Invoke-WebRequest -Uri https://github.com/oras-project/oras/releases/download/v1.0.0/oras_1.0.0_windows_amd64.zip -UseBasicParsing -OutFile oras_1.0.0_windows_amd64.zip
+Expand-Archive -Path oras_1.0.0_windows_amd64.zip -DestinationPath .
+oras.exe pull ghcr.io/appthreat/cpggen-windows-bin:v1
+```
+
 ## Usage
 
 To auto detect the language from the current directory and generate CPG.
 
 ```
 cpggen
 ```
@@ -150,21 +158,21 @@
 ### Export graphs
 
 By passing `--export`, cpggen can export the various graphs to many formats using [joern-export](https://docs.joern.io/exporting/)
 
 Example to export `cpg14` graphs in `dot` format
 
 ```bash
-cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/export_out
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export
 ```
 
 To export `pdg` in `neo4jcsv` format
 
 ```bash
-cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/export_out --export-repr pdg --export-format neo4jcsv
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export --export-repr pdg --export-format neo4jcsv
 ```
 
 ### Artifacts produced
 
 Upon successful completion, cpggen would produce the following artifacts in the directory specified under `out_dir`
 
 - {name}-{lang}-cpg.bin.zip - Code Property Graph for the given language type
```

