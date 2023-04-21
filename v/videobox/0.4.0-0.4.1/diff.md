# Comparing `tmp/videobox-0.4.0.tar.gz` & `tmp/videobox-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videobox-0.4.0.tar", last modified: Sat Apr  8 08:53:56 2023, max compression
+gzip compressed data, was "videobox-0.4.1.tar", last modified: Fri Apr 21 07:40:51 2023, max compression
```

## Comparing `videobox-0.4.0.tar` & `videobox-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2023-04-08 08:53:56.508782 videobox-0.4.0/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1103 2023-02-15 11:35:53.000000 videobox-0.4.0/.gitignore
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2023-04-08 08:53:56.505488 videobox-0.4.0/.vscode/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      856 2023-02-08 10:49:32.000000 videobox-0.4.0/.vscode/launch.json
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       49 2023-01-19 15:12:32.000000 videobox-0.4.0/.vscode/settings.json
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1516 2023-01-19 15:12:32.000000 videobox-0.4.0/LICENSE
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4452 2023-04-08 08:53:56.508561 videobox-0.4.0/PKG-INFO
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3852 2023-04-08 08:43:41.000000 videobox-0.4.0/README.md
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       70 2023-01-19 15:12:32.000000 videobox-0.4.0/Videobox.code-workspace
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      158 2023-04-08 08:43:41.000000 videobox-0.4.0/debugger.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      550 2023-02-15 11:35:53.000000 videobox-0.4.0/makefile
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      916 2023-04-08 08:46:40.000000 videobox-0.4.0/pyproject.toml
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       48 2023-01-19 15:12:32.000000 videobox-0.4.0/requirements.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       38 2023-04-08 08:53:56.508826 videobox-0.4.0/setup.cfg
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2023-04-08 08:53:56.507307 videobox-0.4.0/videobox/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       64 2023-04-08 08:46:13.000000 videobox-0.4.0/videobox/__init__.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       40 2023-01-19 15:12:32.000000 videobox-0.4.0/videobox/__main__.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1644 2023-04-08 08:43:41.000000 videobox-0.4.0/videobox/api.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763    14229 2023-04-08 08:43:41.000000 videobox-0.4.0/videobox/main.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     9802 2023-04-08 08:43:41.000000 videobox-0.4.0/videobox/model.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763    13162 2023-04-08 08:43:41.000000 videobox-0.4.0/videobox/sync.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4153 2023-04-08 08:53:51.000000 videobox-0.4.0/videobox/trackers.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1124 2023-01-19 15:12:32.000000 videobox-0.4.0/videobox/utilities.py
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2023-04-08 08:53:56.508328 videobox-0.4.0/videobox.egg-info/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4452 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/PKG-INFO
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      495 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/SOURCES.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763        1 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/dependency_links.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       47 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/entry_points.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       58 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/requires.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763        9 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/top_level.txt
+drwxr-xr-x   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        0 2023-04-21 07:40:51.963616 videobox-0.4.1/
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     1103 2023-02-15 11:35:53.000000 videobox-0.4.1/.gitignore
+drwxr-xr-x   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        0 2023-04-21 07:40:51.960912 videobox-0.4.1/.vscode/
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)      856 2023-02-08 10:49:32.000000 videobox-0.4.1/.vscode/launch.json
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       49 2023-01-19 15:12:32.000000 videobox-0.4.1/.vscode/settings.json
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     1516 2023-01-19 15:12:32.000000 videobox-0.4.1/LICENSE
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     4452 2023-04-21 07:40:51.963450 videobox-0.4.1/PKG-INFO
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     3852 2023-04-08 08:43:41.000000 videobox-0.4.1/README.md
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       70 2023-01-19 15:12:32.000000 videobox-0.4.1/Videobox.code-workspace
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)      158 2023-04-08 08:43:41.000000 videobox-0.4.1/debugger.py
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)      550 2023-04-21 07:27:33.000000 videobox-0.4.1/makefile
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)      916 2023-04-21 07:35:36.000000 videobox-0.4.1/pyproject.toml
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       48 2023-04-21 07:27:33.000000 videobox-0.4.1/requirements.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       38 2023-04-21 07:40:51.963652 videobox-0.4.1/setup.cfg
+drwxr-xr-x   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        0 2023-04-21 07:40:51.962422 videobox-0.4.1/videobox/
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       64 2023-04-21 07:35:28.000000 videobox-0.4.1/videobox/__init__.py
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       40 2023-01-19 15:12:32.000000 videobox-0.4.1/videobox/__main__.py
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     1644 2023-04-19 08:04:47.000000 videobox-0.4.1/videobox/api.py
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)    14245 2023-04-21 07:27:33.000000 videobox-0.4.1/videobox/main.py
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     9802 2023-04-21 07:27:33.000000 videobox-0.4.1/videobox/model.py
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)    13187 2023-04-21 07:34:04.000000 videobox-0.4.1/videobox/sync.py
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     4161 2023-04-21 07:40:45.000000 videobox-0.4.1/videobox/trackers.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     1124 2023-04-21 07:27:33.000000 videobox-0.4.1/videobox/utilities.py
+drwxr-xr-x   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        0 2023-04-21 07:40:51.963246 videobox-0.4.1/videobox.egg-info/
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     4452 2023-04-21 07:40:51.000000 videobox-0.4.1/videobox.egg-info/PKG-INFO
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)      495 2023-04-21 07:40:51.000000 videobox-0.4.1/videobox.egg-info/SOURCES.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        1 2023-04-21 07:40:51.000000 videobox-0.4.1/videobox.egg-info/dependency_links.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       47 2023-04-21 07:40:51.000000 videobox-0.4.1/videobox.egg-info/entry_points.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       58 2023-04-21 07:40:51.000000 videobox-0.4.1/videobox.egg-info/requires.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        9 2023-04-21 07:40:51.000000 videobox-0.4.1/videobox.egg-info/top_level.txt
```

### Comparing `videobox-0.4.0/.gitignore` & `videobox-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `videobox-0.4.0/.vscode/launch.json` & `videobox-0.4.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `videobox-0.4.0/LICENSE` & `videobox-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `videobox-0.4.0/PKG-INFO` & `videobox-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: videobox
-Version: 0.4.0
-Summary: Video download CLI utility
+Version: 0.4.1
+Summary: TV series download utility
 Author: Andrea Peltrin
 Project-URL: Homepage, https://github.com/passiomatic/videobox
 Project-URL: Bug Tracker, https://github.com/passiomatic/videobox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `videobox-0.4.0/README.md` & `videobox-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `videobox-0.4.0/makefile` & `videobox-0.4.1/makefile`

 * *Files identical despite different names*

### Comparing `videobox-0.4.0/pyproject.toml` & `videobox-0.4.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "videobox"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Andrea Peltrin" },
 ]
-description = "Video download CLI utility"
+description = "TV series download utility"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
   "peewee >= 3.15.4,<4",
   "requests >= 2.28.1,<3",
   "termcolor >= 2.2.0,<3"
 ]
```

### Comparing `videobox-0.4.0/videobox/api.py` & `videobox-0.4.1/videobox/api.py`

 * *Files identical despite different names*

### Comparing `videobox-0.4.0/videobox/main.py` & `videobox-0.4.1/videobox/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     if not query:
         parser.error("missing query.")
 
     if query.startswith("#"):
         series = get_series_by_id(parser, query)
         best_releases = print_download_summary(parser, series, options)
     else:
-        results = model.search_series(query)
+        results = model.search_series(sanitize_query(query))
         if len(results) == 1:
             # Single match from FTS
             series = model.get_series(results[0].rowid)
             best_releases = print_download_summary(parser, series, options)
         elif results:
             # Multiple matches
             print(
```

### Comparing `videobox-0.4.0/videobox/model.py` & `videobox-0.4.1/videobox/model.py`

 * *Files identical despite different names*

### Comparing `videobox-0.4.0/videobox/sync.py` & `videobox-0.4.1/videobox/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,8 +328,8 @@
                 continue  # Next retry
             except HTTPError as ex:
                 message = f'Server error {ex.response.status_code} occurred while handling the request, giving up'
                 logging.error(message)
                 raise SyncError(message)
             return response.json()
         # No more retries, giving up
-        raise SyncError("Server timed out while handling the request")
+        raise SyncError("Server timed out while handling the request. Please try again later.")
```

### Comparing `videobox-0.4.0/videobox/trackers.txt` & `videobox-0.4.1/videobox/trackers.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-http://1337.abcvg.info:80/announce,http://bt.endpot.com:80/announce,http://bt.okmp3.ru:2710/announce,http://incine.ru:6969/announce,http://nyaa.tracker.wf:7777/announce,http://open.acgnxtracker.com:80/announce,http://open.tracker.ink:6969/announce,http://p2p.0g.cx:6969/announce,http://parag.rs:6969/announce,http://share.camoe.cn:8080/announce,http://torrentsmd.com:8080/announce,http://tr.cili001.com:8070/announce,http://tracker.bt4g.com:2095/announce,http://tracker.files.fm:6969/announce,http://tracker.gbitt.info:80/announce,http://tracker.mywaifu.best:6969/announce,http://tracker.openbittorrent.com:80/announce,http://tracker.renfei.net:8080/announce,http://tracker.skyts.net:6969/announce,http://tracker.tfile.co:80/announce,http://trackme.theom.nz:80/announce,http://v6-tracker.0g.cx:6969/announce,http://www.all4nothin.net:80/announce.php,http://www.wareztorrent.com:80/announce,https://1337.abcvg.info:443/announce,https://opentracker.i2p.rocks:443/announce,https://t1.hloli.org:443/announce,https://tr.abiir.top:443/announce,https://tr.burnabyhighstar.com:443/announce,https://tracker.foreverpirates.co:443/announce,https://tracker.gbitt.info:443/announce,https://tracker.imgoingto.icu:443/announce,https://tracker.kuroy.me:443/announce,https://tracker.lilithraws.cf:443/announce,https://tracker.loligirl.cn:443/announce,https://tracker.tamersunion.org:443/announce,https://tracker1.520.jp:443/announce,https://trackme.theom.nz:443/announce,udp://9.rarbg.com:2810/announce,udp://aarsen.me:6969/announce,udp://acxx.de:6969/announce,udp://aegir.sexy:6969/announce,udp://astrr.ru:6969/announce,udp://bedro.cloud:6969/announce,udp://boysbitte.be:6969/announce,udp://bt.ktrackers.com:6666/announce,udp://bt1.archive.org:6969/announce,udp://epider.me:6969/announce,udp://exodus.desync.com:6969/announce,udp://htz3.noho.st:6969/announce,udp://ipv6.tracker.monitorit4.me:6969/announce,udp://laze.cc:6969/announce,udp://linfan.moe:6969/announce,udp://mail.artixlinux.org:6969/announce,udp://moonburrow.club:6969/announce,udp://movies.zsw.ca:6969/announce,udp://open.4ever.tk:6969/announce,udp://open.demonii.com:1337/announce,udp://open.dstud.io:6969/announce,udp://open.publictracker.xyz:6969/announce,udp://open.stealth.si:80/announce,udp://open.tracker.cl:1337/announce,udp://open.tracker.ink:6969/announce,udp://opentor.org:2710/announce,udp://opentracker.i2p.rocks:6969/announce,udp://opentracker.io:6969/announce,udp://p4p.arenabg.com:1337/announce,udp://private.anonseed.com:6969/announce,udp://retracker01-msk-virt.corbina.net:80/announce,udp://run.publictracker.xyz:6969/announce,udp://sanincode.com:6969/announce,udp://static.54.161.216.95.clients.your-server.de:6969/announce,udp://t.133335.xyz:6969/announce,udp://thagoat.rocks:6969/announce,udp://thetracker.org:80/announce,udp://torrents.artixlinux.org:6969/announce,udp://tracker-udp.gbitt.info:80/announce,udp://tracker.4.babico.name.tr:3131/announce,udp://tracker.altrosky.nl:6969/announce,udp://tracker.artixlinux.org:6969/announce,udp://tracker.auctor.tv:6969/announce,udp://tracker.beeimg.com:6969/announce,udp://tracker.birkenwald.de:6969/announce,udp://tracker.bitsearch.to:1337/announce,udp://tracker.ccp.ovh:6969/announce,udp://tracker.cyberia.is:6969/announce,udp://tracker.dler.com:6969/announce,udp://tracker.doko.moe:6969/announce,udp://tracker.filemail.com:6969/announce,udp://tracker.jonaslsa.com:6969/announce,udp://tracker.leech.ie:1337/announce,udp://tracker.moeking.me:6969/announce,udp://tracker.monitorit4.me:6969/announce,udp://tracker.openbittorrent.com:6969/announce,udp://tracker.opentrackr.org:1337/announce,udp://tracker.skyts.net:6969/announce,udp://tracker.srv00.com:6969/announce,udp://tracker.theoks.net:6969/announce,udp://tracker.torrent.eu.org:451/announce,udp://tracker1.bt.moack.co.kr:80/announce,udp://tracker2.dler.com:80/announce,udp://tracker6.lelux.fi:6969/announce,udp://u4.trakx.crim.ist:1337/announce,udp://u6.trakx.crim.ist:1337/announce,udp://uploads.gamecoast.net:6969/announce,udp://v1046920.hosted-by-vdsina.ru:6969/announce,udp://wepzone.net:6969/announce,ws://hub.bugout.link:80/announce,wss://tracker.openwebtorrent.com:443/announce
+http://1337.abcvg.info:80/announce,http://bt.endpot.com:80/announce,http://bt.okmp3.ru:2710/announce,http://dn42.smrsh.net:6969/announce,http://nyaa.tracker.wf:7777/announce,http://open.acgnxtracker.com:80/announce,http://p2p.0g.cx:6969/announce,http://parag.rs:6969/announce,http://share.camoe.cn:8080/announce,http://t.acg.rip:6699/announce,http://t.nyaatracker.com:80/announce,http://torrentsmd.com:8080/announce,http://tr.cili001.com:8070/announce,http://tracker.bt4g.com:2095/announce,http://tracker.files.fm:6969/announce,http://tracker.gbitt.info:80/announce,http://tracker.mywaifu.best:6969/announce,http://tracker.openbittorrent.com:80/announce,http://tracker.renfei.net:8080/announce,http://tracker.tfile.co:80/announce,http://v6-tracker.0g.cx:6969/announce,http://www.all4nothin.net:80/announce.php,http://www.wareztorrent.com:80/announce,https://1337.abcvg.info:443/announce,https://opentracker.i2p.rocks:443/announce,https://t1.hloli.org:443/announce,https://tr.burnabyhighstar.com:443/announce,https://tr.ready4.icu:443/announce,https://tracker.foreverpirates.co:443/announce,https://tracker.gbitt.info:443/announce,https://tracker.imgoingto.icu:443/announce,https://tracker.kuroy.me:443/announce,https://tracker.lilithraws.cf:443/announce,https://tracker.loligirl.cn:443/announce,https://tracker.tamersunion.org:443/announce,https://tracker1.520.jp:443/announce,udp://9.rarbg.com:2810/announce,udp://aarsen.me:6969/announce,udp://acxx.de:6969/announce,udp://aegir.sexy:6969/announce,udp://astrr.ru:6969/announce,udp://bedro.cloud:6969/announce,udp://bt.ktrackers.com:6666/announce,udp://bt1.archive.org:6969/announce,udp://epider.me:6969/announce,udp://exodus.desync.com:6969/announce,udp://htz3.noho.st:6969/announce,udp://ipv6.tracker.monitorit4.me:6969/announce,udp://laze.cc:6969/announce,udp://linfan.moe:6969/announce,udp://mail.artixlinux.org:6969/announce,udp://moonburrow.club:6969/announce,udp://movies.zsw.ca:6969/announce,udp://open.demonii.com:1337/announce,udp://open.dstud.io:6969/announce,udp://open.stealth.si:80/announce,udp://open.tracker.cl:1337/announce,udp://open.tracker.ink:6969/announce,udp://opentor.org:2710/announce,udp://opentracker.i2p.rocks:6969/announce,udp://opentracker.io:6969/announce,udp://p4p.arenabg.com:1337/announce,udp://private.anonseed.com:6969/announce,udp://retracker.hotplug.ru:2710/announce,udp://retracker01-msk-virt.corbina.net:80/announce,udp://run.publictracker.xyz:6969/announce,udp://sanincode.com:6969/announce,udp://static.54.161.216.95.clients.your-server.de:6969/announce,udp://t.133335.xyz:6969/announce,udp://thagoat.rocks:6969/announce,udp://thetracker.org:80/announce,udp://thinking.duckdns.org:6969/announce,udp://thouvenin.cloud:6969/announce,udp://torrents.artixlinux.org:6969/announce,udp://tracker-udp.gbitt.info:80/announce,udp://tracker.4.babico.name.tr:3131/announce,udp://tracker.altrosky.nl:6969/announce,udp://tracker.artixlinux.org:6969/announce,udp://tracker.auctor.tv:6969/announce,udp://tracker.beeimg.com:6969/announce,udp://tracker.birkenwald.de:6969/announce,udp://tracker.bitsearch.to:1337/announce,udp://tracker.cubonegro.lol:6969/announce,udp://tracker.cyberia.is:6969/announce,udp://tracker.dler.com:6969/announce,udp://tracker.doko.moe:6969/announce,udp://tracker.jonaslsa.com:6969/announce,udp://tracker.leech.ie:1337/announce,udp://tracker.moeking.me:6969/announce,udp://tracker.monitorit4.me:6969/announce,udp://tracker.openbittorrent.com:6969/announce,udp://tracker.opentrackr.org:1337/announce,udp://tracker.pimpmyworld.to:6969/announce,udp://tracker.skyts.net:6969/announce,udp://tracker.srv00.com:6969/announce,udp://tracker.theoks.net:6969/announce,udp://tracker.torrent.eu.org:451/announce,udp://tracker1.bt.moack.co.kr:80/announce,udp://tracker2.dler.com:80/announce,udp://tracker2.dler.org:80/announce,udp://tracker6.lelux.fi:6969/announce,udp://u4.trakx.crim.ist:1337/announce,udp://u6.trakx.crim.ist:1337/announce,udp://uploads.gamecoast.net:6969/announce,udp://v1046920.hosted-by-vdsina.ru:6969/announce,udp://wepzone.net:6969/announce,udp://zecircle.xyz:6969/announce,ws://hub.bugout.link:80/announce,wss://tracker.openwebtorrent.com:443/announce
```

### Comparing `videobox-0.4.0/videobox/utilities.py` & `videobox-0.4.1/videobox/utilities.py`

 * *Files identical despite different names*

### Comparing `videobox-0.4.0/videobox.egg-info/PKG-INFO` & `videobox-0.4.1/videobox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: videobox
-Version: 0.4.0
-Summary: Video download CLI utility
+Version: 0.4.1
+Summary: TV series download utility
 Author: Andrea Peltrin
 Project-URL: Homepage, https://github.com/passiomatic/videobox
 Project-URL: Bug Tracker, https://github.com/passiomatic/videobox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

