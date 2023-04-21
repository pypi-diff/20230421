# Comparing `tmp/xklb-1.24.9.tar.gz` & `tmp/xklb-1.25.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xklb-1.24.9.tar", max compression
+gzip compressed data, was "xklb-1.25.1.tar", max compression
```

## Comparing `xklb-1.24.9.tar` & `xklb-1.25.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0     1676 2023-04-02 15:38:48.248247 xklb-1.24.9/LICENSE
--rw-r--r--   0        0        0    39259 2023-04-02 15:38:48.248247 xklb-1.24.9/README.md
--rw-r--r--   0        0        0     8385 2023-04-02 15:38:48.248247 xklb-1.24.9/assets/kotobago.png
--rw-r--r--   0        0        0    13982 2023-04-02 15:38:49.388317 xklb-1.24.9/pyproject.toml
--rw-r--r--   0        0        0      686 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/__init__.py
--rw-r--r--   0        0        0     4199 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/bigdirs.py
--rw-r--r--   0        0        0     7880 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/invalid_paths.py
--rw-r--r--   0        0        0     1370 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4020 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/merge_online_local.py
--rw-r--r--   0        0        0     1009 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1569 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2741 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2085 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/mining/reddit_self.py
--rw-r--r--   0        0        0    17101 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/mining/words.py
--rw-r--r--   0        0        0     6864 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/move_list.py
--rw-r--r--   0        0        0      547 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/optimize_db.py
--rw-r--r--   0        0        0     9412 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/redownload.py
--rw-r--r--   0        0        0      483 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/restore_listen_count.sql
--rw-r--r--   0        0        0    17018 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/scatter.py
--rw-r--r--   0        0        0     2610 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0       25 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/__init__.py
--rw-r--r--   0        0        0     6846 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/av.py
--rw-r--r--   0        0        0     6870 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/books.py
--rw-r--r--   0        0        0     7676 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/consts.py
--rw-r--r--   0        0        0     7602 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/db.py
--rw-r--r--   0        0        0     7051 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/dl_config.py
--rw-r--r--   0        0        0    14665 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/dl_extract.py
--rw-r--r--   0        0        0    13251 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/fs_extract.py
--rw-r--r--   0        0        0     5444 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/gui.py
--rw-r--r--   0        0        0     5904 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/hn_extract.py
--rw-r--r--   0        0        0     8992 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/lb.py
--rw-r--r--   0        0        0    32433 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/play_actions.py
--rw-r--r--   0        0        0     4677 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/playback.py
--rw-r--r--   0        0        0    25518 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/player.py
--rw-r--r--   0        0        0    14553 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/praw_extract.py
--rw-r--r--   0        0        0    16062 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/stats.py
--rw-r--r--   0        0        0     3824 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/subtitle.py
--rw-r--r--   0        0        0    11986 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3607 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21477 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/tube_backend.py
--rw-r--r--   0        0        0     6258 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/tube_extract.py
--rw-r--r--   0        0        0    26282 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/utils.py
--rw-r--r--   0        0        0    40447 1970-01-01 00:00:00.000000 xklb-1.24.9/PKG-INFO
+-rw-r--r--   0        0        0     1676 2023-04-20 10:48:25.650642 xklb-1.25.1/LICENSE
+-rw-r--r--   0        0        0    40027 2023-04-20 10:48:25.650642 xklb-1.25.1/README.md
+-rw-r--r--   0        0        0     8385 2023-04-20 10:48:25.650642 xklb-1.25.1/assets/kotobago.png
+-rw-r--r--   0        0        0    13982 2023-04-20 10:48:26.670645 xklb-1.25.1/pyproject.toml
+-rw-r--r--   0        0        0      693 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/__init__.py
+-rw-r--r--   0        0        0     4199 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2376 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/christen.py
+-rw-r--r--   0        0        0     7864 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/dedupe.py
+-rw-r--r--   0        0        0     1370 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4020 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     1009 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/mining/nfb_ca.py
+-rw-r--r--   0        0        0     1569 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2741 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2085 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/mining/reddit_self.py
+-rw-r--r--   0        0        0    17101 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/mining/words.py
+-rw-r--r--   0        0        0     6864 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/move_list.py
+-rw-r--r--   0        0        0      547 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9412 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/redownload.py
+-rw-r--r--   0        0        0     2294 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/relmv.py
+-rw-r--r--   0        0        0      483 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/restore_listen_count.sql
+-rw-r--r--   0        0        0    17018 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/scatter.py
+-rw-r--r--   0        0        0     2610 2023-04-20 10:48:26.670645 xklb-1.25.1/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0       25 2023-04-20 10:48:26.670645 xklb-1.25.1/xklb/__init__.py
+-rw-r--r--   0        0        0     6846 2023-04-20 10:48:26.670645 xklb-1.25.1/xklb/av.py
+-rw-r--r--   0        0        0     6870 2023-04-20 10:48:26.670645 xklb-1.25.1/xklb/books.py
+-rw-r--r--   0        0        0     7676 2023-04-20 10:48:26.670645 xklb-1.25.1/xklb/consts.py
+-rw-r--r--   0        0        0     7673 2023-04-20 10:48:26.670645 xklb-1.25.1/xklb/db.py
+-rw-r--r--   0        0        0     7051 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/dl_config.py
+-rw-r--r--   0        0        0    14677 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13251 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/fs_extract.py
+-rw-r--r--   0        0        0     5444 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/gui.py
+-rw-r--r--   0        0        0     5904 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9274 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/lb.py
+-rw-r--r--   0        0        0    33562 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/play_actions.py
+-rw-r--r--   0        0        0     4677 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/playback.py
+-rw-r--r--   0        0        0    25588 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/player.py
+-rw-r--r--   0        0        0    14553 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16048 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/stats.py
+-rw-r--r--   0        0        0     3824 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/subtitle.py
+-rw-r--r--   0        0        0    12060 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3607 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21477 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6258 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/tube_extract.py
+-rw-r--r--   0        0        0    26248 2023-04-20 10:48:26.674645 xklb-1.25.1/xklb/utils.py
+-rw-r--r--   0        0        0    41215 1970-01-01 00:00:00.000000 xklb-1.25.1/PKG-INFO
```

### Comparing `xklb-1.24.9/LICENSE` & `xklb-1.25.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/README.md` & `xklb-1.25.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # xk media library
 
 A wise philosopher once told me: "[the future is autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
 Manage large media libraries. An index for your archive.
 Primary usage is local filesystem but also supports some virtual constructs like
-tracking online video playlists (eg. YouTube subscriptions) or daily browser tabs.
+tracking online video playlists (eg. YouTube subscriptions) and scheduling browser tabs.
 
 Required: `ffmpeg`
 
 Recommended: `mpv`, `fish`, `firefox`
 
 ## Install
 
@@ -17,28 +17,30 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.24.009)
+    xk media library subcommands (v1.25.001)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
       lb read                  Read books
       lb view                  View images
 
       lb bigdirs               Discover folders which take much room
-      lb mv-list               Reach a target free space by moving data across mount points
       lb dedupe                Deduplicate local db files
+      lb relmv                 Move files/folders while preserving relative paths
+      lb mv-list               Reach a target free space by moving data across mount points
+      lb scatter               Scatter files across multiple mountpoints (mergerfs balance)
 
       lb christen              Cleanse files by giving them a new name
 
     online media:
       lb tubeadd               Create a tube database; Add playlists
       lb tubeupdate            Fetch new videos from saved playlists
 
@@ -261,19 +263,26 @@
 
     Print instead of play:
         library watch --print --limit 10  # print the next 10 files
         library watch -p -L 10  # print the next 10 files
         library watch -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
 
         Printing modes
-        library watch -p    # print in a table
-        library watch -p p  # equivalent
+        library watch -p    # print as a table
         library watch -p a  # print an aggregate report
         library watch -p b  # print a bigdirs report (see lb bigdirs -h for more info)
-        library watch -p f  # print fields -- useful for piping paths to utilities like xargs or GNU Parallel
+        library watch -p f  # print fields (defaults to path; use --cols to change)
+                               # -- useful for piping paths to utilities like xargs or GNU Parallel
+
+        library watch -p d  # mark deleted
+        library watch -p w  # mark watched
+
+        Some printing modes can be combined
+        library watch -p df  # print files for piping into another program and mark them as deleted within the db
+        library watch -p bf  # print fields from bigdirs report
 
         Check if you have downloaded something before
         library watch -u duration -p -s 'title'
 
         Print an aggregate report of deleted media
         library watch -w time_deleted!=0 -p=a
         ╒═══════════╤══════════════╤═════════╤═════════╕
@@ -281,22 +290,25 @@
         ╞═══════════╪══════════════╪═════════╪═════════╡
         │ Aggregate │ 14 days, 23  │ 50.6 GB │   29058 │
         │           │ hours and 42 │         │         │
         │           │ minutes      │         │         │
         ╘═══════════╧══════════════╧═════════╧═════════╛
         Total duration: 14 days, 23 hours and 42 minutes
 
-        Print an aggregate report of media that has no duration information (likely corrupt or online media)
+        Print an aggregate report of media that has no duration information (ie. online or corrupt local media)
         library watch -w 'duration is null' -p=a
 
         Print a list of filenames which have below 1280px resolution
         library watch -w 'width<1280' -p=f
 
         Print media you have partially viewed with mpv
-        library watch -p=v
+        library watch --partial -p
+        library watch -P -p  # equivalent
+        library watch -P -p f --cols path,progress,duration  # print CSV of partially watched files
+        library watch --partial -pa  # print an aggregate report of partially watched files
 
         View how much time you have watched
         library watch -w play_count'>'0 -p=a
 
         See how much video you have
         library watch video.db -p=a
         ╒═══════════╤═════════╤═════════╤═════════╕
```

### Comparing `xklb-1.24.9/assets/kotobago.png` & `xklb-1.25.1/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/pyproject.toml` & `xklb-1.25.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xklb"
-version = "1.24.009"
+version = "1.25.001"
 description = "xk library"
 authors = ["Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>"]
 readme = "README.md"
 documentation = "https://github.com/chapmanjacobd/library/wiki/Usage"
 homepage = "https://github.com/chapmanjacobd/library/"
 license = "BSD-3-Clause"
 packages = [
```

### Comparing `xklb-1.24.9/scripts/__init__.py` & `xklb-1.25.1/scripts/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from scripts.bigdirs import bigdirs, process_bigdirs
-from scripts.dedupe import deduplicate_db
-from scripts.invalid_paths import rename_invalid_paths
+from scripts.christen import christen
+from scripts.dedupe import dedupe
 from scripts.merge_dbs import merge_dbs
 from scripts.merge_online_local import merge_online_local
 from scripts.mining.nfb_ca import nfb_films
 from scripts.mining.nouns import nouns
 from scripts.mining.pushshift import pushshift_extract
 from scripts.mining.reddit_self import parse_reddit_selftext
 from scripts.move_list import move_list
 from scripts.optimize_db import optimize_db
 from scripts.redownload import redownload
+from scripts.relmv import relmv
 from scripts.scatter import scatter, scatter_usage
 from scripts.streaming_tab_loader import streaming_tab_loader
```

### Comparing `xklb-1.24.9/scripts/bigdirs.py` & `xklb-1.25.1/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/dedupe.py` & `xklb-1.25.1/scripts/dedupe.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     """
 
     media = list(args.db.query(query))
 
     return media
 
 
-def deduplicate_db() -> None:
+def dedupe() -> None:
     args = parse_args()
 
     if args.profile == DBType.audio:
         duplicates = get_music_duplicates(args)
     elif args.profile == "id":
         duplicates = get_id_duplicates(args)
     elif args.profile == "title":
@@ -243,8 +243,8 @@
             path = d["duplicate_path"]
             if not path.startswith("http") and not args.only_soft_delete:
                 utils.trash(path, detach=False)
             player.mark_media_deleted(args, path)
 
 
 if __name__ == "__main__":
-    deduplicate_db()
+    dedupe()
```

### Comparing `xklb-1.24.9/scripts/invalid_paths.py` & `xklb-1.25.1/scripts/christen.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 log.info(fixed)
         else:
             log.warning(printable_p)
             log.warning(fixed)
             print("")
 
 
-def rename_invalid_paths() -> None:
+def christen() -> None:
     args = parse_args()
 
     for path in args.paths:
         log.info("[%s]: Processing subfolders...", path)
         subpaths = sorted((bytes(p) for p in Path(path).rglob("*")), key=len, reverse=True)
         for p in subpaths:
             rename_path(args, p)
@@ -69,8 +69,8 @@
 
         yes | bfs -nohidden -type d -exec bfs -f {} -not -type d -exit 1 \; -prune -ok bfs -f {} -type d -delete \;
         """
     )
 
 
 if __name__ == "__main__":
-    rename_invalid_paths()
+    christen()
```

### Comparing `xklb-1.24.9/scripts/merge_dbs.py` & `xklb-1.25.1/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/merge_online_local.py` & `xklb-1.25.1/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/mining/nfb_ca.py` & `xklb-1.25.1/scripts/mining/nfb_ca.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/mining/nouns.py` & `xklb-1.25.1/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/mining/pushshift.py` & `xklb-1.25.1/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/mining/reddit_self.py` & `xklb-1.25.1/scripts/mining/reddit_self.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/mining/words.py` & `xklb-1.25.1/scripts/mining/words.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/move_list.py` & `xklb-1.25.1/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/optimize_db.py` & `xklb-1.25.1/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/redownload.py` & `xklb-1.25.1/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/scatter.py` & `xklb-1.25.1/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/scripts/streaming_tab_loader.py` & `xklb-1.25.1/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/av.py` & `xklb-1.25.1/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/books.py` & `xklb-1.25.1/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/consts.py` & `xklb-1.25.1/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/db.py` & `xklb-1.25.1/xklb/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,18 +161,18 @@
 
 
 def fts_quote(query: List[str]) -> List[str]:
     fts_words = [" NOT ", " AND ", " OR ", "*", ":", "NEAR("]
     return [s if any([r in s for r in fts_words]) else '"' + s + '"' for s in query]
 
 
-def fts_search(args, bindings) -> str:
-    bindings["query"] = " AND ".join(fts_quote(args.include))
+def fts_search(args) -> str:
+    args.filter_bindings["query"] = " AND ".join(fts_quote(args.include))
     if args.exclude:
-        bindings["query"] += " NOT " + " NOT ".join(fts_quote(args.exclude))
+        args.filter_bindings["query"] += " NOT " + " NOT ".join(fts_quote(args.exclude))
     table = "(" + args.db["media"].search_sql(include_rank=True) + ")"
     return table
 
 
 def gen_include_excludes(cols_available):
     searchable_columns = [
         "path",
@@ -192,16 +192,18 @@
         "artist",
         "tags",
         "playlist_path",
     ]
 
     valid_cols = [f"m.{c}" for c in searchable_columns if c in cols_available]
 
-    include_string = "and (" + " like :include{0} OR ".join(valid_cols) + " like :include{0} )"
-    exclude_string = "and (" + " not like :exclude{0} AND ".join(valid_cols) + " not like :exclude{0} )"
+    incl = ":include{0}"
+    excl = ":exclude{0}"
+    include_string = "AND (" + " OR ".join([f"{col} LIKE {incl}" for col in valid_cols]) + ")"
+    exclude_string = "AND (" + " AND ".join([f"COALESCE({col},'') NOT LIKE {excl}" for col in valid_cols]) + ")"
 
     return include_string, exclude_string
 
 
 def get_playlists(args, cols="path, dl_config", constrain=False, sql_filters=None) -> List[dict]:
     columns = args.db["playlists"].columns_dict
     if sql_filters is None:
```

### Comparing `xklb-1.24.9/xklb/dl_config.py` & `xklb-1.25.1/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/dl_extract.py` & `xklb-1.25.1/xklb/dl_extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,38 +89,35 @@
 
 def construct_query(args) -> Tuple[str, dict]:
     utils.ensure_playlists_exists(args)
 
     m_columns = args.db["media"].columns_dict
     pl_columns = args.db["playlists"].columns_dict
 
-    cf = []
-    bindings = {}
+    args.filter_sql = []
+    args.filter_bindings = {}
 
     if args.duration:
-        cf.append(" and duration IS NOT NULL " + args.duration)
+        args.filter_sql.append(" and duration IS NOT NULL " + args.duration)
 
-    cf.extend([" and " + w for w in args.where])
+    args.filter_sql.extend([" and " + w for w in args.where])
 
-    play_actions.construct_search_bindings(args, cf, bindings, m_columns)
+    play_actions.construct_search_bindings(args, m_columns)
 
-    cf.append(
+    args.filter_sql.append(
         f"""and cast(STRFTIME('%s',
           datetime( COALESCE(time_modified,0), 'unixepoch', '+{args.retry_delay}')
         ) as int) < STRFTIME('%s', datetime()) """
     )
 
     if "uploader" in m_columns:
-        cf.append(
+        args.filter_sql.append(
             f"and (m.uploader is NULL or m.uploader not in (select uploader from playlists where category='{consts.BLOCK_THE_CHANNEL}'))"
         )
 
-    args.sql_filter = " ".join(cf)
-    args.sql_filter_bindings = bindings
-
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     if "playlist_path" in m_columns:
         query = f"""select
                 m.path
                 , playlist_path
                 , m.title
                 {', m.duration' if 'duration' in m_columns else ''}
@@ -139,15 +136,15 @@
             WHERE 1=1
                 and COALESCE(m.time_downloaded,0) = 0
                 and COALESCE(m.time_deleted,0) = 0
                 and COALESCE(p.time_deleted,0) = 0
                 and m.path like "http%"
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
-                {args.sql_filter}
+                {" ".join(args.filter_sql)}
             ORDER BY 1=1
                 , play_count
                 {', ' + args.sort if args.sort else ''}
                 , random()
         {LIMIT}
         """
     else:
@@ -166,33 +163,33 @@
             FROM media m
             WHERE 1=1
                 and COALESCE(m.time_downloaded,0) = 0
                 and COALESCE(m.time_deleted,0) = 0
                 and m.path like "http%"
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
-                {args.sql_filter}
+                {" ".join(args.filter_sql)}
             ORDER BY 1=1
                 , play_count
                 {', ' + args.sort if args.sort else ''}
                 , random()
         {LIMIT}
         """
 
-    return query, bindings
+    return query, args.filter_bindings
 
 
 def process_downloadqueue(args) -> List[dict]:
     query, bindings = construct_query(args)
 
     if args.print:
         player.printer(args, query, bindings)
         return []
 
-    media = list(args.db.query(*construct_query(args)))
+    media = list(args.db.query(query, bindings))
     if not media:
         utils.no_media_found()
 
     return media
 
 
 def dl_download(args=None) -> None:
```

### Comparing `xklb-1.24.9/xklb/fs_extract.py` & `xklb-1.25.1/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/gui.py` & `xklb-1.25.1/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/hn_extract.py` & `xklb-1.25.1/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/lb.py` & `xklb-1.25.1/xklb/lb.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
       lb read                  Read books
       lb view                  View images
 
       lb bigdirs               Discover folders which take much room
-      lb mv-list               Reach a target free space by moving data across mount points
       lb dedupe                Deduplicate local db files
+      lb relmv                 Move files/folders while preserving relative paths
+      lb mv-list               Reach a target free space by moving data across mount points
+      lb scatter               Scatter files across multiple mountpoints (mergerfs balance)
 
       lb christen              Cleanse files by giving them a new name
 
     online media:
       lb tubeadd               Create a tube database; Add playlists
       lb tubeupdate            Fetch new videos from saved playlists
 
@@ -121,20 +123,22 @@
     subp_filesystem = add_parser(subparsers, SC.filesystem, ["fs"])
     subp_filesystem.set_defaults(func=filesystem)
 
     subp_bigdirs = add_parser(subparsers, "bigdirs", ["largefolders", "large_folders"])
     subp_bigdirs.set_defaults(func=scripts.bigdirs)
     subp_move_list = add_parser(subparsers, "mv-list", ["movelist", "move-list", "move_list"])
     subp_move_list.set_defaults(func=scripts.move_list)
+    subp_relmv = add_parser(subparsers, "relmv", ["rel-mv", "mvrel", "mv-rel"])
+    subp_relmv.set_defaults(func=scripts.relmv)
     subp_dedupe = add_parser(subparsers, "dedupe")
-    subp_dedupe.set_defaults(func=scripts.deduplicate_db)
+    subp_dedupe.set_defaults(func=scripts.dedupe)
     subp_scatter = add_parser(subparsers, "scatter")
     subp_scatter.set_defaults(func=scripts.scatter)
     subp_christen = add_parser(subparsers, "christen")
-    subp_christen.set_defaults(func=scripts.rename_invalid_paths)
+    subp_christen.set_defaults(func=scripts.christen)
     subp_merge_db = add_parser(subparsers, "merge-dbs")
     subp_merge_db.set_defaults(func=scripts.merge_dbs)
     subp_dedupe_local = add_parser(subparsers, "merge-online-local")
     subp_dedupe_local.set_defaults(func=scripts.merge_online_local)
     subp_optimize = add_parser(subparsers, "optimize")
     subp_optimize.set_defaults(func=scripts.optimize_db)
```

### Comparing `xklb-1.24.9/xklb/play_actions.py` & `xklb-1.25.1/xklb/play_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,19 +67,26 @@
 
     Print instead of play:
         library {action} --print --limit 10  # print the next 10 files
         library {action} -p -L 10  # print the next 10 files
         library {action} -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
 
         Printing modes
-        library {action} -p    # print in a table
-        library {action} -p p  # equivalent
+        library {action} -p    # print as a table
         library {action} -p a  # print an aggregate report
         library {action} -p b  # print a bigdirs report (see lb bigdirs -h for more info)
-        library {action} -p f  # print fields -- useful for piping paths to utilities like xargs or GNU Parallel
+        library {action} -p f  # print fields (defaults to path; use --cols to change)
+                               # -- useful for piping paths to utilities like xargs or GNU Parallel
+
+        library {action} -p d  # mark deleted
+        library {action} -p w  # mark watched
+
+        Some printing modes can be combined
+        library {action} -p df  # print files for piping into another program and mark them as deleted within the db
+        library {action} -p bf  # print fields from bigdirs report
 
         Check if you have downloaded something before
         library {action} -u duration -p -s 'title'
 
         Print an aggregate report of deleted media
         library {action} -w time_deleted!=0 -p=a
         ╒═══════════╤══════════════╤═════════╤═════════╕
@@ -87,22 +94,25 @@
         ╞═══════════╪══════════════╪═════════╪═════════╡
         │ Aggregate │ 14 days, 23  │ 50.6 GB │   29058 │
         │           │ hours and 42 │         │         │
         │           │ minutes      │         │         │
         ╘═══════════╧══════════════╧═════════╧═════════╛
         Total duration: 14 days, 23 hours and 42 minutes
 
-        Print an aggregate report of media that has no duration information (likely corrupt or online media)
+        Print an aggregate report of media that has no duration information (ie. online or corrupt local media)
         library {action} -w 'duration is null' -p=a
 
         Print a list of filenames which have below 1280px resolution
         library {action} -w 'width<1280' -p=f
 
         Print media you have partially viewed with mpv
-        library {action} -p=v
+        library {action} --partial -p
+        library {action} -P -p  # equivalent
+        library {action} -P -p f --cols path,progress,duration  # print CSV of partially watched files
+        library {action} --partial -pa  # print an aggregate report of partially watched files
 
         View how much time you have {action}ed
         library {action} -w play_count'>'0 -p=a
 
         See how much video you have
         library {action} video.db -p=a
         ╒═══════════╤═════════╤═════════╤═════════╕
@@ -461,78 +471,94 @@
 
     utils.timeout(args.timeout)
 
     args.sock = None
     return args
 
 
-def construct_search_bindings(args, cf, bindings, columns) -> None:
+def construct_search_bindings(args, columns) -> None:
     includes, excludes = db.gen_include_excludes(columns)
 
     for idx, inc in enumerate(args.include):
-        cf.append(includes.format(idx))
-        bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
+        args.filter_sql.append(includes.format(idx))
+        args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
     for idx, exc in enumerate(args.exclude):
-        cf.append(excludes.format(idx))
-        bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
+        args.filter_sql.append(excludes.format(idx))
+        args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
 
 
 def construct_query(args) -> Tuple[str, dict]:
     m_columns = args.db["media"].columns_dict
-    cf = []
-    bindings = {}
+    args.filter_sql = []
+    args.filter_bindings = {}
 
     if args.duration:
-        cf.append(" and duration IS NOT NULL " + args.duration)
+        args.filter_sql.append(" and duration IS NOT NULL " + args.duration)
     if args.size:
-        cf.append(" and size IS NOT NULL " + args.size)
+        args.filter_sql.append(" and size IS NOT NULL " + args.size)
     if args.duration_from_size:
-        cf.append(
+        args.filter_sql.append(
             " and size IS NOT NULL and duration in (select distinct duration from m where 1=1 "
             + args.duration_from_size
             + ")"
         )
 
-    cf.extend([" and " + w for w in args.where])
+    args.filter_sql.extend([" and " + w for w in args.where])
 
     def ii(string):
         if string.isdigit():
             return string + " minutes"
         return string.replace("mins", "minutes").replace("secs", "seconds")
 
     if args.created_within:
-        cf.append(f"and time_created > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.created_within)}')) as int)")
+        args.filter_sql.append(
+            f"and time_created > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.created_within)}')) as int)"
+        )
     if args.created_before:
-        cf.append(f"and time_created < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.created_before)}')) as int)")
+        args.filter_sql.append(
+            f"and time_created < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.created_before)}')) as int)"
+        )
     if args.changed_within:
-        cf.append(f"and time_modified > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.changed_within)}')) as int)")
+        args.filter_sql.append(
+            f"and time_modified > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.changed_within)}')) as int)"
+        )
     if args.changed_before:
-        cf.append(f"and time_modified < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.changed_before)}')) as int)")
+        args.filter_sql.append(
+            f"and time_modified < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.changed_before)}')) as int)"
+        )
     if args.played_within:
-        cf.append(f"and time_played > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_within)}')) as int)")
+        args.filter_sql.append(
+            f"and time_played > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_within)}')) as int)"
+        )
     if args.played_before:
-        cf.append(f"and time_played < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_before)}')) as int)")
+        args.filter_sql.append(
+            f"and time_played < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_before)}')) as int)"
+        )
     if args.deleted_within:
-        cf.append(f"and time_deleted > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_within)}')) as int)")
+        args.filter_sql.append(
+            f"and time_deleted > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_within)}')) as int)"
+        )
     if args.deleted_before:
-        cf.append(f"and time_deleted < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_before)}')) as int)")
+        args.filter_sql.append(
+            f"and time_deleted < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_before)}')) as int)"
+        )
 
     args.table = "media"
     if args.db["media"].detect_fts():
         if args.include:
-            args.table = db.fts_search(args, bindings)
+            args.table = db.fts_search(args)
             m_columns = {**m_columns, "rank": int}
         elif args.exclude:
-            construct_search_bindings(args, cf, bindings, m_columns)
+            construct_search_bindings(args, m_columns)
     else:
-        construct_search_bindings(args, cf, bindings, m_columns)
+        construct_search_bindings(args, m_columns)
 
     if args.table == "media" and not any(
         [
-            cf,
+            args.filter_sql,
             args.where,
             args.print,
             args.partial,
             args.lower,
             args.upper,
             args.limit != consts.DEFAULT_PLAY_QUEUE,
             args.duration_from_size,
@@ -544,49 +570,52 @@
 
         if "limit" in args.defaults:
             where_not_deleted = (
                 "where COALESCE(time_deleted,0) = 0"
                 if "time_deleted" in m_columns and "time_deleted" not in " ".join(sys.argv)
                 else ""
             )
-            cf.append(f"and m.rowid in (select rowid from media {where_not_deleted} order by random() limit {limit})")
-
-    args.sql_filter = " ".join(cf)
-    args.sql_filter_bindings = bindings
+            args.filter_sql.append(
+                f"and m.rowid in (select rowid from media {where_not_deleted} order by random() limit {limit})"
+            )
 
     duration = "duration"
     if args.action == SC.read:
         duration = "cast(length(tags) / 4.2 / 220 * 60 as INT) + 10 duration"
 
     cols = args.cols or ["path", "title", duration, "size", "subtitle_count", "is_dir", "rank"]
     SELECT = "\n        , ".join([c for c in cols if c in m_columns or c == "*"])
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     OFFSET = f"OFFSET {args.skip}" if args.skip and args.limit else ""
     query = f"""WITH m as (
     SELECT rowid, * FROM {args.table}
     WHERE 1=1
         {f'and path like "http%"' if args.safe else ''}
-        {f'and path not like "{Path(args.keep_dir).resolve()}%"' if args.post_action == 'askkeep' else ''}
+        {f'and path not like "{args.keep_dir}%"' if Path(args.keep_dir).exists() else ''}
         {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns and 'time_deleted' not in ' '.join(sys.argv) else ''}
         {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
         {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
         {'AND COALESCE(time_downloaded,0) = 0' if args.online_media_only else ''}
         {'AND COALESCE(time_downloaded,1)!= 0 AND path not like "http%"' if args.local_media_only else ''}
     )
     SELECT
         {SELECT}
     FROM m
     WHERE 1=1
-        {args.sql_filter}
+        {" ".join(args.filter_sql)}
     ORDER BY 1=1
         , {args.sort}
     {LIMIT} {OFFSET}
     """
 
-    return query, bindings
+    args.filter_sql = [
+        s for s in args.filter_sql if "rowid" not in s
+    ]  # only use random rowid constraint in first query
+
+    return query, args.filter_bindings
 
 
 def chromecast_play(args, m) -> None:
     if args.action in (SC.watch):
         catt_log = player.watch_chromecast(args, m, subtitles_file=externalize_subtitle(m["path"]))
     elif args.action in (SC.listen):
         catt_log = player.listen_chromecast(args, m)
@@ -621,63 +650,66 @@
         f" {next_video} && rm {temp_video}"
     )
     print(next_video)
     return next_video
 
 
 def play(args, m: Dict) -> None:
-    media_file = m["path"]
-
     if args.safe and not tube_backend.is_supported(m["path"]):
         log.info("[%s]: Skipping unsupported URL (safe_mode)", m["path"])
         return
 
-    if is_play_in_order_lvl2(args, media_file):
-        media_file = get_ordinal_media(args, media_file)
+    if is_play_in_order_lvl2(args, m["path"]):
+        m = get_ordinal_media(args, m)
+
+    original_path = m["path"]
+    if args.action in (SC.watch, SC.listen) and not m["path"].startswith("http"):
+        if args.prefix:
+            media_path = Path(args.prefix + m["path"]).resolve()
+        else:
+            media_path = Path(m["path"])
+        m["path"] = str(media_path)
 
-    if args.action in (SC.watch, SC.listen) and not media_file.startswith("http"):
-        media_path = Path(args.prefix + media_file).resolve()
         if not media_path.exists():
-            mark_media_deleted(args, media_file)
-            log.warning("[%s]: Does not exist. Skipping...", media_file)
+            log.warning("[%s]: Does not exist. Skipping...", m["path"])
+            mark_media_deleted(args, original_path)
             return
-        media_file = str(media_path)
 
         if args.transcode:
-            media_file = transcode(media_file)
+            media_file = transcode(m["path"])
 
-    print(now_playing(media_file))
+    print(now_playing(m["path"]))
 
-    args.player = player.parse(args, m, media_file)
+    args.player = player.parse(args, m)
 
     if args.chromecast:
         try:
             chromecast_play(args, m)
         except Exception as e:
             if args.ignore_errors:
                 return
             else:
                 raise e
         else:
-            player.post_act(args, media_file)
+            player.post_act(args, original_path)
 
     elif args.interdimensional_cable:
         return player.socket_play(args, m)
 
     else:
-        r = player.local_player(args, m, media_file)
+        r = player.local_player(args, m)
         if r.returncode != 0:
             print("Player exited with code", r.returncode)
             if args.ignore_errors:
                 return
             else:
                 raise SystemExit(r.returncode)
 
     if args.action in (SC.listen, SC.watch):
-        player.post_act(args, media_file)
+        player.post_act(args, original_path)
 
 
 def process_playqueue(args) -> None:
     query, bindings = construct_query(args)
 
     if args.print:
         player.printer(args, query, bindings)
```

### Comparing `xklb-1.24.9/xklb/playback.py` & `xklb-1.25.1/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/player.py` & `xklb-1.25.1/xklb/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import csv, operator, os, platform, re, shutil, socket, subprocess
+import csv, operator, os, platform, re, shutil, socket, subprocess, sys
 from copy import deepcopy
 from io import StringIO
 from numbers import Number
 from pathlib import Path
 from platform import system
 from random import randrange
 from shlex import join, quote, split
 from shutil import which
 from time import sleep
-from typing import List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 from rich.prompt import Confirm
 from tabulate import tabulate
 
 from scripts import process_bigdirs
 from xklb import consts, utils
 from xklb.consts import SC
@@ -68,37 +68,37 @@
         return get_browser()
 
     mimetype = cmd("xdg-mime", "query", "filetype", media_file).stdout
     default_application = cmd("xdg-mime", "query", "default", mimetype).stdout
     return which(default_application.replace(".desktop", ""))
 
 
-def parse(args, m=None, media_file=None) -> List[str]:
+def parse(args, m) -> List[str]:
     player = generic_player(args)
     mpv = which("mpv.com") or which("mpv")
 
     if args.override_player:
         player = args.override_player
         args.player_need_sleep = False
 
-    elif args.action in (SC.read) and media_file:
-        player_path = find_xdg_application(media_file)
+    elif args.action in (SC.read) and m["path"]:
+        player_path = find_xdg_application(m["path"])
         if player_path:
             args.player_need_sleep = False
             player = [player_path]
 
     elif mpv:
         args.player_need_sleep = False
         player = [mpv]
         if args.action in (SC.listen):
             player.extend([f"--input-ipc-server={args.mpv_socket}", "--no-video", "--keep-open=no", "--really-quiet"])
         elif args.action in (SC.watch):
             player.extend(["--force-window=yes", "--really-quiet"])
 
-        if media_file and media_file.startswith("http"):
+        if m["path"] and m["path"].startswith("http"):
             player.extend(["--script-opts=ytdl_hook-try_ytdl_first=yes"])
 
         if not args.multiple_playback:
             player.extend(["--fs"])
 
         if args.loop:
             player.extend(["--loop-file=inf"])
@@ -121,15 +121,15 @@
                 log.debug("Skipping subs player_args: size")
             elif m.get("time_partial_first"):
                 log.debug("Skipping subs player_args: partially watched")
             else:
                 player.extend(args.player_args_no_sub)
 
     elif system() == "Linux":
-        player_path = find_xdg_application(media_file)
+        player_path = find_xdg_application(m["path"])
         if player_path:
             args.player_need_sleep = False
             player = [player_path]
 
     log.debug("player: %s", player)
     return player
 
@@ -242,27 +242,28 @@
             utils.trash(p)
 
     return mark_media_deleted(args, paths)
 
 
 def delete_playlists(args, playlists) -> None:
     with args.db.conn:
+        playlist_paths = playlists + [p.rstrip(os.sep) for p in playlists]
         args.db.conn.execute(
-            "delete from playlists where path in (" + ",".join(["?"] * len(playlists)) + ")", playlists
+            "delete from playlists where path in (" + ",".join(["?"] * len(playlist_paths)) + ")", playlist_paths
         )
 
     online_media = [p for p in playlists if p.startswith("http")]
     if online_media:
         with args.db.conn:
             args.db.conn.execute(
                 "delete from media where playlist_path in (" + ",".join(["?"] * len(online_media)) + ")",
                 (*online_media,),
             )
 
-    local_media = [p for p in playlists if not p.startswith("http")]
+    local_media = [p.rstrip(os.sep) for p in playlists if not p.startswith("http")]
     for folder in local_media:
         with args.db.conn:
             args.db.conn.execute("delete from media where path like ?", (folder + "%",))
 
 
 def post_act(args, media_file: str, action=None) -> None:
     action = action or args.post_action
@@ -328,61 +329,61 @@
     while len(remove_chars) < 1:
         remove_chars += remove_groups[-number_of_groups]
         number_of_groups += 1
 
     return remove_chars
 
 
-def get_ordinal_media(args, path: str) -> str:
+def get_ordinal_media(args, m: Dict) -> Dict:
     # TODO: maybe try https://dba.stackexchange.com/questions/43415/algorithm-for-finding-the-longest-prefix
 
     columns = args.db["media"].columns_dict
 
     total_media = args.db.execute("select count(*) val from media").fetchone()[0]
-    candidate = deepcopy(path)
+    candidate = deepcopy(m["path"])
     similar_videos = []
     while len(similar_videos) < 2:
         if candidate == "":
-            return path
+            return m
 
         remove_chars = last_chars(candidate)
 
         new_candidate = candidate[: -len(remove_chars)]
         log.debug(f"Matches for '{new_candidate}':")
 
         if candidate in ("" or new_candidate):
-            return path
+            return m
 
         candidate = new_candidate
         query = f"""SELECT path FROM {'media' if args.play_in_order >= 3 else args.table}
             WHERE 1=1
                 and path like :candidate
                 {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in columns else ''}
-                {'' if args.play_in_order >= 2 else (args.sql_filter or '')}
+                {'' if args.play_in_order >= 2 else (" ".join(args.filter_sql) or '')}
             ORDER BY play_count, path
             LIMIT 1000
             """
         bindings = {"candidate": candidate + "%"}
         if args.play_in_order == 1:
             if args.include or args.exclude:
-                bindings = {**bindings, "query": args.sql_filter_bindings["query"]}
+                bindings = {**bindings, "query": args.filter_bindings["query"]}
         else:
-            bindings = {**bindings, **args.sql_filter_bindings}
+            bindings = {**bindings, **args.filter_bindings}
 
-        similar_videos = [d["path"] for d in args.db.query(query, bindings)]
+        similar_videos = [d for d in args.db.query(query, bindings)]
         log.debug(similar_videos)
 
         if len(similar_videos) > 999 or len(similar_videos) == total_media:
-            return path
+            return m
 
-        commonprefix = os.path.commonprefix(similar_videos)
+        commonprefix = os.path.commonprefix([d["path"] for d in similar_videos])
         log.debug(commonprefix)
         if len(Path(commonprefix).name) < 3:
             log.debug("Using commonprefix")
-            return path
+            return m
 
     return similar_videos[0]
 
 
 def watch_chromecast(args, m: dict, subtitles_file=None) -> Optional[subprocess.CompletedProcess]:
     if "vlc" in args.player:
         catt_log = cmd(
@@ -574,15 +575,15 @@
         if r == "DELETE":
             post_act(args, m["path"], action="delete")
         elif r == "KEEP" and args.post_action == "ask":
             post_act(args, m["path"], action="keep")
         elif r == "KEEP" and args.post_action == "askkeep":
             mv_to_keep_folder(args, m["path"])
         else:
-            raise Exception("I did not quite catch that... what did you say?")
+            raise NotImplementedError
     else:
         post_act(args, m["path"])
 
 
 def geom(x_size, y_size, x, y) -> str:
     return f"--geometry={x_size}x{y_size}+{x}+{y}"
 
@@ -631,19 +632,19 @@
             log.debug("-- A dragon slumbers over its hoard of %s media --", len(media))
             sleep(0.2)  # I don't know if this is necessary but may as well~~
     finally:
         for m in players:
             m["process"].kill()
 
 
-def local_player(args, m, media_file) -> subprocess.CompletedProcess:
+def local_player(args, m) -> subprocess.CompletedProcess:
     if system() == "Windows" or args.action in (SC.watch):
-        r = cmd(*args.player, media_file, strict=False)
+        r = cmd(*args.player, m["path"], strict=False)
     else:  # args.action in (SC.listen)
-        r = cmd_interactive(*args.player, media_file)
+        r = cmd_interactive(*args.player, m["path"])
 
     if args.player_need_sleep:
         if hasattr(m, "duration"):
             delay = m["duration"]
         else:
             delay = 10  # TODO: idk
         sleep(delay)
@@ -685,30 +686,29 @@
         if args.cols:
             for c in args.cols:
                 if isinstance(media[0][c], Number):
                     D[f"sum_{c}"] = sum((d[c] or 0) for d in media)
                     D[f"avg_{c}"] = sum((d[c] or 0) for d in media) / len(media)
         media = [D]
 
-    elif "d" in args.print:
-        mark_media_deleted(args, list(map(operator.itemgetter("path"), media)))
-        if not "f" in args.print:
-            return print(f"Removed {len(media)} metadata records")
-    elif "w" in args.print:
-        marked = mark_media_watched(args, list(map(operator.itemgetter("path"), media)))
-        if not "f" in args.print:
-            return print(f"Marked {marked} metadata records as watched")
+    else:
+        if "d" in args.print:
+            marked = mark_media_deleted(args, list(map(operator.itemgetter("path"), media)))
+            print(f"Marked {marked} metadata records as deleted", file=sys.stderr)
+        if "w" in args.print:
+            marked = mark_media_watched(args, list(map(operator.itemgetter("path"), media)))
+            print(f"Marked {marked} metadata records as watched", file=sys.stderr)
 
     if "f" in args.print:
         if args.limit == 1:
             f = media[0]["path"]
             if not Path(f).exists():
                 mark_media_deleted(args, f)
-                return printer(args, query, bindings)
-            print(quote(f))
+                return printer(args, query, bindings)  # try again to find a valid file
+            utils.pipe_print(quote(f))
         else:
             if not args.cols:
                 args.cols = ["path"]
 
             selected_cols = [{k: d.get(k, None) for k in args.cols} for d in media]
             virtual_csv = StringIO()
             wr = csv.writer(virtual_csv, quoting=csv.QUOTE_NONE)
```

### Comparing `xklb-1.24.9/xklb/praw_extract.py` & `xklb-1.25.1/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/stats.py` & `xklb-1.25.1/xklb/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,46 +45,44 @@
     args.action = consts.SC.stats
     return args
 
 
 def construct_query(args) -> Tuple[str, dict]:
     utils.ensure_playlists_exists(args)
     pl_columns = args.db["playlists"].columns_dict
-    cf = []
-    bindings = {}
+    args.filter_sql = []
+    args.filter_bindings = {}
 
-    cf.extend([" and " + w for w in args.where])
+    args.filter_sql.extend([" and " + w for w in args.where])
 
     args.table = "playlists"
     if args.db["playlists"].detect_fts():
         if args.include:
-            args.table = db.fts_search(args, bindings)
+            args.table = db.fts_search(args)
         elif args.exclude:
-            play_actions.construct_search_bindings(args, cf, bindings, pl_columns)
+            play_actions.construct_search_bindings(args, pl_columns)
     else:
-        play_actions.construct_search_bindings(args, cf, bindings, pl_columns)
-
-    args.sql_filter = " ".join(cf)
+        play_actions.construct_search_bindings(args, pl_columns)
 
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     query = f"""SELECT
         *
     FROM {args.table}
     WHERE 1=1
         and COALESCE(time_deleted,0) = 0
-        {args.sql_filter}
+        {" ".join(args.filter_sql)}
         and (category is null or category != '{consts.BLOCK_THE_CHANNEL}')
     ORDER BY 1=1
         {', ' + args.sort if args.sort else ''}
         , path
         , random()
     {LIMIT}
     """
 
-    return query, bindings
+    return query, args.filter_bindings
 
 
 def printer(args, query, bindings) -> None:
     media = list(args.db.query(query, bindings))
     media = utils.list_dict_filter_bool(media)
     if not media:
         utils.no_media_found()
```

### Comparing `xklb-1.24.9/xklb/subtitle.py` & `xklb-1.25.1/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/tabs_actions.py` & `xklb-1.25.1/xklb/tabs_actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,27 +139,25 @@
     AND category not like :exclude{x}
     AND frequency not like :exclude{x}
 )"""
 )
 
 
 def construct_tabs_query(args) -> Tuple[str, dict]:
-    cf = []
-    bindings = {}
+    args.filter_sql = []
+    args.filter_bindings = {}
 
-    cf.extend([" and " + w for w in args.where])
+    args.filter_sql.extend([" and " + w for w in args.where])
 
     for idx, inc in enumerate(args.include):
-        cf.append(tabs_include_string(idx))
-        bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
+        args.filter_sql.append(tabs_include_string(idx))
+        args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
     for idx, exc in enumerate(args.exclude):
-        cf.append(tabs_exclude_string(idx))
-        bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
-
-    args.sql_filter = " ".join(cf)
+        args.filter_sql.append(tabs_exclude_string(idx))
+        args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
 
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     OFFSET = f"OFFSET {args.skip}" if args.skip else ""
 
     query = f"""SELECT path
         , frequency
         , CASE
@@ -169,15 +167,15 @@
             WHEN frequency = 'quarterly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+3 Months' )) as int)
             WHEN frequency = 'yearly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+1 Year' )) as int)
         END time_valid
         {', ' + ', '.join(args.cols) if args.cols else ''}
     FROM media
     WHERE 1=1
         and COALESCE(time_deleted,0) = 0
-        {args.sql_filter}
+        {" ".join(args.filter_sql)}
         {"and time_valid < cast(STRFTIME('%s', datetime()) as int)" if not args.print else ''}
     ORDER BY 1=1
         {', ' + args.sort if args.sort else ''}
         {', time_played, time_valid, path' if args.print else ''}
         , play_count
         , frequency = 'daily' desc
         , frequency = 'weekly' desc
@@ -190,15 +188,15 @@
             , hostname
             , category
         ) -- prefer to spread hostname, category over time
         , random()
     {LIMIT} {OFFSET}
     """
 
-    return query, bindings
+    return query, args.filter_bindings
 
 
 def play(args, m: Dict) -> None:
     media_file = m["path"]
 
     cmd(*generic_player(args), media_file, strict=False)
     mark_media_watched(args, media_file)
```

### Comparing `xklb-1.24.9/xklb/tabs_extract.py` & `xklb-1.25.1/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/tube_backend.py` & `xklb-1.25.1/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/tube_extract.py` & `xklb-1.25.1/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.9/xklb/utils.py` & `xklb-1.25.1/xklb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, enum, errno, functools, hashlib, logging, math, multiprocessing, os, platform, re, shlex, shutil, signal, subprocess, sys, tempfile, textwrap
+import argparse, enum, functools, hashlib, logging, math, multiprocessing, os, platform, re, shlex, shutil, signal, subprocess, sys, tempfile, textwrap
 from ast import literal_eval
 from collections.abc import Iterable
 from datetime import datetime, timedelta
 from functools import wraps
 from pathlib import Path
 from random import shuffle
 from shutil import which
@@ -875,13 +875,11 @@
         unit = "m"
 
     return int(float(value) * time_units[unit])
 
 
 def pipe_print(x):
     try:
-        print(x)
-    except IOError as e:
-        if e.errno == errno.EPIPE:
-            pass
-        else:
-            raise e
+        print(x, flush=True)
+    except BrokenPipeError:
+        sys.stdout = None
+        exit(141)
```

### Comparing `xklb-1.24.9/PKG-INFO` & `xklb-1.25.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.24.9
+Version: 1.25.1
 Summary: xk library
 Home-page: https://github.com/chapmanjacobd/library/
 License: BSD-3-Clause
 Author: Jacob Chapman
 Author-email: 7908073+chapmanjacobd@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -39,15 +39,15 @@
 
 # xk media library
 
 A wise philosopher once told me: "[the future is autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
 Manage large media libraries. An index for your archive.
 Primary usage is local filesystem but also supports some virtual constructs like
-tracking online video playlists (eg. YouTube subscriptions) or daily browser tabs.
+tracking online video playlists (eg. YouTube subscriptions) and scheduling browser tabs.
 
 Required: `ffmpeg`
 
 Recommended: `mpv`, `fish`, `firefox`
 
 ## Install
 
@@ -56,28 +56,30 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.24.009)
+    xk media library subcommands (v1.25.001)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
       lb read                  Read books
       lb view                  View images
 
       lb bigdirs               Discover folders which take much room
-      lb mv-list               Reach a target free space by moving data across mount points
       lb dedupe                Deduplicate local db files
+      lb relmv                 Move files/folders while preserving relative paths
+      lb mv-list               Reach a target free space by moving data across mount points
+      lb scatter               Scatter files across multiple mountpoints (mergerfs balance)
 
       lb christen              Cleanse files by giving them a new name
 
     online media:
       lb tubeadd               Create a tube database; Add playlists
       lb tubeupdate            Fetch new videos from saved playlists
 
@@ -300,19 +302,26 @@
 
     Print instead of play:
         library watch --print --limit 10  # print the next 10 files
         library watch -p -L 10  # print the next 10 files
         library watch -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
 
         Printing modes
-        library watch -p    # print in a table
-        library watch -p p  # equivalent
+        library watch -p    # print as a table
         library watch -p a  # print an aggregate report
         library watch -p b  # print a bigdirs report (see lb bigdirs -h for more info)
-        library watch -p f  # print fields -- useful for piping paths to utilities like xargs or GNU Parallel
+        library watch -p f  # print fields (defaults to path; use --cols to change)
+                               # -- useful for piping paths to utilities like xargs or GNU Parallel
+
+        library watch -p d  # mark deleted
+        library watch -p w  # mark watched
+
+        Some printing modes can be combined
+        library watch -p df  # print files for piping into another program and mark them as deleted within the db
+        library watch -p bf  # print fields from bigdirs report
 
         Check if you have downloaded something before
         library watch -u duration -p -s 'title'
 
         Print an aggregate report of deleted media
         library watch -w time_deleted!=0 -p=a
         ╒═══════════╤══════════════╤═════════╤═════════╕
@@ -320,22 +329,25 @@
         ╞═══════════╪══════════════╪═════════╪═════════╡
         │ Aggregate │ 14 days, 23  │ 50.6 GB │   29058 │
         │           │ hours and 42 │         │         │
         │           │ minutes      │         │         │
         ╘═══════════╧══════════════╧═════════╧═════════╛
         Total duration: 14 days, 23 hours and 42 minutes
 
-        Print an aggregate report of media that has no duration information (likely corrupt or online media)
+        Print an aggregate report of media that has no duration information (ie. online or corrupt local media)
         library watch -w 'duration is null' -p=a
 
         Print a list of filenames which have below 1280px resolution
         library watch -w 'width<1280' -p=f
 
         Print media you have partially viewed with mpv
-        library watch -p=v
+        library watch --partial -p
+        library watch -P -p  # equivalent
+        library watch -P -p f --cols path,progress,duration  # print CSV of partially watched files
+        library watch --partial -pa  # print an aggregate report of partially watched files
 
         View how much time you have watched
         library watch -w play_count'>'0 -p=a
 
         See how much video you have
         library watch video.db -p=a
         ╒═══════════╤═════════╤═════════╤═════════╕
```

