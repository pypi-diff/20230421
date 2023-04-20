# Comparing `tmp/copyparty-1.6.8.tar.gz` & `tmp/copyparty-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyparty-1.6.8.tar", last modified: Sun Mar 12 18:24:19 2023, max compression
+gzip compressed data, was "copyparty-1.6.9.tar", last modified: Thu Mar 16 22:12:28 2023, max compression
```

## Comparing `copyparty-1.6.8.tar` & `copyparty-1.6.9.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.173330 copyparty-1.6.8/
--rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.6.8/LICENSE
--rw-r--r--   0 ed        (1000) ed        (1000)      102 2023-03-12 18:24:18.000000 copyparty-1.6.8/MANIFEST.in
--rw-r--r--   0 ed        (1000) ed        (1000)    81877 2023-03-12 18:24:19.172330 copyparty-1.6.8/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)    80081 2023-03-12 16:24:23.000000 copyparty-1.6.8/README.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.157330 copyparty-1.6.8/bin/
--rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-03-12 18:22:26.000000 copyparty-1.6.8/bin/partyfuse.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    35130 2023-03-12 18:22:26.000000 copyparty-1.6.8/bin/up2k.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.161330 copyparty-1.6.8/copyparty/
--rw-r--r--   0 ed        (1000) ed        (1000)     1063 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    66703 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/__main__.py
--rw-r--r--   0 ed        (1000) ed        (1000)      247 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/__version__.py
--rw-r--r--   0 ed        (1000) ed        (1000)    62030 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/authsrv.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.162330 copyparty-1.6.8/copyparty/bos/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/bos/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/bos/bos.py
--rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/bos/path.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3590 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/broker_mp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/broker_mpw.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/broker_thr.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/broker_util.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6436 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/cfg.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/dxml.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/fsutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    13815 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/ftpd.py
--rw-r--r--   0 ed        (1000) ed        (1000)   119171 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/httpcli.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6674 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/httpconn.py
--rw-r--r--   0 ed        (1000) ed        (1000)    14143 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/httpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2643 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/ico.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16978 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/mdns.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16844 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/mtag.py
--rw-r--r--   0 ed        (1000) ed        (1000)    11520 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/multicast.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.162330 copyparty-1.6.8/copyparty/res/
--rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/res/COPYING.txt
--rw-r--r--   0 ed        (1000) ed        (1000)     2876 2021-09-11 12:44:53.000000 copyparty-1.6.8/copyparty/res/insecure.pem
--rw-r--r--   0 ed        (1000) ed        (1000)    10616 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/smbd.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6153 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/ssdp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2699 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/star.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.162330 copyparty-1.6.8/copyparty/stolen/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.163330 copyparty-1.6.8/copyparty/stolen/dnslib/
--rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/dnslib/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/dnslib/bimap.py
--rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/dnslib/bit.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/dnslib/buffer.py
--rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/dnslib/dns.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/dnslib/label.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/dnslib/lex.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/dnslib/ranges.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.164330 copyparty-1.6.8/copyparty/stolen/ifaddr/
--rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/ifaddr/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/ifaddr/_posix.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/ifaddr/_shared.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/ifaddr/_win32.py
--rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/qrcodegen.py
--rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/stolen/surrogateescape.py
--rw-r--r--   0 ed        (1000) ed        (1000)      972 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/sutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    22903 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/svchub.py
--rw-r--r--   0 ed        (1000) ed        (1000)     8166 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/szip.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16633 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/tcpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3826 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/th_cli.py
--rw-r--r--   0 ed        (1000) ed        (1000)    20969 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/th_srv.py
--rw-r--r--   0 ed        (1000) ed        (1000)    10474 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/u2idx.py
--rw-r--r--   0 ed        (1000) ed        (1000)   121053 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/up2k.py
--rw-r--r--   0 ed        (1000) ed        (1000)    71782 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/util.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.166330 copyparty-1.6.8/copyparty/web/
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.167330 copyparty-1.6.8/copyparty/web/a/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/web/a/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/web/a/partyfuse.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    35130 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/web/a/up2k.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.6.8/copyparty/web/a/webdav-cfg.bat
--rw-r--r--   0 ed        (1000) ed        (1000)     7282 2023-01-08 13:51:21.000000 copyparty-1.6.8/copyparty/web/baguettebox.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    10896 2023-03-11 11:07:00.000000 copyparty-1.6.8/copyparty/web/browser.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     5264 2023-02-04 15:16:41.000000 copyparty-1.6.8/copyparty/web/browser.html
--rw-r--r--   0 ed        (1000) ed        (1000)    57106 2023-03-09 22:34:56.000000 copyparty-1.6.8/copyparty/web/browser.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.6.8/copyparty/web/browser2.html
--rw-r--r--   0 ed        (1000) ed        (1000)      585 2022-07-03 13:28:49.000000 copyparty-1.6.8/copyparty/web/cf.html
--rw-r--r--   0 ed        (1000) ed        (1000)      126 2021-09-11 12:44:53.000000 copyparty-1.6.8/copyparty/web/copyparty.gif
--rw-r--r--   0 ed        (1000) ed        (1000)      687 2022-07-14 21:26:48.000000 copyparty-1.6.8/copyparty/web/dbg-audio.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.168330 copyparty-1.6.8/copyparty/web/dd/
--rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.6.8/copyparty/web/dd/2.png
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.6.8/copyparty/web/dd/3.png
--rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.6.8/copyparty/web/dd/4.png
--rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.6.8/copyparty/web/dd/5.png
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/web/dd/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.171330 copyparty-1.6.8/copyparty/web/deps/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-12 18:22:26.000000 copyparty-1.6.8/copyparty/web/deps/__init__.py
--rw-rw-r--   0 ed        (1000) ed        (1000)     3053 2022-12-20 10:12:25.000000 copyparty-1.6.8/copyparty/web/deps/easymde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    76951 2022-12-29 03:38:30.000000 copyparty-1.6.8/copyparty/web/deps/easymde.js.gz
--rw-rw-r--   0 ed        (1000) ed        (1000)    14556 2022-12-29 03:37:35.000000 copyparty-1.6.8/copyparty/web/deps/marked.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      584 2022-12-29 03:38:53.000000 copyparty-1.6.8/copyparty/web/deps/mini-fa.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2784 2022-12-29 03:38:54.000000 copyparty-1.6.8/copyparty/web/deps/mini-fa.woff
--rw-r--r--   0 ed        (1000) ed        (1000)     1478 2022-12-29 03:41:18.000000 copyparty-1.6.8/copyparty/web/deps/prism.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.6.8/copyparty/web/deps/prism.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1647 2022-12-29 03:41:18.000000 copyparty-1.6.8/copyparty/web/deps/prismd.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8612 2022-12-29 03:38:54.000000 copyparty-1.6.8/copyparty/web/deps/scp.woff2
--rw-r--r--   0 ed        (1000) ed        (1000)     7043 2022-12-29 03:37:01.000000 copyparty-1.6.8/copyparty/web/deps/sha512.ac.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8119 2021-07-22 23:48:12.000000 copyparty-1.6.8/copyparty/web/deps/sha512.hw.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.6.8/copyparty/web/md.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     4063 2022-12-10 20:27:29.000000 copyparty-1.6.8/copyparty/web/md.html
--rw-r--r--   0 ed        (1000) ed        (1000)     4112 2022-12-01 22:41:40.000000 copyparty-1.6.8/copyparty/web/md.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      680 2022-12-01 22:41:28.000000 copyparty-1.6.8/copyparty/web/md2.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8209 2023-01-25 20:58:01.000000 copyparty-1.6.8/copyparty/web/md2.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.6.8/copyparty/web/mde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1640 2022-12-10 20:27:33.000000 copyparty-1.6.8/copyparty/web/mde.html
--rw-r--r--   0 ed        (1000) ed        (1000)     2218 2022-12-01 07:23:41.000000 copyparty-1.6.8/copyparty/web/mde.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.6.8/copyparty/web/msg.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      898 2022-12-10 19:57:40.000000 copyparty-1.6.8/copyparty/web/msg.html
--rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.6.8/copyparty/web/splash.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     3741 2023-02-19 19:41:20.000000 copyparty-1.6.8/copyparty/web/splash.html
--rw-r--r--   0 ed        (1000) ed        (1000)     1235 2023-02-17 22:28:18.000000 copyparty-1.6.8/copyparty/web/splash.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     9354 2023-03-06 02:42:55.000000 copyparty-1.6.8/copyparty/web/svcs.html
--rw-r--r--   0 ed        (1000) ed        (1000)      519 2022-12-04 17:10:33.000000 copyparty-1.6.8/copyparty/web/svcs.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2377 2023-02-02 22:14:39.000000 copyparty-1.6.8/copyparty/web/ui.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    21538 2023-03-06 02:35:26.000000 copyparty-1.6.8/copyparty/web/up2k.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    12555 2023-03-01 22:53:27.000000 copyparty-1.6.8/copyparty/web/util.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1059 2023-03-02 22:42:45.000000 copyparty-1.6.8/copyparty/web/w.hash.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-12 18:24:19.161330 copyparty-1.6.8/copyparty.egg-info/
--rw-r--r--   0 ed        (1000) ed        (1000)    81877 2023-03-12 18:24:18.000000 copyparty-1.6.8/copyparty.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)     2828 2023-03-12 18:24:19.000000 copyparty-1.6.8/copyparty.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-03-12 18:24:18.000000 copyparty-1.6.8/copyparty.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       54 2023-03-12 18:24:18.000000 copyparty-1.6.8/copyparty.egg-info/entry_points.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      117 2023-03-12 18:24:18.000000 copyparty-1.6.8/copyparty.egg-info/requires.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-03-12 18:24:18.000000 copyparty-1.6.8/copyparty.egg-info/top_level.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-03-12 18:24:19.173330 copyparty-1.6.8/setup.cfg
--rwxr-xr-x   0 ed        (1000) ed        (1000)     4479 2023-02-15 18:44:28.000000 copyparty-1.6.8/setup.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.984793 copyparty-1.6.9/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.6.9/LICENSE
+-rw-r--r--   0 ed        (1000) ed        (1000)      102 2023-03-16 22:12:27.000000 copyparty-1.6.9/MANIFEST.in
+-rw-r--r--   0 ed        (1000) ed        (1000)    82692 2023-03-16 22:12:28.983793 copyparty-1.6.9/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)    80896 2023-03-16 21:13:36.000000 copyparty-1.6.9/README.md
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.968793 copyparty-1.6.9/bin/
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-03-16 22:10:54.000000 copyparty-1.6.9/bin/partyfuse.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    35130 2023-03-16 22:10:54.000000 copyparty-1.6.9/bin/up2k.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.972793 copyparty-1.6.9/copyparty/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1063 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    66891 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/__main__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      247 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/__version__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    62030 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/authsrv.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.973793 copyparty-1.6.9/copyparty/bos/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/bos/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/bos/bos.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/bos/path.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3590 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/broker_mp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/broker_mpw.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/broker_thr.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/broker_util.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6436 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/cfg.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/dxml.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/fsutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    13841 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/ftpd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   119888 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/httpcli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6674 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/httpconn.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    14143 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/httpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2643 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/ico.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16978 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/mdns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16844 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/mtag.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    11520 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/multicast.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.974793 copyparty-1.6.9/copyparty/res/
+-rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/res/COPYING.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)     2876 2021-09-11 12:44:53.000000 copyparty-1.6.9/copyparty/res/insecure.pem
+-rw-r--r--   0 ed        (1000) ed        (1000)    10616 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/smbd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6153 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/ssdp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2699 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/star.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.974793 copyparty-1.6.9/copyparty/stolen/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.975793 copyparty-1.6.9/copyparty/stolen/dnslib/
+-rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/dnslib/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/dnslib/bimap.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/dnslib/bit.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/dnslib/buffer.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/dnslib/dns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/dnslib/label.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/dnslib/lex.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/dnslib/ranges.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.975793 copyparty-1.6.9/copyparty/stolen/ifaddr/
+-rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/ifaddr/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/ifaddr/_posix.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/ifaddr/_shared.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/ifaddr/_win32.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/qrcodegen.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/stolen/surrogateescape.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      972 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/sutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    22903 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/svchub.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     8166 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/szip.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16633 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/tcpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3826 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/th_cli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    20969 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/th_srv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    10493 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/u2idx.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   121148 2023-03-16 22:10:55.000000 copyparty-1.6.9/copyparty/up2k.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    71782 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/util.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.978793 copyparty-1.6.9/copyparty/web/
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.979793 copyparty-1.6.9/copyparty/web/a/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/web/a/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/web/a/partyfuse.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    35130 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/web/a/up2k.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.6.9/copyparty/web/a/webdav-cfg.bat
+-rw-r--r--   0 ed        (1000) ed        (1000)     7282 2023-01-08 13:51:21.000000 copyparty-1.6.9/copyparty/web/baguettebox.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    10925 2023-03-16 20:21:53.000000 copyparty-1.6.9/copyparty/web/browser.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     5286 2023-03-15 22:20:24.000000 copyparty-1.6.9/copyparty/web/browser.html
+-rw-r--r--   0 ed        (1000) ed        (1000)    57351 2023-03-16 20:51:53.000000 copyparty-1.6.9/copyparty/web/browser.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.6.9/copyparty/web/browser2.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      585 2022-07-03 13:28:49.000000 copyparty-1.6.9/copyparty/web/cf.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      126 2021-09-11 12:44:53.000000 copyparty-1.6.9/copyparty/web/copyparty.gif
+-rw-r--r--   0 ed        (1000) ed        (1000)      687 2022-07-14 21:26:48.000000 copyparty-1.6.9/copyparty/web/dbg-audio.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.980793 copyparty-1.6.9/copyparty/web/dd/
+-rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.6.9/copyparty/web/dd/2.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.6.9/copyparty/web/dd/3.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.6.9/copyparty/web/dd/4.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.6.9/copyparty/web/dd/5.png
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/web/dd/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.983793 copyparty-1.6.9/copyparty/web/deps/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-16 22:10:54.000000 copyparty-1.6.9/copyparty/web/deps/__init__.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)     3053 2022-12-20 10:12:25.000000 copyparty-1.6.9/copyparty/web/deps/easymde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    76951 2022-12-29 03:38:30.000000 copyparty-1.6.9/copyparty/web/deps/easymde.js.gz
+-rw-rw-r--   0 ed        (1000) ed        (1000)    14556 2022-12-29 03:37:35.000000 copyparty-1.6.9/copyparty/web/deps/marked.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      584 2022-12-29 03:38:53.000000 copyparty-1.6.9/copyparty/web/deps/mini-fa.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2784 2022-12-29 03:38:54.000000 copyparty-1.6.9/copyparty/web/deps/mini-fa.woff
+-rw-r--r--   0 ed        (1000) ed        (1000)     1478 2022-12-29 03:41:18.000000 copyparty-1.6.9/copyparty/web/deps/prism.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.6.9/copyparty/web/deps/prism.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1647 2022-12-29 03:41:18.000000 copyparty-1.6.9/copyparty/web/deps/prismd.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8612 2022-12-29 03:38:54.000000 copyparty-1.6.9/copyparty/web/deps/scp.woff2
+-rw-r--r--   0 ed        (1000) ed        (1000)     7043 2022-12-29 03:37:01.000000 copyparty-1.6.9/copyparty/web/deps/sha512.ac.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8119 2021-07-22 23:48:12.000000 copyparty-1.6.9/copyparty/web/deps/sha512.hw.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.6.9/copyparty/web/md.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     4063 2022-12-10 20:27:29.000000 copyparty-1.6.9/copyparty/web/md.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     4112 2022-12-01 22:41:40.000000 copyparty-1.6.9/copyparty/web/md.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      680 2022-12-01 22:41:28.000000 copyparty-1.6.9/copyparty/web/md2.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8209 2023-01-25 20:58:01.000000 copyparty-1.6.9/copyparty/web/md2.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.6.9/copyparty/web/mde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1640 2022-12-10 20:27:33.000000 copyparty-1.6.9/copyparty/web/mde.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     2218 2022-12-01 07:23:41.000000 copyparty-1.6.9/copyparty/web/mde.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.6.9/copyparty/web/msg.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      898 2022-12-10 19:57:40.000000 copyparty-1.6.9/copyparty/web/msg.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.6.9/copyparty/web/splash.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     3741 2023-02-19 19:41:20.000000 copyparty-1.6.9/copyparty/web/splash.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     1235 2023-02-17 22:28:18.000000 copyparty-1.6.9/copyparty/web/splash.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     9354 2023-03-06 02:42:55.000000 copyparty-1.6.9/copyparty/web/svcs.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      519 2022-12-04 17:10:33.000000 copyparty-1.6.9/copyparty/web/svcs.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2377 2023-02-02 22:14:39.000000 copyparty-1.6.9/copyparty/web/ui.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    21538 2023-03-06 02:35:26.000000 copyparty-1.6.9/copyparty/web/up2k.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    12616 2023-03-16 19:44:44.000000 copyparty-1.6.9/copyparty/web/util.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1059 2023-03-02 22:42:45.000000 copyparty-1.6.9/copyparty/web/w.hash.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-16 22:12:28.973793 copyparty-1.6.9/copyparty.egg-info/
+-rw-r--r--   0 ed        (1000) ed        (1000)    82692 2023-03-16 22:12:28.000000 copyparty-1.6.9/copyparty.egg-info/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)     2828 2023-03-16 22:12:28.000000 copyparty-1.6.9/copyparty.egg-info/SOURCES.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-03-16 22:12:28.000000 copyparty-1.6.9/copyparty.egg-info/dependency_links.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       54 2023-03-16 22:12:28.000000 copyparty-1.6.9/copyparty.egg-info/entry_points.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      117 2023-03-16 22:12:28.000000 copyparty-1.6.9/copyparty.egg-info/requires.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-03-16 22:12:28.000000 copyparty-1.6.9/copyparty.egg-info/top_level.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-03-16 22:12:28.984793 copyparty-1.6.9/setup.cfg
+-rwxr-xr-x   0 ed        (1000) ed        (1000)     4479 2023-02-15 18:44:28.000000 copyparty-1.6.9/setup.py
```

### Comparing `copyparty-1.6.8/LICENSE` & `copyparty-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/PKG-INFO` & `copyparty-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.6.8
+Version: 1.6.9
 Summary: Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Home-page: https://github.com/9001/copyparty
 Author: ed
 Author-email: copyparty@ocv.me
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -48,15 +48,15 @@
 
 turn your phone or raspi into a portable file server with resumable uploads/downloads using *any* web browser
 
 * server only needs Python (`2.7` or `3.3+`), all dependencies optional
 * browse/upload with [IE4](#browser-support) / netscape4.0 on win3.11 (heh)
 * protocols: [http](#the-browser) // [ftp](#ftp-server) // [webdav](#webdav-server) // [smb/cifs](#smb-server)
 
-try the **[read-only demo server](https://a.ocv.me/pub/demo/)** 👀 running from a basement in finland
+**[Get started](#quickstart)!** or visit the **[read-only demo server](https://a.ocv.me/pub/demo/)** 👀 running from a basement in finland
 
 📷 **screenshots:** [browser](#the-browser) // [upload](#uploading) // [unpost](#unpost) // [thumbnails](#thumbnails) // [search](#searching) // [fsearch](#file-search) // [zip-DL](#zip-downloads) // [md-viewer](#markdown-viewer)
 
 
 ## get the app
 
 <a href="https://f-droid.org/packages/me.ocv.partyup/"><img src="https://ocv.me/fdroid.png" alt="Get it on F-Droid" height="50" /> '' <img src="https://img.shields.io/f-droid/v/me.ocv.partyup.svg" alt="f-droid version info" /></a> '' <a href="https://github.com/9001/party-up"><img src="https://img.shields.io/github/release/9001/party-up.svg?logo=github" alt="github version info" /></a>
@@ -144,14 +144,15 @@
 
 ## quickstart
 
 just run **[copyparty-sfx.py](https://github.com/9001/copyparty/releases/latest/download/copyparty-sfx.py)** -- that's it! 🎉
 
 * or install through pypi (python3 only): `python3 -m pip install --user -U copyparty`
 * or if you cannot install python, you can use [copyparty.exe](#copypartyexe) instead
+* or if you are on android, [install copyparty in termux](#install-on-android)
 * or if you prefer to [use docker](./scripts/docker/) 🐋 you can do that too
   * docker has all deps built-in, so skip this step:
 
 enable thumbnails (images/audio/video), media indexing, and audio transcoding by installing some recommended deps:
 
 * **Alpine:** `apk add py3-pillow ffmpeg`
 * **Debian:** `apt install python3-pil ffmpeg`
@@ -201,19 +202,23 @@
   * ☑ volumes (mountpoints)
   * ☑ [accounts](#accounts-and-volumes)
   * ☑ [ftp server](#ftp-server)
   * ☑ [webdav server](#webdav-server)
   * ☑ [smb/cifs server](#smb-server)
   * ☑ [qr-code](#qr-code) for quick access
   * ☑ [upnp / zeroconf / mdns / ssdp](#zeroconf)
+  * ☑ [event hooks](#event-hooks) / script runner
+  * ☑ [reverse-proxy support](https://github.com/9001/copyparty#reverse-proxy)
 * upload
   * ☑ basic: plain multipart, ie6 support
   * ☑ [up2k](#uploading): js, resumable, multithreaded
     * unaffected by cloudflare's max-upload-size (100 MiB)
   * ☑ stash: simple PUT filedropper
+  * ☑ filename randomizer
+  * ☑ write-only folders
   * ☑ [unpost](#unpost): undo/delete accidental uploads
   * ☑ [self-destruct](#self-destruct) (specified server-side or client-side)
   * ☑ symlink/discard existing files (content-matching)
 * download
   * ☑ single files in browser
   * ☑ [folders as zip / tar files](#zip-downloads)
   * ☑ [FUSE client](https://github.com/9001/copyparty/tree/hovudstraum/bin#partyfusepy) (read-only)
@@ -229,18 +234,23 @@
     * ☑ ...of audio (spectrograms) using FFmpeg
     * ☑ cache eviction (max-age; maybe max-size eventually)
   * ☑ SPA (browse while uploading)
 * server indexing
   * ☑ [locate files by contents](#file-search)
   * ☑ search by name/path/date/size
   * ☑ [search by ID3-tags etc.](#searching)
+* client support
+  * ☑ [sync folder to server](https://github.com/9001/copyparty/tree/hovudstraum/bin#up2kpy)
+  * ☑ [curl-friendly](https://user-images.githubusercontent.com/241032/215322619-ea5fd606-3654-40ad-94ee-2bc058647bb2.png)
 * markdown
   * ☑ [viewer](#markdown-viewer)
   * ☑ editor (sure why not)
 
+PS: something missing? post any crazy ideas you've got as a [feature request](https://github.com/9001/copyparty/issues/new?assignees=9001&labels=enhancement&template=feature_request.md) or [discussion](https://github.com/9001/copyparty/discussions/new?category=ideas) 🤙
+
 
 ## testimonials
 
 small collection of user feedback
 
 `good enough`, `surprisingly correct`, `certified good software`, `just works`, `why`, `wow this is better than nextcloud`
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_cz2chf20_/tmp321ousi3_TarContainer/0/3", line 1476, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_cz2chf20_/tmp321ousi3_TarContainer/0/3", line 1476, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copyparty Version: 1.6.8 Summary: Portable file
+Metadata-Version: 2.1 Name: copyparty Version: 1.6.9 Summary: Portable file
 server with accelerated resumable uploads, deduplication, WebDAV, FTP,
 zeroconf, media indexer, video thumbnails, audio transcoding, and write-only
 folders Home-page: https://github.com/9001/copyparty Author: ed Author-email:
 copyparty@ocv.me License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
@@ -24,97 +24,98 @@
 Provides-Extra: ftpd Provides-Extra: ftps License-File: LICENSE # ð¾ð
 copyparty * portable file sharing hub (py2/py3) [(on PyPI)](https://pypi.org/
 project/copyparty/) * MIT-Licensed, 2019-05-26, ed @ irc.rizon.net ## summary
 turn your phone or raspi into a portable file server with resumable uploads/
 downloads using *any* web browser * server only needs Python (`2.7` or `3.3+`),
 all dependencies optional * browse/upload with [IE4](#browser-support) /
 netscape4.0 on win3.11 (heh) * protocols: [http](#the-browser) // [ftp](#ftp-
-server) // [webdav](#webdav-server) // [smb/cifs](#smb-server) try the **[read-
-only demo server](https://a.ocv.me/pub/demo/)** ð running from a basement in
-finland ð· **screenshots:** [browser](#the-browser) // [upload](#uploading) /
-/ [unpost](#unpost) // [thumbnails](#thumbnails) // [search](#searching) //
-[fsearch](#file-search) // [zip-DL](#zip-downloads) // [md-viewer](#markdown-
-viewer) ## get the app [Get_it_on_F-Droid]_''_[f-droid_version_info] '' [github
-version_info] (the app is **NOT** the full copyparty server! just a basic
-upload client, nothing fancy yet) ## readme toc * top * [quickstart]
-(#quickstart) - just run **[copyparty-sfx.py](https://github.com/9001/
-copyparty/releases/latest/download/copyparty-sfx.py)** -- that's it! ð * [on
-servers](#on-servers) - you may also want these, especially on servers *
-[features](#features) * [testimonials](#testimonials) - small collection of
-user feedback * [motivations](#motivations) - project goals / philosophy *
-[notes](#notes) - general notes * [bugs](#bugs) * [general bugs](#general-bugs)
-* [not my bugs](#not-my-bugs) * [breaking changes](#breaking-changes) - upgrade
-notes * [FAQ](#FAQ) - "frequently" asked questions * [accounts and volumes]
-(#accounts-and-volumes) - per-folder, per-user permissions * [shadowing]
-(#shadowing) - hiding specific subfolders * [the browser](#the-browser) -
-accessing a copyparty server using a web-browser * [tabs](#tabs) - the main
-tabs in the ui * [hotkeys](#hotkeys) - the browser has the following hotkeys *
-[navpane](#navpane) - switching between breadcrumbs or navpane * [thumbnails]
-(#thumbnails) - press `g` or `ç°` to toggle grid-view instead of the file
-listing * [zip downloads](#zip-downloads) - download folders (or file
-selections) as `zip` or `tar` files * [uploading](#uploading) - drag files/
-folders into the web-browser to upload * [file-search](#file-search) - dropping
-files into the browser also lets you see if they exist on the server * [unpost]
-(#unpost) - undo/delete accidental uploads * [self-destruct](#self-destruct) -
-uploads can be given a lifetime * [file manager](#file-manager) - cut/paste,
-rename, and delete files/folders (if you have permission) * [batch rename]
-(#batch-rename) - select some files and press `F2` to bring up the rename UI *
-[markdown viewer](#markdown-viewer) - and there are *two* editors * [other
-tricks](#other-tricks) * [searching](#searching) - search by size, date, path/
-name, mp3-tags, ... * [server config](#server-config) - using arguments or
-config files, or a mix of both * [zeroconf](#zeroconf) - announce enabled
-services on the LAN ([pic](https://user-images.githubusercontent.com/241032/
-215344737-0eae8d98-9496-4256-9aa8-cd2f6971810d.png)) * [mdns](#mdns) - LAN
-domain-name and feature announcer * [ssdp](#ssdp) - windows-explorer announcer
-* [qr-code](#qr-code) - print a qr-code [(screenshot)](https://user-
-images.githubusercontent.com/241032/194728533-6f00849b-c6ac-43c6-9359-
-83e454d11e00.png) for quick access * [ftp server](#ftp-server) - an FTP server
-can be started using `--ftp 3921` * [webdav server](#webdav-server) - with
-read-write support * [connecting to webdav from windows](#connecting-to-webdav-
-from-windows) - using the GUI * [smb server](#smb-server) - unsafe, slow, not
-recommended for wan * [file indexing](#file-indexing) - enables dedup and music
-search ++ * [exclude-patterns](#exclude-patterns) - to save some time *
-[filesystem guards](#filesystem-guards) - avoid traversing into other
-filesystems * [periodic rescan](#periodic-rescan) - filesystem monitoring *
-[upload rules](#upload-rules) - set upload rules using volflags * [compress
-uploads](#compress-uploads) - files can be autocompressed on upload * [other
-flags](#other-flags) * [database location](#database-location) - in-volume
-(`.hist/up2k.db`, default) or somewhere else * [metadata from audio files]
-(#metadata-from-audio-files) - set `-e2t` to index tags on upload * [file
-parser plugins](#file-parser-plugins) - provide custom parsers to index
-additional tags * [event hooks](#event-hooks) - trigger a program on uploads,
-renames etc ([examples](./bin/hooks/)) * [upload events](#upload-events) - the
-older, more powerful approach ([examples](./bin/mtag/)) * [hiding from google]
-(#hiding-from-google) - tell search engines you dont wanna be indexed *
-[themes](#themes) * [complete examples](#complete-examples) * [reverse-proxy]
-(#reverse-proxy) - running copyparty next to other websites * [browser support]
-(#browser-support) - TLDR: yes * [client examples](#client-examples) - interact
-with copyparty using non-browser clients * [mount as drive](#mount-as-drive) -
-a remote copyparty server as a local filesystem * [performance](#performance) -
-defaults are usually fine - expect `8 GiB/s` download, `1 GiB/s` upload *
-[client-side](#client-side) - when uploading files * [security](#security) -
-some notes on hardening * [gotchas](#gotchas) - behavior that might be
-unexpected * [cors](#cors) - cross-site request config * [recovering from
-crashes](#recovering-from-crashes) * [client crashes](#client-crashes) *
-[frefox wsod](#frefox-wsod) - firefox 87 can crash during uploads * [HTTP API]
-(#HTTP-API) - see [devnotes](#./docs/devnotes.md#http-api) * [dependencies]
-(#dependencies) - mandatory deps * [optional dependencies](#optional-
-dependencies) - install these to enable bonus features * [optional gpl stuff]
-(#optional-gpl-stuff) * [sfx](#sfx) - the self-contained "binary" *
+server) // [webdav](#webdav-server) // [smb/cifs](#smb-server) **[Get started]
+(#quickstart)!** or visit the **[read-only demo server](https://a.ocv.me/pub/
+demo/)** ð running from a basement in finland ð· **screenshots:**
+[browser](#the-browser) // [upload](#uploading) // [unpost](#unpost) //
+[thumbnails](#thumbnails) // [search](#searching) // [fsearch](#file-search) /
+/ [zip-DL](#zip-downloads) // [md-viewer](#markdown-viewer) ## get the app [Get
+it_on_F-Droid]_''_[f-droid_version_info] '' [github_version_info] (the app is
+**NOT** the full copyparty server! just a basic upload client, nothing fancy
+yet) ## readme toc * top * [quickstart](#quickstart) - just run **[copyparty-
+sfx.py](https://github.com/9001/copyparty/releases/latest/download/copyparty-
+sfx.py)** -- that's it! ð * [on servers](#on-servers) - you may also want
+these, especially on servers * [features](#features) * [testimonials]
+(#testimonials) - small collection of user feedback * [motivations]
+(#motivations) - project goals / philosophy * [notes](#notes) - general notes *
+[bugs](#bugs) * [general bugs](#general-bugs) * [not my bugs](#not-my-bugs) *
+[breaking changes](#breaking-changes) - upgrade notes * [FAQ](#FAQ) -
+"frequently" asked questions * [accounts and volumes](#accounts-and-volumes) -
+per-folder, per-user permissions * [shadowing](#shadowing) - hiding specific
+subfolders * [the browser](#the-browser) - accessing a copyparty server using a
+web-browser * [tabs](#tabs) - the main tabs in the ui * [hotkeys](#hotkeys) -
+the browser has the following hotkeys * [navpane](#navpane) - switching between
+breadcrumbs or navpane * [thumbnails](#thumbnails) - press `g` or `ç°` to
+toggle grid-view instead of the file listing * [zip downloads](#zip-downloads)
+- download folders (or file selections) as `zip` or `tar` files * [uploading]
+(#uploading) - drag files/folders into the web-browser to upload * [file-
+search](#file-search) - dropping files into the browser also lets you see if
+they exist on the server * [unpost](#unpost) - undo/delete accidental uploads *
+[self-destruct](#self-destruct) - uploads can be given a lifetime * [file
+manager](#file-manager) - cut/paste, rename, and delete files/folders (if you
+have permission) * [batch rename](#batch-rename) - select some files and press
+`F2` to bring up the rename UI * [markdown viewer](#markdown-viewer) - and
+there are *two* editors * [other tricks](#other-tricks) * [searching]
+(#searching) - search by size, date, path/name, mp3-tags, ... * [server config]
+(#server-config) - using arguments or config files, or a mix of both *
+[zeroconf](#zeroconf) - announce enabled services on the LAN ([pic](https://
+user-images.githubusercontent.com/241032/215344737-0eae8d98-9496-4256-9aa8-
+cd2f6971810d.png)) * [mdns](#mdns) - LAN domain-name and feature announcer *
+[ssdp](#ssdp) - windows-explorer announcer * [qr-code](#qr-code) - print a qr-
+code [(screenshot)](https://user-images.githubusercontent.com/241032/194728533-
+6f00849b-c6ac-43c6-9359-83e454d11e00.png) for quick access * [ftp server](#ftp-
+server) - an FTP server can be started using `--ftp 3921` * [webdav server]
+(#webdav-server) - with read-write support * [connecting to webdav from
+windows](#connecting-to-webdav-from-windows) - using the GUI * [smb server]
+(#smb-server) - unsafe, slow, not recommended for wan * [file indexing](#file-
+indexing) - enables dedup and music search ++ * [exclude-patterns](#exclude-
+patterns) - to save some time * [filesystem guards](#filesystem-guards) - avoid
+traversing into other filesystems * [periodic rescan](#periodic-rescan) -
+filesystem monitoring * [upload rules](#upload-rules) - set upload rules using
+volflags * [compress uploads](#compress-uploads) - files can be autocompressed
+on upload * [other flags](#other-flags) * [database location](#database-
+location) - in-volume (`.hist/up2k.db`, default) or somewhere else * [metadata
+from audio files](#metadata-from-audio-files) - set `-e2t` to index tags on
+upload * [file parser plugins](#file-parser-plugins) - provide custom parsers
+to index additional tags * [event hooks](#event-hooks) - trigger a program on
+uploads, renames etc ([examples](./bin/hooks/)) * [upload events](#upload-
+events) - the older, more powerful approach ([examples](./bin/mtag/)) * [hiding
+from google](#hiding-from-google) - tell search engines you dont wanna be
+indexed * [themes](#themes) * [complete examples](#complete-examples) *
+[reverse-proxy](#reverse-proxy) - running copyparty next to other websites *
+[browser support](#browser-support) - TLDR: yes * [client examples](#client-
+examples) - interact with copyparty using non-browser clients * [mount as
+drive](#mount-as-drive) - a remote copyparty server as a local filesystem *
+[performance](#performance) - defaults are usually fine - expect `8 GiB/s`
+download, `1 GiB/s` upload * [client-side](#client-side) - when uploading files
+* [security](#security) - some notes on hardening * [gotchas](#gotchas) -
+behavior that might be unexpected * [cors](#cors) - cross-site request config *
+[recovering from crashes](#recovering-from-crashes) * [client crashes](#client-
+crashes) * [frefox wsod](#frefox-wsod) - firefox 87 can crash during uploads *
+[HTTP API](#HTTP-API) - see [devnotes](#./docs/devnotes.md#http-api) *
+[dependencies](#dependencies) - mandatory deps * [optional dependencies]
+(#optional-dependencies) - install these to enable bonus features * [optional
+gpl stuff](#optional-gpl-stuff) * [sfx](#sfx) - the self-contained "binary" *
 [copyparty.exe](#copypartyexe) - download [copyparty.exe](https://github.com/
 9001/copyparty/releases/latest/download/copyparty.exe) (win8+) or
 [copyparty32.exe](https://github.com/9001/copyparty/releases/latest/download/
 copyparty32.exe) (win7+) * [install on android](#install-on-android) *
 [reporting bugs](#reporting-bugs) - ideas for context to include in bug reports
 * [devnotes](#devnotes) - for build instructions etc, see [./docs/devnotes.md]
 (./docs/devnotes.md) ## quickstart just run **[copyparty-sfx.py](https://
 github.com/9001/copyparty/releases/latest/download/copyparty-sfx.py)** -
 - that's it! ð * or install through pypi (python3 only): `python3 -m pip
 install --user -U copyparty` * or if you cannot install python, you can use
-[copyparty.exe](#copypartyexe) instead * or if you prefer to [use docker](./
+[copyparty.exe](#copypartyexe) instead * or if you are on android, [install
+copyparty in termux](#install-on-android) * or if you prefer to [use docker](./
 scripts/docker/) ð you can do that too * docker has all deps built-in, so
 skip this step: enable thumbnails (images/audio/video), media indexing, and
 audio transcoding by installing some recommended deps: * **Alpine:** `apk add
 py3-pillow ffmpeg` * **Debian:** `apt install python3-pil ffmpeg` * **Fedora:**
 `dnf install python3-pillow ffmpeg` * **FreeBSD:** `pkg install py39-sqlite3
 py39-pillow ffmpeg` * **MacOS:** `port install py-Pillow ffmpeg` * **MacOS**
 (alternative): `brew install pillow ffmpeg` * **Windows:** `python -m pip
@@ -144,54 +145,64 @@
 --zone=libvirt firewall-cmd --permanent --add-port={1900,5353}/udp # --
 zone=libvirt firewall-cmd --reload ``` (1900:ssdp, 3921:ftp, 3923:http/https,
 3945:smb, 3990:ftps, 5353:mdns, 12000:passive-ftp) ## features * backend stuff
 * â IPv6 * â [multiprocessing](#performance) (actual multithreading) * â
 volumes (mountpoints) * â [accounts](#accounts-and-volumes) * â [ftp
 server](#ftp-server) * â [webdav server](#webdav-server) * â [smb/cifs
 server](#smb-server) * â [qr-code](#qr-code) for quick access * â [upnp /
-zeroconf / mdns / ssdp](#zeroconf) * upload * â basic: plain multipart, ie6
-support * â [up2k](#uploading): js, resumable, multithreaded * unaffected by
-cloudflare's max-upload-size (100 MiB) * â stash: simple PUT filedropper *
-â [unpost](#unpost): undo/delete accidental uploads * â [self-destruct]
-(#self-destruct) (specified server-side or client-side) * â symlink/discard
-existing files (content-matching) * download * â single files in browser *
-â [folders as zip / tar files](#zip-downloads) * â [FUSE client](https://
-github.com/9001/copyparty/tree/hovudstraum/bin#partyfusepy) (read-only) *
-browser * â [navpane](#navpane) (directory tree sidebar) * â file manager
-(cut/paste, delete, [batch-rename](#batch-rename)) * â audio player (with [OS
-media controls](https://user-images.githubusercontent.com/241032/215347492-
-b4250797-6c90-4e09-9a4c-721edf2fb15c.png) and opus transcoding) * â image
-gallery with webm player * â textfile browser with syntax hilighting * â
-[thumbnails](#thumbnails) * â ...of images using Pillow, pyvips, or FFmpeg *
-â ...of videos using FFmpeg * â ...of audio (spectrograms) using FFmpeg *
-â cache eviction (max-age; maybe max-size eventually) * â SPA (browse while
-uploading) * server indexing * â [locate files by contents](#file-search) *
-â search by name/path/date/size * â [search by ID3-tags etc.](#searching) *
-markdown * â [viewer](#markdown-viewer) * â editor (sure why not) ##
-testimonials small collection of user feedback `good enough`, `surprisingly
-correct`, `certified good software`, `just works`, `why`, `wow this is better
-than nextcloud` # motivations project goals / philosophy * inverse linux
-philosophy -- do all the things, and do an *okay* job * quick drop-in service
-to get a lot of features in a pinch * some of [the alternatives](./docs/
-versus.md) might be a better fit for you * run anywhere, support everything *
-as many web-browsers and python versions as possible * every browser should at
-least be able to browse, download, upload files * be a good emergency solution
-for transferring stuff between ancient boxes * minimal dependencies * but
-optional dependencies adding bonus-features are ok * everything being plaintext
-makes it possible to proofread for malicious code * no preparations / setup
-necessary, just run the sfx (which is also plaintext) * adaptable, malleable,
-hackable * no build steps; modify the js/python without needing node.js or
-anything like that ## notes general notes: * paper-printing is affected by
-dark/light-mode! use lightmode for color, darkmode for grayscale * because no
-browsers currently implement the media-query to do this properly orz browser-
-specific: * iPhone/iPad: use Firefox to download files * Android-Chrome:
-increase "parallel uploads" for higher speed (android bug) * Android-Firefox:
-takes a while to select files (their fix for âï¸) * Desktop-Firefox: ~~may
-use gigabytes of RAM if your files are massive~~ *seems to be OK now* *
-Desktop-Firefox: [may stop you from unplugging USB flashdrives](https://
+zeroconf / mdns / ssdp](#zeroconf) * â [event hooks](#event-hooks) / script
+runner * â [reverse-proxy support](https://github.com/9001/copyparty#reverse-
+proxy) * upload * â basic: plain multipart, ie6 support * â [up2k]
+(#uploading): js, resumable, multithreaded * unaffected by cloudflare's max-
+upload-size (100 MiB) * â stash: simple PUT filedropper * â filename
+randomizer * â write-only folders * â [unpost](#unpost): undo/delete
+accidental uploads * â [self-destruct](#self-destruct) (specified server-side
+or client-side) * â symlink/discard existing files (content-matching) *
+download * â single files in browser * â [folders as zip / tar files](#zip-
+downloads) * â [FUSE client](https://github.com/9001/copyparty/tree/
+hovudstraum/bin#partyfusepy) (read-only) * browser * â [navpane](#navpane)
+(directory tree sidebar) * â file manager (cut/paste, delete, [batch-rename]
+(#batch-rename)) * â audio player (with [OS media controls](https://user-
+images.githubusercontent.com/241032/215347492-b4250797-6c90-4e09-9a4c-
+721edf2fb15c.png) and opus transcoding) * â image gallery with webm player *
+â textfile browser with syntax hilighting * â [thumbnails](#thumbnails) *
+â ...of images using Pillow, pyvips, or FFmpeg * â ...of videos using
+FFmpeg * â ...of audio (spectrograms) using FFmpeg * â cache eviction (max-
+age; maybe max-size eventually) * â SPA (browse while uploading) * server
+indexing * â [locate files by contents](#file-search) * â search by name/
+path/date/size * â [search by ID3-tags etc.](#searching) * client support *
+â [sync folder to server](https://github.com/9001/copyparty/tree/hovudstraum/
+bin#up2kpy) * â [curl-friendly](https://user-images.githubusercontent.com/
+241032/215322619-ea5fd606-3654-40ad-94ee-2bc058647bb2.png) * markdown * â
+[viewer](#markdown-viewer) * â editor (sure why not) PS: something missing?
+post any crazy ideas you've got as a [feature request](https://github.com/9001/
+copyparty/issues/
+new?assignees=9001&labels=enhancement&template=feature_request.md) or
+[discussion](https://github.com/9001/copyparty/discussions/new?category=ideas)
+ð¤ ## testimonials small collection of user feedback `good enough`,
+`surprisingly correct`, `certified good software`, `just works`, `why`, `wow
+this is better than nextcloud` # motivations project goals / philosophy *
+inverse linux philosophy -- do all the things, and do an *okay* job * quick
+drop-in service to get a lot of features in a pinch * some of [the
+alternatives](./docs/versus.md) might be a better fit for you * run anywhere,
+support everything * as many web-browsers and python versions as possible *
+every browser should at least be able to browse, download, upload files * be a
+good emergency solution for transferring stuff between ancient boxes * minimal
+dependencies * but optional dependencies adding bonus-features are ok *
+everything being plaintext makes it possible to proofread for malicious code *
+no preparations / setup necessary, just run the sfx (which is also plaintext) *
+adaptable, malleable, hackable * no build steps; modify the js/python without
+needing node.js or anything like that ## notes general notes: * paper-printing
+is affected by dark/light-mode! use lightmode for color, darkmode for grayscale
+* because no browsers currently implement the media-query to do this properly
+orz browser-specific: * iPhone/iPad: use Firefox to download files * Android-
+Chrome: increase "parallel uploads" for higher speed (android bug) * Android-
+Firefox: takes a while to select files (their fix for âï¸) * Desktop-
+Firefox: ~~may use gigabytes of RAM if your files are massive~~ *seems to be OK
+now* * Desktop-Firefox: [may stop you from unplugging USB flashdrives](https://
 bugzilla.mozilla.org/show_bug.cgi?id=1792598) until you visit `about:memory`
 and click `Minimize memory usage` server-os-specific: * RHEL8 / Rocky8: you can
 run copyparty using `/usr/libexec/platform-python` server notes: * pypy is
 supported but regular cpython is faster if you enable the database # bugs *
 Windows: python 2.7 cannot index non-ascii filenames with `-e2d` * Windows:
 python 2.7 cannot handle filenames with mojibake * `--th-ff-jpg` may fix video
 thumbnails on some FFmpeg versions (macos, some linux) * `--th-ff-swr` may fix
```

### Comparing `copyparty-1.6.8/README.md` & `copyparty-1.6.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 turn your phone or raspi into a portable file server with resumable uploads/downloads using *any* web browser
 
 * server only needs Python (`2.7` or `3.3+`), all dependencies optional
 * browse/upload with [IE4](#browser-support) / netscape4.0 on win3.11 (heh)
 * protocols: [http](#the-browser) // [ftp](#ftp-server) // [webdav](#webdav-server) // [smb/cifs](#smb-server)
 
-try the **[read-only demo server](https://a.ocv.me/pub/demo/)** 👀 running from a basement in finland
+**[Get started](#quickstart)!** or visit the **[read-only demo server](https://a.ocv.me/pub/demo/)** 👀 running from a basement in finland
 
 📷 **screenshots:** [browser](#the-browser) // [upload](#uploading) // [unpost](#unpost) // [thumbnails](#thumbnails) // [search](#searching) // [fsearch](#file-search) // [zip-DL](#zip-downloads) // [md-viewer](#markdown-viewer)
 
 
 ## get the app
 
 <a href="https://f-droid.org/packages/me.ocv.partyup/"><img src="https://ocv.me/fdroid.png" alt="Get it on F-Droid" height="50" /> '' <img src="https://img.shields.io/f-droid/v/me.ocv.partyup.svg" alt="f-droid version info" /></a> '' <a href="https://github.com/9001/party-up"><img src="https://img.shields.io/github/release/9001/party-up.svg?logo=github" alt="github version info" /></a>
@@ -104,14 +104,15 @@
 
 ## quickstart
 
 just run **[copyparty-sfx.py](https://github.com/9001/copyparty/releases/latest/download/copyparty-sfx.py)** -- that's it! 🎉
 
 * or install through pypi (python3 only): `python3 -m pip install --user -U copyparty`
 * or if you cannot install python, you can use [copyparty.exe](#copypartyexe) instead
+* or if you are on android, [install copyparty in termux](#install-on-android)
 * or if you prefer to [use docker](./scripts/docker/) 🐋 you can do that too
   * docker has all deps built-in, so skip this step:
 
 enable thumbnails (images/audio/video), media indexing, and audio transcoding by installing some recommended deps:
 
 * **Alpine:** `apk add py3-pillow ffmpeg`
 * **Debian:** `apt install python3-pil ffmpeg`
@@ -161,19 +162,23 @@
   * ☑ volumes (mountpoints)
   * ☑ [accounts](#accounts-and-volumes)
   * ☑ [ftp server](#ftp-server)
   * ☑ [webdav server](#webdav-server)
   * ☑ [smb/cifs server](#smb-server)
   * ☑ [qr-code](#qr-code) for quick access
   * ☑ [upnp / zeroconf / mdns / ssdp](#zeroconf)
+  * ☑ [event hooks](#event-hooks) / script runner
+  * ☑ [reverse-proxy support](https://github.com/9001/copyparty#reverse-proxy)
 * upload
   * ☑ basic: plain multipart, ie6 support
   * ☑ [up2k](#uploading): js, resumable, multithreaded
     * unaffected by cloudflare's max-upload-size (100 MiB)
   * ☑ stash: simple PUT filedropper
+  * ☑ filename randomizer
+  * ☑ write-only folders
   * ☑ [unpost](#unpost): undo/delete accidental uploads
   * ☑ [self-destruct](#self-destruct) (specified server-side or client-side)
   * ☑ symlink/discard existing files (content-matching)
 * download
   * ☑ single files in browser
   * ☑ [folders as zip / tar files](#zip-downloads)
   * ☑ [FUSE client](https://github.com/9001/copyparty/tree/hovudstraum/bin#partyfusepy) (read-only)
@@ -189,18 +194,23 @@
     * ☑ ...of audio (spectrograms) using FFmpeg
     * ☑ cache eviction (max-age; maybe max-size eventually)
   * ☑ SPA (browse while uploading)
 * server indexing
   * ☑ [locate files by contents](#file-search)
   * ☑ search by name/path/date/size
   * ☑ [search by ID3-tags etc.](#searching)
+* client support
+  * ☑ [sync folder to server](https://github.com/9001/copyparty/tree/hovudstraum/bin#up2kpy)
+  * ☑ [curl-friendly](https://user-images.githubusercontent.com/241032/215322619-ea5fd606-3654-40ad-94ee-2bc058647bb2.png)
 * markdown
   * ☑ [viewer](#markdown-viewer)
   * ☑ editor (sure why not)
 
+PS: something missing? post any crazy ideas you've got as a [feature request](https://github.com/9001/copyparty/issues/new?assignees=9001&labels=enhancement&template=feature_request.md) or [discussion](https://github.com/9001/copyparty/discussions/new?category=ideas) 🤙
+
 
 ## testimonials
 
 small collection of user feedback
 
 `good enough`, `surprisingly correct`, `certified good software`, `just works`, `why`, `wow this is better than nextcloud`
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_cz2chf20_/tmp321ousi3_TarContainer/0/4.md", line 1436, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_cz2chf20_/tmp321ousi3_TarContainer/0/4.md", line 1436, column 0: CDATA terminal not found*

```diff
@@ -1,96 +1,97 @@
 # ð¾ð copyparty * portable file sharing hub (py2/py3) [(on PyPI)](https://
 pypi.org/project/copyparty/) * MIT-Licensed, 2019-05-26, ed @ irc.rizon.net ##
 summary turn your phone or raspi into a portable file server with resumable
 uploads/downloads using *any* web browser * server only needs Python (`2.7` or
 `3.3+`), all dependencies optional * browse/upload with [IE4](#browser-support)
 / netscape4.0 on win3.11 (heh) * protocols: [http](#the-browser) // [ftp](#ftp-
-server) // [webdav](#webdav-server) // [smb/cifs](#smb-server) try the **[read-
-only demo server](https://a.ocv.me/pub/demo/)** ð running from a basement in
-finland ð· **screenshots:** [browser](#the-browser) // [upload](#uploading) /
-/ [unpost](#unpost) // [thumbnails](#thumbnails) // [search](#searching) //
-[fsearch](#file-search) // [zip-DL](#zip-downloads) // [md-viewer](#markdown-
-viewer) ## get the app [Get_it_on_F-Droid]_''_[f-droid_version_info] '' [github
-version_info] (the app is **NOT** the full copyparty server! just a basic
-upload client, nothing fancy yet) ## readme toc * top * [quickstart]
-(#quickstart) - just run **[copyparty-sfx.py](https://github.com/9001/
-copyparty/releases/latest/download/copyparty-sfx.py)** -- that's it! ð * [on
-servers](#on-servers) - you may also want these, especially on servers *
-[features](#features) * [testimonials](#testimonials) - small collection of
-user feedback * [motivations](#motivations) - project goals / philosophy *
-[notes](#notes) - general notes * [bugs](#bugs) * [general bugs](#general-bugs)
-* [not my bugs](#not-my-bugs) * [breaking changes](#breaking-changes) - upgrade
-notes * [FAQ](#FAQ) - "frequently" asked questions * [accounts and volumes]
-(#accounts-and-volumes) - per-folder, per-user permissions * [shadowing]
-(#shadowing) - hiding specific subfolders * [the browser](#the-browser) -
-accessing a copyparty server using a web-browser * [tabs](#tabs) - the main
-tabs in the ui * [hotkeys](#hotkeys) - the browser has the following hotkeys *
-[navpane](#navpane) - switching between breadcrumbs or navpane * [thumbnails]
-(#thumbnails) - press `g` or `ç°` to toggle grid-view instead of the file
-listing * [zip downloads](#zip-downloads) - download folders (or file
-selections) as `zip` or `tar` files * [uploading](#uploading) - drag files/
-folders into the web-browser to upload * [file-search](#file-search) - dropping
-files into the browser also lets you see if they exist on the server * [unpost]
-(#unpost) - undo/delete accidental uploads * [self-destruct](#self-destruct) -
-uploads can be given a lifetime * [file manager](#file-manager) - cut/paste,
-rename, and delete files/folders (if you have permission) * [batch rename]
-(#batch-rename) - select some files and press `F2` to bring up the rename UI *
-[markdown viewer](#markdown-viewer) - and there are *two* editors * [other
-tricks](#other-tricks) * [searching](#searching) - search by size, date, path/
-name, mp3-tags, ... * [server config](#server-config) - using arguments or
-config files, or a mix of both * [zeroconf](#zeroconf) - announce enabled
-services on the LAN ([pic](https://user-images.githubusercontent.com/241032/
-215344737-0eae8d98-9496-4256-9aa8-cd2f6971810d.png)) * [mdns](#mdns) - LAN
-domain-name and feature announcer * [ssdp](#ssdp) - windows-explorer announcer
-* [qr-code](#qr-code) - print a qr-code [(screenshot)](https://user-
-images.githubusercontent.com/241032/194728533-6f00849b-c6ac-43c6-9359-
-83e454d11e00.png) for quick access * [ftp server](#ftp-server) - an FTP server
-can be started using `--ftp 3921` * [webdav server](#webdav-server) - with
-read-write support * [connecting to webdav from windows](#connecting-to-webdav-
-from-windows) - using the GUI * [smb server](#smb-server) - unsafe, slow, not
-recommended for wan * [file indexing](#file-indexing) - enables dedup and music
-search ++ * [exclude-patterns](#exclude-patterns) - to save some time *
-[filesystem guards](#filesystem-guards) - avoid traversing into other
-filesystems * [periodic rescan](#periodic-rescan) - filesystem monitoring *
-[upload rules](#upload-rules) - set upload rules using volflags * [compress
-uploads](#compress-uploads) - files can be autocompressed on upload * [other
-flags](#other-flags) * [database location](#database-location) - in-volume
-(`.hist/up2k.db`, default) or somewhere else * [metadata from audio files]
-(#metadata-from-audio-files) - set `-e2t` to index tags on upload * [file
-parser plugins](#file-parser-plugins) - provide custom parsers to index
-additional tags * [event hooks](#event-hooks) - trigger a program on uploads,
-renames etc ([examples](./bin/hooks/)) * [upload events](#upload-events) - the
-older, more powerful approach ([examples](./bin/mtag/)) * [hiding from google]
-(#hiding-from-google) - tell search engines you dont wanna be indexed *
-[themes](#themes) * [complete examples](#complete-examples) * [reverse-proxy]
-(#reverse-proxy) - running copyparty next to other websites * [browser support]
-(#browser-support) - TLDR: yes * [client examples](#client-examples) - interact
-with copyparty using non-browser clients * [mount as drive](#mount-as-drive) -
-a remote copyparty server as a local filesystem * [performance](#performance) -
-defaults are usually fine - expect `8 GiB/s` download, `1 GiB/s` upload *
-[client-side](#client-side) - when uploading files * [security](#security) -
-some notes on hardening * [gotchas](#gotchas) - behavior that might be
-unexpected * [cors](#cors) - cross-site request config * [recovering from
-crashes](#recovering-from-crashes) * [client crashes](#client-crashes) *
-[frefox wsod](#frefox-wsod) - firefox 87 can crash during uploads * [HTTP API]
-(#HTTP-API) - see [devnotes](#./docs/devnotes.md#http-api) * [dependencies]
-(#dependencies) - mandatory deps * [optional dependencies](#optional-
-dependencies) - install these to enable bonus features * [optional gpl stuff]
-(#optional-gpl-stuff) * [sfx](#sfx) - the self-contained "binary" *
+server) // [webdav](#webdav-server) // [smb/cifs](#smb-server) **[Get started]
+(#quickstart)!** or visit the **[read-only demo server](https://a.ocv.me/pub/
+demo/)** ð running from a basement in finland ð· **screenshots:**
+[browser](#the-browser) // [upload](#uploading) // [unpost](#unpost) //
+[thumbnails](#thumbnails) // [search](#searching) // [fsearch](#file-search) /
+/ [zip-DL](#zip-downloads) // [md-viewer](#markdown-viewer) ## get the app [Get
+it_on_F-Droid]_''_[f-droid_version_info] '' [github_version_info] (the app is
+**NOT** the full copyparty server! just a basic upload client, nothing fancy
+yet) ## readme toc * top * [quickstart](#quickstart) - just run **[copyparty-
+sfx.py](https://github.com/9001/copyparty/releases/latest/download/copyparty-
+sfx.py)** -- that's it! ð * [on servers](#on-servers) - you may also want
+these, especially on servers * [features](#features) * [testimonials]
+(#testimonials) - small collection of user feedback * [motivations]
+(#motivations) - project goals / philosophy * [notes](#notes) - general notes *
+[bugs](#bugs) * [general bugs](#general-bugs) * [not my bugs](#not-my-bugs) *
+[breaking changes](#breaking-changes) - upgrade notes * [FAQ](#FAQ) -
+"frequently" asked questions * [accounts and volumes](#accounts-and-volumes) -
+per-folder, per-user permissions * [shadowing](#shadowing) - hiding specific
+subfolders * [the browser](#the-browser) - accessing a copyparty server using a
+web-browser * [tabs](#tabs) - the main tabs in the ui * [hotkeys](#hotkeys) -
+the browser has the following hotkeys * [navpane](#navpane) - switching between
+breadcrumbs or navpane * [thumbnails](#thumbnails) - press `g` or `ç°` to
+toggle grid-view instead of the file listing * [zip downloads](#zip-downloads)
+- download folders (or file selections) as `zip` or `tar` files * [uploading]
+(#uploading) - drag files/folders into the web-browser to upload * [file-
+search](#file-search) - dropping files into the browser also lets you see if
+they exist on the server * [unpost](#unpost) - undo/delete accidental uploads *
+[self-destruct](#self-destruct) - uploads can be given a lifetime * [file
+manager](#file-manager) - cut/paste, rename, and delete files/folders (if you
+have permission) * [batch rename](#batch-rename) - select some files and press
+`F2` to bring up the rename UI * [markdown viewer](#markdown-viewer) - and
+there are *two* editors * [other tricks](#other-tricks) * [searching]
+(#searching) - search by size, date, path/name, mp3-tags, ... * [server config]
+(#server-config) - using arguments or config files, or a mix of both *
+[zeroconf](#zeroconf) - announce enabled services on the LAN ([pic](https://
+user-images.githubusercontent.com/241032/215344737-0eae8d98-9496-4256-9aa8-
+cd2f6971810d.png)) * [mdns](#mdns) - LAN domain-name and feature announcer *
+[ssdp](#ssdp) - windows-explorer announcer * [qr-code](#qr-code) - print a qr-
+code [(screenshot)](https://user-images.githubusercontent.com/241032/194728533-
+6f00849b-c6ac-43c6-9359-83e454d11e00.png) for quick access * [ftp server](#ftp-
+server) - an FTP server can be started using `--ftp 3921` * [webdav server]
+(#webdav-server) - with read-write support * [connecting to webdav from
+windows](#connecting-to-webdav-from-windows) - using the GUI * [smb server]
+(#smb-server) - unsafe, slow, not recommended for wan * [file indexing](#file-
+indexing) - enables dedup and music search ++ * [exclude-patterns](#exclude-
+patterns) - to save some time * [filesystem guards](#filesystem-guards) - avoid
+traversing into other filesystems * [periodic rescan](#periodic-rescan) -
+filesystem monitoring * [upload rules](#upload-rules) - set upload rules using
+volflags * [compress uploads](#compress-uploads) - files can be autocompressed
+on upload * [other flags](#other-flags) * [database location](#database-
+location) - in-volume (`.hist/up2k.db`, default) or somewhere else * [metadata
+from audio files](#metadata-from-audio-files) - set `-e2t` to index tags on
+upload * [file parser plugins](#file-parser-plugins) - provide custom parsers
+to index additional tags * [event hooks](#event-hooks) - trigger a program on
+uploads, renames etc ([examples](./bin/hooks/)) * [upload events](#upload-
+events) - the older, more powerful approach ([examples](./bin/mtag/)) * [hiding
+from google](#hiding-from-google) - tell search engines you dont wanna be
+indexed * [themes](#themes) * [complete examples](#complete-examples) *
+[reverse-proxy](#reverse-proxy) - running copyparty next to other websites *
+[browser support](#browser-support) - TLDR: yes * [client examples](#client-
+examples) - interact with copyparty using non-browser clients * [mount as
+drive](#mount-as-drive) - a remote copyparty server as a local filesystem *
+[performance](#performance) - defaults are usually fine - expect `8 GiB/s`
+download, `1 GiB/s` upload * [client-side](#client-side) - when uploading files
+* [security](#security) - some notes on hardening * [gotchas](#gotchas) -
+behavior that might be unexpected * [cors](#cors) - cross-site request config *
+[recovering from crashes](#recovering-from-crashes) * [client crashes](#client-
+crashes) * [frefox wsod](#frefox-wsod) - firefox 87 can crash during uploads *
+[HTTP API](#HTTP-API) - see [devnotes](#./docs/devnotes.md#http-api) *
+[dependencies](#dependencies) - mandatory deps * [optional dependencies]
+(#optional-dependencies) - install these to enable bonus features * [optional
+gpl stuff](#optional-gpl-stuff) * [sfx](#sfx) - the self-contained "binary" *
 [copyparty.exe](#copypartyexe) - download [copyparty.exe](https://github.com/
 9001/copyparty/releases/latest/download/copyparty.exe) (win8+) or
 [copyparty32.exe](https://github.com/9001/copyparty/releases/latest/download/
 copyparty32.exe) (win7+) * [install on android](#install-on-android) *
 [reporting bugs](#reporting-bugs) - ideas for context to include in bug reports
 * [devnotes](#devnotes) - for build instructions etc, see [./docs/devnotes.md]
 (./docs/devnotes.md) ## quickstart just run **[copyparty-sfx.py](https://
 github.com/9001/copyparty/releases/latest/download/copyparty-sfx.py)** -
 - that's it! ð * or install through pypi (python3 only): `python3 -m pip
 install --user -U copyparty` * or if you cannot install python, you can use
-[copyparty.exe](#copypartyexe) instead * or if you prefer to [use docker](./
+[copyparty.exe](#copypartyexe) instead * or if you are on android, [install
+copyparty in termux](#install-on-android) * or if you prefer to [use docker](./
 scripts/docker/) ð you can do that too * docker has all deps built-in, so
 skip this step: enable thumbnails (images/audio/video), media indexing, and
 audio transcoding by installing some recommended deps: * **Alpine:** `apk add
 py3-pillow ffmpeg` * **Debian:** `apt install python3-pil ffmpeg` * **Fedora:**
 `dnf install python3-pillow ffmpeg` * **FreeBSD:** `pkg install py39-sqlite3
 py39-pillow ffmpeg` * **MacOS:** `port install py-Pillow ffmpeg` * **MacOS**
 (alternative): `brew install pillow ffmpeg` * **Windows:** `python -m pip
@@ -120,54 +121,64 @@
 --zone=libvirt firewall-cmd --permanent --add-port={1900,5353}/udp # --
 zone=libvirt firewall-cmd --reload ``` (1900:ssdp, 3921:ftp, 3923:http/https,
 3945:smb, 3990:ftps, 5353:mdns, 12000:passive-ftp) ## features * backend stuff
 * â IPv6 * â [multiprocessing](#performance) (actual multithreading) * â
 volumes (mountpoints) * â [accounts](#accounts-and-volumes) * â [ftp
 server](#ftp-server) * â [webdav server](#webdav-server) * â [smb/cifs
 server](#smb-server) * â [qr-code](#qr-code) for quick access * â [upnp /
-zeroconf / mdns / ssdp](#zeroconf) * upload * â basic: plain multipart, ie6
-support * â [up2k](#uploading): js, resumable, multithreaded * unaffected by
-cloudflare's max-upload-size (100 MiB) * â stash: simple PUT filedropper *
-â [unpost](#unpost): undo/delete accidental uploads * â [self-destruct]
-(#self-destruct) (specified server-side or client-side) * â symlink/discard
-existing files (content-matching) * download * â single files in browser *
-â [folders as zip / tar files](#zip-downloads) * â [FUSE client](https://
-github.com/9001/copyparty/tree/hovudstraum/bin#partyfusepy) (read-only) *
-browser * â [navpane](#navpane) (directory tree sidebar) * â file manager
-(cut/paste, delete, [batch-rename](#batch-rename)) * â audio player (with [OS
-media controls](https://user-images.githubusercontent.com/241032/215347492-
-b4250797-6c90-4e09-9a4c-721edf2fb15c.png) and opus transcoding) * â image
-gallery with webm player * â textfile browser with syntax hilighting * â
-[thumbnails](#thumbnails) * â ...of images using Pillow, pyvips, or FFmpeg *
-â ...of videos using FFmpeg * â ...of audio (spectrograms) using FFmpeg *
-â cache eviction (max-age; maybe max-size eventually) * â SPA (browse while
-uploading) * server indexing * â [locate files by contents](#file-search) *
-â search by name/path/date/size * â [search by ID3-tags etc.](#searching) *
-markdown * â [viewer](#markdown-viewer) * â editor (sure why not) ##
-testimonials small collection of user feedback `good enough`, `surprisingly
-correct`, `certified good software`, `just works`, `why`, `wow this is better
-than nextcloud` # motivations project goals / philosophy * inverse linux
-philosophy -- do all the things, and do an *okay* job * quick drop-in service
-to get a lot of features in a pinch * some of [the alternatives](./docs/
-versus.md) might be a better fit for you * run anywhere, support everything *
-as many web-browsers and python versions as possible * every browser should at
-least be able to browse, download, upload files * be a good emergency solution
-for transferring stuff between ancient boxes * minimal dependencies * but
-optional dependencies adding bonus-features are ok * everything being plaintext
-makes it possible to proofread for malicious code * no preparations / setup
-necessary, just run the sfx (which is also plaintext) * adaptable, malleable,
-hackable * no build steps; modify the js/python without needing node.js or
-anything like that ## notes general notes: * paper-printing is affected by
-dark/light-mode! use lightmode for color, darkmode for grayscale * because no
-browsers currently implement the media-query to do this properly orz browser-
-specific: * iPhone/iPad: use Firefox to download files * Android-Chrome:
-increase "parallel uploads" for higher speed (android bug) * Android-Firefox:
-takes a while to select files (their fix for âï¸) * Desktop-Firefox: ~~may
-use gigabytes of RAM if your files are massive~~ *seems to be OK now* *
-Desktop-Firefox: [may stop you from unplugging USB flashdrives](https://
+zeroconf / mdns / ssdp](#zeroconf) * â [event hooks](#event-hooks) / script
+runner * â [reverse-proxy support](https://github.com/9001/copyparty#reverse-
+proxy) * upload * â basic: plain multipart, ie6 support * â [up2k]
+(#uploading): js, resumable, multithreaded * unaffected by cloudflare's max-
+upload-size (100 MiB) * â stash: simple PUT filedropper * â filename
+randomizer * â write-only folders * â [unpost](#unpost): undo/delete
+accidental uploads * â [self-destruct](#self-destruct) (specified server-side
+or client-side) * â symlink/discard existing files (content-matching) *
+download * â single files in browser * â [folders as zip / tar files](#zip-
+downloads) * â [FUSE client](https://github.com/9001/copyparty/tree/
+hovudstraum/bin#partyfusepy) (read-only) * browser * â [navpane](#navpane)
+(directory tree sidebar) * â file manager (cut/paste, delete, [batch-rename]
+(#batch-rename)) * â audio player (with [OS media controls](https://user-
+images.githubusercontent.com/241032/215347492-b4250797-6c90-4e09-9a4c-
+721edf2fb15c.png) and opus transcoding) * â image gallery with webm player *
+â textfile browser with syntax hilighting * â [thumbnails](#thumbnails) *
+â ...of images using Pillow, pyvips, or FFmpeg * â ...of videos using
+FFmpeg * â ...of audio (spectrograms) using FFmpeg * â cache eviction (max-
+age; maybe max-size eventually) * â SPA (browse while uploading) * server
+indexing * â [locate files by contents](#file-search) * â search by name/
+path/date/size * â [search by ID3-tags etc.](#searching) * client support *
+â [sync folder to server](https://github.com/9001/copyparty/tree/hovudstraum/
+bin#up2kpy) * â [curl-friendly](https://user-images.githubusercontent.com/
+241032/215322619-ea5fd606-3654-40ad-94ee-2bc058647bb2.png) * markdown * â
+[viewer](#markdown-viewer) * â editor (sure why not) PS: something missing?
+post any crazy ideas you've got as a [feature request](https://github.com/9001/
+copyparty/issues/
+new?assignees=9001&labels=enhancement&template=feature_request.md) or
+[discussion](https://github.com/9001/copyparty/discussions/new?category=ideas)
+ð¤ ## testimonials small collection of user feedback `good enough`,
+`surprisingly correct`, `certified good software`, `just works`, `why`, `wow
+this is better than nextcloud` # motivations project goals / philosophy *
+inverse linux philosophy -- do all the things, and do an *okay* job * quick
+drop-in service to get a lot of features in a pinch * some of [the
+alternatives](./docs/versus.md) might be a better fit for you * run anywhere,
+support everything * as many web-browsers and python versions as possible *
+every browser should at least be able to browse, download, upload files * be a
+good emergency solution for transferring stuff between ancient boxes * minimal
+dependencies * but optional dependencies adding bonus-features are ok *
+everything being plaintext makes it possible to proofread for malicious code *
+no preparations / setup necessary, just run the sfx (which is also plaintext) *
+adaptable, malleable, hackable * no build steps; modify the js/python without
+needing node.js or anything like that ## notes general notes: * paper-printing
+is affected by dark/light-mode! use lightmode for color, darkmode for grayscale
+* because no browsers currently implement the media-query to do this properly
+orz browser-specific: * iPhone/iPad: use Firefox to download files * Android-
+Chrome: increase "parallel uploads" for higher speed (android bug) * Android-
+Firefox: takes a while to select files (their fix for âï¸) * Desktop-
+Firefox: ~~may use gigabytes of RAM if your files are massive~~ *seems to be OK
+now* * Desktop-Firefox: [may stop you from unplugging USB flashdrives](https://
 bugzilla.mozilla.org/show_bug.cgi?id=1792598) until you visit `about:memory`
 and click `Minimize memory usage` server-os-specific: * RHEL8 / Rocky8: you can
 run copyparty using `/usr/libexec/platform-python` server notes: * pypy is
 supported but regular cpython is faster if you enable the database # bugs *
 Windows: python 2.7 cannot index non-ascii filenames with `-e2d` * Windows:
 python 2.7 cannot handle filenames with mojibake * `--th-ff-jpg` may fix video
 thumbnails on some FFmpeg versions (macos, some linux) * `--th-ff-swr` may fix
```

### Comparing `copyparty-1.6.8/bin/partyfuse.py` & `copyparty-1.6.9/bin/partyfuse.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/bin/up2k.py` & `copyparty-1.6.9/bin/up2k.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/__init__.py` & `copyparty-1.6.9/copyparty/__init__.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/__main__.py` & `copyparty-1.6.9/copyparty/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -936,14 +936,15 @@
     ap2.add_argument("--theme", metavar="NUM", type=int, default=0, help="default theme to use")
     ap2.add_argument("--themes", metavar="NUM", type=int, default=8, help="number of themes installed")
     ap2.add_argument("--favico", metavar="TXT", type=u, default="c 000 none" if retry else "🎉 000 none", help="\033[33mfavicon-text\033[0m [ \033[33mforeground\033[0m [ \033[33mbackground\033[0m ] ], set blank to disable")
     ap2.add_argument("--mpmc", metavar="URL", type=u, default="", help="change the mediaplayer-toggle mouse cursor; URL to a folder with {2..5}.png inside (or disable with [\033[32m.\033[0m])")
     ap2.add_argument("--js-browser", metavar="L", type=u, help="URL to additional JS to include")
     ap2.add_argument("--css-browser", metavar="L", type=u, help="URL to additional CSS to include")
     ap2.add_argument("--html-head", metavar="TXT", type=u, default="", help="text to append to the <head> of all HTML pages")
+    ap2.add_argument("--ih", action="store_true", help="if a folder contains index.html, show that instead of the directory listing by default (can be changed in the client settings UI)")
     ap2.add_argument("--textfiles", metavar="CSV", type=u, default="txt,nfo,diz,cue,readme", help="file extensions to present as plaintext")
     ap2.add_argument("--txt-max", metavar="KiB", type=int, default=64, help="max size of embedded textfiles on ?doc= (anything bigger will be lazy-loaded by JS)")
     ap2.add_argument("--doctitle", metavar="TXT", type=u, default="copyparty", help="title / service-name to show in html documents")
     ap2.add_argument("--pb-url", metavar="URL", type=u, default="https://github.com/9001/copyparty", help="powered-by link; disable with -np")
     ap2.add_argument("--ver", action="store_true", help="show version on the control panel (incompatible by -np)")
     ap2.add_argument("--md-sbf", metavar="FLAGS", type=u, default="downloads forms popups scripts top-navigation-by-user-activation", help="list of capabilities to ALLOW for README.md docs (volflag=md_sbf); see https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe#attr-sandbox")
     ap2.add_argument("--lg-sbf", metavar="FLAGS", type=u, default="downloads forms popups scripts top-navigation-by-user-activation", help="list of capabilities to ALLOW for prologue/epilogue docs  (volflag=lg_sbf)")
```

### Comparing `copyparty-1.6.8/copyparty/authsrv.py` & `copyparty-1.6.9/copyparty/authsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/bos/bos.py` & `copyparty-1.6.9/copyparty/bos/bos.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/bos/path.py` & `copyparty-1.6.9/copyparty/bos/path.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/broker_mp.py` & `copyparty-1.6.9/copyparty/broker_mp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/broker_mpw.py` & `copyparty-1.6.9/copyparty/broker_mpw.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/broker_thr.py` & `copyparty-1.6.9/copyparty/broker_thr.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/broker_util.py` & `copyparty-1.6.9/copyparty/broker_util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/cfg.py` & `copyparty-1.6.9/copyparty/cfg.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/dxml.py` & `copyparty-1.6.9/copyparty/dxml.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/fsutil.py` & `copyparty-1.6.9/copyparty/fsutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/ftpd.py` & `copyparty-1.6.9/copyparty/ftpd.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,15 @@
         self.can_delete = self.can_get = self.can_upget = False
 
         self.listdirinfo = self.listdir
         self.chdir(".")
 
     def die(self, msg):
         self.h.die(msg)
+        raise Exception()
 
     def v2a(
         self,
         vpath ,
         r  = False,
         w  = False,
         m  = False,
```

### Comparing `copyparty-1.6.8/copyparty/httpcli.py` & `copyparty-1.6.9/copyparty/httpcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1530,5920 +1530,5964 @@
 00005f90: 2020 2072 6574 7572 6e20 7365 6c66 2e74     return self.t
 00005fa0: 785f 7570 7328 290a 0a20 2020 2020 2020  x_ups()..       
 00005fb0: 2020 2020 2069 6620 226b 3330 3422 2069       if "k304" i
 00005fc0: 6e20 7365 6c66 2e75 7061 7261 6d3a 0a20  n self.uparam:. 
 00005fd0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
 00005fe0: 6574 7572 6e20 7365 6c66 2e73 6574 5f6b  eturn self.set_k
 00005ff0: 3330 3428 290a 0a20 2020 2020 2020 2020  304()..         
-00006000: 2020 2069 6620 2261 6d5f 6a73 2220 696e     if "am_js" in
+00006000: 2020 2069 6620 2273 6574 636b 2220 696e     if "setck" in
 00006010: 2073 656c 662e 7570 6172 616d 3a0a 2020   self.uparam:.  
 00006020: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00006030: 7475 726e 2073 656c 662e 7365 745f 616d  turn self.set_am
-00006040: 5f6a 7328 290a 0a20 2020 2020 2020 2020  _js()..         
-00006050: 2020 2069 6620 2272 6573 6574 2220 696e     if "reset" in
-00006060: 2073 656c 662e 7570 6172 616d 3a0a 2020   self.uparam:.  
-00006070: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00006080: 7475 726e 2073 656c 662e 7365 745f 6366  turn self.set_cf
-00006090: 675f 7265 7365 7428 290a 0a20 2020 2020  g_reset()..     
-000060a0: 2020 2020 2020 2069 6620 2268 6322 2069         if "hc" i
-000060b0: 6e20 7365 6c66 2e75 7061 7261 6d3a 0a20  n self.uparam:. 
-000060c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000060d0: 6574 7572 6e20 7365 6c66 2e74 785f 7376  eturn self.tx_sv
-000060e0: 6373 2829 0a0a 2020 2020 2020 2020 6966  cs()..        if
-000060f0: 2022 6822 2069 6e20 7365 6c66 2e75 7061   "h" in self.upa
-00006100: 7261 6d3a 0a20 2020 2020 2020 2020 2020  ram:.           
-00006110: 2072 6574 7572 6e20 7365 6c66 2e74 785f   return self.tx_
-00006120: 6d6f 756e 7473 2829 0a0a 2020 2020 2020  mounts()..      
-00006130: 2020 2320 636f 6e64 6974 696f 6e61 6c20    # conditional 
-00006140: 7265 6469 7265 6374 2074 6f20 7369 6e67  redirect to sing
-00006150: 6c65 2076 6f6c 756d 6573 0a20 2020 2020  le volumes.     
-00006160: 2020 2069 6620 7365 6c66 2e76 7061 7468     if self.vpath
-00006170: 203d 3d20 2222 2061 6e64 206e 6f74 2073   == "" and not s
-00006180: 656c 662e 6f75 7061 7261 6d3a 0a20 2020  elf.ouparam:.   
-00006190: 2020 2020 2020 2020 206e 7265 6164 203d           nread =
-000061a0: 206c 656e 2873 656c 662e 7276 6f6c 290a   len(self.rvol).
-000061b0: 2020 2020 2020 2020 2020 2020 6e77 7269              nwri
-000061c0: 7465 203d 206c 656e 2873 656c 662e 7776  te = len(self.wv
-000061d0: 6f6c 290a 2020 2020 2020 2020 2020 2020  ol).            
-000061e0: 6966 206e 7265 6164 202b 206e 7772 6974  if nread + nwrit
-000061f0: 6520 3d3d 2031 206f 7220 2873 656c 662e  e == 1 or (self.
-00006200: 7276 6f6c 203d 3d20 7365 6c66 2e77 766f  rvol == self.wvo
-00006210: 6c20 616e 6420 6e72 6561 6420 3d3d 2031  l and nread == 1
-00006220: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00006230: 2020 2069 6620 6e72 6561 6420 3d3d 2031     if nread == 1
-00006240: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006250: 2020 2020 2020 7670 6174 6820 3d20 7365        vpath = se
-00006260: 6c66 2e72 766f 6c5b 305d 0a20 2020 2020  lf.rvol[0].     
-00006270: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00006280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006290: 2020 2020 2076 7061 7468 203d 2073 656c       vpath = sel
-000062a0: 662e 7776 6f6c 5b30 5d0a 0a20 2020 2020  f.wvol[0]..     
-000062b0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000062c0: 6c66 2e76 7061 7468 2021 3d20 7670 6174  lf.vpath != vpat
-000062d0: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
-000062e0: 2020 2020 2020 2073 656c 662e 7265 6469         self.redi
-000062f0: 7265 6374 2876 7061 7468 2c20 666c 6176  rect(vpath, flav
-00006300: 6f72 3d22 7265 6469 7265 6374 696e 6720  or="redirecting 
-00006310: 746f 222c 2075 7365 3330 323d 5472 7565  to", use302=True
-00006320: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00006330: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00006340: 650a 0a20 2020 2020 2020 2072 6574 7572  e..        retur
-00006350: 6e20 7365 6c66 2e74 785f 6272 6f77 7365  n self.tx_browse
-00006360: 7228 290a 0a20 2020 2064 6566 2068 616e  r()..    def han
-00006370: 646c 655f 7072 6f70 6669 6e64 2873 656c  dle_propfind(sel
-00006380: 6629 2020 3a0a 2020 2020 2020 2020 6966  f)  :.        if
-00006390: 2073 656c 662e 646f 5f6c 6f67 3a0a 2020   self.do_log:.  
-000063a0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-000063b0: 6f67 2822 5046 494e 4420 2220 2b20 7365  og("PFIND " + se
-000063c0: 6c66 2e72 6571 290a 0a20 2020 2020 2020  lf.req)..       
-000063d0: 2069 6620 7365 6c66 2e61 7267 732e 6e6f   if self.args.no
-000063e0: 5f64 6176 3a0a 2020 2020 2020 2020 2020  _dav:.          
-000063f0: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
-00006400: 3035 2c20 2257 6562 4441 5620 6973 2064  05, "WebDAV is d
-00006410: 6973 6162 6c65 6420 696e 2073 6572 7665  isabled in serve
-00006420: 7220 636f 6e66 6967 2229 0a0a 2020 2020  r config")..    
-00006430: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-00006440: 6361 6e5f 7265 6164 2061 6e64 206e 6f74  can_read and not
-00006450: 2073 656c 662e 6361 6e5f 7772 6974 6520   self.can_write 
-00006460: 616e 6420 6e6f 7420 7365 6c66 2e63 616e  and not self.can
-00006470: 5f67 6574 3a0a 2020 2020 2020 2020 2020  _get:.          
-00006480: 2020 6966 2073 656c 662e 7670 6174 683a    if self.vpath:
-00006490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000064a0: 2073 656c 662e 6c6f 6728 2269 6e61 6363   self.log("inacc
-000064b0: 6573 7369 626c 653a 205b 7b7d 5d22 2e66  essible: [{}]".f
-000064c0: 6f72 6d61 7428 7365 6c66 2e76 7061 7468  ormat(self.vpath
-000064d0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-000064e0: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
-000064f0: 3430 312c 2022 6175 7468 656e 7469 6361  401, "authentica
-00006500: 7465 2229 0a0a 2020 2020 2020 2020 2020  te")..          
-00006510: 2020 7365 6c66 2e75 7061 7261 6d5b 2268    self.uparam["h
-00006520: 225d 203d 2022 220a 0a20 2020 2020 2020  "] = ""..       
-00006530: 2066 726f 6d20 2e64 786d 6c20 696d 706f   from .dxml impo
-00006540: 7274 2070 6172 7365 5f78 6d6c 0a0a 2020  rt parse_xml..  
-00006550: 2020 2020 2020 2320 656e 6320 3d20 2277        # enc = "w
-00006560: 696e 646f 7773 2d33 316a 220a 2020 2020  indows-31j".    
-00006570: 2020 2020 2320 656e 6320 3d20 2273 6869      # enc = "shi
-00006580: 6674 5f6a 6973 220a 2020 2020 2020 2020  ft_jis".        
-00006590: 656e 6320 3d20 2275 7466 2d38 220a 2020  enc = "utf-8".  
-000065a0: 2020 2020 2020 7565 6e63 203d 2065 6e63        uenc = enc
-000065b0: 2e75 7070 6572 2829 0a0a 2020 2020 2020  .upper()..      
-000065c0: 2020 636c 656e 203d 2069 6e74 2873 656c    clen = int(sel
-000065d0: 662e 6865 6164 6572 732e 6765 7428 2263  f.headers.get("c
-000065e0: 6f6e 7465 6e74 2d6c 656e 6774 6822 2c20  ontent-length", 
-000065f0: 3029 290a 2020 2020 2020 2020 6966 2063  0)).        if c
-00006600: 6c65 6e3a 0a20 2020 2020 2020 2020 2020  len:.           
-00006610: 2062 7566 203d 2062 2222 0a20 2020 2020   buf = b"".     
-00006620: 2020 2020 2020 2066 6f72 2072 6275 6620         for rbuf 
-00006630: 696e 2073 656c 662e 6765 745f 626f 6479  in self.get_body
-00006640: 5f72 6561 6465 7228 295b 305d 3a0a 2020  _reader()[0]:.  
-00006650: 2020 2020 2020 2020 2020 2020 2020 6275                bu
-00006660: 6620 2b3d 2072 6275 660a 2020 2020 2020  f += rbuf.      
-00006670: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00006680: 2072 6275 6620 6f72 206c 656e 2862 7566   rbuf or len(buf
-00006690: 2920 3e3d 2033 3237 3638 3a0a 2020 2020  ) >= 32768:.    
-000066a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066b0: 6272 6561 6b0a 0a20 2020 2020 2020 2020  break..         
-000066c0: 2020 2078 726f 6f74 203d 2070 6172 7365     xroot = parse
-000066d0: 5f78 6d6c 2862 7566 2e64 6563 6f64 6528  _xml(buf.decode(
-000066e0: 656e 632c 2022 7265 706c 6163 6522 2929  enc, "replace"))
-000066f0: 0a20 2020 2020 2020 2020 2020 2078 7461  .            xta
-00006700: 6720 3d20 6e65 7874 2878 2066 6f72 2078  g = next(x for x
-00006710: 2069 6e20 7872 6f6f 7420 6966 2078 2e74   in xroot if x.t
-00006720: 6167 2e73 706c 6974 2822 7d22 295b 2d31  ag.split("}")[-1
-00006730: 5d20 3d3d 2022 7072 6f70 2229 0a20 2020  ] == "prop").   
-00006740: 2020 2020 2020 2020 2070 726f 7073 5f6c           props_l
-00006750: 7374 203d 205b 792e 7461 672e 7370 6c69  st = [y.tag.spli
-00006760: 7428 227d 2229 5b2d 315d 2066 6f72 2079  t("}")[-1] for y
-00006770: 2069 6e20 7874 6167 5d0a 2020 2020 2020   in xtag].      
-00006780: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00006790: 2020 2020 7072 6f70 735f 6c73 7420 3d20      props_lst = 
-000067a0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-000067b0: 2020 2263 6f6e 7465 6e74 636c 6173 7322    "contentclass"
-000067c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000067d0: 2020 2263 7265 6174 696f 6e64 6174 6522    "creationdate"
-000067e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000067f0: 2020 2264 6566 6175 6c74 646f 6375 6d65    "defaultdocume
-00006800: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
-00006810: 2020 2020 2022 6469 7370 6c61 796e 616d       "displaynam
-00006820: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00006830: 2020 2020 2267 6574 636f 6e74 656e 746c      "getcontentl
-00006840: 616e 6775 6167 6522 2c0a 2020 2020 2020  anguage",.      
-00006850: 2020 2020 2020 2020 2020 2267 6574 636f            "getco
-00006860: 6e74 656e 746c 656e 6774 6822 2c0a 2020  ntentlength",.  
-00006870: 2020 2020 2020 2020 2020 2020 2020 2267                "g
-00006880: 6574 636f 6e74 656e 7474 7970 6522 2c0a  etcontenttype",.
-00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068a0: 2267 6574 6c61 7374 6d6f 6469 6669 6564  "getlastmodified
-000068b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000068c0: 2020 2022 6872 6566 222c 0a20 2020 2020     "href",.     
-000068d0: 2020 2020 2020 2020 2020 2022 6973 636f             "isco
-000068e0: 6c6c 6563 7469 6f6e 222c 0a20 2020 2020  llection",.     
-000068f0: 2020 2020 2020 2020 2020 2022 6973 6869             "ishi
-00006900: 6464 656e 222c 0a20 2020 2020 2020 2020  dden",.         
-00006910: 2020 2020 2020 2022 6973 7265 6164 6f6e         "isreadon
-00006920: 6c79 222c 0a20 2020 2020 2020 2020 2020  ly",.           
-00006930: 2020 2020 2022 6973 726f 6f74 222c 0a20       "isroot",. 
-00006940: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006950: 6973 7374 7275 6374 7572 6564 646f 6375  isstructureddocu
-00006960: 6d65 6e74 222c 0a20 2020 2020 2020 2020  ment",.         
-00006970: 2020 2020 2020 2022 6c61 7374 6163 6365         "lastacce
-00006980: 7373 6564 222c 0a20 2020 2020 2020 2020  ssed",.         
-00006990: 2020 2020 2020 2022 6e61 6d65 222c 0a20         "name",. 
-000069a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000069b0: 7061 7265 6e74 6e61 6d65 222c 0a20 2020  parentname",.   
-000069c0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-000069d0: 736f 7572 6365 7479 7065 222c 0a20 2020  sourcetype",.   
-000069e0: 2020 2020 2020 2020 2020 2020 2022 7375               "su
-000069f0: 7070 6f72 7465 646c 6f63 6b22 2c0a 2020  pportedlock",.  
-00006a00: 2020 2020 2020 2020 2020 5d0a 0a20 2020            ]..   
-00006a10: 2020 2020 2070 726f 7073 203d 2073 6574       props = set
-00006a20: 2870 726f 7073 5f6c 7374 290a 2020 2020  (props_lst).    
-00006a30: 2020 2020 766e 2c20 7265 6d20 3d20 7365      vn, rem = se
-00006a40: 6c66 2e61 7372 762e 7666 732e 6765 7428  lf.asrv.vfs.get(
-00006a50: 7365 6c66 2e76 7061 7468 2c20 7365 6c66  self.vpath, self
-00006a60: 2e75 6e61 6d65 2c20 5472 7565 2c20 4661  .uname, True, Fa
-00006a70: 6c73 652c 2065 7272 3d34 3031 290a 2020  lse, err=401).  
-00006a80: 2020 2020 2020 6465 7074 6820 3d20 7365        depth = se
-00006a90: 6c66 2e68 6561 6465 7273 2e67 6574 2822  lf.headers.get("
-00006aa0: 6465 7074 6822 2c20 2269 6e66 696e 6974  depth", "infinit
-00006ab0: 7922 292e 6c6f 7765 7228 290a 0a20 2020  y").lower()..   
-00006ac0: 2020 2020 2069 6620 6465 7074 6820 3d3d       if depth ==
-00006ad0: 2022 696e 6669 6e69 7479 223a 0a20 2020   "infinity":.   
-00006ae0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00006af0: 7365 6c66 2e61 7267 732e 6461 765f 696e  self.args.dav_in
-00006b00: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-00006b10: 2020 2073 656c 662e 6c6f 6728 2263 6c69     self.log("cli
-00006b20: 656e 7420 7761 6e74 7320 2d2d 6461 762d  ent wants --dav-
-00006b30: 696e 6622 2c20 3329 0a20 2020 2020 2020  inf", 3).       
-00006b40: 2020 2020 2020 2020 207a 6220 3d20 6227           zb = b'
-00006b50: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
-00006b60: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
-00006b70: 662d 3822 3f3e 5c6e 3c44 3a65 7272 6f72  f-8"?>\n<D:error
-00006b80: 2078 6d6c 6e73 3a44 3d22 4441 563a 223e   xmlns:D="DAV:">
-00006b90: 3c44 3a70 726f 7066 696e 642d 6669 6e69  <D:propfind-fini
-00006ba0: 7465 2d64 6570 7468 2f3e 3c2f 443a 6572  te-depth/></D:er
-00006bb0: 726f 723e 270a 2020 2020 2020 2020 2020  ror>'.          
-00006bc0: 2020 2020 2020 7365 6c66 2e72 6570 6c79        self.reply
-00006bd0: 287a 622c 2034 3033 2c20 2261 7070 6c69  (zb, 403, "appli
-00006be0: 6361 7469 6f6e 2f78 6d6c 3b20 6368 6172  cation/xml; char
-00006bf0: 7365 743d 7574 662d 3822 290a 2020 2020  set=utf-8").    
-00006c00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006c10: 726e 2054 7275 650a 0a20 2020 2020 2020  rn True..       
-00006c20: 2020 2020 2066 6765 6e20 3d20 766e 2e7a       fgen = vn.z
-00006c30: 6970 6765 6e28 0a20 2020 2020 2020 2020  ipgen(.         
-00006c40: 2020 2020 2020 2072 656d 2c0a 2020 2020         rem,.    
-00006c50: 2020 2020 2020 2020 2020 2020 7365 7428              set(
-00006c60: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00006c70: 2020 2073 656c 662e 756e 616d 652c 0a20     self.uname,. 
-00006c80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006c90: 656c 662e 6172 6773 2e65 642c 0a20 2020  elf.args.ed,.   
-00006ca0: 2020 2020 2020 2020 2020 2020 2054 7275               Tru
-00006cb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00006cc0: 2020 206e 6f74 2073 656c 662e 6172 6773     not self.args
-00006cd0: 2e6e 6f5f 7363 616e 6469 722c 0a20 2020  .no_scandir,.   
-00006ce0: 2020 2020 2020 2020 2020 2020 2077 7261               wra
-00006cf0: 703d 4661 6c73 652c 0a20 2020 2020 2020  p=False,.       
-00006d00: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00006d10: 656c 6966 2064 6570 7468 203d 3d20 2231  elif depth == "1
-00006d20: 223a 0a20 2020 2020 2020 2020 2020 205f  ":.            _
-00006d30: 2c20 7666 735f 6c73 2c20 7666 735f 7669  , vfs_ls, vfs_vi
-00006d40: 7274 203d 2076 6e2e 6c73 280a 2020 2020  rt = vn.ls(.    
-00006d50: 2020 2020 2020 2020 2020 2020 7265 6d2c              rem,
-00006d60: 2073 656c 662e 756e 616d 652c 206e 6f74   self.uname, not
-00006d70: 2073 656c 662e 6172 6773 2e6e 6f5f 7363   self.args.no_sc
-00006d80: 616e 6469 722c 205b 5b54 7275 652c 2046  andir, [[True, F
-00006d90: 616c 7365 5d5d 0a20 2020 2020 2020 2020  alse]].         
-00006da0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00006db0: 2069 6620 6e6f 7420 7365 6c66 2e61 7267   if not self.arg
-00006dc0: 732e 6564 3a0a 2020 2020 2020 2020 2020  s.ed:.          
-00006dd0: 2020 2020 2020 6e61 6d65 7320 3d20 7365        names = se
-00006de0: 7428 6578 636c 7564 655f 646f 7466 696c  t(exclude_dotfil
-00006df0: 6573 285b 785b 305d 2066 6f72 2078 2069  es([x[0] for x i
-00006e00: 6e20 7666 735f 6c73 5d29 290a 2020 2020  n vfs_ls])).    
-00006e10: 2020 2020 2020 2020 2020 2020 7666 735f              vfs_
-00006e20: 6c73 203d 205b 7820 666f 7220 7820 696e  ls = [x for x in
-00006e30: 2076 6673 5f6c 7320 6966 2078 5b30 5d20   vfs_ls if x[0] 
-00006e40: 696e 206e 616d 6573 5d0a 0a20 2020 2020  in names]..     
-00006e50: 2020 2020 2020 207a 6920 3d20 696e 7428         zi = int(
-00006e60: 7469 6d65 2e74 696d 6528 2929 0a20 2020  time.time()).   
-00006e70: 2020 2020 2020 2020 207a 7372 203d 206f           zsr = o
-00006e80: 732e 7374 6174 5f72 6573 756c 7428 2831  s.stat_result((1
-00006e90: 3638 3737 2c20 2d31 2c20 2d31 2c20 312c  6877, -1, -1, 1,
-00006ea0: 2031 3030 302c 2031 3030 302c 2038 2c20   1000, 1000, 8, 
-00006eb0: 7a69 2c20 7a69 2c20 7a69 2929 0a20 2020  zi, zi, zi)).   
-00006ec0: 2020 2020 2020 2020 206c 7320 3d20 5b7b           ls = [{
-00006ed0: 2276 7022 3a20 7670 2c20 2273 7422 3a20  "vp": vp, "st": 
-00006ee0: 7374 7d20 666f 7220 7670 2c20 7374 2069  st} for vp, st i
-00006ef0: 6e20 7666 735f 6c73 5d0a 2020 2020 2020  n vfs_ls].      
-00006f00: 2020 2020 2020 6c73 202b 3d20 5b7b 2276        ls += [{"v
-00006f10: 7022 3a20 762c 2022 7374 223a 207a 7372  p": v, "st": zsr
-00006f20: 7d20 666f 7220 7620 696e 2076 6673 5f76  } for v in vfs_v
-00006f30: 6972 745d 0a20 2020 2020 2020 2020 2020  irt].           
-00006f40: 2066 6765 6e20 3d20 6c73 2020 2320 7479   fgen = ls  # ty
-00006f50: 7065 3a20 6967 6e6f 7265 0a0a 2020 2020  pe: ignore..    
-00006f60: 2020 2020 656c 6966 2064 6570 7468 203d      elif depth =
-00006f70: 3d20 2230 223a 0a20 2020 2020 2020 2020  = "0":.         
-00006f80: 2020 2066 6765 6e20 3d20 5b5d 2020 2320     fgen = []  # 
-00006f90: 7479 7065 3a20 6967 6e6f 7265 0a0a 2020  type: ignore..  
-00006fa0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00006fb0: 2020 2020 2020 2020 7420 3d20 2269 6e76          t = "inv
-00006fc0: 616c 6964 2064 6570 7468 2076 616c 7565  alid depth value
-00006fd0: 2027 7b7d 2720 286d 7573 7420 6265 2065   '{}' (must be e
-00006fe0: 6974 6865 7220 2730 2720 6f72 2027 3127  ither '0' or '1'
-00006ff0: 7b7d 2922 0a20 2020 2020 2020 2020 2020  {})".           
-00007000: 2074 3220 3d20 2220 6f72 2027 696e 6669   t2 = " or 'infi
-00007010: 6e69 7479 2722 2069 6620 7365 6c66 2e61  nity'" if self.a
-00007020: 7267 732e 6461 765f 696e 6620 656c 7365  rgs.dav_inf else
-00007030: 2022 220a 2020 2020 2020 2020 2020 2020   "".            
-00007040: 7261 6973 6520 5065 626b 6163 2834 3132  raise Pebkac(412
-00007050: 2c20 742e 666f 726d 6174 2864 6570 7468  , t.format(depth
-00007060: 2c20 7432 2929 0a0a 2020 2020 2020 2020  , t2))..        
-00007070: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00007080: 2074 6f70 6469 7220 3d20 7b22 7670 223a   topdir = {"vp":
-00007090: 2022 222c 2022 7374 223a 206f 732e 7374   "", "st": os.st
-000070a0: 6174 2876 6e2e 6361 6e6f 6e69 6361 6c28  at(vn.canonical(
-000070b0: 7265 6d29 297d 0a20 2020 2020 2020 2065  rem))}.        e
-000070c0: 7863 6570 7420 4f53 4572 726f 7220 6173  xcept OSError as
-000070d0: 2065 783a 0a20 2020 2020 2020 2020 2020   ex:.           
-000070e0: 2069 6620 6578 2e65 7272 6e6f 2021 3d20   if ex.errno != 
-000070f0: 6572 726e 6f2e 454e 4f45 4e54 3a0a 2020  errno.ENOENT:.  
-00007100: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00007110: 6973 650a 2020 2020 2020 2020 2020 2020  ise.            
-00007120: 7261 6973 6520 5065 626b 6163 2834 3034  raise Pebkac(404
-00007130: 290a 0a20 2020 2020 2020 2066 6765 6e20  )..        fgen 
-00007140: 3d20 6974 6572 746f 6f6c 732e 6368 6169  = itertools.chai
-00007150: 6e28 5b74 6f70 6469 725d 2c20 6667 656e  n([topdir], fgen
-00007160: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
-00007170: 650a 2020 2020 2020 2020 7674 6f70 203d  e.        vtop =
-00007180: 2076 6a6f 696e 2873 656c 662e 6172 6773   vjoin(self.args
-00007190: 2e52 2c20 766a 6f69 6e28 766e 2e76 7061  .R, vjoin(vn.vpa
-000071a0: 7468 2c20 7265 6d29 290a 0a20 2020 2020  th, rem))..     
-000071b0: 2020 2063 6875 6e6b 737a 203d 2030 7837     chunksz = 0x7
-000071c0: 4646 3820 2023 2070 7265 6665 7272 6564  FF8  # preferred
-000071d0: 2062 7920 6e67 696e 7820 6f72 2063 6620   by nginx or cf 
-000071e0: 2864 756e 6e6f 2077 6869 6368 290a 0a20  (dunno which).. 
-000071f0: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-00007200: 5f68 6561 6465 7273 280a 2020 2020 2020  _headers(.      
-00007210: 2020 2020 2020 4e6f 6e65 2c20 3230 372c        None, 207,
-00007220: 2022 7465 7874 2f78 6d6c 3b20 6368 6172   "text/xml; char
-00007230: 7365 743d 2220 2b20 656e 632c 207b 2254  set=" + enc, {"T
-00007240: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
-00007250: 223a 2022 6368 756e 6b65 6422 7d0a 2020  ": "chunked"}.  
-00007260: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00007270: 2072 6574 203d 2027 3c3f 786d 6c20 7665   ret = '<?xml ve
-00007280: 7273 696f 6e3d 2231 2e30 2220 656e 636f  rsion="1.0" enco
-00007290: 6469 6e67 3d22 7b7d 223f 3e5c 6e3c 443a  ding="{}"?>\n<D:
-000072a0: 6d75 6c74 6973 7461 7475 7320 786d 6c6e  multistatus xmln
-000072b0: 733a 443d 2244 4156 3a22 3e27 0a20 2020  s:D="DAV:">'.   
-000072c0: 2020 2020 2072 6574 203d 2072 6574 2e66       ret = ret.f
-000072d0: 6f72 6d61 7428 7565 6e63 290a 2020 2020  ormat(uenc).    
-000072e0: 2020 2020 666f 7220 7820 696e 2066 6765      for x in fge
-000072f0: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
-00007300: 7020 3d20 766a 6f69 6e28 7674 6f70 2c20  p = vjoin(vtop, 
-00007310: 785b 2276 7022 5d29 0a20 2020 2020 2020  x["vp"]).       
-00007320: 2020 2020 2073 7420 203d 2078 5b22 7374       st  = x["st
-00007330: 225d 0a20 2020 2020 2020 2020 2020 2069  "].            i
-00007340: 7364 6972 203d 2073 7461 742e 535f 4953  sdir = stat.S_IS
-00007350: 4449 5228 7374 2e73 745f 6d6f 6465 290a  DIR(st.st_mode).
-00007360: 0a20 2020 2020 2020 2020 2020 2074 203d  .            t =
-00007370: 2022 3c44 3a72 6573 706f 6e73 653e 3c44   "<D:response><D
-00007380: 3a68 7265 663e 2f7b 7d7b 7d3c 2f44 3a68  :href>/{}{}</D:h
-00007390: 7265 663e 3c44 3a70 726f 7073 7461 743e  ref><D:propstat>
-000073a0: 3c44 3a70 726f 703e 220a 2020 2020 2020  <D:prop>".      
-000073b0: 2020 2020 2020 7265 7420 2b3d 2074 2e66        ret += t.f
-000073c0: 6f72 6d61 7428 7175 6f74 6570 2872 7029  ormat(quotep(rp)
-000073d0: 2c20 222f 2220 6966 2069 7364 6972 2061  , "/" if isdir a
-000073e0: 6e64 2072 7020 656c 7365 2022 2229 0a0a  nd rp else "")..
-000073f0: 2020 2020 2020 2020 2020 2020 7076 7320              pvs 
-00007400: 2020 3d20 7b0a 2020 2020 2020 2020 2020    = {.          
-00007410: 2020 2020 2020 2264 6973 706c 6179 6e61        "displayna
-00007420: 6d65 223a 2068 746d 6c5f 6573 6361 7065  me": html_escape
-00007430: 2872 702e 7370 6c69 7428 222f 2229 5b2d  (rp.split("/")[-
-00007440: 315d 292c 0a20 2020 2020 2020 2020 2020  1]),.           
-00007450: 2020 2020 2022 6765 746c 6173 746d 6f64       "getlastmod
-00007460: 6966 6965 6422 3a20 666f 726d 6174 6461  ified": formatda
-00007470: 7465 2873 742e 7374 5f6d 7469 6d65 2c20  te(st.st_mtime, 
-00007480: 7573 6567 6d74 3d54 7275 6529 2c0a 2020  usegmt=True),.  
-00007490: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-000074a0: 6573 6f75 7263 6574 7970 6522 3a20 273c  esourcetype": '<
-000074b0: 443a 636f 6c6c 6563 7469 6f6e 2078 6d6c  D:collection xml
-000074c0: 6e73 3a44 3d22 4441 563a 222f 3e27 2069  ns:D="DAV:"/>' i
-000074d0: 6620 6973 6469 7220 656c 7365 2022 222c  f isdir else "",
-000074e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000074f0: 2022 7375 7070 6f72 7465 646c 6f63 6b22   "supportedlock"
-00007500: 3a20 273c 443a 6c6f 636b 656e 7472 7920  : '<D:lockentry 
-00007510: 786d 6c6e 733a 443d 2244 4156 3a22 3e3c  xmlns:D="DAV:"><
-00007520: 443a 6c6f 636b 7363 6f70 653e 3c44 3a65  D:lockscope><D:e
-00007530: 7863 6c75 7369 7665 2f3e 3c2f 443a 6c6f  xclusive/></D:lo
-00007540: 636b 7363 6f70 653e 3c44 3a6c 6f63 6b74  ckscope><D:lockt
-00007550: 7970 653e 3c44 3a77 7269 7465 2f3e 3c2f  ype><D:write/></
-00007560: 443a 6c6f 636b 7479 7065 3e3c 2f44 3a6c  D:locktype></D:l
-00007570: 6f63 6b65 6e74 7279 3e27 2c0a 2020 2020  ockentry>',.    
-00007580: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00007590: 2020 2020 2020 6966 206e 6f74 2069 7364        if not isd
-000075a0: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
-000075b0: 2020 2020 7076 735b 2267 6574 636f 6e74      pvs["getcont
-000075c0: 656e 7474 7970 6522 5d20 3d20 6874 6d6c  enttype"] = html
-000075d0: 5f65 7363 6170 6528 6775 6573 735f 6d69  _escape(guess_mi
-000075e0: 6d65 2872 7029 290a 2020 2020 2020 2020  me(rp)).        
-000075f0: 2020 2020 2020 2020 7076 735b 2267 6574          pvs["get
-00007600: 636f 6e74 656e 746c 656e 6774 6822 5d20  contentlength"] 
-00007610: 3d20 7374 7228 7374 2e73 745f 7369 7a65  = str(st.st_size
-00007620: 290a 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00007630: 6f72 206b 2c20 7620 696e 2070 7673 2e69  or k, v in pvs.i
-00007640: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-00007650: 2020 2020 2020 2020 6966 206b 206e 6f74          if k not
-00007660: 2069 6e20 7072 6f70 733a 0a20 2020 2020   in props:.     
-00007670: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00007680: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00007690: 2020 2020 2020 2020 656c 6966 2076 3a0a          elif v:.
+00006030: 7475 726e 2073 656c 662e 7365 7463 6b28  turn self.setck(
+00006040: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00006050: 6620 2272 6573 6574 2220 696e 2073 656c  f "reset" in sel
+00006060: 662e 7570 6172 616d 3a0a 2020 2020 2020  f.uparam:.      
+00006070: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00006080: 2073 656c 662e 7365 745f 6366 675f 7265   self.set_cfg_re
+00006090: 7365 7428 290a 0a20 2020 2020 2020 2020  set()..         
+000060a0: 2020 2069 6620 2268 6322 2069 6e20 7365     if "hc" in se
+000060b0: 6c66 2e75 7061 7261 6d3a 0a20 2020 2020  lf.uparam:.     
+000060c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000060d0: 6e20 7365 6c66 2e74 785f 7376 6373 2829  n self.tx_svcs()
+000060e0: 0a0a 2020 2020 2020 2020 6966 2022 6822  ..        if "h"
+000060f0: 2069 6e20 7365 6c66 2e75 7061 7261 6d3a   in self.uparam:
+00006100: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00006110: 7572 6e20 7365 6c66 2e74 785f 6d6f 756e  urn self.tx_moun
+00006120: 7473 2829 0a0a 2020 2020 2020 2020 2320  ts()..        # 
+00006130: 636f 6e64 6974 696f 6e61 6c20 7265 6469  conditional redi
+00006140: 7265 6374 2074 6f20 7369 6e67 6c65 2076  rect to single v
+00006150: 6f6c 756d 6573 0a20 2020 2020 2020 2069  olumes.        i
+00006160: 6620 7365 6c66 2e76 7061 7468 203d 3d20  f self.vpath == 
+00006170: 2222 2061 6e64 206e 6f74 2073 656c 662e  "" and not self.
+00006180: 6f75 7061 7261 6d3a 0a20 2020 2020 2020  ouparam:.       
+00006190: 2020 2020 206e 7265 6164 203d 206c 656e       nread = len
+000061a0: 2873 656c 662e 7276 6f6c 290a 2020 2020  (self.rvol).    
+000061b0: 2020 2020 2020 2020 6e77 7269 7465 203d          nwrite =
+000061c0: 206c 656e 2873 656c 662e 7776 6f6c 290a   len(self.wvol).
+000061d0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+000061e0: 7265 6164 202b 206e 7772 6974 6520 3d3d  read + nwrite ==
+000061f0: 2031 206f 7220 2873 656c 662e 7276 6f6c   1 or (self.rvol
+00006200: 203d 3d20 7365 6c66 2e77 766f 6c20 616e   == self.wvol an
+00006210: 6420 6e72 6561 6420 3d3d 2031 293a 0a20  d nread == 1):. 
+00006220: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00006230: 6620 6e72 6561 6420 3d3d 2031 3a0a 2020  f nread == 1:.  
+00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006250: 2020 7670 6174 6820 3d20 7365 6c66 2e72    vpath = self.r
+00006260: 766f 6c5b 305d 0a20 2020 2020 2020 2020  vol[0].         
+00006270: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006290: 2076 7061 7468 203d 2073 656c 662e 7776   vpath = self.wv
+000062a0: 6f6c 5b30 5d0a 0a20 2020 2020 2020 2020  ol[0]..         
+000062b0: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+000062c0: 7061 7468 2021 3d20 7670 6174 683a 0a20  path != vpath:. 
+000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062e0: 2020 2073 656c 662e 7265 6469 7265 6374     self.redirect
+000062f0: 2876 7061 7468 2c20 666c 6176 6f72 3d22  (vpath, flavor="
+00006300: 7265 6469 7265 6374 696e 6720 746f 222c  redirecting to",
+00006310: 2075 7365 3330 323d 5472 7565 290a 2020   use302=True).  
+00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006330: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+00006340: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00006350: 6c66 2e74 785f 6272 6f77 7365 7228 290a  lf.tx_browser().
+00006360: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
+00006370: 7072 6f70 6669 6e64 2873 656c 6629 2020  propfind(self)  
+00006380: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00006390: 662e 646f 5f6c 6f67 3a0a 2020 2020 2020  f.do_log:.      
+000063a0: 2020 2020 2020 7365 6c66 2e6c 6f67 2822        self.log("
+000063b0: 5046 494e 4420 2220 2b20 7365 6c66 2e72  PFIND " + self.r
+000063c0: 6571 290a 0a20 2020 2020 2020 2069 6620  eq)..        if 
+000063d0: 7365 6c66 2e61 7267 732e 6e6f 5f64 6176  self.args.no_dav
+000063e0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000063f0: 6973 6520 5065 626b 6163 2834 3035 2c20  ise Pebkac(405, 
+00006400: 2257 6562 4441 5620 6973 2064 6973 6162  "WebDAV is disab
+00006410: 6c65 6420 696e 2073 6572 7665 7220 636f  led in server co
+00006420: 6e66 6967 2229 0a0a 2020 2020 2020 2020  nfig")..        
+00006430: 6966 206e 6f74 2073 656c 662e 6361 6e5f  if not self.can_
+00006440: 7265 6164 2061 6e64 206e 6f74 2073 656c  read and not sel
+00006450: 662e 6361 6e5f 7772 6974 6520 616e 6420  f.can_write and 
+00006460: 6e6f 7420 7365 6c66 2e63 616e 5f67 6574  not self.can_get
+00006470: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00006480: 2073 656c 662e 7670 6174 683a 0a20 2020   self.vpath:.   
+00006490: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000064a0: 662e 6c6f 6728 2269 6e61 6363 6573 7369  f.log("inaccessi
+000064b0: 626c 653a 205b 7b7d 5d22 2e66 6f72 6d61  ble: [{}]".forma
+000064c0: 7428 7365 6c66 2e76 7061 7468 2929 0a20  t(self.vpath)). 
+000064d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000064e0: 6169 7365 2050 6562 6b61 6328 3430 312c  aise Pebkac(401,
+000064f0: 2022 6175 7468 656e 7469 6361 7465 2229   "authenticate")
+00006500: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00006510: 6c66 2e75 7061 7261 6d5b 2268 225d 203d  lf.uparam["h"] =
+00006520: 2022 220a 0a20 2020 2020 2020 2066 726f   ""..        fro
+00006530: 6d20 2e64 786d 6c20 696d 706f 7274 2070  m .dxml import p
+00006540: 6172 7365 5f78 6d6c 0a0a 2020 2020 2020  arse_xml..      
+00006550: 2020 2320 656e 6320 3d20 2277 696e 646f    # enc = "windo
+00006560: 7773 2d33 316a 220a 2020 2020 2020 2020  ws-31j".        
+00006570: 2320 656e 6320 3d20 2273 6869 6674 5f6a  # enc = "shift_j
+00006580: 6973 220a 2020 2020 2020 2020 656e 6320  is".        enc 
+00006590: 3d20 2275 7466 2d38 220a 2020 2020 2020  = "utf-8".      
+000065a0: 2020 7565 6e63 203d 2065 6e63 2e75 7070    uenc = enc.upp
+000065b0: 6572 2829 0a0a 2020 2020 2020 2020 636c  er()..        cl
+000065c0: 656e 203d 2069 6e74 2873 656c 662e 6865  en = int(self.he
+000065d0: 6164 6572 732e 6765 7428 2263 6f6e 7465  aders.get("conte
+000065e0: 6e74 2d6c 656e 6774 6822 2c20 3029 290a  nt-length", 0)).
+000065f0: 2020 2020 2020 2020 6966 2063 6c65 6e3a          if clen:
+00006600: 0a20 2020 2020 2020 2020 2020 2062 7566  .            buf
+00006610: 203d 2062 2222 0a20 2020 2020 2020 2020   = b"".         
+00006620: 2020 2066 6f72 2072 6275 6620 696e 2073     for rbuf in s
+00006630: 656c 662e 6765 745f 626f 6479 5f72 6561  elf.get_body_rea
+00006640: 6465 7228 295b 305d 3a0a 2020 2020 2020  der()[0]:.      
+00006650: 2020 2020 2020 2020 2020 6275 6620 2b3d            buf +=
+00006660: 2072 6275 660a 2020 2020 2020 2020 2020   rbuf.          
+00006670: 2020 2020 2020 6966 206e 6f74 2072 6275        if not rbu
+00006680: 6620 6f72 206c 656e 2862 7566 2920 3e3d  f or len(buf) >=
+00006690: 2033 3237 3638 3a0a 2020 2020 2020 2020   32768:.        
+000066a0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+000066b0: 6b0a 0a20 2020 2020 2020 2020 2020 2078  k..            x
+000066c0: 726f 6f74 203d 2070 6172 7365 5f78 6d6c  root = parse_xml
+000066d0: 2862 7566 2e64 6563 6f64 6528 656e 632c  (buf.decode(enc,
+000066e0: 2022 7265 706c 6163 6522 2929 0a20 2020   "replace")).   
+000066f0: 2020 2020 2020 2020 2078 7461 6720 3d20           xtag = 
+00006700: 6e65 7874 2878 2066 6f72 2078 2069 6e20  next(x for x in 
+00006710: 7872 6f6f 7420 6966 2078 2e74 6167 2e73  xroot if x.tag.s
+00006720: 706c 6974 2822 7d22 295b 2d31 5d20 3d3d  plit("}")[-1] ==
+00006730: 2022 7072 6f70 2229 0a20 2020 2020 2020   "prop").       
+00006740: 2020 2020 2070 726f 7073 5f6c 7374 203d       props_lst =
+00006750: 205b 792e 7461 672e 7370 6c69 7428 227d   [y.tag.split("}
+00006760: 2229 5b2d 315d 2066 6f72 2079 2069 6e20  ")[-1] for y in 
+00006770: 7874 6167 5d0a 2020 2020 2020 2020 656c  xtag].        el
+00006780: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00006790: 7072 6f70 735f 6c73 7420 3d20 5b0a 2020  props_lst = [.  
+000067a0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+000067b0: 6f6e 7465 6e74 636c 6173 7322 2c0a 2020  ontentclass",.  
+000067c0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+000067d0: 7265 6174 696f 6e64 6174 6522 2c0a 2020  reationdate",.  
+000067e0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000067f0: 6566 6175 6c74 646f 6375 6d65 6e74 222c  efaultdocument",
+00006800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006810: 2022 6469 7370 6c61 796e 616d 6522 2c0a   "displayname",.
+00006820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006830: 2267 6574 636f 6e74 656e 746c 616e 6775  "getcontentlangu
+00006840: 6167 6522 2c0a 2020 2020 2020 2020 2020  age",.          
+00006850: 2020 2020 2020 2267 6574 636f 6e74 656e        "getconten
+00006860: 746c 656e 6774 6822 2c0a 2020 2020 2020  tlength",.      
+00006870: 2020 2020 2020 2020 2020 2267 6574 636f            "getco
+00006880: 6e74 656e 7474 7970 6522 2c0a 2020 2020  ntenttype",.    
+00006890: 2020 2020 2020 2020 2020 2020 2267 6574              "get
+000068a0: 6c61 7374 6d6f 6469 6669 6564 222c 0a20  lastmodified",. 
+000068b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000068c0: 6872 6566 222c 0a20 2020 2020 2020 2020  href",.         
+000068d0: 2020 2020 2020 2022 6973 636f 6c6c 6563         "iscollec
+000068e0: 7469 6f6e 222c 0a20 2020 2020 2020 2020  tion",.         
+000068f0: 2020 2020 2020 2022 6973 6869 6464 656e         "ishidden
+00006900: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006910: 2020 2022 6973 7265 6164 6f6e 6c79 222c     "isreadonly",
+00006920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006930: 2022 6973 726f 6f74 222c 0a20 2020 2020   "isroot",.     
+00006940: 2020 2020 2020 2020 2020 2022 6973 7374             "isst
+00006950: 7275 6374 7572 6564 646f 6375 6d65 6e74  ructureddocument
+00006960: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006970: 2020 2022 6c61 7374 6163 6365 7373 6564     "lastaccessed
+00006980: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006990: 2020 2022 6e61 6d65 222c 0a20 2020 2020     "name",.     
+000069a0: 2020 2020 2020 2020 2020 2022 7061 7265             "pare
+000069b0: 6e74 6e61 6d65 222c 0a20 2020 2020 2020  ntname",.       
+000069c0: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
+000069d0: 6365 7479 7065 222c 0a20 2020 2020 2020  cetype",.       
+000069e0: 2020 2020 2020 2020 2022 7375 7070 6f72           "suppor
+000069f0: 7465 646c 6f63 6b22 2c0a 2020 2020 2020  tedlock",.      
+00006a00: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
+00006a10: 2070 726f 7073 203d 2073 6574 2870 726f   props = set(pro
+00006a20: 7073 5f6c 7374 290a 2020 2020 2020 2020  ps_lst).        
+00006a30: 766e 2c20 7265 6d20 3d20 7365 6c66 2e61  vn, rem = self.a
+00006a40: 7372 762e 7666 732e 6765 7428 7365 6c66  srv.vfs.get(self
+00006a50: 2e76 7061 7468 2c20 7365 6c66 2e75 6e61  .vpath, self.una
+00006a60: 6d65 2c20 5472 7565 2c20 4661 6c73 652c  me, True, False,
+00006a70: 2065 7272 3d34 3031 290a 2020 2020 2020   err=401).      
+00006a80: 2020 6465 7074 6820 3d20 7365 6c66 2e68    depth = self.h
+00006a90: 6561 6465 7273 2e67 6574 2822 6465 7074  eaders.get("dept
+00006aa0: 6822 2c20 2269 6e66 696e 6974 7922 292e  h", "infinity").
+00006ab0: 6c6f 7765 7228 290a 0a20 2020 2020 2020  lower()..       
+00006ac0: 2069 6620 6465 7074 6820 3d3d 2022 696e   if depth == "in
+00006ad0: 6669 6e69 7479 223a 0a20 2020 2020 2020  finity":.       
+00006ae0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00006af0: 2e61 7267 732e 6461 765f 696e 663a 0a20  .args.dav_inf:. 
+00006b00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006b10: 656c 662e 6c6f 6728 2263 6c69 656e 7420  elf.log("client 
+00006b20: 7761 6e74 7320 2d2d 6461 762d 696e 6622  wants --dav-inf"
+00006b30: 2c20 3329 0a20 2020 2020 2020 2020 2020  , 3).           
+00006b40: 2020 2020 207a 6220 3d20 6227 3c3f 786d       zb = b'<?xm
+00006b50: 6c20 7665 7273 696f 6e3d 2231 2e30 2220  l version="1.0" 
+00006b60: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+00006b70: 3f3e 5c6e 3c44 3a65 7272 6f72 2078 6d6c  ?>\n<D:error xml
+00006b80: 6e73 3a44 3d22 4441 563a 223e 3c44 3a70  ns:D="DAV:"><D:p
+00006b90: 726f 7066 696e 642d 6669 6e69 7465 2d64  ropfind-finite-d
+00006ba0: 6570 7468 2f3e 3c2f 443a 6572 726f 723e  epth/></D:error>
+00006bb0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00006bc0: 2020 7365 6c66 2e72 6570 6c79 287a 622c    self.reply(zb,
+00006bd0: 2034 3033 2c20 2261 7070 6c69 6361 7469   403, "applicati
+00006be0: 6f6e 2f78 6d6c 3b20 6368 6172 7365 743d  on/xml; charset=
+00006bf0: 7574 662d 3822 290a 2020 2020 2020 2020  utf-8").        
+00006c00: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00006c10: 7275 650a 0a20 2020 2020 2020 2020 2020  rue..           
+00006c20: 2066 6765 6e20 3d20 766e 2e7a 6970 6765   fgen = vn.zipge
+00006c30: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00006c40: 2020 2072 656d 2c0a 2020 2020 2020 2020     rem,.        
+00006c50: 2020 2020 2020 2020 7365 7428 292c 0a20          set(),. 
+00006c60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006c70: 656c 662e 756e 616d 652c 0a20 2020 2020  elf.uname,.     
+00006c80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006c90: 6172 6773 2e65 642c 0a20 2020 2020 2020  args.ed,.       
+00006ca0: 2020 2020 2020 2020 2054 7275 652c 0a20           True,. 
+00006cb0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00006cc0: 6f74 2073 656c 662e 6172 6773 2e6e 6f5f  ot self.args.no_
+00006cd0: 7363 616e 6469 722c 0a20 2020 2020 2020  scandir,.       
+00006ce0: 2020 2020 2020 2020 2077 7261 703d 4661           wrap=Fa
+00006cf0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00006d00: 2029 0a0a 2020 2020 2020 2020 656c 6966   )..        elif
+00006d10: 2064 6570 7468 203d 3d20 2231 223a 0a20   depth == "1":. 
+00006d20: 2020 2020 2020 2020 2020 205f 2c20 7666             _, vf
+00006d30: 735f 6c73 2c20 7666 735f 7669 7274 203d  s_ls, vfs_virt =
+00006d40: 2076 6e2e 6c73 280a 2020 2020 2020 2020   vn.ls(.        
+00006d50: 2020 2020 2020 2020 7265 6d2c 2073 656c          rem, sel
+00006d60: 662e 756e 616d 652c 206e 6f74 2073 656c  f.uname, not sel
+00006d70: 662e 6172 6773 2e6e 6f5f 7363 616e 6469  f.args.no_scandi
+00006d80: 722c 205b 5b54 7275 652c 2046 616c 7365  r, [[True, False
+00006d90: 5d5d 0a20 2020 2020 2020 2020 2020 2029  ]].            )
+00006da0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00006db0: 6e6f 7420 7365 6c66 2e61 7267 732e 6564  not self.args.ed
+00006dc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006dd0: 2020 6e61 6d65 7320 3d20 7365 7428 6578    names = set(ex
+00006de0: 636c 7564 655f 646f 7466 696c 6573 285b  clude_dotfiles([
+00006df0: 785b 305d 2066 6f72 2078 2069 6e20 7666  x[0] for x in vf
+00006e00: 735f 6c73 5d29 290a 2020 2020 2020 2020  s_ls])).        
+00006e10: 2020 2020 2020 2020 7666 735f 6c73 203d          vfs_ls =
+00006e20: 205b 7820 666f 7220 7820 696e 2076 6673   [x for x in vfs
+00006e30: 5f6c 7320 6966 2078 5b30 5d20 696e 206e  _ls if x[0] in n
+00006e40: 616d 6573 5d0a 0a20 2020 2020 2020 2020  ames]..         
+00006e50: 2020 207a 6920 3d20 696e 7428 7469 6d65     zi = int(time
+00006e60: 2e74 696d 6528 2929 0a20 2020 2020 2020  .time()).       
+00006e70: 2020 2020 207a 7372 203d 206f 732e 7374       zsr = os.st
+00006e80: 6174 5f72 6573 756c 7428 2831 3638 3737  at_result((16877
+00006e90: 2c20 2d31 2c20 2d31 2c20 312c 2031 3030  , -1, -1, 1, 100
+00006ea0: 302c 2031 3030 302c 2038 2c20 7a69 2c20  0, 1000, 8, zi, 
+00006eb0: 7a69 2c20 7a69 2929 0a20 2020 2020 2020  zi, zi)).       
+00006ec0: 2020 2020 206c 7320 3d20 5b7b 2276 7022       ls = [{"vp"
+00006ed0: 3a20 7670 2c20 2273 7422 3a20 7374 7d20  : vp, "st": st} 
+00006ee0: 666f 7220 7670 2c20 7374 2069 6e20 7666  for vp, st in vf
+00006ef0: 735f 6c73 5d0a 2020 2020 2020 2020 2020  s_ls].          
+00006f00: 2020 6c73 202b 3d20 5b7b 2276 7022 3a20    ls += [{"vp": 
+00006f10: 762c 2022 7374 223a 207a 7372 7d20 666f  v, "st": zsr} fo
+00006f20: 7220 7620 696e 2076 6673 5f76 6972 745d  r v in vfs_virt]
+00006f30: 0a20 2020 2020 2020 2020 2020 2066 6765  .            fge
+00006f40: 6e20 3d20 6c73 2020 2320 7479 7065 3a20  n = ls  # type: 
+00006f50: 6967 6e6f 7265 0a0a 2020 2020 2020 2020  ignore..        
+00006f60: 656c 6966 2064 6570 7468 203d 3d20 2230  elif depth == "0
+00006f70: 223a 0a20 2020 2020 2020 2020 2020 2066  ":.            f
+00006f80: 6765 6e20 3d20 5b5d 2020 2320 7479 7065  gen = []  # type
+00006f90: 3a20 6967 6e6f 7265 0a0a 2020 2020 2020  : ignore..      
+00006fa0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00006fb0: 2020 2020 7420 3d20 2269 6e76 616c 6964      t = "invalid
+00006fc0: 2064 6570 7468 2076 616c 7565 2027 7b7d   depth value '{}
+00006fd0: 2720 286d 7573 7420 6265 2065 6974 6865  ' (must be eithe
+00006fe0: 7220 2730 2720 6f72 2027 3127 7b7d 2922  r '0' or '1'{})"
+00006ff0: 0a20 2020 2020 2020 2020 2020 2074 3220  .            t2 
+00007000: 3d20 2220 6f72 2027 696e 6669 6e69 7479  = " or 'infinity
+00007010: 2722 2069 6620 7365 6c66 2e61 7267 732e  '" if self.args.
+00007020: 6461 765f 696e 6620 656c 7365 2022 220a  dav_inf else "".
+00007030: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00007040: 6520 5065 626b 6163 2834 3132 2c20 742e  e Pebkac(412, t.
+00007050: 666f 726d 6174 2864 6570 7468 2c20 7432  format(depth, t2
+00007060: 2929 0a0a 2020 2020 2020 2020 7472 793a  ))..        try:
+00007070: 0a20 2020 2020 2020 2020 2020 2074 6f70  .            top
+00007080: 6469 7220 3d20 7b22 7670 223a 2022 222c  dir = {"vp": "",
+00007090: 2022 7374 223a 206f 732e 7374 6174 2876   "st": os.stat(v
+000070a0: 6e2e 6361 6e6f 6e69 6361 6c28 7265 6d29  n.canonical(rem)
+000070b0: 297d 0a20 2020 2020 2020 2065 7863 6570  )}.        excep
+000070c0: 7420 4f53 4572 726f 7220 6173 2065 783a  t OSError as ex:
+000070d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000070e0: 6578 2e65 7272 6e6f 2021 3d20 6572 726e  ex.errno != errn
+000070f0: 6f2e 454e 4f45 4e54 3a0a 2020 2020 2020  o.ENOENT:.      
+00007100: 2020 2020 2020 2020 2020 7261 6973 650a            raise.
+00007110: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00007120: 6520 5065 626b 6163 2834 3034 290a 0a20  e Pebkac(404).. 
+00007130: 2020 2020 2020 2066 6765 6e20 3d20 6974         fgen = it
+00007140: 6572 746f 6f6c 732e 6368 6169 6e28 5b74  ertools.chain([t
+00007150: 6f70 6469 725d 2c20 6667 656e 2920 2023  opdir], fgen)  #
+00007160: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
+00007170: 2020 2020 2020 7674 6f70 203d 2076 6a6f        vtop = vjo
+00007180: 696e 2873 656c 662e 6172 6773 2e52 2c20  in(self.args.R, 
+00007190: 766a 6f69 6e28 766e 2e76 7061 7468 2c20  vjoin(vn.vpath, 
+000071a0: 7265 6d29 290a 0a20 2020 2020 2020 2063  rem))..        c
+000071b0: 6875 6e6b 737a 203d 2030 7837 4646 3820  hunksz = 0x7FF8 
+000071c0: 2023 2070 7265 6665 7272 6564 2062 7920   # preferred by 
+000071d0: 6e67 696e 7820 6f72 2063 6620 2864 756e  nginx or cf (dun
+000071e0: 6e6f 2077 6869 6368 290a 0a20 2020 2020  no which)..     
+000071f0: 2020 2073 656c 662e 7365 6e64 5f68 6561     self.send_hea
+00007200: 6465 7273 280a 2020 2020 2020 2020 2020  ders(.          
+00007210: 2020 4e6f 6e65 2c20 3230 372c 2022 7465    None, 207, "te
+00007220: 7874 2f78 6d6c 3b20 6368 6172 7365 743d  xt/xml; charset=
+00007230: 2220 2b20 656e 632c 207b 2254 7261 6e73  " + enc, {"Trans
+00007240: 6665 722d 456e 636f 6469 6e67 223a 2022  fer-Encoding": "
+00007250: 6368 756e 6b65 6422 7d0a 2020 2020 2020  chunked"}.      
+00007260: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+00007270: 203d 2027 3c3f 786d 6c20 7665 7273 696f   = '<?xml versio
+00007280: 6e3d 2231 2e30 2220 656e 636f 6469 6e67  n="1.0" encoding
+00007290: 3d22 7b7d 223f 3e5c 6e3c 443a 6d75 6c74  ="{}"?>\n<D:mult
+000072a0: 6973 7461 7475 7320 786d 6c6e 733a 443d  istatus xmlns:D=
+000072b0: 2244 4156 3a22 3e27 0a20 2020 2020 2020  "DAV:">'.       
+000072c0: 2072 6574 203d 2072 6574 2e66 6f72 6d61   ret = ret.forma
+000072d0: 7428 7565 6e63 290a 2020 2020 2020 2020  t(uenc).        
+000072e0: 666f 7220 7820 696e 2066 6765 6e3a 0a20  for x in fgen:. 
+000072f0: 2020 2020 2020 2020 2020 2072 7020 3d20             rp = 
+00007300: 766a 6f69 6e28 7674 6f70 2c20 785b 2276  vjoin(vtop, x["v
+00007310: 7022 5d29 0a20 2020 2020 2020 2020 2020  p"]).           
+00007320: 2073 7420 203d 2078 5b22 7374 225d 0a20   st  = x["st"]. 
+00007330: 2020 2020 2020 2020 2020 2069 7364 6972             isdir
+00007340: 203d 2073 7461 742e 535f 4953 4449 5228   = stat.S_ISDIR(
+00007350: 7374 2e73 745f 6d6f 6465 290a 0a20 2020  st.st_mode)..   
+00007360: 2020 2020 2020 2020 2074 203d 2022 3c44           t = "<D
+00007370: 3a72 6573 706f 6e73 653e 3c44 3a68 7265  :response><D:hre
+00007380: 663e 2f7b 7d7b 7d3c 2f44 3a68 7265 663e  f>/{}{}</D:href>
+00007390: 3c44 3a70 726f 7073 7461 743e 3c44 3a70  <D:propstat><D:p
+000073a0: 726f 703e 220a 2020 2020 2020 2020 2020  rop>".          
+000073b0: 2020 7265 7420 2b3d 2074 2e66 6f72 6d61    ret += t.forma
+000073c0: 7428 7175 6f74 6570 2872 7029 2c20 222f  t(quotep(rp), "/
+000073d0: 2220 6966 2069 7364 6972 2061 6e64 2072  " if isdir and r
+000073e0: 7020 656c 7365 2022 2229 0a0a 2020 2020  p else "")..    
+000073f0: 2020 2020 2020 2020 7076 7320 2020 3d20          pvs   = 
+00007400: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00007410: 2020 2264 6973 706c 6179 6e61 6d65 223a    "displayname":
+00007420: 2068 746d 6c5f 6573 6361 7065 2872 702e   html_escape(rp.
+00007430: 7370 6c69 7428 222f 2229 5b2d 315d 292c  split("/")[-1]),
+00007440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007450: 2022 6765 746c 6173 746d 6f64 6966 6965   "getlastmodifie
+00007460: 6422 3a20 666f 726d 6174 6461 7465 2873  d": formatdate(s
+00007470: 742e 7374 5f6d 7469 6d65 2c20 7573 6567  t.st_mtime, useg
+00007480: 6d74 3d54 7275 6529 2c0a 2020 2020 2020  mt=True),.      
+00007490: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+000074a0: 7263 6574 7970 6522 3a20 273c 443a 636f  rcetype": '<D:co
+000074b0: 6c6c 6563 7469 6f6e 2078 6d6c 6e73 3a44  llection xmlns:D
+000074c0: 3d22 4441 563a 222f 3e27 2069 6620 6973  ="DAV:"/>' if is
+000074d0: 6469 7220 656c 7365 2022 222c 0a20 2020  dir else "",.   
+000074e0: 2020 2020 2020 2020 2020 2020 2022 7375               "su
+000074f0: 7070 6f72 7465 646c 6f63 6b22 3a20 273c  pportedlock": '<
+00007500: 443a 6c6f 636b 656e 7472 7920 786d 6c6e  D:lockentry xmln
+00007510: 733a 443d 2244 4156 3a22 3e3c 443a 6c6f  s:D="DAV:"><D:lo
+00007520: 636b 7363 6f70 653e 3c44 3a65 7863 6c75  ckscope><D:exclu
+00007530: 7369 7665 2f3e 3c2f 443a 6c6f 636b 7363  sive/></D:locksc
+00007540: 6f70 653e 3c44 3a6c 6f63 6b74 7970 653e  ope><D:locktype>
+00007550: 3c44 3a77 7269 7465 2f3e 3c2f 443a 6c6f  <D:write/></D:lo
+00007560: 636b 7479 7065 3e3c 2f44 3a6c 6f63 6b65  cktype></D:locke
+00007570: 6e74 7279 3e27 2c0a 2020 2020 2020 2020  ntry>',.        
+00007580: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00007590: 2020 6966 206e 6f74 2069 7364 6972 3a0a    if not isdir:.
+000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075b0: 7076 735b 2267 6574 636f 6e74 656e 7474  pvs["getcontentt
+000075c0: 7970 6522 5d20 3d20 6874 6d6c 5f65 7363  ype"] = html_esc
+000075d0: 6170 6528 6775 6573 735f 6d69 6d65 2872  ape(guess_mime(r
+000075e0: 7029 290a 2020 2020 2020 2020 2020 2020  p)).            
+000075f0: 2020 2020 7076 735b 2267 6574 636f 6e74      pvs["getcont
+00007600: 656e 746c 656e 6774 6822 5d20 3d20 7374  entlength"] = st
+00007610: 7228 7374 2e73 745f 7369 7a65 290a 0a20  r(st.st_size).. 
+00007620: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+00007630: 2c20 7620 696e 2070 7673 2e69 7465 6d73  , v in pvs.items
+00007640: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00007650: 2020 2020 6966 206b 206e 6f74 2069 6e20      if k not in 
+00007660: 7072 6f70 733a 0a20 2020 2020 2020 2020  props:.         
+00007670: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00007680: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+00007690: 2020 2020 656c 6966 2076 3a0a 2020 2020      elif v:.    
 000076a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076b0: 2020 2020 7265 7420 2b3d 2022 3c44 3a7b      ret += "<D:{
-000076c0: 307d 3e7b 317d 3c2f 443a 7b30 7d3e 222e  0}>{1}</D:{0}>".
-000076d0: 666f 726d 6174 286b 2c20 7629 0a20 2020  format(k, v).   
-000076e0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000076f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00007700: 2020 2020 2020 2072 6574 202b 3d20 223c         ret += "<
-00007710: 443a 7b7d 2f3e 222e 666f 726d 6174 286b  D:{}/>".format(k
-00007720: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00007730: 6574 202b 3d20 223c 2f44 3a70 726f 703e  et += "</D:prop>
-00007740: 3c44 3a73 7461 7475 733e 4854 5450 2f31  <D:status>HTTP/1
-00007750: 2e31 2032 3030 204f 4b3c 2f44 3a73 7461  .1 200 OK</D:sta
-00007760: 7475 733e 3c2f 443a 7072 6f70 7374 6174  tus></D:propstat
-00007770: 3e22 0a0a 2020 2020 2020 2020 2020 2020  >"..            
-00007780: 6d69 7373 696e 6720 3d20 5b22 3c44 3a7b  missing = ["<D:{
-00007790: 7d2f 3e22 2e66 6f72 6d61 7428 7829 2066  }/>".format(x) f
-000077a0: 6f72 2078 2069 6e20 7072 6f70 7320 6966  or x in props if
-000077b0: 2078 206e 6f74 2069 6e20 7076 735d 0a20   x not in pvs]. 
-000077c0: 2020 2020 2020 2020 2020 2069 6620 6d69             if mi
-000077d0: 7373 696e 6720 616e 6420 636c 656e 3a0a  ssing and clen:.
-000077e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077f0: 7420 3d20 223c 443a 7072 6f70 7374 6174  t = "<D:propstat
-00007800: 3e3c 443a 7072 6f70 3e7b 7d3c 2f44 3a70  ><D:prop>{}</D:p
-00007810: 726f 703e 3c44 3a73 7461 7475 733e 4854  rop><D:status>HT
-00007820: 5450 2f31 2e31 2034 3034 204e 6f74 2046  TP/1.1 404 Not F
-00007830: 6f75 6e64 3c2f 443a 7374 6174 7573 3e3c  ound</D:status><
-00007840: 2f44 3a70 726f 7073 7461 743e 220a 2020  /D:propstat>".  
-00007850: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00007860: 7420 2b3d 2074 2e66 6f72 6d61 7428 2222  t += t.format(""
-00007870: 2e6a 6f69 6e28 6d69 7373 696e 6729 290a  .join(missing)).
-00007880: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00007890: 202b 3d20 223c 2f44 3a72 6573 706f 6e73   += "</D:respons
-000078a0: 653e 220a 2020 2020 2020 2020 2020 2020  e>".            
-000078b0: 7768 696c 6520 6c65 6e28 7265 7429 203e  while len(ret) >
-000078c0: 3d20 6368 756e 6b73 7a3a 0a20 2020 2020  = chunksz:.     
-000078d0: 2020 2020 2020 2020 2020 2072 6574 203d             ret =
-000078e0: 2073 656c 662e 7365 6e64 5f63 6875 6e6b   self.send_chunk
-000078f0: 2872 6574 2c20 656e 632c 2063 6875 6e6b  (ret, enc, chunk
-00007900: 737a 290a 0a20 2020 2020 2020 2072 6574  sz)..        ret
-00007910: 202b 3d20 223c 2f44 3a6d 756c 7469 7374   += "</D:multist
-00007920: 6174 7573 3e22 0a20 2020 2020 2020 2077  atus>".        w
-00007930: 6869 6c65 2072 6574 3a0a 2020 2020 2020  hile ret:.      
-00007940: 2020 2020 2020 7265 7420 3d20 7365 6c66        ret = self
-00007950: 2e73 656e 645f 6368 756e 6b28 7265 742c  .send_chunk(ret,
-00007960: 2065 6e63 2c20 6368 756e 6b73 7a29 0a0a   enc, chunksz)..
-00007970: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00007980: 645f 6368 756e 6b28 2222 2c20 656e 632c  d_chunk("", enc,
-00007990: 2063 6875 6e6b 737a 290a 2020 2020 2020   chunksz).      
-000079a0: 2020 2320 7365 6c66 2e72 6570 6c79 2872    # self.reply(r
-000079b0: 6574 2e65 6e63 6f64 6528 656e 632c 2022  et.encode(enc, "
-000079c0: 7265 706c 6163 6522 292c 3230 372c 2022  replace"),207, "
-000079d0: 7465 7874 2f78 6d6c 3b20 6368 6172 7365  text/xml; charse
-000079e0: 743d 2220 2b20 656e 6329 0a20 2020 2020  t=" + enc).     
-000079f0: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00007a00: 2020 2020 6465 6620 6861 6e64 6c65 5f70      def handle_p
-00007a10: 726f 7070 6174 6368 2873 656c 6629 2020  roppatch(self)  
-00007a20: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00007a30: 662e 646f 5f6c 6f67 3a0a 2020 2020 2020  f.do_log:.      
-00007a40: 2020 2020 2020 7365 6c66 2e6c 6f67 2822        self.log("
-00007a50: 5050 4154 4348 2022 202b 2073 656c 662e  PPATCH " + self.
-00007a60: 7265 7129 0a0a 2020 2020 2020 2020 6966  req)..        if
-00007a70: 2073 656c 662e 6172 6773 2e6e 6f5f 6461   self.args.no_da
-00007a80: 763a 0a20 2020 2020 2020 2020 2020 2072  v:.            r
-00007a90: 6169 7365 2050 6562 6b61 6328 3430 352c  aise Pebkac(405,
-00007aa0: 2022 5765 6244 4156 2069 7320 6469 7361   "WebDAV is disa
-00007ab0: 626c 6564 2069 6e20 7365 7276 6572 2063  bled in server c
-00007ac0: 6f6e 6669 6722 290a 0a20 2020 2020 2020  onfig")..       
-00007ad0: 2069 6620 6e6f 7420 7365 6c66 2e63 616e   if not self.can
-00007ae0: 5f77 7269 7465 3a0a 2020 2020 2020 2020  _write:.        
-00007af0: 2020 2020 7365 6c66 2e6c 6f67 2822 7b7d      self.log("{}
-00007b00: 2074 7269 6564 2074 6f20 7072 6f70 7061   tried to proppa
-00007b10: 7463 6820 5b7b 7d5d 222e 666f 726d 6174  tch [{}]".format
-00007b20: 2873 656c 662e 756e 616d 652c 2073 656c  (self.uname, sel
-00007b30: 662e 7670 6174 6829 290a 2020 2020 2020  f.vpath)).      
-00007b40: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
-00007b50: 6163 2834 3031 2c20 2261 7574 6865 6e74  ac(401, "authent
-00007b60: 6963 6174 6522 290a 0a20 2020 2020 2020  icate")..       
-00007b70: 2066 726f 6d20 786d 6c2e 6574 7265 6520   from xml.etree 
-00007b80: 696d 706f 7274 2045 6c65 6d65 6e74 5472  import ElementTr
-00007b90: 6565 2061 7320 4554 0a0a 2020 2020 2020  ee as ET..      
-00007ba0: 2020 6672 6f6d 202e 6478 6d6c 2069 6d70    from .dxml imp
-00007bb0: 6f72 7420 6d6b 656e 6f64 2c20 6d6b 746e  ort mkenod, mktn
-00007bc0: 6f64 2c20 7061 7273 655f 786d 6c0a 0a20  od, parse_xml.. 
-00007bd0: 2020 2020 2020 2073 656c 662e 6173 7276         self.asrv
-00007be0: 2e76 6673 2e67 6574 2873 656c 662e 7670  .vfs.get(self.vp
-00007bf0: 6174 682c 2073 656c 662e 756e 616d 652c  ath, self.uname,
-00007c00: 2046 616c 7365 2c20 4661 6c73 6529 0a20   False, False). 
-00007c10: 2020 2020 2020 2023 2061 6273 7061 7468         # abspath
-00007c20: 203d 2076 6e2e 6463 616e 6f6e 6963 616c   = vn.dcanonical
-00007c30: 2872 656d 290a 0a20 2020 2020 2020 2062  (rem)..        b
-00007c40: 7566 203d 2062 2222 0a20 2020 2020 2020  uf = b"".       
-00007c50: 2066 6f72 2072 6275 6620 696e 2073 656c   for rbuf in sel
-00007c60: 662e 6765 745f 626f 6479 5f72 6561 6465  f.get_body_reade
-00007c70: 7228 295b 305d 3a0a 2020 2020 2020 2020  r()[0]:.        
-00007c80: 2020 2020 6275 6620 2b3d 2072 6275 660a      buf += rbuf.
-00007c90: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00007ca0: 6f74 2072 6275 6620 6f72 206c 656e 2862  ot rbuf or len(b
-00007cb0: 7566 2920 3e3d 2031 3238 202a 2031 3032  uf) >= 128 * 102
-00007cc0: 343a 0a20 2020 2020 2020 2020 2020 2020  4:.             
-00007cd0: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
-00007ce0: 2020 6966 2073 656c 662e 5f61 7070 6c65    if self._apple
-00007cf0: 7361 6e28 293a 0a20 2020 2020 2020 2020  san():.         
-00007d00: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00007d10: 2020 2020 2020 2020 7478 7420 3d20 6275          txt = bu
-00007d20: 662e 6465 636f 6465 2822 6173 6369 6922  f.decode("ascii"
-00007d30: 2c20 2272 6570 6c61 6365 2229 2e6c 6f77  , "replace").low
-00007d40: 6572 2829 0a20 2020 2020 2020 2065 6e63  er().        enc
-00007d50: 203d 2073 656c 662e 6765 745f 786d 6c5f   = self.get_xml_
-00007d60: 656e 6328 7478 7429 0a20 2020 2020 2020  enc(txt).       
-00007d70: 2075 656e 6320 3d20 656e 632e 7570 7065   uenc = enc.uppe
-00007d80: 7228 290a 0a20 2020 2020 2020 2074 7874  r()..        txt
-00007d90: 203d 2062 7566 2e64 6563 6f64 6528 656e   = buf.decode(en
-00007da0: 632c 2022 7265 706c 6163 6522 290a 2020  c, "replace").  
-00007db0: 2020 2020 2020 4554 2e72 6567 6973 7465        ET.registe
-00007dc0: 725f 6e61 6d65 7370 6163 6528 2244 222c  r_namespace("D",
-00007dd0: 2022 4441 563a 2229 0a20 2020 2020 2020   "DAV:").       
-00007de0: 2078 726f 6f74 203d 206d 6b65 6e6f 6428   xroot = mkenod(
-00007df0: 2244 3a6f 727a 2229 0a20 2020 2020 2020  "D:orz").       
-00007e00: 2078 726f 6f74 2e69 6e73 6572 7428 302c   xroot.insert(0,
-00007e10: 2070 6172 7365 5f78 6d6c 2874 7874 2929   parse_xml(txt))
-00007e20: 0a20 2020 2020 2020 2078 7072 6f70 203d  .        xprop =
-00007e30: 2078 726f 6f74 2e66 696e 6428 7222 2e2f   xroot.find(r"./
-00007e40: 7b44 4156 3a7d 7072 6f70 6572 7479 7570  {DAV:}propertyup
-00007e50: 6461 7465 2f7b 4441 563a 7d73 6574 2f7b  date/{DAV:}set/{
-00007e60: 4441 563a 7d70 726f 7022 290a 2020 2020  DAV:}prop").    
-00007e70: 2020 2020 6173 7365 7274 2078 7072 6f70      assert xprop
-00007e80: 0a20 2020 2020 2020 2066 6f72 207a 6520  .        for ze 
-00007e90: 696e 2078 7072 6f70 3a0a 2020 2020 2020  in xprop:.      
-00007ea0: 2020 2020 2020 7a65 2e63 6c65 6172 2829        ze.clear()
-00007eb0: 0a0a 2020 2020 2020 2020 7478 7420 3d20  ..        txt = 
-00007ec0: 2222 223c 6d75 6c74 6973 7461 7475 7320  """<multistatus 
-00007ed0: 786d 6c6e 733d 2244 4156 3a22 3e3c 7265  xmlns="DAV:"><re
-00007ee0: 7370 6f6e 7365 3e3c 7072 6f70 7374 6174  sponse><propstat
-00007ef0: 3e3c 7374 6174 7573 3e48 5454 502f 312e  ><status>HTTP/1.
-00007f00: 3120 3430 3320 466f 7262 6964 6465 6e3c  1 403 Forbidden<
-00007f10: 2f73 7461 7475 733e 3c2f 7072 6f70 7374  /status></propst
-00007f20: 6174 3e3c 2f72 6573 706f 6e73 653e 3c2f  at></response></
-00007f30: 6d75 6c74 6973 7461 7475 733e 2222 220a  multistatus>""".
-00007f40: 2020 2020 2020 2020 7872 6f6f 7420 3d20          xroot = 
-00007f50: 7061 7273 655f 786d 6c28 7478 7429 0a0a  parse_xml(txt)..
-00007f60: 2020 2020 2020 2020 656c 203d 2078 726f          el = xro
-00007f70: 6f74 2e66 696e 6428 7222 2e2f 7b44 4156  ot.find(r"./{DAV
-00007f80: 3a7d 7265 7370 6f6e 7365 2229 0a20 2020  :}response").   
-00007f90: 2020 2020 2061 7373 6572 7420 656c 0a20       assert el. 
-00007fa0: 2020 2020 2020 2065 3220 3d20 6d6b 746e         e2 = mktn
-00007fb0: 6f64 2822 443a 6872 6566 222c 2071 756f  od("D:href", quo
-00007fc0: 7465 7028 7365 6c66 2e61 7267 732e 5352  tep(self.args.SR
-00007fd0: 5320 2b20 7365 6c66 2e76 7061 7468 2929  S + self.vpath))
-00007fe0: 0a20 2020 2020 2020 2065 6c2e 696e 7365  .        el.inse
-00007ff0: 7274 2830 2c20 6532 290a 0a20 2020 2020  rt(0, e2)..     
-00008000: 2020 2065 6c20 3d20 7872 6f6f 742e 6669     el = xroot.fi
-00008010: 6e64 2872 222e 2f7b 4441 563a 7d72 6573  nd(r"./{DAV:}res
-00008020: 706f 6e73 652f 7b44 4156 3a7d 7072 6f70  ponse/{DAV:}prop
-00008030: 7374 6174 2229 0a20 2020 2020 2020 2061  stat").        a
-00008040: 7373 6572 7420 656c 0a20 2020 2020 2020  ssert el.       
-00008050: 2065 6c2e 696e 7365 7274 2830 2c20 7870   el.insert(0, xp
-00008060: 726f 7029 0a0a 2020 2020 2020 2020 7265  rop)..        re
-00008070: 7420 3d20 273c 3f78 6d6c 2076 6572 7369  t = '<?xml versi
-00008080: 6f6e 3d22 312e 3022 2065 6e63 6f64 696e  on="1.0" encodin
-00008090: 673d 227b 7d22 3f3e 5c6e 272e 666f 726d  g="{}"?>\n'.form
-000080a0: 6174 2875 656e 6329 0a20 2020 2020 2020  at(uenc).       
-000080b0: 2072 6574 202b 3d20 4554 2e74 6f73 7472   ret += ET.tostr
-000080c0: 696e 6728 7872 6f6f 7429 2e64 6563 6f64  ing(xroot).decod
-000080d0: 6528 2275 7466 2d38 2229 0a0a 2020 2020  e("utf-8")..    
-000080e0: 2020 2020 7365 6c66 2e72 6570 6c79 2872      self.reply(r
-000080f0: 6574 2e65 6e63 6f64 6528 656e 632c 2022  et.encode(enc, "
-00008100: 7265 706c 6163 6522 292c 2032 3037 2c20  replace"), 207, 
-00008110: 2274 6578 742f 786d 6c3b 2063 6861 7273  "text/xml; chars
-00008120: 6574 3d22 202b 2065 6e63 290a 2020 2020  et=" + enc).    
-00008130: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-00008140: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
-00008150: 6c6f 636b 2873 656c 6629 2020 3a0a 2020  lock(self)  :.  
-00008160: 2020 2020 2020 6966 2073 656c 662e 646f        if self.do
-00008170: 5f6c 6f67 3a0a 2020 2020 2020 2020 2020  _log:.          
-00008180: 2020 7365 6c66 2e6c 6f67 2822 4c4f 434b    self.log("LOCK
-00008190: 2022 202b 2073 656c 662e 7265 7129 0a0a   " + self.req)..
-000081a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000081b0: 6172 6773 2e6e 6f5f 6461 763a 0a20 2020  args.no_dav:.   
-000081c0: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
-000081d0: 6562 6b61 6328 3430 352c 2022 5765 6244  ebkac(405, "WebD
-000081e0: 4156 2069 7320 6469 7361 626c 6564 2069  AV is disabled i
-000081f0: 6e20 7365 7276 6572 2063 6f6e 6669 6722  n server config"
-00008200: 290a 0a20 2020 2020 2020 2023 2077 696e  )..        # win
-00008210: 372b 2064 6561 646c 6f63 6b73 2069 6620  7+ deadlocks if 
-00008220: 7765 2073 6179 206e 6f3b 206a 7573 7420  we say no; just 
-00008230: 736d 696c 6520 616e 6420 6e6f 640a 2020  smile and nod.  
-00008240: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00008250: 662e 6361 6e5f 7772 6974 6520 616e 6420  f.can_write and 
-00008260: 224d 6963 726f 736f 6674 2d57 6562 4441  "Microsoft-WebDA
-00008270: 5622 206e 6f74 2069 6e20 7365 6c66 2e75  V" not in self.u
-00008280: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
-00008290: 656c 662e 6c6f 6728 227b 7d20 7472 6965  elf.log("{} trie
-000082a0: 6420 746f 206c 6f63 6b20 5b7b 7d5d 222e  d to lock [{}]".
-000082b0: 666f 726d 6174 2873 656c 662e 756e 616d  format(self.unam
-000082c0: 652c 2073 656c 662e 7670 6174 6829 290a  e, self.vpath)).
-000082d0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000082e0: 6520 5065 626b 6163 2834 3031 2c20 2261  e Pebkac(401, "a
-000082f0: 7574 6865 6e74 6963 6174 6522 290a 0a20  uthenticate").. 
-00008300: 2020 2020 2020 2066 726f 6d20 786d 6c2e         from xml.
-00008310: 6574 7265 6520 696d 706f 7274 2045 6c65  etree import Ele
-00008320: 6d65 6e74 5472 6565 2061 7320 4554 0a0a  mentTree as ET..
-00008330: 2020 2020 2020 2020 6672 6f6d 202e 6478          from .dx
-00008340: 6d6c 2069 6d70 6f72 7420 6d6b 656e 6f64  ml import mkenod
-00008350: 2c20 6d6b 746e 6f64 2c20 7061 7273 655f  , mktnod, parse_
-00008360: 786d 6c0a 0a20 2020 2020 2020 2076 6e2c  xml..        vn,
-00008370: 2072 656d 203d 2073 656c 662e 6173 7276   rem = self.asrv
-00008380: 2e76 6673 2e67 6574 2873 656c 662e 7670  .vfs.get(self.vp
-00008390: 6174 682c 2073 656c 662e 756e 616d 652c  ath, self.uname,
-000083a0: 2046 616c 7365 2c20 4661 6c73 6529 0a20   False, False). 
-000083b0: 2020 2020 2020 2061 6273 7061 7468 203d         abspath =
-000083c0: 2076 6e2e 6463 616e 6f6e 6963 616c 2872   vn.dcanonical(r
-000083d0: 656d 290a 0a20 2020 2020 2020 2062 7566  em)..        buf
-000083e0: 203d 2062 2222 0a20 2020 2020 2020 2066   = b"".        f
-000083f0: 6f72 2072 6275 6620 696e 2073 656c 662e  or rbuf in self.
-00008400: 6765 745f 626f 6479 5f72 6561 6465 7228  get_body_reader(
-00008410: 295b 305d 3a0a 2020 2020 2020 2020 2020  )[0]:.          
-00008420: 2020 6275 6620 2b3d 2072 6275 660a 2020    buf += rbuf.  
-00008430: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00008440: 2072 6275 6620 6f72 206c 656e 2862 7566   rbuf or len(buf
-00008450: 2920 3e3d 2031 3238 202a 2031 3032 343a  ) >= 128 * 1024:
-00008460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008470: 2062 7265 616b 0a0a 2020 2020 2020 2020   break..        
-00008480: 6966 2073 656c 662e 5f61 7070 6c65 7361  if self._applesa
-00008490: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
-000084a0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-000084b0: 2020 2020 2020 7478 7420 3d20 6275 662e        txt = buf.
-000084c0: 6465 636f 6465 2822 6173 6369 6922 2c20  decode("ascii", 
-000084d0: 2272 6570 6c61 6365 2229 2e6c 6f77 6572  "replace").lower
-000084e0: 2829 0a20 2020 2020 2020 2065 6e63 203d  ().        enc =
-000084f0: 2073 656c 662e 6765 745f 786d 6c5f 656e   self.get_xml_en
-00008500: 6328 7478 7429 0a20 2020 2020 2020 2075  c(txt).        u
-00008510: 656e 6320 3d20 656e 632e 7570 7065 7228  enc = enc.upper(
-00008520: 290a 0a20 2020 2020 2020 2074 7874 203d  )..        txt =
-00008530: 2062 7566 2e64 6563 6f64 6528 656e 632c   buf.decode(enc,
-00008540: 2022 7265 706c 6163 6522 290a 2020 2020   "replace").    
-00008550: 2020 2020 4554 2e72 6567 6973 7465 725f      ET.register_
-00008560: 6e61 6d65 7370 6163 6528 2244 222c 2022  namespace("D", "
-00008570: 4441 563a 2229 0a20 2020 2020 2020 206c  DAV:").        l
-00008580: 6b20 3d20 7061 7273 655f 786d 6c28 7478  k = parse_xml(tx
-00008590: 7429 0a20 2020 2020 2020 2061 7373 6572  t).        asser
-000085a0: 7420 6c6b 2e74 6167 203d 3d20 227b 4441  t lk.tag == "{DA
-000085b0: 563a 7d6c 6f63 6b69 6e66 6f22 0a0a 2020  V:}lockinfo"..  
-000085c0: 2020 2020 2020 746f 6b65 6e20 3d20 7374        token = st
-000085d0: 7228 7575 6964 2e75 7569 6434 2829 290a  r(uuid.uuid4()).
-000085e0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000085f0: 6c6b 2e66 696e 6428 7222 2e2f 7b44 4156  lk.find(r"./{DAV
-00008600: 3a7d 6465 7074 6822 293a 0a20 2020 2020  :}depth"):.     
-00008610: 2020 2020 2020 2064 6570 7468 203d 2073         depth = s
-00008620: 656c 662e 6865 6164 6572 732e 6765 7428  elf.headers.get(
-00008630: 2264 6570 7468 222c 2022 696e 6669 6e69  "depth", "infini
-00008640: 7479 2229 0a20 2020 2020 2020 2020 2020  ty").           
-00008650: 206c 6b2e 6170 7065 6e64 286d 6b74 6e6f   lk.append(mktno
-00008660: 6428 2244 3a64 6570 7468 222c 2064 6570  d("D:depth", dep
-00008670: 7468 2929 0a0a 2020 2020 2020 2020 6c6b  th))..        lk
-00008680: 2e61 7070 656e 6428 6d6b 746e 6f64 2822  .append(mktnod("
-00008690: 443a 7469 6d65 6f75 7422 2c20 2253 6563  D:timeout", "Sec
-000086a0: 6f6e 642d 3333 3130 2229 290a 2020 2020  ond-3310")).    
-000086b0: 2020 2020 6c6b 2e61 7070 656e 6428 6d6b      lk.append(mk
-000086c0: 656e 6f64 2822 443a 6c6f 636b 746f 6b65  enod("D:locktoke
-000086d0: 6e22 2c20 6d6b 746e 6f64 2822 443a 6872  n", mktnod("D:hr
-000086e0: 6566 222c 2074 6f6b 656e 2929 290a 2020  ef", token))).  
-000086f0: 2020 2020 2020 6c6b 2e61 7070 656e 6428        lk.append(
-00008700: 0a20 2020 2020 2020 2020 2020 206d 6b65  .            mke
-00008710: 6e6f 6428 2244 3a6c 6f63 6b72 6f6f 7422  nod("D:lockroot"
-00008720: 2c20 6d6b 746e 6f64 2822 443a 6872 6566  , mktnod("D:href
-00008730: 222c 2071 756f 7465 7028 7365 6c66 2e61  ", quotep(self.a
-00008740: 7267 732e 5352 5320 2b20 7365 6c66 2e76  rgs.SRS + self.v
-00008750: 7061 7468 2929 290a 2020 2020 2020 2020  path))).        
-00008760: 290a 0a20 2020 2020 2020 206c 6b32 203d  )..        lk2 =
-00008770: 206d 6b65 6e6f 6428 2244 3a61 6374 6976   mkenod("D:activ
-00008780: 656c 6f63 6b22 290a 2020 2020 2020 2020  elock").        
-00008790: 7872 6f6f 7420 3d20 6d6b 656e 6f64 2822  xroot = mkenod("
-000087a0: 443a 7072 6f70 222c 206d 6b65 6e6f 6428  D:prop", mkenod(
-000087b0: 2244 3a6c 6f63 6b64 6973 636f 7665 7279  "D:lockdiscovery
-000087c0: 222c 206c 6b32 2929 0a20 2020 2020 2020  ", lk2)).       
-000087d0: 2066 6f72 2061 2069 6e20 6c6b 3a0a 2020   for a in lk:.  
-000087e0: 2020 2020 2020 2020 2020 6c6b 322e 6170            lk2.ap
-000087f0: 7065 6e64 2861 290a 0a20 2020 2020 2020  pend(a)..       
-00008800: 2072 6574 203d 2027 3c3f 786d 6c20 7665   ret = '<?xml ve
-00008810: 7273 696f 6e3d 2231 2e30 2220 656e 636f  rsion="1.0" enco
-00008820: 6469 6e67 3d22 7b7d 223f 3e5c 6e27 2e66  ding="{}"?>\n'.f
-00008830: 6f72 6d61 7428 7565 6e63 290a 2020 2020  ormat(uenc).    
-00008840: 2020 2020 7265 7420 2b3d 2045 542e 746f      ret += ET.to
-00008850: 7374 7269 6e67 2878 726f 6f74 292e 6465  string(xroot).de
-00008860: 636f 6465 2822 7574 662d 3822 290a 0a20  code("utf-8").. 
-00008870: 2020 2020 2020 2072 6320 3d20 3230 300a         rc = 200.
-00008880: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00008890: 6361 6e5f 7772 6974 6520 616e 6420 6e6f  can_write and no
-000088a0: 7420 626f 732e 7061 7468 2e69 7366 696c  t bos.path.isfil
-000088b0: 6528 6162 7370 6174 6829 3a0a 2020 2020  e(abspath):.    
-000088c0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-000088d0: 6e28 6673 656e 6328 6162 7370 6174 6829  n(fsenc(abspath)
-000088e0: 2c20 2277 6222 2920 6173 205f 3a0a 2020  , "wb") as _:.  
-000088f0: 2020 2020 2020 2020 2020 2020 2020 7263                rc
-00008900: 203d 2032 3031 0a0a 2020 2020 2020 2020   = 201..        
-00008910: 7365 6c66 2e6f 7574 5f68 6561 6465 7273  self.out_headers
-00008920: 5b22 4c6f 636b 2d54 6f6b 656e 225d 203d  ["Lock-Token"] =
-00008930: 2022 3c7b 7d3e 222e 666f 726d 6174 2874   "<{}>".format(t
-00008940: 6f6b 656e 290a 2020 2020 2020 2020 7365  oken).        se
-00008950: 6c66 2e72 6570 6c79 2872 6574 2e65 6e63  lf.reply(ret.enc
-00008960: 6f64 6528 656e 632c 2022 7265 706c 6163  ode(enc, "replac
-00008970: 6522 292c 2072 632c 2022 7465 7874 2f78  e"), rc, "text/x
-00008980: 6d6c 3b20 6368 6172 7365 743d 2220 2b20  ml; charset=" + 
-00008990: 656e 6329 0a20 2020 2020 2020 2072 6574  enc).        ret
-000089a0: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
-000089b0: 6620 6861 6e64 6c65 5f75 6e6c 6f63 6b28  f handle_unlock(
-000089c0: 7365 6c66 2920 203a 0a20 2020 2020 2020  self)  :.       
-000089d0: 2069 6620 7365 6c66 2e64 6f5f 6c6f 673a   if self.do_log:
-000089e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000089f0: 662e 6c6f 6728 2255 4e4c 4f43 4b20 2220  f.log("UNLOCK " 
-00008a00: 2b20 7365 6c66 2e72 6571 290a 0a20 2020  + self.req)..   
-00008a10: 2020 2020 2069 6620 7365 6c66 2e61 7267       if self.arg
-00008a20: 732e 6e6f 5f64 6176 3a0a 2020 2020 2020  s.no_dav:.      
-00008a30: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
-00008a40: 6163 2834 3035 2c20 2257 6562 4441 5620  ac(405, "WebDAV 
-00008a50: 6973 2064 6973 6162 6c65 6420 696e 2073  is disabled in s
-00008a60: 6572 7665 7220 636f 6e66 6967 2229 0a0a  erver config")..
-00008a70: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00008a80: 656c 662e 6361 6e5f 7772 6974 6520 616e  elf.can_write an
-00008a90: 6420 224d 6963 726f 736f 6674 2d57 6562  d "Microsoft-Web
-00008aa0: 4441 5622 206e 6f74 2069 6e20 7365 6c66  DAV" not in self
-00008ab0: 2e75 613a 0a20 2020 2020 2020 2020 2020  .ua:.           
-00008ac0: 2073 656c 662e 6c6f 6728 227b 7d20 7472   self.log("{} tr
-00008ad0: 6965 6420 746f 206c 6f63 6b20 5b7b 7d5d  ied to lock [{}]
-00008ae0: 222e 666f 726d 6174 2873 656c 662e 756e  ".format(self.un
-00008af0: 616d 652c 2073 656c 662e 7670 6174 6829  ame, self.vpath)
-00008b00: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
-00008b10: 6973 6520 5065 626b 6163 2834 3031 2c20  ise Pebkac(401, 
-00008b20: 2261 7574 6865 6e74 6963 6174 6522 290a  "authenticate").
-00008b30: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00008b40: 6e64 5f68 6561 6465 7273 284e 6f6e 652c  nd_headers(None,
-00008b50: 2032 3034 290a 2020 2020 2020 2020 7265   204).        re
-00008b60: 7475 726e 2054 7275 650a 0a20 2020 2064  turn True..    d
-00008b70: 6566 2068 616e 646c 655f 6d6b 636f 6c28  ef handle_mkcol(
-00008b80: 7365 6c66 2920 203a 0a20 2020 2020 2020  self)  :.       
-00008b90: 2069 6620 7365 6c66 2e5f 6170 706c 6573   if self._apples
-00008ba0: 616e 2829 3a0a 2020 2020 2020 2020 2020  an():.          
-00008bb0: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
-00008bc0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00008bd0: 6f5f 6c6f 673a 0a20 2020 2020 2020 2020  o_log:.         
-00008be0: 2020 2073 656c 662e 6c6f 6728 224d 4b43     self.log("MKC
-00008bf0: 4f4c 2022 202b 2073 656c 662e 7265 7129  OL " + self.req)
-00008c00: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00008c10: 2073 656c 662e 5f6d 6b64 6972 2873 656c   self._mkdir(sel
-00008c20: 662e 7670 6174 6829 0a0a 2020 2020 6465  f.vpath)..    de
-00008c30: 6620 6861 6e64 6c65 5f6d 6f76 6528 7365  f handle_move(se
-00008c40: 6c66 2920 203a 0a20 2020 2020 2020 2064  lf)  :.        d
-00008c50: 7374 203d 2073 656c 662e 6865 6164 6572  st = self.header
-00008c60: 735b 2264 6573 7469 6e61 7469 6f6e 225d  s["destination"]
-00008c70: 0a20 2020 2020 2020 2064 7374 203d 2072  .        dst = r
-00008c80: 652e 7375 6228 225e 6874 7470 733f 3a2f  e.sub("^https?:/
-00008c90: 2f5b 5e2f 5d2b 222c 2022 222c 2064 7374  /[^/]+", "", dst
-00008ca0: 292e 6c73 7472 6970 2829 0a20 2020 2020  ).lstrip().     
-00008cb0: 2020 2064 7374 203d 2075 6e71 756f 7465     dst = unquote
-00008cc0: 7028 6473 7429 0a20 2020 2020 2020 2069  p(dst).        i
-00008cd0: 6620 6e6f 7420 7365 6c66 2e5f 6d76 2873  f not self._mv(s
-00008ce0: 656c 662e 7670 6174 682c 2064 7374 293a  elf.vpath, dst):
-00008cf0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00008d00: 7572 6e20 4661 6c73 650a 0a20 2020 2020  urn False..     
-00008d10: 2020 2023 2075 7032 6b20 6f6e 6c79 2063     # up2k only c
-00008d20: 6172 6573 2061 626f 7574 2066 696c 6573  ares about files
-00008d30: 2061 6e64 2072 656d 6f76 6573 2061 6c6c   and removes all
-00008d40: 2065 6d70 7479 2066 6f6c 6465 7273 3b0a   empty folders;.
-00008d50: 2020 2020 2020 2020 2320 636c 6965 6e74          # client
-00008d60: 7320 6e61 7475 7261 6c6c 7920 6578 7065  s naturally expe
-00008d70: 6374 2065 6d70 7479 2066 6f6c 6465 7273  ct empty folders
-00008d80: 2074 6f20 7375 7276 6976 6520 6120 7265   to survive a re
-00008d90: 6e61 6d65 0a20 2020 2020 2020 2076 6e2c  name.        vn,
-00008da0: 2072 656d 203d 2073 656c 662e 6173 7276   rem = self.asrv
-00008db0: 2e76 6673 2e67 6574 2864 7374 2c20 7365  .vfs.get(dst, se
-00008dc0: 6c66 2e75 6e61 6d65 2c20 4661 6c73 652c  lf.uname, False,
-00008dd0: 2046 616c 7365 290a 2020 2020 2020 2020   False).        
-00008de0: 6461 6273 203d 2076 6e2e 6361 6e6f 6e69  dabs = vn.canoni
-00008df0: 6361 6c28 7265 6d29 0a20 2020 2020 2020  cal(rem).       
-00008e00: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00008e10: 2020 626f 732e 6d61 6b65 6469 7273 2864    bos.makedirs(d
-00008e20: 6162 7329 0a20 2020 2020 2020 2065 7863  abs).        exc
-00008e30: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-00008e40: 2070 6173 730a 0a20 2020 2020 2020 2072   pass..        r
-00008e50: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-00008e60: 6465 6620 5f61 7070 6c65 7361 6e28 7365  def _applesan(se
-00008e70: 6c66 2920 203a 0a20 2020 2020 2020 2069  lf)  :.        i
-00008e80: 6620 7365 6c66 2e61 7267 732e 6461 765f  f self.args.dav_
-00008e90: 6d61 6320 6f72 2022 4461 7277 696e 2f22  mac or "Darwin/"
-00008ea0: 206e 6f74 2069 6e20 7365 6c66 2e75 613a   not in self.ua:
-00008eb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00008ec0: 7572 6e20 4661 6c73 650a 0a20 2020 2020  urn False..     
-00008ed0: 2020 2076 7020 3d20 222f 2220 2b20 7365     vp = "/" + se
-00008ee0: 6c66 2e76 7061 7468 0a20 2020 2020 2020  lf.vpath.       
-00008ef0: 2070 746e 203d 2072 222f 5c2e 285f 7c44   ptn = r"/\.(_|D
-00008f00: 535f 5374 6f72 657c 5370 6f74 6c69 6768  S_Store|Spotligh
-00008f10: 742d 7c66 7365 7665 6e74 7364 7c54 7261  t-|fseventsd|Tra
-00008f20: 7368 6573 7c41 7070 6c65 446f 7562 6c65  shes|AppleDouble
-00008f30: 297c 2f5f 5f4d 4143 4f53 220a 2020 2020  )|/__MACOS".    
-00008f40: 2020 2020 6966 2072 652e 7365 6172 6368      if re.search
-00008f50: 2870 746e 2c20 7670 293a 0a20 2020 2020  (ptn, vp):.     
-00008f60: 2020 2020 2020 207a 7420 3d20 273c 3f78         zt = '<?x
-00008f70: 6d6c 2076 6572 7369 6f6e 3d22 312e 3022  ml version="1.0"
-00008f80: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
-00008f90: 223f 3e5c 6e3c 443a 6572 726f 7220 786d  "?>\n<D:error xm
-00008fa0: 6c6e 733a 443d 2244 4156 3a22 3e3c 443a  lns:D="DAV:"><D:
-00008fb0: 6c6f 636b 2d74 6f6b 656e 2d73 7562 6d69  lock-token-submi
-00008fc0: 7474 6564 3e3c 443a 6872 6566 3e7b 7d3c  tted><D:href>{}<
-00008fd0: 2f44 3a68 7265 663e 3c2f 443a 6c6f 636b  /D:href></D:lock
-00008fe0: 2d74 6f6b 656e 2d73 7562 6d69 7474 6564  -token-submitted
-00008ff0: 3e3c 2f44 3a65 7272 6f72 3e27 0a20 2020  ></D:error>'.   
-00009000: 2020 2020 2020 2020 207a 6220 3d20 7a74           zb = zt
-00009010: 2e66 6f72 6d61 7428 7670 292e 656e 636f  .format(vp).enco
-00009020: 6465 2822 7574 662d 3822 2c20 2272 6570  de("utf-8", "rep
-00009030: 6c61 6365 2229 0a20 2020 2020 2020 2020  lace").         
-00009040: 2020 2073 656c 662e 7265 706c 7928 7a62     self.reply(zb
-00009050: 2c20 3432 332c 2022 7465 7874 2f78 6d6c  , 423, "text/xml
-00009060: 3b20 6368 6172 7365 743d 7574 662d 3822  ; charset=utf-8"
-00009070: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00009080: 7475 726e 2054 7275 650a 0a20 2020 2020  turn True..     
-00009090: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-000090a0: 0a20 2020 2064 6566 2073 656e 645f 6368  .    def send_ch
-000090b0: 756e 6b28 7365 6c66 2c20 7478 7420 2c20  unk(self, txt , 
-000090c0: 656e 6320 2c20 626d 6178 2029 2020 3a0a  enc , bmax )  :.
-000090d0: 2020 2020 2020 2020 6f72 6967 5f6c 656e          orig_len
-000090e0: 203d 206c 656e 2874 7874 290a 2020 2020   = len(txt).    
-000090f0: 2020 2020 6275 6620 3d20 7478 745b 3a62      buf = txt[:b
-00009100: 6d61 785d 2e65 6e63 6f64 6528 656e 632c  max].encode(enc,
-00009110: 2022 7265 706c 6163 6522 295b 3a62 6d61   "replace")[:bma
-00009120: 785d 0a20 2020 2020 2020 2074 7279 3a0a  x].        try:.
-00009130: 2020 2020 2020 2020 2020 2020 5f20 3d20              _ = 
-00009140: 6275 662e 6465 636f 6465 2865 6e63 290a  buf.decode(enc).
-00009150: 2020 2020 2020 2020 6578 6365 7074 2055          except U
-00009160: 6e69 636f 6465 4465 636f 6465 4572 726f  nicodeDecodeErro
-00009170: 7220 6173 2075 6465 3a0a 2020 2020 2020  r as ude:.      
-00009180: 2020 2020 2020 6275 6620 3d20 6275 665b        buf = buf[
-00009190: 3a20 7564 652e 7374 6172 745d 0a0a 2020  : ude.start]..  
-000091a0: 2020 2020 2020 7478 7420 3d20 7478 745b        txt = txt[
-000091b0: 6c65 6e28 6275 662e 6465 636f 6465 2865  len(buf.decode(e
-000091c0: 6e63 2929 203a 5d0a 2020 2020 2020 2020  nc)) :].        
-000091d0: 6966 2074 7874 2061 6e64 206c 656e 2874  if txt and len(t
-000091e0: 7874 2920 3d3d 206f 7269 675f 6c65 6e3a  xt) == orig_len:
-000091f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00009200: 7365 2050 6562 6b61 6328 3530 302c 2022  se Pebkac(500, "
-00009210: 6368 756e 6b20 736c 6963 696e 6720 6661  chunk slicing fa
-00009220: 696c 6564 2229 0a0a 2020 2020 2020 2020  iled")..        
-00009230: 6275 6620 3d20 227b 3a78 7d5c 725c 6e22  buf = "{:x}\r\n"
-00009240: 2e66 6f72 6d61 7428 6c65 6e28 6275 6629  .format(len(buf)
-00009250: 292e 656e 636f 6465 2865 6e63 2920 2b20  ).encode(enc) + 
-00009260: 6275 660a 2020 2020 2020 2020 7365 6c66  buf.        self
-00009270: 2e73 2e73 656e 6461 6c6c 2862 7566 202b  .s.sendall(buf +
-00009280: 2062 225c 725c 6e22 290a 2020 2020 2020   b"\r\n").      
-00009290: 2020 7265 7475 726e 2074 7874 0a0a 2020    return txt..  
-000092a0: 2020 6465 6620 6861 6e64 6c65 5f6f 7074    def handle_opt
-000092b0: 696f 6e73 2873 656c 6629 2020 3a0a 2020  ions(self)  :.  
-000092c0: 2020 2020 2020 6966 2073 656c 662e 646f        if self.do
-000092d0: 5f6c 6f67 3a0a 2020 2020 2020 2020 2020  _log:.          
-000092e0: 2020 7365 6c66 2e6c 6f67 2822 4f50 5449    self.log("OPTI
-000092f0: 4f4e 5320 2220 2b20 7365 6c66 2e72 6571  ONS " + self.req
-00009300: 290a 0a20 2020 2020 2020 206f 6820 3d20  )..        oh = 
-00009310: 7365 6c66 2e6f 7574 5f68 6561 6465 7273  self.out_headers
-00009320: 0a20 2020 2020 2020 206f 685b 2241 6c6c  .        oh["All
-00009330: 6f77 225d 203d 2022 2c20 222e 6a6f 696e  ow"] = ", ".join
-00009340: 2873 656c 662e 636f 6e6e 2e68 7372 762e  (self.conn.hsrv.
-00009350: 6d61 6c6c 6f77 290a 0a20 2020 2020 2020  mallow)..       
-00009360: 2069 6620 6e6f 7420 7365 6c66 2e61 7267   if not self.arg
-00009370: 732e 6e6f 5f64 6176 3a0a 2020 2020 2020  s.no_dav:.      
-00009380: 2020 2020 2020 2320 5052 4f50 5041 5443        # PROPPATC
-00009390: 482c 204c 4f43 4b2c 2055 4e4c 4f43 4b2c  H, LOCK, UNLOCK,
-000093a0: 2043 4f50 593a 206e 6f6f 7020 2873 7065   COPY: noop (spe
-000093b0: 632d 6d75 7374 290a 2020 2020 2020 2020  c-must).        
-000093c0: 2020 2020 6f68 5b22 4461 7622 5d20 3d20      oh["Dav"] = 
-000093d0: 2231 2c20 3222 0a20 2020 2020 2020 2020  "1, 2".         
-000093e0: 2020 206f 685b 224d 732d 4175 7468 6f72     oh["Ms-Author
-000093f0: 2d56 6961 225d 203d 2022 4441 5622 0a0a  -Via"] = "DAV"..
-00009400: 2020 2020 2020 2020 2320 7769 6e78 702d          # winxp-
-00009410: 7765 6264 6176 2064 6f65 736e 7420 6b6e  webdav doesnt kn
-00009420: 6f77 2077 6861 7420 3230 3420 6973 0a20  ow what 204 is. 
-00009430: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-00009440: 5f68 6561 6465 7273 2830 2c20 3230 3029  _headers(0, 200)
-00009450: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009460: 5472 7565 0a0a 2020 2020 6465 6620 6861  True..    def ha
-00009470: 6e64 6c65 5f64 656c 6574 6528 7365 6c66  ndle_delete(self
-00009480: 2920 203a 0a20 2020 2020 2020 2073 656c  )  :.        sel
-00009490: 662e 6c6f 6728 2244 454c 4554 4520 2220  f.log("DELETE " 
-000094a0: 2b20 7365 6c66 2e72 6571 290a 2020 2020  + self.req).    
-000094b0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000094c0: 6861 6e64 6c65 5f72 6d28 5b5d 290a 0a20  handle_rm([]).. 
-000094d0: 2020 2064 6566 2068 616e 646c 655f 7075     def handle_pu
-000094e0: 7428 7365 6c66 2920 203a 0a20 2020 2020  t(self)  :.     
-000094f0: 2020 2073 656c 662e 6c6f 6728 2250 5554     self.log("PUT
-00009500: 2022 202b 2073 656c 662e 7265 7129 0a0a   " + self.req)..
-00009510: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00009520: 656c 662e 6361 6e5f 7772 6974 653a 0a20  elf.can_write:. 
-00009530: 2020 2020 2020 2020 2020 2074 203d 2022             t = "
-00009540: 7573 6572 207b 7d20 646f 6573 206e 6f74  user {} does not
-00009550: 2068 6176 6520 7772 6974 652d 6163 6365   have write-acce
-00009560: 7373 2068 6572 6522 0a20 2020 2020 2020  ss here".       
-00009570: 2020 2020 2072 6169 7365 2050 6562 6b61       raise Pebka
-00009580: 6328 3430 332c 2074 2e66 6f72 6d61 7428  c(403, t.format(
-00009590: 7365 6c66 2e75 6e61 6d65 2929 0a0a 2020  self.uname))..  
-000095a0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-000095b0: 662e 6172 6773 2e6e 6f5f 6461 7620 616e  f.args.no_dav an
-000095c0: 6420 7365 6c66 2e5f 6170 706c 6573 616e  d self._applesan
-000095d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000095e0: 7265 7475 726e 2073 656c 662e 6865 6164  return self.head
-000095f0: 6572 732e 6765 7428 2263 6f6e 7465 6e74  ers.get("content
-00009600: 2d6c 656e 6774 6822 2920 3d3d 2022 3022  -length") == "0"
-00009610: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00009620: 662e 6865 6164 6572 732e 6765 7428 2265  f.headers.get("e
-00009630: 7870 6563 7422 2c20 2222 292e 6c6f 7765  xpect", "").lowe
-00009640: 7228 2920 3d3d 2022 3130 302d 636f 6e74  r() == "100-cont
-00009650: 696e 7565 223a 0a20 2020 2020 2020 2020  inue":.         
-00009660: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00009670: 2020 2020 2020 2020 7365 6c66 2e73 2e73          self.s.s
-00009680: 6574 7469 6d65 6f75 7428 4e6f 6e65 290a  ettimeout(None).
-00009690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096a0: 7365 6c66 2e73 2e73 656e 6461 6c6c 2862  self.s.sendall(b
-000096b0: 2248 5454 502f 312e 3120 3130 3020 436f  "HTTP/1.1 100 Co
-000096c0: 6e74 696e 7565 5c72 5c6e 5c72 5c6e 2229  ntinue\r\n\r\n")
-000096d0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-000096e0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-000096f0: 2020 2020 2072 6169 7365 2050 6562 6b61       raise Pebka
-00009700: 6328 3430 302c 2022 636c 6965 6e74 2064  c(400, "client d
-00009710: 2f63 2062 6566 6f72 6520 3130 3020 636f  /c before 100 co
-00009720: 6e74 696e 7565 2229 0a0a 2020 2020 2020  ntinue")..      
-00009730: 2020 7265 7475 726e 2073 656c 662e 6861    return self.ha
-00009740: 6e64 6c65 5f73 7461 7368 2854 7275 6529  ndle_stash(True)
-00009750: 0a0a 2020 2020 6465 6620 6861 6e64 6c65  ..    def handle
-00009760: 5f70 6f73 7428 7365 6c66 2920 203a 0a20  _post(self)  :. 
-00009770: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
-00009780: 2250 4f53 5420 2220 2b20 7365 6c66 2e72  "POST " + self.r
-00009790: 6571 290a 0a20 2020 2020 2020 2069 6620  eq)..        if 
-000097a0: 7365 6c66 2e68 6561 6465 7273 2e67 6574  self.headers.get
-000097b0: 2822 6578 7065 6374 222c 2022 2229 2e6c  ("expect", "").l
-000097c0: 6f77 6572 2829 203d 3d20 2231 3030 2d63  ower() == "100-c
-000097d0: 6f6e 7469 6e75 6522 3a0a 2020 2020 2020  ontinue":.      
-000097e0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000097f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009800: 732e 7365 7474 696d 656f 7574 284e 6f6e  s.settimeout(Non
-00009810: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00009820: 2020 2073 656c 662e 732e 7365 6e64 616c     self.s.sendal
-00009830: 6c28 6222 4854 5450 2f31 2e31 2031 3030  l(b"HTTP/1.1 100
-00009840: 2043 6f6e 7469 6e75 655c 725c 6e5c 725c   Continue\r\n\r\
-00009850: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
-00009860: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00009870: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
-00009880: 626b 6163 2834 3030 2c20 2263 6c69 656e  bkac(400, "clien
-00009890: 7420 642f 6320 6265 666f 7265 2031 3030  t d/c before 100
-000098a0: 2063 6f6e 7469 6e75 6522 290a 0a20 2020   continue")..   
-000098b0: 2020 2020 2069 6620 2272 6177 2220 696e       if "raw" in
-000098c0: 2073 656c 662e 7570 6172 616d 3a0a 2020   self.uparam:.  
-000098d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000098e0: 2073 656c 662e 6861 6e64 6c65 5f73 7461   self.handle_sta
-000098f0: 7368 2846 616c 7365 290a 0a20 2020 2020  sh(False)..     
-00009900: 2020 2063 7479 7065 203d 2073 656c 662e     ctype = self.
-00009910: 6865 6164 6572 732e 6765 7428 2263 6f6e  headers.get("con
-00009920: 7465 6e74 2d74 7970 6522 2c20 2222 292e  tent-type", "").
-00009930: 6c6f 7765 7228 290a 0a20 2020 2020 2020  lower()..       
-00009940: 2069 6620 226d 756c 7469 7061 7274 2f66   if "multipart/f
-00009950: 6f72 6d2d 6461 7461 2220 696e 2063 7479  orm-data" in cty
-00009960: 7065 3a0a 2020 2020 2020 2020 2020 2020  pe:.            
-00009970: 7265 7475 726e 2073 656c 662e 6861 6e64  return self.hand
-00009980: 6c65 5f70 6f73 745f 6d75 6c74 6970 6172  le_post_multipar
-00009990: 7428 290a 0a20 2020 2020 2020 2069 6620  t()..        if 
-000099a0: 280a 2020 2020 2020 2020 2020 2020 2261  (.            "a
-000099b0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e22  pplication/json"
-000099c0: 2069 6e20 6374 7970 650a 2020 2020 2020   in ctype.      
-000099d0: 2020 2020 2020 6f72 2022 7465 7874 2f70        or "text/p
-000099e0: 6c61 696e 2220 696e 2063 7479 7065 0a20  lain" in ctype. 
-000099f0: 2020 2020 2020 2020 2020 206f 7220 2261             or "a
-00009a00: 7070 6c69 6361 7469 6f6e 2f78 6d6c 2220  pplication/xml" 
-00009a10: 696e 2063 7479 7065 0a20 2020 2020 2020  in ctype.       
-00009a20: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00009a30: 7265 7475 726e 2073 656c 662e 6861 6e64  return self.hand
-00009a40: 6c65 5f70 6f73 745f 6a73 6f6e 2829 0a0a  le_post_json()..
-00009a50: 2020 2020 2020 2020 6966 2022 6d6f 7665          if "move
-00009a60: 2220 696e 2073 656c 662e 7570 6172 616d  " in self.uparam
-00009a70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00009a80: 7475 726e 2073 656c 662e 6861 6e64 6c65  turn self.handle
-00009a90: 5f6d 7628 290a 0a20 2020 2020 2020 2069  _mv()..        i
-00009aa0: 6620 2264 656c 6574 6522 2069 6e20 7365  f "delete" in se
-00009ab0: 6c66 2e75 7061 7261 6d3a 0a20 2020 2020  lf.uparam:.     
-00009ac0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00009ad0: 6c66 2e68 616e 646c 655f 726d 285b 5d29  lf.handle_rm([])
-00009ae0: 0a0a 2020 2020 2020 2020 6966 2022 6170  ..        if "ap
-00009af0: 706c 6963 6174 696f 6e2f 6f63 7465 742d  plication/octet-
-00009b00: 7374 7265 616d 2220 696e 2063 7479 7065  stream" in ctype
-00009b10: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00009b20: 7475 726e 2073 656c 662e 6861 6e64 6c65  turn self.handle
-00009b30: 5f70 6f73 745f 6269 6e61 7279 2829 0a0a  _post_binary()..
-00009b40: 2020 2020 2020 2020 6966 2022 6170 706c          if "appl
-00009b50: 6963 6174 696f 6e2f 782d 7777 772d 666f  ication/x-www-fo
-00009b60: 726d 2d75 726c 656e 636f 6465 6422 2069  rm-urlencoded" i
-00009b70: 6e20 6374 7970 653a 0a20 2020 2020 2020  n ctype:.       
-00009b80: 2020 2020 206f 7074 203d 2073 656c 662e       opt = self.
-00009b90: 6172 6773 2e75 726c 666f 726d 0a20 2020  args.urlform.   
-00009ba0: 2020 2020 2020 2020 2069 6620 2273 7461           if "sta
-00009bb0: 7368 2220 696e 206f 7074 3a0a 2020 2020  sh" in opt:.    
-00009bc0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009bd0: 726e 2073 656c 662e 6861 6e64 6c65 5f73  rn self.handle_s
-00009be0: 7461 7368 2846 616c 7365 290a 0a20 2020  tash(False)..   
-00009bf0: 2020 2020 2020 2020 2069 6620 2273 6176           if "sav
-00009c00: 6522 2069 6e20 6f70 743a 0a20 2020 2020  e" in opt:.     
-00009c10: 2020 2020 2020 2020 2020 2070 6f73 745f             post_
-00009c20: 737a 2c20 5f2c 205f 2c20 5f2c 2070 6174  sz, _, _, _, pat
-00009c30: 682c 205f 203d 2073 656c 662e 6475 6d70  h, _ = self.dump
-00009c40: 5f74 6f5f 6669 6c65 2846 616c 7365 290a  _to_file(False).
-00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c60: 7365 6c66 2e6c 6f67 2822 7572 6c66 6f72  self.log("urlfor
-00009c70: 6d3a 207b 7d20 6279 7465 732c 207b 7d22  m: {} bytes, {}"
-00009c80: 2e66 6f72 6d61 7428 706f 7374 5f73 7a2c  .format(post_sz,
-00009c90: 2070 6174 6829 290a 2020 2020 2020 2020   path)).        
-00009ca0: 2020 2020 656c 6966 2022 7072 696e 7422      elif "print"
-00009cb0: 2069 6e20 6f70 743a 0a20 2020 2020 2020   in opt:.       
-00009cc0: 2020 2020 2020 2020 2072 6561 6465 722c           reader,
-00009cd0: 205f 203d 2073 656c 662e 6765 745f 626f   _ = self.get_bo
-00009ce0: 6479 5f72 6561 6465 7228 290a 2020 2020  dy_reader().    
-00009cf0: 2020 2020 2020 2020 2020 2020 6275 6620              buf 
-00009d00: 3d20 6222 220a 2020 2020 2020 2020 2020  = b"".          
-00009d10: 2020 2020 2020 666f 7220 7262 7566 2069        for rbuf i
-00009d20: 6e20 7265 6164 6572 3a0a 2020 2020 2020  n reader:.      
-00009d30: 2020 2020 2020 2020 2020 2020 2020 6275                bu
-00009d40: 6620 2b3d 2072 6275 660a 2020 2020 2020  f += rbuf.      
-00009d50: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00009d60: 206e 6f74 2072 6275 6620 6f72 206c 656e   not rbuf or len
-00009d70: 2862 7566 2920 3e3d 2033 3237 3638 3a0a  (buf) >= 32768:.
+000076b0: 7265 7420 2b3d 2022 3c44 3a7b 307d 3e7b  ret += "<D:{0}>{
+000076c0: 317d 3c2f 443a 7b30 7d3e 222e 666f 726d  1}</D:{0}>".form
+000076d0: 6174 286b 2c20 7629 0a20 2020 2020 2020  at(k, v).       
+000076e0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007700: 2020 2072 6574 202b 3d20 223c 443a 7b7d     ret += "<D:{}
+00007710: 2f3e 222e 666f 726d 6174 286b 290a 0a20  />".format(k).. 
+00007720: 2020 2020 2020 2020 2020 2072 6574 202b             ret +
+00007730: 3d20 223c 2f44 3a70 726f 703e 3c44 3a73  = "</D:prop><D:s
+00007740: 7461 7475 733e 4854 5450 2f31 2e31 2032  tatus>HTTP/1.1 2
+00007750: 3030 204f 4b3c 2f44 3a73 7461 7475 733e  00 OK</D:status>
+00007760: 3c2f 443a 7072 6f70 7374 6174 3e22 0a0a  </D:propstat>"..
+00007770: 2020 2020 2020 2020 2020 2020 6d69 7373              miss
+00007780: 696e 6720 3d20 5b22 3c44 3a7b 7d2f 3e22  ing = ["<D:{}/>"
+00007790: 2e66 6f72 6d61 7428 7829 2066 6f72 2078  .format(x) for x
+000077a0: 2069 6e20 7072 6f70 7320 6966 2078 206e   in props if x n
+000077b0: 6f74 2069 6e20 7076 735d 0a20 2020 2020  ot in pvs].     
+000077c0: 2020 2020 2020 2069 6620 6d69 7373 696e         if missin
+000077d0: 6720 616e 6420 636c 656e 3a0a 2020 2020  g and clen:.    
+000077e0: 2020 2020 2020 2020 2020 2020 7420 3d20              t = 
+000077f0: 223c 443a 7072 6f70 7374 6174 3e3c 443a  "<D:propstat><D:
+00007800: 7072 6f70 3e7b 7d3c 2f44 3a70 726f 703e  prop>{}</D:prop>
+00007810: 3c44 3a73 7461 7475 733e 4854 5450 2f31  <D:status>HTTP/1
+00007820: 2e31 2034 3034 204e 6f74 2046 6f75 6e64  .1 404 Not Found
+00007830: 3c2f 443a 7374 6174 7573 3e3c 2f44 3a70  </D:status></D:p
+00007840: 726f 7073 7461 743e 220a 2020 2020 2020  ropstat>".      
+00007850: 2020 2020 2020 2020 2020 7265 7420 2b3d            ret +=
+00007860: 2074 2e66 6f72 6d61 7428 2222 2e6a 6f69   t.format("".joi
+00007870: 6e28 6d69 7373 696e 6729 290a 0a20 2020  n(missing))..   
+00007880: 2020 2020 2020 2020 2072 6574 202b 3d20           ret += 
+00007890: 223c 2f44 3a72 6573 706f 6e73 653e 220a  "</D:response>".
+000078a0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
+000078b0: 6520 6c65 6e28 7265 7429 203e 3d20 6368  e len(ret) >= ch
+000078c0: 756e 6b73 7a3a 0a20 2020 2020 2020 2020  unksz:.         
+000078d0: 2020 2020 2020 2072 6574 203d 2073 656c         ret = sel
+000078e0: 662e 7365 6e64 5f63 6875 6e6b 2872 6574  f.send_chunk(ret
+000078f0: 2c20 656e 632c 2063 6875 6e6b 737a 290a  , enc, chunksz).
+00007900: 0a20 2020 2020 2020 2072 6574 202b 3d20  .        ret += 
+00007910: 223c 2f44 3a6d 756c 7469 7374 6174 7573  "</D:multistatus
+00007920: 3e22 0a20 2020 2020 2020 2077 6869 6c65  >".        while
+00007930: 2072 6574 3a0a 2020 2020 2020 2020 2020   ret:.          
+00007940: 2020 7265 7420 3d20 7365 6c66 2e73 656e    ret = self.sen
+00007950: 645f 6368 756e 6b28 7265 742c 2065 6e63  d_chunk(ret, enc
+00007960: 2c20 6368 756e 6b73 7a29 0a0a 2020 2020  , chunksz)..    
+00007970: 2020 2020 7365 6c66 2e73 656e 645f 6368      self.send_ch
+00007980: 756e 6b28 2222 2c20 656e 632c 2063 6875  unk("", enc, chu
+00007990: 6e6b 737a 290a 2020 2020 2020 2020 2320  nksz).        # 
+000079a0: 7365 6c66 2e72 6570 6c79 2872 6574 2e65  self.reply(ret.e
+000079b0: 6e63 6f64 6528 656e 632c 2022 7265 706c  ncode(enc, "repl
+000079c0: 6163 6522 292c 3230 372c 2022 7465 7874  ace"),207, "text
+000079d0: 2f78 6d6c 3b20 6368 6172 7365 743d 2220  /xml; charset=" 
+000079e0: 2b20 656e 6329 0a20 2020 2020 2020 2072  + enc).        r
+000079f0: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
+00007a00: 6465 6620 6861 6e64 6c65 5f70 726f 7070  def handle_propp
+00007a10: 6174 6368 2873 656c 6629 2020 3a0a 2020  atch(self)  :.  
+00007a20: 2020 2020 2020 6966 2073 656c 662e 646f        if self.do
+00007a30: 5f6c 6f67 3a0a 2020 2020 2020 2020 2020  _log:.          
+00007a40: 2020 7365 6c66 2e6c 6f67 2822 5050 4154    self.log("PPAT
+00007a50: 4348 2022 202b 2073 656c 662e 7265 7129  CH " + self.req)
+00007a60: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00007a70: 662e 6172 6773 2e6e 6f5f 6461 763a 0a20  f.args.no_dav:. 
+00007a80: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00007a90: 2050 6562 6b61 6328 3430 352c 2022 5765   Pebkac(405, "We
+00007aa0: 6244 4156 2069 7320 6469 7361 626c 6564  bDAV is disabled
+00007ab0: 2069 6e20 7365 7276 6572 2063 6f6e 6669   in server confi
+00007ac0: 6722 290a 0a20 2020 2020 2020 2069 6620  g")..        if 
+00007ad0: 6e6f 7420 7365 6c66 2e63 616e 5f77 7269  not self.can_wri
+00007ae0: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
+00007af0: 7365 6c66 2e6c 6f67 2822 7b7d 2074 7269  self.log("{} tri
+00007b00: 6564 2074 6f20 7072 6f70 7061 7463 6820  ed to proppatch 
+00007b10: 5b7b 7d5d 222e 666f 726d 6174 2873 656c  [{}]".format(sel
+00007b20: 662e 756e 616d 652c 2073 656c 662e 7670  f.uname, self.vp
+00007b30: 6174 6829 290a 2020 2020 2020 2020 2020  ath)).          
+00007b40: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
+00007b50: 3031 2c20 2261 7574 6865 6e74 6963 6174  01, "authenticat
+00007b60: 6522 290a 0a20 2020 2020 2020 2066 726f  e")..        fro
+00007b70: 6d20 786d 6c2e 6574 7265 6520 696d 706f  m xml.etree impo
+00007b80: 7274 2045 6c65 6d65 6e74 5472 6565 2061  rt ElementTree a
+00007b90: 7320 4554 0a0a 2020 2020 2020 2020 6672  s ET..        fr
+00007ba0: 6f6d 202e 6478 6d6c 2069 6d70 6f72 7420  om .dxml import 
+00007bb0: 6d6b 656e 6f64 2c20 6d6b 746e 6f64 2c20  mkenod, mktnod, 
+00007bc0: 7061 7273 655f 786d 6c0a 0a20 2020 2020  parse_xml..     
+00007bd0: 2020 2073 656c 662e 6173 7276 2e76 6673     self.asrv.vfs
+00007be0: 2e67 6574 2873 656c 662e 7670 6174 682c  .get(self.vpath,
+00007bf0: 2073 656c 662e 756e 616d 652c 2046 616c   self.uname, Fal
+00007c00: 7365 2c20 4661 6c73 6529 0a20 2020 2020  se, False).     
+00007c10: 2020 2023 2061 6273 7061 7468 203d 2076     # abspath = v
+00007c20: 6e2e 6463 616e 6f6e 6963 616c 2872 656d  n.dcanonical(rem
+00007c30: 290a 0a20 2020 2020 2020 2062 7566 203d  )..        buf =
+00007c40: 2062 2222 0a20 2020 2020 2020 2066 6f72   b"".        for
+00007c50: 2072 6275 6620 696e 2073 656c 662e 6765   rbuf in self.ge
+00007c60: 745f 626f 6479 5f72 6561 6465 7228 295b  t_body_reader()[
+00007c70: 305d 3a0a 2020 2020 2020 2020 2020 2020  0]:.            
+00007c80: 6275 6620 2b3d 2072 6275 660a 2020 2020  buf += rbuf.    
+00007c90: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+00007ca0: 6275 6620 6f72 206c 656e 2862 7566 2920  buf or len(buf) 
+00007cb0: 3e3d 2031 3238 202a 2031 3032 343a 0a20  >= 128 * 1024:. 
+00007cc0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00007cd0: 7265 616b 0a0a 2020 2020 2020 2020 6966  reak..        if
+00007ce0: 2073 656c 662e 5f61 7070 6c65 7361 6e28   self._applesan(
+00007cf0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00007d00: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
+00007d10: 2020 2020 7478 7420 3d20 6275 662e 6465      txt = buf.de
+00007d20: 636f 6465 2822 6173 6369 6922 2c20 2272  code("ascii", "r
+00007d30: 6570 6c61 6365 2229 2e6c 6f77 6572 2829  eplace").lower()
+00007d40: 0a20 2020 2020 2020 2065 6e63 203d 2073  .        enc = s
+00007d50: 656c 662e 6765 745f 786d 6c5f 656e 6328  elf.get_xml_enc(
+00007d60: 7478 7429 0a20 2020 2020 2020 2075 656e  txt).        uen
+00007d70: 6320 3d20 656e 632e 7570 7065 7228 290a  c = enc.upper().
+00007d80: 0a20 2020 2020 2020 2074 7874 203d 2062  .        txt = b
+00007d90: 7566 2e64 6563 6f64 6528 656e 632c 2022  uf.decode(enc, "
+00007da0: 7265 706c 6163 6522 290a 2020 2020 2020  replace").      
+00007db0: 2020 4554 2e72 6567 6973 7465 725f 6e61    ET.register_na
+00007dc0: 6d65 7370 6163 6528 2244 222c 2022 4441  mespace("D", "DA
+00007dd0: 563a 2229 0a20 2020 2020 2020 2078 726f  V:").        xro
+00007de0: 6f74 203d 206d 6b65 6e6f 6428 2244 3a6f  ot = mkenod("D:o
+00007df0: 727a 2229 0a20 2020 2020 2020 2078 726f  rz").        xro
+00007e00: 6f74 2e69 6e73 6572 7428 302c 2070 6172  ot.insert(0, par
+00007e10: 7365 5f78 6d6c 2874 7874 2929 0a20 2020  se_xml(txt)).   
+00007e20: 2020 2020 2078 7072 6f70 203d 2078 726f       xprop = xro
+00007e30: 6f74 2e66 696e 6428 7222 2e2f 7b44 4156  ot.find(r"./{DAV
+00007e40: 3a7d 7072 6f70 6572 7479 7570 6461 7465  :}propertyupdate
+00007e50: 2f7b 4441 563a 7d73 6574 2f7b 4441 563a  /{DAV:}set/{DAV:
+00007e60: 7d70 726f 7022 290a 2020 2020 2020 2020  }prop").        
+00007e70: 6173 7365 7274 2078 7072 6f70 0a20 2020  assert xprop.   
+00007e80: 2020 2020 2066 6f72 207a 6520 696e 2078       for ze in x
+00007e90: 7072 6f70 3a0a 2020 2020 2020 2020 2020  prop:.          
+00007ea0: 2020 7a65 2e63 6c65 6172 2829 0a0a 2020    ze.clear()..  
+00007eb0: 2020 2020 2020 7478 7420 3d20 2222 223c        txt = """<
+00007ec0: 6d75 6c74 6973 7461 7475 7320 786d 6c6e  multistatus xmln
+00007ed0: 733d 2244 4156 3a22 3e3c 7265 7370 6f6e  s="DAV:"><respon
+00007ee0: 7365 3e3c 7072 6f70 7374 6174 3e3c 7374  se><propstat><st
+00007ef0: 6174 7573 3e48 5454 502f 312e 3120 3430  atus>HTTP/1.1 40
+00007f00: 3320 466f 7262 6964 6465 6e3c 2f73 7461  3 Forbidden</sta
+00007f10: 7475 733e 3c2f 7072 6f70 7374 6174 3e3c  tus></propstat><
+00007f20: 2f72 6573 706f 6e73 653e 3c2f 6d75 6c74  /response></mult
+00007f30: 6973 7461 7475 733e 2222 220a 2020 2020  istatus>""".    
+00007f40: 2020 2020 7872 6f6f 7420 3d20 7061 7273      xroot = pars
+00007f50: 655f 786d 6c28 7478 7429 0a0a 2020 2020  e_xml(txt)..    
+00007f60: 2020 2020 656c 203d 2078 726f 6f74 2e66      el = xroot.f
+00007f70: 696e 6428 7222 2e2f 7b44 4156 3a7d 7265  ind(r"./{DAV:}re
+00007f80: 7370 6f6e 7365 2229 0a20 2020 2020 2020  sponse").       
+00007f90: 2061 7373 6572 7420 656c 0a20 2020 2020   assert el.     
+00007fa0: 2020 2065 3220 3d20 6d6b 746e 6f64 2822     e2 = mktnod("
+00007fb0: 443a 6872 6566 222c 2071 756f 7465 7028  D:href", quotep(
+00007fc0: 7365 6c66 2e61 7267 732e 5352 5320 2b20  self.args.SRS + 
+00007fd0: 7365 6c66 2e76 7061 7468 2929 0a20 2020  self.vpath)).   
+00007fe0: 2020 2020 2065 6c2e 696e 7365 7274 2830       el.insert(0
+00007ff0: 2c20 6532 290a 0a20 2020 2020 2020 2065  , e2)..        e
+00008000: 6c20 3d20 7872 6f6f 742e 6669 6e64 2872  l = xroot.find(r
+00008010: 222e 2f7b 4441 563a 7d72 6573 706f 6e73  "./{DAV:}respons
+00008020: 652f 7b44 4156 3a7d 7072 6f70 7374 6174  e/{DAV:}propstat
+00008030: 2229 0a20 2020 2020 2020 2061 7373 6572  ").        asser
+00008040: 7420 656c 0a20 2020 2020 2020 2065 6c2e  t el.        el.
+00008050: 696e 7365 7274 2830 2c20 7870 726f 7029  insert(0, xprop)
+00008060: 0a0a 2020 2020 2020 2020 7265 7420 3d20  ..        ret = 
+00008070: 273c 3f78 6d6c 2076 6572 7369 6f6e 3d22  '<?xml version="
+00008080: 312e 3022 2065 6e63 6f64 696e 673d 227b  1.0" encoding="{
+00008090: 7d22 3f3e 5c6e 272e 666f 726d 6174 2875  }"?>\n'.format(u
+000080a0: 656e 6329 0a20 2020 2020 2020 2072 6574  enc).        ret
+000080b0: 202b 3d20 4554 2e74 6f73 7472 696e 6728   += ET.tostring(
+000080c0: 7872 6f6f 7429 2e64 6563 6f64 6528 2275  xroot).decode("u
+000080d0: 7466 2d38 2229 0a0a 2020 2020 2020 2020  tf-8")..        
+000080e0: 7365 6c66 2e72 6570 6c79 2872 6574 2e65  self.reply(ret.e
+000080f0: 6e63 6f64 6528 656e 632c 2022 7265 706c  ncode(enc, "repl
+00008100: 6163 6522 292c 2032 3037 2c20 2274 6578  ace"), 207, "tex
+00008110: 742f 786d 6c3b 2063 6861 7273 6574 3d22  t/xml; charset="
+00008120: 202b 2065 6e63 290a 2020 2020 2020 2020   + enc).        
+00008130: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+00008140: 2064 6566 2068 616e 646c 655f 6c6f 636b   def handle_lock
+00008150: 2873 656c 6629 2020 3a0a 2020 2020 2020  (self)  :.      
+00008160: 2020 6966 2073 656c 662e 646f 5f6c 6f67    if self.do_log
+00008170: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008180: 6c66 2e6c 6f67 2822 4c4f 434b 2022 202b  lf.log("LOCK " +
+00008190: 2073 656c 662e 7265 7129 0a0a 2020 2020   self.req)..    
+000081a0: 2020 2020 6966 2073 656c 662e 6172 6773      if self.args
+000081b0: 2e6e 6f5f 6461 763a 0a20 2020 2020 2020  .no_dav:.       
+000081c0: 2020 2020 2072 6169 7365 2050 6562 6b61       raise Pebka
+000081d0: 6328 3430 352c 2022 5765 6244 4156 2069  c(405, "WebDAV i
+000081e0: 7320 6469 7361 626c 6564 2069 6e20 7365  s disabled in se
+000081f0: 7276 6572 2063 6f6e 6669 6722 290a 0a20  rver config").. 
+00008200: 2020 2020 2020 2023 2077 696e 372b 2064         # win7+ d
+00008210: 6561 646c 6f63 6b73 2069 6620 7765 2073  eadlocks if we s
+00008220: 6179 206e 6f3b 206a 7573 7420 736d 696c  ay no; just smil
+00008230: 6520 616e 6420 6e6f 640a 2020 2020 2020  e and nod.      
+00008240: 2020 6966 206e 6f74 2073 656c 662e 6361    if not self.ca
+00008250: 6e5f 7772 6974 6520 616e 6420 224d 6963  n_write and "Mic
+00008260: 726f 736f 6674 2d57 6562 4441 5622 206e  rosoft-WebDAV" n
+00008270: 6f74 2069 6e20 7365 6c66 2e75 613a 0a20  ot in self.ua:. 
+00008280: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008290: 6c6f 6728 227b 7d20 7472 6965 6420 746f  log("{} tried to
+000082a0: 206c 6f63 6b20 5b7b 7d5d 222e 666f 726d   lock [{}]".form
+000082b0: 6174 2873 656c 662e 756e 616d 652c 2073  at(self.uname, s
+000082c0: 656c 662e 7670 6174 6829 290a 2020 2020  elf.vpath)).    
+000082d0: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
+000082e0: 626b 6163 2834 3031 2c20 2261 7574 6865  bkac(401, "authe
+000082f0: 6e74 6963 6174 6522 290a 0a20 2020 2020  nticate")..     
+00008300: 2020 2066 726f 6d20 786d 6c2e 6574 7265     from xml.etre
+00008310: 6520 696d 706f 7274 2045 6c65 6d65 6e74  e import Element
+00008320: 5472 6565 2061 7320 4554 0a0a 2020 2020  Tree as ET..    
+00008330: 2020 2020 6672 6f6d 202e 6478 6d6c 2069      from .dxml i
+00008340: 6d70 6f72 7420 6d6b 656e 6f64 2c20 6d6b  mport mkenod, mk
+00008350: 746e 6f64 2c20 7061 7273 655f 786d 6c0a  tnod, parse_xml.
+00008360: 0a20 2020 2020 2020 2076 6e2c 2072 656d  .        vn, rem
+00008370: 203d 2073 656c 662e 6173 7276 2e76 6673   = self.asrv.vfs
+00008380: 2e67 6574 2873 656c 662e 7670 6174 682c  .get(self.vpath,
+00008390: 2073 656c 662e 756e 616d 652c 2046 616c   self.uname, Fal
+000083a0: 7365 2c20 4661 6c73 6529 0a20 2020 2020  se, False).     
+000083b0: 2020 2061 6273 7061 7468 203d 2076 6e2e     abspath = vn.
+000083c0: 6463 616e 6f6e 6963 616c 2872 656d 290a  dcanonical(rem).
+000083d0: 0a20 2020 2020 2020 2062 7566 203d 2062  .        buf = b
+000083e0: 2222 0a20 2020 2020 2020 2066 6f72 2072  "".        for r
+000083f0: 6275 6620 696e 2073 656c 662e 6765 745f  buf in self.get_
+00008400: 626f 6479 5f72 6561 6465 7228 295b 305d  body_reader()[0]
+00008410: 3a0a 2020 2020 2020 2020 2020 2020 6275  :.            bu
+00008420: 6620 2b3d 2072 6275 660a 2020 2020 2020  f += rbuf.      
+00008430: 2020 2020 2020 6966 206e 6f74 2072 6275        if not rbu
+00008440: 6620 6f72 206c 656e 2862 7566 2920 3e3d  f or len(buf) >=
+00008450: 2031 3238 202a 2031 3032 343a 0a20 2020   128 * 1024:.   
+00008460: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00008470: 616b 0a0a 2020 2020 2020 2020 6966 2073  ak..        if s
+00008480: 656c 662e 5f61 7070 6c65 7361 6e28 293a  elf._applesan():
+00008490: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000084a0: 7572 6e20 5472 7565 0a0a 2020 2020 2020  urn True..      
+000084b0: 2020 7478 7420 3d20 6275 662e 6465 636f    txt = buf.deco
+000084c0: 6465 2822 6173 6369 6922 2c20 2272 6570  de("ascii", "rep
+000084d0: 6c61 6365 2229 2e6c 6f77 6572 2829 0a20  lace").lower(). 
+000084e0: 2020 2020 2020 2065 6e63 203d 2073 656c         enc = sel
+000084f0: 662e 6765 745f 786d 6c5f 656e 6328 7478  f.get_xml_enc(tx
+00008500: 7429 0a20 2020 2020 2020 2075 656e 6320  t).        uenc 
+00008510: 3d20 656e 632e 7570 7065 7228 290a 0a20  = enc.upper().. 
+00008520: 2020 2020 2020 2074 7874 203d 2062 7566         txt = buf
+00008530: 2e64 6563 6f64 6528 656e 632c 2022 7265  .decode(enc, "re
+00008540: 706c 6163 6522 290a 2020 2020 2020 2020  place").        
+00008550: 4554 2e72 6567 6973 7465 725f 6e61 6d65  ET.register_name
+00008560: 7370 6163 6528 2244 222c 2022 4441 563a  space("D", "DAV:
+00008570: 2229 0a20 2020 2020 2020 206c 6b20 3d20  ").        lk = 
+00008580: 7061 7273 655f 786d 6c28 7478 7429 0a20  parse_xml(txt). 
+00008590: 2020 2020 2020 2061 7373 6572 7420 6c6b         assert lk
+000085a0: 2e74 6167 203d 3d20 227b 4441 563a 7d6c  .tag == "{DAV:}l
+000085b0: 6f63 6b69 6e66 6f22 0a0a 2020 2020 2020  ockinfo"..      
+000085c0: 2020 746f 6b65 6e20 3d20 7374 7228 7575    token = str(uu
+000085d0: 6964 2e75 7569 6434 2829 290a 0a20 2020  id.uuid4())..   
+000085e0: 2020 2020 2069 6620 6e6f 7420 6c6b 2e66       if not lk.f
+000085f0: 696e 6428 7222 2e2f 7b44 4156 3a7d 6465  ind(r"./{DAV:}de
+00008600: 7074 6822 293a 0a20 2020 2020 2020 2020  pth"):.         
+00008610: 2020 2064 6570 7468 203d 2073 656c 662e     depth = self.
+00008620: 6865 6164 6572 732e 6765 7428 2264 6570  headers.get("dep
+00008630: 7468 222c 2022 696e 6669 6e69 7479 2229  th", "infinity")
+00008640: 0a20 2020 2020 2020 2020 2020 206c 6b2e  .            lk.
+00008650: 6170 7065 6e64 286d 6b74 6e6f 6428 2244  append(mktnod("D
+00008660: 3a64 6570 7468 222c 2064 6570 7468 2929  :depth", depth))
+00008670: 0a0a 2020 2020 2020 2020 6c6b 2e61 7070  ..        lk.app
+00008680: 656e 6428 6d6b 746e 6f64 2822 443a 7469  end(mktnod("D:ti
+00008690: 6d65 6f75 7422 2c20 2253 6563 6f6e 642d  meout", "Second-
+000086a0: 3333 3130 2229 290a 2020 2020 2020 2020  3310")).        
+000086b0: 6c6b 2e61 7070 656e 6428 6d6b 656e 6f64  lk.append(mkenod
+000086c0: 2822 443a 6c6f 636b 746f 6b65 6e22 2c20  ("D:locktoken", 
+000086d0: 6d6b 746e 6f64 2822 443a 6872 6566 222c  mktnod("D:href",
+000086e0: 2074 6f6b 656e 2929 290a 2020 2020 2020   token))).      
+000086f0: 2020 6c6b 2e61 7070 656e 6428 0a20 2020    lk.append(.   
+00008700: 2020 2020 2020 2020 206d 6b65 6e6f 6428           mkenod(
+00008710: 2244 3a6c 6f63 6b72 6f6f 7422 2c20 6d6b  "D:lockroot", mk
+00008720: 746e 6f64 2822 443a 6872 6566 222c 2071  tnod("D:href", q
+00008730: 756f 7465 7028 7365 6c66 2e61 7267 732e  uotep(self.args.
+00008740: 5352 5320 2b20 7365 6c66 2e76 7061 7468  SRS + self.vpath
+00008750: 2929 290a 2020 2020 2020 2020 290a 0a20  ))).        ).. 
+00008760: 2020 2020 2020 206c 6b32 203d 206d 6b65         lk2 = mke
+00008770: 6e6f 6428 2244 3a61 6374 6976 656c 6f63  nod("D:activeloc
+00008780: 6b22 290a 2020 2020 2020 2020 7872 6f6f  k").        xroo
+00008790: 7420 3d20 6d6b 656e 6f64 2822 443a 7072  t = mkenod("D:pr
+000087a0: 6f70 222c 206d 6b65 6e6f 6428 2244 3a6c  op", mkenod("D:l
+000087b0: 6f63 6b64 6973 636f 7665 7279 222c 206c  ockdiscovery", l
+000087c0: 6b32 2929 0a20 2020 2020 2020 2066 6f72  k2)).        for
+000087d0: 2061 2069 6e20 6c6b 3a0a 2020 2020 2020   a in lk:.      
+000087e0: 2020 2020 2020 6c6b 322e 6170 7065 6e64        lk2.append
+000087f0: 2861 290a 0a20 2020 2020 2020 2072 6574  (a)..        ret
+00008800: 203d 2027 3c3f 786d 6c20 7665 7273 696f   = '<?xml versio
+00008810: 6e3d 2231 2e30 2220 656e 636f 6469 6e67  n="1.0" encoding
+00008820: 3d22 7b7d 223f 3e5c 6e27 2e66 6f72 6d61  ="{}"?>\n'.forma
+00008830: 7428 7565 6e63 290a 2020 2020 2020 2020  t(uenc).        
+00008840: 7265 7420 2b3d 2045 542e 746f 7374 7269  ret += ET.tostri
+00008850: 6e67 2878 726f 6f74 292e 6465 636f 6465  ng(xroot).decode
+00008860: 2822 7574 662d 3822 290a 0a20 2020 2020  ("utf-8")..     
+00008870: 2020 2072 6320 3d20 3230 300a 2020 2020     rc = 200.    
+00008880: 2020 2020 6966 2073 656c 662e 6361 6e5f      if self.can_
+00008890: 7772 6974 6520 616e 6420 6e6f 7420 626f  write and not bo
+000088a0: 732e 7061 7468 2e69 7366 696c 6528 6162  s.path.isfile(ab
+000088b0: 7370 6174 6829 3a0a 2020 2020 2020 2020  spath):.        
+000088c0: 2020 2020 7769 7468 206f 7065 6e28 6673      with open(fs
+000088d0: 656e 6328 6162 7370 6174 6829 2c20 2277  enc(abspath), "w
+000088e0: 6222 2920 6173 205f 3a0a 2020 2020 2020  b") as _:.      
+000088f0: 2020 2020 2020 2020 2020 7263 203d 2032            rc = 2
+00008900: 3031 0a0a 2020 2020 2020 2020 7365 6c66  01..        self
+00008910: 2e6f 7574 5f68 6561 6465 7273 5b22 4c6f  .out_headers["Lo
+00008920: 636b 2d54 6f6b 656e 225d 203d 2022 3c7b  ck-Token"] = "<{
+00008930: 7d3e 222e 666f 726d 6174 2874 6f6b 656e  }>".format(token
+00008940: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+00008950: 6570 6c79 2872 6574 2e65 6e63 6f64 6528  eply(ret.encode(
+00008960: 656e 632c 2022 7265 706c 6163 6522 292c  enc, "replace"),
+00008970: 2072 632c 2022 7465 7874 2f78 6d6c 3b20   rc, "text/xml; 
+00008980: 6368 6172 7365 743d 2220 2b20 656e 6329  charset=" + enc)
+00008990: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000089a0: 5472 7565 0a0a 2020 2020 6465 6620 6861  True..    def ha
+000089b0: 6e64 6c65 5f75 6e6c 6f63 6b28 7365 6c66  ndle_unlock(self
+000089c0: 2920 203a 0a20 2020 2020 2020 2069 6620  )  :.        if 
+000089d0: 7365 6c66 2e64 6f5f 6c6f 673a 0a20 2020  self.do_log:.   
+000089e0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+000089f0: 6728 2255 4e4c 4f43 4b20 2220 2b20 7365  g("UNLOCK " + se
+00008a00: 6c66 2e72 6571 290a 0a20 2020 2020 2020  lf.req)..       
+00008a10: 2069 6620 7365 6c66 2e61 7267 732e 6e6f   if self.args.no
+00008a20: 5f64 6176 3a0a 2020 2020 2020 2020 2020  _dav:.          
+00008a30: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
+00008a40: 3035 2c20 2257 6562 4441 5620 6973 2064  05, "WebDAV is d
+00008a50: 6973 6162 6c65 6420 696e 2073 6572 7665  isabled in serve
+00008a60: 7220 636f 6e66 6967 2229 0a0a 2020 2020  r config")..    
+00008a70: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00008a80: 6361 6e5f 7772 6974 6520 616e 6420 224d  can_write and "M
+00008a90: 6963 726f 736f 6674 2d57 6562 4441 5622  icrosoft-WebDAV"
+00008aa0: 206e 6f74 2069 6e20 7365 6c66 2e75 613a   not in self.ua:
+00008ab0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008ac0: 662e 6c6f 6728 227b 7d20 7472 6965 6420  f.log("{} tried 
+00008ad0: 746f 206c 6f63 6b20 5b7b 7d5d 222e 666f  to lock [{}]".fo
+00008ae0: 726d 6174 2873 656c 662e 756e 616d 652c  rmat(self.uname,
+00008af0: 2073 656c 662e 7670 6174 6829 290a 2020   self.vpath)).  
+00008b00: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00008b10: 5065 626b 6163 2834 3031 2c20 2261 7574  Pebkac(401, "aut
+00008b20: 6865 6e74 6963 6174 6522 290a 0a20 2020  henticate")..   
+00008b30: 2020 2020 2073 656c 662e 7365 6e64 5f68       self.send_h
+00008b40: 6561 6465 7273 284e 6f6e 652c 2032 3034  eaders(None, 204
+00008b50: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00008b60: 2054 7275 650a 0a20 2020 2064 6566 2068   True..    def h
+00008b70: 616e 646c 655f 6d6b 636f 6c28 7365 6c66  andle_mkcol(self
+00008b80: 2920 203a 0a20 2020 2020 2020 2069 6620  )  :.        if 
+00008b90: 7365 6c66 2e5f 6170 706c 6573 616e 2829  self._applesan()
+00008ba0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00008bb0: 7475 726e 2054 7275 650a 0a20 2020 2020  turn True..     
+00008bc0: 2020 2069 6620 7365 6c66 2e64 6f5f 6c6f     if self.do_lo
+00008bd0: 673a 0a20 2020 2020 2020 2020 2020 2073  g:.            s
+00008be0: 656c 662e 6c6f 6728 224d 4b43 4f4c 2022  elf.log("MKCOL "
+00008bf0: 202b 2073 656c 662e 7265 7129 0a0a 2020   + self.req)..  
+00008c00: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00008c10: 662e 5f6d 6b64 6972 2873 656c 662e 7670  f._mkdir(self.vp
+00008c20: 6174 6829 0a0a 2020 2020 6465 6620 6861  ath)..    def ha
+00008c30: 6e64 6c65 5f6d 6f76 6528 7365 6c66 2920  ndle_move(self) 
+00008c40: 203a 0a20 2020 2020 2020 2064 7374 203d   :.        dst =
+00008c50: 2073 656c 662e 6865 6164 6572 735b 2264   self.headers["d
+00008c60: 6573 7469 6e61 7469 6f6e 225d 0a20 2020  estination"].   
+00008c70: 2020 2020 2064 7374 203d 2072 652e 7375       dst = re.su
+00008c80: 6228 225e 6874 7470 733f 3a2f 2f5b 5e2f  b("^https?://[^/
+00008c90: 5d2b 222c 2022 222c 2064 7374 292e 6c73  ]+", "", dst).ls
+00008ca0: 7472 6970 2829 0a20 2020 2020 2020 2064  trip().        d
+00008cb0: 7374 203d 2075 6e71 756f 7465 7028 6473  st = unquotep(ds
+00008cc0: 7429 0a20 2020 2020 2020 2069 6620 6e6f  t).        if no
+00008cd0: 7420 7365 6c66 2e5f 6d76 2873 656c 662e  t self._mv(self.
+00008ce0: 7670 6174 682c 2064 7374 293a 0a20 2020  vpath, dst):.   
+00008cf0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008d00: 4661 6c73 650a 0a20 2020 2020 2020 2023  False..        #
+00008d10: 2075 7032 6b20 6f6e 6c79 2063 6172 6573   up2k only cares
+00008d20: 2061 626f 7574 2066 696c 6573 2061 6e64   about files and
+00008d30: 2072 656d 6f76 6573 2061 6c6c 2065 6d70   removes all emp
+00008d40: 7479 2066 6f6c 6465 7273 3b0a 2020 2020  ty folders;.    
+00008d50: 2020 2020 2320 636c 6965 6e74 7320 6e61      # clients na
+00008d60: 7475 7261 6c6c 7920 6578 7065 6374 2065  turally expect e
+00008d70: 6d70 7479 2066 6f6c 6465 7273 2074 6f20  mpty folders to 
+00008d80: 7375 7276 6976 6520 6120 7265 6e61 6d65  survive a rename
+00008d90: 0a20 2020 2020 2020 2076 6e2c 2072 656d  .        vn, rem
+00008da0: 203d 2073 656c 662e 6173 7276 2e76 6673   = self.asrv.vfs
+00008db0: 2e67 6574 2864 7374 2c20 7365 6c66 2e75  .get(dst, self.u
+00008dc0: 6e61 6d65 2c20 4661 6c73 652c 2046 616c  name, False, Fal
+00008dd0: 7365 290a 2020 2020 2020 2020 6461 6273  se).        dabs
+00008de0: 203d 2076 6e2e 6361 6e6f 6e69 6361 6c28   = vn.canonical(
+00008df0: 7265 6d29 0a20 2020 2020 2020 2074 7279  rem).        try
+00008e00: 3a0a 2020 2020 2020 2020 2020 2020 626f  :.            bo
+00008e10: 732e 6d61 6b65 6469 7273 2864 6162 7329  s.makedirs(dabs)
+00008e20: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
+00008e30: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+00008e40: 730a 0a20 2020 2020 2020 2072 6574 7572  s..        retur
+00008e50: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
+00008e60: 5f61 7070 6c65 7361 6e28 7365 6c66 2920  _applesan(self) 
+00008e70: 203a 0a20 2020 2020 2020 2069 6620 7365   :.        if se
+00008e80: 6c66 2e61 7267 732e 6461 765f 6d61 6320  lf.args.dav_mac 
+00008e90: 6f72 2022 4461 7277 696e 2f22 206e 6f74  or "Darwin/" not
+00008ea0: 2069 6e20 7365 6c66 2e75 613a 0a20 2020   in self.ua:.   
+00008eb0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008ec0: 4661 6c73 650a 0a20 2020 2020 2020 2076  False..        v
+00008ed0: 7020 3d20 222f 2220 2b20 7365 6c66 2e76  p = "/" + self.v
+00008ee0: 7061 7468 0a20 2020 2020 2020 2070 746e  path.        ptn
+00008ef0: 203d 2072 222f 5c2e 285f 7c44 535f 5374   = r"/\.(_|DS_St
+00008f00: 6f72 657c 5370 6f74 6c69 6768 742d 7c66  ore|Spotlight-|f
+00008f10: 7365 7665 6e74 7364 7c54 7261 7368 6573  seventsd|Trashes
+00008f20: 7c41 7070 6c65 446f 7562 6c65 297c 2f5f  |AppleDouble)|/_
+00008f30: 5f4d 4143 4f53 220a 2020 2020 2020 2020  _MACOS".        
+00008f40: 6966 2072 652e 7365 6172 6368 2870 746e  if re.search(ptn
+00008f50: 2c20 7670 293a 0a20 2020 2020 2020 2020  , vp):.         
+00008f60: 2020 207a 7420 3d20 273c 3f78 6d6c 2076     zt = '<?xml v
+00008f70: 6572 7369 6f6e 3d22 312e 3022 2065 6e63  ersion="1.0" enc
+00008f80: 6f64 696e 673d 2275 7466 2d38 223f 3e5c  oding="utf-8"?>\
+00008f90: 6e3c 443a 6572 726f 7220 786d 6c6e 733a  n<D:error xmlns:
+00008fa0: 443d 2244 4156 3a22 3e3c 443a 6c6f 636b  D="DAV:"><D:lock
+00008fb0: 2d74 6f6b 656e 2d73 7562 6d69 7474 6564  -token-submitted
+00008fc0: 3e3c 443a 6872 6566 3e7b 7d3c 2f44 3a68  ><D:href>{}</D:h
+00008fd0: 7265 663e 3c2f 443a 6c6f 636b 2d74 6f6b  ref></D:lock-tok
+00008fe0: 656e 2d73 7562 6d69 7474 6564 3e3c 2f44  en-submitted></D
+00008ff0: 3a65 7272 6f72 3e27 0a20 2020 2020 2020  :error>'.       
+00009000: 2020 2020 207a 6220 3d20 7a74 2e66 6f72       zb = zt.for
+00009010: 6d61 7428 7670 292e 656e 636f 6465 2822  mat(vp).encode("
+00009020: 7574 662d 3822 2c20 2272 6570 6c61 6365  utf-8", "replace
+00009030: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+00009040: 656c 662e 7265 706c 7928 7a62 2c20 3432  elf.reply(zb, 42
+00009050: 332c 2022 7465 7874 2f78 6d6c 3b20 6368  3, "text/xml; ch
+00009060: 6172 7365 743d 7574 662d 3822 290a 2020  arset=utf-8").  
+00009070: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009080: 2054 7275 650a 0a20 2020 2020 2020 2072   True..        r
+00009090: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+000090a0: 2064 6566 2073 656e 645f 6368 756e 6b28   def send_chunk(
+000090b0: 7365 6c66 2c20 7478 7420 2c20 656e 6320  self, txt , enc 
+000090c0: 2c20 626d 6178 2029 2020 3a0a 2020 2020  , bmax )  :.    
+000090d0: 2020 2020 6f72 6967 5f6c 656e 203d 206c      orig_len = l
+000090e0: 656e 2874 7874 290a 2020 2020 2020 2020  en(txt).        
+000090f0: 6275 6620 3d20 7478 745b 3a62 6d61 785d  buf = txt[:bmax]
+00009100: 2e65 6e63 6f64 6528 656e 632c 2022 7265  .encode(enc, "re
+00009110: 706c 6163 6522 295b 3a62 6d61 785d 0a20  place")[:bmax]. 
+00009120: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00009130: 2020 2020 2020 2020 5f20 3d20 6275 662e          _ = buf.
+00009140: 6465 636f 6465 2865 6e63 290a 2020 2020  decode(enc).    
+00009150: 2020 2020 6578 6365 7074 2055 6e69 636f      except Unico
+00009160: 6465 4465 636f 6465 4572 726f 7220 6173  deDecodeError as
+00009170: 2075 6465 3a0a 2020 2020 2020 2020 2020   ude:.          
+00009180: 2020 6275 6620 3d20 6275 665b 3a20 7564    buf = buf[: ud
+00009190: 652e 7374 6172 745d 0a0a 2020 2020 2020  e.start]..      
+000091a0: 2020 7478 7420 3d20 7478 745b 6c65 6e28    txt = txt[len(
+000091b0: 6275 662e 6465 636f 6465 2865 6e63 2929  buf.decode(enc))
+000091c0: 203a 5d0a 2020 2020 2020 2020 6966 2074   :].        if t
+000091d0: 7874 2061 6e64 206c 656e 2874 7874 2920  xt and len(txt) 
+000091e0: 3d3d 206f 7269 675f 6c65 6e3a 0a20 2020  == orig_len:.   
+000091f0: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
+00009200: 6562 6b61 6328 3530 302c 2022 6368 756e  ebkac(500, "chun
+00009210: 6b20 736c 6963 696e 6720 6661 696c 6564  k slicing failed
+00009220: 2229 0a0a 2020 2020 2020 2020 6275 6620  ")..        buf 
+00009230: 3d20 227b 3a78 7d5c 725c 6e22 2e66 6f72  = "{:x}\r\n".for
+00009240: 6d61 7428 6c65 6e28 6275 6629 292e 656e  mat(len(buf)).en
+00009250: 636f 6465 2865 6e63 2920 2b20 6275 660a  code(enc) + buf.
+00009260: 2020 2020 2020 2020 7365 6c66 2e73 2e73          self.s.s
+00009270: 656e 6461 6c6c 2862 7566 202b 2062 225c  endall(buf + b"\
+00009280: 725c 6e22 290a 2020 2020 2020 2020 7265  r\n").        re
+00009290: 7475 726e 2074 7874 0a0a 2020 2020 6465  turn txt..    de
+000092a0: 6620 6861 6e64 6c65 5f6f 7074 696f 6e73  f handle_options
+000092b0: 2873 656c 6629 2020 3a0a 2020 2020 2020  (self)  :.      
+000092c0: 2020 6966 2073 656c 662e 646f 5f6c 6f67    if self.do_log
+000092d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000092e0: 6c66 2e6c 6f67 2822 4f50 5449 4f4e 5320  lf.log("OPTIONS 
+000092f0: 2220 2b20 7365 6c66 2e72 6571 290a 0a20  " + self.req).. 
+00009300: 2020 2020 2020 206f 6820 3d20 7365 6c66         oh = self
+00009310: 2e6f 7574 5f68 6561 6465 7273 0a20 2020  .out_headers.   
+00009320: 2020 2020 206f 685b 2241 6c6c 6f77 225d       oh["Allow"]
+00009330: 203d 2022 2c20 222e 6a6f 696e 2873 656c   = ", ".join(sel
+00009340: 662e 636f 6e6e 2e68 7372 762e 6d61 6c6c  f.conn.hsrv.mall
+00009350: 6f77 290a 0a20 2020 2020 2020 2069 6620  ow)..        if 
+00009360: 6e6f 7420 7365 6c66 2e61 7267 732e 6e6f  not self.args.no
+00009370: 5f64 6176 3a0a 2020 2020 2020 2020 2020  _dav:.          
+00009380: 2020 2320 5052 4f50 5041 5443 482c 204c    # PROPPATCH, L
+00009390: 4f43 4b2c 2055 4e4c 4f43 4b2c 2043 4f50  OCK, UNLOCK, COP
+000093a0: 593a 206e 6f6f 7020 2873 7065 632d 6d75  Y: noop (spec-mu
+000093b0: 7374 290a 2020 2020 2020 2020 2020 2020  st).            
+000093c0: 6f68 5b22 4461 7622 5d20 3d20 2231 2c20  oh["Dav"] = "1, 
+000093d0: 3222 0a20 2020 2020 2020 2020 2020 206f  2".            o
+000093e0: 685b 224d 732d 4175 7468 6f72 2d56 6961  h["Ms-Author-Via
+000093f0: 225d 203d 2022 4441 5622 0a0a 2020 2020  "] = "DAV"..    
+00009400: 2020 2020 2320 7769 6e78 702d 7765 6264      # winxp-webd
+00009410: 6176 2064 6f65 736e 7420 6b6e 6f77 2077  av doesnt know w
+00009420: 6861 7420 3230 3420 6973 0a20 2020 2020  hat 204 is.     
+00009430: 2020 2073 656c 662e 7365 6e64 5f68 6561     self.send_hea
+00009440: 6465 7273 2830 2c20 3230 3029 0a20 2020  ders(0, 200).   
+00009450: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00009460: 0a0a 2020 2020 6465 6620 6861 6e64 6c65  ..    def handle
+00009470: 5f64 656c 6574 6528 7365 6c66 2920 203a  _delete(self)  :
+00009480: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+00009490: 6728 2244 454c 4554 4520 2220 2b20 7365  g("DELETE " + se
+000094a0: 6c66 2e72 6571 290a 2020 2020 2020 2020  lf.req).        
+000094b0: 7265 7475 726e 2073 656c 662e 6861 6e64  return self.hand
+000094c0: 6c65 5f72 6d28 5b5d 290a 0a20 2020 2064  le_rm([])..    d
+000094d0: 6566 2068 616e 646c 655f 7075 7428 7365  ef handle_put(se
+000094e0: 6c66 2920 203a 0a20 2020 2020 2020 2073  lf)  :.        s
+000094f0: 656c 662e 6c6f 6728 2250 5554 2022 202b  elf.log("PUT " +
+00009500: 2073 656c 662e 7265 7129 0a0a 2020 2020   self.req)..    
+00009510: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00009520: 6361 6e5f 7772 6974 653a 0a20 2020 2020  can_write:.     
+00009530: 2020 2020 2020 2074 203d 2022 7573 6572         t = "user
+00009540: 207b 7d20 646f 6573 206e 6f74 2068 6176   {} does not hav
+00009550: 6520 7772 6974 652d 6163 6365 7373 2068  e write-access h
+00009560: 6572 6522 0a20 2020 2020 2020 2020 2020  ere".           
+00009570: 2072 6169 7365 2050 6562 6b61 6328 3430   raise Pebkac(40
+00009580: 332c 2074 2e66 6f72 6d61 7428 7365 6c66  3, t.format(self
+00009590: 2e75 6e61 6d65 2929 0a0a 2020 2020 2020  .uname))..      
+000095a0: 2020 6966 206e 6f74 2073 656c 662e 6172    if not self.ar
+000095b0: 6773 2e6e 6f5f 6461 7620 616e 6420 7365  gs.no_dav and se
+000095c0: 6c66 2e5f 6170 706c 6573 616e 2829 3a0a  lf._applesan():.
+000095d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000095e0: 726e 2073 656c 662e 6865 6164 6572 732e  rn self.headers.
+000095f0: 6765 7428 2263 6f6e 7465 6e74 2d6c 656e  get("content-len
+00009600: 6774 6822 2920 3d3d 2022 3022 0a0a 2020  gth") == "0"..  
+00009610: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+00009620: 6164 6572 732e 6765 7428 2265 7870 6563  aders.get("expec
+00009630: 7422 2c20 2222 292e 6c6f 7765 7228 2920  t", "").lower() 
+00009640: 3d3d 2022 3130 302d 636f 6e74 696e 7565  == "100-continue
+00009650: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
+00009660: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00009670: 2020 2020 7365 6c66 2e73 2e73 6574 7469      self.s.setti
+00009680: 6d65 6f75 7428 4e6f 6e65 290a 2020 2020  meout(None).    
+00009690: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000096a0: 2e73 2e73 656e 6461 6c6c 2862 2248 5454  .s.sendall(b"HTT
+000096b0: 502f 312e 3120 3130 3020 436f 6e74 696e  P/1.1 100 Contin
+000096c0: 7565 5c72 5c6e 5c72 5c6e 2229 0a20 2020  ue\r\n\r\n").   
+000096d0: 2020 2020 2020 2020 2065 7863 6570 743a           except:
+000096e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000096f0: 2072 6169 7365 2050 6562 6b61 6328 3430   raise Pebkac(40
+00009700: 302c 2022 636c 6965 6e74 2064 2f63 2062  0, "client d/c b
+00009710: 6566 6f72 6520 3130 3020 636f 6e74 696e  efore 100 contin
+00009720: 7565 2229 0a0a 2020 2020 2020 2020 7265  ue")..        re
+00009730: 7475 726e 2073 656c 662e 6861 6e64 6c65  turn self.handle
+00009740: 5f73 7461 7368 2854 7275 6529 0a0a 2020  _stash(True)..  
+00009750: 2020 6465 6620 6861 6e64 6c65 5f70 6f73    def handle_pos
+00009760: 7428 7365 6c66 2920 203a 0a20 2020 2020  t(self)  :.     
+00009770: 2020 2073 656c 662e 6c6f 6728 2250 4f53     self.log("POS
+00009780: 5420 2220 2b20 7365 6c66 2e72 6571 290a  T " + self.req).
+00009790: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000097a0: 2e68 6561 6465 7273 2e67 6574 2822 6578  .headers.get("ex
+000097b0: 7065 6374 222c 2022 2229 2e6c 6f77 6572  pect", "").lower
+000097c0: 2829 203d 3d20 2231 3030 2d63 6f6e 7469  () == "100-conti
+000097d0: 6e75 6522 3a0a 2020 2020 2020 2020 2020  nue":.          
+000097e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000097f0: 2020 2020 2020 2073 656c 662e 732e 7365         self.s.se
+00009800: 7474 696d 656f 7574 284e 6f6e 6529 0a20  ttimeout(None). 
+00009810: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009820: 656c 662e 732e 7365 6e64 616c 6c28 6222  elf.s.sendall(b"
+00009830: 4854 5450 2f31 2e31 2031 3030 2043 6f6e  HTTP/1.1 100 Con
+00009840: 7469 6e75 655c 725c 6e5c 725c 6e22 290a  tinue\r\n\r\n").
+00009850: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00009860: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+00009870: 2020 2020 7261 6973 6520 5065 626b 6163      raise Pebkac
+00009880: 2834 3030 2c20 2263 6c69 656e 7420 642f  (400, "client d/
+00009890: 6320 6265 666f 7265 2031 3030 2063 6f6e  c before 100 con
+000098a0: 7469 6e75 6522 290a 0a20 2020 2020 2020  tinue")..       
+000098b0: 2069 6620 2272 6177 2220 696e 2073 656c   if "raw" in sel
+000098c0: 662e 7570 6172 616d 3a0a 2020 2020 2020  f.uparam:.      
+000098d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000098e0: 662e 6861 6e64 6c65 5f73 7461 7368 2846  f.handle_stash(F
+000098f0: 616c 7365 290a 0a20 2020 2020 2020 2063  alse)..        c
+00009900: 7479 7065 203d 2073 656c 662e 6865 6164  type = self.head
+00009910: 6572 732e 6765 7428 2263 6f6e 7465 6e74  ers.get("content
+00009920: 2d74 7970 6522 2c20 2222 292e 6c6f 7765  -type", "").lowe
+00009930: 7228 290a 0a20 2020 2020 2020 2069 6620  r()..        if 
+00009940: 226d 756c 7469 7061 7274 2f66 6f72 6d2d  "multipart/form-
+00009950: 6461 7461 2220 696e 2063 7479 7065 3a0a  data" in ctype:.
+00009960: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009970: 726e 2073 656c 662e 6861 6e64 6c65 5f70  rn self.handle_p
+00009980: 6f73 745f 6d75 6c74 6970 6172 7428 290a  ost_multipart().
+00009990: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
+000099a0: 2020 2020 2020 2020 2020 2261 7070 6c69            "appli
+000099b0: 6361 7469 6f6e 2f6a 736f 6e22 2069 6e20  cation/json" in 
+000099c0: 6374 7970 650a 2020 2020 2020 2020 2020  ctype.          
+000099d0: 2020 6f72 2022 7465 7874 2f70 6c61 696e    or "text/plain
+000099e0: 2220 696e 2063 7479 7065 0a20 2020 2020  " in ctype.     
+000099f0: 2020 2020 2020 206f 7220 2261 7070 6c69         or "appli
+00009a00: 6361 7469 6f6e 2f78 6d6c 2220 696e 2063  cation/xml" in c
+00009a10: 7479 7065 0a20 2020 2020 2020 2029 3a0a  type.        ):.
+00009a20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009a30: 726e 2073 656c 662e 6861 6e64 6c65 5f70  rn self.handle_p
+00009a40: 6f73 745f 6a73 6f6e 2829 0a0a 2020 2020  ost_json()..    
+00009a50: 2020 2020 6966 2022 6d6f 7665 2220 696e      if "move" in
+00009a60: 2073 656c 662e 7570 6172 616d 3a0a 2020   self.uparam:.  
+00009a70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009a80: 2073 656c 662e 6861 6e64 6c65 5f6d 7628   self.handle_mv(
+00009a90: 290a 0a20 2020 2020 2020 2069 6620 2264  )..        if "d
+00009aa0: 656c 6574 6522 2069 6e20 7365 6c66 2e75  elete" in self.u
+00009ab0: 7061 7261 6d3a 0a20 2020 2020 2020 2020  param:.         
+00009ac0: 2020 2072 6574 7572 6e20 7365 6c66 2e68     return self.h
+00009ad0: 616e 646c 655f 726d 285b 5d29 0a0a 2020  andle_rm([])..  
+00009ae0: 2020 2020 2020 6966 2022 6170 706c 6963        if "applic
+00009af0: 6174 696f 6e2f 6f63 7465 742d 7374 7265  ation/octet-stre
+00009b00: 616d 2220 696e 2063 7479 7065 3a0a 2020  am" in ctype:.  
+00009b10: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009b20: 2073 656c 662e 6861 6e64 6c65 5f70 6f73   self.handle_pos
+00009b30: 745f 6269 6e61 7279 2829 0a0a 2020 2020  t_binary()..    
+00009b40: 2020 2020 6966 2022 6170 706c 6963 6174      if "applicat
+00009b50: 696f 6e2f 782d 7777 772d 666f 726d 2d75  ion/x-www-form-u
+00009b60: 726c 656e 636f 6465 6422 2069 6e20 6374  rlencoded" in ct
+00009b70: 7970 653a 0a20 2020 2020 2020 2020 2020  ype:.           
+00009b80: 206f 7074 203d 2073 656c 662e 6172 6773   opt = self.args
+00009b90: 2e75 726c 666f 726d 0a20 2020 2020 2020  .urlform.       
+00009ba0: 2020 2020 2069 6620 2273 7461 7368 2220       if "stash" 
+00009bb0: 696e 206f 7074 3a0a 2020 2020 2020 2020  in opt:.        
+00009bc0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00009bd0: 656c 662e 6861 6e64 6c65 5f73 7461 7368  elf.handle_stash
+00009be0: 2846 616c 7365 290a 0a20 2020 2020 2020  (False)..       
+00009bf0: 2020 2020 2069 6620 2273 6176 6522 2069       if "save" i
+00009c00: 6e20 6f70 743a 0a20 2020 2020 2020 2020  n opt:.         
+00009c10: 2020 2020 2020 2070 6f73 745f 737a 2c20         post_sz, 
+00009c20: 5f2c 205f 2c20 5f2c 2070 6174 682c 205f  _, _, _, path, _
+00009c30: 203d 2073 656c 662e 6475 6d70 5f74 6f5f   = self.dump_to_
+00009c40: 6669 6c65 2846 616c 7365 290a 2020 2020  file(False).    
+00009c50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009c60: 2e6c 6f67 2822 7572 6c66 6f72 6d3a 207b  .log("urlform: {
+00009c70: 7d20 6279 7465 732c 207b 7d22 2e66 6f72  } bytes, {}".for
+00009c80: 6d61 7428 706f 7374 5f73 7a2c 2070 6174  mat(post_sz, pat
+00009c90: 6829 290a 2020 2020 2020 2020 2020 2020  h)).            
+00009ca0: 656c 6966 2022 7072 696e 7422 2069 6e20  elif "print" in 
+00009cb0: 6f70 743a 0a20 2020 2020 2020 2020 2020  opt:.           
+00009cc0: 2020 2020 2072 6561 6465 722c 205f 203d       reader, _ =
+00009cd0: 2073 656c 662e 6765 745f 626f 6479 5f72   self.get_body_r
+00009ce0: 6561 6465 7228 290a 2020 2020 2020 2020  eader().        
+00009cf0: 2020 2020 2020 2020 6275 6620 3d20 6222          buf = b"
+00009d00: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00009d10: 2020 666f 7220 7262 7566 2069 6e20 7265    for rbuf in re
+00009d20: 6164 6572 3a0a 2020 2020 2020 2020 2020  ader:.          
+00009d30: 2020 2020 2020 2020 2020 6275 6620 2b3d            buf +=
+00009d40: 2072 6275 660a 2020 2020 2020 2020 2020   rbuf.          
+00009d50: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00009d60: 2072 6275 6620 6f72 206c 656e 2862 7566   rbuf or len(buf
+00009d70: 2920 3e3d 2033 3237 3638 3a0a 2020 2020  ) >= 32768:.    
 00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d90: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-00009da0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00009db0: 6620 6275 663a 0a20 2020 2020 2020 2020  f buf:.         
-00009dc0: 2020 2020 2020 2020 2020 206f 7269 6720             orig 
-00009dd0: 3d20 6275 662e 6465 636f 6465 2822 7574  = buf.decode("ut
-00009de0: 662d 3822 2c20 2272 6570 6c61 6365 2229  f-8", "replace")
-00009df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e00: 2020 2020 2074 203d 2022 7572 6c66 6f72       t = "urlfor
-00009e10: 6d5f 7261 7720 7b7d 2040 207b 7d5c 6e20  m_raw {} @ {}\n 
-00009e20: 207b 7d5c 6e22 0a20 2020 2020 2020 2020   {}\n".         
-00009e30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009e40: 6c6f 6728 742e 666f 726d 6174 286c 656e  log(t.format(len
-00009e50: 286f 7269 6729 2c20 7365 6c66 2e76 7061  (orig), self.vpa
-00009e60: 7468 2c20 6f72 6967 2929 0a20 2020 2020  th, orig)).     
-00009e70: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00009e80: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00009e90: 2020 2020 2020 2020 2020 2020 7a62 203d              zb =
-00009ea0: 2075 6e71 756f 7465 2862 7566 2e72 6570   unquote(buf.rep
-00009eb0: 6c61 6365 2862 222b 222c 2062 2220 2229  lace(b"+", b" ")
-00009ec0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009ed0: 2020 2020 2020 2020 2020 706c 6169 6e20            plain 
-00009ee0: 3d20 7a62 2e64 6563 6f64 6528 2275 7466  = zb.decode("utf
-00009ef0: 2d38 222c 2022 7265 706c 6163 6522 290a  -8", "replace").
+00009d90: 2020 2020 6272 6561 6b0a 0a20 2020 2020      break..     
+00009da0: 2020 2020 2020 2020 2020 2069 6620 6275             if bu
+00009db0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
+00009dc0: 2020 2020 2020 206f 7269 6720 3d20 6275         orig = bu
+00009dd0: 662e 6465 636f 6465 2822 7574 662d 3822  f.decode("utf-8"
+00009de0: 2c20 2272 6570 6c61 6365 2229 0a20 2020  , "replace").   
+00009df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e00: 2074 203d 2022 7572 6c66 6f72 6d5f 7261   t = "urlform_ra
+00009e10: 7720 7b7d 2040 207b 7d5c 6e20 207b 7d5c  w {} @ {}\n  {}\
+00009e20: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
+00009e30: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
+00009e40: 742e 666f 726d 6174 286c 656e 286f 7269  t.format(len(ori
+00009e50: 6729 2c20 7365 6c66 2e76 7061 7468 2c20  g), self.vpath, 
+00009e60: 6f72 6967 2929 0a20 2020 2020 2020 2020  orig)).         
+00009e70: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00009e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e90: 2020 2020 2020 2020 7a62 203d 2075 6e71          zb = unq
+00009ea0: 756f 7465 2862 7566 2e72 6570 6c61 6365  uote(buf.replace
+00009eb0: 2862 222b 222c 2062 2220 2229 290a 2020  (b"+", b" ")).  
+00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ed0: 2020 2020 2020 706c 6169 6e20 3d20 7a62        plain = zb
+00009ee0: 2e64 6563 6f64 6528 2275 7466 2d38 222c  .decode("utf-8",
+00009ef0: 2022 7265 706c 6163 6522 290a 2020 2020   "replace").    
 00009f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f10: 2020 2020 2020 2020 6966 2062 7566 2e73          if buf.s
-00009f20: 7461 7274 7377 6974 6828 6222 6d73 673d  tartswith(b"msg=
-00009f30: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00009f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f50: 706c 6169 6e20 3d20 706c 6169 6e5b 343a  plain = plain[4:
-00009f60: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00009f70: 2020 2020 2020 2020 2020 2020 2020 7666                vf
-00009f80: 732c 2072 656d 203d 2073 656c 662e 6173  s, rem = self.as
-00009f90: 7276 2e76 6673 2e67 6574 280a 2020 2020  rv.vfs.get(.    
+00009f10: 2020 2020 6966 2062 7566 2e73 7461 7274      if buf.start
+00009f20: 7377 6974 6828 6222 6d73 673d 2229 3a0a  swith(b"msg="):.
+00009f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f40: 2020 2020 2020 2020 2020 2020 706c 6169              plai
+00009f50: 6e20 3d20 706c 6169 6e5b 343a 5d0a 2020  n = plain[4:].  
+00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f70: 2020 2020 2020 2020 2020 7666 732c 2072            vfs, r
+00009f80: 656d 203d 2073 656c 662e 6173 7276 2e76  em = self.asrv.v
+00009f90: 6673 2e67 6574 280a 2020 2020 2020 2020  fs.get(.        
 00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009fc0: 2e76 7061 7468 2c20 7365 6c66 2e75 6e61  .vpath, self.una
-00009fd0: 6d65 2c20 4661 6c73 652c 2046 616c 7365  me, False, False
-00009fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ff0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00009fb0: 2020 2020 2020 2020 7365 6c66 2e76 7061          self.vpa
+00009fc0: 7468 2c20 7365 6c66 2e75 6e61 6d65 2c20  th, self.uname, 
+00009fd0: 4661 6c73 652c 2046 616c 7365 0a20 2020  False, False.   
+00009fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ff0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
 0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a010: 2020 2020 2020 2020 2020 2078 6d20 3d20             xm = 
-0000a020: 7666 732e 666c 6167 732e 6765 7428 2278  vfs.flags.get("x
-0000a030: 6d22 290a 2020 2020 2020 2020 2020 2020  m").            
-0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a050: 6966 2078 6d3a 0a20 2020 2020 2020 2020  if xm:.         
+0000a010: 2020 2020 2020 2078 6d20 3d20 7666 732e         xm = vfs.
+0000a020: 666c 6167 732e 6765 7428 2278 6d22 290a  flags.get("xm").
+0000a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a040: 2020 2020 2020 2020 2020 2020 6966 2078              if x
+0000a050: 6d3a 0a20 2020 2020 2020 2020 2020 2020  m:.             
 0000a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a070: 2020 2020 2020 2072 756e 686f 6f6b 280a         runhook(.
+0000a070: 2020 2072 756e 686f 6f6b 280a 2020 2020     runhook(.    
 0000a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0a0: 2020 2020 7365 6c66 2e6c 6f67 2c0a 2020      self.log,.  
+0000a0a0: 7365 6c66 2e6c 6f67 2c0a 2020 2020 2020  self.log,.      
 0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0d0: 2020 786d 2c0a 2020 2020 2020 2020 2020    xm,.          
+0000a0c0: 2020 2020 2020 2020 2020 2020 2020 786d                xm
+0000a0d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0f0: 2020 2020 2020 2020 2020 7666 732e 6361            vfs.ca
-0000a100: 6e6f 6e69 6361 6c28 7265 6d29 2c0a 2020  nonical(rem),.  
+0000a0f0: 2020 2020 2020 7666 732e 6361 6e6f 6e69        vfs.canoni
+0000a100: 6361 6c28 7265 6d29 2c0a 2020 2020 2020  cal(rem),.      
 0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a130: 2020 7365 6c66 2e76 7061 7468 2c0a 2020    self.vpath,.  
+0000a120: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a130: 6c66 2e76 7061 7468 2c0a 2020 2020 2020  lf.vpath,.      
 0000a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a160: 2020 7365 6c66 2e68 6f73 742c 0a20 2020    self.host,.   
+0000a150: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a160: 6c66 2e68 6f73 742c 0a20 2020 2020 2020  lf.host,.       
 0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a190: 2073 656c 662e 756e 616d 652c 0a20 2020   self.uname,.   
+0000a180: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a190: 662e 756e 616d 652c 0a20 2020 2020 2020  f.uname,.       
 0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1c0: 2074 696d 652e 7469 6d65 2829 2c0a 2020   time.time(),.  
+0000a1b0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+0000a1c0: 652e 7469 6d65 2829 2c0a 2020 2020 2020  e.time(),.      
 0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1f0: 2020 6c65 6e28 786d 292c 0a20 2020 2020    len(xm),.     
+0000a1e0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0000a1f0: 6e28 786d 292c 0a20 2020 2020 2020 2020  n(xm),.         
 0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a210: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a220: 656c 662e 6970 2c0a 2020 2020 2020 2020  elf.ip,.        
+0000a210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a220: 6970 2c0a 2020 2020 2020 2020 2020 2020  ip,.            
 0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a240: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000a250: 2e74 696d 6528 292c 0a20 2020 2020 2020  .time(),.       
+0000a240: 2020 2020 2020 2020 7469 6d65 2e74 696d          time.tim
+0000a250: 6528 292c 0a20 2020 2020 2020 2020 2020  e(),.           
 0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a270: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-0000a280: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
+0000a270: 2020 2020 2020 2020 2070 6c61 696e 2c0a           plain,.
+0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2a0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000a2c0: 203d 2022 7572 6c66 6f72 6d5f 6465 6320   = "urlform_dec 
-0000a2d0: 7b7d 2040 207b 7d5c 6e20 207b 7d5c 6e22  {} @ {}\n  {}\n"
-0000a2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a2f0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-0000a300: 6728 742e 666f 726d 6174 286c 656e 2870  g(t.format(len(p
-0000a310: 6c61 696e 292c 2073 656c 662e 7670 6174  lain), self.vpat
-0000a320: 682c 2070 6c61 696e 2929 0a0a 2020 2020  h, plain))..    
-0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a340: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0000a350: 2061 7320 6578 3a0a 2020 2020 2020 2020   as ex:.        
-0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a370: 7365 6c66 2e6c 6f67 2872 6570 7228 6578  self.log(repr(ex
-0000a380: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
-0000a390: 6966 2022 6765 7422 2069 6e20 6f70 743a  if "get" in opt:
-0000a3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a3b0: 2072 6574 7572 6e20 7365 6c66 2e68 616e   return self.han
-0000a3c0: 646c 655f 6765 7428 290a 0a20 2020 2020  dle_get()..     
-0000a3d0: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
-0000a3e0: 6b61 6328 3430 352c 2022 504f 5354 287b  kac(405, "POST({
-0000a3f0: 7d29 2069 7320 6469 7361 626c 6564 2069  }) is disabled i
-0000a400: 6e20 7365 7276 6572 2063 6f6e 6669 6722  n server config"
-0000a410: 2e66 6f72 6d61 7428 6374 7970 6529 290a  .format(ctype)).
-0000a420: 0a20 2020 2020 2020 2072 6169 7365 2050  .        raise P
-0000a430: 6562 6b61 6328 3430 352c 2022 646f 6e27  ebkac(405, "don'
-0000a440: 7420 6b6e 6f77 2068 6f77 2074 6f20 6861  t know how to ha
-0000a450: 6e64 6c65 2050 4f53 5428 7b7d 2922 2e66  ndle POST({})".f
-0000a460: 6f72 6d61 7428 6374 7970 6529 290a 0a20  ormat(ctype)).. 
-0000a470: 2020 2064 6566 2067 6574 5f78 6d6c 5f65     def get_xml_e
-0000a480: 6e63 2873 656c 662c 2074 7874 2029 2020  nc(self, txt )  
-0000a490: 3a0a 2020 2020 2020 2020 6f66 7320 3d20  :.        ofs = 
-0000a4a0: 7478 745b 3a35 3132 5d2e 6669 6e64 2827  txt[:512].find('
-0000a4b0: 2065 6e63 6f64 696e 673d 2227 290a 2020   encoding="').  
-0000a4c0: 2020 2020 2020 656e 6320 3d20 2222 0a20        enc = "". 
-0000a4d0: 2020 2020 2020 2069 6620 6f66 7320 2b20         if ofs + 
-0000a4e0: 313a 0a20 2020 2020 2020 2020 2020 2065  1:.            e
-0000a4f0: 6e63 203d 2074 7874 5b6f 6673 202b 2036  nc = txt[ofs + 6
-0000a500: 203a 5d2e 7370 6c69 7428 2722 2729 5b31   :].split('"')[1
-0000a510: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-0000a520: 2020 2020 2020 2020 2020 2020 656e 6320              enc 
-0000a530: 3d20 7365 6c66 2e68 6561 6465 7273 2e67  = self.headers.g
-0000a540: 6574 2822 636f 6e74 656e 742d 7479 7065  et("content-type
-0000a550: 222c 2022 2229 2e6c 6f77 6572 2829 0a20  ", "").lower(). 
-0000a560: 2020 2020 2020 2020 2020 206f 6673 203d             ofs =
-0000a570: 2065 6e63 2e66 696e 6428 2263 6861 7273   enc.find("chars
-0000a580: 6574 3d22 290a 2020 2020 2020 2020 2020  et=").          
-0000a590: 2020 6966 206f 6673 202b 2031 3a0a 2020    if ofs + 1:.  
-0000a5a0: 2020 2020 2020 2020 2020 2020 2020 656e                en
-0000a5b0: 6320 3d20 656e 635b 6f66 7320 2b20 345d  c = enc[ofs + 4]
-0000a5c0: 2e73 706c 6974 2822 3d22 295b 315d 2e73  .split("=")[1].s
-0000a5d0: 706c 6974 2822 3b22 295b 305d 2e73 7472  plit(";")[0].str
-0000a5e0: 6970 2822 5c22 2722 290a 2020 2020 2020  ip("\"'").      
-0000a5f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000a600: 2020 2020 2020 2020 2020 2020 656e 6320              enc 
-0000a610: 3d20 2222 0a0a 2020 2020 2020 2020 7265  = ""..        re
-0000a620: 7475 726e 2065 6e63 206f 7220 2275 7466  turn enc or "utf
-0000a630: 2d38 220a 0a20 2020 2064 6566 2067 6574  -8"..    def get
-0000a640: 5f62 6f64 795f 7265 6164 6572 2873 656c  _body_reader(sel
-0000a650: 6629 2020 2020 203a 0a20 2020 2020 2020  f)     :.       
-0000a660: 2069 6620 2263 6875 6e6b 6564 2220 696e   if "chunked" in
-0000a670: 2073 656c 662e 6865 6164 6572 732e 6765   self.headers.ge
-0000a680: 7428 2274 7261 6e73 6665 722d 656e 636f  t("transfer-enco
-0000a690: 6469 6e67 222c 2022 2229 2e6c 6f77 6572  ding", "").lower
-0000a6a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000a6b0: 7265 7475 726e 2072 6561 645f 736f 636b  return read_sock
-0000a6c0: 6574 5f63 6875 6e6b 6564 2873 656c 662e  et_chunked(self.
-0000a6d0: 7372 292c 202d 310a 0a20 2020 2020 2020  sr), -1..       
-0000a6e0: 2072 656d 6169 6e73 203d 2069 6e74 2873   remains = int(s
-0000a6f0: 656c 662e 6865 6164 6572 732e 6765 7428  elf.headers.get(
-0000a700: 2263 6f6e 7465 6e74 2d6c 656e 6774 6822  "content-length"
-0000a710: 2c20 2d31 2929 0a20 2020 2020 2020 2069  , -1)).        i
-0000a720: 6620 7265 6d61 696e 7320 3d3d 202d 313a  f remains == -1:
-0000a730: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000a740: 662e 6b65 6570 616c 6976 6520 3d20 4661  f.keepalive = Fa
-0000a750: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-0000a760: 7265 7475 726e 2072 6561 645f 736f 636b  return read_sock
-0000a770: 6574 5f75 6e62 6f75 6e64 6564 2873 656c  et_unbounded(sel
-0000a780: 662e 7372 292c 2072 656d 6169 6e73 0a20  f.sr), remains. 
-0000a790: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000a7a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000a7b0: 7265 6164 5f73 6f63 6b65 7428 7365 6c66  read_socket(self
-0000a7c0: 2e73 722c 2072 656d 6169 6e73 292c 2072  .sr, remains), r
-0000a7d0: 656d 6169 6e73 0a0a 2020 2020 6465 6620  emains..    def 
-0000a7e0: 6475 6d70 5f74 6f5f 6669 6c65 2873 656c  dump_to_file(sel
-0000a7f0: 662c 2069 735f 7075 7420 2920 2020 2020  f, is_put )     
-0000a800: 2020 3a0a 2020 2020 2020 2020 2320 706f    :.        # po
-0000a810: 7374 5f73 7a2c 2073 6861 5f68 6578 2c20  st_sz, sha_hex, 
-0000a820: 7368 615f 6236 342c 2072 656d 6169 6e73  sha_b64, remains
-0000a830: 2c20 7061 7468 2c20 7572 6c0a 2020 2020  , path, url.    
-0000a840: 2020 2020 7265 6164 6572 2c20 7265 6d61      reader, rema
-0000a850: 696e 7320 3d20 7365 6c66 2e67 6574 5f62  ins = self.get_b
-0000a860: 6f64 795f 7265 6164 6572 2829 0a20 2020  ody_reader().   
-0000a870: 2020 2020 2076 6673 2c20 7265 6d20 3d20       vfs, rem = 
-0000a880: 7365 6c66 2e61 7372 762e 7666 732e 6765  self.asrv.vfs.ge
-0000a890: 7428 7365 6c66 2e76 7061 7468 2c20 7365  t(self.vpath, se
-0000a8a0: 6c66 2e75 6e61 6d65 2c20 4661 6c73 652c  lf.uname, False,
-0000a8b0: 2054 7275 6529 0a20 2020 2020 2020 2072   True).        r
-0000a8c0: 6e64 2c20 5f2c 206c 6966 6574 696d 652c  nd, _, lifetime,
-0000a8d0: 2078 6275 2c20 7861 7520 3d20 7365 6c66   xbu, xau = self
-0000a8e0: 2e75 706c 6f61 645f 666c 6167 7328 7666  .upload_flags(vf
-0000a8f0: 7329 0a20 2020 2020 2020 206c 696d 203d  s).        lim =
-0000a900: 2076 6673 2e67 6574 5f64 6276 2872 656d   vfs.get_dbv(rem
-0000a910: 295b 305d 2e6c 696d 0a20 2020 2020 2020  )[0].lim.       
-0000a920: 2066 6469 7220 3d20 7666 732e 6361 6e6f   fdir = vfs.cano
-0000a930: 6e69 6361 6c28 7265 6d29 0a20 2020 2020  nical(rem).     
-0000a940: 2020 2069 6620 6c69 6d3a 0a20 2020 2020     if lim:.     
-0000a950: 2020 2020 2020 2066 6469 722c 2072 656d         fdir, rem
-0000a960: 203d 206c 696d 2e61 6c6c 2873 656c 662e   = lim.all(self.
-0000a970: 6970 2c20 7265 6d2c 2072 656d 6169 6e73  ip, rem, remains
-0000a980: 2c20 6664 6972 290a 0a20 2020 2020 2020  , fdir)..       
-0000a990: 2066 6e20 3d20 4e6f 6e65 0a20 2020 2020   fn = None.     
-0000a9a0: 2020 2069 6620 7265 6d20 616e 6420 6e6f     if rem and no
-0000a9b0: 7420 7365 6c66 2e74 7261 696c 696e 675f  t self.trailing_
-0000a9c0: 736c 6173 6820 616e 6420 6e6f 7420 626f  slash and not bo
-0000a9d0: 732e 7061 7468 2e69 7364 6972 2866 6469  s.path.isdir(fdi
-0000a9e0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0000a9f0: 6664 6972 2c20 666e 203d 206f 732e 7061  fdir, fn = os.pa
-0000aa00: 7468 2e73 706c 6974 2866 6469 7229 0a20  th.split(fdir). 
-0000aa10: 2020 2020 2020 2020 2020 2072 656d 2c20             rem, 
-0000aa20: 5f20 3d20 7673 706c 6974 2872 656d 290a  _ = vsplit(rem).
-0000aa30: 0a20 2020 2020 2020 2062 6f73 2e6d 616b  .        bos.mak
-0000aa40: 6564 6972 7328 6664 6972 290a 0a20 2020  edirs(fdir)..   
-0000aa50: 2020 2020 206f 7065 6e5f 6b61 2020 203d       open_ka   =
-0000aa60: 207b 2266 756e 223a 206f 7065 6e7d 0a20   {"fun": open}. 
-0000aa70: 2020 2020 2020 206f 7065 6e5f 6120 3d20         open_a = 
-0000aa80: 5b22 7762 222c 2035 3132 202a 2031 3032  ["wb", 512 * 102
-0000aa90: 345d 0a0a 2020 2020 2020 2020 2320 7573  4]..        # us
-0000aaa0: 6572 2d72 6571 7565 7374 207c 7c20 636f  er-request || co
-0000aab0: 6e66 6967 2d66 6f72 6365 0a20 2020 2020  nfig-force.     
-0000aac0: 2020 2069 6620 2822 677a 2220 696e 2076     if ("gz" in v
-0000aad0: 6673 2e66 6c61 6773 206f 7220 2278 7a22  fs.flags or "xz"
-0000aae0: 2069 6e20 7666 732e 666c 6167 7329 2061   in vfs.flags) a
-0000aaf0: 6e64 2028 0a20 2020 2020 2020 2020 2020  nd (.           
-0000ab00: 2022 706b 2220 696e 2076 6673 2e66 6c61   "pk" in vfs.fla
-0000ab10: 6773 0a20 2020 2020 2020 2020 2020 206f  gs.            o
-0000ab20: 7220 2270 6b22 2069 6e20 7365 6c66 2e75  r "pk" in self.u
-0000ab30: 7061 7261 6d0a 2020 2020 2020 2020 2020  param.          
-0000ab40: 2020 6f72 2022 677a 2220 696e 2073 656c    or "gz" in sel
-0000ab50: 662e 7570 6172 616d 0a20 2020 2020 2020  f.uparam.       
-0000ab60: 2020 2020 206f 7220 2278 7a22 2069 6e20       or "xz" in 
-0000ab70: 7365 6c66 2e75 7061 7261 6d0a 2020 2020  self.uparam.    
-0000ab80: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-0000ab90: 2020 2066 6220 3d20 7b22 677a 223a 2039     fb = {"gz": 9
-0000aba0: 2c20 2278 7a22 3a20 307d 2020 2320 6465  , "xz": 0}  # de
-0000abb0: 6661 756c 742f 6661 6c6c 6261 636b 206c  fault/fallback l
-0000abc0: 6576 656c 0a20 2020 2020 2020 2020 2020  evel.           
-0000abd0: 206c 7620 3d20 7b7d 2020 2320 7365 6c65   lv = {}  # sele
-0000abe0: 6374 6564 206c 6576 656c 0a20 2020 2020  cted level.     
-0000abf0: 2020 2020 2020 2061 6c67 203d 2022 2220         alg = "" 
-0000ac00: 2023 2073 656c 6563 7465 6420 616c 676f   # selected algo
-0000ac10: 2028 677a 3d70 7265 6665 7272 6564 290a   (gz=preferred).
-0000ac20: 0a20 2020 2020 2020 2020 2020 2023 2075  .            # u
-0000ac30: 7365 722d 7072 6566 7320 6669 7273 740a  ser-prefs first.
-0000ac40: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-0000ac50: 677a 2220 696e 2073 656c 662e 7570 6172  gz" in self.upar
-0000ac60: 616d 206f 7220 2270 6b22 2069 6e20 7365  am or "pk" in se
-0000ac70: 6c66 2e75 7061 7261 6d3a 2020 2320 6465  lf.uparam:  # de
-0000ac80: 662e 706b 0a20 2020 2020 2020 2020 2020  f.pk.           
-0000ac90: 2020 2020 2061 6c67 203d 2022 677a 220a       alg = "gz".
-0000aca0: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-0000acb0: 787a 2220 696e 2073 656c 662e 7570 6172  xz" in self.upar
-0000acc0: 616d 3a0a 2020 2020 2020 2020 2020 2020  am:.            
-0000acd0: 2020 2020 616c 6720 3d20 2278 7a22 0a20      alg = "xz". 
-0000ace0: 2020 2020 2020 2020 2020 2069 6620 616c             if al
-0000acf0: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-0000ad00: 2020 207a 736f 203d 2073 656c 662e 7570     zso = self.up
-0000ad10: 6172 616d 2e67 6574 2861 6c67 290a 2020  aram.get(alg).  
-0000ad20: 2020 2020 2020 2020 2020 2020 2020 6c76                lv
-0000ad30: 5b61 6c67 5d20 3d20 6662 5b61 6c67 5d20  [alg] = fb[alg] 
-0000ad40: 6966 207a 736f 2069 7320 4e6f 6e65 2065  if zso is None e
-0000ad50: 6c73 6520 696e 7428 7a73 6f29 0a0a 2020  lse int(zso)..  
-0000ad60: 2020 2020 2020 2020 2020 6966 2061 6c67            if alg
-0000ad70: 206e 6f74 2069 6e20 7666 732e 666c 6167   not in vfs.flag
-0000ad80: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000ad90: 2020 2061 6c67 203d 2022 677a 2220 6966     alg = "gz" if
-0000ada0: 2022 677a 2220 696e 2076 6673 2e66 6c61   "gz" in vfs.fla
-0000adb0: 6773 2065 6c73 6520 2278 7a22 0a0a 2020  gs else "xz"..  
-0000adc0: 2020 2020 2020 2020 2020 2320 7468 656e            # then
-0000add0: 2073 6572 7665 7220 6f76 6572 7269 6465   server override
-0000ade0: 730a 2020 2020 2020 2020 2020 2020 706b  s.            pk
-0000adf0: 203d 2076 6673 2e66 6c61 6773 2e67 6574   = vfs.flags.get
-0000ae00: 2822 706b 2229 0a20 2020 2020 2020 2020  ("pk").         
-0000ae10: 2020 2069 6620 706b 2069 7320 6e6f 7420     if pk is not 
-0000ae20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000ae30: 2020 2020 2020 2320 636f 6e66 6967 2d66        # config-f
-0000ae40: 6f72 6365 6420 6f6e 0a20 2020 2020 2020  orced on.       
-0000ae50: 2020 2020 2020 2020 2061 6c67 203d 2061           alg = a
-0000ae60: 6c67 206f 7220 2267 7a22 2020 2320 6465  lg or "gz"  # de
-0000ae70: 662e 706b 0a20 2020 2020 2020 2020 2020  f.pk.           
-0000ae80: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000ae90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000aea0: 636f 6e66 6967 2d66 6f72 6365 6420 6f70  config-forced op
-0000aeb0: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
-0000aec0: 2020 2020 2020 2061 6c67 2c20 6e6c 7620         alg, nlv 
-0000aed0: 3d20 706b 2e73 706c 6974 2822 2c22 290a  = pk.split(",").
+0000a2a0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a2b0: 2020 2020 2020 2020 2020 2074 203d 2022             t = "
+0000a2c0: 7572 6c66 6f72 6d5f 6465 6320 7b7d 2040  urlform_dec {} @
+0000a2d0: 207b 7d5c 6e20 207b 7d5c 6e22 0a20 2020   {}\n  {}\n".   
+0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2f0: 2020 2020 2073 656c 662e 6c6f 6728 742e       self.log(t.
+0000a300: 666f 726d 6174 286c 656e 2870 6c61 696e  format(len(plain
+0000a310: 292c 2073 656c 662e 7670 6174 682c 2070  ), self.vpath, p
+0000a320: 6c61 696e 2929 0a0a 2020 2020 2020 2020  lain))..        
+0000a330: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0000a340: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+0000a350: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
+0000a360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a370: 2e6c 6f67 2872 6570 7228 6578 2929 0a0a  .log(repr(ex))..
+0000a380: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+0000a390: 6765 7422 2069 6e20 6f70 743a 0a20 2020  get" in opt:.   
+0000a3a0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000a3b0: 7572 6e20 7365 6c66 2e68 616e 646c 655f  urn self.handle_
+0000a3c0: 6765 7428 290a 0a20 2020 2020 2020 2020  get()..         
+0000a3d0: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
+0000a3e0: 3430 352c 2022 504f 5354 287b 7d29 2069  405, "POST({}) i
+0000a3f0: 7320 6469 7361 626c 6564 2069 6e20 7365  s disabled in se
+0000a400: 7276 6572 2063 6f6e 6669 6722 2e66 6f72  rver config".for
+0000a410: 6d61 7428 6374 7970 6529 290a 0a20 2020  mat(ctype))..   
+0000a420: 2020 2020 2072 6169 7365 2050 6562 6b61       raise Pebka
+0000a430: 6328 3430 352c 2022 646f 6e27 7420 6b6e  c(405, "don't kn
+0000a440: 6f77 2068 6f77 2074 6f20 6861 6e64 6c65  ow how to handle
+0000a450: 2050 4f53 5428 7b7d 2922 2e66 6f72 6d61   POST({})".forma
+0000a460: 7428 6374 7970 6529 290a 0a20 2020 2064  t(ctype))..    d
+0000a470: 6566 2067 6574 5f78 6d6c 5f65 6e63 2873  ef get_xml_enc(s
+0000a480: 656c 662c 2074 7874 2029 2020 3a0a 2020  elf, txt )  :.  
+0000a490: 2020 2020 2020 6f66 7320 3d20 7478 745b        ofs = txt[
+0000a4a0: 3a35 3132 5d2e 6669 6e64 2827 2065 6e63  :512].find(' enc
+0000a4b0: 6f64 696e 673d 2227 290a 2020 2020 2020  oding="').      
+0000a4c0: 2020 656e 6320 3d20 2222 0a20 2020 2020    enc = "".     
+0000a4d0: 2020 2069 6620 6f66 7320 2b20 313a 0a20     if ofs + 1:. 
+0000a4e0: 2020 2020 2020 2020 2020 2065 6e63 203d             enc =
+0000a4f0: 2074 7874 5b6f 6673 202b 2036 203a 5d2e   txt[ofs + 6 :].
+0000a500: 7370 6c69 7428 2722 2729 5b31 5d0a 2020  split('"')[1].  
+0000a510: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000a520: 2020 2020 2020 2020 656e 6320 3d20 7365          enc = se
+0000a530: 6c66 2e68 6561 6465 7273 2e67 6574 2822  lf.headers.get("
+0000a540: 636f 6e74 656e 742d 7479 7065 222c 2022  content-type", "
+0000a550: 2229 2e6c 6f77 6572 2829 0a20 2020 2020  ").lower().     
+0000a560: 2020 2020 2020 206f 6673 203d 2065 6e63         ofs = enc
+0000a570: 2e66 696e 6428 2263 6861 7273 6574 3d22  .find("charset="
+0000a580: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000a590: 206f 6673 202b 2031 3a0a 2020 2020 2020   ofs + 1:.      
+0000a5a0: 2020 2020 2020 2020 2020 656e 6320 3d20            enc = 
+0000a5b0: 656e 635b 6f66 7320 2b20 345d 2e73 706c  enc[ofs + 4].spl
+0000a5c0: 6974 2822 3d22 295b 315d 2e73 706c 6974  it("=")[1].split
+0000a5d0: 2822 3b22 295b 305d 2e73 7472 6970 2822  (";")[0].strip("
+0000a5e0: 5c22 2722 290a 2020 2020 2020 2020 2020  \"'").          
+0000a5f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a600: 2020 2020 2020 2020 656e 6320 3d20 2222          enc = ""
+0000a610: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000a620: 2065 6e63 206f 7220 2275 7466 2d38 220a   enc or "utf-8".
+0000a630: 0a20 2020 2064 6566 2067 6574 5f62 6f64  .    def get_bod
+0000a640: 795f 7265 6164 6572 2873 656c 6629 2020  y_reader(self)  
+0000a650: 2020 203a 0a20 2020 2020 2020 2069 6620     :.        if 
+0000a660: 2263 6875 6e6b 6564 2220 696e 2073 656c  "chunked" in sel
+0000a670: 662e 6865 6164 6572 732e 6765 7428 2274  f.headers.get("t
+0000a680: 7261 6e73 6665 722d 656e 636f 6469 6e67  ransfer-encoding
+0000a690: 222c 2022 2229 2e6c 6f77 6572 2829 3a0a  ", "").lower():.
+0000a6a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000a6b0: 726e 2072 6561 645f 736f 636b 6574 5f63  rn read_socket_c
+0000a6c0: 6875 6e6b 6564 2873 656c 662e 7372 292c  hunked(self.sr),
+0000a6d0: 202d 310a 0a20 2020 2020 2020 2072 656d   -1..        rem
+0000a6e0: 6169 6e73 203d 2069 6e74 2873 656c 662e  ains = int(self.
+0000a6f0: 6865 6164 6572 732e 6765 7428 2263 6f6e  headers.get("con
+0000a700: 7465 6e74 2d6c 656e 6774 6822 2c20 2d31  tent-length", -1
+0000a710: 2929 0a20 2020 2020 2020 2069 6620 7265  )).        if re
+0000a720: 6d61 696e 7320 3d3d 202d 313a 0a20 2020  mains == -1:.   
+0000a730: 2020 2020 2020 2020 2073 656c 662e 6b65           self.ke
+0000a740: 6570 616c 6976 6520 3d20 4661 6c73 650a  epalive = False.
+0000a750: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000a760: 726e 2072 6561 645f 736f 636b 6574 5f75  rn read_socket_u
+0000a770: 6e62 6f75 6e64 6564 2873 656c 662e 7372  nbounded(self.sr
+0000a780: 292c 2072 656d 6169 6e73 0a20 2020 2020  ), remains.     
+0000a790: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a7a0: 2020 2020 2072 6574 7572 6e20 7265 6164       return read
+0000a7b0: 5f73 6f63 6b65 7428 7365 6c66 2e73 722c  _socket(self.sr,
+0000a7c0: 2072 656d 6169 6e73 292c 2072 656d 6169   remains), remai
+0000a7d0: 6e73 0a0a 2020 2020 6465 6620 6475 6d70  ns..    def dump
+0000a7e0: 5f74 6f5f 6669 6c65 2873 656c 662c 2069  _to_file(self, i
+0000a7f0: 735f 7075 7420 2920 2020 2020 2020 3a0a  s_put )       :.
+0000a800: 2020 2020 2020 2020 2320 706f 7374 5f73          # post_s
+0000a810: 7a2c 2073 6861 5f68 6578 2c20 7368 615f  z, sha_hex, sha_
+0000a820: 6236 342c 2072 656d 6169 6e73 2c20 7061  b64, remains, pa
+0000a830: 7468 2c20 7572 6c0a 2020 2020 2020 2020  th, url.        
+0000a840: 7265 6164 6572 2c20 7265 6d61 696e 7320  reader, remains 
+0000a850: 3d20 7365 6c66 2e67 6574 5f62 6f64 795f  = self.get_body_
+0000a860: 7265 6164 6572 2829 0a20 2020 2020 2020  reader().       
+0000a870: 2076 6673 2c20 7265 6d20 3d20 7365 6c66   vfs, rem = self
+0000a880: 2e61 7372 762e 7666 732e 6765 7428 7365  .asrv.vfs.get(se
+0000a890: 6c66 2e76 7061 7468 2c20 7365 6c66 2e75  lf.vpath, self.u
+0000a8a0: 6e61 6d65 2c20 4661 6c73 652c 2054 7275  name, False, Tru
+0000a8b0: 6529 0a20 2020 2020 2020 2072 6e64 2c20  e).        rnd, 
+0000a8c0: 5f2c 206c 6966 6574 696d 652c 2078 6275  _, lifetime, xbu
+0000a8d0: 2c20 7861 7520 3d20 7365 6c66 2e75 706c  , xau = self.upl
+0000a8e0: 6f61 645f 666c 6167 7328 7666 7329 0a20  oad_flags(vfs). 
+0000a8f0: 2020 2020 2020 206c 696d 203d 2076 6673         lim = vfs
+0000a900: 2e67 6574 5f64 6276 2872 656d 295b 305d  .get_dbv(rem)[0]
+0000a910: 2e6c 696d 0a20 2020 2020 2020 2066 6469  .lim.        fdi
+0000a920: 7220 3d20 7666 732e 6361 6e6f 6e69 6361  r = vfs.canonica
+0000a930: 6c28 7265 6d29 0a20 2020 2020 2020 2069  l(rem).        i
+0000a940: 6620 6c69 6d3a 0a20 2020 2020 2020 2020  f lim:.         
+0000a950: 2020 2066 6469 722c 2072 656d 203d 206c     fdir, rem = l
+0000a960: 696d 2e61 6c6c 2873 656c 662e 6970 2c20  im.all(self.ip, 
+0000a970: 7265 6d2c 2072 656d 6169 6e73 2c20 6664  rem, remains, fd
+0000a980: 6972 290a 0a20 2020 2020 2020 2066 6e20  ir)..        fn 
+0000a990: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+0000a9a0: 6620 7265 6d20 616e 6420 6e6f 7420 7365  f rem and not se
+0000a9b0: 6c66 2e74 7261 696c 696e 675f 736c 6173  lf.trailing_slas
+0000a9c0: 6820 616e 6420 6e6f 7420 626f 732e 7061  h and not bos.pa
+0000a9d0: 7468 2e69 7364 6972 2866 6469 7229 3a0a  th.isdir(fdir):.
+0000a9e0: 2020 2020 2020 2020 2020 2020 6664 6972              fdir
+0000a9f0: 2c20 666e 203d 206f 732e 7061 7468 2e73  , fn = os.path.s
+0000aa00: 706c 6974 2866 6469 7229 0a20 2020 2020  plit(fdir).     
+0000aa10: 2020 2020 2020 2072 656d 2c20 5f20 3d20         rem, _ = 
+0000aa20: 7673 706c 6974 2872 656d 290a 0a20 2020  vsplit(rem)..   
+0000aa30: 2020 2020 2062 6f73 2e6d 616b 6564 6972       bos.makedir
+0000aa40: 7328 6664 6972 290a 0a20 2020 2020 2020  s(fdir)..       
+0000aa50: 206f 7065 6e5f 6b61 2020 203d 207b 2266   open_ka   = {"f
+0000aa60: 756e 223a 206f 7065 6e7d 0a20 2020 2020  un": open}.     
+0000aa70: 2020 206f 7065 6e5f 6120 3d20 5b22 7762     open_a = ["wb
+0000aa80: 222c 2035 3132 202a 2031 3032 345d 0a0a  ", 512 * 1024]..
+0000aa90: 2020 2020 2020 2020 2320 7573 6572 2d72          # user-r
+0000aaa0: 6571 7565 7374 207c 7c20 636f 6e66 6967  equest || config
+0000aab0: 2d66 6f72 6365 0a20 2020 2020 2020 2069  -force.        i
+0000aac0: 6620 2822 677a 2220 696e 2076 6673 2e66  f ("gz" in vfs.f
+0000aad0: 6c61 6773 206f 7220 2278 7a22 2069 6e20  lags or "xz" in 
+0000aae0: 7666 732e 666c 6167 7329 2061 6e64 2028  vfs.flags) and (
+0000aaf0: 0a20 2020 2020 2020 2020 2020 2022 706b  .            "pk
+0000ab00: 2220 696e 2076 6673 2e66 6c61 6773 0a20  " in vfs.flags. 
+0000ab10: 2020 2020 2020 2020 2020 206f 7220 2270             or "p
+0000ab20: 6b22 2069 6e20 7365 6c66 2e75 7061 7261  k" in self.upara
+0000ab30: 6d0a 2020 2020 2020 2020 2020 2020 6f72  m.            or
+0000ab40: 2022 677a 2220 696e 2073 656c 662e 7570   "gz" in self.up
+0000ab50: 6172 616d 0a20 2020 2020 2020 2020 2020  aram.           
+0000ab60: 206f 7220 2278 7a22 2069 6e20 7365 6c66   or "xz" in self
+0000ab70: 2e75 7061 7261 6d0a 2020 2020 2020 2020  .uparam.        
+0000ab80: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+0000ab90: 6220 3d20 7b22 677a 223a 2039 2c20 2278  b = {"gz": 9, "x
+0000aba0: 7a22 3a20 307d 2020 2320 6465 6661 756c  z": 0}  # defaul
+0000abb0: 742f 6661 6c6c 6261 636b 206c 6576 656c  t/fallback level
+0000abc0: 0a20 2020 2020 2020 2020 2020 206c 7620  .            lv 
+0000abd0: 3d20 7b7d 2020 2320 7365 6c65 6374 6564  = {}  # selected
+0000abe0: 206c 6576 656c 0a20 2020 2020 2020 2020   level.         
+0000abf0: 2020 2061 6c67 203d 2022 2220 2023 2073     alg = ""  # s
+0000ac00: 656c 6563 7465 6420 616c 676f 2028 677a  elected algo (gz
+0000ac10: 3d70 7265 6665 7272 6564 290a 0a20 2020  =preferred)..   
+0000ac20: 2020 2020 2020 2020 2023 2075 7365 722d           # user-
+0000ac30: 7072 6566 7320 6669 7273 740a 2020 2020  prefs first.    
+0000ac40: 2020 2020 2020 2020 6966 2022 677a 2220          if "gz" 
+0000ac50: 696e 2073 656c 662e 7570 6172 616d 206f  in self.uparam o
+0000ac60: 7220 2270 6b22 2069 6e20 7365 6c66 2e75  r "pk" in self.u
+0000ac70: 7061 7261 6d3a 2020 2320 6465 662e 706b  param:  # def.pk
+0000ac80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ac90: 2061 6c67 203d 2022 677a 220a 2020 2020   alg = "gz".    
+0000aca0: 2020 2020 2020 2020 6966 2022 787a 2220          if "xz" 
+0000acb0: 696e 2073 656c 662e 7570 6172 616d 3a0a  in self.uparam:.
+0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acd0: 616c 6720 3d20 2278 7a22 0a20 2020 2020  alg = "xz".     
+0000ace0: 2020 2020 2020 2069 6620 616c 673a 0a20         if alg:. 
+0000acf0: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+0000ad00: 736f 203d 2073 656c 662e 7570 6172 616d  so = self.uparam
+0000ad10: 2e67 6574 2861 6c67 290a 2020 2020 2020  .get(alg).      
+0000ad20: 2020 2020 2020 2020 2020 6c76 5b61 6c67            lv[alg
+0000ad30: 5d20 3d20 6662 5b61 6c67 5d20 6966 207a  ] = fb[alg] if z
+0000ad40: 736f 2069 7320 4e6f 6e65 2065 6c73 6520  so is None else 
+0000ad50: 696e 7428 7a73 6f29 0a0a 2020 2020 2020  int(zso)..      
+0000ad60: 2020 2020 2020 6966 2061 6c67 206e 6f74        if alg not
+0000ad70: 2069 6e20 7666 732e 666c 6167 733a 0a20   in vfs.flags:. 
+0000ad80: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000ad90: 6c67 203d 2022 677a 2220 6966 2022 677a  lg = "gz" if "gz
+0000ada0: 2220 696e 2076 6673 2e66 6c61 6773 2065  " in vfs.flags e
+0000adb0: 6c73 6520 2278 7a22 0a0a 2020 2020 2020  lse "xz"..      
+0000adc0: 2020 2020 2020 2320 7468 656e 2073 6572        # then ser
+0000add0: 7665 7220 6f76 6572 7269 6465 730a 2020  ver overrides.  
+0000ade0: 2020 2020 2020 2020 2020 706b 203d 2076            pk = v
+0000adf0: 6673 2e66 6c61 6773 2e67 6574 2822 706b  fs.flags.get("pk
+0000ae00: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+0000ae10: 6620 706b 2069 7320 6e6f 7420 4e6f 6e65  f pk is not None
+0000ae20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ae30: 2020 2320 636f 6e66 6967 2d66 6f72 6365    # config-force
+0000ae40: 6420 6f6e 0a20 2020 2020 2020 2020 2020  d on.           
+0000ae50: 2020 2020 2061 6c67 203d 2061 6c67 206f       alg = alg o
+0000ae60: 7220 2267 7a22 2020 2320 6465 662e 706b  r "gz"  # def.pk
+0000ae70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ae80: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000ae90: 2020 2020 2020 2020 2020 2320 636f 6e66            # conf
+0000aea0: 6967 2d66 6f72 6365 6420 6f70 7473 0a20  ig-forced opts. 
+0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aec0: 2020 2061 6c67 2c20 6e6c 7620 3d20 706b     alg, nlv = pk
+0000aed0: 2e73 706c 6974 2822 2c22 290a 2020 2020  .split(",").    
 0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aef0: 2020 2020 6c76 5b61 6c67 5d20 3d20 696e      lv[alg] = in
-0000af00: 7428 6e6c 7629 0a20 2020 2020 2020 2020  t(nlv).         
-0000af10: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
-0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af30: 2020 2070 6173 730a 0a20 2020 2020 2020     pass..       
-0000af40: 2020 2020 206c 765b 616c 675d 203d 206c       lv[alg] = l
-0000af50: 762e 6765 7428 616c 6729 206f 7220 6662  v.get(alg) or fb
-0000af60: 2e67 6574 2861 6c67 2920 6f72 2030 0a0a  .get(alg) or 0..
-0000af70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000af80: 2e6c 6f67 2822 636f 6d70 7265 7373 696e  .log("compressin
-0000af90: 6720 7769 7468 207b 7d20 6c65 7665 6c20  g with {} level 
-0000afa0: 7b7d 222e 666f 726d 6174 2861 6c67 2c20  {}".format(alg, 
-0000afb0: 6c76 2e67 6574 2861 6c67 2929 290a 2020  lv.get(alg))).  
-0000afc0: 2020 2020 2020 2020 2020 6966 2061 6c67            if alg
-0000afd0: 203d 3d20 2267 7a22 3a0a 2020 2020 2020   == "gz":.      
-0000afe0: 2020 2020 2020 2020 2020 6f70 656e 5f6b            open_k
-0000aff0: 615b 2266 756e 225d 203d 2067 7a69 702e  a["fun"] = gzip.
-0000b000: 477a 6970 4669 6c65 0a20 2020 2020 2020  GzipFile.       
-0000b010: 2020 2020 2020 2020 206f 7065 6e5f 6120           open_a 
-0000b020: 3d20 5b22 7762 222c 206c 765b 616c 675d  = ["wb", lv[alg]
-0000b030: 2c20 4e6f 6e65 2c20 3078 3546 4545 3636  , None, 0x5FEE66
-0000b040: 3030 5d20 2023 2032 3032 312d 3031 2d30  00]  # 2021-01-0
-0000b050: 310a 2020 2020 2020 2020 2020 2020 656c  1.            el
-0000b060: 6966 2061 6c67 203d 3d20 2278 7a22 3a0a  if alg == "xz":.
-0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b080: 6f70 656e 5f6b 6120 3d20 7b22 6675 6e22  open_ka = {"fun"
-0000b090: 3a20 6c7a 6d61 2e6f 7065 6e2c 2022 7072  : lzma.open, "pr
-0000b0a0: 6573 6574 223a 206c 765b 616c 675d 7d0a  eset": lv[alg]}.
-0000b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0c0: 6f70 656e 5f61 203d 205b 2277 6222 5d0a  open_a = ["wb"].
-0000b0d0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000b0e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b0f0: 2020 7365 6c66 2e6c 6f67 2822 6661 6c6c    self.log("fall
-0000b100: 7468 726f 7567 683f 2074 6861 7473 2061  through? thats a
-0000b110: 2062 7567 222c 2031 290a 0a20 2020 2020   bug", 1)..     
-0000b120: 2020 2073 7566 6669 7820 3d20 222d 7b3a     suffix = "-{:
-0000b130: 2e36 667d 2d7b 7d22 2e66 6f72 6d61 7428  .6f}-{}".format(
-0000b140: 7469 6d65 2e74 696d 6528 292c 2073 656c  time.time(), sel
-0000b150: 662e 6469 7028 2929 0a20 2020 2020 2020  f.dip()).       
-0000b160: 206e 616d 656c 6573 7320 3d20 6e6f 7420   nameless = not 
-0000b170: 666e 0a20 2020 2020 2020 2069 6620 6e61  fn.        if na
-0000b180: 6d65 6c65 7373 3a0a 2020 2020 2020 2020  meless:.        
-0000b190: 2020 2020 7375 6666 6978 202b 3d20 222e      suffix += ".
-0000b1a0: 6269 6e22 0a20 2020 2020 2020 2020 2020  bin".           
-0000b1b0: 2066 6e20 3d20 2270 7574 2220 2b20 7375   fn = "put" + su
-0000b1c0: 6666 6978 0a0a 2020 2020 2020 2020 7061  ffix..        pa
-0000b1d0: 7261 6d73 203d 207b 2273 7566 6669 7822  rams = {"suffix"
-0000b1e0: 3a20 7375 6666 6978 2c20 2266 6469 7222  : suffix, "fdir"
-0000b1f0: 3a20 6664 6972 7d0a 2020 2020 2020 2020  : fdir}.        
-0000b200: 6966 2073 656c 662e 6172 6773 2e6e 773a  if self.args.nw:
-0000b210: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-0000b220: 616d 7320 3d20 7b7d 0a20 2020 2020 2020  ams = {}.       
-0000b230: 2020 2020 2066 6e20 3d20 6f73 2e64 6576       fn = os.dev
-0000b240: 6e75 6c6c 0a0a 2020 2020 2020 2020 7061  null..        pa
-0000b250: 7261 6d73 2e75 7064 6174 6528 6f70 656e  rams.update(open
-0000b260: 5f6b 6129 0a20 2020 2020 2020 2061 7373  _ka).        ass
-0000b270: 6572 7420 666e 0a0a 2020 2020 2020 2020  ert fn..        
-0000b280: 6966 206e 6f74 2073 656c 662e 6172 6773  if not self.args
-0000b290: 2e6e 773a 0a20 2020 2020 2020 2020 2020  .nw:.           
-0000b2a0: 2069 6620 726e 643a 0a20 2020 2020 2020   if rnd:.       
-0000b2b0: 2020 2020 2020 2020 2066 6e20 3d20 7261           fn = ra
-0000b2c0: 6e64 5f6e 616d 6528 6664 6972 2c20 666e  nd_name(fdir, fn
-0000b2d0: 2c20 726e 6429 0a0a 2020 2020 2020 2020  , rnd)..        
-0000b2e0: 2020 2020 666e 203d 2073 616e 6974 697a      fn = sanitiz
-0000b2f0: 655f 666e 2866 6e20 6f72 2022 222c 2022  e_fn(fn or "", "
-0000b300: 222c 205b 222e 7072 6f6c 6f67 7565 2e68  ", [".prologue.h
-0000b310: 746d 6c22 2c20 222e 6570 696c 6f67 7565  tml", ".epilogue
-0000b320: 2e68 746d 6c22 5d29 0a0a 2020 2020 2020  .html"])..      
-0000b330: 2020 7061 7468 203d 206f 732e 7061 7468    path = os.path
-0000b340: 2e6a 6f69 6e28 6664 6972 2c20 666e 290a  .join(fdir, fn).
-0000b350: 0a20 2020 2020 2020 2069 6620 7862 753a  .        if xbu:
-0000b360: 0a20 2020 2020 2020 2020 2020 2061 7420  .            at 
-0000b370: 3d20 7469 6d65 2e74 696d 6528 2920 2d20  = time.time() - 
-0000b380: 6c69 6665 7469 6d65 0a20 2020 2020 2020  lifetime.       
-0000b390: 2020 2020 2069 6620 6e6f 7420 7275 6e68       if not runh
-0000b3a0: 6f6f 6b28 0a20 2020 2020 2020 2020 2020  ook(.           
-0000b3b0: 2020 2020 2073 656c 662e 6c6f 672c 0a20       self.log,. 
-0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-0000b3d0: 6275 2c0a 2020 2020 2020 2020 2020 2020  bu,.            
-0000b3e0: 2020 2020 7061 7468 2c0a 2020 2020 2020      path,.      
-0000b3f0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-0000b400: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
-0000b410: 2020 2020 2020 7365 6c66 2e68 6f73 742c        self.host,
-0000b420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b430: 2073 656c 662e 756e 616d 652c 0a20 2020   self.uname,.   
-0000b440: 2020 2020 2020 2020 2020 2020 2061 742c               at,
-0000b450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b460: 2072 656d 6169 6e73 2c0a 2020 2020 2020   remains,.      
-0000b470: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-0000b480: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
-0000b490: 2020 2061 742c 0a20 2020 2020 2020 2020     at,.         
-0000b4a0: 2020 2020 2020 2022 222c 0a20 2020 2020         "",.     
-0000b4b0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-0000b4c0: 2020 2020 2020 2020 2020 7420 3d20 2275            t = "u
-0000b4d0: 706c 6f61 6420 626c 6f63 6b65 6420 6279  pload blocked by
-0000b4e0: 2078 6275 2073 6572 7665 7220 636f 6e66   xbu server conf
-0000b4f0: 6967 220a 2020 2020 2020 2020 2020 2020  ig".            
-0000b500: 2020 2020 7365 6c66 2e6c 6f67 2874 2c20      self.log(t, 
-0000b510: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-0000b520: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
-0000b530: 3430 332c 2074 290a 0a20 2020 2020 2020  403, t)..       
-0000b540: 2069 6620 6973 5f70 7574 2061 6e64 206e   if is_put and n
-0000b550: 6f74 2028 7365 6c66 2e61 7267 732e 6e6f  ot (self.args.no
-0000b560: 5f64 6176 206f 7220 7365 6c66 2e61 7267  _dav or self.arg
-0000b570: 732e 6e77 293a 0a20 2020 2020 2020 2020  s.nw):.         
-0000b580: 2020 2023 2061 6c6c 6f77 206f 7665 7277     # allow overw
-0000b590: 7269 7465 2069 662e 2e2e 0a20 2020 2020  rite if....     
-0000b5a0: 2020 2020 2020 2023 2020 2a20 766f 6c66         #  * volf
-0000b5b0: 6c61 6720 2764 6177 2720 6973 2073 6574  lag 'daw' is set
-0000b5c0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000b5d0: 2a20 616e 6420 6163 636f 756e 7420 6861  * and account ha
-0000b5e0: 7320 6465 6c65 7465 2d61 6363 6573 730a  s delete-access.
-0000b5f0: 2020 2020 2020 2020 2020 2020 2320 6f72              # or
-0000b600: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-0000b610: 2320 202a 2066 696c 6520 6578 6973 7473  #  * file exists
-0000b620: 2c20 6973 2065 6d70 7479 2c20 7375 6666  , is empty, suff
-0000b630: 6963 6965 6e74 6c79 206e 6577 0a20 2020  iciently new.   
-0000b640: 2020 2020 2020 2020 2023 2020 2a20 616e           #  * an
-0000b650: 6420 7468 6572 6520 6973 206e 6f20 2e50  d there is no .P
-0000b660: 4152 5449 414c 0a0a 2020 2020 2020 2020  ARTIAL..        
-0000b670: 2020 2020 746e 616d 203d 2066 6e20 2b20      tnam = fn + 
-0000b680: 222e 5041 5254 4941 4c22 0a20 2020 2020  ".PARTIAL".     
-0000b690: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-0000b6a0: 7267 732e 646f 7470 6172 743a 0a20 2020  rgs.dotpart:.   
-0000b6b0: 2020 2020 2020 2020 2020 2020 2074 6e61               tna
-0000b6c0: 6d20 3d20 222e 2220 2b20 746e 616d 0a0a  m = "." + tnam..
-0000b6d0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-0000b6e0: 7666 732e 666c 6167 732e 6765 7428 2264  vfs.flags.get("d
-0000b6f0: 6177 2229 2061 6e64 2073 656c 662e 6361  aw") and self.ca
-0000b700: 6e5f 6465 6c65 7465 2920 6f72 2028 0a20  n_delete) or (. 
-0000b710: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000b720: 6f74 2062 6f73 2e70 6174 682e 6578 6973  ot bos.path.exis
-0000b730: 7473 286f 732e 7061 7468 2e6a 6f69 6e28  ts(os.path.join(
-0000b740: 6664 6972 2c20 746e 616d 2929 0a20 2020  fdir, tnam)).   
-0000b750: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-0000b760: 2062 6f73 2e70 6174 682e 6578 6973 7473   bos.path.exists
-0000b770: 2870 6174 6829 0a20 2020 2020 2020 2020  (path).         
-0000b780: 2020 2020 2020 2061 6e64 206e 6f74 2062         and not b
-0000b790: 6f73 2e70 6174 682e 6765 7473 697a 6528  os.path.getsize(
-0000b7a0: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
-0000b7b0: 2020 2020 2020 616e 6420 626f 732e 7061        and bos.pa
-0000b7c0: 7468 2e67 6574 6d74 696d 6528 7061 7468  th.getmtime(path
-0000b7d0: 2920 3e3d 2074 696d 652e 7469 6d65 2829  ) >= time.time()
-0000b7e0: 202d 2073 656c 662e 6172 6773 2e62 6c61   - self.args.bla
-0000b7f0: 6e6b 5f77 740a 2020 2020 2020 2020 2020  nk_wt.          
-0000b800: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-0000b810: 2020 2020 2023 2073 6d61 6c6c 2074 6f63       # small toc
-0000b820: 746f 752c 2062 7574 2062 6574 7465 7220  tou, but better 
-0000b830: 7468 616e 2063 6c6f 6262 6572 696e 6720  than clobbering 
-0000b840: 6120 6861 7264 6c69 6e6b 0a20 2020 2020  a hardlink.     
-0000b850: 2020 2020 2020 2020 2020 2062 6f73 2e75             bos.u
-0000b860: 6e6c 696e 6b28 7061 7468 290a 0a20 2020  nlink(path)..   
-0000b870: 2020 2020 2077 6974 6820 7265 6e5f 6f70       with ren_op
-0000b880: 656e 2866 6e2c 202a 6f70 656e 5f61 2c20  en(fn, *open_a, 
-0000b890: 2a2a 7061 7261 6d73 2920 6173 207a 6677  **params) as zfw
-0000b8a0: 3a0a 2020 2020 2020 2020 2020 2020 662c  :.            f,
-0000b8b0: 2066 6e20 3d20 7a66 775b 226f 727a 225d   fn = zfw["orz"]
-0000b8c0: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
-0000b8d0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-0000b8e0: 2866 6469 722c 2066 6e29 0a20 2020 2020  (fdir, fn).     
-0000b8f0: 2020 2020 2020 2070 6f73 745f 737a 2c20         post_sz, 
-0000b900: 7368 615f 6865 782c 2073 6861 5f62 3634  sha_hex, sha_b64
-0000b910: 203d 2068 6173 6863 6f70 7928 7265 6164   = hashcopy(read
-0000b920: 6572 2c20 662c 2073 656c 662e 6172 6773  er, f, self.args
-0000b930: 2e73 5f77 725f 736c 7029 0a0a 2020 2020  .s_wr_slp)..    
-0000b940: 2020 2020 6966 206c 696d 3a0a 2020 2020      if lim:.    
-0000b950: 2020 2020 2020 2020 6c69 6d2e 6e75 7028          lim.nup(
-0000b960: 7365 6c66 2e69 7029 0a20 2020 2020 2020  self.ip).       
-0000b970: 2020 2020 206c 696d 2e62 7570 2873 656c       lim.bup(sel
-0000b980: 662e 6970 2c20 706f 7374 5f73 7a29 0a20  f.ip, post_sz). 
-0000b990: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9b0: 6c69 6d2e 6368 6b5f 737a 2870 6f73 745f  lim.chk_sz(post_
-0000b9c0: 737a 290a 2020 2020 2020 2020 2020 2020  sz).            
-0000b9d0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-0000b9e0: 2020 2020 2020 2020 626f 732e 756e 6c69          bos.unli
-0000b9f0: 6e6b 2870 6174 6829 0a20 2020 2020 2020  nk(path).       
-0000ba00: 2020 2020 2020 2020 2072 6169 7365 0a0a           raise..
-0000ba10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000ba20: 6172 6773 2e6e 773a 0a20 2020 2020 2020  args.nw:.       
-0000ba30: 2020 2020 2072 6574 7572 6e20 706f 7374       return post
-0000ba40: 5f73 7a2c 2073 6861 5f68 6578 2c20 7368  _sz, sha_hex, sh
-0000ba50: 615f 6236 342c 2072 656d 6169 6e73 2c20  a_b64, remains, 
-0000ba60: 7061 7468 2c20 2222 0a0a 2020 2020 2020  path, ""..      
-0000ba70: 2020 6966 206e 616d 656c 6573 7320 616e    if nameless an
-0000ba80: 6420 226d 6167 6963 2220 696e 2076 6673  d "magic" in vfs
-0000ba90: 2e66 6c61 6773 3a0a 2020 2020 2020 2020  .flags:.        
-0000baa0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000bab0: 2020 2020 2020 2020 2065 7874 203d 2073           ext = s
-0000bac0: 656c 662e 636f 6e6e 2e68 7372 762e 6d61  elf.conn.hsrv.ma
-0000bad0: 6769 6369 616e 2e65 7874 2870 6174 6829  gician.ext(path)
-0000bae0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-0000baf0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-0000bb00: 2065 783a 0a20 2020 2020 2020 2020 2020   ex:.           
-0000bb10: 2020 2020 2073 656c 662e 6c6f 6728 2266       self.log("f
-0000bb20: 696c 6574 7970 6520 6465 7465 6374 696f  iletype detectio
-0000bb30: 6e20 6661 696c 6564 2066 6f72 205b 7b7d  n failed for [{}
-0000bb40: 5d3a 207b 7d22 2e66 6f72 6d61 7428 7061  ]: {}".format(pa
-0000bb50: 7468 2c20 6578 292c 2036 290a 2020 2020  th, ex), 6).    
-0000bb60: 2020 2020 2020 2020 2020 2020 6578 7420              ext 
-0000bb70: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
-0000bb80: 2020 2020 6966 2065 7874 3a0a 2020 2020      if ext:.    
-0000bb90: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-0000bba0: 6e64 3a0a 2020 2020 2020 2020 2020 2020  nd:.            
-0000bbb0: 2020 2020 2020 2020 666e 3220 3d20 7261          fn2 = ra
-0000bbc0: 6e64 5f6e 616d 6528 6664 6972 2c20 2261  nd_name(fdir, "a
-0000bbd0: 2e22 202b 2065 7874 2c20 726e 6429 0a20  ." + ext, rnd). 
-0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000bbf0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000bc00: 2020 2020 2020 2020 2066 6e32 203d 2066           fn2 = f
-0000bc10: 6e2e 7273 706c 6974 2822 2e22 2c20 3129  n.rsplit(".", 1)
-0000bc20: 5b30 5d20 2b20 222e 2220 2b20 6578 740a  [0] + "." + ext.
-0000bc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bc40: 2070 6172 616d 735b 2273 7566 6669 7822   params["suffix"
-0000bc50: 5d20 3d20 7375 6666 6978 5b3a 2d34 5d0a  ] = suffix[:-4].
-0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc70: 7769 7468 2072 656e 5f6f 7065 6e28 666e  with ren_open(fn
-0000bc80: 2c20 2a6f 7065 6e5f 612c 202a 2a70 6172  , *open_a, **par
-0000bc90: 616d 7329 2061 7320 7a66 773a 0a20 2020  ams) as zfw:.   
-0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcb0: 2066 2c20 666e 203d 207a 6677 5b22 6f72   f, fn = zfw["or
-0000bcc0: 7a22 5d0a 0a20 2020 2020 2020 2020 2020  z"]..           
-0000bcd0: 2020 2020 2070 6174 6832 203d 206f 732e       path2 = os.
-0000bce0: 7061 7468 2e6a 6f69 6e28 6664 6972 2c20  path.join(fdir, 
-0000bcf0: 666e 3229 0a20 2020 2020 2020 2020 2020  fn2).           
-0000bd00: 2020 2020 2061 746f 6d69 635f 6d6f 7665       atomic_move
-0000bd10: 2870 6174 682c 2070 6174 6832 290a 2020  (path, path2).  
-0000bd20: 2020 2020 2020 2020 2020 2020 2020 666e                fn
-0000bd30: 203d 2066 6e32 0a20 2020 2020 2020 2020   = fn2.         
-0000bd40: 2020 2020 2020 2070 6174 6820 3d20 7061         path = pa
-0000bd50: 7468 320a 0a20 2020 2020 2020 2061 7420  th2..        at 
-0000bd60: 3d20 7469 6d65 2e74 696d 6528 2920 2d20  = time.time() - 
-0000bd70: 6c69 6665 7469 6d65 0a20 2020 2020 2020  lifetime.       
-0000bd80: 2069 6620 7861 7520 616e 6420 6e6f 7420   if xau and not 
-0000bd90: 7275 6e68 6f6f 6b28 0a20 2020 2020 2020  runhook(.       
-0000bda0: 2020 2020 2073 656c 662e 6c6f 672c 0a20       self.log,. 
-0000bdb0: 2020 2020 2020 2020 2020 2078 6175 2c0a             xau,.
-0000bdc0: 2020 2020 2020 2020 2020 2020 7061 7468              path
-0000bdd0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-0000bde0: 6c66 2e76 7061 7468 2c0a 2020 2020 2020  lf.vpath,.      
-0000bdf0: 2020 2020 2020 7365 6c66 2e68 6f73 742c        self.host,
-0000be00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000be10: 662e 756e 616d 652c 0a20 2020 2020 2020  f.uname,.       
-0000be20: 2020 2020 2061 742c 0a20 2020 2020 2020       at,.       
-0000be30: 2020 2020 2070 6f73 745f 737a 2c0a 2020       post_sz,.  
-0000be40: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-0000be50: 702c 0a20 2020 2020 2020 2020 2020 2061  p,.            a
-0000be60: 742c 0a20 2020 2020 2020 2020 2020 2022  t,.            "
-0000be70: 222c 0a20 2020 2020 2020 2029 3a0a 2020  ",.        ):.  
-0000be80: 2020 2020 2020 2020 2020 7420 3d20 2275            t = "u
-0000be90: 706c 6f61 6420 626c 6f63 6b65 6420 6279  pload blocked by
-0000bea0: 2078 6175 2073 6572 7665 7220 636f 6e66   xau server conf
-0000beb0: 6967 220a 2020 2020 2020 2020 2020 2020  ig".            
-0000bec0: 7365 6c66 2e6c 6f67 2874 2c20 3129 0a20  self.log(t, 1). 
-0000bed0: 2020 2020 2020 2020 2020 206f 732e 756e             os.un
-0000bee0: 6c69 6e6b 2870 6174 6829 0a20 2020 2020  link(path).     
-0000bef0: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
-0000bf00: 6b61 6328 3430 332c 2074 290a 0a20 2020  kac(403, t)..   
-0000bf10: 2020 2020 2076 6673 2c20 7265 6d20 3d20       vfs, rem = 
-0000bf20: 7666 732e 6765 745f 6462 7628 7265 6d29  vfs.get_dbv(rem)
-0000bf30: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0000bf40: 6e6e 2e68 7372 762e 6272 6f6b 6572 2e73  nn.hsrv.broker.s
-0000bf50: 6179 280a 2020 2020 2020 2020 2020 2020  ay(.            
-0000bf60: 2275 7032 6b2e 6861 7368 5f66 696c 6522  "up2k.hash_file"
-0000bf70: 2c0a 2020 2020 2020 2020 2020 2020 7666  ,.            vf
-0000bf80: 732e 7265 616c 7061 7468 2c0a 2020 2020  s.realpath,.    
-0000bf90: 2020 2020 2020 2020 7666 732e 7670 6174          vfs.vpat
-0000bfa0: 682c 0a20 2020 2020 2020 2020 2020 2076  h,.            v
-0000bfb0: 6673 2e66 6c61 6773 2c0a 2020 2020 2020  fs.flags,.      
-0000bfc0: 2020 2020 2020 7265 6d2c 0a20 2020 2020        rem,.     
-0000bfd0: 2020 2020 2020 2066 6e2c 0a20 2020 2020         fn,.     
-0000bfe0: 2020 2020 2020 2073 656c 662e 6970 2c0a         self.ip,.
-0000bff0: 2020 2020 2020 2020 2020 2020 6174 2c0a              at,.
-0000c000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c010: 2e75 6e61 6d65 2c0a 2020 2020 2020 2020  .uname,.        
-0000c020: 2020 2020 5472 7565 2c0a 2020 2020 2020      True,.      
-0000c030: 2020 290a 0a20 2020 2020 2020 2076 7375    )..        vsu
-0000c040: 6620 3d20 2222 0a20 2020 2020 2020 2069  f = "".        i
-0000c050: 6620 2873 656c 662e 6361 6e5f 7265 6164  f (self.can_read
-0000c060: 206f 7220 7365 6c66 2e63 616e 5f75 7067   or self.can_upg
-0000c070: 6574 2920 616e 6420 2266 6b22 2069 6e20  et) and "fk" in 
-0000c080: 7666 732e 666c 6167 733a 0a20 2020 2020  vfs.flags:.     
-0000c090: 2020 2020 2020 2076 7375 6620 3d20 223f         vsuf = "?
-0000c0a0: 6b3d 2220 2b20 7365 6c66 2e67 656e 5f66  k=" + self.gen_f
-0000c0b0: 6b28 0a20 2020 2020 2020 2020 2020 2020  k(.             
-0000c0c0: 2020 2073 656c 662e 6172 6773 2e66 6b5f     self.args.fk_
-0000c0d0: 7361 6c74 2c0a 2020 2020 2020 2020 2020  salt,.          
-0000c0e0: 2020 2020 2020 7061 7468 2c0a 2020 2020        path,.    
-0000c0f0: 2020 2020 2020 2020 2020 2020 706f 7374              post
-0000c100: 5f73 7a2c 0a20 2020 2020 2020 2020 2020  _sz,.           
-0000c110: 2020 2020 2030 2069 6620 414e 5957 494e       0 if ANYWIN
-0000c120: 2065 6c73 6520 626f 732e 7374 6174 2870   else bos.stat(p
-0000c130: 6174 6829 2e73 745f 696e 6f2c 0a20 2020  ath).st_ino,.   
-0000c140: 2020 2020 2020 2020 2029 5b3a 2076 6673           )[: vfs
-0000c150: 2e66 6c61 6773 5b22 666b 225d 5d0a 0a20  .flags["fk"]].. 
-0000c160: 2020 2020 2020 2076 7061 7468 203d 2022         vpath = "
-0000c170: 2f22 2e6a 6f69 6e28 5b78 2066 6f72 2078  /".join([x for x
-0000c180: 2069 6e20 5b76 6673 2e76 7061 7468 2c20   in [vfs.vpath, 
-0000c190: 7265 6d2c 2066 6e5d 2069 6620 785d 290a  rem, fn] if x]).
-0000c1a0: 2020 2020 2020 2020 7670 6174 6820 3d20          vpath = 
-0000c1b0: 7175 6f74 6570 2876 7061 7468 290a 0a20  quotep(vpath).. 
-0000c1c0: 2020 2020 2020 2075 726c 203d 2022 7b7d         url = "{}
-0000c1d0: 3a2f 2f7b 7d2f 7b7d 222e 666f 726d 6174  ://{}/{}".format
-0000c1e0: 280a 2020 2020 2020 2020 2020 2020 2268  (.            "h
-0000c1f0: 7474 7073 2220 6966 2073 656c 662e 6973  ttps" if self.is
-0000c200: 5f68 7474 7073 2065 6c73 6520 2268 7474  _https else "htt
-0000c210: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-0000c220: 7365 6c66 2e68 6f73 742c 0a20 2020 2020  self.host,.     
-0000c230: 2020 2020 2020 2073 656c 662e 6172 6773         self.args
-0000c240: 2e52 5320 2b20 7670 6174 6820 2b20 7673  .RS + vpath + vs
-0000c250: 7566 2c0a 2020 2020 2020 2020 290a 0a20  uf,.        ).. 
-0000c260: 2020 2020 2020 2072 6574 7572 6e20 706f         return po
-0000c270: 7374 5f73 7a2c 2073 6861 5f68 6578 2c20  st_sz, sha_hex, 
-0000c280: 7368 615f 6236 342c 2072 656d 6169 6e73  sha_b64, remains
-0000c290: 2c20 7061 7468 2c20 7572 6c0a 0a20 2020  , path, url..   
-0000c2a0: 2064 6566 2068 616e 646c 655f 7374 6173   def handle_stas
-0000c2b0: 6828 7365 6c66 2c20 6973 5f70 7574 2029  h(self, is_put )
-0000c2c0: 2020 3a0a 2020 2020 2020 2020 706f 7374    :.        post
-0000c2d0: 5f73 7a2c 2073 6861 5f68 6578 2c20 7368  _sz, sha_hex, sh
-0000c2e0: 615f 6236 342c 2072 656d 6169 6e73 2c20  a_b64, remains, 
-0000c2f0: 7061 7468 2c20 7572 6c20 3d20 7365 6c66  path, url = self
-0000c300: 2e64 756d 705f 746f 5f66 696c 6528 6973  .dump_to_file(is
-0000c310: 5f70 7574 290a 2020 2020 2020 2020 7370  _put).        sp
-0000c320: 6420 3d20 7365 6c66 2e5f 7370 6428 706f  d = self._spd(po
-0000c330: 7374 5f73 7a29 0a20 2020 2020 2020 2074  st_sz).        t
-0000c340: 203d 2022 7b7d 2077 726f 7465 207b 7d2f   = "{} wrote {}/
-0000c350: 7b7d 2062 7974 6573 2074 6f20 7b7d 2020  {} bytes to {}  
-0000c360: 2320 7b7d 220a 2020 2020 2020 2020 7365  # {}".        se
-0000c370: 6c66 2e6c 6f67 2874 2e66 6f72 6d61 7428  lf.log(t.format(
-0000c380: 7370 642c 2070 6f73 745f 737a 2c20 7265  spd, post_sz, re
-0000c390: 6d61 696e 732c 2070 6174 682c 2073 6861  mains, path, sha
-0000c3a0: 5f62 3634 5b3a 3238 5d29 2920 2023 2032  _b64[:28]))  # 2
-0000c3b0: 310a 0a20 2020 2020 2020 2061 6320 3d20  1..        ac = 
-0000c3c0: 7365 6c66 2e75 7061 7261 6d2e 6765 7428  self.uparam.get(
-0000c3d0: 0a20 2020 2020 2020 2020 2020 2022 7761  .            "wa
-0000c3e0: 6e74 222c 2073 656c 662e 6865 6164 6572  nt", self.header
-0000c3f0: 732e 6765 7428 2261 6363 6570 7422 2c20  s.get("accept", 
-0000c400: 2222 292e 6c6f 7765 7228 292e 7370 6c69  "").lower().spli
-0000c410: 7428 223b 2229 5b2d 315d 0a20 2020 2020  t(";")[-1].     
-0000c420: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-0000c430: 6163 203d 3d20 2275 726c 223a 0a20 2020  ac == "url":.   
-0000c440: 2020 2020 2020 2020 2074 203d 2075 726c           t = url
-0000c450: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000c460: 2020 2020 2020 2020 2020 2074 203d 2022             t = "
-0000c470: 7b7d 5c6e 7b7d 5c6e 7b7d 5c6e 7b7d 5c6e  {}\n{}\n{}\n{}\n
-0000c480: 222e 666f 726d 6174 2870 6f73 745f 737a  ".format(post_sz
-0000c490: 2c20 7368 615f 6236 342c 2073 6861 5f68  , sha_b64, sha_h
-0000c4a0: 6578 5b3a 3536 5d2c 2075 726c 290a 0a20  ex[:56], url).. 
-0000c4b0: 2020 2020 2020 2068 203d 207b 224c 6f63         h = {"Loc
-0000c4c0: 6174 696f 6e22 3a20 7572 6c7d 2069 6620  ation": url} if 
-0000c4d0: 6973 5f70 7574 2061 6e64 2075 726c 2065  is_put and url e
-0000c4e0: 6c73 6520 7b7d 0a20 2020 2020 2020 2073  lse {}.        s
-0000c4f0: 656c 662e 7265 706c 7928 742e 656e 636f  elf.reply(t.enco
-0000c500: 6465 2822 7574 662d 3822 292c 2032 3031  de("utf-8"), 201
-0000c510: 2c20 6865 6164 6572 733d 6829 0a20 2020  , headers=h).   
-0000c520: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-0000c530: 0a0a 2020 2020 6465 6620 6261 6b66 6c69  ..    def bakfli
-0000c540: 7028 7365 6c66 2c20 6620 2c20 6f66 7320  p(self, f , ofs 
-0000c550: 2c20 737a 202c 2073 6861 2029 2020 3a0a  , sz , sha )  :.
-0000c560: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-0000c570: 656c 662e 6172 6773 2e62 616b 5f66 6c69  elf.args.bak_fli
-0000c580: 7073 206f 7220 7365 6c66 2e61 7267 732e  ps or self.args.
-0000c590: 6e77 3a0a 2020 2020 2020 2020 2020 2020  nw:.            
-0000c5a0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-0000c5b0: 7364 6972 203d 2073 656c 662e 6172 6773  sdir = self.args
-0000c5c0: 2e62 665f 6469 720a 2020 2020 2020 2020  .bf_dir.        
-0000c5d0: 6670 203d 206f 732e 7061 7468 2e6a 6f69  fp = os.path.joi
-0000c5e0: 6e28 7364 6972 2c20 7368 6129 0a20 2020  n(sdir, sha).   
-0000c5f0: 2020 2020 2069 6620 626f 732e 7061 7468       if bos.path
-0000c600: 2e65 7869 7374 7328 6670 293a 0a20 2020  .exists(fp):.   
-0000c610: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000c620: 7365 6c66 2e6c 6f67 2822 6e6f 2062 616b  self.log("no bak
-0000c630: 666c 6970 3b20 6861 7665 2069 7422 2c20  flip; have it", 
-0000c640: 3629 0a0a 2020 2020 2020 2020 6966 206e  6)..        if n
-0000c650: 6f74 2062 6f73 2e70 6174 682e 6973 6469  ot bos.path.isdi
-0000c660: 7228 7364 6972 293a 0a20 2020 2020 2020  r(sdir):.       
-0000c670: 2020 2020 2062 6f73 2e6d 616b 6564 6972       bos.makedir
-0000c680: 7328 7364 6972 290a 0a20 2020 2020 2020  s(sdir)..       
-0000c690: 2069 6620 6c65 6e28 626f 732e 6c69 7374   if len(bos.list
-0000c6a0: 6469 7228 7364 6972 2929 203e 3d20 7365  dir(sdir)) >= se
-0000c6b0: 6c66 2e61 7267 732e 6266 5f6e 633a 0a20  lf.args.bf_nc:. 
-0000c6c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000c6d0: 6e20 7365 6c66 2e6c 6f67 2822 6e6f 2062  n self.log("no b
-0000c6e0: 616b 666c 6970 3b20 746f 6f20 6d61 6e79  akflip; too many
-0000c6f0: 222c 2033 290a 0a20 2020 2020 2020 206e  ", 3)..        n
-0000c700: 7265 6d20 3d20 737a 0a20 2020 2020 2020  rem = sz.       
-0000c710: 2066 2e73 6565 6b28 6f66 7329 0a20 2020   f.seek(ofs).   
-0000c720: 2020 2020 2077 6974 6820 6f70 656e 2866       with open(f
-0000c730: 702c 2022 7762 2229 2061 7320 666f 3a0a  p, "wb") as fo:.
-0000c740: 2020 2020 2020 2020 2020 2020 7768 696c              whil
-0000c750: 6520 6e72 656d 3a0a 2020 2020 2020 2020  e nrem:.        
-0000c760: 2020 2020 2020 2020 6275 6620 3d20 662e          buf = f.
-0000c770: 7265 6164 286d 696e 286e 7265 6d2c 2035  read(min(nrem, 5
-0000c780: 3132 202a 2031 3032 3429 290a 2020 2020  12 * 1024)).    
-0000c790: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000c7a0: 6f74 2062 7566 3a0a 2020 2020 2020 2020  ot buf:.        
-0000c7b0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-0000c7c0: 6b0a 0a20 2020 2020 2020 2020 2020 2020  k..             
-0000c7d0: 2020 206e 7265 6d20 2d3d 206c 656e 2862     nrem -= len(b
-0000c7e0: 7566 290a 2020 2020 2020 2020 2020 2020  uf).            
-0000c7f0: 2020 2020 666f 2e77 7269 7465 2862 7566      fo.write(buf
-0000c800: 290a 0a20 2020 2020 2020 2069 6620 6e72  )..        if nr
-0000c810: 656d 3a0a 2020 2020 2020 2020 2020 2020  em:.            
-0000c820: 7365 6c66 2e6c 6f67 2822 6261 6b66 6c69  self.log("bakfli
-0000c830: 7020 7472 756e 6361 7465 643b 207b 7d20  p truncated; {} 
-0000c840: 7265 6d61 696e 7322 2e66 6f72 6d61 7428  remains".format(
-0000c850: 6e72 656d 292c 2031 290a 2020 2020 2020  nrem), 1).      
-0000c860: 2020 2020 2020 6174 6f6d 6963 5f6d 6f76        atomic_mov
-0000c870: 6528 6670 2c20 6670 202b 2022 2e74 7275  e(fp, fp + ".tru
-0000c880: 6e63 2229 0a20 2020 2020 2020 2065 6c73  nc").        els
-0000c890: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000c8a0: 656c 662e 6c6f 6728 2262 616b 666c 6970  elf.log("bakflip
-0000c8b0: 206f 6b22 2c20 3229 0a0a 2020 2020 6465   ok", 2)..    de
-0000c8c0: 6620 5f73 7064 2873 656c 662c 206e 6279  f _spd(self, nby
-0000c8d0: 7465 7320 2c20 6164 6420 203d 2054 7275  tes , add  = Tru
-0000c8e0: 6529 2020 3a0a 2020 2020 2020 2020 6966  e)  :.        if
-0000c8f0: 2061 6464 3a0a 2020 2020 2020 2020 2020   add:.          
-0000c900: 2020 7365 6c66 2e63 6f6e 6e2e 6e62 7974    self.conn.nbyt
-0000c910: 6520 2b3d 206e 6279 7465 730a 0a20 2020  e += nbytes..   
-0000c920: 2020 2020 2073 7064 3120 3d20 6765 745f       spd1 = get_
-0000c930: 7370 6428 6e62 7974 6573 2c20 7365 6c66  spd(nbytes, self
-0000c940: 2e74 3029 0a20 2020 2020 2020 2073 7064  .t0).        spd
-0000c950: 3220 3d20 6765 745f 7370 6428 7365 6c66  2 = get_spd(self
-0000c960: 2e63 6f6e 6e2e 6e62 7974 652c 2073 656c  .conn.nbyte, sel
-0000c970: 662e 636f 6e6e 2e74 3029 0a20 2020 2020  f.conn.t0).     
-0000c980: 2020 2072 6574 7572 6e20 227b 7d20 7b7d     return "{} {}
-0000c990: 206e 7b7d 222e 666f 726d 6174 2873 7064   n{}".format(spd
-0000c9a0: 312c 2073 7064 322c 2073 656c 662e 636f  1, spd2, self.co
-0000c9b0: 6e6e 2e6e 7265 7129 0a0a 2020 2020 6465  nn.nreq)..    de
-0000c9c0: 6620 6861 6e64 6c65 5f70 6f73 745f 6d75  f handle_post_mu
-0000c9d0: 6c74 6970 6172 7428 7365 6c66 2920 203a  ltipart(self)  :
-0000c9e0: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
-0000c9f0: 7273 6572 203d 204d 756c 7469 7061 7274  rser = Multipart
-0000ca00: 5061 7273 6572 2873 656c 662e 6c6f 672c  Parser(self.log,
-0000ca10: 2073 656c 662e 7372 2c20 7365 6c66 2e68   self.sr, self.h
-0000ca20: 6561 6465 7273 290a 2020 2020 2020 2020  eaders).        
-0000ca30: 7365 6c66 2e70 6172 7365 722e 7061 7273  self.parser.pars
-0000ca40: 6528 290a 0a20 2020 2020 2020 2061 6374  e()..        act
-0000ca50: 203d 2073 656c 662e 7061 7273 6572 2e72   = self.parser.r
-0000ca60: 6571 7569 7265 2822 6163 7422 2c20 3634  equire("act", 64
-0000ca70: 290a 0a20 2020 2020 2020 2069 6620 6163  )..        if ac
-0000ca80: 7420 3d3d 2022 6c6f 6769 6e22 3a0a 2020  t == "login":.  
-0000ca90: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000caa0: 2073 656c 662e 6861 6e64 6c65 5f6c 6f67   self.handle_log
-0000cab0: 696e 2829 0a0a 2020 2020 2020 2020 6966  in()..        if
-0000cac0: 2061 6374 203d 3d20 226d 6b64 6972 223a   act == "mkdir":
-0000cad0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000cae0: 7572 6e20 7365 6c66 2e68 616e 646c 655f  urn self.handle_
-0000caf0: 6d6b 6469 7228 290a 0a20 2020 2020 2020  mkdir()..       
-0000cb00: 2069 6620 6163 7420 3d3d 2022 6e65 775f   if act == "new_
-0000cb10: 6d64 223a 0a20 2020 2020 2020 2020 2020  md":.           
-0000cb20: 2023 206b 696e 6461 2073 696c 6c79 2062   # kinda silly b
-0000cb30: 7574 2068 6173 2074 6865 206c 6561 7374  ut has the least
-0000cb40: 2073 6964 6520 6566 6665 6374 730a 2020   side effects.  
-0000cb50: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000cb60: 2073 656c 662e 6861 6e64 6c65 5f6e 6577   self.handle_new
-0000cb70: 5f6d 6428 290a 0a20 2020 2020 2020 2069  _md()..        i
-0000cb80: 6620 6163 7420 3d3d 2022 6270 7574 223a  f act == "bput":
-0000cb90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000cba0: 7572 6e20 7365 6c66 2e68 616e 646c 655f  urn self.handle_
-0000cbb0: 706c 6169 6e5f 7570 6c6f 6164 2829 0a0a  plain_upload()..
-0000cbc0: 2020 2020 2020 2020 6966 2061 6374 203d          if act =
-0000cbd0: 3d20 2274 7075 7422 3a0a 2020 2020 2020  = "tput":.      
-0000cbe0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000cbf0: 662e 6861 6e64 6c65 5f74 6578 745f 7570  f.handle_text_up
-0000cc00: 6c6f 6164 2829 0a0a 2020 2020 2020 2020  load()..        
-0000cc10: 6966 2061 6374 203d 3d20 227a 6970 223a  if act == "zip":
-0000cc20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000cc30: 7572 6e20 7365 6c66 2e68 616e 646c 655f  urn self.handle_
-0000cc40: 7a69 705f 706f 7374 2829 0a0a 2020 2020  zip_post()..    
-0000cc50: 2020 2020 7261 6973 6520 5065 626b 6163      raise Pebkac
-0000cc60: 2834 3232 2c20 2769 6e76 616c 6964 2061  (422, 'invalid a
-0000cc70: 6374 696f 6e20 227b 7d22 272e 666f 726d  ction "{}"'.form
-0000cc80: 6174 2861 6374 2929 0a0a 2020 2020 6465  at(act))..    de
-0000cc90: 6620 6861 6e64 6c65 5f7a 6970 5f70 6f73  f handle_zip_pos
-0000cca0: 7428 7365 6c66 2920 203a 0a20 2020 2020  t(self)  :.     
-0000ccb0: 2020 2061 7373 6572 7420 7365 6c66 2e70     assert self.p
-0000ccc0: 6172 7365 720a 2020 2020 2020 2020 7472  arser.        tr
-0000ccd0: 793a 0a20 2020 2020 2020 2020 2020 206b  y:.            k
-0000cce0: 203d 206e 6578 7428 7820 666f 7220 7820   = next(x for x 
-0000ccf0: 696e 2073 656c 662e 7570 6172 616d 2069  in self.uparam i
-0000cd00: 6620 7820 696e 2028 227a 6970 222c 2022  f x in ("zip", "
-0000cd10: 7461 7222 2929 0a20 2020 2020 2020 2065  tar")).        e
-0000cd20: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
-0000cd30: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
-0000cd40: 3432 322c 2022 6e65 6564 207a 6970 206f  422, "need zip o
-0000cd50: 7220 7461 7220 6b65 7977 6f72 6422 290a  r tar keyword").
-0000cd60: 0a20 2020 2020 2020 2076 203d 2073 656c  .        v = sel
-0000cd70: 662e 7570 6172 616d 5b6b 5d0a 0a20 2020  f.uparam[k]..   
-0000cd80: 2020 2020 2076 6e2c 2072 656d 203d 2073       vn, rem = s
-0000cd90: 656c 662e 6173 7276 2e76 6673 2e67 6574  elf.asrv.vfs.get
-0000cda0: 2873 656c 662e 7670 6174 682c 2073 656c  (self.vpath, sel
-0000cdb0: 662e 756e 616d 652c 2054 7275 652c 2046  f.uname, True, F
-0000cdc0: 616c 7365 290a 2020 2020 2020 2020 7a73  alse).        zs
-0000cdd0: 203d 2073 656c 662e 7061 7273 6572 2e72   = self.parser.r
-0000cde0: 6571 7569 7265 2822 6669 6c65 7322 2c20  equire("files", 
-0000cdf0: 3130 3234 202a 2031 3032 3429 0a20 2020  1024 * 1024).   
-0000ce00: 2020 2020 2069 6620 6e6f 7420 7a73 3a0a       if not zs:.
-0000ce10: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000ce20: 6520 5065 626b 6163 2834 3232 2c20 226e  e Pebkac(422, "n
-0000ce30: 6565 6420 6669 6c65 7320 6c69 7374 2229  eed files list")
-0000ce40: 0a0a 2020 2020 2020 2020 6974 656d 7320  ..        items 
-0000ce50: 3d20 7a73 2e72 6570 6c61 6365 2822 5c72  = zs.replace("\r
-0000ce60: 222c 2022 2229 2e73 706c 6974 2822 5c6e  ", "").split("\n
-0000ce70: 2229 0a20 2020 2020 2020 2069 7465 6d73  ").        items
-0000ce80: 203d 205b 756e 7175 6f74 6570 2878 2920   = [unquotep(x) 
-0000ce90: 666f 7220 7820 696e 2069 7465 6d73 2069  for x in items i
-0000cea0: 6620 6974 656d 735d 0a0a 2020 2020 2020  f items]..      
-0000ceb0: 2020 7365 6c66 2e70 6172 7365 722e 6472    self.parser.dr
-0000cec0: 6f70 2829 0a20 2020 2020 2020 2072 6574  op().        ret
-0000ced0: 7572 6e20 7365 6c66 2e74 785f 7a69 7028  urn self.tx_zip(
-0000cee0: 6b2c 2076 2c20 766e 2c20 7265 6d2c 2069  k, v, vn, rem, i
-0000cef0: 7465 6d73 2c20 7365 6c66 2e61 7267 732e  tems, self.args.
-0000cf00: 6564 290a 0a20 2020 2064 6566 2068 616e  ed)..    def han
-0000cf10: 646c 655f 706f 7374 5f6a 736f 6e28 7365  dle_post_json(se
-0000cf20: 6c66 2920 203a 0a20 2020 2020 2020 2074  lf)  :.        t
-0000cf30: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000cf40: 7265 6d61 696e 7320 3d20 696e 7428 7365  remains = int(se
-0000cf50: 6c66 2e68 6561 6465 7273 5b22 636f 6e74  lf.headers["cont
-0000cf60: 656e 742d 6c65 6e67 7468 225d 290a 2020  ent-length"]).  
-0000cf70: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-0000cf80: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000cf90: 5065 626b 6163 2834 3131 290a 0a20 2020  Pebkac(411)..   
-0000cfa0: 2020 2020 2069 6620 7265 6d61 696e 7320       if remains 
-0000cfb0: 3e20 3130 3234 202a 2031 3032 343a 0a20  > 1024 * 1024:. 
-0000cfc0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000cfd0: 2050 6562 6b61 6328 3431 332c 2022 6a73   Pebkac(413, "js
-0000cfe0: 6f6e 2032 6269 6722 290a 0a20 2020 2020  on 2big")..     
-0000cff0: 2020 2065 6e63 203d 2022 7574 662d 3822     enc = "utf-8"
-0000d000: 0a20 2020 2020 2020 2063 7479 7065 203d  .        ctype =
-0000d010: 2073 656c 662e 6865 6164 6572 732e 6765   self.headers.ge
-0000d020: 7428 2263 6f6e 7465 6e74 2d74 7970 6522  t("content-type"
-0000d030: 2c20 2222 292e 6c6f 7765 7228 290a 2020  , "").lower().  
-0000d040: 2020 2020 2020 6966 2022 6368 6172 7365        if "charse
-0000d050: 7422 2069 6e20 6374 7970 653a 0a20 2020  t" in ctype:.   
-0000d060: 2020 2020 2020 2020 2065 6e63 203d 2063           enc = c
-0000d070: 7479 7065 2e73 706c 6974 2822 6368 6172  type.split("char
-0000d080: 7365 7422 295b 315d 2e73 7472 6970 2822  set")[1].strip("
-0000d090: 203d 2229 2e73 706c 6974 2822 3b22 295b   =").split(";")[
-0000d0a0: 305d 2e73 7472 6970 2829 0a0a 2020 2020  0].strip()..    
-0000d0b0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000d0c0: 2020 2020 206a 736f 6e5f 6275 6620 3d20       json_buf = 
-0000d0d0: 7365 6c66 2e73 722e 7265 6376 5f65 7828  self.sr.recv_ex(
-0000d0e0: 7265 6d61 696e 7329 0a20 2020 2020 2020  remains).       
-0000d0f0: 2065 7863 6570 7420 556e 7265 6376 454f   except UnrecvEO
-0000d100: 463a 0a20 2020 2020 2020 2020 2020 2072  F:.            r
-0000d110: 6169 7365 2050 6562 6b61 6328 3432 322c  aise Pebkac(422,
-0000d120: 2022 636c 6965 6e74 2064 6973 636f 6e6e   "client disconn
-0000d130: 6563 7465 6420 7768 696c 6520 706f 7374  ected while post
-0000d140: 696e 6720 4a53 4f4e 2229 0a0a 2020 2020  ing JSON")..    
-0000d150: 2020 2020 7365 6c66 2e6c 6f67 2822 6465      self.log("de
-0000d160: 636f 6469 6e67 207b 7d20 6279 7465 7320  coding {} bytes 
-0000d170: 6f66 207b 7d20 6a73 6f6e 222e 666f 726d  of {} json".form
-0000d180: 6174 286c 656e 286a 736f 6e5f 6275 6629  at(len(json_buf)
-0000d190: 2c20 656e 6329 290a 2020 2020 2020 2020  , enc)).        
-0000d1a0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000d1b0: 2062 6f64 7920 3d20 6a73 6f6e 2e6c 6f61   body = json.loa
-0000d1c0: 6473 286a 736f 6e5f 6275 662e 6465 636f  ds(json_buf.deco
-0000d1d0: 6465 2865 6e63 2c20 2272 6570 6c61 6365  de(enc, "replace
-0000d1e0: 2229 290a 2020 2020 2020 2020 6578 6365  ")).        exce
-0000d1f0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-0000d200: 7261 6973 6520 5065 626b 6163 2834 3232  raise Pebkac(422
-0000d210: 2c20 2279 6f75 2050 4f53 5465 6420 696e  , "you POSTed in
-0000d220: 7661 6c69 6420 6a73 6f6e 2229 0a0a 2020  valid json")..  
-0000d230: 2020 2020 2020 2320 7365 6c66 2e72 6570        # self.rep
-0000d240: 6c79 2862 2263 6c6f 7564 666c 6172 6522  ly(b"cloudflare"
-0000d250: 2c20 3530 3329 0a20 2020 2020 2020 2023  , 503).        #
-0000d260: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-0000d270: 2020 2020 2020 6966 2022 7372 6368 2220        if "srch" 
-0000d280: 696e 2073 656c 662e 7570 6172 616d 206f  in self.uparam o
-0000d290: 7220 2273 7263 6822 2069 6e20 626f 6479  r "srch" in body
-0000d2a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000d2b0: 7475 726e 2073 656c 662e 6861 6e64 6c65  turn self.handle
-0000d2c0: 5f73 6561 7263 6828 626f 6479 290a 0a20  _search(body).. 
-0000d2d0: 2020 2020 2020 2069 6620 2264 656c 6574         if "delet
-0000d2e0: 6522 2069 6e20 7365 6c66 2e75 7061 7261  e" in self.upara
-0000d2f0: 6d3a 0a20 2020 2020 2020 2020 2020 2072  m:.            r
-0000d300: 6574 7572 6e20 7365 6c66 2e68 616e 646c  eturn self.handl
-0000d310: 655f 726d 2862 6f64 7929 0a0a 2020 2020  e_rm(body)..    
-0000d320: 2020 2020 6e61 6d65 203d 2075 6e64 6f74      name = undot
-0000d330: 2862 6f64 795b 226e 616d 6522 5d29 0a20  (body["name"]). 
-0000d340: 2020 2020 2020 2069 6620 222f 2220 696e         if "/" in
-0000d350: 206e 616d 653a 0a20 2020 2020 2020 2020   name:.         
-0000d360: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
-0000d370: 3430 302c 2022 796f 7572 2063 6c69 656e  400, "your clien
-0000d380: 7420 6973 206f 6c64 3b20 7072 6573 7320  t is old; press 
-0000d390: 4354 524c 2d53 4849 4654 2d52 2061 6e64  CTRL-SHIFT-R and
-0000d3a0: 2074 7279 2061 6761 696e 2229 0a0a 2020   try again")..  
-0000d3b0: 2020 2020 2020 7666 732c 2072 656d 203d        vfs, rem =
-0000d3c0: 2073 656c 662e 6173 7276 2e76 6673 2e67   self.asrv.vfs.g
-0000d3d0: 6574 2873 656c 662e 7670 6174 682c 2073  et(self.vpath, s
-0000d3e0: 656c 662e 756e 616d 652c 2046 616c 7365  elf.uname, False
-0000d3f0: 2c20 5472 7565 290a 2020 2020 2020 2020  , True).        
-0000d400: 6462 762c 2076 7265 6d20 3d20 7666 732e  dbv, vrem = vfs.
-0000d410: 6765 745f 6462 7628 7265 6d29 0a0a 2020  get_dbv(rem)..  
-0000d420: 2020 2020 2020 626f 6479 5b22 7674 6f70        body["vtop
-0000d430: 225d 203d 2064 6276 2e76 7061 7468 0a20  "] = dbv.vpath. 
-0000d440: 2020 2020 2020 2062 6f64 795b 2270 746f         body["pto
-0000d450: 7022 5d20 3d20 6462 762e 7265 616c 7061  p"] = dbv.realpa
-0000d460: 7468 0a20 2020 2020 2020 2062 6f64 795b  th.        body[
-0000d470: 2270 7265 6c22 5d20 3d20 7672 656d 0a20  "prel"] = vrem. 
-0000d480: 2020 2020 2020 2062 6f64 795b 2268 6f73         body["hos
-0000d490: 7422 5d20 3d20 7365 6c66 2e68 6f73 740a  t"] = self.host.
-0000d4a0: 2020 2020 2020 2020 626f 6479 5b22 7573          body["us
-0000d4b0: 6572 225d 203d 2073 656c 662e 756e 616d  er"] = self.unam
-0000d4c0: 650a 2020 2020 2020 2020 626f 6479 5b22  e.        body["
-0000d4d0: 6164 6472 225d 203d 2073 656c 662e 6970  addr"] = self.ip
-0000d4e0: 0a20 2020 2020 2020 2062 6f64 795b 2276  .        body["v
-0000d4f0: 6366 6722 5d20 3d20 6462 762e 666c 6167  cfg"] = dbv.flag
-0000d500: 730a 0a20 2020 2020 2020 2069 6620 6e6f  s..        if no
-0000d510: 7420 7365 6c66 2e63 616e 5f64 656c 6574  t self.can_delet
-0000d520: 653a 0a20 2020 2020 2020 2020 2020 2062  e:.            b
-0000d530: 6f64 792e 706f 7028 2272 6570 6c61 6365  ody.pop("replace
-0000d540: 222c 204e 6f6e 6529 0a0a 2020 2020 2020  ", None)..      
-0000d550: 2020 6966 2072 656d 3a0a 2020 2020 2020    if rem:.      
-0000d560: 2020 2020 2020 6473 7420 3d20 7666 732e        dst = vfs.
-0000d570: 6361 6e6f 6e69 6361 6c28 7265 6d29 0a20  canonical(rem). 
-0000d580: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5a0: 6966 206e 6f74 2062 6f73 2e70 6174 682e  if not bos.path.
-0000d5b0: 6973 6469 7228 6473 7429 3a0a 2020 2020  isdir(dst):.    
-0000d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5d0: 626f 732e 6d61 6b65 6469 7273 2864 7374  bos.makedirs(dst
-0000d5e0: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-0000d5f0: 6365 7074 204f 5345 7272 6f72 2061 7320  cept OSError as 
-0000d600: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
-0000d610: 2020 2020 7365 6c66 2e6c 6f67 2822 6d61      self.log("ma
-0000d620: 6b65 6469 7273 2066 6169 6c65 6420 5b7b  kedirs failed [{
-0000d630: 7d5d 222e 666f 726d 6174 2864 7374 2929  }]".format(dst))
-0000d640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d650: 2069 6620 6e6f 7420 626f 732e 7061 7468   if not bos.path
-0000d660: 2e69 7364 6972 2864 7374 293a 0a20 2020  .isdir(dst):.   
-0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d680: 2069 6620 6578 2e65 7272 6e6f 203d 3d20   if ex.errno == 
-0000d690: 6572 726e 6f2e 4541 4343 4553 3a0a 2020  errno.EACCES:.  
+0000aef0: 6c76 5b61 6c67 5d20 3d20 696e 7428 6e6c  lv[alg] = int(nl
+0000af00: 7629 0a20 2020 2020 2020 2020 2020 2020  v).             
+0000af10: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+0000af20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000af30: 6173 730a 0a20 2020 2020 2020 2020 2020  ass..           
+0000af40: 206c 765b 616c 675d 203d 206c 762e 6765   lv[alg] = lv.ge
+0000af50: 7428 616c 6729 206f 7220 6662 2e67 6574  t(alg) or fb.get
+0000af60: 2861 6c67 2920 6f72 2030 0a0a 2020 2020  (alg) or 0..    
+0000af70: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+0000af80: 2822 636f 6d70 7265 7373 696e 6720 7769  ("compressing wi
+0000af90: 7468 207b 7d20 6c65 7665 6c20 7b7d 222e  th {} level {}".
+0000afa0: 666f 726d 6174 2861 6c67 2c20 6c76 2e67  format(alg, lv.g
+0000afb0: 6574 2861 6c67 2929 290a 2020 2020 2020  et(alg))).      
+0000afc0: 2020 2020 2020 6966 2061 6c67 203d 3d20        if alg == 
+0000afd0: 2267 7a22 3a0a 2020 2020 2020 2020 2020  "gz":.          
+0000afe0: 2020 2020 2020 6f70 656e 5f6b 615b 2266        open_ka["f
+0000aff0: 756e 225d 203d 2067 7a69 702e 477a 6970  un"] = gzip.Gzip
+0000b000: 4669 6c65 0a20 2020 2020 2020 2020 2020  File.           
+0000b010: 2020 2020 206f 7065 6e5f 6120 3d20 5b22       open_a = ["
+0000b020: 7762 222c 206c 765b 616c 675d 2c20 4e6f  wb", lv[alg], No
+0000b030: 6e65 2c20 3078 3546 4545 3636 3030 5d20  ne, 0x5FEE6600] 
+0000b040: 2023 2032 3032 312d 3031 2d30 310a 2020   # 2021-01-01.  
+0000b050: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
+0000b060: 6c67 203d 3d20 2278 7a22 3a0a 2020 2020  lg == "xz":.    
+0000b070: 2020 2020 2020 2020 2020 2020 6f70 656e              open
+0000b080: 5f6b 6120 3d20 7b22 6675 6e22 3a20 6c7a  _ka = {"fun": lz
+0000b090: 6d61 2e6f 7065 6e2c 2022 7072 6573 6574  ma.open, "preset
+0000b0a0: 223a 206c 765b 616c 675d 7d0a 2020 2020  ": lv[alg]}.    
+0000b0b0: 2020 2020 2020 2020 2020 2020 6f70 656e              open
+0000b0c0: 5f61 203d 205b 2277 6222 5d0a 2020 2020  _a = ["wb"].    
+0000b0d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000b0e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b0f0: 6c66 2e6c 6f67 2822 6661 6c6c 7468 726f  lf.log("fallthro
+0000b100: 7567 683f 2074 6861 7473 2061 2062 7567  ugh? thats a bug
+0000b110: 222c 2031 290a 0a20 2020 2020 2020 2073  ", 1)..        s
+0000b120: 7566 6669 7820 3d20 222d 7b3a 2e36 667d  uffix = "-{:.6f}
+0000b130: 2d7b 7d22 2e66 6f72 6d61 7428 7469 6d65  -{}".format(time
+0000b140: 2e74 696d 6528 292c 2073 656c 662e 6469  .time(), self.di
+0000b150: 7028 2929 0a20 2020 2020 2020 206e 616d  p()).        nam
+0000b160: 656c 6573 7320 3d20 6e6f 7420 666e 0a20  eless = not fn. 
+0000b170: 2020 2020 2020 2069 6620 6e61 6d65 6c65         if namele
+0000b180: 7373 3a0a 2020 2020 2020 2020 2020 2020  ss:.            
+0000b190: 7375 6666 6978 202b 3d20 222e 6269 6e22  suffix += ".bin"
+0000b1a0: 0a20 2020 2020 2020 2020 2020 2066 6e20  .            fn 
+0000b1b0: 3d20 2270 7574 2220 2b20 7375 6666 6978  = "put" + suffix
+0000b1c0: 0a0a 2020 2020 2020 2020 7061 7261 6d73  ..        params
+0000b1d0: 203d 207b 2273 7566 6669 7822 3a20 7375   = {"suffix": su
+0000b1e0: 6666 6978 2c20 2266 6469 7222 3a20 6664  ffix, "fdir": fd
+0000b1f0: 6972 7d0a 2020 2020 2020 2020 6966 2073  ir}.        if s
+0000b200: 656c 662e 6172 6773 2e6e 773a 0a20 2020  elf.args.nw:.   
+0000b210: 2020 2020 2020 2020 2070 6172 616d 7320           params 
+0000b220: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
+0000b230: 2066 6e20 3d20 6f73 2e64 6576 6e75 6c6c   fn = os.devnull
+0000b240: 0a0a 2020 2020 2020 2020 7061 7261 6d73  ..        params
+0000b250: 2e75 7064 6174 6528 6f70 656e 5f6b 6129  .update(open_ka)
+0000b260: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000b270: 666e 0a0a 2020 2020 2020 2020 6966 206e  fn..        if n
+0000b280: 6f74 2073 656c 662e 6172 6773 2e6e 773a  ot self.args.nw:
+0000b290: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b2a0: 726e 643a 0a20 2020 2020 2020 2020 2020  rnd:.           
+0000b2b0: 2020 2020 2066 6e20 3d20 7261 6e64 5f6e       fn = rand_n
+0000b2c0: 616d 6528 6664 6972 2c20 666e 2c20 726e  ame(fdir, fn, rn
+0000b2d0: 6429 0a0a 2020 2020 2020 2020 2020 2020  d)..            
+0000b2e0: 666e 203d 2073 616e 6974 697a 655f 666e  fn = sanitize_fn
+0000b2f0: 2866 6e20 6f72 2022 222c 2022 222c 205b  (fn or "", "", [
+0000b300: 222e 7072 6f6c 6f67 7565 2e68 746d 6c22  ".prologue.html"
+0000b310: 2c20 222e 6570 696c 6f67 7565 2e68 746d  , ".epilogue.htm
+0000b320: 6c22 5d29 0a0a 2020 2020 2020 2020 7061  l"])..        pa
+0000b330: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+0000b340: 6e28 6664 6972 2c20 666e 290a 0a20 2020  n(fdir, fn)..   
+0000b350: 2020 2020 2069 6620 7862 753a 0a20 2020       if xbu:.   
+0000b360: 2020 2020 2020 2020 2061 7420 3d20 7469           at = ti
+0000b370: 6d65 2e74 696d 6528 2920 2d20 6c69 6665  me.time() - life
+0000b380: 7469 6d65 0a20 2020 2020 2020 2020 2020  time.           
+0000b390: 2069 6620 6e6f 7420 7275 6e68 6f6f 6b28   if not runhook(
+0000b3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b3b0: 2073 656c 662e 6c6f 672c 0a20 2020 2020   self.log,.     
+0000b3c0: 2020 2020 2020 2020 2020 2078 6275 2c0a             xbu,.
+0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3e0: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
+0000b3f0: 2020 2020 2020 7365 6c66 2e76 7061 7468        self.vpath
+0000b400: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b410: 2020 7365 6c66 2e68 6f73 742c 0a20 2020    self.host,.   
+0000b420: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b430: 662e 756e 616d 652c 0a20 2020 2020 2020  f.uname,.       
+0000b440: 2020 2020 2020 2020 2061 742c 0a20 2020           at,.   
+0000b450: 2020 2020 2020 2020 2020 2020 2072 656d               rem
+0000b460: 6169 6e73 2c0a 2020 2020 2020 2020 2020  ains,.          
+0000b470: 2020 2020 2020 7365 6c66 2e69 702c 0a20        self.ip,. 
+0000b480: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000b490: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+0000b4a0: 2020 2022 222c 0a20 2020 2020 2020 2020     "",.         
+0000b4b0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0000b4c0: 2020 2020 2020 7420 3d20 2275 706c 6f61        t = "uploa
+0000b4d0: 6420 626c 6f63 6b65 6420 6279 2078 6275  d blocked by xbu
+0000b4e0: 2073 6572 7665 7220 636f 6e66 6967 220a   server config".
+0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b500: 7365 6c66 2e6c 6f67 2874 2c20 3129 0a20  self.log(t, 1). 
+0000b510: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000b520: 6169 7365 2050 6562 6b61 6328 3430 332c  aise Pebkac(403,
+0000b530: 2074 290a 0a20 2020 2020 2020 2069 6620   t)..        if 
+0000b540: 6973 5f70 7574 2061 6e64 206e 6f74 2028  is_put and not (
+0000b550: 7365 6c66 2e61 7267 732e 6e6f 5f64 6176  self.args.no_dav
+0000b560: 206f 7220 7365 6c66 2e61 7267 732e 6e77   or self.args.nw
+0000b570: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
+0000b580: 2061 6c6c 6f77 206f 7665 7277 7269 7465   allow overwrite
+0000b590: 2069 662e 2e2e 0a20 2020 2020 2020 2020   if....         
+0000b5a0: 2020 2023 2020 2a20 766f 6c66 6c61 6720     #  * volflag 
+0000b5b0: 2764 6177 2720 6973 2073 6574 0a20 2020  'daw' is set.   
+0000b5c0: 2020 2020 2020 2020 2023 2020 2a20 616e           #  * an
+0000b5d0: 6420 6163 636f 756e 7420 6861 7320 6465  d account has de
+0000b5e0: 6c65 7465 2d61 6363 6573 730a 2020 2020  lete-access.    
+0000b5f0: 2020 2020 2020 2020 2320 6f72 2e2e 2e0a          # or....
+0000b600: 2020 2020 2020 2020 2020 2020 2320 202a              #  *
+0000b610: 2066 696c 6520 6578 6973 7473 2c20 6973   file exists, is
+0000b620: 2065 6d70 7479 2c20 7375 6666 6963 6965   empty, sufficie
+0000b630: 6e74 6c79 206e 6577 0a20 2020 2020 2020  ntly new.       
+0000b640: 2020 2020 2023 2020 2a20 616e 6420 7468       #  * and th
+0000b650: 6572 6520 6973 206e 6f20 2e50 4152 5449  ere is no .PARTI
+0000b660: 414c 0a0a 2020 2020 2020 2020 2020 2020  AL..            
+0000b670: 746e 616d 203d 2066 6e20 2b20 222e 5041  tnam = fn + ".PA
+0000b680: 5254 4941 4c22 0a20 2020 2020 2020 2020  RTIAL".         
+0000b690: 2020 2069 6620 7365 6c66 2e61 7267 732e     if self.args.
+0000b6a0: 646f 7470 6172 743a 0a20 2020 2020 2020  dotpart:.       
+0000b6b0: 2020 2020 2020 2020 2074 6e61 6d20 3d20           tnam = 
+0000b6c0: 222e 2220 2b20 746e 616d 0a0a 2020 2020  "." + tnam..    
+0000b6d0: 2020 2020 2020 2020 6966 2028 7666 732e          if (vfs.
+0000b6e0: 666c 6167 732e 6765 7428 2264 6177 2229  flags.get("daw")
+0000b6f0: 2061 6e64 2073 656c 662e 6361 6e5f 6465   and self.can_de
+0000b700: 6c65 7465 2920 6f72 2028 0a20 2020 2020  lete) or (.     
+0000b710: 2020 2020 2020 2020 2020 206e 6f74 2062             not b
+0000b720: 6f73 2e70 6174 682e 6578 6973 7473 286f  os.path.exists(o
+0000b730: 732e 7061 7468 2e6a 6f69 6e28 6664 6972  s.path.join(fdir
+0000b740: 2c20 746e 616d 2929 0a20 2020 2020 2020  , tnam)).       
+0000b750: 2020 2020 2020 2020 2061 6e64 2062 6f73           and bos
+0000b760: 2e70 6174 682e 6578 6973 7473 2870 6174  .path.exists(pat
+0000b770: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
+0000b780: 2020 2061 6e64 206e 6f74 2062 6f73 2e70     and not bos.p
+0000b790: 6174 682e 6765 7473 697a 6528 7061 7468  ath.getsize(path
+0000b7a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000b7b0: 2020 616e 6420 626f 732e 7061 7468 2e67    and bos.path.g
+0000b7c0: 6574 6d74 696d 6528 7061 7468 2920 3e3d  etmtime(path) >=
+0000b7d0: 2074 696d 652e 7469 6d65 2829 202d 2073   time.time() - s
+0000b7e0: 656c 662e 6172 6773 2e62 6c61 6e6b 5f77  elf.args.blank_w
+0000b7f0: 740a 2020 2020 2020 2020 2020 2020 293a  t.            ):
+0000b800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b810: 2023 2073 6d61 6c6c 2074 6f63 746f 752c   # small toctou,
+0000b820: 2062 7574 2062 6574 7465 7220 7468 616e   but better than
+0000b830: 2063 6c6f 6262 6572 696e 6720 6120 6861   clobbering a ha
+0000b840: 7264 6c69 6e6b 0a20 2020 2020 2020 2020  rdlink.         
+0000b850: 2020 2020 2020 2062 6f73 2e75 6e6c 696e         bos.unlin
+0000b860: 6b28 7061 7468 290a 0a20 2020 2020 2020  k(path)..       
+0000b870: 2077 6974 6820 7265 6e5f 6f70 656e 2866   with ren_open(f
+0000b880: 6e2c 202a 6f70 656e 5f61 2c20 2a2a 7061  n, *open_a, **pa
+0000b890: 7261 6d73 2920 6173 207a 6677 3a0a 2020  rams) as zfw:.  
+0000b8a0: 2020 2020 2020 2020 2020 662c 2066 6e20            f, fn 
+0000b8b0: 3d20 7a66 775b 226f 727a 225d 0a20 2020  = zfw["orz"].   
+0000b8c0: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
+0000b8d0: 6f73 2e70 6174 682e 6a6f 696e 2866 6469  os.path.join(fdi
+0000b8e0: 722c 2066 6e29 0a20 2020 2020 2020 2020  r, fn).         
+0000b8f0: 2020 2070 6f73 745f 737a 2c20 7368 615f     post_sz, sha_
+0000b900: 6865 782c 2073 6861 5f62 3634 203d 2068  hex, sha_b64 = h
+0000b910: 6173 6863 6f70 7928 7265 6164 6572 2c20  ashcopy(reader, 
+0000b920: 662c 2073 656c 662e 6172 6773 2e73 5f77  f, self.args.s_w
+0000b930: 725f 736c 7029 0a0a 2020 2020 2020 2020  r_slp)..        
+0000b940: 6966 206c 696d 3a0a 2020 2020 2020 2020  if lim:.        
+0000b950: 2020 2020 6c69 6d2e 6e75 7028 7365 6c66      lim.nup(self
+0000b960: 2e69 7029 0a20 2020 2020 2020 2020 2020  .ip).           
+0000b970: 206c 696d 2e62 7570 2873 656c 662e 6970   lim.bup(self.ip
+0000b980: 2c20 706f 7374 5f73 7a29 0a20 2020 2020  , post_sz).     
+0000b990: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000b9a0: 2020 2020 2020 2020 2020 2020 6c69 6d2e              lim.
+0000b9b0: 6368 6b5f 737a 2870 6f73 745f 737a 290a  chk_sz(post_sz).
+0000b9c0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0000b9d0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+0000b9e0: 2020 2020 626f 732e 756e 6c69 6e6b 2870      bos.unlink(p
+0000b9f0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+0000ba00: 2020 2020 2072 6169 7365 0a0a 2020 2020       raise..    
+0000ba10: 2020 2020 6966 2073 656c 662e 6172 6773      if self.args
+0000ba20: 2e6e 773a 0a20 2020 2020 2020 2020 2020  .nw:.           
+0000ba30: 2072 6574 7572 6e20 706f 7374 5f73 7a2c   return post_sz,
+0000ba40: 2073 6861 5f68 6578 2c20 7368 615f 6236   sha_hex, sha_b6
+0000ba50: 342c 2072 656d 6169 6e73 2c20 7061 7468  4, remains, path
+0000ba60: 2c20 2222 0a0a 2020 2020 2020 2020 6966  , ""..        if
+0000ba70: 206e 616d 656c 6573 7320 616e 6420 226d   nameless and "m
+0000ba80: 6167 6963 2220 696e 2076 6673 2e66 6c61  agic" in vfs.fla
+0000ba90: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000baa0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000bab0: 2020 2020 2065 7874 203d 2073 656c 662e       ext = self.
+0000bac0: 636f 6e6e 2e68 7372 762e 6d61 6769 6369  conn.hsrv.magici
+0000bad0: 616e 2e65 7874 2870 6174 6829 0a20 2020  an.ext(path).   
+0000bae0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+0000baf0: 4578 6365 7074 696f 6e20 6173 2065 783a  Exception as ex:
+0000bb00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bb10: 2073 656c 662e 6c6f 6728 2266 696c 6574   self.log("filet
+0000bb20: 7970 6520 6465 7465 6374 696f 6e20 6661  ype detection fa
+0000bb30: 696c 6564 2066 6f72 205b 7b7d 5d3a 207b  iled for [{}]: {
+0000bb40: 7d22 2e66 6f72 6d61 7428 7061 7468 2c20  }".format(path, 
+0000bb50: 6578 292c 2036 290a 2020 2020 2020 2020  ex), 6).        
+0000bb60: 2020 2020 2020 2020 6578 7420 3d20 4e6f          ext = No
+0000bb70: 6e65 0a0a 2020 2020 2020 2020 2020 2020  ne..            
+0000bb80: 6966 2065 7874 3a0a 2020 2020 2020 2020  if ext:.        
+0000bb90: 2020 2020 2020 2020 6966 2072 6e64 3a0a          if rnd:.
+0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbb0: 2020 2020 666e 3220 3d20 7261 6e64 5f6e      fn2 = rand_n
+0000bbc0: 616d 6528 6664 6972 2c20 2261 2e22 202b  ame(fdir, "a." +
+0000bbd0: 2065 7874 2c20 726e 6429 0a20 2020 2020   ext, rnd).     
+0000bbe0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000bbf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bc00: 2020 2020 2066 6e32 203d 2066 6e2e 7273       fn2 = fn.rs
+0000bc10: 706c 6974 2822 2e22 2c20 3129 5b30 5d20  plit(".", 1)[0] 
+0000bc20: 2b20 222e 2220 2b20 6578 740a 0a20 2020  + "." + ext..   
+0000bc30: 2020 2020 2020 2020 2020 2020 2070 6172               par
+0000bc40: 616d 735b 2273 7566 6669 7822 5d20 3d20  ams["suffix"] = 
+0000bc50: 7375 6666 6978 5b3a 2d34 5d0a 2020 2020  suffix[:-4].    
+0000bc60: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000bc70: 2072 656e 5f6f 7065 6e28 666e 2c20 2a6f   ren_open(fn, *o
+0000bc80: 7065 6e5f 612c 202a 2a70 6172 616d 7329  pen_a, **params)
+0000bc90: 2061 7320 7a66 773a 0a20 2020 2020 2020   as zfw:.       
+0000bca0: 2020 2020 2020 2020 2020 2020 2066 2c20               f, 
+0000bcb0: 666e 203d 207a 6677 5b22 6f72 7a22 5d0a  fn = zfw["orz"].
+0000bcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bcd0: 2070 6174 6832 203d 206f 732e 7061 7468   path2 = os.path
+0000bce0: 2e6a 6f69 6e28 6664 6972 2c20 666e 3229  .join(fdir, fn2)
+0000bcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bd00: 2061 746f 6d69 635f 6d6f 7665 2870 6174   atomic_move(pat
+0000bd10: 682c 2070 6174 6832 290a 2020 2020 2020  h, path2).      
+0000bd20: 2020 2020 2020 2020 2020 666e 203d 2066            fn = f
+0000bd30: 6e32 0a20 2020 2020 2020 2020 2020 2020  n2.             
+0000bd40: 2020 2070 6174 6820 3d20 7061 7468 320a     path = path2.
+0000bd50: 0a20 2020 2020 2020 2061 7420 3d20 7469  .        at = ti
+0000bd60: 6d65 2e74 696d 6528 2920 2d20 6c69 6665  me.time() - life
+0000bd70: 7469 6d65 0a20 2020 2020 2020 2069 6620  time.        if 
+0000bd80: 7861 7520 616e 6420 6e6f 7420 7275 6e68  xau and not runh
+0000bd90: 6f6f 6b28 0a20 2020 2020 2020 2020 2020  ook(.           
+0000bda0: 2073 656c 662e 6c6f 672c 0a20 2020 2020   self.log,.     
+0000bdb0: 2020 2020 2020 2078 6175 2c0a 2020 2020         xau,.    
+0000bdc0: 2020 2020 2020 2020 7061 7468 2c0a 2020          path,.  
+0000bdd0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+0000bde0: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
+0000bdf0: 2020 7365 6c66 2e68 6f73 742c 0a20 2020    self.host,.   
+0000be00: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+0000be10: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+0000be20: 2061 742c 0a20 2020 2020 2020 2020 2020   at,.           
+0000be30: 2070 6f73 745f 737a 2c0a 2020 2020 2020   post_sz,.      
+0000be40: 2020 2020 2020 7365 6c66 2e69 702c 0a20        self.ip,. 
+0000be50: 2020 2020 2020 2020 2020 2061 742c 0a20             at,. 
+0000be60: 2020 2020 2020 2020 2020 2022 222c 0a20             "",. 
+0000be70: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+0000be80: 2020 2020 2020 7420 3d20 2275 706c 6f61        t = "uploa
+0000be90: 6420 626c 6f63 6b65 6420 6279 2078 6175  d blocked by xau
+0000bea0: 2073 6572 7665 7220 636f 6e66 6967 220a   server config".
+0000beb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000bec0: 2e6c 6f67 2874 2c20 3129 0a20 2020 2020  .log(t, 1).     
+0000bed0: 2020 2020 2020 206f 732e 756e 6c69 6e6b         os.unlink
+0000bee0: 2870 6174 6829 0a20 2020 2020 2020 2020  (path).         
+0000bef0: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
+0000bf00: 3430 332c 2074 290a 0a20 2020 2020 2020  403, t)..       
+0000bf10: 2076 6673 2c20 7265 6d20 3d20 7666 732e   vfs, rem = vfs.
+0000bf20: 6765 745f 6462 7628 7265 6d29 0a20 2020  get_dbv(rem).   
+0000bf30: 2020 2020 2073 656c 662e 636f 6e6e 2e68       self.conn.h
+0000bf40: 7372 762e 6272 6f6b 6572 2e73 6179 280a  srv.broker.say(.
+0000bf50: 2020 2020 2020 2020 2020 2020 2275 7032              "up2
+0000bf60: 6b2e 6861 7368 5f66 696c 6522 2c0a 2020  k.hash_file",.  
+0000bf70: 2020 2020 2020 2020 2020 7666 732e 7265            vfs.re
+0000bf80: 616c 7061 7468 2c0a 2020 2020 2020 2020  alpath,.        
+0000bf90: 2020 2020 7666 732e 7670 6174 682c 0a20      vfs.vpath,. 
+0000bfa0: 2020 2020 2020 2020 2020 2076 6673 2e66             vfs.f
+0000bfb0: 6c61 6773 2c0a 2020 2020 2020 2020 2020  lags,.          
+0000bfc0: 2020 7265 6d2c 0a20 2020 2020 2020 2020    rem,.         
+0000bfd0: 2020 2066 6e2c 0a20 2020 2020 2020 2020     fn,.         
+0000bfe0: 2020 2073 656c 662e 6970 2c0a 2020 2020     self.ip,.    
+0000bff0: 2020 2020 2020 2020 6174 2c0a 2020 2020          at,.    
+0000c000: 2020 2020 2020 2020 7365 6c66 2e75 6e61          self.una
+0000c010: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+0000c020: 5472 7565 2c0a 2020 2020 2020 2020 290a  True,.        ).
+0000c030: 0a20 2020 2020 2020 2076 7375 6620 3d20  .        vsuf = 
+0000c040: 2222 0a20 2020 2020 2020 2069 6620 2873  "".        if (s
+0000c050: 656c 662e 6361 6e5f 7265 6164 206f 7220  elf.can_read or 
+0000c060: 7365 6c66 2e63 616e 5f75 7067 6574 2920  self.can_upget) 
+0000c070: 616e 6420 2266 6b22 2069 6e20 7666 732e  and "fk" in vfs.
+0000c080: 666c 6167 733a 0a20 2020 2020 2020 2020  flags:.         
+0000c090: 2020 2076 7375 6620 3d20 223f 6b3d 2220     vsuf = "?k=" 
+0000c0a0: 2b20 7365 6c66 2e67 656e 5f66 6b28 0a20  + self.gen_fk(. 
+0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c0c0: 656c 662e 6172 6773 2e66 6b5f 7361 6c74  elf.args.fk_salt
+0000c0d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c0e0: 2020 7061 7468 2c0a 2020 2020 2020 2020    path,.        
+0000c0f0: 2020 2020 2020 2020 706f 7374 5f73 7a2c          post_sz,
+0000c100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c110: 2030 2069 6620 414e 5957 494e 2065 6c73   0 if ANYWIN els
+0000c120: 6520 626f 732e 7374 6174 2870 6174 6829  e bos.stat(path)
+0000c130: 2e73 745f 696e 6f2c 0a20 2020 2020 2020  .st_ino,.       
+0000c140: 2020 2020 2029 5b3a 2076 6673 2e66 6c61       )[: vfs.fla
+0000c150: 6773 5b22 666b 225d 5d0a 0a20 2020 2020  gs["fk"]]..     
+0000c160: 2020 2076 7061 7468 203d 2022 2f22 2e6a     vpath = "/".j
+0000c170: 6f69 6e28 5b78 2066 6f72 2078 2069 6e20  oin([x for x in 
+0000c180: 5b76 6673 2e76 7061 7468 2c20 7265 6d2c  [vfs.vpath, rem,
+0000c190: 2066 6e5d 2069 6620 785d 290a 2020 2020   fn] if x]).    
+0000c1a0: 2020 2020 7670 6174 6820 3d20 7175 6f74      vpath = quot
+0000c1b0: 6570 2876 7061 7468 290a 0a20 2020 2020  ep(vpath)..     
+0000c1c0: 2020 2075 726c 203d 2022 7b7d 3a2f 2f7b     url = "{}://{
+0000c1d0: 7d2f 7b7d 222e 666f 726d 6174 280a 2020  }/{}".format(.  
+0000c1e0: 2020 2020 2020 2020 2020 2268 7474 7073            "https
+0000c1f0: 2220 6966 2073 656c 662e 6973 5f68 7474  " if self.is_htt
+0000c200: 7073 2065 6c73 6520 2268 7474 7022 2c0a  ps else "http",.
+0000c210: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c220: 2e68 6f73 742c 0a20 2020 2020 2020 2020  .host,.         
+0000c230: 2020 2073 656c 662e 6172 6773 2e52 5320     self.args.RS 
+0000c240: 2b20 7670 6174 6820 2b20 7673 7566 2c0a  + vpath + vsuf,.
+0000c250: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000c260: 2020 2072 6574 7572 6e20 706f 7374 5f73     return post_s
+0000c270: 7a2c 2073 6861 5f68 6578 2c20 7368 615f  z, sha_hex, sha_
+0000c280: 6236 342c 2072 656d 6169 6e73 2c20 7061  b64, remains, pa
+0000c290: 7468 2c20 7572 6c0a 0a20 2020 2064 6566  th, url..    def
+0000c2a0: 2068 616e 646c 655f 7374 6173 6828 7365   handle_stash(se
+0000c2b0: 6c66 2c20 6973 5f70 7574 2029 2020 3a0a  lf, is_put )  :.
+0000c2c0: 2020 2020 2020 2020 706f 7374 5f73 7a2c          post_sz,
+0000c2d0: 2073 6861 5f68 6578 2c20 7368 615f 6236   sha_hex, sha_b6
+0000c2e0: 342c 2072 656d 6169 6e73 2c20 7061 7468  4, remains, path
+0000c2f0: 2c20 7572 6c20 3d20 7365 6c66 2e64 756d  , url = self.dum
+0000c300: 705f 746f 5f66 696c 6528 6973 5f70 7574  p_to_file(is_put
+0000c310: 290a 2020 2020 2020 2020 7370 6420 3d20  ).        spd = 
+0000c320: 7365 6c66 2e5f 7370 6428 706f 7374 5f73  self._spd(post_s
+0000c330: 7a29 0a20 2020 2020 2020 2074 203d 2022  z).        t = "
+0000c340: 7b7d 2077 726f 7465 207b 7d2f 7b7d 2062  {} wrote {}/{} b
+0000c350: 7974 6573 2074 6f20 7b7d 2020 2320 7b7d  ytes to {}  # {}
+0000c360: 220a 2020 2020 2020 2020 7365 6c66 2e6c  ".        self.l
+0000c370: 6f67 2874 2e66 6f72 6d61 7428 7370 642c  og(t.format(spd,
+0000c380: 2070 6f73 745f 737a 2c20 7265 6d61 696e   post_sz, remain
+0000c390: 732c 2070 6174 682c 2073 6861 5f62 3634  s, path, sha_b64
+0000c3a0: 5b3a 3238 5d29 2920 2023 2032 310a 0a20  [:28]))  # 21.. 
+0000c3b0: 2020 2020 2020 2061 6320 3d20 7365 6c66         ac = self
+0000c3c0: 2e75 7061 7261 6d2e 6765 7428 0a20 2020  .uparam.get(.   
+0000c3d0: 2020 2020 2020 2020 2022 7761 6e74 222c           "want",
+0000c3e0: 2073 656c 662e 6865 6164 6572 732e 6765   self.headers.ge
+0000c3f0: 7428 2261 6363 6570 7422 2c20 2222 292e  t("accept", "").
+0000c400: 6c6f 7765 7228 292e 7370 6c69 7428 223b  lower().split(";
+0000c410: 2229 5b2d 315d 0a20 2020 2020 2020 2029  ")[-1].        )
+0000c420: 0a20 2020 2020 2020 2069 6620 6163 203d  .        if ac =
+0000c430: 3d20 2275 726c 223a 0a20 2020 2020 2020  = "url":.       
+0000c440: 2020 2020 2074 203d 2075 726c 0a20 2020       t = url.   
+0000c450: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000c460: 2020 2020 2020 2074 203d 2022 7b7d 5c6e         t = "{}\n
+0000c470: 7b7d 5c6e 7b7d 5c6e 7b7d 5c6e 222e 666f  {}\n{}\n{}\n".fo
+0000c480: 726d 6174 2870 6f73 745f 737a 2c20 7368  rmat(post_sz, sh
+0000c490: 615f 6236 342c 2073 6861 5f68 6578 5b3a  a_b64, sha_hex[:
+0000c4a0: 3536 5d2c 2075 726c 290a 0a20 2020 2020  56], url)..     
+0000c4b0: 2020 2068 203d 207b 224c 6f63 6174 696f     h = {"Locatio
+0000c4c0: 6e22 3a20 7572 6c7d 2069 6620 6973 5f70  n": url} if is_p
+0000c4d0: 7574 2061 6e64 2075 726c 2065 6c73 6520  ut and url else 
+0000c4e0: 7b7d 0a20 2020 2020 2020 2073 656c 662e  {}.        self.
+0000c4f0: 7265 706c 7928 742e 656e 636f 6465 2822  reply(t.encode("
+0000c500: 7574 662d 3822 292c 2032 3031 2c20 6865  utf-8"), 201, he
+0000c510: 6164 6572 733d 6829 0a20 2020 2020 2020  aders=h).       
+0000c520: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
+0000c530: 2020 6465 6620 6261 6b66 6c69 7028 7365    def bakflip(se
+0000c540: 6c66 2c20 6620 2c20 6f66 7320 2c20 737a  lf, f , ofs , sz
+0000c550: 202c 2073 6861 2029 2020 3a0a 2020 2020   , sha )  :.    
+0000c560: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+0000c570: 6172 6773 2e62 616b 5f66 6c69 7073 206f  args.bak_flips o
+0000c580: 7220 7365 6c66 2e61 7267 732e 6e77 3a0a  r self.args.nw:.
+0000c590: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c5a0: 726e 0a0a 2020 2020 2020 2020 7364 6972  rn..        sdir
+0000c5b0: 203d 2073 656c 662e 6172 6773 2e62 665f   = self.args.bf_
+0000c5c0: 6469 720a 2020 2020 2020 2020 6670 203d  dir.        fp =
+0000c5d0: 206f 732e 7061 7468 2e6a 6f69 6e28 7364   os.path.join(sd
+0000c5e0: 6972 2c20 7368 6129 0a20 2020 2020 2020  ir, sha).       
+0000c5f0: 2069 6620 626f 732e 7061 7468 2e65 7869   if bos.path.exi
+0000c600: 7374 7328 6670 293a 0a20 2020 2020 2020  sts(fp):.       
+0000c610: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000c620: 2e6c 6f67 2822 6e6f 2062 616b 666c 6970  .log("no bakflip
+0000c630: 3b20 6861 7665 2069 7422 2c20 3629 0a0a  ; have it", 6)..
+0000c640: 2020 2020 2020 2020 6966 206e 6f74 2062          if not b
+0000c650: 6f73 2e70 6174 682e 6973 6469 7228 7364  os.path.isdir(sd
+0000c660: 6972 293a 0a20 2020 2020 2020 2020 2020  ir):.           
+0000c670: 2062 6f73 2e6d 616b 6564 6972 7328 7364   bos.makedirs(sd
+0000c680: 6972 290a 0a20 2020 2020 2020 2069 6620  ir)..        if 
+0000c690: 6c65 6e28 626f 732e 6c69 7374 6469 7228  len(bos.listdir(
+0000c6a0: 7364 6972 2929 203e 3d20 7365 6c66 2e61  sdir)) >= self.a
+0000c6b0: 7267 732e 6266 5f6e 633a 0a20 2020 2020  rgs.bf_nc:.     
+0000c6c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000c6d0: 6c66 2e6c 6f67 2822 6e6f 2062 616b 666c  lf.log("no bakfl
+0000c6e0: 6970 3b20 746f 6f20 6d61 6e79 222c 2033  ip; too many", 3
+0000c6f0: 290a 0a20 2020 2020 2020 206e 7265 6d20  )..        nrem 
+0000c700: 3d20 737a 0a20 2020 2020 2020 2066 2e73  = sz.        f.s
+0000c710: 6565 6b28 6f66 7329 0a20 2020 2020 2020  eek(ofs).       
+0000c720: 2077 6974 6820 6f70 656e 2866 702c 2022   with open(fp, "
+0000c730: 7762 2229 2061 7320 666f 3a0a 2020 2020  wb") as fo:.    
+0000c740: 2020 2020 2020 2020 7768 696c 6520 6e72          while nr
+0000c750: 656d 3a0a 2020 2020 2020 2020 2020 2020  em:.            
+0000c760: 2020 2020 6275 6620 3d20 662e 7265 6164      buf = f.read
+0000c770: 286d 696e 286e 7265 6d2c 2035 3132 202a  (min(nrem, 512 *
+0000c780: 2031 3032 3429 290a 2020 2020 2020 2020   1024)).        
+0000c790: 2020 2020 2020 2020 6966 206e 6f74 2062          if not b
+0000c7a0: 7566 3a0a 2020 2020 2020 2020 2020 2020  uf:.            
+0000c7b0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
+0000c7c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000c7d0: 7265 6d20 2d3d 206c 656e 2862 7566 290a  rem -= len(buf).
+0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7f0: 666f 2e77 7269 7465 2862 7566 290a 0a20  fo.write(buf).. 
+0000c800: 2020 2020 2020 2069 6620 6e72 656d 3a0a         if nrem:.
+0000c810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c820: 2e6c 6f67 2822 6261 6b66 6c69 7020 7472  .log("bakflip tr
+0000c830: 756e 6361 7465 643b 207b 7d20 7265 6d61  uncated; {} rema
+0000c840: 696e 7322 2e66 6f72 6d61 7428 6e72 656d  ins".format(nrem
+0000c850: 292c 2031 290a 2020 2020 2020 2020 2020  ), 1).          
+0000c860: 2020 6174 6f6d 6963 5f6d 6f76 6528 6670    atomic_move(fp
+0000c870: 2c20 6670 202b 2022 2e74 7275 6e63 2229  , fp + ".trunc")
+0000c880: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000c890: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c8a0: 6c6f 6728 2262 616b 666c 6970 206f 6b22  log("bakflip ok"
+0000c8b0: 2c20 3229 0a0a 2020 2020 6465 6620 5f73  , 2)..    def _s
+0000c8c0: 7064 2873 656c 662c 206e 6279 7465 7320  pd(self, nbytes 
+0000c8d0: 2c20 6164 6420 203d 2054 7275 6529 2020  , add  = True)  
+0000c8e0: 3a0a 2020 2020 2020 2020 6966 2061 6464  :.        if add
+0000c8f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000c900: 6c66 2e63 6f6e 6e2e 6e62 7974 6520 2b3d  lf.conn.nbyte +=
+0000c910: 206e 6279 7465 730a 0a20 2020 2020 2020   nbytes..       
+0000c920: 2073 7064 3120 3d20 6765 745f 7370 6428   spd1 = get_spd(
+0000c930: 6e62 7974 6573 2c20 7365 6c66 2e74 3029  nbytes, self.t0)
+0000c940: 0a20 2020 2020 2020 2073 7064 3220 3d20  .        spd2 = 
+0000c950: 6765 745f 7370 6428 7365 6c66 2e63 6f6e  get_spd(self.con
+0000c960: 6e2e 6e62 7974 652c 2073 656c 662e 636f  n.nbyte, self.co
+0000c970: 6e6e 2e74 3029 0a20 2020 2020 2020 2072  nn.t0).        r
+0000c980: 6574 7572 6e20 227b 7d20 7b7d 206e 7b7d  eturn "{} {} n{}
+0000c990: 222e 666f 726d 6174 2873 7064 312c 2073  ".format(spd1, s
+0000c9a0: 7064 322c 2073 656c 662e 636f 6e6e 2e6e  pd2, self.conn.n
+0000c9b0: 7265 7129 0a0a 2020 2020 6465 6620 6861  req)..    def ha
+0000c9c0: 6e64 6c65 5f70 6f73 745f 6d75 6c74 6970  ndle_post_multip
+0000c9d0: 6172 7428 7365 6c66 2920 203a 0a20 2020  art(self)  :.   
+0000c9e0: 2020 2020 2073 656c 662e 7061 7273 6572       self.parser
+0000c9f0: 203d 204d 756c 7469 7061 7274 5061 7273   = MultipartPars
+0000ca00: 6572 2873 656c 662e 6c6f 672c 2073 656c  er(self.log, sel
+0000ca10: 662e 7372 2c20 7365 6c66 2e68 6561 6465  f.sr, self.heade
+0000ca20: 7273 290a 2020 2020 2020 2020 7365 6c66  rs).        self
+0000ca30: 2e70 6172 7365 722e 7061 7273 6528 290a  .parser.parse().
+0000ca40: 0a20 2020 2020 2020 2061 6374 203d 2073  .        act = s
+0000ca50: 656c 662e 7061 7273 6572 2e72 6571 7569  elf.parser.requi
+0000ca60: 7265 2822 6163 7422 2c20 3634 290a 0a20  re("act", 64).. 
+0000ca70: 2020 2020 2020 2069 6620 6163 7420 3d3d         if act ==
+0000ca80: 2022 6c6f 6769 6e22 3a0a 2020 2020 2020   "login":.      
+0000ca90: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000caa0: 662e 6861 6e64 6c65 5f6c 6f67 696e 2829  f.handle_login()
+0000cab0: 0a0a 2020 2020 2020 2020 6966 2061 6374  ..        if act
+0000cac0: 203d 3d20 226d 6b64 6972 223a 0a20 2020   == "mkdir":.   
+0000cad0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000cae0: 7365 6c66 2e68 616e 646c 655f 6d6b 6469  self.handle_mkdi
+0000caf0: 7228 290a 0a20 2020 2020 2020 2069 6620  r()..        if 
+0000cb00: 6163 7420 3d3d 2022 6e65 775f 6d64 223a  act == "new_md":
+0000cb10: 0a20 2020 2020 2020 2020 2020 2023 206b  .            # k
+0000cb20: 696e 6461 2073 696c 6c79 2062 7574 2068  inda silly but h
+0000cb30: 6173 2074 6865 206c 6561 7374 2073 6964  as the least sid
+0000cb40: 6520 6566 6665 6374 730a 2020 2020 2020  e effects.      
+0000cb50: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000cb60: 662e 6861 6e64 6c65 5f6e 6577 5f6d 6428  f.handle_new_md(
+0000cb70: 290a 0a20 2020 2020 2020 2069 6620 6163  )..        if ac
+0000cb80: 7420 3d3d 2022 6270 7574 223a 0a20 2020  t == "bput":.   
+0000cb90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000cba0: 7365 6c66 2e68 616e 646c 655f 706c 6169  self.handle_plai
+0000cbb0: 6e5f 7570 6c6f 6164 2829 0a0a 2020 2020  n_upload()..    
+0000cbc0: 2020 2020 6966 2061 6374 203d 3d20 2274      if act == "t
+0000cbd0: 7075 7422 3a0a 2020 2020 2020 2020 2020  put":.          
+0000cbe0: 2020 7265 7475 726e 2073 656c 662e 6861    return self.ha
+0000cbf0: 6e64 6c65 5f74 6578 745f 7570 6c6f 6164  ndle_text_upload
+0000cc00: 2829 0a0a 2020 2020 2020 2020 6966 2061  ()..        if a
+0000cc10: 6374 203d 3d20 227a 6970 223a 0a20 2020  ct == "zip":.   
+0000cc20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000cc30: 7365 6c66 2e68 616e 646c 655f 7a69 705f  self.handle_zip_
+0000cc40: 706f 7374 2829 0a0a 2020 2020 2020 2020  post()..        
+0000cc50: 7261 6973 6520 5065 626b 6163 2834 3232  raise Pebkac(422
+0000cc60: 2c20 2769 6e76 616c 6964 2061 6374 696f  , 'invalid actio
+0000cc70: 6e20 227b 7d22 272e 666f 726d 6174 2861  n "{}"'.format(a
+0000cc80: 6374 2929 0a0a 2020 2020 6465 6620 6861  ct))..    def ha
+0000cc90: 6e64 6c65 5f7a 6970 5f70 6f73 7428 7365  ndle_zip_post(se
+0000cca0: 6c66 2920 203a 0a20 2020 2020 2020 2061  lf)  :.        a
+0000ccb0: 7373 6572 7420 7365 6c66 2e70 6172 7365  ssert self.parse
+0000ccc0: 720a 2020 2020 2020 2020 7472 793a 0a20  r.        try:. 
+0000ccd0: 2020 2020 2020 2020 2020 206b 203d 206e             k = n
+0000cce0: 6578 7428 7820 666f 7220 7820 696e 2073  ext(x for x in s
+0000ccf0: 656c 662e 7570 6172 616d 2069 6620 7820  elf.uparam if x 
+0000cd00: 696e 2028 227a 6970 222c 2022 7461 7222  in ("zip", "tar"
+0000cd10: 2929 0a20 2020 2020 2020 2065 7863 6570  )).        excep
+0000cd20: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+0000cd30: 6169 7365 2050 6562 6b61 6328 3432 322c  aise Pebkac(422,
+0000cd40: 2022 6e65 6564 207a 6970 206f 7220 7461   "need zip or ta
+0000cd50: 7220 6b65 7977 6f72 6422 290a 0a20 2020  r keyword")..   
+0000cd60: 2020 2020 2076 203d 2073 656c 662e 7570       v = self.up
+0000cd70: 6172 616d 5b6b 5d0a 0a20 2020 2020 2020  aram[k]..       
+0000cd80: 2076 6e2c 2072 656d 203d 2073 656c 662e   vn, rem = self.
+0000cd90: 6173 7276 2e76 6673 2e67 6574 2873 656c  asrv.vfs.get(sel
+0000cda0: 662e 7670 6174 682c 2073 656c 662e 756e  f.vpath, self.un
+0000cdb0: 616d 652c 2054 7275 652c 2046 616c 7365  ame, True, False
+0000cdc0: 290a 2020 2020 2020 2020 7a73 203d 2073  ).        zs = s
+0000cdd0: 656c 662e 7061 7273 6572 2e72 6571 7569  elf.parser.requi
+0000cde0: 7265 2822 6669 6c65 7322 2c20 3130 3234  re("files", 1024
+0000cdf0: 202a 2031 3032 3429 0a20 2020 2020 2020   * 1024).       
+0000ce00: 2069 6620 6e6f 7420 7a73 3a0a 2020 2020   if not zs:.    
+0000ce10: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
+0000ce20: 626b 6163 2834 3232 2c20 226e 6565 6420  bkac(422, "need 
+0000ce30: 6669 6c65 7320 6c69 7374 2229 0a0a 2020  files list")..  
+0000ce40: 2020 2020 2020 6974 656d 7320 3d20 7a73        items = zs
+0000ce50: 2e72 6570 6c61 6365 2822 5c72 222c 2022  .replace("\r", "
+0000ce60: 2229 2e73 706c 6974 2822 5c6e 2229 0a20  ").split("\n"). 
+0000ce70: 2020 2020 2020 2069 7465 6d73 203d 205b         items = [
+0000ce80: 756e 7175 6f74 6570 2878 2920 666f 7220  unquotep(x) for 
+0000ce90: 7820 696e 2069 7465 6d73 2069 6620 6974  x in items if it
+0000cea0: 656d 735d 0a0a 2020 2020 2020 2020 7365  ems]..        se
+0000ceb0: 6c66 2e70 6172 7365 722e 6472 6f70 2829  lf.parser.drop()
+0000cec0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000ced0: 7365 6c66 2e74 785f 7a69 7028 6b2c 2076  self.tx_zip(k, v
+0000cee0: 2c20 766e 2c20 7265 6d2c 2069 7465 6d73  , vn, rem, items
+0000cef0: 2c20 7365 6c66 2e61 7267 732e 6564 290a  , self.args.ed).
+0000cf00: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
+0000cf10: 706f 7374 5f6a 736f 6e28 7365 6c66 2920  post_json(self) 
+0000cf20: 203a 0a20 2020 2020 2020 2074 7279 3a0a   :.        try:.
+0000cf30: 2020 2020 2020 2020 2020 2020 7265 6d61              rema
+0000cf40: 696e 7320 3d20 696e 7428 7365 6c66 2e68  ins = int(self.h
+0000cf50: 6561 6465 7273 5b22 636f 6e74 656e 742d  eaders["content-
+0000cf60: 6c65 6e67 7468 225d 290a 2020 2020 2020  length"]).      
+0000cf70: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+0000cf80: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
+0000cf90: 6163 2834 3131 290a 0a20 2020 2020 2020  ac(411)..       
+0000cfa0: 2069 6620 7265 6d61 696e 7320 3e20 3130   if remains > 10
+0000cfb0: 3234 202a 2031 3032 343a 0a20 2020 2020  24 * 1024:.     
+0000cfc0: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
+0000cfd0: 6b61 6328 3431 332c 2022 6a73 6f6e 2032  kac(413, "json 2
+0000cfe0: 6269 6722 290a 0a20 2020 2020 2020 2065  big")..        e
+0000cff0: 6e63 203d 2022 7574 662d 3822 0a20 2020  nc = "utf-8".   
+0000d000: 2020 2020 2063 7479 7065 203d 2073 656c       ctype = sel
+0000d010: 662e 6865 6164 6572 732e 6765 7428 2263  f.headers.get("c
+0000d020: 6f6e 7465 6e74 2d74 7970 6522 2c20 2222  ontent-type", ""
+0000d030: 292e 6c6f 7765 7228 290a 2020 2020 2020  ).lower().      
+0000d040: 2020 6966 2022 6368 6172 7365 7422 2069    if "charset" i
+0000d050: 6e20 6374 7970 653a 0a20 2020 2020 2020  n ctype:.       
+0000d060: 2020 2020 2065 6e63 203d 2063 7479 7065       enc = ctype
+0000d070: 2e73 706c 6974 2822 6368 6172 7365 7422  .split("charset"
+0000d080: 295b 315d 2e73 7472 6970 2822 203d 2229  )[1].strip(" =")
+0000d090: 2e73 706c 6974 2822 3b22 295b 305d 2e73  .split(";")[0].s
+0000d0a0: 7472 6970 2829 0a0a 2020 2020 2020 2020  trip()..        
+0000d0b0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000d0c0: 206a 736f 6e5f 6275 6620 3d20 7365 6c66   json_buf = self
+0000d0d0: 2e73 722e 7265 6376 5f65 7828 7265 6d61  .sr.recv_ex(rema
+0000d0e0: 696e 7329 0a20 2020 2020 2020 2065 7863  ins).        exc
+0000d0f0: 6570 7420 556e 7265 6376 454f 463a 0a20  ept UnrecvEOF:. 
+0000d100: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000d110: 2050 6562 6b61 6328 3432 322c 2022 636c   Pebkac(422, "cl
+0000d120: 6965 6e74 2064 6973 636f 6e6e 6563 7465  ient disconnecte
+0000d130: 6420 7768 696c 6520 706f 7374 696e 6720  d while posting 
+0000d140: 4a53 4f4e 2229 0a0a 2020 2020 2020 2020  JSON")..        
+0000d150: 7365 6c66 2e6c 6f67 2822 6465 636f 6469  self.log("decodi
+0000d160: 6e67 207b 7d20 6279 7465 7320 6f66 207b  ng {} bytes of {
+0000d170: 7d20 6a73 6f6e 222e 666f 726d 6174 286c  } json".format(l
+0000d180: 656e 286a 736f 6e5f 6275 6629 2c20 656e  en(json_buf), en
+0000d190: 6329 290a 2020 2020 2020 2020 7472 793a  c)).        try:
+0000d1a0: 0a20 2020 2020 2020 2020 2020 2062 6f64  .            bod
+0000d1b0: 7920 3d20 6a73 6f6e 2e6c 6f61 6473 286a  y = json.loads(j
+0000d1c0: 736f 6e5f 6275 662e 6465 636f 6465 2865  son_buf.decode(e
+0000d1d0: 6e63 2c20 2272 6570 6c61 6365 2229 290a  nc, "replace")).
+0000d1e0: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
+0000d1f0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000d200: 6520 5065 626b 6163 2834 3232 2c20 2279  e Pebkac(422, "y
+0000d210: 6f75 2050 4f53 5465 6420 696e 7661 6c69  ou POSTed invali
+0000d220: 6420 6a73 6f6e 2229 0a0a 2020 2020 2020  d json")..      
+0000d230: 2020 2320 7365 6c66 2e72 6570 6c79 2862    # self.reply(b
+0000d240: 2263 6c6f 7564 666c 6172 6522 2c20 3530  "cloudflare", 50
+0000d250: 3329 0a20 2020 2020 2020 2023 2072 6574  3).        # ret
+0000d260: 7572 6e20 5472 7565 0a0a 2020 2020 2020  urn True..      
+0000d270: 2020 6966 2022 7372 6368 2220 696e 2073    if "srch" in s
+0000d280: 656c 662e 7570 6172 616d 206f 7220 2273  elf.uparam or "s
+0000d290: 7263 6822 2069 6e20 626f 6479 3a0a 2020  rch" in body:.  
+0000d2a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000d2b0: 2073 656c 662e 6861 6e64 6c65 5f73 6561   self.handle_sea
+0000d2c0: 7263 6828 626f 6479 290a 0a20 2020 2020  rch(body)..     
+0000d2d0: 2020 2069 6620 2264 656c 6574 6522 2069     if "delete" i
+0000d2e0: 6e20 7365 6c66 2e75 7061 7261 6d3a 0a20  n self.uparam:. 
+0000d2f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000d300: 6e20 7365 6c66 2e68 616e 646c 655f 726d  n self.handle_rm
+0000d310: 2862 6f64 7929 0a0a 2020 2020 2020 2020  (body)..        
+0000d320: 6e61 6d65 203d 2075 6e64 6f74 2862 6f64  name = undot(bod
+0000d330: 795b 226e 616d 6522 5d29 0a20 2020 2020  y["name"]).     
+0000d340: 2020 2069 6620 222f 2220 696e 206e 616d     if "/" in nam
+0000d350: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000d360: 6169 7365 2050 6562 6b61 6328 3430 302c  aise Pebkac(400,
+0000d370: 2022 796f 7572 2063 6c69 656e 7420 6973   "your client is
+0000d380: 206f 6c64 3b20 7072 6573 7320 4354 524c   old; press CTRL
+0000d390: 2d53 4849 4654 2d52 2061 6e64 2074 7279  -SHIFT-R and try
+0000d3a0: 2061 6761 696e 2229 0a0a 2020 2020 2020   again")..      
+0000d3b0: 2020 7666 732c 2072 656d 203d 2073 656c    vfs, rem = sel
+0000d3c0: 662e 6173 7276 2e76 6673 2e67 6574 2873  f.asrv.vfs.get(s
+0000d3d0: 656c 662e 7670 6174 682c 2073 656c 662e  elf.vpath, self.
+0000d3e0: 756e 616d 652c 2046 616c 7365 2c20 5472  uname, False, Tr
+0000d3f0: 7565 290a 2020 2020 2020 2020 6462 762c  ue).        dbv,
+0000d400: 2076 7265 6d20 3d20 7666 732e 6765 745f   vrem = vfs.get_
+0000d410: 6462 7628 7265 6d29 0a0a 2020 2020 2020  dbv(rem)..      
+0000d420: 2020 626f 6479 5b22 7674 6f70 225d 203d    body["vtop"] =
+0000d430: 2064 6276 2e76 7061 7468 0a20 2020 2020   dbv.vpath.     
+0000d440: 2020 2062 6f64 795b 2270 746f 7022 5d20     body["ptop"] 
+0000d450: 3d20 6462 762e 7265 616c 7061 7468 0a20  = dbv.realpath. 
+0000d460: 2020 2020 2020 2062 6f64 795b 2270 7265         body["pre
+0000d470: 6c22 5d20 3d20 7672 656d 0a20 2020 2020  l"] = vrem.     
+0000d480: 2020 2062 6f64 795b 2268 6f73 7422 5d20     body["host"] 
+0000d490: 3d20 7365 6c66 2e68 6f73 740a 2020 2020  = self.host.    
+0000d4a0: 2020 2020 626f 6479 5b22 7573 6572 225d      body["user"]
+0000d4b0: 203d 2073 656c 662e 756e 616d 650a 2020   = self.uname.  
+0000d4c0: 2020 2020 2020 626f 6479 5b22 6164 6472        body["addr
+0000d4d0: 225d 203d 2073 656c 662e 6970 0a20 2020  "] = self.ip.   
+0000d4e0: 2020 2020 2062 6f64 795b 2276 6366 6722       body["vcfg"
+0000d4f0: 5d20 3d20 6462 762e 666c 6167 730a 0a20  ] = dbv.flags.. 
+0000d500: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000d510: 6c66 2e63 616e 5f64 656c 6574 653a 0a20  lf.can_delete:. 
+0000d520: 2020 2020 2020 2020 2020 2062 6f64 792e             body.
+0000d530: 706f 7028 2272 6570 6c61 6365 222c 204e  pop("replace", N
+0000d540: 6f6e 6529 0a0a 2020 2020 2020 2020 6966  one)..        if
+0000d550: 2072 656d 3a0a 2020 2020 2020 2020 2020   rem:.          
+0000d560: 2020 6473 7420 3d20 7666 732e 6361 6e6f    dst = vfs.cano
+0000d570: 6e69 6361 6c28 7265 6d29 0a20 2020 2020  nical(rem).     
+0000d580: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000d590: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000d5a0: 6f74 2062 6f73 2e70 6174 682e 6973 6469  ot bos.path.isdi
+0000d5b0: 7228 6473 7429 3a0a 2020 2020 2020 2020  r(dst):.        
+0000d5c0: 2020 2020 2020 2020 2020 2020 626f 732e              bos.
+0000d5d0: 6d61 6b65 6469 7273 2864 7374 290a 2020  makedirs(dst).  
+0000d5e0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0000d5f0: 204f 5345 7272 6f72 2061 7320 6578 3a0a   OSError as ex:.
+0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d610: 7365 6c66 2e6c 6f67 2822 6d61 6b65 6469  self.log("makedi
+0000d620: 7273 2066 6169 6c65 6420 5b7b 7d5d 222e  rs failed [{}]".
+0000d630: 666f 726d 6174 2864 7374 2929 0a20 2020  format(dst)).   
+0000d640: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d650: 6e6f 7420 626f 732e 7061 7468 2e69 7364  not bos.path.isd
+0000d660: 6972 2864 7374 293a 0a20 2020 2020 2020  ir(dst):.       
+0000d670: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d680: 6578 2e65 7272 6e6f 203d 3d20 6572 726e  ex.errno == errn
+0000d690: 6f2e 4541 4343 4553 3a0a 2020 2020 2020  o.EACCES:.      
 0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6b0: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
-0000d6c0: 6163 2835 3030 2c20 2274 6865 2073 6572  ac(500, "the ser
-0000d6d0: 7665 7220 4f53 2064 656e 6965 6420 7772  ver OS denied wr
-0000d6e0: 6974 652d 6163 6365 7373 2229 0a0a 2020  ite-access")..  
-0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d700: 2020 6966 2065 782e 6572 726e 6f20 3d3d    if ex.errno ==
-0000d710: 2065 7272 6e6f 2e45 4558 4953 543a 0a20   errno.EEXIST:. 
+0000d6b0: 2020 7261 6973 6520 5065 626b 6163 2835    raise Pebkac(5
+0000d6c0: 3030 2c20 2274 6865 2073 6572 7665 7220  00, "the server 
+0000d6d0: 4f53 2064 656e 6965 6420 7772 6974 652d  OS denied write-
+0000d6e0: 6163 6365 7373 2229 0a0a 2020 2020 2020  access")..      
+0000d6f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000d700: 2065 782e 6572 726e 6f20 3d3d 2065 7272   ex.errno == err
+0000d710: 6e6f 2e45 4558 4953 543a 0a20 2020 2020  no.EEXIST:.     
 0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d730: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
-0000d740: 6b61 6328 3430 302c 2022 736f 6d65 2066  kac(400, "some f
-0000d750: 696c 6520 676f 7420 796f 7572 2066 6f6c  ile got your fol
-0000d760: 6465 7220 6e61 6d65 2229 0a0a 2020 2020  der name")..    
-0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d780: 7261 6973 6520 5065 626b 6163 2835 3030  raise Pebkac(500
-0000d790: 2c20 6d69 6e5f 6578 2829 290a 2020 2020  , min_ex()).    
-0000d7a0: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-0000d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7c0: 7261 6973 6520 5065 626b 6163 2835 3030  raise Pebkac(500
-0000d7d0: 2c20 6d69 6e5f 6578 2829 290a 0a20 2020  , min_ex())..   
-0000d7e0: 2020 2020 2078 203d 2073 656c 662e 636f       x = self.co
-0000d7f0: 6e6e 2e68 7372 762e 6272 6f6b 6572 2e61  nn.hsrv.broker.a
-0000d800: 736b 2822 7570 326b 2e68 616e 646c 655f  sk("up2k.handle_
-0000d810: 6a73 6f6e 222c 2062 6f64 792c 2073 656c  json", body, sel
-0000d820: 662e 7532 6668 2e61 7073 290a 2020 2020  f.u2fh.aps).    
-0000d830: 2020 2020 7265 7420 3d20 782e 6765 7428      ret = x.get(
-0000d840: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000d850: 662e 6973 5f76 7072 6f78 6965 643a 0a20  f.is_vproxied:. 
-0000d860: 2020 2020 2020 2020 2020 2069 6620 2270             if "p
-0000d870: 7572 6c22 2069 6e20 7265 743a 0a20 2020  url" in ret:.   
-0000d880: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000d890: 5b22 7075 726c 225d 203d 2073 656c 662e  ["purl"] = self.
-0000d8a0: 6172 6773 2e53 5220 2b20 7265 745b 2270  args.SR + ret["p
-0000d8b0: 7572 6c22 5d0a 0a20 2020 2020 2020 2072  url"]..        r
-0000d8c0: 6574 203d 206a 736f 6e2e 6475 6d70 7328  et = json.dumps(
-0000d8d0: 7265 7429 0a20 2020 2020 2020 2073 656c  ret).        sel
-0000d8e0: 662e 6c6f 6728 7265 7429 0a20 2020 2020  f.log(ret).     
-0000d8f0: 2020 2073 656c 662e 7265 706c 7928 7265     self.reply(re
-0000d900: 742e 656e 636f 6465 2822 7574 662d 3822  t.encode("utf-8"
-0000d910: 292c 206d 696d 653d 2261 7070 6c69 6361  ), mime="applica
-0000d920: 7469 6f6e 2f6a 736f 6e22 290a 2020 2020  tion/json").    
-0000d930: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-0000d940: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
-0000d950: 7365 6172 6368 2873 656c 662c 2062 6f64  search(self, bod
-0000d960: 7920 2029 2020 3a0a 2020 2020 2020 2020  y  )  :.        
-0000d970: 6964 7820 3d20 7365 6c66 2e63 6f6e 6e2e  idx = self.conn.
-0000d980: 6765 745f 7532 6964 7828 290a 2020 2020  get_u2idx().    
-0000d990: 2020 2020 6966 206e 6f74 2068 6173 6174      if not hasat
-0000d9a0: 7472 2869 6478 2c20 2270 5f65 6e64 2229  tr(idx, "p_end")
-0000d9b0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000d9c0: 6973 6520 5065 626b 6163 2835 3030 2c20  ise Pebkac(500, 
-0000d9d0: 2273 716c 6974 6533 2069 7320 6e6f 7420  "sqlite3 is not 
-0000d9e0: 6176 6169 6c61 626c 6520 6f6e 2074 6865  available on the
-0000d9f0: 2073 6572 7665 723b 2063 616e 6e6f 7420   server; cannot 
-0000da00: 7365 6172 6368 2229 0a0a 2020 2020 2020  search")..      
-0000da10: 2020 766f 6c73 203d 205b 5d0a 2020 2020    vols = [].    
-0000da20: 2020 2020 7365 656e 203d 207b 7d0a 2020      seen = {}.  
-0000da30: 2020 2020 2020 666f 7220 7674 6f70 2069        for vtop i
-0000da40: 6e20 7365 6c66 2e72 766f 6c3a 0a20 2020  n self.rvol:.   
-0000da50: 2020 2020 2020 2020 2076 6673 2c20 5f20           vfs, _ 
-0000da60: 3d20 7365 6c66 2e61 7372 762e 7666 732e  = self.asrv.vfs.
-0000da70: 6765 7428 7674 6f70 2c20 7365 6c66 2e75  get(vtop, self.u
-0000da80: 6e61 6d65 2c20 5472 7565 2c20 4661 6c73  name, True, Fals
-0000da90: 6529 0a20 2020 2020 2020 2020 2020 2076  e).            v
-0000daa0: 6673 203d 2076 6673 2e64 6276 206f 7220  fs = vfs.dbv or 
-0000dab0: 7666 730a 2020 2020 2020 2020 2020 2020  vfs.            
-0000dac0: 6966 2076 6673 2069 6e20 7365 656e 3a0a  if vfs in seen:.
-0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dae0: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
-0000daf0: 2020 2020 2020 7365 656e 5b76 6673 5d20        seen[vfs] 
-0000db00: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-0000db10: 2020 2076 6f6c 732e 6170 7065 6e64 2828     vols.append((
-0000db20: 7666 732e 7670 6174 682c 2076 6673 2e72  vfs.vpath, vfs.r
-0000db30: 6561 6c70 6174 682c 2076 6673 2e66 6c61  ealpath, vfs.fla
-0000db40: 6773 2929 0a0a 2020 2020 2020 2020 7430  gs))..        t0
-0000db50: 203d 2074 696d 652e 7469 6d65 2829 0a20   = time.time(). 
-0000db60: 2020 2020 2020 2069 6620 6964 782e 705f         if idx.p_
-0000db70: 656e 643a 0a20 2020 2020 2020 2020 2020  end:.           
-0000db80: 2070 656e 616c 7479 203d 2030 2e37 0a20   penalty = 0.7. 
-0000db90: 2020 2020 2020 2020 2020 2074 5f69 646c             t_idl
-0000dba0: 6520 3d20 7430 202d 2069 6478 2e70 5f65  e = t0 - idx.p_e
-0000dbb0: 6e64 0a20 2020 2020 2020 2020 2020 2069  nd.            i
-0000dbc0: 6620 6964 782e 705f 6475 7220 3e20 302e  f idx.p_dur > 0.
-0000dbd0: 3720 616e 6420 745f 6964 6c65 203c 2070  7 and t_idle < p
-0000dbe0: 656e 616c 7479 3a0a 2020 2020 2020 2020  enalty:.        
-0000dbf0: 2020 2020 2020 2020 7420 3d20 2272 6174          t = "rat
-0000dc00: 652d 6c69 6d69 7420 7b3a 2e31 667d 2073  e-limit {:.1f} s
-0000dc10: 6563 2c20 636f 7374 207b 3a2e 3266 7d2c  ec, cost {:.2f},
-0000dc20: 2069 646c 6520 7b3a 2e32 667d 220a 2020   idle {:.2f}".  
-0000dc30: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000dc40: 6973 6520 5065 626b 6163 2834 3239 2c20  ise Pebkac(429, 
-0000dc50: 742e 666f 726d 6174 2870 656e 616c 7479  t.format(penalty
-0000dc60: 2c20 6964 782e 705f 6475 722c 2074 5f69  , idx.p_dur, t_i
-0000dc70: 646c 6529 290a 0a20 2020 2020 2020 2069  dle))..        i
-0000dc80: 6620 2273 7263 6822 2069 6e20 626f 6479  f "srch" in body
-0000dc90: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000dca0: 7365 6172 6368 2062 7920 7570 326b 2068  search by up2k h
-0000dcb0: 6173 686c 6973 740a 2020 2020 2020 2020  ashlist.        
-0000dcc0: 2020 2020 7662 6f64 7920 3d20 636f 7079      vbody = copy
-0000dcd0: 2e64 6565 7063 6f70 7928 626f 6479 290a  .deepcopy(body).
-0000dce0: 2020 2020 2020 2020 2020 2020 7662 6f64              vbod
-0000dcf0: 795b 2268 6173 6822 5d20 3d20 6c65 6e28  y["hash"] = len(
-0000dd00: 7662 6f64 795b 2268 6173 6822 5d29 0a20  vbody["hash"]). 
-0000dd10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000dd20: 6c6f 6728 2271 6a3a 2022 202b 2072 6570  log("qj: " + rep
-0000dd30: 7228 7662 6f64 7929 290a 2020 2020 2020  r(vbody)).      
-0000dd40: 2020 2020 2020 6869 7473 203d 2069 6478        hits = idx
-0000dd50: 2e66 7365 6172 6368 2876 6f6c 732c 2062  .fsearch(vols, b
-0000dd60: 6f64 7929 0a20 2020 2020 2020 2020 2020  ody).           
-0000dd70: 206d 7367 2020 3d20 7265 7072 2868 6974   msg  = repr(hit
-0000dd80: 7329 0a20 2020 2020 2020 2020 2020 2074  s).            t
-0000dd90: 6167 6c69 7374 2020 3d20 5b5d 0a20 2020  aglist  = [].   
-0000dda0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000ddb0: 2020 2020 2020 2023 2073 6561 7263 6820         # search 
-0000ddc0: 6279 2071 7565 7279 2070 6172 616d 730a  by query params.
-0000ddd0: 2020 2020 2020 2020 2020 2020 7120 3d20              q = 
-0000dde0: 626f 6479 5b22 7122 5d0a 2020 2020 2020  body["q"].      
-0000ddf0: 2020 2020 2020 6e20 3d20 626f 6479 2e67        n = body.g
-0000de00: 6574 2822 6e22 2c20 7365 6c66 2e61 7267  et("n", self.arg
-0000de10: 732e 7372 6368 5f68 6974 7329 0a20 2020  s.srch_hits).   
-0000de20: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-0000de30: 6728 2271 6a3a 207b 7d20 7c7b 7d7c 222e  g("qj: {} |{}|".
-0000de40: 666f 726d 6174 2871 2c20 6e29 290a 2020  format(q, n)).  
-0000de50: 2020 2020 2020 2020 2020 6869 7473 2c20            hits, 
-0000de60: 7461 676c 6973 7420 3d20 6964 782e 7365  taglist = idx.se
-0000de70: 6172 6368 2876 6f6c 732c 2071 2c20 6e29  arch(vols, q, n)
-0000de80: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-0000de90: 203d 206c 656e 2868 6974 7329 0a0a 2020   = len(hits)..  
-0000dea0: 2020 2020 2020 6964 782e 705f 656e 6420        idx.p_end 
-0000deb0: 3d20 7469 6d65 2e74 696d 6528 290a 2020  = time.time().  
-0000dec0: 2020 2020 2020 6964 782e 705f 6475 7220        idx.p_dur 
-0000ded0: 3d20 6964 782e 705f 656e 6420 2d20 7430  = idx.p_end - t0
-0000dee0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
-0000def0: 6728 2271 233a 207b 7d20 287b 3a2e 3266  g("q#: {} ({:.2f
-0000df00: 7d73 2922 2e66 6f72 6d61 7428 6d73 672c  }s)".format(msg,
-0000df10: 2069 6478 2e70 5f64 7572 2929 0a0a 2020   idx.p_dur))..  
-0000df20: 2020 2020 2020 6f72 6465 7220 3d20 5b5d        order = []
-0000df30: 0a20 2020 2020 2020 2063 6667 203d 2073  .        cfg = s
-0000df40: 656c 662e 6172 6773 2e6d 7465 2e73 706c  elf.args.mte.spl
-0000df50: 6974 2822 2c22 290a 2020 2020 2020 2020  it(",").        
-0000df60: 666f 7220 7420 696e 2063 6667 3a0a 2020  for t in cfg:.  
-0000df70: 2020 2020 2020 2020 2020 6966 2074 2069            if t i
-0000df80: 6e20 7461 676c 6973 743a 0a20 2020 2020  n taglist:.     
-0000df90: 2020 2020 2020 2020 2020 206f 7264 6572             order
-0000dfa0: 2e61 7070 656e 6428 7429 0a20 2020 2020  .append(t).     
-0000dfb0: 2020 2066 6f72 2074 2069 6e20 7461 676c     for t in tagl
-0000dfc0: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
-0000dfd0: 2069 6620 7420 6e6f 7420 696e 206f 7264   if t not in ord
-0000dfe0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-0000dff0: 2020 2020 6f72 6465 722e 6170 7065 6e64      order.append
-0000e000: 2874 290a 0a20 2020 2020 2020 2069 6620  (t)..        if 
-0000e010: 7365 6c66 2e69 735f 7670 726f 7869 6564  self.is_vproxied
-0000e020: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0000e030: 7220 6869 7420 696e 2068 6974 733a 0a20  r hit in hits:. 
-0000e040: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0000e050: 6974 5b22 7270 225d 203d 2073 656c 662e  it["rp"] = self.
-0000e060: 6172 6773 2e52 5320 2b20 6869 745b 2272  args.RS + hit["r
-0000e070: 7022 5d0a 0a20 2020 2020 2020 2072 203d  p"]..        r =
-0000e080: 206a 736f 6e2e 6475 6d70 7328 7b22 6869   json.dumps({"hi
-0000e090: 7473 223a 2068 6974 732c 2022 7461 675f  ts": hits, "tag_
-0000e0a0: 6f72 6465 7222 3a20 6f72 6465 727d 292e  order": order}).
-0000e0b0: 656e 636f 6465 2822 7574 662d 3822 290a  encode("utf-8").
-0000e0c0: 2020 2020 2020 2020 7365 6c66 2e72 6570          self.rep
-0000e0d0: 6c79 2872 2c20 6d69 6d65 3d22 6170 706c  ly(r, mime="appl
-0000e0e0: 6963 6174 696f 6e2f 6a73 6f6e 2229 0a20  ication/json"). 
-0000e0f0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000e100: 7565 0a0a 2020 2020 6465 6620 6861 6e64  ue..    def hand
-0000e110: 6c65 5f70 6f73 745f 6269 6e61 7279 2873  le_post_binary(s
-0000e120: 656c 6629 2020 3a0a 2020 2020 2020 2020  elf)  :.        
-0000e130: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000e140: 2072 656d 6169 6e73 203d 2069 6e74 2873   remains = int(s
-0000e150: 656c 662e 6865 6164 6572 735b 2263 6f6e  elf.headers["con
-0000e160: 7465 6e74 2d6c 656e 6774 6822 5d29 0a20  tent-length"]). 
-0000e170: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
-0000e180: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000e190: 2050 6562 6b61 6328 3430 302c 2022 796f   Pebkac(400, "yo
-0000e1a0: 7520 6d75 7374 2073 7570 706c 7920 6120  u must supply a 
-0000e1b0: 636f 6e74 656e 742d 6c65 6e67 7468 2066  content-length f
-0000e1c0: 6f72 2062 696e 6172 7920 504f 5354 2229  or binary POST")
-0000e1d0: 0a0a 2020 2020 2020 2020 7472 793a 0a20  ..        try:. 
-0000e1e0: 2020 2020 2020 2020 2020 2063 6861 7368             chash
-0000e1f0: 203d 2073 656c 662e 6865 6164 6572 735b   = self.headers[
-0000e200: 2278 2d75 7032 6b2d 6861 7368 225d 0a20  "x-up2k-hash"]. 
-0000e210: 2020 2020 2020 2020 2020 2077 6172 6b20             wark 
-0000e220: 3d20 7365 6c66 2e68 6561 6465 7273 5b22  = self.headers["
-0000e230: 782d 7570 326b 2d77 6172 6b22 5d0a 2020  x-up2k-wark"].  
-0000e240: 2020 2020 2020 6578 6365 7074 204b 6579        except Key
-0000e250: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-0000e260: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
-0000e270: 3430 302c 2022 6e65 6564 2068 6173 6820  400, "need hash 
-0000e280: 616e 6420 7761 726b 2068 6561 6465 7273  and wark headers
-0000e290: 2066 6f72 2062 696e 6172 7920 504f 5354   for binary POST
-0000e2a0: 2229 0a0a 2020 2020 2020 2020 7666 732c  ")..        vfs,
-0000e2b0: 205f 203d 2073 656c 662e 6173 7276 2e76   _ = self.asrv.v
-0000e2c0: 6673 2e67 6574 2873 656c 662e 7670 6174  fs.get(self.vpat
-0000e2d0: 682c 2073 656c 662e 756e 616d 652c 2046  h, self.uname, F
-0000e2e0: 616c 7365 2c20 5472 7565 290a 2020 2020  alse, True).    
-0000e2f0: 2020 2020 7074 6f70 203d 2028 7666 732e      ptop = (vfs.
-0000e300: 6462 7620 6f72 2076 6673 292e 7265 616c  dbv or vfs).real
-0000e310: 7061 7468 0a0a 2020 2020 2020 2020 7820  path..        x 
-0000e320: 3d20 7365 6c66 2e63 6f6e 6e2e 6873 7276  = self.conn.hsrv
-0000e330: 2e62 726f 6b65 722e 6173 6b28 2275 7032  .broker.ask("up2
-0000e340: 6b2e 6861 6e64 6c65 5f63 6875 6e6b 222c  k.handle_chunk",
-0000e350: 2070 746f 702c 2077 6172 6b2c 2063 6861   ptop, wark, cha
-0000e360: 7368 290a 2020 2020 2020 2020 7265 7370  sh).        resp
-0000e370: 6f6e 7365 203d 2078 2e67 6574 2829 0a20  onse = x.get(). 
-0000e380: 2020 2020 2020 2063 6875 6e6b 7369 7a65         chunksize
-0000e390: 2c20 6373 7461 7274 2c20 7061 7468 2c20  , cstart, path, 
-0000e3a0: 6c61 7374 6d6f 642c 2073 7072 7320 3d20  lastmod, sprs = 
-0000e3b0: 7265 7370 6f6e 7365 0a0a 2020 2020 2020  response..      
-0000e3c0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0000e3d0: 2020 2069 6620 7365 6c66 2e61 7267 732e     if self.args.
-0000e3e0: 6e77 3a0a 2020 2020 2020 2020 2020 2020  nw:.            
-0000e3f0: 2020 2020 7061 7468 203d 206f 732e 6465      path = os.de
-0000e400: 766e 756c 6c0a 0a20 2020 2020 2020 2020  vnull..         
-0000e410: 2020 2069 6620 7265 6d61 696e 7320 3e20     if remains > 
-0000e420: 6368 756e 6b73 697a 653a 0a20 2020 2020  chunksize:.     
-0000e430: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000e440: 2050 6562 6b61 6328 3430 302c 2022 796f   Pebkac(400, "yo
-0000e450: 7572 2063 6875 6e6b 2069 7320 746f 6f20  ur chunk is too 
-0000e460: 6269 6720 746f 2066 6974 2229 0a0a 2020  big to fit")..  
-0000e470: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-0000e480: 6f67 2822 7772 6974 696e 6720 7b7d 2023  og("writing {} #
-0000e490: 7b7d 2040 7b7d 206c 656e 207b 7d22 2e66  {} @{} len {}".f
-0000e4a0: 6f72 6d61 7428 7061 7468 2c20 6368 6173  ormat(path, chas
-0000e4b0: 682c 2063 7374 6172 742c 2072 656d 6169  h, cstart, remai
-0000e4c0: 6e73 2929 0a0a 2020 2020 2020 2020 2020  ns))..          
-0000e4d0: 2020 7265 6164 6572 203d 2072 6561 645f    reader = read_
-0000e4e0: 736f 636b 6574 2873 656c 662e 7372 2c20  socket(self.sr, 
-0000e4f0: 7265 6d61 696e 7329 0a0a 2020 2020 2020  remains)..      
-0000e500: 2020 2020 2020 6620 3d20 4e6f 6e65 0a20        f = None. 
-0000e510: 2020 2020 2020 2020 2020 2066 706f 6f6c             fpool
-0000e520: 203d 206e 6f74 2073 656c 662e 6172 6773   = not self.args
-0000e530: 2e6e 6f5f 6670 6f6f 6c20 616e 6420 7370  .no_fpool and sp
-0000e540: 7273 0a20 2020 2020 2020 2020 2020 2069  rs.            i
-0000e550: 6620 6670 6f6f 6c3a 0a20 2020 2020 2020  f fpool:.       
-0000e560: 2020 2020 2020 2020 2077 6974 6820 7365           with se
-0000e570: 6c66 2e6d 7574 6578 3a0a 2020 2020 2020  lf.mutex:.      
-0000e580: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000e590: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000e5a0: 2020 2020 2020 2020 2020 2066 203d 2073             f = s
-0000e5b0: 656c 662e 7532 6668 2e70 6f70 2870 6174  elf.u2fh.pop(pat
-0000e5c0: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
-0000e5d0: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
-0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5f0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-0000e600: 2020 2020 2020 2020 2066 203d 2066 206f           f = f o
-0000e610: 7220 6f70 656e 2866 7365 6e63 2870 6174  r open(fsenc(pat
-0000e620: 6829 2c20 2272 622b 222c 2035 3132 202a  h), "rb+", 512 *
-0000e630: 2031 3032 3429 0a0a 2020 2020 2020 2020   1024)..        
-0000e640: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000e650: 2020 2020 2020 2020 2066 2e73 6565 6b28           f.seek(
-0000e660: 6373 7461 7274 5b30 5d29 0a20 2020 2020  cstart[0]).     
-0000e670: 2020 2020 2020 2020 2020 2070 6f73 745f             post_
-0000e680: 737a 2c20 5f2c 2073 6861 5f62 3634 203d  sz, _, sha_b64 =
-0000e690: 2068 6173 6863 6f70 7928 7265 6164 6572   hashcopy(reader
-0000e6a0: 2c20 662c 2073 656c 662e 6172 6773 2e73  , f, self.args.s
-0000e6b0: 5f77 725f 736c 7029 0a0a 2020 2020 2020  _wr_slp)..      
-0000e6c0: 2020 2020 2020 2020 2020 6966 2073 6861            if sha
-0000e6d0: 5f62 3634 2021 3d20 6368 6173 683a 0a20  _b64 != chash:. 
-0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6f0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e710: 7365 6c66 2e62 616b 666c 6970 2866 2c20  self.bakflip(f, 
-0000e720: 6373 7461 7274 5b30 5d2c 2070 6f73 745f  cstart[0], post_
-0000e730: 737a 2c20 7368 615f 6236 3429 0a20 2020  sz, sha_b64).   
-0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e750: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e770: 2073 656c 662e 6c6f 6728 2262 616b 666c   self.log("bakfl
-0000e780: 6970 2066 6169 6c65 643a 2022 202b 206d  ip failed: " + m
-0000e790: 696e 5f65 7828 2929 0a0a 2020 2020 2020  in_ex())..      
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 7420                t 
-0000e7b0: 3d20 2279 6f75 7220 6368 756e 6b20 676f  = "your chunk go
-0000e7c0: 7420 636f 7272 7570 7465 6420 736f 6d65  t corrupted some
-0000e7d0: 686f 7720 2872 6563 6569 7665 6420 7b7d  how (received {}
-0000e7e0: 2062 7974 6573 293b 2065 7870 6563 7465   bytes); expecte
-0000e7f0: 6420 7673 2072 6563 6569 7665 6420 6861  d vs received ha
-0000e800: 7368 3a5c 6e7b 7d5c 6e7b 7d22 0a20 2020  sh:\n{}\n{}".   
-0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e820: 2072 6169 7365 2050 6562 6b61 6328 3430   raise Pebkac(40
-0000e830: 302c 2074 2e66 6f72 6d61 7428 706f 7374  0, t.format(post
-0000e840: 5f73 7a2c 2063 6861 7368 2c20 7368 615f  _sz, chash, sha_
-0000e850: 6236 3429 290a 0a20 2020 2020 2020 2020  b64))..         
-0000e860: 2020 2020 2020 2069 6620 6c65 6e28 6373         if len(cs
-0000e870: 7461 7274 2920 3e20 3120 616e 6420 7061  tart) > 1 and pa
-0000e880: 7468 2021 3d20 6f73 2e64 6576 6e75 6c6c  th != os.devnull
-0000e890: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e8a0: 2020 2020 2020 7365 6c66 2e6c 6f67 280a        self.log(.
-0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8c0: 2020 2020 2020 2020 2263 6c6f 6e65 207b          "clone {
-0000e8d0: 7d20 746f 207b 7d22 2e66 6f72 6d61 7428  } to {}".format(
-0000e8e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e8f0: 2020 2020 2020 2020 2020 2020 2063 7374               cst
-0000e900: 6172 745b 305d 2c20 2220 2620 222e 6a6f  art[0], " & ".jo
-0000e910: 696e 2875 6e69 636f 6465 2878 2920 666f  in(unicode(x) fo
-0000e920: 7220 7820 696e 2063 7374 6172 745b 313a  r x in cstart[1:
-0000e930: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000e940: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000e950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e960: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000e970: 2020 2020 2020 206f 6673 203d 2030 0a20         ofs = 0. 
-0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e990: 2020 2077 6869 6c65 206f 6673 203c 2063     while ofs < c
-0000e9a0: 6875 6e6b 7369 7a65 3a0a 2020 2020 2020  hunksize:.      
-0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9c0: 2020 6275 6673 7a20 3d20 6d69 6e28 6368    bufsz = min(ch
-0000e9d0: 756e 6b73 697a 6520 2d20 6f66 732c 2034  unksize - ofs, 4
-0000e9e0: 202a 2031 3032 3420 2a20 3130 3234 290a   * 1024 * 1024).
-0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea00: 2020 2020 2020 2020 662e 7365 656b 2863          f.seek(c
-0000ea10: 7374 6172 745b 305d 202b 206f 6673 290a  start[0] + ofs).
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2020 2020 2020 6275 6620 3d20 662e          buf = f.
-0000ea40: 7265 6164 2862 7566 737a 290a 2020 2020  read(bufsz).    
-0000ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea60: 2020 2020 666f 7220 776f 6673 2069 6e20      for wofs in 
-0000ea70: 6373 7461 7274 5b31 3a5d 3a0a 2020 2020  cstart[1:]:.    
-0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea90: 2020 2020 2020 2020 662e 7365 656b 2877          f.seek(w
-0000eaa0: 6f66 7320 2b20 6f66 7329 0a20 2020 2020  ofs + ofs).     
-0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eac0: 2020 2020 2020 2066 2e77 7269 7465 2862         f.write(b
-0000ead0: 7566 290a 0a20 2020 2020 2020 2020 2020  uf)..           
-0000eae0: 2020 2020 2020 2020 2020 2020 206f 6673               ofs
-0000eaf0: 202b 3d20 6c65 6e28 6275 6629 0a0a 2020   += len(buf)..  
-0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb10: 2020 7365 6c66 2e6c 6f67 2822 636c 6f6e    self.log("clon
-0000eb20: 6520 7b7d 2064 6f6e 6522 2e66 6f72 6d61  e {} done".forma
-0000eb30: 7428 6373 7461 7274 5b30 5d29 290a 0a20  t(cstart[0])).. 
-0000eb40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000eb50: 6620 6e6f 7420 6670 6f6f 6c3a 0a20 2020  f not fpool:.   
-0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb70: 2066 2e63 6c6f 7365 2829 0a20 2020 2020   f.close().     
-0000eb80: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000eb90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eba0: 2020 2020 2077 6974 6820 7365 6c66 2e6d       with self.m
-0000ebb0: 7574 6578 3a0a 2020 2020 2020 2020 2020  utex:.          
-0000ebc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ebd0: 6c66 2e75 3266 682e 7075 7428 7061 7468  lf.u2fh.put(path
-0000ebe0: 2c20 6629 0a20 2020 2020 2020 2020 2020  , f).           
-0000ebf0: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-0000ec00: 2020 2020 2020 2020 2023 206d 6179 6265           # maybe
-0000ec10: 2062 7573 7465 6420 6861 6e64 6c65 2028   busted handle (
-0000ec20: 6567 2e20 6469 736b 2077 656e 7420 6675  eg. disk went fu
-0000ec30: 6c6c 290a 2020 2020 2020 2020 2020 2020  ll).            
-0000ec40: 2020 2020 662e 636c 6f73 6528 290a 2020      f.close().  
-0000ec50: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000ec60: 6973 650a 2020 2020 2020 2020 6669 6e61  ise.        fina
-0000ec70: 6c6c 793a 0a20 2020 2020 2020 2020 2020  lly:.           
-0000ec80: 2078 203d 2073 656c 662e 636f 6e6e 2e68   x = self.conn.h
-0000ec90: 7372 762e 6272 6f6b 6572 2e61 736b 2822  srv.broker.ask("
-0000eca0: 7570 326b 2e72 656c 6561 7365 5f63 6875  up2k.release_chu
-0000ecb0: 6e6b 222c 2070 746f 702c 2077 6172 6b2c  nk", ptop, wark,
-0000ecc0: 2063 6861 7368 290a 2020 2020 2020 2020   chash).        
-0000ecd0: 2020 2020 782e 6765 7428 2920 2023 2062      x.get()  # b
-0000ece0: 6c6f 636b 2063 6c69 656e 7420 756e 7469  lock client unti
-0000ecf0: 6c20 7265 6c65 6173 6564 0a0a 2020 2020  l released..    
-0000ed00: 2020 2020 7820 3d20 7365 6c66 2e63 6f6e      x = self.con
-0000ed10: 6e2e 6873 7276 2e62 726f 6b65 722e 6173  n.hsrv.broker.as
-0000ed20: 6b28 2275 7032 6b2e 636f 6e66 6972 6d5f  k("up2k.confirm_
-0000ed30: 6368 756e 6b22 2c20 7074 6f70 2c20 7761  chunk", ptop, wa
-0000ed40: 726b 2c20 6368 6173 6829 0a20 2020 2020  rk, chash).     
-0000ed50: 2020 207a 7469 7320 3d20 782e 6765 7428     ztis = x.get(
-0000ed60: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
-0000ed70: 2020 2020 2020 2020 2020 206e 756d 5f6c             num_l
-0000ed80: 6566 742c 2066 696e 5f70 6174 6820 3d20  eft, fin_path = 
-0000ed90: 7a74 6973 0a20 2020 2020 2020 2065 7863  ztis.        exc
-0000eda0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-0000edb0: 2073 656c 662e 6c6f 7564 5f72 6570 6c79   self.loud_reply
-0000edc0: 287a 7469 732c 2073 7461 7475 733d 3530  (ztis, status=50
-0000edd0: 3029 0a20 2020 2020 2020 2020 2020 2072  0).            r
-0000ede0: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-0000edf0: 2020 2020 2069 6620 6e6f 7420 6e75 6d5f       if not num_
-0000ee00: 6c65 6674 2061 6e64 2066 706f 6f6c 3a0a  left and fpool:.
-0000ee10: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000ee20: 2073 656c 662e 6d75 7465 783a 0a20 2020   self.mutex:.   
-0000ee30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ee40: 662e 7532 6668 2e63 6c6f 7365 2870 6174  f.u2fh.close(pat
-0000ee50: 6829 0a0a 2020 2020 2020 2020 6966 206e  h)..        if n
-0000ee60: 6f74 206e 756d 5f6c 6566 7420 616e 6420  ot num_left and 
-0000ee70: 6e6f 7420 7365 6c66 2e61 7267 732e 6e77  not self.args.nw
-0000ee80: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000ee90: 6c66 2e63 6f6e 6e2e 6873 7276 2e62 726f  lf.conn.hsrv.bro
-0000eea0: 6b65 722e 6173 6b28 0a20 2020 2020 2020  ker.ask(.       
-0000eeb0: 2020 2020 2020 2020 2022 7570 326b 2e66           "up2k.f
-0000eec0: 696e 6973 685f 7570 6c6f 6164 222c 2070  inish_upload", p
-0000eed0: 746f 702c 2077 6172 6b2c 2073 656c 662e  top, wark, self.
-0000eee0: 7532 6668 2e61 7073 0a20 2020 2020 2020  u2fh.aps.       
-0000eef0: 2020 2020 2029 2e67 6574 2829 0a0a 2020       ).get()..  
-0000ef00: 2020 2020 2020 6369 6e66 203d 2073 656c        cinf = sel
-0000ef10: 662e 6865 6164 6572 732e 6765 7428 2278  f.headers.get("x
-0000ef20: 2d75 7032 6b2d 7374 6174 222c 2022 2229  -up2k-stat", "")
-0000ef30: 0a0a 2020 2020 2020 2020 7370 6420 3d20  ..        spd = 
-0000ef40: 7365 6c66 2e5f 7370 6428 706f 7374 5f73  self._spd(post_s
-0000ef50: 7a29 0a20 2020 2020 2020 2073 656c 662e  z).        self.
-0000ef60: 6c6f 6728 227b 3a37 307d 2074 6861 6e6b  log("{:70} thank
-0000ef70: 207b 7d22 2e66 6f72 6d61 7428 7370 642c   {}".format(spd,
-0000ef80: 2063 696e 6629 290a 2020 2020 2020 2020   cinf)).        
-0000ef90: 7365 6c66 2e72 6570 6c79 2862 2274 6861  self.reply(b"tha
-0000efa0: 6e6b 2229 0a20 2020 2020 2020 2072 6574  nk").        ret
-0000efb0: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
-0000efc0: 6620 6861 6e64 6c65 5f6c 6f67 696e 2873  f handle_login(s
-0000efd0: 656c 6629 2020 3a0a 2020 2020 2020 2020  elf)  :.        
-0000efe0: 6173 7365 7274 2073 656c 662e 7061 7273  assert self.pars
-0000eff0: 6572 0a20 2020 2020 2020 2070 7764 203d  er.        pwd =
-0000f000: 2073 656c 662e 7061 7273 6572 2e72 6571   self.parser.req
-0000f010: 7569 7265 2822 6370 7077 6422 2c20 3634  uire("cppwd", 64
-0000f020: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-0000f030: 6172 7365 722e 6472 6f70 2829 0a0a 2020  arser.drop()..  
-0000f040: 2020 2020 2020 7365 6c66 2e6f 7574 5f68        self.out_h
-0000f050: 6561 6465 726c 6973 7420 3d20 5b0a 2020  eaderlist = [.  
-0000f060: 2020 2020 2020 2020 2020 7820 666f 7220            x for 
-0000f070: 7820 696e 2073 656c 662e 6f75 745f 6865  x in self.out_he
-0000f080: 6164 6572 6c69 7374 2069 6620 785b 305d  aderlist if x[0]
-0000f090: 2021 3d20 2253 6574 2d43 6f6f 6b69 6522   != "Set-Cookie"
-0000f0a0: 206f 7220 2263 7070 7722 2021 3d20 785b   or "cppw" != x[
-0000f0b0: 315d 5b3a 345d 0a20 2020 2020 2020 205d  1][:4].        ]
-0000f0c0: 0a0a 2020 2020 2020 2020 6473 7420 3d20  ..        dst = 
-0000f0d0: 7365 6c66 2e61 7267 732e 5352 530a 2020  self.args.SRS.  
-0000f0e0: 2020 2020 2020 6966 2073 656c 662e 7670        if self.vp
-0000f0f0: 6174 683a 0a20 2020 2020 2020 2020 2020  ath:.           
-0000f100: 2064 7374 202b 3d20 7175 6f74 6570 2873   dst += quotep(s
-0000f110: 656c 662e 7670 6174 6829 0a0a 2020 2020  elf.vpath)..    
-0000f120: 2020 2020 6d73 6720 3d20 7365 6c66 2e67      msg = self.g
-0000f130: 6574 5f70 7764 5f63 6f6f 6b69 6528 7077  et_pwd_cookie(pw
-0000f140: 6429 0a20 2020 2020 2020 2068 746d 6c20  d).        html 
-0000f150: 3d20 7365 6c66 2e6a 3273 2822 6d73 6722  = self.j2s("msg"
-0000f160: 2c20 6831 3d6d 7367 2c20 6832 3d27 3c61  , h1=msg, h2='<a
-0000f170: 2068 7265 663d 2227 202b 2064 7374 202b   href="' + dst +
-0000f180: 2027 223e 6163 6b3c 2f61 3e27 2c20 7265   '">ack</a>', re
-0000f190: 6469 723d 6473 7429 0a20 2020 2020 2020  dir=dst).       
-0000f1a0: 2073 656c 662e 7265 706c 7928 6874 6d6c   self.reply(html
-0000f1b0: 2e65 6e63 6f64 6528 2275 7466 2d38 2229  .encode("utf-8")
-0000f1c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000f1d0: 2054 7275 650a 0a20 2020 2064 6566 2067   True..    def g
-0000f1e0: 6574 5f70 7764 5f63 6f6f 6b69 6528 7365  et_pwd_cookie(se
-0000f1f0: 6c66 2c20 7077 6420 2920 203a 0a20 2020  lf, pwd )  :.   
-0000f200: 2020 2020 2069 6620 7077 6420 696e 2073       if pwd in s
-0000f210: 656c 662e 6173 7276 2e69 6163 6374 3a0a  elf.asrv.iacct:.
-0000f220: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-0000f230: 3d20 226c 6f67 696e 206f 6b22 0a20 2020  = "login ok".   
-0000f240: 2020 2020 2020 2020 2064 7572 203d 2069           dur = i
-0000f250: 6e74 2836 3020 2a20 3630 202a 2073 656c  nt(60 * 60 * sel
-0000f260: 662e 6172 6773 2e6c 6f67 6f75 7429 0a20  f.args.logout). 
-0000f270: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000f280: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-0000f290: 6728 2269 6e76 616c 6964 2070 6173 7377  g("invalid passw
-0000f2a0: 6f72 643a 207b 7d22 2e66 6f72 6d61 7428  ord: {}".format(
-0000f2b0: 7077 6429 2c20 3329 0a20 2020 2020 2020  pwd), 3).       
-0000f2c0: 2020 2020 2067 203d 2073 656c 662e 636f       g = self.co
-0000f2d0: 6e6e 2e68 7372 762e 6770 7764 0a20 2020  nn.hsrv.gpwd.   
-0000f2e0: 2020 2020 2020 2020 2069 6620 672e 6c69           if g.li
-0000f2f0: 6d3a 0a20 2020 2020 2020 2020 2020 2020  m:.             
-0000f300: 2020 2062 6f6e 6b2c 2069 7020 3d20 672e     bonk, ip = g.
-0000f310: 626f 6e6b 2873 656c 662e 6970 2c20 7077  bonk(self.ip, pw
-0000f320: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-0000f330: 2020 2069 6620 626f 6e6b 3a0a 2020 2020     if bonk:.    
-0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f350: 7365 6c66 2e6c 6f67 2822 636c 6965 6e74  self.log("client
-0000f360: 2062 616e 6e65 643a 2069 6e76 616c 6964   banned: invalid
-0000f370: 2070 6173 7377 6f72 6473 222c 2031 290a   passwords", 1).
-0000f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f390: 2020 2020 7365 6c66 2e63 6f6e 6e2e 6873      self.conn.hs
-0000f3a0: 7276 2e62 616e 735b 6970 5d20 3d20 626f  rv.bans[ip] = bo
-0000f3b0: 6e6b 0a0a 2020 2020 2020 2020 2020 2020  nk..            
-0000f3c0: 6d73 6720 3d20 226e 6177 2064 7564 6522  msg = "naw dude"
-0000f3d0: 0a20 2020 2020 2020 2020 2020 2070 7764  .            pwd
-0000f3e0: 203d 2022 7822 2020 2320 6e6f 7365 630a   = "x"  # nosec.
-0000f3f0: 2020 2020 2020 2020 2020 2020 6475 7220              dur 
-0000f400: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
-0000f410: 6966 2070 7764 203d 3d20 2278 223a 0a20  if pwd == "x":. 
-0000f420: 2020 2020 2020 2020 2020 2023 2072 6573             # res
-0000f430: 6574 2062 6f74 6820 706c 6169 6e74 6578  et both plaintex
-0000f440: 7420 616e 6420 746c 730a 2020 2020 2020  t and tls.      
-0000f450: 2020 2020 2020 2320 286f 6e6c 7920 6166        # (only af
-0000f460: 6665 6374 7320 6163 7469 7665 2074 6c73  fects active tls
-0000f470: 2063 6f6f 6b69 6573 2077 6865 6e20 746c   cookies when tl
-0000f480: 7329 0a20 2020 2020 2020 2020 2020 2066  s).            f
-0000f490: 6f72 206b 2069 6e20 2822 6370 7077 6422  or k in ("cppwd"
-0000f4a0: 2c20 2263 7070 7773 2229 2069 6620 7365  , "cppws") if se
-0000f4b0: 6c66 2e69 735f 6874 7470 7320 656c 7365  lf.is_https else
-0000f4c0: 2028 2263 7070 7764 222c 293a 0a20 2020   ("cppwd",):.   
-0000f4d0: 2020 2020 2020 2020 2020 2020 2063 6b20               ck 
-0000f4e0: 3d20 6765 6e63 6f6f 6b69 6528 6b2c 2070  = gencookie(k, p
-0000f4f0: 7764 2c20 7365 6c66 2e61 7267 732e 522c  wd, self.args.R,
-0000f500: 2046 616c 7365 2c20 6475 7229 0a20 2020   False, dur).   
-0000f510: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f520: 662e 6f75 745f 6865 6164 6572 6c69 7374  f.out_headerlist
-0000f530: 2e61 7070 656e 6428 2822 5365 742d 436f  .append(("Set-Co
-0000f540: 6f6b 6965 222c 2063 6b29 290a 2020 2020  okie", ck)).    
-0000f550: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000f560: 2020 2020 2020 6b20 3d20 2263 7070 7773        k = "cppws
-0000f570: 2220 6966 2073 656c 662e 6973 5f68 7474  " if self.is_htt
-0000f580: 7073 2065 6c73 6520 2263 7070 7764 220a  ps else "cppwd".
-0000f590: 2020 2020 2020 2020 2020 2020 636b 203d              ck =
-0000f5a0: 2067 656e 636f 6f6b 6965 286b 2c20 7077   gencookie(k, pw
-0000f5b0: 642c 2073 656c 662e 6172 6773 2e52 2c20  d, self.args.R, 
-0000f5c0: 7365 6c66 2e69 735f 6874 7470 732c 2064  self.is_https, d
-0000f5d0: 7572 290a 2020 2020 2020 2020 2020 2020  ur).            
-0000f5e0: 7365 6c66 2e6f 7574 5f68 6561 6465 726c  self.out_headerl
-0000f5f0: 6973 742e 6170 7065 6e64 2828 2253 6574  ist.append(("Set
-0000f600: 2d43 6f6f 6b69 6522 2c20 636b 2929 0a0a  -Cookie", ck))..
-0000f610: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-0000f620: 7367 0a0a 2020 2020 6465 6620 6861 6e64  sg..    def hand
-0000f630: 6c65 5f6d 6b64 6972 2873 656c 6629 2020  le_mkdir(self)  
-0000f640: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
-0000f650: 2073 656c 662e 7061 7273 6572 0a20 2020   self.parser.   
-0000f660: 2020 2020 206e 6577 5f64 6972 203d 2073       new_dir = s
-0000f670: 656c 662e 7061 7273 6572 2e72 6571 7569  elf.parser.requi
-0000f680: 7265 2822 6e61 6d65 222c 2035 3132 290a  re("name", 512).
-0000f690: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
-0000f6a0: 7365 722e 6472 6f70 2829 0a0a 2020 2020  ser.drop()..    
-0000f6b0: 2020 2020 7361 6e69 7469 7a65 6420 3d20      sanitized = 
-0000f6c0: 7361 6e69 7469 7a65 5f66 6e28 6e65 775f  sanitize_fn(new_
-0000f6d0: 6469 722c 2022 222c 205b 5d29 0a20 2020  dir, "", []).   
-0000f6e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000f6f0: 2e5f 6d6b 6469 7228 766a 6f69 6e28 7365  ._mkdir(vjoin(se
-0000f700: 6c66 2e76 7061 7468 2c20 7361 6e69 7469  lf.vpath, saniti
-0000f710: 7a65 6429 290a 0a20 2020 2064 6566 205f  zed))..    def _
-0000f720: 6d6b 6469 7228 7365 6c66 2c20 7670 6174  mkdir(self, vpat
-0000f730: 6820 2920 203a 0a20 2020 2020 2020 206e  h )  :.        n
-0000f740: 756c 6c77 7269 7465 203d 2073 656c 662e  ullwrite = self.
-0000f750: 6172 6773 2e6e 770a 2020 2020 2020 2020  args.nw.        
-0000f760: 7666 732c 2072 656d 203d 2073 656c 662e  vfs, rem = self.
-0000f770: 6173 7276 2e76 6673 2e67 6574 2876 7061  asrv.vfs.get(vpa
-0000f780: 7468 2c20 7365 6c66 2e75 6e61 6d65 2c20  th, self.uname, 
-0000f790: 4661 6c73 652c 2054 7275 6529 0a20 2020  False, True).   
-0000f7a0: 2020 2020 2073 656c 662e 5f61 7373 6572       self._asser
-0000f7b0: 745f 7361 6665 5f72 656d 2872 656d 290a  t_safe_rem(rem).
-0000f7c0: 2020 2020 2020 2020 666e 203d 2076 6673          fn = vfs
-0000f7d0: 2e63 616e 6f6e 6963 616c 2872 656d 290a  .canonical(rem).
-0000f7e0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000f7f0: 6e75 6c6c 7772 6974 653a 0a20 2020 2020  nullwrite:.     
-0000f800: 2020 2020 2020 2066 6469 7220 3d20 6f73         fdir = os
-0000f810: 2e70 6174 682e 6469 726e 616d 6528 666e  .path.dirname(fn
-0000f820: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-0000f830: 6620 6e6f 7420 626f 732e 7061 7468 2e69  f not bos.path.i
-0000f840: 7364 6972 2866 6469 7229 3a0a 2020 2020  sdir(fdir):.    
-0000f850: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000f860: 6520 5065 626b 6163 2834 3039 2c20 2270  e Pebkac(409, "p
-0000f870: 6172 656e 7420 666f 6c64 6572 2064 6f65  arent folder doe
-0000f880: 7320 6e6f 7420 6578 6973 7422 290a 0a20  s not exist").. 
-0000f890: 2020 2020 2020 2020 2020 2069 6620 626f             if bo
-0000f8a0: 732e 7061 7468 2e69 7364 6972 2866 6e29  s.path.isdir(fn)
-0000f8b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f8c0: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
-0000f8d0: 3035 2c20 2274 6861 7420 666f 6c64 6572  05, "that folder
-0000f8e0: 2065 7869 7374 7320 616c 7265 6164 7922   exists already"
-0000f8f0: 290a 0a20 2020 2020 2020 2020 2020 2074  )..            t
-0000f900: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000f910: 2020 2020 626f 732e 6d6b 6469 7228 666e      bos.mkdir(fn
-0000f920: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-0000f930: 6365 7074 204f 5345 7272 6f72 2061 7320  cept OSError as 
-0000f940: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
-0000f950: 2020 2020 6966 2065 782e 6572 726e 6f20      if ex.errno 
-0000f960: 3d3d 2065 7272 6e6f 2e45 4143 4345 533a  == errno.EACCES:
-0000f970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f980: 2020 2020 2072 6169 7365 2050 6562 6b61       raise Pebka
-0000f990: 6328 3530 302c 2022 7468 6520 7365 7276  c(500, "the serv
-0000f9a0: 6572 204f 5320 6465 6e69 6564 2077 7269  er OS denied wri
-0000f9b0: 7465 2d61 6363 6573 7322 290a 0a20 2020  te-access")..   
-0000f9c0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000f9d0: 7365 2050 6562 6b61 6328 3530 302c 2022  se Pebkac(500, "
-0000f9e0: 6d6b 6469 7220 6661 696c 6564 3a5c 6e22  mkdir failed:\n"
-0000f9f0: 202b 206d 696e 5f65 7828 2929 0a20 2020   + min_ex()).   
-0000fa00: 2020 2020 2020 2020 2065 7863 6570 743a           except:
-0000fa10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fa20: 2072 6169 7365 2050 6562 6b61 6328 3530   raise Pebkac(50
-0000fa30: 302c 206d 696e 5f65 7828 2929 0a0a 2020  0, min_ex())..  
-0000fa40: 2020 2020 2020 7365 6c66 2e6f 7574 5f68        self.out_h
-0000fa50: 6561 6465 7273 5b22 582d 4e65 772d 4469  eaders["X-New-Di
-0000fa60: 7222 5d20 3d20 7175 6f74 6570 2876 7061  r"] = quotep(vpa
-0000fa70: 7468 2e73 706c 6974 2822 2f22 295b 2d31  th.split("/")[-1
-0000fa80: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
-0000fa90: 7265 6469 7265 6374 2876 7061 7468 2c20  redirect(vpath, 
-0000faa0: 7374 6174 7573 3d32 3031 290a 2020 2020  status=201).    
-0000fab0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-0000fac0: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
-0000fad0: 6e65 775f 6d64 2873 656c 6629 2020 3a0a  new_md(self)  :.
-0000fae0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-0000faf0: 656c 662e 7061 7273 6572 0a20 2020 2020  elf.parser.     
-0000fb00: 2020 206e 6577 5f66 696c 6520 3d20 7365     new_file = se
-0000fb10: 6c66 2e70 6172 7365 722e 7265 7175 6972  lf.parser.requir
-0000fb20: 6528 226e 616d 6522 2c20 3531 3229 0a20  e("name", 512). 
-0000fb30: 2020 2020 2020 2073 656c 662e 7061 7273         self.pars
-0000fb40: 6572 2e64 726f 7028 290a 0a20 2020 2020  er.drop()..     
-0000fb50: 2020 206e 756c 6c77 7269 7465 203d 2073     nullwrite = s
-0000fb60: 656c 662e 6172 6773 2e6e 770a 2020 2020  elf.args.nw.    
-0000fb70: 2020 2020 7666 732c 2072 656d 203d 2073      vfs, rem = s
-0000fb80: 656c 662e 6173 7276 2e76 6673 2e67 6574  elf.asrv.vfs.get
-0000fb90: 2873 656c 662e 7670 6174 682c 2073 656c  (self.vpath, sel
-0000fba0: 662e 756e 616d 652c 2046 616c 7365 2c20  f.uname, False, 
-0000fbb0: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
-0000fbc0: 6c66 2e5f 6173 7365 7274 5f73 6166 655f  lf._assert_safe_
-0000fbd0: 7265 6d28 7265 6d29 0a0a 2020 2020 2020  rem(rem)..      
-0000fbe0: 2020 6966 206e 6f74 206e 6577 5f66 696c    if not new_fil
-0000fbf0: 652e 656e 6473 7769 7468 2822 2e6d 6422  e.endswith(".md"
-0000fc00: 293a 0a20 2020 2020 2020 2020 2020 206e  ):.            n
-0000fc10: 6577 5f66 696c 6520 2b3d 2022 2e6d 6422  ew_file += ".md"
-0000fc20: 0a0a 2020 2020 2020 2020 7361 6e69 7469  ..        saniti
-0000fc30: 7a65 6420 3d20 7361 6e69 7469 7a65 5f66  zed = sanitize_f
-0000fc40: 6e28 6e65 775f 6669 6c65 2c20 2222 2c20  n(new_file, "", 
-0000fc50: 5b5d 290a 0a20 2020 2020 2020 2069 6620  [])..        if 
-0000fc60: 6e6f 7420 6e75 6c6c 7772 6974 653a 0a20  not nullwrite:. 
-0000fc70: 2020 2020 2020 2020 2020 2066 6469 7220             fdir 
-0000fc80: 3d20 7666 732e 6361 6e6f 6e69 6361 6c28  = vfs.canonical(
-0000fc90: 7265 6d29 0a20 2020 2020 2020 2020 2020  rem).           
-0000fca0: 2066 6e20 3d20 6f73 2e70 6174 682e 6a6f   fn = os.path.jo
-0000fcb0: 696e 2866 6469 722c 2073 616e 6974 697a  in(fdir, sanitiz
-0000fcc0: 6564 290a 0a20 2020 2020 2020 2020 2020  ed)..           
-0000fcd0: 2069 6620 626f 732e 7061 7468 2e65 7869   if bos.path.exi
-0000fce0: 7374 7328 666e 293a 0a20 2020 2020 2020  sts(fn):.       
-0000fcf0: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
-0000fd00: 6562 6b61 6328 3530 302c 2022 7468 6174  ebkac(500, "that
-0000fd10: 2066 696c 6520 6578 6973 7473 2061 6c72   file exists alr
-0000fd20: 6561 6479 2229 0a0a 2020 2020 2020 2020  eady")..        
-0000fd30: 2020 2020 7769 7468 206f 7065 6e28 6673      with open(fs
-0000fd40: 656e 6328 666e 292c 2022 7762 2229 2061  enc(fn), "wb") a
-0000fd50: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
-0000fd60: 2020 2020 2066 2e77 7269 7465 2862 2260       f.write(b"`
-0000fd70: 4752 554e 4e55 5260 5c6e 2229 0a0a 2020  GRUNNUR`\n")..  
-0000fd80: 2020 2020 2020 7670 6174 6820 3d20 227b        vpath = "{
-0000fd90: 7d2f 7b7d 222e 666f 726d 6174 2873 656c  }/{}".format(sel
-0000fda0: 662e 7670 6174 682c 2073 616e 6974 697a  f.vpath, sanitiz
-0000fdb0: 6564 292e 6c73 7472 6970 2822 2f22 290a  ed).lstrip("/").
-0000fdc0: 2020 2020 2020 2020 7365 6c66 2e72 6564          self.red
-0000fdd0: 6972 6563 7428 7670 6174 682c 2022 3f65  irect(vpath, "?e
-0000fde0: 6469 7422 290a 2020 2020 2020 2020 7265  dit").        re
-0000fdf0: 7475 726e 2054 7275 650a 0a20 2020 2064  turn True..    d
-0000fe00: 6566 2075 706c 6f61 645f 666c 6167 7328  ef upload_flags(
-0000fe10: 7365 6c66 2c20 7666 7320 2920 2020 2020  self, vfs )     
-0000fe20: 203a 0a20 2020 2020 2020 2069 6620 7365   :.        if se
-0000fe30: 6c66 2e61 7267 732e 6e77 3a0a 2020 2020  lf.args.nw:.    
-0000fe40: 2020 2020 2020 2020 726e 6420 3d20 300a          rnd = 0.
-0000fe50: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000fe60: 2020 2020 2020 2020 2020 726e 6420 3d20            rnd = 
-0000fe70: 696e 7428 7365 6c66 2e75 7061 7261 6d2e  int(self.uparam.
-0000fe80: 6765 7428 2272 616e 6422 2920 6f72 2073  get("rand") or s
-0000fe90: 656c 662e 6865 6164 6572 732e 6765 7428  elf.headers.get(
-0000fea0: 2272 616e 6422 2920 6f72 2030 290a 2020  "rand") or 0).  
-0000feb0: 2020 2020 2020 2020 2020 6966 2076 6673            if vfs
-0000fec0: 2e66 6c61 6773 2e67 6574 2822 7261 6e64  .flags.get("rand
-0000fed0: 2229 3a20 2023 2066 6f72 6365 2d65 6e61  "):  # force-ena
-0000fee0: 626c 650a 2020 2020 2020 2020 2020 2020  ble.            
-0000fef0: 2020 2020 726e 6420 3d20 6d61 7828 726e      rnd = max(rn
-0000ff00: 642c 2076 6673 2e66 6c61 6773 5b22 6e72  d, vfs.flags["nr
-0000ff10: 616e 6422 5d29 0a0a 2020 2020 2020 2020  and"])..        
-0000ff20: 6163 203d 2073 656c 662e 7570 6172 616d  ac = self.uparam
-0000ff30: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
-0000ff40: 2020 2277 616e 7422 2c20 7365 6c66 2e68    "want", self.h
-0000ff50: 6561 6465 7273 2e67 6574 2822 6163 6365  eaders.get("acce
-0000ff60: 7074 222c 2022 2229 2e6c 6f77 6572 2829  pt", "").lower()
-0000ff70: 2e73 706c 6974 2822 3b22 295b 2d31 5d0a  .split(";")[-1].
-0000ff80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000ff90: 2020 7761 6e74 5f75 726c 203d 2061 6320    want_url = ac 
-0000ffa0: 3d3d 2022 7572 6c22 0a20 2020 2020 2020  == "url".       
-0000ffb0: 207a 7320 3d20 7365 6c66 2e75 7061 7261   zs = self.upara
-0000ffc0: 6d2e 6765 7428 226c 6966 6522 2c20 7365  m.get("life", se
-0000ffd0: 6c66 2e68 6561 6465 7273 2e67 6574 2822  lf.headers.get("
-0000ffe0: 6c69 6665 222c 2022 2229 290a 2020 2020  life", "")).    
-0000fff0: 2020 2020 6966 207a 733a 0a20 2020 2020      if zs:.     
-00010000: 2020 2020 2020 2076 6c69 6665 203d 2076         vlife = v
-00010010: 6673 2e66 6c61 6773 2e67 6574 2822 6c69  fs.flags.get("li
-00010020: 6665 7469 6d65 2229 206f 7220 300a 2020  fetime") or 0.  
-00010030: 2020 2020 2020 2020 2020 6c69 6665 7469            lifeti
-00010040: 6d65 203d 206d 6178 2830 2c20 696e 7428  me = max(0, int(
-00010050: 766c 6966 6520 2d20 696e 7428 7a73 2929  vlife - int(zs))
-00010060: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00010070: 2020 2020 2020 2020 2020 2020 6c69 6665              life
-00010080: 7469 6d65 203d 2030 0a0a 2020 2020 2020  time = 0..      
-00010090: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
-000100a0: 2020 2020 2020 2072 6e64 2c0a 2020 2020         rnd,.    
-000100b0: 2020 2020 2020 2020 7761 6e74 5f75 726c          want_url
-000100c0: 2c0a 2020 2020 2020 2020 2020 2020 6c69  ,.            li
-000100d0: 6665 7469 6d65 2c0a 2020 2020 2020 2020  fetime,.        
-000100e0: 2020 2020 7666 732e 666c 6167 732e 6765      vfs.flags.ge
-000100f0: 7428 2278 6275 2229 206f 7220 5b5d 2c0a  t("xbu") or [],.
-00010100: 2020 2020 2020 2020 2020 2020 7666 732e              vfs.
-00010110: 666c 6167 732e 6765 7428 2278 6175 2229  flags.get("xau")
-00010120: 206f 7220 5b5d 2c0a 2020 2020 2020 2020   or [],.        
-00010130: 290a 0a20 2020 2064 6566 2068 616e 646c  )..    def handl
-00010140: 655f 706c 6169 6e5f 7570 6c6f 6164 2873  e_plain_upload(s
-00010150: 656c 6629 2020 3a0a 2020 2020 2020 2020  elf)  :.        
-00010160: 6173 7365 7274 2073 656c 662e 7061 7273  assert self.pars
-00010170: 6572 0a20 2020 2020 2020 206e 756c 6c77  er.        nullw
-00010180: 7269 7465 203d 2073 656c 662e 6172 6773  rite = self.args
-00010190: 2e6e 770a 2020 2020 2020 2020 7666 732c  .nw.        vfs,
-000101a0: 2072 656d 203d 2073 656c 662e 6173 7276   rem = self.asrv
-000101b0: 2e76 6673 2e67 6574 2873 656c 662e 7670  .vfs.get(self.vp
-000101c0: 6174 682c 2073 656c 662e 756e 616d 652c  ath, self.uname,
-000101d0: 2046 616c 7365 2c20 5472 7565 290a 2020   False, True).  
-000101e0: 2020 2020 2020 7365 6c66 2e5f 6173 7365        self._asse
-000101f0: 7274 5f73 6166 655f 7265 6d28 7265 6d29  rt_safe_rem(rem)
-00010200: 0a0a 2020 2020 2020 2020 7570 6c6f 6164  ..        upload
-00010210: 5f76 7061 7468 203d 2073 656c 662e 7670  _vpath = self.vp
-00010220: 6174 680a 2020 2020 2020 2020 6c69 6d20  ath.        lim 
-00010230: 3d20 7666 732e 6765 745f 6462 7628 7265  = vfs.get_dbv(re
-00010240: 6d29 5b30 5d2e 6c69 6d0a 2020 2020 2020  m)[0].lim.      
-00010250: 2020 6664 6972 5f62 6173 6520 3d20 7666    fdir_base = vf
-00010260: 732e 6361 6e6f 6e69 6361 6c28 7265 6d29  s.canonical(rem)
-00010270: 0a20 2020 2020 2020 2069 6620 6c69 6d3a  .        if lim:
-00010280: 0a20 2020 2020 2020 2020 2020 2066 6469  .            fdi
-00010290: 725f 6261 7365 2c20 7265 6d20 3d20 6c69  r_base, rem = li
-000102a0: 6d2e 616c 6c28 7365 6c66 2e69 702c 2072  m.all(self.ip, r
-000102b0: 656d 2c20 2d31 2c20 6664 6972 5f62 6173  em, -1, fdir_bas
-000102c0: 6529 0a20 2020 2020 2020 2020 2020 2075  e).            u
-000102d0: 706c 6f61 645f 7670 6174 6820 3d20 227b  pload_vpath = "{
-000102e0: 7d2f 7b7d 222e 666f 726d 6174 2876 6673  }/{}".format(vfs
-000102f0: 2e76 7061 7468 2c20 7265 6d29 2e73 7472  .vpath, rem).str
-00010300: 6970 2822 2f22 290a 2020 2020 2020 2020  ip("/").        
-00010310: 2020 2020 6966 206e 6f74 206e 756c 6c77      if not nullw
-00010320: 7269 7465 3a0a 2020 2020 2020 2020 2020  rite:.          
-00010330: 2020 2020 2020 626f 732e 6d61 6b65 6469        bos.makedi
-00010340: 7273 2866 6469 725f 6261 7365 290a 0a20  rs(fdir_base).. 
-00010350: 2020 2020 2020 2072 6e64 2c20 7761 6e74         rnd, want
-00010360: 5f75 726c 2c20 6c69 6665 7469 6d65 2c20  _url, lifetime, 
-00010370: 7862 752c 2078 6175 203d 2073 656c 662e  xbu, xau = self.
-00010380: 7570 6c6f 6164 5f66 6c61 6773 2876 6673  upload_flags(vfs
-00010390: 290a 0a20 2020 2020 2020 2066 696c 6573  )..        files
-000103a0: 2020 2020 2020 203d 205b 5d0a 2020 2020         = [].    
-000103b0: 2020 2020 2320 737a 2c20 7368 615f 6865      # sz, sha_he
-000103c0: 782c 2073 6861 5f62 3634 2c20 705f 6669  x, sha_b64, p_fi
-000103d0: 6c65 2c20 666e 616d 652c 2061 6273 7061  le, fname, abspa
-000103e0: 7468 0a20 2020 2020 2020 2065 7272 6d73  th.        errms
-000103f0: 6720 3d20 2222 0a20 2020 2020 2020 2064  g = "".        d
-00010400: 6970 203d 2073 656c 662e 6469 7028 290a  ip = self.dip().
-00010410: 2020 2020 2020 2020 7430 203d 2074 696d          t0 = tim
-00010420: 652e 7469 6d65 2829 0a20 2020 2020 2020  e.time().       
-00010430: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00010440: 2020 6173 7365 7274 2073 656c 662e 7061    assert self.pa
-00010450: 7273 6572 2e67 656e 0a20 2020 2020 2020  rser.gen.       
-00010460: 2020 2020 2066 6f72 206e 6669 6c65 2c20       for nfile, 
-00010470: 2870 5f66 6965 6c64 2c20 705f 6669 6c65  (p_field, p_file
-00010480: 2c20 705f 6461 7461 2920 696e 2065 6e75  , p_data) in enu
-00010490: 6d65 7261 7465 2873 656c 662e 7061 7273  merate(self.pars
-000104a0: 6572 2e67 656e 293a 0a20 2020 2020 2020  er.gen):.       
-000104b0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-000104c0: 705f 6669 6c65 3a0a 2020 2020 2020 2020  p_file:.        
-000104d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000104e0: 2e6c 6f67 2822 6469 7363 6172 6469 6e67  .log("discarding
-000104f0: 2069 6e63 6f6d 696e 6720 6669 6c65 2077   incoming file w
-00010500: 6974 686f 7574 2066 696c 656e 616d 6522  ithout filename"
-00010510: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010520: 2020 2020 2020 2320 6661 6c6c 7468 726f        # fallthro
-00010530: 7567 680a 0a20 2020 2020 2020 2020 2020  ugh..           
-00010540: 2020 2020 2066 6469 7220 3d20 6664 6972       fdir = fdir
-00010550: 5f62 6173 650a 2020 2020 2020 2020 2020  _base.          
-00010560: 2020 2020 2020 666e 616d 6520 3d20 7361        fname = sa
-00010570: 6e69 7469 7a65 5f66 6e28 0a20 2020 2020  nitize_fn(.     
-00010580: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00010590: 5f66 696c 6520 6f72 2022 222c 2022 222c  _file or "", "",
-000105a0: 205b 222e 7072 6f6c 6f67 7565 2e68 746d   [".prologue.htm
-000105b0: 6c22 2c20 222e 6570 696c 6f67 7565 2e68  l", ".epilogue.h
-000105c0: 746d 6c22 5d0a 2020 2020 2020 2020 2020  tml"].          
-000105d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000105e0: 2020 2020 2020 2020 6966 2070 5f66 696c          if p_fil
-000105f0: 6520 616e 6420 6e6f 7420 6e75 6c6c 7772  e and not nullwr
-00010600: 6974 653a 0a20 2020 2020 2020 2020 2020  ite:.           
-00010610: 2020 2020 2020 2020 2069 6620 726e 643a           if rnd:
-00010620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010630: 2020 2020 2020 2020 2066 6e61 6d65 203d           fname =
-00010640: 2072 616e 645f 6e61 6d65 2866 6469 722c   rand_name(fdir,
-00010650: 2066 6e61 6d65 2c20 726e 6429 0a0a 2020   fname, rnd)..  
+0000d730: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
+0000d740: 3430 302c 2022 736f 6d65 2066 696c 6520  400, "some file 
+0000d750: 676f 7420 796f 7572 2066 6f6c 6465 7220  got your folder 
+0000d760: 6e61 6d65 2229 0a0a 2020 2020 2020 2020  name")..        
+0000d770: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000d780: 6520 5065 626b 6163 2835 3030 2c20 6d69  e Pebkac(500, mi
+0000d790: 6e5f 6578 2829 290a 2020 2020 2020 2020  n_ex()).        
+0000d7a0: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+0000d7b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000d7c0: 6520 5065 626b 6163 2835 3030 2c20 6d69  e Pebkac(500, mi
+0000d7d0: 6e5f 6578 2829 290a 0a20 2020 2020 2020  n_ex())..       
+0000d7e0: 2078 203d 2073 656c 662e 636f 6e6e 2e68   x = self.conn.h
+0000d7f0: 7372 762e 6272 6f6b 6572 2e61 736b 2822  srv.broker.ask("
+0000d800: 7570 326b 2e68 616e 646c 655f 6a73 6f6e  up2k.handle_json
+0000d810: 222c 2062 6f64 792c 2073 656c 662e 7532  ", body, self.u2
+0000d820: 6668 2e61 7073 290a 2020 2020 2020 2020  fh.aps).        
+0000d830: 7265 7420 3d20 782e 6765 7428 290a 2020  ret = x.get().  
+0000d840: 2020 2020 2020 6966 2073 656c 662e 6973        if self.is
+0000d850: 5f76 7072 6f78 6965 643a 0a20 2020 2020  _vproxied:.     
+0000d860: 2020 2020 2020 2069 6620 2270 7572 6c22         if "purl"
+0000d870: 2069 6e20 7265 743a 0a20 2020 2020 2020   in ret:.       
+0000d880: 2020 2020 2020 2020 2072 6574 5b22 7075           ret["pu
+0000d890: 726c 225d 203d 2073 656c 662e 6172 6773  rl"] = self.args
+0000d8a0: 2e53 5220 2b20 7265 745b 2270 7572 6c22  .SR + ret["purl"
+0000d8b0: 5d0a 0a20 2020 2020 2020 2072 6574 203d  ]..        ret =
+0000d8c0: 206a 736f 6e2e 6475 6d70 7328 7265 7429   json.dumps(ret)
+0000d8d0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+0000d8e0: 6728 7265 7429 0a20 2020 2020 2020 2073  g(ret).        s
+0000d8f0: 656c 662e 7265 706c 7928 7265 742e 656e  elf.reply(ret.en
+0000d900: 636f 6465 2822 7574 662d 3822 292c 206d  code("utf-8"), m
+0000d910: 696d 653d 2261 7070 6c69 6361 7469 6f6e  ime="application
+0000d920: 2f6a 736f 6e22 290a 2020 2020 2020 2020  /json").        
+0000d930: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+0000d940: 2064 6566 2068 616e 646c 655f 7365 6172   def handle_sear
+0000d950: 6368 2873 656c 662c 2062 6f64 7920 2029  ch(self, body  )
+0000d960: 2020 3a0a 2020 2020 2020 2020 6964 7820    :.        idx 
+0000d970: 3d20 7365 6c66 2e63 6f6e 6e2e 6765 745f  = self.conn.get_
+0000d980: 7532 6964 7828 290a 2020 2020 2020 2020  u2idx().        
+0000d990: 6966 206e 6f74 2068 6173 6174 7472 2869  if not hasattr(i
+0000d9a0: 6478 2c20 2270 5f65 6e64 2229 3a0a 2020  dx, "p_end"):.  
+0000d9b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000d9c0: 5065 626b 6163 2835 3030 2c20 2273 716c  Pebkac(500, "sql
+0000d9d0: 6974 6533 2069 7320 6e6f 7420 6176 6169  ite3 is not avai
+0000d9e0: 6c61 626c 6520 6f6e 2074 6865 2073 6572  lable on the ser
+0000d9f0: 7665 723b 2063 616e 6e6f 7420 7365 6172  ver; cannot sear
+0000da00: 6368 2229 0a0a 2020 2020 2020 2020 766f  ch")..        vo
+0000da10: 6c73 203d 205b 5d0a 2020 2020 2020 2020  ls = [].        
+0000da20: 7365 656e 203d 207b 7d0a 2020 2020 2020  seen = {}.      
+0000da30: 2020 666f 7220 7674 6f70 2069 6e20 7365    for vtop in se
+0000da40: 6c66 2e72 766f 6c3a 0a20 2020 2020 2020  lf.rvol:.       
+0000da50: 2020 2020 2076 6673 2c20 5f20 3d20 7365       vfs, _ = se
+0000da60: 6c66 2e61 7372 762e 7666 732e 6765 7428  lf.asrv.vfs.get(
+0000da70: 7674 6f70 2c20 7365 6c66 2e75 6e61 6d65  vtop, self.uname
+0000da80: 2c20 5472 7565 2c20 4661 6c73 6529 0a20  , True, False). 
+0000da90: 2020 2020 2020 2020 2020 2076 6673 203d             vfs =
+0000daa0: 2076 6673 2e64 6276 206f 7220 7666 730a   vfs.dbv or vfs.
+0000dab0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+0000dac0: 6673 2069 6e20 7365 656e 3a0a 2020 2020  fs in seen:.    
+0000dad0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000dae0: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
+0000daf0: 2020 7365 656e 5b76 6673 5d20 3d20 5472    seen[vfs] = Tr
+0000db00: 7565 0a20 2020 2020 2020 2020 2020 2076  ue.            v
+0000db10: 6f6c 732e 6170 7065 6e64 2828 7666 732e  ols.append((vfs.
+0000db20: 7670 6174 682c 2076 6673 2e72 6561 6c70  vpath, vfs.realp
+0000db30: 6174 682c 2076 6673 2e66 6c61 6773 2929  ath, vfs.flags))
+0000db40: 0a0a 2020 2020 2020 2020 7430 203d 2074  ..        t0 = t
+0000db50: 696d 652e 7469 6d65 2829 0a20 2020 2020  ime.time().     
+0000db60: 2020 2069 6620 6964 782e 705f 656e 643a     if idx.p_end:
+0000db70: 0a20 2020 2020 2020 2020 2020 2070 656e  .            pen
+0000db80: 616c 7479 203d 2030 2e37 0a20 2020 2020  alty = 0.7.     
+0000db90: 2020 2020 2020 2074 5f69 646c 6520 3d20         t_idle = 
+0000dba0: 7430 202d 2069 6478 2e70 5f65 6e64 0a20  t0 - idx.p_end. 
+0000dbb0: 2020 2020 2020 2020 2020 2069 6620 6964             if id
+0000dbc0: 782e 705f 6475 7220 3e20 302e 3720 616e  x.p_dur > 0.7 an
+0000dbd0: 6420 745f 6964 6c65 203c 2070 656e 616c  d t_idle < penal
+0000dbe0: 7479 3a0a 2020 2020 2020 2020 2020 2020  ty:.            
+0000dbf0: 2020 2020 7420 3d20 2272 6174 652d 6c69      t = "rate-li
+0000dc00: 6d69 7420 7b3a 2e31 667d 2073 6563 2c20  mit {:.1f} sec, 
+0000dc10: 636f 7374 207b 3a2e 3266 7d2c 2069 646c  cost {:.2f}, idl
+0000dc20: 6520 7b3a 2e32 667d 220a 2020 2020 2020  e {:.2f}".      
+0000dc30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000dc40: 5065 626b 6163 2834 3239 2c20 742e 666f  Pebkac(429, t.fo
+0000dc50: 726d 6174 2870 656e 616c 7479 2c20 6964  rmat(penalty, id
+0000dc60: 782e 705f 6475 722c 2074 5f69 646c 6529  x.p_dur, t_idle)
+0000dc70: 290a 0a20 2020 2020 2020 2069 6620 2273  )..        if "s
+0000dc80: 7263 6822 2069 6e20 626f 6479 3a0a 2020  rch" in body:.  
+0000dc90: 2020 2020 2020 2020 2020 2320 7365 6172            # sear
+0000dca0: 6368 2062 7920 7570 326b 2068 6173 686c  ch by up2k hashl
+0000dcb0: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
+0000dcc0: 7662 6f64 7920 3d20 636f 7079 2e64 6565  vbody = copy.dee
+0000dcd0: 7063 6f70 7928 626f 6479 290a 2020 2020  pcopy(body).    
+0000dce0: 2020 2020 2020 2020 7662 6f64 795b 2268          vbody["h
+0000dcf0: 6173 6822 5d20 3d20 6c65 6e28 7662 6f64  ash"] = len(vbod
+0000dd00: 795b 2268 6173 6822 5d29 0a20 2020 2020  y["hash"]).     
+0000dd10: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
+0000dd20: 2271 6a3a 2022 202b 2072 6570 7228 7662  "qj: " + repr(vb
+0000dd30: 6f64 7929 290a 2020 2020 2020 2020 2020  ody)).          
+0000dd40: 2020 6869 7473 203d 2069 6478 2e66 7365    hits = idx.fse
+0000dd50: 6172 6368 2876 6f6c 732c 2062 6f64 7929  arch(vols, body)
+0000dd60: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
+0000dd70: 2020 3d20 7265 7072 2868 6974 7329 0a20    = repr(hits). 
+0000dd80: 2020 2020 2020 2020 2020 2074 6167 6c69             tagli
+0000dd90: 7374 2020 3d20 5b5d 0a20 2020 2020 2020  st  = [].       
+0000dda0: 2020 2020 2074 7275 6e63 203d 2046 616c       trunc = Fal
+0000ddb0: 7365 0a20 2020 2020 2020 2065 6c73 653a  se.        else:
+0000ddc0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
+0000ddd0: 6561 7263 6820 6279 2071 7565 7279 2070  earch by query p
+0000dde0: 6172 616d 730a 2020 2020 2020 2020 2020  arams.          
+0000ddf0: 2020 7120 3d20 626f 6479 5b22 7122 5d0a    q = body["q"].
+0000de00: 2020 2020 2020 2020 2020 2020 6e20 3d20              n = 
+0000de10: 626f 6479 2e67 6574 2822 6e22 2c20 7365  body.get("n", se
+0000de20: 6c66 2e61 7267 732e 7372 6368 5f68 6974  lf.args.srch_hit
+0000de30: 7329 0a20 2020 2020 2020 2020 2020 2073  s).            s
+0000de40: 656c 662e 6c6f 6728 2271 6a3a 207b 7d20  elf.log("qj: {} 
+0000de50: 7c7b 7d7c 222e 666f 726d 6174 2871 2c20  |{}|".format(q, 
+0000de60: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
+0000de70: 6869 7473 2c20 7461 676c 6973 742c 2074  hits, taglist, t
+0000de80: 7275 6e63 203d 2069 6478 2e73 6561 7263  runc = idx.searc
+0000de90: 6828 766f 6c73 2c20 712c 206e 290a 2020  h(vols, q, n).  
+0000dea0: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
+0000deb0: 6c65 6e28 6869 7473 290a 0a20 2020 2020  len(hits)..     
+0000dec0: 2020 2069 6478 2e70 5f65 6e64 203d 2074     idx.p_end = t
+0000ded0: 696d 652e 7469 6d65 2829 0a20 2020 2020  ime.time().     
+0000dee0: 2020 2069 6478 2e70 5f64 7572 203d 2069     idx.p_dur = i
+0000def0: 6478 2e70 5f65 6e64 202d 2074 300a 2020  dx.p_end - t0.  
+0000df00: 2020 2020 2020 7365 6c66 2e6c 6f67 2822        self.log("
+0000df10: 7123 3a20 7b7d 2028 7b3a 2e32 667d 7329  q#: {} ({:.2f}s)
+0000df20: 222e 666f 726d 6174 286d 7367 2c20 6964  ".format(msg, id
+0000df30: 782e 705f 6475 7229 290a 0a20 2020 2020  x.p_dur))..     
+0000df40: 2020 206f 7264 6572 203d 205b 5d0a 2020     order = [].  
+0000df50: 2020 2020 2020 6366 6720 3d20 7365 6c66        cfg = self
+0000df60: 2e61 7267 732e 6d74 652e 7370 6c69 7428  .args.mte.split(
+0000df70: 222c 2229 0a20 2020 2020 2020 2066 6f72  ",").        for
+0000df80: 2074 2069 6e20 6366 673a 0a20 2020 2020   t in cfg:.     
+0000df90: 2020 2020 2020 2069 6620 7420 696e 2074         if t in t
+0000dfa0: 6167 6c69 7374 3a0a 2020 2020 2020 2020  aglist:.        
+0000dfb0: 2020 2020 2020 2020 6f72 6465 722e 6170          order.ap
+0000dfc0: 7065 6e64 2874 290a 2020 2020 2020 2020  pend(t).        
+0000dfd0: 666f 7220 7420 696e 2074 6167 6c69 7374  for t in taglist
+0000dfe0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000dff0: 2074 206e 6f74 2069 6e20 6f72 6465 723a   t not in order:
+0000e000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e010: 206f 7264 6572 2e61 7070 656e 6428 7429   order.append(t)
+0000e020: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000e030: 662e 6973 5f76 7072 6f78 6965 643a 0a20  f.is_vproxied:. 
+0000e040: 2020 2020 2020 2020 2020 2066 6f72 2068             for h
+0000e050: 6974 2069 6e20 6869 7473 3a0a 2020 2020  it in hits:.    
+0000e060: 2020 2020 2020 2020 2020 2020 6869 745b              hit[
+0000e070: 2272 7022 5d20 3d20 7365 6c66 2e61 7267  "rp"] = self.arg
+0000e080: 732e 5253 202b 2068 6974 5b22 7270 225d  s.RS + hit["rp"]
+0000e090: 0a0a 2020 2020 2020 2020 726a 203d 207b  ..        rj = {
+0000e0a0: 2268 6974 7322 3a20 6869 7473 2c20 2274  "hits": hits, "t
+0000e0b0: 6167 5f6f 7264 6572 223a 206f 7264 6572  ag_order": order
+0000e0c0: 2c20 2274 7275 6e63 223a 2074 7275 6e63  , "trunc": trunc
+0000e0d0: 7d0a 2020 2020 2020 2020 7220 3d20 6a73  }.        r = js
+0000e0e0: 6f6e 2e64 756d 7073 2872 6a29 2e65 6e63  on.dumps(rj).enc
+0000e0f0: 6f64 6528 2275 7466 2d38 2229 0a20 2020  ode("utf-8").   
+0000e100: 2020 2020 2073 656c 662e 7265 706c 7928       self.reply(
+0000e110: 722c 206d 696d 653d 2261 7070 6c69 6361  r, mime="applica
+0000e120: 7469 6f6e 2f6a 736f 6e22 290a 2020 2020  tion/json").    
+0000e130: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000e140: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
+0000e150: 706f 7374 5f62 696e 6172 7928 7365 6c66  post_binary(self
+0000e160: 2920 203a 0a20 2020 2020 2020 2074 7279  )  :.        try
+0000e170: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000e180: 6d61 696e 7320 3d20 696e 7428 7365 6c66  mains = int(self
+0000e190: 2e68 6561 6465 7273 5b22 636f 6e74 656e  .headers["conten
+0000e1a0: 742d 6c65 6e67 7468 225d 290a 2020 2020  t-length"]).    
+0000e1b0: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+0000e1c0: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
+0000e1d0: 626b 6163 2834 3030 2c20 2279 6f75 206d  bkac(400, "you m
+0000e1e0: 7573 7420 7375 7070 6c79 2061 2063 6f6e  ust supply a con
+0000e1f0: 7465 6e74 2d6c 656e 6774 6820 666f 7220  tent-length for 
+0000e200: 6269 6e61 7279 2050 4f53 5422 290a 0a20  binary POST").. 
+0000e210: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000e220: 2020 2020 2020 2020 6368 6173 6820 3d20          chash = 
+0000e230: 7365 6c66 2e68 6561 6465 7273 5b22 782d  self.headers["x-
+0000e240: 7570 326b 2d68 6173 6822 5d0a 2020 2020  up2k-hash"].    
+0000e250: 2020 2020 2020 2020 7761 726b 203d 2073          wark = s
+0000e260: 656c 662e 6865 6164 6572 735b 2278 2d75  elf.headers["x-u
+0000e270: 7032 6b2d 7761 726b 225d 0a20 2020 2020  p2k-wark"].     
+0000e280: 2020 2065 7863 6570 7420 4b65 7945 7272     except KeyErr
+0000e290: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+0000e2a0: 7261 6973 6520 5065 626b 6163 2834 3030  raise Pebkac(400
+0000e2b0: 2c20 226e 6565 6420 6861 7368 2061 6e64  , "need hash and
+0000e2c0: 2077 6172 6b20 6865 6164 6572 7320 666f   wark headers fo
+0000e2d0: 7220 6269 6e61 7279 2050 4f53 5422 290a  r binary POST").
+0000e2e0: 0a20 2020 2020 2020 2076 6673 2c20 5f20  .        vfs, _ 
+0000e2f0: 3d20 7365 6c66 2e61 7372 762e 7666 732e  = self.asrv.vfs.
+0000e300: 6765 7428 7365 6c66 2e76 7061 7468 2c20  get(self.vpath, 
+0000e310: 7365 6c66 2e75 6e61 6d65 2c20 4661 6c73  self.uname, Fals
+0000e320: 652c 2054 7275 6529 0a20 2020 2020 2020  e, True).       
+0000e330: 2070 746f 7020 3d20 2876 6673 2e64 6276   ptop = (vfs.dbv
+0000e340: 206f 7220 7666 7329 2e72 6561 6c70 6174   or vfs).realpat
+0000e350: 680a 0a20 2020 2020 2020 2078 203d 2073  h..        x = s
+0000e360: 656c 662e 636f 6e6e 2e68 7372 762e 6272  elf.conn.hsrv.br
+0000e370: 6f6b 6572 2e61 736b 2822 7570 326b 2e68  oker.ask("up2k.h
+0000e380: 616e 646c 655f 6368 756e 6b22 2c20 7074  andle_chunk", pt
+0000e390: 6f70 2c20 7761 726b 2c20 6368 6173 6829  op, wark, chash)
+0000e3a0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+0000e3b0: 6520 3d20 782e 6765 7428 290a 2020 2020  e = x.get().    
+0000e3c0: 2020 2020 6368 756e 6b73 697a 652c 2063      chunksize, c
+0000e3d0: 7374 6172 742c 2070 6174 682c 206c 6173  start, path, las
+0000e3e0: 746d 6f64 2c20 7370 7273 203d 2072 6573  tmod, sprs = res
+0000e3f0: 706f 6e73 650a 0a20 2020 2020 2020 2074  ponse..        t
+0000e400: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000e410: 6966 2073 656c 662e 6172 6773 2e6e 773a  if self.args.nw:
+0000e420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e430: 2070 6174 6820 3d20 6f73 2e64 6576 6e75   path = os.devnu
+0000e440: 6c6c 0a0a 2020 2020 2020 2020 2020 2020  ll..            
+0000e450: 6966 2072 656d 6169 6e73 203e 2063 6875  if remains > chu
+0000e460: 6e6b 7369 7a65 3a0a 2020 2020 2020 2020  nksize:.        
+0000e470: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
+0000e480: 626b 6163 2834 3030 2c20 2279 6f75 7220  bkac(400, "your 
+0000e490: 6368 756e 6b20 6973 2074 6f6f 2062 6967  chunk is too big
+0000e4a0: 2074 6f20 6669 7422 290a 0a20 2020 2020   to fit")..     
+0000e4b0: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
+0000e4c0: 2277 7269 7469 6e67 207b 7d20 237b 7d20  "writing {} #{} 
+0000e4d0: 407b 7d20 6c65 6e20 7b7d 222e 666f 726d  @{} len {}".form
+0000e4e0: 6174 2870 6174 682c 2063 6861 7368 2c20  at(path, chash, 
+0000e4f0: 6373 7461 7274 2c20 7265 6d61 696e 7329  cstart, remains)
+0000e500: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
+0000e510: 6561 6465 7220 3d20 7265 6164 5f73 6f63  eader = read_soc
+0000e520: 6b65 7428 7365 6c66 2e73 722c 2072 656d  ket(self.sr, rem
+0000e530: 6169 6e73 290a 0a20 2020 2020 2020 2020  ains)..         
+0000e540: 2020 2066 203d 204e 6f6e 650a 2020 2020     f = None.    
+0000e550: 2020 2020 2020 2020 6670 6f6f 6c20 3d20          fpool = 
+0000e560: 6e6f 7420 7365 6c66 2e61 7267 732e 6e6f  not self.args.no
+0000e570: 5f66 706f 6f6c 2061 6e64 2073 7072 730a  _fpool and sprs.
+0000e580: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+0000e590: 706f 6f6c 3a0a 2020 2020 2020 2020 2020  pool:.          
+0000e5a0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000e5b0: 6d75 7465 783a 0a20 2020 2020 2020 2020  mutex:.         
+0000e5c0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5e0: 2020 2020 2020 2020 6620 3d20 7365 6c66          f = self
+0000e5f0: 2e75 3266 682e 706f 7028 7061 7468 290a  .u2fh.pop(path).
+0000e600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e610: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e630: 2020 2020 7061 7373 0a0a 2020 2020 2020      pass..      
+0000e640: 2020 2020 2020 6620 3d20 6620 6f72 206f        f = f or o
+0000e650: 7065 6e28 6673 656e 6328 7061 7468 292c  pen(fsenc(path),
+0000e660: 2022 7262 2b22 2c20 3531 3220 2a20 3130   "rb+", 512 * 10
+0000e670: 3234 290a 0a20 2020 2020 2020 2020 2020  24)..           
+0000e680: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000e690: 2020 2020 2020 662e 7365 656b 2863 7374        f.seek(cst
+0000e6a0: 6172 745b 305d 290a 2020 2020 2020 2020  art[0]).        
+0000e6b0: 2020 2020 2020 2020 706f 7374 5f73 7a2c          post_sz,
+0000e6c0: 205f 2c20 7368 615f 6236 3420 3d20 6861   _, sha_b64 = ha
+0000e6d0: 7368 636f 7079 2872 6561 6465 722c 2066  shcopy(reader, f
+0000e6e0: 2c20 7365 6c66 2e61 7267 732e 735f 7772  , self.args.s_wr
+0000e6f0: 5f73 6c70 290a 0a20 2020 2020 2020 2020  _slp)..         
+0000e700: 2020 2020 2020 2069 6620 7368 615f 6236         if sha_b6
+0000e710: 3420 213d 2063 6861 7368 3a0a 2020 2020  4 != chash:.    
+0000e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e730: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000e740: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e750: 662e 6261 6b66 6c69 7028 662c 2063 7374  f.bakflip(f, cst
+0000e760: 6172 745b 305d 2c20 706f 7374 5f73 7a2c  art[0], post_sz,
+0000e770: 2073 6861 5f62 3634 290a 2020 2020 2020   sha_b64).      
+0000e780: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0000e790: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+0000e7a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e7b0: 6c66 2e6c 6f67 2822 6261 6b66 6c69 7020  lf.log("bakflip 
+0000e7c0: 6661 696c 6564 3a20 2220 2b20 6d69 6e5f  failed: " + min_
+0000e7d0: 6578 2829 290a 0a20 2020 2020 2020 2020  ex())..         
+0000e7e0: 2020 2020 2020 2020 2020 2074 203d 2022             t = "
+0000e7f0: 796f 7572 2063 6875 6e6b 2067 6f74 2063  your chunk got c
+0000e800: 6f72 7275 7074 6564 2073 6f6d 6568 6f77  orrupted somehow
+0000e810: 2028 7265 6365 6976 6564 207b 7d20 6279   (received {} by
+0000e820: 7465 7329 3b20 6578 7065 6374 6564 2076  tes); expected v
+0000e830: 7320 7265 6365 6976 6564 2068 6173 683a  s received hash:
+0000e840: 5c6e 7b7d 5c6e 7b7d 220a 2020 2020 2020  \n{}\n{}".      
+0000e850: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000e860: 6973 6520 5065 626b 6163 2834 3030 2c20  ise Pebkac(400, 
+0000e870: 742e 666f 726d 6174 2870 6f73 745f 737a  t.format(post_sz
+0000e880: 2c20 6368 6173 682c 2073 6861 5f62 3634  , chash, sha_b64
+0000e890: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+0000e8a0: 2020 2020 6966 206c 656e 2863 7374 6172      if len(cstar
+0000e8b0: 7429 203e 2031 2061 6e64 2070 6174 6820  t) > 1 and path 
+0000e8c0: 213d 206f 732e 6465 766e 756c 6c3a 0a20  != os.devnull:. 
+0000e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8e0: 2020 2073 656c 662e 6c6f 6728 0a20 2020     self.log(.   
+0000e8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e900: 2020 2020 2022 636c 6f6e 6520 7b7d 2074       "clone {} t
+0000e910: 6f20 7b7d 222e 666f 726d 6174 280a 2020  o {}".format(.  
+0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e930: 2020 2020 2020 2020 2020 6373 7461 7274            cstart
+0000e940: 5b30 5d2c 2022 2026 2022 2e6a 6f69 6e28  [0], " & ".join(
+0000e950: 756e 6963 6f64 6528 7829 2066 6f72 2078  unicode(x) for x
+0000e960: 2069 6e20 6373 7461 7274 5b31 3a5d 290a   in cstart[1:]).
+0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e980: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000e990: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9b0: 2020 2020 6f66 7320 3d20 300a 2020 2020      ofs = 0.    
+0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9d0: 7768 696c 6520 6f66 7320 3c20 6368 756e  while ofs < chun
+0000e9e0: 6b73 697a 653a 0a20 2020 2020 2020 2020  ksize:.         
+0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000ea00: 7566 737a 203d 206d 696e 2863 6875 6e6b  ufsz = min(chunk
+0000ea10: 7369 7a65 202d 206f 6673 2c20 3420 2a20  size - ofs, 4 * 
+0000ea20: 3130 3234 202a 2031 3032 3429 0a20 2020  1024 * 1024).   
+0000ea30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea40: 2020 2020 2066 2e73 6565 6b28 6373 7461       f.seek(csta
+0000ea50: 7274 5b30 5d20 2b20 6f66 7329 0a20 2020  rt[0] + ofs).   
+0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea70: 2020 2020 2062 7566 203d 2066 2e72 6561       buf = f.rea
+0000ea80: 6428 6275 6673 7a29 0a20 2020 2020 2020  d(bufsz).       
+0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eaa0: 2066 6f72 2077 6f66 7320 696e 2063 7374   for wofs in cst
+0000eab0: 6172 745b 313a 5d3a 0a20 2020 2020 2020  art[1:]:.       
+0000eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ead0: 2020 2020 2066 2e73 6565 6b28 776f 6673       f.seek(wofs
+0000eae0: 202b 206f 6673 290a 2020 2020 2020 2020   + ofs).        
+0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb00: 2020 2020 662e 7772 6974 6528 6275 6629      f.write(buf)
+0000eb10: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000eb20: 2020 2020 2020 2020 2020 6f66 7320 2b3d            ofs +=
+0000eb30: 206c 656e 2862 7566 290a 0a20 2020 2020   len(buf)..     
+0000eb40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000eb50: 656c 662e 6c6f 6728 2263 6c6f 6e65 207b  elf.log("clone {
+0000eb60: 7d20 646f 6e65 222e 666f 726d 6174 2863  } done".format(c
+0000eb70: 7374 6172 745b 305d 2929 0a0a 2020 2020  start[0]))..    
+0000eb80: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000eb90: 6f74 2066 706f 6f6c 3a0a 2020 2020 2020  ot fpool:.      
+0000eba0: 2020 2020 2020 2020 2020 2020 2020 662e                f.
+0000ebb0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+0000ebc0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000ebd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebe0: 2020 7769 7468 2073 656c 662e 6d75 7465    with self.mute
+0000ebf0: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
+0000ec00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ec10: 7532 6668 2e70 7574 2870 6174 682c 2066  u2fh.put(path, f
+0000ec20: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+0000ec30: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+0000ec40: 2020 2020 2020 2320 6d61 7962 6520 6275        # maybe bu
+0000ec50: 7374 6564 2068 616e 646c 6520 2865 672e  sted handle (eg.
+0000ec60: 2064 6973 6b20 7765 6e74 2066 756c 6c29   disk went full)
+0000ec70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ec80: 2066 2e63 6c6f 7365 2829 0a20 2020 2020   f.close().     
+0000ec90: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000eca0: 0a20 2020 2020 2020 2066 696e 616c 6c79  .        finally
+0000ecb0: 3a0a 2020 2020 2020 2020 2020 2020 7820  :.            x 
+0000ecc0: 3d20 7365 6c66 2e63 6f6e 6e2e 6873 7276  = self.conn.hsrv
+0000ecd0: 2e62 726f 6b65 722e 6173 6b28 2275 7032  .broker.ask("up2
+0000ece0: 6b2e 7265 6c65 6173 655f 6368 756e 6b22  k.release_chunk"
+0000ecf0: 2c20 7074 6f70 2c20 7761 726b 2c20 6368  , ptop, wark, ch
+0000ed00: 6173 6829 0a20 2020 2020 2020 2020 2020  ash).           
+0000ed10: 2078 2e67 6574 2829 2020 2320 626c 6f63   x.get()  # bloc
+0000ed20: 6b20 636c 6965 6e74 2075 6e74 696c 2072  k client until r
+0000ed30: 656c 6561 7365 640a 0a20 2020 2020 2020  eleased..       
+0000ed40: 2078 203d 2073 656c 662e 636f 6e6e 2e68   x = self.conn.h
+0000ed50: 7372 762e 6272 6f6b 6572 2e61 736b 2822  srv.broker.ask("
+0000ed60: 7570 326b 2e63 6f6e 6669 726d 5f63 6875  up2k.confirm_chu
+0000ed70: 6e6b 222c 2070 746f 702c 2077 6172 6b2c  nk", ptop, wark,
+0000ed80: 2063 6861 7368 290a 2020 2020 2020 2020   chash).        
+0000ed90: 7a74 6973 203d 2078 2e67 6574 2829 0a20  ztis = x.get(). 
+0000eda0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000edb0: 2020 2020 2020 2020 6e75 6d5f 6c65 6674          num_left
+0000edc0: 2c20 6669 6e5f 7061 7468 203d 207a 7469  , fin_path = zti
+0000edd0: 730a 2020 2020 2020 2020 6578 6365 7074  s.        except
+0000ede0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000edf0: 6c66 2e6c 6f75 645f 7265 706c 7928 7a74  lf.loud_reply(zt
+0000ee00: 6973 2c20 7374 6174 7573 3d35 3030 290a  is, status=500).
+0000ee10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000ee20: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
+0000ee30: 2020 6966 206e 6f74 206e 756d 5f6c 6566    if not num_lef
+0000ee40: 7420 616e 6420 6670 6f6f 6c3a 0a20 2020  t and fpool:.   
+0000ee50: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+0000ee60: 6c66 2e6d 7574 6578 3a0a 2020 2020 2020  lf.mutex:.      
+0000ee70: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000ee80: 3266 682e 636c 6f73 6528 7061 7468 290a  2fh.close(path).
+0000ee90: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000eea0: 6e75 6d5f 6c65 6674 2061 6e64 206e 6f74  num_left and not
+0000eeb0: 2073 656c 662e 6172 6773 2e6e 773a 0a20   self.args.nw:. 
+0000eec0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000eed0: 636f 6e6e 2e68 7372 762e 6272 6f6b 6572  conn.hsrv.broker
+0000eee0: 2e61 736b 280a 2020 2020 2020 2020 2020  .ask(.          
+0000eef0: 2020 2020 2020 2275 7032 6b2e 6669 6e69        "up2k.fini
+0000ef00: 7368 5f75 706c 6f61 6422 2c20 7074 6f70  sh_upload", ptop
+0000ef10: 2c20 7761 726b 2c20 7365 6c66 2e75 3266  , wark, self.u2f
+0000ef20: 682e 6170 730a 2020 2020 2020 2020 2020  h.aps.          
+0000ef30: 2020 292e 6765 7428 290a 0a20 2020 2020    ).get()..     
+0000ef40: 2020 2063 696e 6620 3d20 7365 6c66 2e68     cinf = self.h
+0000ef50: 6561 6465 7273 2e67 6574 2822 782d 7570  eaders.get("x-up
+0000ef60: 326b 2d73 7461 7422 2c20 2222 290a 0a20  2k-stat", "").. 
+0000ef70: 2020 2020 2020 2073 7064 203d 2073 656c         spd = sel
+0000ef80: 662e 5f73 7064 2870 6f73 745f 737a 290a  f._spd(post_sz).
+0000ef90: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+0000efa0: 2822 7b3a 3730 7d20 7468 616e 6b20 7b7d  ("{:70} thank {}
+0000efb0: 222e 666f 726d 6174 2873 7064 2c20 6369  ".format(spd, ci
+0000efc0: 6e66 2929 0a20 2020 2020 2020 2073 656c  nf)).        sel
+0000efd0: 662e 7265 706c 7928 6222 7468 616e 6b22  f.reply(b"thank"
+0000efe0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000eff0: 2054 7275 650a 0a20 2020 2064 6566 2068   True..    def h
+0000f000: 616e 646c 655f 6c6f 6769 6e28 7365 6c66  andle_login(self
+0000f010: 2920 203a 0a20 2020 2020 2020 2061 7373  )  :.        ass
+0000f020: 6572 7420 7365 6c66 2e70 6172 7365 720a  ert self.parser.
+0000f030: 2020 2020 2020 2020 7077 6420 3d20 7365          pwd = se
+0000f040: 6c66 2e70 6172 7365 722e 7265 7175 6972  lf.parser.requir
+0000f050: 6528 2263 7070 7764 222c 2036 3429 0a20  e("cppwd", 64). 
+0000f060: 2020 2020 2020 2073 656c 662e 7061 7273         self.pars
+0000f070: 6572 2e64 726f 7028 290a 0a20 2020 2020  er.drop()..     
+0000f080: 2020 2073 656c 662e 6f75 745f 6865 6164     self.out_head
+0000f090: 6572 6c69 7374 203d 205b 0a20 2020 2020  erlist = [.     
+0000f0a0: 2020 2020 2020 2078 2066 6f72 2078 2069         x for x i
+0000f0b0: 6e20 7365 6c66 2e6f 7574 5f68 6561 6465  n self.out_heade
+0000f0c0: 726c 6973 7420 6966 2078 5b30 5d20 213d  rlist if x[0] !=
+0000f0d0: 2022 5365 742d 436f 6f6b 6965 2220 6f72   "Set-Cookie" or
+0000f0e0: 2022 6370 7077 2220 213d 2078 5b31 5d5b   "cppw" != x[1][
+0000f0f0: 3a34 5d0a 2020 2020 2020 2020 5d0a 0a20  :4].        ].. 
+0000f100: 2020 2020 2020 2064 7374 203d 2073 656c         dst = sel
+0000f110: 662e 6172 6773 2e53 5253 0a20 2020 2020  f.args.SRS.     
+0000f120: 2020 2069 6620 7365 6c66 2e76 7061 7468     if self.vpath
+0000f130: 3a0a 2020 2020 2020 2020 2020 2020 6473  :.            ds
+0000f140: 7420 2b3d 2071 756f 7465 7028 7365 6c66  t += quotep(self
+0000f150: 2e76 7061 7468 290a 0a20 2020 2020 2020  .vpath)..       
+0000f160: 206d 7367 203d 2073 656c 662e 6765 745f   msg = self.get_
+0000f170: 7077 645f 636f 6f6b 6965 2870 7764 290a  pwd_cookie(pwd).
+0000f180: 2020 2020 2020 2020 6874 6d6c 203d 2073          html = s
+0000f190: 656c 662e 6a32 7328 226d 7367 222c 2068  elf.j2s("msg", h
+0000f1a0: 313d 6d73 672c 2068 323d 273c 6120 6872  1=msg, h2='<a hr
+0000f1b0: 6566 3d22 2720 2b20 6473 7420 2b20 2722  ef="' + dst + '"
+0000f1c0: 3e61 636b 3c2f 613e 272c 2072 6564 6972  >ack</a>', redir
+0000f1d0: 3d64 7374 290a 2020 2020 2020 2020 7365  =dst).        se
+0000f1e0: 6c66 2e72 6570 6c79 2868 746d 6c2e 656e  lf.reply(html.en
+0000f1f0: 636f 6465 2822 7574 662d 3822 2929 0a20  code("utf-8")). 
+0000f200: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+0000f210: 7565 0a0a 2020 2020 6465 6620 6765 745f  ue..    def get_
+0000f220: 7077 645f 636f 6f6b 6965 2873 656c 662c  pwd_cookie(self,
+0000f230: 2070 7764 2029 2020 3a0a 2020 2020 2020   pwd )  :.      
+0000f240: 2020 6966 2070 7764 2069 6e20 7365 6c66    if pwd in self
+0000f250: 2e61 7372 762e 6961 6363 743a 0a20 2020  .asrv.iacct:.   
+0000f260: 2020 2020 2020 2020 206d 7367 203d 2022           msg = "
+0000f270: 6c6f 6769 6e20 6f6b 220a 2020 2020 2020  login ok".      
+0000f280: 2020 2020 2020 6475 7220 3d20 696e 7428        dur = int(
+0000f290: 3630 202a 2036 3020 2a20 7365 6c66 2e61  60 * 60 * self.a
+0000f2a0: 7267 732e 6c6f 676f 7574 290a 2020 2020  rgs.logout).    
+0000f2b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000f2c0: 2020 2020 2020 7365 6c66 2e6c 6f67 2822        self.log("
+0000f2d0: 696e 7661 6c69 6420 7061 7373 776f 7264  invalid password
+0000f2e0: 3a20 7b7d 222e 666f 726d 6174 2870 7764  : {}".format(pwd
+0000f2f0: 292c 2033 290a 2020 2020 2020 2020 2020  ), 3).          
+0000f300: 2020 6720 3d20 7365 6c66 2e63 6f6e 6e2e    g = self.conn.
+0000f310: 6873 7276 2e67 7077 640a 2020 2020 2020  hsrv.gpwd.      
+0000f320: 2020 2020 2020 6966 2067 2e6c 696d 3a0a        if g.lim:.
+0000f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f340: 626f 6e6b 2c20 6970 203d 2067 2e62 6f6e  bonk, ip = g.bon
+0000f350: 6b28 7365 6c66 2e69 702c 2070 7764 290a  k(self.ip, pwd).
+0000f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f370: 6966 2062 6f6e 6b3a 0a20 2020 2020 2020  if bonk:.       
+0000f380: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f390: 662e 6c6f 6728 2263 6c69 656e 7420 6261  f.log("client ba
+0000f3a0: 6e6e 6564 3a20 696e 7661 6c69 6420 7061  nned: invalid pa
+0000f3b0: 7373 776f 7264 7322 2c20 3129 0a20 2020  sswords", 1).   
+0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3d0: 2073 656c 662e 636f 6e6e 2e68 7372 762e   self.conn.hsrv.
+0000f3e0: 6261 6e73 5b69 705d 203d 2062 6f6e 6b0a  bans[ip] = bonk.
+0000f3f0: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
+0000f400: 203d 2022 6e61 7720 6475 6465 220a 2020   = "naw dude".  
+0000f410: 2020 2020 2020 2020 2020 7077 6420 3d20            pwd = 
+0000f420: 2278 2220 2023 206e 6f73 6563 0a20 2020  "x"  # nosec.   
+0000f430: 2020 2020 2020 2020 2064 7572 203d 204e           dur = N
+0000f440: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
+0000f450: 7077 6420 3d3d 2022 7822 3a0a 2020 2020  pwd == "x":.    
+0000f460: 2020 2020 2020 2020 2320 7265 7365 7420          # reset 
+0000f470: 626f 7468 2070 6c61 696e 7465 7874 2061  both plaintext a
+0000f480: 6e64 2074 6c73 0a20 2020 2020 2020 2020  nd tls.         
+0000f490: 2020 2023 2028 6f6e 6c79 2061 6666 6563     # (only affec
+0000f4a0: 7473 2061 6374 6976 6520 746c 7320 636f  ts active tls co
+0000f4b0: 6f6b 6965 7320 7768 656e 2074 6c73 290a  okies when tls).
+0000f4c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000f4d0: 6b20 696e 2028 2263 7070 7764 222c 2022  k in ("cppwd", "
+0000f4e0: 6370 7077 7322 2920 6966 2073 656c 662e  cppws") if self.
+0000f4f0: 6973 5f68 7474 7073 2065 6c73 6520 2822  is_https else ("
+0000f500: 6370 7077 6422 2c29 3a0a 2020 2020 2020  cppwd",):.      
+0000f510: 2020 2020 2020 2020 2020 636b 203d 2067            ck = g
+0000f520: 656e 636f 6f6b 6965 286b 2c20 7077 642c  encookie(k, pwd,
+0000f530: 2073 656c 662e 6172 6773 2e52 2c20 4661   self.args.R, Fa
+0000f540: 6c73 652c 2064 7572 290a 2020 2020 2020  lse, dur).      
+0000f550: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
+0000f560: 7574 5f68 6561 6465 726c 6973 742e 6170  ut_headerlist.ap
+0000f570: 7065 6e64 2828 2253 6574 2d43 6f6f 6b69  pend(("Set-Cooki
+0000f580: 6522 2c20 636b 2929 0a20 2020 2020 2020  e", ck)).       
+0000f590: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000f5a0: 2020 206b 203d 2022 6370 7077 7322 2069     k = "cppws" i
+0000f5b0: 6620 7365 6c66 2e69 735f 6874 7470 7320  f self.is_https 
+0000f5c0: 656c 7365 2022 6370 7077 6422 0a20 2020  else "cppwd".   
+0000f5d0: 2020 2020 2020 2020 2063 6b20 3d20 6765           ck = ge
+0000f5e0: 6e63 6f6f 6b69 6528 6b2c 2070 7764 2c20  ncookie(k, pwd, 
+0000f5f0: 7365 6c66 2e61 7267 732e 522c 2073 656c  self.args.R, sel
+0000f600: 662e 6973 5f68 7474 7073 2c20 6475 7229  f.is_https, dur)
+0000f610: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f620: 662e 6f75 745f 6865 6164 6572 6c69 7374  f.out_headerlist
+0000f630: 2e61 7070 656e 6428 2822 5365 742d 436f  .append(("Set-Co
+0000f640: 6f6b 6965 222c 2063 6b29 290a 0a20 2020  okie", ck))..   
+0000f650: 2020 2020 2072 6574 7572 6e20 6d73 670a       return msg.
+0000f660: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
+0000f670: 6d6b 6469 7228 7365 6c66 2920 203a 0a20  mkdir(self)  :. 
+0000f680: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+0000f690: 6c66 2e70 6172 7365 720a 2020 2020 2020  lf.parser.      
+0000f6a0: 2020 6e65 775f 6469 7220 3d20 7365 6c66    new_dir = self
+0000f6b0: 2e70 6172 7365 722e 7265 7175 6972 6528  .parser.require(
+0000f6c0: 226e 616d 6522 2c20 3531 3229 0a20 2020  "name", 512).   
+0000f6d0: 2020 2020 2073 656c 662e 7061 7273 6572       self.parser
+0000f6e0: 2e64 726f 7028 290a 0a20 2020 2020 2020  .drop()..       
+0000f6f0: 2073 616e 6974 697a 6564 203d 2073 616e   sanitized = san
+0000f700: 6974 697a 655f 666e 286e 6577 5f64 6972  itize_fn(new_dir
+0000f710: 2c20 2222 2c20 5b5d 290a 2020 2020 2020  , "", []).      
+0000f720: 2020 7265 7475 726e 2073 656c 662e 5f6d    return self._m
+0000f730: 6b64 6972 2876 6a6f 696e 2873 656c 662e  kdir(vjoin(self.
+0000f740: 7670 6174 682c 2073 616e 6974 697a 6564  vpath, sanitized
+0000f750: 2929 0a0a 2020 2020 6465 6620 5f6d 6b64  ))..    def _mkd
+0000f760: 6972 2873 656c 662c 2076 7061 7468 2029  ir(self, vpath )
+0000f770: 2020 3a0a 2020 2020 2020 2020 6e75 6c6c    :.        null
+0000f780: 7772 6974 6520 3d20 7365 6c66 2e61 7267  write = self.arg
+0000f790: 732e 6e77 0a20 2020 2020 2020 2076 6673  s.nw.        vfs
+0000f7a0: 2c20 7265 6d20 3d20 7365 6c66 2e61 7372  , rem = self.asr
+0000f7b0: 762e 7666 732e 6765 7428 7670 6174 682c  v.vfs.get(vpath,
+0000f7c0: 2073 656c 662e 756e 616d 652c 2046 616c   self.uname, Fal
+0000f7d0: 7365 2c20 5472 7565 290a 2020 2020 2020  se, True).      
+0000f7e0: 2020 7365 6c66 2e5f 6173 7365 7274 5f73    self._assert_s
+0000f7f0: 6166 655f 7265 6d28 7265 6d29 0a20 2020  afe_rem(rem).   
+0000f800: 2020 2020 2066 6e20 3d20 7666 732e 6361       fn = vfs.ca
+0000f810: 6e6f 6e69 6361 6c28 7265 6d29 0a0a 2020  nonical(rem)..  
+0000f820: 2020 2020 2020 6966 206e 6f74 206e 756c        if not nul
+0000f830: 6c77 7269 7465 3a0a 2020 2020 2020 2020  lwrite:.        
+0000f840: 2020 2020 6664 6972 203d 206f 732e 7061      fdir = os.pa
+0000f850: 7468 2e64 6972 6e61 6d65 2866 6e29 0a0a  th.dirname(fn)..
+0000f860: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000f870: 6f74 2062 6f73 2e70 6174 682e 6973 6469  ot bos.path.isdi
+0000f880: 7228 6664 6972 293a 0a20 2020 2020 2020  r(fdir):.       
+0000f890: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
+0000f8a0: 6562 6b61 6328 3430 392c 2022 7061 7265  ebkac(409, "pare
+0000f8b0: 6e74 2066 6f6c 6465 7220 646f 6573 206e  nt folder does n
+0000f8c0: 6f74 2065 7869 7374 2229 0a0a 2020 2020  ot exist")..    
+0000f8d0: 2020 2020 2020 2020 6966 2062 6f73 2e70          if bos.p
+0000f8e0: 6174 682e 6973 6469 7228 666e 293a 0a20  ath.isdir(fn):. 
+0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000f900: 6169 7365 2050 6562 6b61 6328 3430 352c  aise Pebkac(405,
+0000f910: 2022 7468 6174 2066 6f6c 6465 7220 6578   "that folder ex
+0000f920: 6973 7473 2061 6c72 6561 6479 2229 0a0a  ists already")..
+0000f930: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0000f940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f950: 2062 6f73 2e6d 6b64 6972 2866 6e29 0a20   bos.mkdir(fn). 
+0000f960: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0000f970: 7420 4f53 4572 726f 7220 6173 2065 783a  t OSError as ex:
+0000f980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f990: 2069 6620 6578 2e65 7272 6e6f 203d 3d20   if ex.errno == 
+0000f9a0: 6572 726e 6f2e 4541 4343 4553 3a0a 2020  errno.EACCES:.  
+0000f9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9c0: 2020 7261 6973 6520 5065 626b 6163 2835    raise Pebkac(5
+0000f9d0: 3030 2c20 2274 6865 2073 6572 7665 7220  00, "the server 
+0000f9e0: 4f53 2064 656e 6965 6420 7772 6974 652d  OS denied write-
+0000f9f0: 6163 6365 7373 2229 0a0a 2020 2020 2020  access")..      
+0000fa00: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000fa10: 5065 626b 6163 2835 3030 2c20 226d 6b64  Pebkac(500, "mkd
+0000fa20: 6972 2066 6169 6c65 643a 5c6e 2220 2b20  ir failed:\n" + 
+0000fa30: 6d69 6e5f 6578 2829 290a 2020 2020 2020  min_ex()).      
+0000fa40: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+0000fa50: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000fa60: 6973 6520 5065 626b 6163 2835 3030 2c20  ise Pebkac(500, 
+0000fa70: 6d69 6e5f 6578 2829 290a 0a20 2020 2020  min_ex())..     
+0000fa80: 2020 2073 656c 662e 6f75 745f 6865 6164     self.out_head
+0000fa90: 6572 735b 2258 2d4e 6577 2d44 6972 225d  ers["X-New-Dir"]
+0000faa0: 203d 2071 756f 7465 7028 7670 6174 682e   = quotep(vpath.
+0000fab0: 7370 6c69 7428 222f 2229 5b2d 315d 290a  split("/")[-1]).
+0000fac0: 2020 2020 2020 2020 7365 6c66 2e72 6564          self.red
+0000fad0: 6972 6563 7428 7670 6174 682c 2073 7461  irect(vpath, sta
+0000fae0: 7475 733d 3230 3129 0a20 2020 2020 2020  tus=201).       
+0000faf0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
+0000fb00: 2020 6465 6620 6861 6e64 6c65 5f6e 6577    def handle_new
+0000fb10: 5f6d 6428 7365 6c66 2920 203a 0a20 2020  _md(self)  :.   
+0000fb20: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+0000fb30: 2e70 6172 7365 720a 2020 2020 2020 2020  .parser.        
+0000fb40: 6e65 775f 6669 6c65 203d 2073 656c 662e  new_file = self.
+0000fb50: 7061 7273 6572 2e72 6571 7569 7265 2822  parser.require("
+0000fb60: 6e61 6d65 222c 2035 3132 290a 2020 2020  name", 512).    
+0000fb70: 2020 2020 7365 6c66 2e70 6172 7365 722e      self.parser.
+0000fb80: 6472 6f70 2829 0a0a 2020 2020 2020 2020  drop()..        
+0000fb90: 6e75 6c6c 7772 6974 6520 3d20 7365 6c66  nullwrite = self
+0000fba0: 2e61 7267 732e 6e77 0a20 2020 2020 2020  .args.nw.       
+0000fbb0: 2076 6673 2c20 7265 6d20 3d20 7365 6c66   vfs, rem = self
+0000fbc0: 2e61 7372 762e 7666 732e 6765 7428 7365  .asrv.vfs.get(se
+0000fbd0: 6c66 2e76 7061 7468 2c20 7365 6c66 2e75  lf.vpath, self.u
+0000fbe0: 6e61 6d65 2c20 4661 6c73 652c 2054 7275  name, False, Tru
+0000fbf0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+0000fc00: 5f61 7373 6572 745f 7361 6665 5f72 656d  _assert_safe_rem
+0000fc10: 2872 656d 290a 0a20 2020 2020 2020 2069  (rem)..        i
+0000fc20: 6620 6e6f 7420 6e65 775f 6669 6c65 2e65  f not new_file.e
+0000fc30: 6e64 7377 6974 6828 222e 6d64 2229 3a0a  ndswith(".md"):.
+0000fc40: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000fc50: 6669 6c65 202b 3d20 222e 6d64 220a 0a20  file += ".md".. 
+0000fc60: 2020 2020 2020 2073 616e 6974 697a 6564         sanitized
+0000fc70: 203d 2073 616e 6974 697a 655f 666e 286e   = sanitize_fn(n
+0000fc80: 6577 5f66 696c 652c 2022 222c 205b 5d29  ew_file, "", [])
+0000fc90: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+0000fca0: 206e 756c 6c77 7269 7465 3a0a 2020 2020   nullwrite:.    
+0000fcb0: 2020 2020 2020 2020 6664 6972 203d 2076          fdir = v
+0000fcc0: 6673 2e63 616e 6f6e 6963 616c 2872 656d  fs.canonical(rem
+0000fcd0: 290a 2020 2020 2020 2020 2020 2020 666e  ).            fn
+0000fce0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+0000fcf0: 6664 6972 2c20 7361 6e69 7469 7a65 6429  fdir, sanitized)
+0000fd00: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000fd10: 2062 6f73 2e70 6174 682e 6578 6973 7473   bos.path.exists
+0000fd20: 2866 6e29 3a0a 2020 2020 2020 2020 2020  (fn):.          
+0000fd30: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
+0000fd40: 6163 2835 3030 2c20 2274 6861 7420 6669  ac(500, "that fi
+0000fd50: 6c65 2065 7869 7374 7320 616c 7265 6164  le exists alread
+0000fd60: 7922 290a 0a20 2020 2020 2020 2020 2020  y")..           
+0000fd70: 2077 6974 6820 6f70 656e 2866 7365 6e63   with open(fsenc
+0000fd80: 2866 6e29 2c20 2277 6222 2920 6173 2066  (fn), "wb") as f
+0000fd90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fda0: 2020 662e 7772 6974 6528 6222 6047 5255    f.write(b"`GRU
+0000fdb0: 4e4e 5552 605c 6e22 290a 0a20 2020 2020  NNUR`\n")..     
+0000fdc0: 2020 2076 7061 7468 203d 2022 7b7d 2f7b     vpath = "{}/{
+0000fdd0: 7d22 2e66 6f72 6d61 7428 7365 6c66 2e76  }".format(self.v
+0000fde0: 7061 7468 2c20 7361 6e69 7469 7a65 6429  path, sanitized)
+0000fdf0: 2e6c 7374 7269 7028 222f 2229 0a20 2020  .lstrip("/").   
+0000fe00: 2020 2020 2073 656c 662e 7265 6469 7265       self.redire
+0000fe10: 6374 2876 7061 7468 2c20 223f 6564 6974  ct(vpath, "?edit
+0000fe20: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+0000fe30: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
+0000fe40: 7570 6c6f 6164 5f66 6c61 6773 2873 656c  upload_flags(sel
+0000fe50: 662c 2076 6673 2029 2020 2020 2020 3a0a  f, vfs )      :.
+0000fe60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000fe70: 6172 6773 2e6e 773a 0a20 2020 2020 2020  args.nw:.       
+0000fe80: 2020 2020 2072 6e64 203d 2030 0a20 2020       rnd = 0.   
+0000fe90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000fea0: 2020 2020 2020 2072 6e64 203d 2069 6e74         rnd = int
+0000feb0: 2873 656c 662e 7570 6172 616d 2e67 6574  (self.uparam.get
+0000fec0: 2822 7261 6e64 2229 206f 7220 7365 6c66  ("rand") or self
+0000fed0: 2e68 6561 6465 7273 2e67 6574 2822 7261  .headers.get("ra
+0000fee0: 6e64 2229 206f 7220 3029 0a20 2020 2020  nd") or 0).     
+0000fef0: 2020 2020 2020 2069 6620 7666 732e 666c         if vfs.fl
+0000ff00: 6167 732e 6765 7428 2272 616e 6422 293a  ags.get("rand"):
+0000ff10: 2020 2320 666f 7263 652d 656e 6162 6c65    # force-enable
+0000ff20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ff30: 2072 6e64 203d 206d 6178 2872 6e64 2c20   rnd = max(rnd, 
+0000ff40: 7666 732e 666c 6167 735b 226e 7261 6e64  vfs.flags["nrand
+0000ff50: 225d 290a 0a20 2020 2020 2020 2061 6320  "])..        ac 
+0000ff60: 3d20 7365 6c66 2e75 7061 7261 6d2e 6765  = self.uparam.ge
+0000ff70: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
+0000ff80: 7761 6e74 222c 2073 656c 662e 6865 6164  want", self.head
+0000ff90: 6572 732e 6765 7428 2261 6363 6570 7422  ers.get("accept"
+0000ffa0: 2c20 2222 292e 6c6f 7765 7228 292e 7370  , "").lower().sp
+0000ffb0: 6c69 7428 223b 2229 5b2d 315d 0a20 2020  lit(";")[-1].   
+0000ffc0: 2020 2020 2029 0a20 2020 2020 2020 2077       ).        w
+0000ffd0: 616e 745f 7572 6c20 3d20 6163 203d 3d20  ant_url = ac == 
+0000ffe0: 2275 726c 220a 2020 2020 2020 2020 7a73  "url".        zs
+0000fff0: 203d 2073 656c 662e 7570 6172 616d 2e67   = self.uparam.g
+00010000: 6574 2822 6c69 6665 222c 2073 656c 662e  et("life", self.
+00010010: 6865 6164 6572 732e 6765 7428 226c 6966  headers.get("lif
+00010020: 6522 2c20 2222 2929 0a20 2020 2020 2020  e", "")).       
+00010030: 2069 6620 7a73 3a0a 2020 2020 2020 2020   if zs:.        
+00010040: 2020 2020 766c 6966 6520 3d20 7666 732e      vlife = vfs.
+00010050: 666c 6167 732e 6765 7428 226c 6966 6574  flags.get("lifet
+00010060: 696d 6522 2920 6f72 2030 0a20 2020 2020  ime") or 0.     
+00010070: 2020 2020 2020 206c 6966 6574 696d 6520         lifetime 
+00010080: 3d20 6d61 7828 302c 2069 6e74 2876 6c69  = max(0, int(vli
+00010090: 6665 202d 2069 6e74 287a 7329 2929 0a20  fe - int(zs))). 
+000100a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000100b0: 2020 2020 2020 2020 206c 6966 6574 696d           lifetim
+000100c0: 6520 3d20 300a 0a20 2020 2020 2020 2072  e = 0..        r
+000100d0: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
+000100e0: 2020 2020 726e 642c 0a20 2020 2020 2020      rnd,.       
+000100f0: 2020 2020 2077 616e 745f 7572 6c2c 0a20       want_url,. 
+00010100: 2020 2020 2020 2020 2020 206c 6966 6574             lifet
+00010110: 696d 652c 0a20 2020 2020 2020 2020 2020  ime,.           
+00010120: 2076 6673 2e66 6c61 6773 2e67 6574 2822   vfs.flags.get("
+00010130: 7862 7522 2920 6f72 205b 5d2c 0a20 2020  xbu") or [],.   
+00010140: 2020 2020 2020 2020 2076 6673 2e66 6c61           vfs.fla
+00010150: 6773 2e67 6574 2822 7861 7522 2920 6f72  gs.get("xau") or
+00010160: 205b 5d2c 0a20 2020 2020 2020 2029 0a0a   [],.        )..
+00010170: 2020 2020 6465 6620 6861 6e64 6c65 5f70      def handle_p
+00010180: 6c61 696e 5f75 706c 6f61 6428 7365 6c66  lain_upload(self
+00010190: 2920 203a 0a20 2020 2020 2020 2061 7373  )  :.        ass
+000101a0: 6572 7420 7365 6c66 2e70 6172 7365 720a  ert self.parser.
+000101b0: 2020 2020 2020 2020 6e75 6c6c 7772 6974          nullwrit
+000101c0: 6520 3d20 7365 6c66 2e61 7267 732e 6e77  e = self.args.nw
+000101d0: 0a20 2020 2020 2020 2076 6673 2c20 7265  .        vfs, re
+000101e0: 6d20 3d20 7365 6c66 2e61 7372 762e 7666  m = self.asrv.vf
+000101f0: 732e 6765 7428 7365 6c66 2e76 7061 7468  s.get(self.vpath
+00010200: 2c20 7365 6c66 2e75 6e61 6d65 2c20 4661  , self.uname, Fa
+00010210: 6c73 652c 2054 7275 6529 0a20 2020 2020  lse, True).     
+00010220: 2020 2073 656c 662e 5f61 7373 6572 745f     self._assert_
+00010230: 7361 6665 5f72 656d 2872 656d 290a 0a20  safe_rem(rem).. 
+00010240: 2020 2020 2020 2075 706c 6f61 645f 7670         upload_vp
+00010250: 6174 6820 3d20 7365 6c66 2e76 7061 7468  ath = self.vpath
+00010260: 0a20 2020 2020 2020 206c 696d 203d 2076  .        lim = v
+00010270: 6673 2e67 6574 5f64 6276 2872 656d 295b  fs.get_dbv(rem)[
+00010280: 305d 2e6c 696d 0a20 2020 2020 2020 2066  0].lim.        f
+00010290: 6469 725f 6261 7365 203d 2076 6673 2e63  dir_base = vfs.c
+000102a0: 616e 6f6e 6963 616c 2872 656d 290a 2020  anonical(rem).  
+000102b0: 2020 2020 2020 6966 206c 696d 3a0a 2020        if lim:.  
+000102c0: 2020 2020 2020 2020 2020 6664 6972 5f62            fdir_b
+000102d0: 6173 652c 2072 656d 203d 206c 696d 2e61  ase, rem = lim.a
+000102e0: 6c6c 2873 656c 662e 6970 2c20 7265 6d2c  ll(self.ip, rem,
+000102f0: 202d 312c 2066 6469 725f 6261 7365 290a   -1, fdir_base).
+00010300: 2020 2020 2020 2020 2020 2020 7570 6c6f              uplo
+00010310: 6164 5f76 7061 7468 203d 2022 7b7d 2f7b  ad_vpath = "{}/{
+00010320: 7d22 2e66 6f72 6d61 7428 7666 732e 7670  }".format(vfs.vp
+00010330: 6174 682c 2072 656d 292e 7374 7269 7028  ath, rem).strip(
+00010340: 222f 2229 0a20 2020 2020 2020 2020 2020  "/").           
+00010350: 2069 6620 6e6f 7420 6e75 6c6c 7772 6974   if not nullwrit
+00010360: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00010370: 2020 2062 6f73 2e6d 616b 6564 6972 7328     bos.makedirs(
+00010380: 6664 6972 5f62 6173 6529 0a0a 2020 2020  fdir_base)..    
+00010390: 2020 2020 726e 642c 2077 616e 745f 7572      rnd, want_ur
+000103a0: 6c2c 206c 6966 6574 696d 652c 2078 6275  l, lifetime, xbu
+000103b0: 2c20 7861 7520 3d20 7365 6c66 2e75 706c  , xau = self.upl
+000103c0: 6f61 645f 666c 6167 7328 7666 7329 0a0a  oad_flags(vfs)..
+000103d0: 2020 2020 2020 2020 6669 6c65 7320 2020          files   
+000103e0: 2020 2020 3d20 5b5d 0a20 2020 2020 2020      = [].       
+000103f0: 2023 2073 7a2c 2073 6861 5f68 6578 2c20   # sz, sha_hex, 
+00010400: 7368 615f 6236 342c 2070 5f66 696c 652c  sha_b64, p_file,
+00010410: 2066 6e61 6d65 2c20 6162 7370 6174 680a   fname, abspath.
+00010420: 2020 2020 2020 2020 6572 726d 7367 203d          errmsg =
+00010430: 2022 220a 2020 2020 2020 2020 6469 7020   "".        dip 
+00010440: 3d20 7365 6c66 2e64 6970 2829 0a20 2020  = self.dip().   
+00010450: 2020 2020 2074 3020 3d20 7469 6d65 2e74       t0 = time.t
+00010460: 696d 6528 290a 2020 2020 2020 2020 7472  ime().        tr
+00010470: 793a 0a20 2020 2020 2020 2020 2020 2061  y:.            a
+00010480: 7373 6572 7420 7365 6c66 2e70 6172 7365  ssert self.parse
+00010490: 722e 6765 6e0a 2020 2020 2020 2020 2020  r.gen.          
+000104a0: 2020 666f 7220 6e66 696c 652c 2028 705f    for nfile, (p_
+000104b0: 6669 656c 642c 2070 5f66 696c 652c 2070  field, p_file, p
+000104c0: 5f64 6174 6129 2069 6e20 656e 756d 6572  _data) in enumer
+000104d0: 6174 6528 7365 6c66 2e70 6172 7365 722e  ate(self.parser.
+000104e0: 6765 6e29 3a0a 2020 2020 2020 2020 2020  gen):.          
+000104f0: 2020 2020 2020 6966 206e 6f74 2070 5f66        if not p_f
+00010500: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
+00010510: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+00010520: 6728 2264 6973 6361 7264 696e 6720 696e  g("discarding in
+00010530: 636f 6d69 6e67 2066 696c 6520 7769 7468  coming file with
+00010540: 6f75 7420 6669 6c65 6e61 6d65 2229 0a20  out filename"). 
+00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010560: 2020 2023 2066 616c 6c74 6872 6f75 6768     # fallthrough
+00010570: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010580: 2020 6664 6972 203d 2066 6469 725f 6261    fdir = fdir_ba
+00010590: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+000105a0: 2020 2066 6e61 6d65 203d 2073 616e 6974     fname = sanit
+000105b0: 697a 655f 666e 280a 2020 2020 2020 2020  ize_fn(.        
+000105c0: 2020 2020 2020 2020 2020 2020 705f 6669              p_fi
+000105d0: 6c65 206f 7220 2222 2c20 2222 2c20 5b22  le or "", "", ["
+000105e0: 2e70 726f 6c6f 6775 652e 6874 6d6c 222c  .prologue.html",
+000105f0: 2022 2e65 7069 6c6f 6775 652e 6874 6d6c   ".epilogue.html
+00010600: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00010610: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00010620: 2020 2020 2069 6620 705f 6669 6c65 2061       if p_file a
+00010630: 6e64 206e 6f74 206e 756c 6c77 7269 7465  nd not nullwrite
+00010640: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010650: 2020 2020 2020 6966 2072 6e64 3a0a 2020        if rnd:.  
 00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010670: 2020 6966 206e 6f74 2062 6f73 2e70 6174    if not bos.pat
-00010680: 682e 6973 6469 7228 6664 6972 293a 0a20  h.isdir(fdir):. 
-00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106a0: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
-000106b0: 6b61 6328 3430 342c 2022 7468 6174 2066  kac(404, "that f
-000106c0: 6f6c 6465 7220 646f 6573 206e 6f74 2065  older does not e
-000106d0: 7869 7374 2229 0a0a 2020 2020 2020 2020  xist")..        
-000106e0: 2020 2020 2020 2020 2020 2020 7375 6666              suff
-000106f0: 6978 203d 2022 2d7b 3a2e 3666 7d2d 7b7d  ix = "-{:.6f}-{}
-00010700: 222e 666f 726d 6174 2874 696d 652e 7469  ".format(time.ti
-00010710: 6d65 2829 2c20 6469 7029 0a20 2020 2020  me(), dip).     
-00010720: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00010730: 7065 6e5f 6172 6773 203d 207b 2266 6469  pen_args = {"fdi
-00010740: 7222 3a20 6664 6972 2c20 2273 7566 6669  r": fdir, "suffi
-00010750: 7822 3a20 7375 6666 6978 7d0a 0a20 2020  x": suffix}..   
-00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010770: 2023 2072 6573 6572 7665 2064 6573 7469   # reserve desti
-00010780: 6e61 7469 6f6e 2066 696c 656e 616d 650a  nation filename.
-00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107a0: 2020 2020 7769 7468 2072 656e 5f6f 7065      with ren_ope
-000107b0: 6e28 666e 616d 652c 2022 7762 222c 2066  n(fname, "wb", f
-000107c0: 6469 723d 6664 6972 2c20 7375 6666 6978  dir=fdir, suffix
-000107d0: 3d73 7566 6669 7829 2061 7320 7a66 773a  =suffix) as zfw:
-000107e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000107f0: 2020 2020 2020 2020 2066 6e61 6d65 203d           fname =
-00010800: 207a 6677 5b22 6f72 7a22 5d5b 315d 0a0a   zfw["orz"][1]..
-00010810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010820: 2020 2020 746e 616d 203d 2066 6e61 6d65      tnam = fname
-00010830: 202b 2022 2e50 4152 5449 414c 220a 2020   + ".PARTIAL".  
-00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010850: 2020 6966 2073 656c 662e 6172 6773 2e64    if self.args.d
-00010860: 6f74 7061 7274 3a0a 2020 2020 2020 2020  otpart:.        
-00010870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010880: 746e 616d 203d 2022 2e22 202b 2074 6e61  tnam = "." + tna
-00010890: 6d0a 0a20 2020 2020 2020 2020 2020 2020  m..             
-000108a0: 2020 2020 2020 2061 6273 7061 7468 203d         abspath =
-000108b0: 206f 732e 7061 7468 2e6a 6f69 6e28 6664   os.path.join(fd
-000108c0: 6972 2c20 666e 616d 6529 0a20 2020 2020  ir, fname).     
-000108d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000108e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000108f0: 2020 2020 206f 7065 6e5f 6172 6773 203d       open_args =
-00010900: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-00010910: 2020 2020 2020 2020 746e 616d 203d 2066          tnam = f
-00010920: 6e61 6d65 203d 206f 732e 6465 766e 756c  name = os.devnul
-00010930: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
-00010940: 2020 2020 2020 6664 6972 203d 2061 6273        fdir = abs
-00010950: 7061 7468 203d 2022 220a 0a20 2020 2020  path = ""..     
-00010960: 2020 2020 2020 2020 2020 2069 6620 7862             if xb
-00010970: 753a 0a20 2020 2020 2020 2020 2020 2020  u:.             
-00010980: 2020 2020 2020 2061 7420 3d20 7469 6d65         at = time
-00010990: 2e74 696d 6528 2920 2d20 6c69 6665 7469  .time() - lifeti
-000109a0: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
-000109b0: 2020 2020 2020 2069 6620 6e6f 7420 7275         if not ru
-000109c0: 6e68 6f6f 6b28 0a20 2020 2020 2020 2020  nhook(.         
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000109e0: 656c 662e 6c6f 672c 0a20 2020 2020 2020  elf.log,.       
-000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a00: 2078 6275 2c0a 2020 2020 2020 2020 2020   xbu,.          
-00010a10: 2020 2020 2020 2020 2020 2020 2020 6162                ab
-00010a20: 7370 6174 682c 0a20 2020 2020 2020 2020  spath,.         
-00010a30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010a40: 656c 662e 7670 6174 682c 0a20 2020 2020  elf.vpath,.     
-00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a60: 2020 2073 656c 662e 686f 7374 2c0a 2020     self.host,.  
-00010a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a80: 2020 2020 2020 7365 6c66 2e75 6e61 6d65        self.uname
-00010a90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010aa0: 2020 2020 2020 2020 2020 6174 2c0a 2020            at,.  
+00010670: 2020 2020 2020 666e 616d 6520 3d20 7261        fname = ra
+00010680: 6e64 5f6e 616d 6528 6664 6972 2c20 666e  nd_name(fdir, fn
+00010690: 616d 652c 2072 6e64 290a 0a20 2020 2020  ame, rnd)..     
+000106a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000106b0: 6620 6e6f 7420 626f 732e 7061 7468 2e69  f not bos.path.i
+000106c0: 7364 6972 2866 6469 7229 3a0a 2020 2020  sdir(fdir):.    
+000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106e0: 2020 2020 7261 6973 6520 5065 626b 6163      raise Pebkac
+000106f0: 2834 3034 2c20 2274 6861 7420 666f 6c64  (404, "that fold
+00010700: 6572 2064 6f65 7320 6e6f 7420 6578 6973  er does not exis
+00010710: 7422 290a 0a20 2020 2020 2020 2020 2020  t")..           
+00010720: 2020 2020 2020 2020 2073 7566 6669 7820           suffix 
+00010730: 3d20 222d 7b3a 2e36 667d 2d7b 7d22 2e66  = "-{:.6f}-{}".f
+00010740: 6f72 6d61 7428 7469 6d65 2e74 696d 6528  ormat(time.time(
+00010750: 292c 2064 6970 290a 2020 2020 2020 2020  ), dip).        
+00010760: 2020 2020 2020 2020 2020 2020 6f70 656e              open
+00010770: 5f61 7267 7320 3d20 7b22 6664 6972 223a  _args = {"fdir":
+00010780: 2066 6469 722c 2022 7375 6666 6978 223a   fdir, "suffix":
+00010790: 2073 7566 6669 787d 0a0a 2020 2020 2020   suffix}..      
+000107a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000107b0: 7265 7365 7276 6520 6465 7374 696e 6174  reserve destinat
+000107c0: 696f 6e20 6669 6c65 6e61 6d65 0a20 2020  ion filename.   
+000107d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107e0: 2077 6974 6820 7265 6e5f 6f70 656e 2866   with ren_open(f
+000107f0: 6e61 6d65 2c20 2277 6222 2c20 6664 6972  name, "wb", fdir
+00010800: 3d66 6469 722c 2073 7566 6669 783d 7375  =fdir, suffix=su
+00010810: 6666 6978 2920 6173 207a 6677 3a0a 2020  ffix) as zfw:.  
+00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010830: 2020 2020 2020 666e 616d 6520 3d20 7a66        fname = zf
+00010840: 775b 226f 727a 225d 5b31 5d0a 0a20 2020  w["orz"][1]..   
+00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010860: 2074 6e61 6d20 3d20 666e 616d 6520 2b20   tnam = fname + 
+00010870: 222e 5041 5254 4941 4c22 0a20 2020 2020  ".PARTIAL".     
+00010880: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010890: 6620 7365 6c66 2e61 7267 732e 646f 7470  f self.args.dotp
+000108a0: 6172 743a 0a20 2020 2020 2020 2020 2020  art:.           
+000108b0: 2020 2020 2020 2020 2020 2020 2074 6e61               tna
+000108c0: 6d20 3d20 222e 2220 2b20 746e 616d 0a0a  m = "." + tnam..
+000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108e0: 2020 2020 6162 7370 6174 6820 3d20 6f73      abspath = os
+000108f0: 2e70 6174 682e 6a6f 696e 2866 6469 722c  .path.join(fdir,
+00010900: 2066 6e61 6d65 290a 2020 2020 2020 2020   fname).        
+00010910: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010930: 2020 6f70 656e 5f61 7267 7320 3d20 7b7d    open_args = {}
+00010940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010950: 2020 2020 2074 6e61 6d20 3d20 666e 616d       tnam = fnam
+00010960: 6520 3d20 6f73 2e64 6576 6e75 6c6c 0a20  e = os.devnull. 
+00010970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010980: 2020 2066 6469 7220 3d20 6162 7370 6174     fdir = abspat
+00010990: 6820 3d20 2222 0a0a 2020 2020 2020 2020  h = ""..        
+000109a0: 2020 2020 2020 2020 6966 2078 6275 3a0a          if xbu:.
+000109b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109c0: 2020 2020 6174 203d 2074 696d 652e 7469      at = time.ti
+000109d0: 6d65 2829 202d 206c 6966 6574 696d 650a  me() - lifetime.
+000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109f0: 2020 2020 6966 206e 6f74 2072 756e 686f      if not runho
+00010a00: 6f6b 280a 2020 2020 2020 2020 2020 2020  ok(.            
+00010a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010a20: 2e6c 6f67 2c0a 2020 2020 2020 2020 2020  .log,.          
+00010a30: 2020 2020 2020 2020 2020 2020 2020 7862                xb
+00010a40: 752c 0a20 2020 2020 2020 2020 2020 2020  u,.             
+00010a50: 2020 2020 2020 2020 2020 2061 6273 7061             abspa
+00010a60: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00010a70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010a80: 2e76 7061 7468 2c0a 2020 2020 2020 2020  .vpath,.        
+00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010aa0: 7365 6c66 2e68 6f73 742c 0a20 2020 2020  self.host,.     
 00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ac0: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
+00010ac0: 2020 2073 656c 662e 756e 616d 652c 0a20     self.uname,. 
 00010ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ae0: 2073 656c 662e 6970 2c0a 2020 2020 2020   self.ip,.      
+00010ae0: 2020 2020 2020 2061 742c 0a20 2020 2020         at,.     
 00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b00: 2020 6174 2c0a 2020 2020 2020 2020 2020    at,.          
-00010b10: 2020 2020 2020 2020 2020 2020 2020 2222                ""
-00010b20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010b30: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b50: 2074 203d 2022 7570 6c6f 6164 2062 6c6f   t = "upload blo
-00010b60: 636b 6564 2062 7920 7862 7520 7365 7276  cked by xbu serv
-00010b70: 6572 2063 6f6e 6669 6722 0a20 2020 2020  er config".     
-00010b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b90: 2020 2073 656c 662e 6c6f 6728 742c 2031     self.log(t, 1
-00010ba0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010bb0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00010bc0: 5065 626b 6163 2834 3033 2c20 7429 0a0a  Pebkac(403, t)..
-00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010be0: 6966 206c 696d 3a0a 2020 2020 2020 2020  if lim:.        
-00010bf0: 2020 2020 2020 2020 2020 2020 6c69 6d2e              lim.
-00010c00: 6368 6b5f 6275 7028 7365 6c66 2e69 7029  chk_bup(self.ip)
-00010c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010c20: 2020 2020 206c 696d 2e63 686b 5f6e 7570       lim.chk_nup
-00010c30: 2873 656c 662e 6970 290a 0a20 2020 2020  (self.ip)..     
-00010c40: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00010b00: 2020 2030 2c0a 2020 2020 2020 2020 2020     0,.          
+00010b10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010b20: 6c66 2e69 702c 0a20 2020 2020 2020 2020  lf.ip,.         
+00010b30: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00010b40: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00010b50: 2020 2020 2020 2020 2020 2022 222c 0a20             "",. 
+00010b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b70: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00010b80: 2020 2020 2020 2020 2020 2020 2020 7420                t 
+00010b90: 3d20 2275 706c 6f61 6420 626c 6f63 6b65  = "upload blocke
+00010ba0: 6420 6279 2078 6275 2073 6572 7665 7220  d by xbu server 
+00010bb0: 636f 6e66 6967 220a 2020 2020 2020 2020  config".        
+00010bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bd0: 7365 6c66 2e6c 6f67 2874 2c20 3129 0a20  self.log(t, 1). 
+00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bf0: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
+00010c00: 6b61 6328 3430 332c 2074 290a 0a20 2020  kac(403, t)..   
+00010c10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010c20: 6c69 6d3a 0a20 2020 2020 2020 2020 2020  lim:.           
+00010c30: 2020 2020 2020 2020 206c 696d 2e63 686b           lim.chk
+00010c40: 5f62 7570 2873 656c 662e 6970 290a 2020  _bup(self.ip).  
 00010c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c60: 2020 2020 6d61 785f 737a 203d 2030 0a20      max_sz = 0. 
-00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c80: 2020 2069 6620 6c69 6d3a 0a20 2020 2020     if lim:.     
+00010c60: 2020 6c69 6d2e 6368 6b5f 6e75 7028 7365    lim.chk_nup(se
+00010c70: 6c66 2e69 7029 0a0a 2020 2020 2020 2020  lf.ip)..        
+00010c80: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
 00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ca0: 2020 2076 3120 3d20 6c69 6d2e 736d 6178     v1 = lim.smax
-00010cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010cc0: 2020 2020 2020 2020 2076 3220 3d20 6c69           v2 = li
-00010cd0: 6d2e 6466 7620 2d20 6c69 6d2e 6466 6c0a  m.dfv - lim.dfl.
-00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cf0: 2020 2020 2020 2020 6d61 785f 737a 203d          max_sz =
-00010d00: 206d 696e 2876 312c 2076 3229 2069 6620   min(v1, v2) if 
-00010d10: 7631 2061 6e64 2076 3220 656c 7365 2076  v1 and v2 else v
-00010d20: 3120 6f72 2076 320a 0a20 2020 2020 2020  1 or v2..       
-00010d30: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-00010d40: 6820 7265 6e5f 6f70 656e 2874 6e61 6d2c  h ren_open(tnam,
-00010d50: 2022 7762 222c 2035 3132 202a 2031 3032   "wb", 512 * 102
-00010d60: 342c 202a 2a6f 7065 6e5f 6172 6773 2920  4, **open_args) 
-00010d70: 6173 207a 6677 3a0a 2020 2020 2020 2020  as zfw:.        
-00010d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d90: 662c 2074 6e61 6d20 3d20 7a66 775b 226f  f, tnam = zfw["o
-00010da0: 727a 225d 0a20 2020 2020 2020 2020 2020  rz"].           
-00010db0: 2020 2020 2020 2020 2020 2020 2074 6162               tab
-00010dc0: 7370 6174 6820 3d20 6f73 2e70 6174 682e  spath = os.path.
-00010dd0: 6a6f 696e 2866 6469 722c 2074 6e61 6d29  join(fdir, tnam)
-00010de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010df0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-00010e00: 6728 2277 7269 7469 6e67 2074 6f20 7b7d  g("writing to {}
-00010e10: 222e 666f 726d 6174 2874 6162 7370 6174  ".format(tabspat
-00010e20: 6829 290a 2020 2020 2020 2020 2020 2020  h)).            
-00010e30: 2020 2020 2020 2020 2020 2020 737a 2c20              sz, 
-00010e40: 7368 615f 6865 782c 2073 6861 5f62 3634  sha_hex, sha_b64
-00010e50: 203d 2068 6173 6863 6f70 7928 0a20 2020   = hashcopy(.   
-00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e70: 2020 2020 2020 2020 2070 5f64 6174 612c           p_data,
-00010e80: 2066 2c20 7365 6c66 2e61 7267 732e 735f   f, self.args.s_
-00010e90: 7772 5f73 6c70 2c20 6d61 785f 737a 0a20  wr_slp, max_sz. 
+00010ca0: 206d 6178 5f73 7a20 3d20 300a 2020 2020   max_sz = 0.    
+00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cc0: 6966 206c 696d 3a0a 2020 2020 2020 2020  if lim:.        
+00010cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ce0: 7631 203d 206c 696d 2e73 6d61 780a 2020  v1 = lim.smax.  
+00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d00: 2020 2020 2020 7632 203d 206c 696d 2e64        v2 = lim.d
+00010d10: 6676 202d 206c 696d 2e64 666c 0a20 2020  fv - lim.dfl.   
+00010d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d30: 2020 2020 206d 6178 5f73 7a20 3d20 6d69       max_sz = mi
+00010d40: 6e28 7631 2c20 7632 2920 6966 2076 3120  n(v1, v2) if v1 
+00010d50: 616e 6420 7632 2065 6c73 6520 7631 206f  and v2 else v1 o
+00010d60: 7220 7632 0a0a 2020 2020 2020 2020 2020  r v2..          
+00010d70: 2020 2020 2020 2020 2020 7769 7468 2072            with r
+00010d80: 656e 5f6f 7065 6e28 746e 616d 2c20 2277  en_open(tnam, "w
+00010d90: 6222 2c20 3531 3220 2a20 3130 3234 2c20  b", 512 * 1024, 
+00010da0: 2a2a 6f70 656e 5f61 7267 7329 2061 7320  **open_args) as 
+00010db0: 7a66 773a 0a20 2020 2020 2020 2020 2020  zfw:.           
+00010dc0: 2020 2020 2020 2020 2020 2020 2066 2c20               f, 
+00010dd0: 746e 616d 203d 207a 6677 5b22 6f72 7a22  tnam = zfw["orz"
+00010de0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00010df0: 2020 2020 2020 2020 2020 7461 6273 7061            tabspa
+00010e00: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+00010e10: 6e28 6664 6972 2c20 746e 616d 290a 2020  n(fdir, tnam).  
+00010e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e30: 2020 2020 2020 7365 6c66 2e6c 6f67 2822        self.log("
+00010e40: 7772 6974 696e 6720 746f 207b 7d22 2e66  writing to {}".f
+00010e50: 6f72 6d61 7428 7461 6273 7061 7468 2929  ormat(tabspath))
+00010e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e70: 2020 2020 2020 2020 2073 7a2c 2073 6861           sz, sha
+00010e80: 5f68 6578 2c20 7368 615f 6236 3420 3d20  _hex, sha_b64 = 
+00010e90: 6861 7368 636f 7079 280a 2020 2020 2020  hashcopy(.      
 00010ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010eb0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ed0: 2069 6620 737a 203d 3d20 303a 0a20 2020   if sz == 0:.   
+00010eb0: 2020 2020 2020 705f 6461 7461 2c20 662c        p_data, f,
+00010ec0: 2073 656c 662e 6172 6773 2e73 5f77 725f   self.args.s_wr_
+00010ed0: 736c 702c 206d 6178 5f73 7a0a 2020 2020  slp, max_sz.    
 00010ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ef0: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
-00010f00: 6562 6b61 6328 3430 302c 2022 656d 7074  ebkac(400, "empt
-00010f10: 7920 6669 6c65 7320 696e 2070 6f73 7422  y files in post"
-00010f20: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010f30: 2020 2020 2020 2069 6620 6c69 6d3a 0a20         if lim:. 
-00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f50: 2020 2020 2020 206c 696d 2e6e 7570 2873         lim.nup(s
-00010f60: 656c 662e 6970 290a 2020 2020 2020 2020  elf.ip).        
-00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f80: 6c69 6d2e 6275 7028 7365 6c66 2e69 702c  lim.bup(self.ip,
-00010f90: 2073 7a29 0a20 2020 2020 2020 2020 2020   sz).           
-00010fa0: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00010fb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010fc0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00010fd0: 6d2e 6368 6b5f 6466 2874 6162 7370 6174  m.chk_df(tabspat
-00010fe0: 682c 2073 7a2c 2054 7275 6529 0a20 2020  h, sz, True).   
+00010ef0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00010f00: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00010f10: 2073 7a20 3d3d 2030 3a0a 2020 2020 2020   sz == 0:.      
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
+00010f40: 6163 2834 3030 2c20 2265 6d70 7479 2066  ac(400, "empty f
+00010f50: 696c 6573 2069 6e20 706f 7374 2229 0a0a  iles in post")..
+00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f70: 2020 2020 6966 206c 696d 3a0a 2020 2020      if lim:.    
+00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f90: 2020 2020 6c69 6d2e 6e75 7028 7365 6c66      lim.nup(self
+00010fa0: 2e69 7029 0a20 2020 2020 2020 2020 2020  .ip).           
+00010fb0: 2020 2020 2020 2020 2020 2020 206c 696d               lim
+00010fc0: 2e62 7570 2873 656c 662e 6970 2c20 737a  .bup(self.ip, sz
+00010fd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010fe0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
 00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011000: 2020 2020 2020 2020 206c 696d 2e63 686b           lim.chk
-00011010: 5f73 7a28 737a 290a 2020 2020 2020 2020  _sz(sz).        
-00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011030: 2020 2020 6c69 6d2e 6368 6b5f 6275 7028      lim.chk_bup(
-00011040: 7365 6c66 2e69 7029 0a20 2020 2020 2020  self.ip).       
-00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011060: 2020 2020 206c 696d 2e63 686b 5f6e 7570       lim.chk_nup
-00011070: 2873 656c 662e 6970 290a 2020 2020 2020  (self.ip).      
-00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 2020 2020 2020 6966 206e 6f74 206e 756c        if not nul
-000110c0: 6c77 7269 7465 3a0a 2020 2020 2020 2020  lwrite:.        
-000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110e0: 2020 2020 2020 2020 626f 732e 756e 6c69          bos.unli
-000110f0: 6e6b 2874 6162 7370 6174 6829 0a20 2020  nk(tabspath).   
-00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011110: 2020 2020 2020 2020 2020 2020 2062 6f73               bos
-00011120: 2e75 6e6c 696e 6b28 6162 7370 6174 6829  .unlink(abspath)
-00011130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011140: 2020 2020 2020 2020 2020 2020 2066 6e61               fna
-00011150: 6d65 203d 206f 732e 6465 766e 756c 6c0a  me = os.devnull.
-00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011170: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00011180: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
-00011190: 2020 2020 2020 2069 6620 6e6f 7420 6e75         if not nu
-000111a0: 6c6c 7772 6974 653a 0a20 2020 2020 2020  llwrite:.       
-000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111c0: 2061 746f 6d69 635f 6d6f 7665 2874 6162   atomic_move(tab
-000111d0: 7370 6174 682c 2061 6273 7061 7468 290a  spath, abspath).
-000111e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000111f0: 2020 2020 2066 696c 6573 2e61 7070 656e       files.appen
-00011200: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
-00011210: 2020 2020 2020 2020 2020 2028 737a 2c20             (sz, 
-00011220: 7368 615f 6865 782c 2073 6861 5f62 3634  sha_hex, sha_b64
-00011230: 2c20 705f 6669 6c65 206f 7220 2228 6469  , p_file or "(di
-00011240: 7363 6172 6465 6429 222c 2066 6e61 6d65  scarded)", fname
-00011250: 2c20 6162 7370 6174 6829 0a20 2020 2020  , abspath).     
-00011260: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00011270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011280: 2020 2020 2061 7420 3d20 7469 6d65 2e74       at = time.t
-00011290: 696d 6528 2920 2d20 6c69 6665 7469 6d65  ime() - lifetime
-000112a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000112b0: 2020 2020 2069 6620 7861 7520 616e 6420       if xau and 
-000112c0: 6e6f 7420 7275 6e68 6f6f 6b28 0a20 2020  not runhook(.   
-000112d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112e0: 2020 2020 2073 656c 662e 6c6f 672c 0a20       self.log,. 
-000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011300: 2020 2020 2020 2078 6175 2c0a 2020 2020         xau,.    
+00011000: 2020 2020 2020 2020 2020 206c 696d 2e63             lim.c
+00011010: 686b 5f64 6628 7461 6273 7061 7468 2c20  hk_df(tabspath, 
+00011020: 737a 2c20 5472 7565 290a 2020 2020 2020  sz, True).      
+00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011040: 2020 2020 2020 6c69 6d2e 6368 6b5f 737a        lim.chk_sz
+00011050: 2873 7a29 0a20 2020 2020 2020 2020 2020  (sz).           
+00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011070: 206c 696d 2e63 686b 5f62 7570 2873 656c   lim.chk_bup(sel
+00011080: 662e 6970 290a 2020 2020 2020 2020 2020  f.ip).          
+00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110a0: 2020 6c69 6d2e 6368 6b5f 6e75 7028 7365    lim.chk_nup(se
+000110b0: 6c66 2e69 7029 0a20 2020 2020 2020 2020  lf.ip).         
+000110c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000110d0: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110f0: 2020 2069 6620 6e6f 7420 6e75 6c6c 7772     if not nullwr
+00011100: 6974 653a 0a20 2020 2020 2020 2020 2020  ite:.           
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011120: 2020 2020 2062 6f73 2e75 6e6c 696e 6b28       bos.unlink(
+00011130: 7461 6273 7061 7468 290a 2020 2020 2020  tabspath).      
+00011140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011150: 2020 2020 2020 2020 2020 626f 732e 756e            bos.un
+00011160: 6c69 6e6b 2861 6273 7061 7468 290a 2020  link(abspath).  
+00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011180: 2020 2020 2020 2020 2020 666e 616d 6520            fname 
+00011190: 3d20 6f73 2e64 6576 6e75 6c6c 0a20 2020  = os.devnull.   
+000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111b0: 2020 2020 2020 2020 2072 6169 7365 0a0a           raise..
+000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111d0: 2020 2020 6966 206e 6f74 206e 756c 6c77      if not nullw
+000111e0: 7269 7465 3a0a 2020 2020 2020 2020 2020  rite:.          
+000111f0: 2020 2020 2020 2020 2020 2020 2020 6174                at
+00011200: 6f6d 6963 5f6d 6f76 6528 7461 6273 7061  omic_move(tabspa
+00011210: 7468 2c20 6162 7370 6174 6829 0a0a 2020  th, abspath)..  
+00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011230: 2020 6669 6c65 732e 6170 7065 6e64 280a    files.append(.
+00011240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011250: 2020 2020 2020 2020 2873 7a2c 2073 6861          (sz, sha
+00011260: 5f68 6578 2c20 7368 615f 6236 342c 2070  _hex, sha_b64, p
+00011270: 5f66 696c 6520 6f72 2022 2864 6973 6361  _file or "(disca
+00011280: 7264 6564 2922 2c20 666e 616d 652c 2061  rded)", fname, a
+00011290: 6273 7061 7468 290a 2020 2020 2020 2020  bspath).        
+000112a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112c0: 2020 6174 203d 2074 696d 652e 7469 6d65    at = time.time
+000112d0: 2829 202d 206c 6966 6574 696d 650a 2020  () - lifetime.  
+000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112f0: 2020 6966 2078 6175 2061 6e64 206e 6f74    if xau and not
+00011300: 2072 756e 686f 6f6b 280a 2020 2020 2020   runhook(.      
 00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011320: 2020 2020 6162 7370 6174 682c 0a20 2020      abspath,.   
+00011320: 2020 7365 6c66 2e6c 6f67 2c0a 2020 2020    self.log,.    
 00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011340: 2020 2020 2073 656c 662e 7670 6174 682c       self.vpath,
-00011350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011360: 2020 2020 2020 2020 2073 656c 662e 686f           self.ho
-00011370: 7374 2c0a 2020 2020 2020 2020 2020 2020  st,.            
-00011380: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011390: 2e75 6e61 6d65 2c0a 2020 2020 2020 2020  .uname,.        
-000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113b0: 6174 2c0a 2020 2020 2020 2020 2020 2020  at,.            
-000113c0: 2020 2020 2020 2020 2020 2020 737a 2c0a              sz,.
-000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113e0: 2020 2020 2020 2020 7365 6c66 2e69 702c          self.ip,
+00011340: 2020 2020 7861 752c 0a20 2020 2020 2020      xau,.       
+00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011360: 2061 6273 7061 7468 2c0a 2020 2020 2020   abspath,.      
+00011370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011380: 2020 7365 6c66 2e76 7061 7468 2c0a 2020    self.vpath,.  
+00011390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113a0: 2020 2020 2020 7365 6c66 2e68 6f73 742c        self.host,
+000113b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000113c0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000113d0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+000113e0: 2020 2020 2020 2020 2020 2020 2061 742c               at,
 000113f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011400: 2020 2020 2020 2020 2061 742c 0a20 2020           at,.   
+00011400: 2020 2020 2020 2020 2073 7a2c 0a20 2020           sz,.   
 00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011420: 2020 2020 2022 222c 0a20 2020 2020 2020       "",.       
-00011430: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
-00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011450: 2020 2020 2020 2020 7420 3d20 2275 706c          t = "upl
-00011460: 6f61 6420 626c 6f63 6b65 6420 6279 2078  oad blocked by x
-00011470: 6175 2073 6572 7665 7220 636f 6e66 6967  au server config
-00011480: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00011490: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-000114a0: 6f67 2874 2c20 3129 0a20 2020 2020 2020  og(t, 1).       
-000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114c0: 206f 732e 756e 6c69 6e6b 2861 6273 7061   os.unlink(abspa
-000114d0: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
-000114e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000114f0: 6520 5065 626b 6163 2834 3033 2c20 7429  e Pebkac(403, t)
-00011500: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011510: 2020 2020 2020 6462 762c 2076 7265 6d20        dbv, vrem 
-00011520: 3d20 7666 732e 6765 745f 6462 7628 7265  = vfs.get_dbv(re
-00011530: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
-00011540: 2020 2020 2020 2073 656c 662e 636f 6e6e         self.conn
-00011550: 2e68 7372 762e 6272 6f6b 6572 2e73 6179  .hsrv.broker.say
-00011560: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00011570: 2020 2020 2020 2020 2020 2275 7032 6b2e            "up2k.
-00011580: 6861 7368 5f66 696c 6522 2c0a 2020 2020  hash_file",.    
-00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115a0: 2020 2020 6462 762e 7265 616c 7061 7468      dbv.realpath
-000115b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000115c0: 2020 2020 2020 2020 2020 7666 732e 7670            vfs.vp
-000115d0: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
-000115e0: 2020 2020 2020 2020 2020 2020 2064 6276               dbv
-000115f0: 2e66 6c61 6773 2c0a 2020 2020 2020 2020  .flags,.        
-00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011610: 7672 656d 2c0a 2020 2020 2020 2020 2020  vrem,.          
-00011620: 2020 2020 2020 2020 2020 2020 2020 666e                fn
-00011630: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00011640: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011650: 662e 6970 2c0a 2020 2020 2020 2020 2020  f.ip,.          
-00011660: 2020 2020 2020 2020 2020 2020 2020 6174                at
+00011420: 2020 2020 2073 656c 662e 6970 2c0a 2020       self.ip,.  
+00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 2020 2020 2020 6174 2c0a 2020 2020 2020        at,.      
+00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011460: 2020 2222 2c0a 2020 2020 2020 2020 2020    "",.          
+00011470: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011490: 2020 2020 2074 203d 2022 7570 6c6f 6164       t = "upload
+000114a0: 2062 6c6f 636b 6564 2062 7920 7861 7520   blocked by xau 
+000114b0: 7365 7276 6572 2063 6f6e 6669 6722 0a20  server config". 
+000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114d0: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
+000114e0: 742c 2031 290a 2020 2020 2020 2020 2020  t, 1).          
+000114f0: 2020 2020 2020 2020 2020 2020 2020 6f73                os
+00011500: 2e75 6e6c 696e 6b28 6162 7370 6174 6829  .unlink(abspath)
+00011510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011520: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
+00011530: 6562 6b61 6328 3430 332c 2074 290a 0a20  ebkac(403, t).. 
+00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011550: 2020 2064 6276 2c20 7672 656d 203d 2076     dbv, vrem = v
+00011560: 6673 2e67 6574 5f64 6276 2872 656d 290a  fs.get_dbv(rem).
+00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011580: 2020 2020 7365 6c66 2e63 6f6e 6e2e 6873      self.conn.hs
+00011590: 7276 2e62 726f 6b65 722e 7361 7928 0a20  rv.broker.say(. 
+000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115b0: 2020 2020 2020 2022 7570 326b 2e68 6173         "up2k.has
+000115c0: 685f 6669 6c65 222c 0a20 2020 2020 2020  h_file",.       
+000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115e0: 2064 6276 2e72 6561 6c70 6174 682c 0a20   dbv.realpath,. 
+000115f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011600: 2020 2020 2020 2076 6673 2e76 7061 7468         vfs.vpath
+00011610: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011620: 2020 2020 2020 2020 2020 6462 762e 666c            dbv.fl
+00011630: 6167 732c 0a20 2020 2020 2020 2020 2020  ags,.           
+00011640: 2020 2020 2020 2020 2020 2020 2076 7265               vre
+00011650: 6d2c 0a20 2020 2020 2020 2020 2020 2020  m,.             
+00011660: 2020 2020 2020 2020 2020 2066 6e61 6d65             fname
 00011670: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011680: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00011690: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-000116a0: 2020 2020 2020 2020 2020 2020 2020 5472                Tr
-000116b0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-000116c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000116d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000116e0: 6c66 2e63 6f6e 6e2e 6e62 7974 6520 2b3d  lf.conn.nbyte +=
-000116f0: 2073 7a0a 0a20 2020 2020 2020 2020 2020   sz..           
-00011700: 2020 2020 2065 7863 6570 7420 5065 626b       except Pebk
-00011710: 6163 3a0a 2020 2020 2020 2020 2020 2020  ac:.            
-00011720: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
-00011730: 7365 722e 6472 6f70 2829 0a20 2020 2020  ser.drop().     
-00011740: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011750: 6169 7365 0a0a 2020 2020 2020 2020 6578  aise..        ex
-00011760: 6365 7074 2050 6562 6b61 6320 6173 2065  cept Pebkac as e
-00011770: 783a 0a20 2020 2020 2020 2020 2020 2065  x:.            e
-00011780: 7272 6d73 6720 3d20 766f 6c5f 7361 6e28  rrmsg = vol_san(
-00011790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000117a0: 206c 6973 7428 7365 6c66 2e61 7372 762e   list(self.asrv.
-000117b0: 7666 732e 616c 6c5f 766f 6c73 2e76 616c  vfs.all_vols.val
-000117c0: 7565 7328 2929 2c20 756e 6963 6f64 6528  ues()), unicode(
-000117d0: 6578 292e 656e 636f 6465 2822 7574 662d  ex).encode("utf-
-000117e0: 3822 290a 2020 2020 2020 2020 2020 2020  8").            
-000117f0: 292e 6465 636f 6465 2822 7574 662d 3822  ).decode("utf-8"
-00011800: 290a 0a20 2020 2020 2020 2074 6420 3d20  )..        td = 
-00011810: 6d61 7828 302e 312c 2074 696d 652e 7469  max(0.1, time.ti
-00011820: 6d65 2829 202d 2074 3029 0a20 2020 2020  me() - t0).     
-00011830: 2020 2073 7a5f 746f 7461 6c20 3d20 7375     sz_total = su
-00011840: 6d28 785b 305d 2066 6f72 2078 2069 6e20  m(x[0] for x in 
-00011850: 6669 6c65 7329 0a20 2020 2020 2020 2073  files).        s
-00011860: 7064 203d 2028 737a 5f74 6f74 616c 202f  pd = (sz_total /
-00011870: 2074 6429 202f 2028 3130 3234 202a 2031   td) / (1024 * 1
-00011880: 3032 3429 0a0a 2020 2020 2020 2020 7374  024)..        st
-00011890: 6174 7573 203d 2022 4f4b 220a 2020 2020  atus = "OK".    
-000118a0: 2020 2020 6966 2065 7272 6d73 673a 0a20      if errmsg:. 
-000118b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000118c0: 6c6f 6728 6572 726d 7367 2c20 3329 0a20  log(errmsg, 3). 
-000118d0: 2020 2020 2020 2020 2020 2073 7461 7475             statu
-000118e0: 7320 3d20 2245 5252 4f52 220a 0a20 2020  s = "ERROR"..   
-000118f0: 2020 2020 206d 7367 203d 2022 7b7d 202f       msg = "{} /
-00011900: 2f20 7b7d 2062 7974 6573 202f 2f20 7b3a  / {} bytes // {:
-00011910: 2e33 667d 204d 6942 2f73 5c6e 222e 666f  .3f} MiB/s\n".fo
-00011920: 726d 6174 2873 7461 7475 732c 2073 7a5f  rmat(status, sz_
-00011930: 746f 7461 6c2c 2073 7064 290a 2020 2020  total, spd).    
-00011940: 2020 2020 6a6d 7367 2020 203d 207b 0a20      jmsg   = {. 
-00011950: 2020 2020 2020 2020 2020 2022 7374 6174             "stat
-00011960: 7573 223a 2073 7461 7475 732c 0a20 2020  us": status,.   
-00011970: 2020 2020 2020 2020 2022 737a 223a 2073           "sz": s
-00011980: 7a5f 746f 7461 6c2c 0a20 2020 2020 2020  z_total,.       
-00011990: 2020 2020 2022 6d62 7073 223a 2072 6f75       "mbps": rou
-000119a0: 6e64 2873 7064 2c20 3329 2c0a 2020 2020  nd(spd, 3),.    
-000119b0: 2020 2020 2020 2020 2266 696c 6573 223a          "files":
-000119c0: 205b 5d2c 0a20 2020 2020 2020 207d 0a0a   [],.        }..
-000119d0: 2020 2020 2020 2020 6966 2065 7272 6d73          if errms
-000119e0: 673a 0a20 2020 2020 2020 2020 2020 206d  g:.            m
-000119f0: 7367 202b 3d20 6572 726d 7367 202b 2022  sg += errmsg + "
-00011a00: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-00011a10: 6a6d 7367 5b22 6572 726f 7222 5d20 3d20  jmsg["error"] = 
-00011a20: 6572 726d 7367 0a20 2020 2020 2020 2020  errmsg.         
-00011a30: 2020 2065 7272 6d73 6720 3d20 2245 5252     errmsg = "ERR
-00011a40: 4f52 3a20 2220 2b20 6572 726d 7367 0a0a  OR: " + errmsg..
-00011a50: 2020 2020 2020 2020 666f 7220 737a 2c20          for sz, 
-00011a60: 7368 615f 6865 782c 2073 6861 5f62 3634  sha_hex, sha_b64
-00011a70: 2c20 6f66 6e2c 206c 666e 2c20 6170 2069  , ofn, lfn, ap i
-00011a80: 6e20 6669 6c65 733a 0a20 2020 2020 2020  n files:.       
-00011a90: 2020 2020 2076 7375 6620 3d20 2222 0a20       vsuf = "". 
-00011aa0: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
-00011ab0: 656c 662e 6361 6e5f 7265 6164 206f 7220  elf.can_read or 
-00011ac0: 7365 6c66 2e63 616e 5f75 7067 6574 2920  self.can_upget) 
-00011ad0: 616e 6420 2266 6b22 2069 6e20 7666 732e  and "fk" in vfs.
-00011ae0: 666c 6167 733a 0a20 2020 2020 2020 2020  flags:.         
-00011af0: 2020 2020 2020 2076 7375 6620 3d20 223f         vsuf = "?
-00011b00: 6b3d 2220 2b20 7365 6c66 2e67 656e 5f66  k=" + self.gen_f
-00011b10: 6b28 0a20 2020 2020 2020 2020 2020 2020  k(.             
-00011b20: 2020 2020 2020 2073 656c 662e 6172 6773         self.args
-00011b30: 2e66 6b5f 7361 6c74 2c0a 2020 2020 2020  .fk_salt,.      
-00011b40: 2020 2020 2020 2020 2020 2020 2020 6170                ap
-00011b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011b60: 2020 2020 2020 737a 2c0a 2020 2020 2020        sz,.      
-00011b70: 2020 2020 2020 2020 2020 2020 2020 3020                0 
-00011b80: 6966 2041 4e59 5749 4e20 6f72 206e 6f74  if ANYWIN or not
-00011b90: 2061 7020 656c 7365 2062 6f73 2e73 7461   ap else bos.sta
-00011ba0: 7428 6170 292e 7374 5f69 6e6f 2c0a 2020  t(ap).st_ino,.  
-00011bb0: 2020 2020 2020 2020 2020 2020 2020 295b                )[
-00011bc0: 3a20 7666 732e 666c 6167 735b 2266 6b22  : vfs.flags["fk"
-00011bd0: 5d5d 0a0a 2020 2020 2020 2020 2020 2020  ]]..            
-00011be0: 7670 6174 6820 3d20 227b 7d2f 7b7d 222e  vpath = "{}/{}".
-00011bf0: 666f 726d 6174 2875 706c 6f61 645f 7670  format(upload_vp
-00011c00: 6174 682c 206c 666e 292e 7374 7269 7028  ath, lfn).strip(
-00011c10: 222f 2229 0a20 2020 2020 2020 2020 2020  "/").           
-00011c20: 2072 656c 5f75 726c 203d 2071 756f 7465   rel_url = quote
-00011c30: 7028 7365 6c66 2e61 7267 732e 5253 202b  p(self.args.RS +
-00011c40: 2076 7061 7468 2920 2b20 7673 7566 0a20   vpath) + vsuf. 
-00011c50: 2020 2020 2020 2020 2020 206d 7367 202b             msg +
-00011c60: 3d20 2773 6861 3531 323a 207b 7d20 2f2f  = 'sha512: {} //
-00011c70: 207b 7d20 2f2f 207b 7d20 6279 7465 7320   {} // {} bytes 
-00011c80: 2f2f 203c 6120 6872 6566 3d22 2f7b 7d22  // <a href="/{}"
-00011c90: 3e7b 7d3c 2f61 3e20 7b7d 5c6e 272e 666f  >{}</a> {}\n'.fo
-00011ca0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00011cb0: 2020 2020 2020 7368 615f 6865 785b 3a35        sha_hex[:5
-00011cc0: 365d 2c0a 2020 2020 2020 2020 2020 2020  6],.            
-00011cd0: 2020 2020 7368 615f 6236 342c 0a20 2020      sha_b64,.   
-00011ce0: 2020 2020 2020 2020 2020 2020 2073 7a2c               sz,
-00011cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011d00: 2072 656c 5f75 726c 2c0a 2020 2020 2020   rel_url,.      
-00011d10: 2020 2020 2020 2020 2020 6874 6d6c 5f65            html_e
-00011d20: 7363 6170 6528 6f66 6e2c 2063 726c 663d  scape(ofn, crlf=
-00011d30: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-00011d40: 2020 2020 2020 2076 7375 662c 0a20 2020         vsuf,.   
-00011d50: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00011d60: 2020 2020 2020 2023 2074 7275 6e63 6174         # truncat
-00011d70: 6564 2053 4841 2d35 3132 2070 7265 7665  ed SHA-512 preve
-00011d80: 6e74 7320 6c65 6e67 7468 2065 7874 656e  nts length exten
-00011d90: 7369 6f6e 2061 7474 6163 6b73 3b0a 2020  sion attacks;.  
-00011da0: 2020 2020 2020 2020 2020 2320 7573 696e            # usin
-00011db0: 6720 5348 412d 3531 322f 3232 342c 206f  g SHA-512/224, o
-00011dc0: 7074 696f 6e61 6c6c 7920 5348 412d 3531  ptionally SHA-51
-00011dd0: 322f 3235 3620 3d20 3a36 340a 2020 2020  2/256 = :64.    
-00011de0: 2020 2020 2020 2020 6a70 6172 7420 3d20          jpart = 
-00011df0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00011e00: 2020 2275 726c 223a 2022 7b7d 3a2f 2f7b    "url": "{}://{
-00011e10: 7d2f 7b7d 222e 666f 726d 6174 280a 2020  }/{}".format(.  
-00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e30: 2020 2268 7474 7073 2220 6966 2073 656c    "https" if sel
-00011e40: 662e 6973 5f68 7474 7073 2065 6c73 6520  f.is_https else 
-00011e50: 2268 7474 7022 2c0a 2020 2020 2020 2020  "http",.        
-00011e60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011e70: 2e68 6f73 742c 0a20 2020 2020 2020 2020  .host,.         
-00011e80: 2020 2020 2020 2020 2020 2072 656c 5f75             rel_u
-00011e90: 726c 2c0a 2020 2020 2020 2020 2020 2020  rl,.            
-00011ea0: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00011eb0: 2020 2020 2020 2022 7368 6135 3132 223a         "sha512":
-00011ec0: 2073 6861 5f68 6578 5b3a 3536 5d2c 0a20   sha_hex[:56],. 
-00011ed0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011ee0: 7368 615f 6236 3422 3a20 7368 615f 6236  sha_b64": sha_b6
-00011ef0: 342c 0a20 2020 2020 2020 2020 2020 2020  4,.             
-00011f00: 2020 2022 737a 223a 2073 7a2c 0a20 2020     "sz": sz,.   
-00011f10: 2020 2020 2020 2020 2020 2020 2022 666e               "fn
-00011f20: 223a 206c 666e 2c0a 2020 2020 2020 2020  ": lfn,.        
-00011f30: 2020 2020 2020 2020 2266 6e5f 6f72 6967          "fn_orig
-00011f40: 223a 206f 666e 2c0a 2020 2020 2020 2020  ": ofn,.        
-00011f50: 2020 2020 2020 2020 2270 6174 6822 3a20          "path": 
-00011f60: 7265 6c5f 7572 6c2c 0a20 2020 2020 2020  rel_url,.       
-00011f70: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00011f80: 2020 206a 6d73 675b 2266 696c 6573 225d     jmsg["files"]
-00011f90: 2e61 7070 656e 6428 6a70 6172 7429 0a0a  .append(jpart)..
-00011fa0: 2020 2020 2020 2020 7673 7064 203d 2073          vspd = s
-00011fb0: 656c 662e 5f73 7064 2873 7a5f 746f 7461  elf._spd(sz_tota
-00011fc0: 6c2c 2046 616c 7365 290a 2020 2020 2020  l, False).      
-00011fd0: 2020 7365 6c66 2e6c 6f67 2822 7b7d 207b    self.log("{} {
-00011fe0: 7d22 2e66 6f72 6d61 7428 7673 7064 2c20  }".format(vspd, 
-00011ff0: 6d73 6729 290a 0a20 2020 2020 2020 2073  msg))..        s
-00012000: 7566 203d 2022 220a 2020 2020 2020 2020  uf = "".        
-00012010: 6966 206e 6f74 206e 756c 6c77 7269 7465  if not nullwrite
-00012020: 2061 6e64 2073 656c 662e 6172 6773 2e77   and self.args.w
-00012030: 7269 7465 5f75 706c 6f67 3a0a 2020 2020  rite_uplog:.    
-00012040: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00012050: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00012060: 5f66 6e20 3d20 2275 702e 7b3a 2e36 667d  _fn = "up.{:.6f}
-00012070: 2e74 7874 222e 666f 726d 6174 2874 3029  .txt".format(t0)
-00012080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012090: 2077 6974 6820 6f70 656e 286c 6f67 5f66   with open(log_f
-000120a0: 6e2c 2022 7762 2229 2061 7320 663a 0a20  n, "wb") as f:. 
-000120b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120c0: 2020 2066 7420 3d20 227b 7d3a 7b7d 222e     ft = "{}:{}".
-000120d0: 666f 726d 6174 2873 656c 662e 6970 2c20  format(self.ip, 
-000120e0: 7365 6c66 2e61 6464 725b 315d 290a 2020  self.addr[1]).  
+00011680: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+00011690: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
+000116a0: 2020 2020 2020 2020 2020 2061 742c 0a20             at,. 
+000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116c0: 2020 2020 2020 2073 656c 662e 756e 616d         self.unam
+000116d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000116e0: 2020 2020 2020 2020 2020 2054 7275 652c             True,
+000116f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011700: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00011710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011720: 636f 6e6e 2e6e 6279 7465 202b 3d20 737a  conn.nbyte += sz
+00011730: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011740: 2020 6578 6365 7074 2050 6562 6b61 633a    except Pebkac:
+00011750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011760: 2020 2020 2073 656c 662e 7061 7273 6572       self.parser
+00011770: 2e64 726f 7028 290a 2020 2020 2020 2020  .drop().        
+00011780: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00011790: 650a 0a20 2020 2020 2020 2065 7863 6570  e..        excep
+000117a0: 7420 5065 626b 6163 2061 7320 6578 3a0a  t Pebkac as ex:.
+000117b0: 2020 2020 2020 2020 2020 2020 6572 726d              errm
+000117c0: 7367 203d 2076 6f6c 5f73 616e 280a 2020  sg = vol_san(.  
+000117d0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+000117e0: 7374 2873 656c 662e 6173 7276 2e76 6673  st(self.asrv.vfs
+000117f0: 2e61 6c6c 5f76 6f6c 732e 7661 6c75 6573  .all_vols.values
+00011800: 2829 292c 2075 6e69 636f 6465 2865 7829  ()), unicode(ex)
+00011810: 2e65 6e63 6f64 6528 2275 7466 2d38 2229  .encode("utf-8")
+00011820: 0a20 2020 2020 2020 2020 2020 2029 2e64  .            ).d
+00011830: 6563 6f64 6528 2275 7466 2d38 2229 0a0a  ecode("utf-8")..
+00011840: 2020 2020 2020 2020 7464 203d 206d 6178          td = max
+00011850: 2830 2e31 2c20 7469 6d65 2e74 696d 6528  (0.1, time.time(
+00011860: 2920 2d20 7430 290a 2020 2020 2020 2020  ) - t0).        
+00011870: 737a 5f74 6f74 616c 203d 2073 756d 2878  sz_total = sum(x
+00011880: 5b30 5d20 666f 7220 7820 696e 2066 696c  [0] for x in fil
+00011890: 6573 290a 2020 2020 2020 2020 7370 6420  es).        spd 
+000118a0: 3d20 2873 7a5f 746f 7461 6c20 2f20 7464  = (sz_total / td
+000118b0: 2920 2f20 2831 3032 3420 2a20 3130 3234  ) / (1024 * 1024
+000118c0: 290a 0a20 2020 2020 2020 2073 7461 7475  )..        statu
+000118d0: 7320 3d20 224f 4b22 0a20 2020 2020 2020  s = "OK".       
+000118e0: 2069 6620 6572 726d 7367 3a0a 2020 2020   if errmsg:.    
+000118f0: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+00011900: 2865 7272 6d73 672c 2033 290a 2020 2020  (errmsg, 3).    
+00011910: 2020 2020 2020 2020 7374 6174 7573 203d          status =
+00011920: 2022 4552 524f 5222 0a0a 2020 2020 2020   "ERROR"..      
+00011930: 2020 6d73 6720 3d20 227b 7d20 2f2f 207b    msg = "{} // {
+00011940: 7d20 6279 7465 7320 2f2f 207b 3a2e 3366  } bytes // {:.3f
+00011950: 7d20 4d69 422f 735c 6e22 2e66 6f72 6d61  } MiB/s\n".forma
+00011960: 7428 7374 6174 7573 2c20 737a 5f74 6f74  t(status, sz_tot
+00011970: 616c 2c20 7370 6429 0a20 2020 2020 2020  al, spd).       
+00011980: 206a 6d73 6720 2020 3d20 7b0a 2020 2020   jmsg   = {.    
+00011990: 2020 2020 2020 2020 2273 7461 7475 7322          "status"
+000119a0: 3a20 7374 6174 7573 2c0a 2020 2020 2020  : status,.      
+000119b0: 2020 2020 2020 2273 7a22 3a20 737a 5f74        "sz": sz_t
+000119c0: 6f74 616c 2c0a 2020 2020 2020 2020 2020  otal,.          
+000119d0: 2020 226d 6270 7322 3a20 726f 756e 6428    "mbps": round(
+000119e0: 7370 642c 2033 292c 0a20 2020 2020 2020  spd, 3),.       
+000119f0: 2020 2020 2022 6669 6c65 7322 3a20 5b5d       "files": []
+00011a00: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
+00011a10: 2020 2020 2069 6620 6572 726d 7367 3a0a       if errmsg:.
+00011a20: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+00011a30: 2b3d 2065 7272 6d73 6720 2b20 225c 6e22  += errmsg + "\n"
+00011a40: 0a20 2020 2020 2020 2020 2020 206a 6d73  .            jms
+00011a50: 675b 2265 7272 6f72 225d 203d 2065 7272  g["error"] = err
+00011a60: 6d73 670a 2020 2020 2020 2020 2020 2020  msg.            
+00011a70: 6572 726d 7367 203d 2022 4552 524f 523a  errmsg = "ERROR:
+00011a80: 2022 202b 2065 7272 6d73 670a 0a20 2020   " + errmsg..   
+00011a90: 2020 2020 2066 6f72 2073 7a2c 2073 6861       for sz, sha
+00011aa0: 5f68 6578 2c20 7368 615f 6236 342c 206f  _hex, sha_b64, o
+00011ab0: 666e 2c20 6c66 6e2c 2061 7020 696e 2066  fn, lfn, ap in f
+00011ac0: 696c 6573 3a0a 2020 2020 2020 2020 2020  iles:.          
+00011ad0: 2020 7673 7566 203d 2022 220a 2020 2020    vsuf = "".    
+00011ae0: 2020 2020 2020 2020 6966 2028 7365 6c66          if (self
+00011af0: 2e63 616e 5f72 6561 6420 6f72 2073 656c  .can_read or sel
+00011b00: 662e 6361 6e5f 7570 6765 7429 2061 6e64  f.can_upget) and
+00011b10: 2022 666b 2220 696e 2076 6673 2e66 6c61   "fk" in vfs.fla
+00011b20: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00011b30: 2020 2020 7673 7566 203d 2022 3f6b 3d22      vsuf = "?k="
+00011b40: 202b 2073 656c 662e 6765 6e5f 666b 280a   + self.gen_fk(.
+00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b60: 2020 2020 7365 6c66 2e61 7267 732e 666b      self.args.fk
+00011b70: 5f73 616c 742c 0a20 2020 2020 2020 2020  _salt,.         
+00011b80: 2020 2020 2020 2020 2020 2061 702c 0a20             ap,. 
+00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ba0: 2020 2073 7a2c 0a20 2020 2020 2020 2020     sz,.         
+00011bb0: 2020 2020 2020 2020 2020 2030 2069 6620             0 if 
+00011bc0: 414e 5957 494e 206f 7220 6e6f 7420 6170  ANYWIN or not ap
+00011bd0: 2065 6c73 6520 626f 732e 7374 6174 2861   else bos.stat(a
+00011be0: 7029 2e73 745f 696e 6f2c 0a20 2020 2020  p).st_ino,.     
+00011bf0: 2020 2020 2020 2020 2020 2029 5b3a 2076             )[: v
+00011c00: 6673 2e66 6c61 6773 5b22 666b 225d 5d0a  fs.flags["fk"]].
+00011c10: 0a20 2020 2020 2020 2020 2020 2076 7061  .            vpa
+00011c20: 7468 203d 2022 7b7d 2f7b 7d22 2e66 6f72  th = "{}/{}".for
+00011c30: 6d61 7428 7570 6c6f 6164 5f76 7061 7468  mat(upload_vpath
+00011c40: 2c20 6c66 6e29 2e73 7472 6970 2822 2f22  , lfn).strip("/"
+00011c50: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00011c60: 6c5f 7572 6c20 3d20 7175 6f74 6570 2873  l_url = quotep(s
+00011c70: 656c 662e 6172 6773 2e52 5320 2b20 7670  elf.args.RS + vp
+00011c80: 6174 6829 202b 2076 7375 660a 2020 2020  ath) + vsuf.    
+00011c90: 2020 2020 2020 2020 6d73 6720 2b3d 2027          msg += '
+00011ca0: 7368 6135 3132 3a20 7b7d 202f 2f20 7b7d  sha512: {} // {}
+00011cb0: 202f 2f20 7b7d 2062 7974 6573 202f 2f20   // {} bytes // 
+00011cc0: 3c61 2068 7265 663d 222f 7b7d 223e 7b7d  <a href="/{}">{}
+00011cd0: 3c2f 613e 207b 7d5c 6e27 2e66 6f72 6d61  </a> {}\n'.forma
+00011ce0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00011cf0: 2020 2073 6861 5f68 6578 5b3a 3536 5d2c     sha_hex[:56],
+00011d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d10: 2073 6861 5f62 3634 2c0a 2020 2020 2020   sha_b64,.      
+00011d20: 2020 2020 2020 2020 2020 737a 2c0a 2020            sz,.  
+00011d30: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00011d40: 6c5f 7572 6c2c 0a20 2020 2020 2020 2020  l_url,.         
+00011d50: 2020 2020 2020 2068 746d 6c5f 6573 6361         html_esca
+00011d60: 7065 286f 666e 2c20 6372 6c66 3d54 7275  pe(ofn, crlf=Tru
+00011d70: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+00011d80: 2020 2020 7673 7566 2c0a 2020 2020 2020      vsuf,.      
+00011d90: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00011da0: 2020 2020 2320 7472 756e 6361 7465 6420      # truncated 
+00011db0: 5348 412d 3531 3220 7072 6576 656e 7473  SHA-512 prevents
+00011dc0: 206c 656e 6774 6820 6578 7465 6e73 696f   length extensio
+00011dd0: 6e20 6174 7461 636b 733b 0a20 2020 2020  n attacks;.     
+00011de0: 2020 2020 2020 2023 2075 7369 6e67 2053         # using S
+00011df0: 4841 2d35 3132 2f32 3234 2c20 6f70 7469  HA-512/224, opti
+00011e00: 6f6e 616c 6c79 2053 4841 2d35 3132 2f32  onally SHA-512/2
+00011e10: 3536 203d 203a 3634 0a20 2020 2020 2020  56 = :64.       
+00011e20: 2020 2020 206a 7061 7274 203d 207b 0a20       jpart = {. 
+00011e30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011e40: 7572 6c22 3a20 227b 7d3a 2f2f 7b7d 2f7b  url": "{}://{}/{
+00011e50: 7d22 2e66 6f72 6d61 7428 0a20 2020 2020  }".format(.     
+00011e60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011e70: 6874 7470 7322 2069 6620 7365 6c66 2e69  https" if self.i
+00011e80: 735f 6874 7470 7320 656c 7365 2022 6874  s_https else "ht
+00011e90: 7470 222c 0a20 2020 2020 2020 2020 2020  tp",.           
+00011ea0: 2020 2020 2020 2020 2073 656c 662e 686f           self.ho
+00011eb0: 7374 2c0a 2020 2020 2020 2020 2020 2020  st,.            
+00011ec0: 2020 2020 2020 2020 7265 6c5f 7572 6c2c          rel_url,
+00011ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011ee0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00011ef0: 2020 2020 2273 6861 3531 3222 3a20 7368      "sha512": sh
+00011f00: 615f 6865 785b 3a35 365d 2c0a 2020 2020  a_hex[:56],.    
+00011f10: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00011f20: 5f62 3634 223a 2073 6861 5f62 3634 2c0a  _b64": sha_b64,.
+00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f40: 2273 7a22 3a20 737a 2c0a 2020 2020 2020  "sz": sz,.      
+00011f50: 2020 2020 2020 2020 2020 2266 6e22 3a20            "fn": 
+00011f60: 6c66 6e2c 0a20 2020 2020 2020 2020 2020  lfn,.           
+00011f70: 2020 2020 2022 666e 5f6f 7269 6722 3a20       "fn_orig": 
+00011f80: 6f66 6e2c 0a20 2020 2020 2020 2020 2020  ofn,.           
+00011f90: 2020 2020 2022 7061 7468 223a 2072 656c       "path": rel
+00011fa0: 5f75 726c 2c0a 2020 2020 2020 2020 2020  _url,.          
+00011fb0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00011fc0: 6a6d 7367 5b22 6669 6c65 7322 5d2e 6170  jmsg["files"].ap
+00011fd0: 7065 6e64 286a 7061 7274 290a 0a20 2020  pend(jpart)..   
+00011fe0: 2020 2020 2076 7370 6420 3d20 7365 6c66       vspd = self
+00011ff0: 2e5f 7370 6428 737a 5f74 6f74 616c 2c20  ._spd(sz_total, 
+00012000: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
+00012010: 656c 662e 6c6f 6728 227b 7d20 7b7d 222e  elf.log("{} {}".
+00012020: 666f 726d 6174 2876 7370 642c 206d 7367  format(vspd, msg
+00012030: 2929 0a0a 2020 2020 2020 2020 7375 6620  ))..        suf 
+00012040: 3d20 2222 0a20 2020 2020 2020 2069 6620  = "".        if 
+00012050: 6e6f 7420 6e75 6c6c 7772 6974 6520 616e  not nullwrite an
+00012060: 6420 7365 6c66 2e61 7267 732e 7772 6974  d self.args.writ
+00012070: 655f 7570 6c6f 673a 0a20 2020 2020 2020  e_uplog:.       
+00012080: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00012090: 2020 2020 2020 2020 2020 6c6f 675f 666e            log_fn
+000120a0: 203d 2022 7570 2e7b 3a2e 3666 7d2e 7478   = "up.{:.6f}.tx
+000120b0: 7422 2e66 6f72 6d61 7428 7430 290a 2020  t".format(t0).  
+000120c0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+000120d0: 7468 206f 7065 6e28 6c6f 675f 666e 2c20  th open(log_fn, 
+000120e0: 2277 6222 2920 6173 2066 3a0a 2020 2020  "wb") as f:.    
 000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012100: 2020 6674 203d 2022 7b7d 5c6e 7b7d 5c6e    ft = "{}\n{}\n
-00012110: 7b7d 5c6e 222e 666f 726d 6174 2866 742c  {}\n".format(ft,
-00012120: 206d 7367 2e72 7374 7269 7028 292c 2065   msg.rstrip(), e
-00012130: 7272 6d73 6729 0a20 2020 2020 2020 2020  rrmsg).         
-00012140: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-00012150: 7465 2866 742e 656e 636f 6465 2822 7574  te(ft.encode("ut
-00012160: 662d 3822 2929 0a20 2020 2020 2020 2020  f-8")).         
-00012170: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00012180: 696f 6e20 6173 2065 783a 0a20 2020 2020  ion as ex:.     
-00012190: 2020 2020 2020 2020 2020 2073 7566 203d             suf =
-000121a0: 2022 5c6e 6661 696c 6564 2074 6f20 7772   "\nfailed to wr
-000121b0: 6974 6520 7468 6520 7570 6c6f 6164 2072  ite the upload r
-000121c0: 6570 6f72 743a 207b 7d22 2e66 6f72 6d61  eport: {}".forma
-000121d0: 7428 6578 290a 0a20 2020 2020 2020 2073  t(ex)..        s
-000121e0: 6320 3d20 3430 3020 6966 2065 7272 6d73  c = 400 if errms
-000121f0: 6720 656c 7365 2032 3031 0a20 2020 2020  g else 201.     
-00012200: 2020 2069 6620 7761 6e74 5f75 726c 3a0a     if want_url:.
-00012210: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-00012220: 3d20 225c 6e22 2e6a 6f69 6e28 5b78 5b22  = "\n".join([x["
-00012230: 7572 6c22 5d20 666f 7220 7820 696e 206a  url"] for x in j
-00012240: 6d73 675b 2266 696c 6573 225d 5d29 0a20  msg["files"]]). 
-00012250: 2020 2020 2020 2020 2020 2069 6620 6572             if er
-00012260: 726d 7367 3a0a 2020 2020 2020 2020 2020  rmsg:.          
-00012270: 2020 2020 2020 6d73 6720 2b3d 2022 5c6e        msg += "\n
-00012280: 2220 2b20 6572 726d 7367 0a0a 2020 2020  " + errmsg..    
-00012290: 2020 2020 2020 2020 7365 6c66 2e72 6570          self.rep
-000122a0: 6c79 286d 7367 2e65 6e63 6f64 6528 2275  ly(msg.encode("u
-000122b0: 7466 2d38 222c 2022 7265 706c 6163 6522  tf-8", "replace"
-000122c0: 292c 2073 7461 7475 733d 7363 290a 2020  ), status=sc).  
-000122d0: 2020 2020 2020 656c 6966 2022 6a22 2069        elif "j" i
-000122e0: 6e20 7365 6c66 2e75 7061 7261 6d3a 0a20  n self.uparam:. 
-000122f0: 2020 2020 2020 2020 2020 206a 7478 7420             jtxt 
-00012300: 3d20 6a73 6f6e 2e64 756d 7073 286a 6d73  = json.dumps(jms
-00012310: 672c 2069 6e64 656e 743d 322c 2073 6f72  g, indent=2, sor
-00012320: 745f 6b65 7973 3d54 7275 6529 2e65 6e63  t_keys=True).enc
-00012330: 6f64 6528 2275 7466 2d38 222c 2022 7265  ode("utf-8", "re
-00012340: 706c 6163 6522 290a 2020 2020 2020 2020  place").        
-00012350: 2020 2020 7365 6c66 2e72 6570 6c79 286a      self.reply(j
-00012360: 7478 742c 206d 696d 653d 2261 7070 6c69  txt, mime="appli
-00012370: 6361 7469 6f6e 2f6a 736f 6e22 2c20 7374  cation/json", st
-00012380: 6174 7573 3d73 6329 0a20 2020 2020 2020  atus=sc).       
-00012390: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000123a0: 2020 2073 656c 662e 7265 6469 7265 6374     self.redirect
-000123b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000123c0: 2020 7365 6c66 2e76 7061 7468 2c0a 2020    self.vpath,.  
-000123d0: 2020 2020 2020 2020 2020 2020 2020 6d73                ms
-000123e0: 673d 6d73 6720 2b20 7375 662c 0a20 2020  g=msg + suf,.   
-000123f0: 2020 2020 2020 2020 2020 2020 2066 6c61               fla
-00012400: 766f 723d 2272 6574 7572 6e20 746f 222c  vor="return to",
-00012410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012420: 2063 6c69 636b 3d46 616c 7365 2c0a 2020   click=False,.  
-00012430: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00012440: 6174 7573 3d73 632c 0a20 2020 2020 2020  atus=sc,.       
-00012450: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00012460: 6966 2065 7272 6d73 673a 0a20 2020 2020  if errmsg:.     
-00012470: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00012480: 6c73 650a 0a20 2020 2020 2020 2073 656c  lse..        sel
-00012490: 662e 7061 7273 6572 2e64 726f 7028 290a  f.parser.drop().
-000124a0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-000124b0: 7275 650a 0a20 2020 2064 6566 2068 616e  rue..    def han
-000124c0: 646c 655f 7465 7874 5f75 706c 6f61 6428  dle_text_upload(
-000124d0: 7365 6c66 2920 203a 0a20 2020 2020 2020  self)  :.       
-000124e0: 2061 7373 6572 7420 7365 6c66 2e70 6172   assert self.par
-000124f0: 7365 720a 2020 2020 2020 2020 7472 793a  ser.        try:
-00012500: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00012510: 5f6c 6173 746d 6f64 3320 3d20 696e 7428  _lastmod3 = int(
-00012520: 7365 6c66 2e70 6172 7365 722e 7265 7175  self.parser.requ
-00012530: 6972 6528 226c 6173 746d 6f64 222c 2031  ire("lastmod", 1
-00012540: 3629 290a 2020 2020 2020 2020 6578 6365  6)).        exce
-00012550: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-00012560: 7261 6973 6520 5065 626b 6163 2834 3030  raise Pebkac(400
-00012570: 2c20 2263 6f75 6c64 206e 6f74 2072 6561  , "could not rea
-00012580: 6420 6c61 7374 6d6f 6420 6672 6f6d 2072  d lastmod from r
-00012590: 6571 7565 7374 2229 0a0a 2020 2020 2020  equest")..      
-000125a0: 2020 6e75 6c6c 7772 6974 6520 3d20 7365    nullwrite = se
-000125b0: 6c66 2e61 7267 732e 6e77 0a20 2020 2020  lf.args.nw.     
-000125c0: 2020 2076 6673 2c20 7265 6d20 3d20 7365     vfs, rem = se
-000125d0: 6c66 2e61 7372 762e 7666 732e 6765 7428  lf.asrv.vfs.get(
-000125e0: 7365 6c66 2e76 7061 7468 2c20 7365 6c66  self.vpath, self
-000125f0: 2e75 6e61 6d65 2c20 5472 7565 2c20 5472  .uname, True, Tr
-00012600: 7565 290a 2020 2020 2020 2020 7365 6c66  ue).        self
-00012610: 2e5f 6173 7365 7274 5f73 6166 655f 7265  ._assert_safe_re
-00012620: 6d28 7265 6d29 0a0a 2020 2020 2020 2020  m(rem)..        
-00012630: 636c 656e 203d 2069 6e74 2873 656c 662e  clen = int(self.
-00012640: 6865 6164 6572 732e 6765 7428 2263 6f6e  headers.get("con
-00012650: 7465 6e74 2d6c 656e 6774 6822 2c20 2d31  tent-length", -1
-00012660: 2929 0a20 2020 2020 2020 2069 6620 636c  )).        if cl
-00012670: 656e 203d 3d20 2d31 3a0a 2020 2020 2020  en == -1:.      
-00012680: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
-00012690: 6163 2834 3131 290a 0a20 2020 2020 2020  ac(411)..       
-000126a0: 2072 702c 2066 6e20 3d20 7673 706c 6974   rp, fn = vsplit
-000126b0: 2872 656d 290a 2020 2020 2020 2020 6670  (rem).        fp
-000126c0: 203d 2076 6673 2e63 616e 6f6e 6963 616c   = vfs.canonical
-000126d0: 2872 7029 0a20 2020 2020 2020 206c 696d  (rp).        lim
-000126e0: 203d 2076 6673 2e67 6574 5f64 6276 2872   = vfs.get_dbv(r
-000126f0: 656d 295b 305d 2e6c 696d 0a20 2020 2020  em)[0].lim.     
-00012700: 2020 2069 6620 6c69 6d3a 0a20 2020 2020     if lim:.     
-00012710: 2020 2020 2020 2066 702c 2072 7020 3d20         fp, rp = 
-00012720: 6c69 6d2e 616c 6c28 7365 6c66 2e69 702c  lim.all(self.ip,
-00012730: 2072 702c 2063 6c65 6e2c 2066 7029 0a20   rp, clen, fp). 
-00012740: 2020 2020 2020 2020 2020 2062 6f73 2e6d             bos.m
-00012750: 616b 6564 6972 7328 6670 290a 0a20 2020  akedirs(fp)..   
-00012760: 2020 2020 2066 7020 3d20 6f73 2e70 6174       fp = os.pat
-00012770: 682e 6a6f 696e 2866 702c 2066 6e29 0a20  h.join(fp, fn). 
-00012780: 2020 2020 2020 2072 656d 203d 2022 7b7d         rem = "{}
-00012790: 2f7b 7d22 2e66 6f72 6d61 7428 7270 2c20  /{}".format(rp, 
-000127a0: 666e 292e 7374 7269 7028 222f 2229 0a0a  fn).strip("/")..
-000127b0: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-000127c0: 656d 2e65 6e64 7377 6974 6828 222e 6d64  em.endswith(".md
-000127d0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000127e0: 7261 6973 6520 5065 626b 6163 2834 3030  raise Pebkac(400
-000127f0: 2c20 226f 6e6c 7920 6d61 726b 646f 776e  , "only markdown
-00012800: 2070 6c73 2229 0a0a 2020 2020 2020 2020   pls")..        
-00012810: 6966 206e 756c 6c77 7269 7465 3a0a 2020  if nullwrite:.  
-00012820: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-00012830: 7365 203d 206a 736f 6e2e 6475 6d70 7328  se = json.dumps(
-00012840: 7b22 6f6b 223a 2054 7275 652c 2022 6c61  {"ok": True, "la
-00012850: 7374 6d6f 6422 3a20 307d 290a 2020 2020  stmod": 0}).    
-00012860: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
-00012870: 2872 6573 706f 6e73 6529 0a20 2020 2020  (response).     
-00012880: 2020 2020 2020 2023 2054 4f44 4f20 7265         # TODO re
-00012890: 706c 7920 7368 6f75 6c64 2070 6172 7365  ply should parse
-000128a0: 722e 6472 6f70 2829 0a20 2020 2020 2020  r.drop().       
-000128b0: 2020 2020 2073 656c 662e 7061 7273 6572       self.parser
-000128c0: 2e64 726f 7028 290a 2020 2020 2020 2020  .drop().        
-000128d0: 2020 2020 7365 6c66 2e72 6570 6c79 2872      self.reply(r
-000128e0: 6573 706f 6e73 652e 656e 636f 6465 2822  esponse.encode("
-000128f0: 7574 662d 3822 2929 0a20 2020 2020 2020  utf-8")).       
-00012900: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00012910: 0a0a 2020 2020 2020 2020 7372 765f 6c61  ..        srv_la
-00012920: 7374 6d6f 6420 3d20 2d31 2e30 0a20 2020  stmod = -1.0.   
-00012930: 2020 2020 2073 7276 5f6c 6173 746d 6f64       srv_lastmod
-00012940: 3320 3d20 2d31 0a20 2020 2020 2020 2074  3 = -1.        t
-00012950: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00012960: 7374 203d 2062 6f73 2e73 7461 7428 6670  st = bos.stat(fp
-00012970: 290a 2020 2020 2020 2020 2020 2020 7372  ).            sr
-00012980: 765f 6c61 7374 6d6f 6420 3d20 7374 2e73  v_lastmod = st.s
-00012990: 745f 6d74 696d 650a 2020 2020 2020 2020  t_mtime.        
-000129a0: 2020 2020 7372 765f 6c61 7374 6d6f 6433      srv_lastmod3
-000129b0: 203d 2069 6e74 2873 7276 5f6c 6173 746d   = int(srv_lastm
-000129c0: 6f64 202a 2031 3030 3029 0a20 2020 2020  od * 1000).     
-000129d0: 2020 2065 7863 6570 7420 4f53 4572 726f     except OSErro
-000129e0: 7220 6173 2065 783a 0a20 2020 2020 2020  r as ex:.       
-000129f0: 2020 2020 2069 6620 6578 2e65 7272 6e6f       if ex.errno
-00012a00: 2021 3d20 6572 726e 6f2e 454e 4f45 4e54   != errno.ENOENT
-00012a10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012a20: 2020 7261 6973 650a 0a20 2020 2020 2020    raise..       
-00012a30: 2023 2069 6620 6669 6c65 2065 7869 7374   # if file exist
-00012a40: 732c 2063 6865 6b63 2074 6861 7420 7469  s, chekc that ti
-00012a50: 6d65 7374 616d 7020 6d61 7463 6865 7320  mestamp matches 
-00012a60: 7468 6520 636c 6965 6e74 2773 0a20 2020  the client's.   
-00012a70: 2020 2020 2069 6620 7372 765f 6c61 7374       if srv_last
-00012a80: 6d6f 6420 3e3d 2030 3a0a 2020 2020 2020  mod >= 0:.      
-00012a90: 2020 2020 2020 7361 6d65 5f6c 6173 746d        same_lastm
-00012aa0: 6f64 203d 2063 6c69 5f6c 6173 746d 6f64  od = cli_lastmod
-00012ab0: 3320 696e 205b 2d31 2c20 7372 765f 6c61  3 in [-1, srv_la
-00012ac0: 7374 6d6f 6433 5d0a 2020 2020 2020 2020  stmod3].        
-00012ad0: 2020 2020 6966 206e 6f74 2073 616d 655f      if not same_
-00012ae0: 6c61 7374 6d6f 643a 0a20 2020 2020 2020  lastmod:.       
-00012af0: 2020 2020 2020 2020 2023 2073 6f6d 6520           # some 
-00012b00: 6669 6c65 7379 7374 656d 732f 7472 616e  filesystems/tran
-00012b10: 7370 6f72 7473 206c 696d 6974 2070 7265  sports limit pre
-00012b20: 6369 7369 6f6e 2074 6f20 3173 6563 2c20  cision to 1sec, 
-00012b30: 686f 7065 6675 6c6c 7920 666c 6f6f 7265  hopefully floore
-00012b40: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00012b50: 2020 7361 6d65 5f6c 6173 746d 6f64 203d    same_lastmod =
-00012b60: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00012b70: 2020 2020 2020 2073 7276 5f6c 6173 746d         srv_lastm
-00012b80: 6f64 203d 3d20 696e 7428 636c 695f 6c61  od == int(cli_la
-00012b90: 7374 6d6f 6433 202f 2031 3030 3029 0a20  stmod3 / 1000). 
+00012100: 6674 203d 2022 7b7d 3a7b 7d22 2e66 6f72  ft = "{}:{}".for
+00012110: 6d61 7428 7365 6c66 2e69 702c 2073 656c  mat(self.ip, sel
+00012120: 662e 6164 6472 5b31 5d29 0a20 2020 2020  f.addr[1]).     
+00012130: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00012140: 7420 3d20 227b 7d5c 6e7b 7d5c 6e7b 7d5c  t = "{}\n{}\n{}\
+00012150: 6e22 2e66 6f72 6d61 7428 6674 2c20 6d73  n".format(ft, ms
+00012160: 672e 7273 7472 6970 2829 2c20 6572 726d  g.rstrip(), errm
+00012170: 7367 290a 2020 2020 2020 2020 2020 2020  sg).            
+00012180: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00012190: 6674 2e65 6e63 6f64 6528 2275 7466 2d38  ft.encode("utf-8
+000121a0: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+000121b0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+000121c0: 2061 7320 6578 3a0a 2020 2020 2020 2020   as ex:.        
+000121d0: 2020 2020 2020 2020 7375 6620 3d20 225c          suf = "\
+000121e0: 6e66 6169 6c65 6420 746f 2077 7269 7465  nfailed to write
+000121f0: 2074 6865 2075 706c 6f61 6420 7265 706f   the upload repo
+00012200: 7274 3a20 7b7d 222e 666f 726d 6174 2865  rt: {}".format(e
+00012210: 7829 0a0a 2020 2020 2020 2020 7363 203d  x)..        sc =
+00012220: 2034 3030 2069 6620 6572 726d 7367 2065   400 if errmsg e
+00012230: 6c73 6520 3230 310a 2020 2020 2020 2020  lse 201.        
+00012240: 6966 2077 616e 745f 7572 6c3a 0a20 2020  if want_url:.   
+00012250: 2020 2020 2020 2020 206d 7367 203d 2022           msg = "
+00012260: 5c6e 222e 6a6f 696e 285b 785b 2275 726c  \n".join([x["url
+00012270: 225d 2066 6f72 2078 2069 6e20 6a6d 7367  "] for x in jmsg
+00012280: 5b22 6669 6c65 7322 5d5d 290a 2020 2020  ["files"]]).    
+00012290: 2020 2020 2020 2020 6966 2065 7272 6d73          if errms
+000122a0: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
+000122b0: 2020 206d 7367 202b 3d20 225c 6e22 202b     msg += "\n" +
+000122c0: 2065 7272 6d73 670a 0a20 2020 2020 2020   errmsg..       
+000122d0: 2020 2020 2073 656c 662e 7265 706c 7928       self.reply(
+000122e0: 6d73 672e 656e 636f 6465 2822 7574 662d  msg.encode("utf-
+000122f0: 3822 2c20 2272 6570 6c61 6365 2229 2c20  8", "replace"), 
+00012300: 7374 6174 7573 3d73 6329 0a20 2020 2020  status=sc).     
+00012310: 2020 2065 6c69 6620 226a 2220 696e 2073     elif "j" in s
+00012320: 656c 662e 7570 6172 616d 3a0a 2020 2020  elf.uparam:.    
+00012330: 2020 2020 2020 2020 6a74 7874 203d 206a          jtxt = j
+00012340: 736f 6e2e 6475 6d70 7328 6a6d 7367 2c20  son.dumps(jmsg, 
+00012350: 696e 6465 6e74 3d32 2c20 736f 7274 5f6b  indent=2, sort_k
+00012360: 6579 733d 5472 7565 292e 656e 636f 6465  eys=True).encode
+00012370: 2822 7574 662d 3822 2c20 2272 6570 6c61  ("utf-8", "repla
+00012380: 6365 2229 0a20 2020 2020 2020 2020 2020  ce").           
+00012390: 2073 656c 662e 7265 706c 7928 6a74 7874   self.reply(jtxt
+000123a0: 2c20 6d69 6d65 3d22 6170 706c 6963 6174  , mime="applicat
+000123b0: 696f 6e2f 6a73 6f6e 222c 2073 7461 7475  ion/json", statu
+000123c0: 733d 7363 290a 2020 2020 2020 2020 656c  s=sc).        el
+000123d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000123e0: 7365 6c66 2e72 6564 6972 6563 7428 0a20  self.redirect(. 
+000123f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012400: 656c 662e 7670 6174 682c 0a20 2020 2020  elf.vpath,.     
+00012410: 2020 2020 2020 2020 2020 206d 7367 3d6d             msg=m
+00012420: 7367 202b 2073 7566 2c0a 2020 2020 2020  sg + suf,.      
+00012430: 2020 2020 2020 2020 2020 666c 6176 6f72            flavor
+00012440: 3d22 7265 7475 726e 2074 6f22 2c0a 2020  ="return to",.  
+00012450: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00012460: 6963 6b3d 4661 6c73 652c 0a20 2020 2020  ick=False,.     
+00012470: 2020 2020 2020 2020 2020 2073 7461 7475             statu
+00012480: 733d 7363 2c0a 2020 2020 2020 2020 2020  s=sc,.          
+00012490: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
+000124a0: 6572 726d 7367 3a0a 2020 2020 2020 2020  errmsg:.        
+000124b0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000124c0: 0a0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+000124d0: 6172 7365 722e 6472 6f70 2829 0a20 2020  arser.drop().   
+000124e0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+000124f0: 0a0a 2020 2020 6465 6620 6861 6e64 6c65  ..    def handle
+00012500: 5f74 6578 745f 7570 6c6f 6164 2873 656c  _text_upload(sel
+00012510: 6629 2020 3a0a 2020 2020 2020 2020 6173  f)  :.        as
+00012520: 7365 7274 2073 656c 662e 7061 7273 6572  sert self.parser
+00012530: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00012540: 2020 2020 2020 2020 2020 636c 695f 6c61            cli_la
+00012550: 7374 6d6f 6433 203d 2069 6e74 2873 656c  stmod3 = int(sel
+00012560: 662e 7061 7273 6572 2e72 6571 7569 7265  f.parser.require
+00012570: 2822 6c61 7374 6d6f 6422 2c20 3136 2929  ("lastmod", 16))
+00012580: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
+00012590: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000125a0: 7365 2050 6562 6b61 6328 3430 302c 2022  se Pebkac(400, "
+000125b0: 636f 756c 6420 6e6f 7420 7265 6164 206c  could not read l
+000125c0: 6173 746d 6f64 2066 726f 6d20 7265 7175  astmod from requ
+000125d0: 6573 7422 290a 0a20 2020 2020 2020 206e  est")..        n
+000125e0: 756c 6c77 7269 7465 203d 2073 656c 662e  ullwrite = self.
+000125f0: 6172 6773 2e6e 770a 2020 2020 2020 2020  args.nw.        
+00012600: 7666 732c 2072 656d 203d 2073 656c 662e  vfs, rem = self.
+00012610: 6173 7276 2e76 6673 2e67 6574 2873 656c  asrv.vfs.get(sel
+00012620: 662e 7670 6174 682c 2073 656c 662e 756e  f.vpath, self.un
+00012630: 616d 652c 2054 7275 652c 2054 7275 6529  ame, True, True)
+00012640: 0a20 2020 2020 2020 2073 656c 662e 5f61  .        self._a
+00012650: 7373 6572 745f 7361 6665 5f72 656d 2872  ssert_safe_rem(r
+00012660: 656d 290a 0a20 2020 2020 2020 2063 6c65  em)..        cle
+00012670: 6e20 3d20 696e 7428 7365 6c66 2e68 6561  n = int(self.hea
+00012680: 6465 7273 2e67 6574 2822 636f 6e74 656e  ders.get("conten
+00012690: 742d 6c65 6e67 7468 222c 202d 3129 290a  t-length", -1)).
+000126a0: 2020 2020 2020 2020 6966 2063 6c65 6e20          if clen 
+000126b0: 3d3d 202d 313a 0a20 2020 2020 2020 2020  == -1:.         
+000126c0: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
+000126d0: 3431 3129 0a0a 2020 2020 2020 2020 7270  411)..        rp
+000126e0: 2c20 666e 203d 2076 7370 6c69 7428 7265  , fn = vsplit(re
+000126f0: 6d29 0a20 2020 2020 2020 2066 7020 3d20  m).        fp = 
+00012700: 7666 732e 6361 6e6f 6e69 6361 6c28 7270  vfs.canonical(rp
+00012710: 290a 2020 2020 2020 2020 6c69 6d20 3d20  ).        lim = 
+00012720: 7666 732e 6765 745f 6462 7628 7265 6d29  vfs.get_dbv(rem)
+00012730: 5b30 5d2e 6c69 6d0a 2020 2020 2020 2020  [0].lim.        
+00012740: 6966 206c 696d 3a0a 2020 2020 2020 2020  if lim:.        
+00012750: 2020 2020 6670 2c20 7270 203d 206c 696d      fp, rp = lim
+00012760: 2e61 6c6c 2873 656c 662e 6970 2c20 7270  .all(self.ip, rp
+00012770: 2c20 636c 656e 2c20 6670 290a 2020 2020  , clen, fp).    
+00012780: 2020 2020 2020 2020 626f 732e 6d61 6b65          bos.make
+00012790: 6469 7273 2866 7029 0a0a 2020 2020 2020  dirs(fp)..      
+000127a0: 2020 6670 203d 206f 732e 7061 7468 2e6a    fp = os.path.j
+000127b0: 6f69 6e28 6670 2c20 666e 290a 2020 2020  oin(fp, fn).    
+000127c0: 2020 2020 7265 6d20 3d20 227b 7d2f 7b7d      rem = "{}/{}
+000127d0: 222e 666f 726d 6174 2872 702c 2066 6e29  ".format(rp, fn)
+000127e0: 2e73 7472 6970 2822 2f22 290a 0a20 2020  .strip("/")..   
+000127f0: 2020 2020 2069 6620 6e6f 7420 7265 6d2e       if not rem.
+00012800: 656e 6473 7769 7468 2822 2e6d 6422 293a  endswith(".md"):
+00012810: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00012820: 7365 2050 6562 6b61 6328 3430 302c 2022  se Pebkac(400, "
+00012830: 6f6e 6c79 206d 6172 6b64 6f77 6e20 706c  only markdown pl
+00012840: 7322 290a 0a20 2020 2020 2020 2069 6620  s")..        if 
+00012850: 6e75 6c6c 7772 6974 653a 0a20 2020 2020  nullwrite:.     
+00012860: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+00012870: 3d20 6a73 6f6e 2e64 756d 7073 287b 226f  = json.dumps({"o
+00012880: 6b22 3a20 5472 7565 2c20 226c 6173 746d  k": True, "lastm
+00012890: 6f64 223a 2030 7d29 0a20 2020 2020 2020  od": 0}).       
+000128a0: 2020 2020 2073 656c 662e 6c6f 6728 7265       self.log(re
+000128b0: 7370 6f6e 7365 290a 2020 2020 2020 2020  sponse).        
+000128c0: 2020 2020 2320 544f 444f 2072 6570 6c79      # TODO reply
+000128d0: 2073 686f 756c 6420 7061 7273 6572 2e64   should parser.d
+000128e0: 726f 7028 290a 2020 2020 2020 2020 2020  rop().          
+000128f0: 2020 7365 6c66 2e70 6172 7365 722e 6472    self.parser.dr
+00012900: 6f70 2829 0a20 2020 2020 2020 2020 2020  op().           
+00012910: 2073 656c 662e 7265 706c 7928 7265 7370   self.reply(resp
+00012920: 6f6e 7365 2e65 6e63 6f64 6528 2275 7466  onse.encode("utf
+00012930: 2d38 2229 290a 2020 2020 2020 2020 2020  -8")).          
+00012940: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+00012950: 2020 2020 2020 2073 7276 5f6c 6173 746d         srv_lastm
+00012960: 6f64 203d 202d 312e 300a 2020 2020 2020  od = -1.0.      
+00012970: 2020 7372 765f 6c61 7374 6d6f 6433 203d    srv_lastmod3 =
+00012980: 202d 310a 2020 2020 2020 2020 7472 793a   -1.        try:
+00012990: 0a20 2020 2020 2020 2020 2020 2073 7420  .            st 
+000129a0: 3d20 626f 732e 7374 6174 2866 7029 0a20  = bos.stat(fp). 
+000129b0: 2020 2020 2020 2020 2020 2073 7276 5f6c             srv_l
+000129c0: 6173 746d 6f64 203d 2073 742e 7374 5f6d  astmod = st.st_m
+000129d0: 7469 6d65 0a20 2020 2020 2020 2020 2020  time.           
+000129e0: 2073 7276 5f6c 6173 746d 6f64 3320 3d20   srv_lastmod3 = 
+000129f0: 696e 7428 7372 765f 6c61 7374 6d6f 6420  int(srv_lastmod 
+00012a00: 2a20 3130 3030 290a 2020 2020 2020 2020  * 1000).        
+00012a10: 6578 6365 7074 204f 5345 7272 6f72 2061  except OSError a
+00012a20: 7320 6578 3a0a 2020 2020 2020 2020 2020  s ex:.          
+00012a30: 2020 6966 2065 782e 6572 726e 6f20 213d    if ex.errno !=
+00012a40: 2065 7272 6e6f 2e45 4e4f 454e 543a 0a20   errno.ENOENT:. 
+00012a50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00012a60: 6169 7365 0a0a 2020 2020 2020 2020 2320  aise..        # 
+00012a70: 6966 2066 696c 6520 6578 6973 7473 2c20  if file exists, 
+00012a80: 6368 656b 6320 7468 6174 2074 696d 6573  chekc that times
+00012a90: 7461 6d70 206d 6174 6368 6573 2074 6865  tamp matches the
+00012aa0: 2063 6c69 656e 7427 730a 2020 2020 2020   client's.      
+00012ab0: 2020 6966 2073 7276 5f6c 6173 746d 6f64    if srv_lastmod
+00012ac0: 203e 3d20 303a 0a20 2020 2020 2020 2020   >= 0:.         
+00012ad0: 2020 2073 616d 655f 6c61 7374 6d6f 6420     same_lastmod 
+00012ae0: 3d20 636c 695f 6c61 7374 6d6f 6433 2069  = cli_lastmod3 i
+00012af0: 6e20 5b2d 312c 2073 7276 5f6c 6173 746d  n [-1, srv_lastm
+00012b00: 6f64 335d 0a20 2020 2020 2020 2020 2020  od3].           
+00012b10: 2069 6620 6e6f 7420 7361 6d65 5f6c 6173   if not same_las
+00012b20: 746d 6f64 3a0a 2020 2020 2020 2020 2020  tmod:.          
+00012b30: 2020 2020 2020 2320 736f 6d65 2066 696c        # some fil
+00012b40: 6573 7973 7465 6d73 2f74 7261 6e73 706f  esystems/transpo
+00012b50: 7274 7320 6c69 6d69 7420 7072 6563 6973  rts limit precis
+00012b60: 696f 6e20 746f 2031 7365 632c 2068 6f70  ion to 1sec, hop
+00012b70: 6566 756c 6c79 2066 6c6f 6f72 6564 0a20  efully floored. 
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012b90: 616d 655f 6c61 7374 6d6f 6420 3d20 280a  ame_lastmod = (.
 00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bb0: 2020 2061 6e64 2063 6c69 5f6c 6173 746d     and cli_lastm
-00012bc0: 6f64 3320 3e20 7372 765f 6c61 7374 6d6f  od3 > srv_lastmo
-00012bd0: 6433 0a20 2020 2020 2020 2020 2020 2020  d3.             
-00012be0: 2020 2020 2020 2061 6e64 2063 6c69 5f6c         and cli_l
-00012bf0: 6173 746d 6f64 3320 2d20 7372 765f 6c61  astmod3 - srv_la
-00012c00: 7374 6d6f 6433 203c 2031 3030 300a 2020  stmod3 < 1000.  
-00012c10: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00012c20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00012c30: 6e6f 7420 7361 6d65 5f6c 6173 746d 6f64  not same_lastmod
-00012c40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012c50: 2020 7265 7370 6f6e 7365 203d 206a 736f    response = jso
-00012c60: 6e2e 6475 6d70 7328 0a20 2020 2020 2020  n.dumps(.       
-00012c70: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c90: 2020 2020 2020 2022 6f6b 223a 2046 616c         "ok": Fal
-00012ca0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00012cb0: 2020 2020 2020 2020 2020 2020 226c 6173              "las
-00012cc0: 746d 6f64 223a 2073 7276 5f6c 6173 746d  tmod": srv_lastm
-00012cd0: 6f64 332c 0a20 2020 2020 2020 2020 2020  od3,.           
-00012ce0: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
-00012cf0: 7722 3a20 696e 7428 7469 6d65 2e74 696d  w": int(time.tim
-00012d00: 6528 2920 2a20 3130 3030 292c 0a20 2020  e() * 1000),.   
-00012d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d20: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00012d30: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00012d40: 2020 2020 2073 656c 662e 6c6f 6728 0a20       self.log(. 
-00012d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d60: 2020 2022 7b7d 202d 207b 7d20 3d20 7b7d     "{} - {} = {}
-00012d70: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
-00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d90: 2020 7372 765f 6c61 7374 6d6f 6433 2c20    srv_lastmod3, 
-00012da0: 636c 695f 6c61 7374 6d6f 6433 2c20 7372  cli_lastmod3, sr
-00012db0: 765f 6c61 7374 6d6f 6433 202d 2063 6c69  v_lastmod3 - cli
-00012dc0: 5f6c 6173 746d 6f64 330a 2020 2020 2020  _lastmod3.      
-00012dd0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012df0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012e00: 2020 7365 6c66 2e6c 6f67 2872 6573 706f    self.log(respo
-00012e10: 6e73 6529 0a20 2020 2020 2020 2020 2020  nse).           
-00012e20: 2020 2020 2073 656c 662e 7061 7273 6572       self.parser
-00012e30: 2e64 726f 7028 290a 2020 2020 2020 2020  .drop().        
-00012e40: 2020 2020 2020 2020 7365 6c66 2e72 6570          self.rep
-00012e50: 6c79 2872 6573 706f 6e73 652e 656e 636f  ly(response.enco
-00012e60: 6465 2822 7574 662d 3822 2929 0a20 2020  de("utf-8")).   
-00012e70: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00012e80: 7572 6e20 5472 7565 0a0a 2020 2020 2020  urn True..      
-00012e90: 2020 2020 2020 6d64 6972 2c20 6d66 696c        mdir, mfil
-00012ea0: 6520 3d20 6f73 2e70 6174 682e 7370 6c69  e = os.path.spli
-00012eb0: 7428 6670 290a 2020 2020 2020 2020 2020  t(fp).          
-00012ec0: 2020 6d66 696c 6532 203d 2022 7b7d 2e7b    mfile2 = "{}.{
-00012ed0: 3a2e 3366 7d2e 6d64 222e 666f 726d 6174  :.3f}.md".format
-00012ee0: 286d 6669 6c65 5b3a 2d33 5d2c 2073 7276  (mfile[:-3], srv
-00012ef0: 5f6c 6173 746d 6f64 290a 2020 2020 2020  _lastmod).      
-00012f00: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00012f10: 2020 2020 2020 2020 2020 2064 7020 3d20             dp = 
-00012f20: 6f73 2e70 6174 682e 6a6f 696e 286d 6469  os.path.join(mdi
-00012f30: 722c 2022 2e68 6973 7422 290a 2020 2020  r, ".hist").    
-00012f40: 2020 2020 2020 2020 2020 2020 626f 732e              bos.
-00012f50: 6d6b 6469 7228 6470 290a 2020 2020 2020  mkdir(dp).      
-00012f60: 2020 2020 2020 2020 2020 6869 6465 6469            hidedi
-00012f70: 7228 6470 290a 2020 2020 2020 2020 2020  r(dp).          
-00012f80: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-00012f90: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
-00012fa0: 2020 2020 2020 2020 2020 2062 6f73 2e72             bos.r
-00012fb0: 656e 616d 6528 6670 2c20 6f73 2e70 6174  ename(fp, os.pat
-00012fc0: 682e 6a6f 696e 286d 6469 722c 2022 2e68  h.join(mdir, ".h
-00012fd0: 6973 7422 2c20 6d66 696c 6532 2929 0a0a  ist", mfile2))..
-00012fe0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00012ff0: 656c 662e 7061 7273 6572 2e67 656e 0a20  elf.parser.gen. 
-00013000: 2020 2020 2020 2070 5f66 6965 6c64 2c20         p_field, 
-00013010: 5f2c 2070 5f64 6174 6120 3d20 6e65 7874  _, p_data = next
-00013020: 2873 656c 662e 7061 7273 6572 2e67 656e  (self.parser.gen
-00013030: 290a 2020 2020 2020 2020 6966 2070 5f66  ).        if p_f
-00013040: 6965 6c64 2021 3d20 2262 6f64 7922 3a0a  ield != "body":.
-00013050: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00013060: 6520 5065 626b 6163 2834 3030 2c20 2265  e Pebkac(400, "e
-00013070: 7870 6563 7465 6420 626f 6479 2c20 676f  xpected body, go
-00013080: 7420 7b7d 222e 666f 726d 6174 2870 5f66  t {}".format(p_f
-00013090: 6965 6c64 2929 0a0a 2020 2020 2020 2020  ield))..        
-000130a0: 6966 2062 6f73 2e70 6174 682e 6578 6973  if bos.path.exis
-000130b0: 7473 2866 7029 3a0a 2020 2020 2020 2020  ts(fp):.        
-000130c0: 2020 2020 626f 732e 756e 6c69 6e6b 2866      bos.unlink(f
-000130d0: 7029 0a0a 2020 2020 2020 2020 7769 7468  p)..        with
-000130e0: 206f 7065 6e28 6673 656e 6328 6670 292c   open(fsenc(fp),
-000130f0: 2022 7762 222c 2035 3132 202a 2031 3032   "wb", 512 * 102
-00013100: 3429 2061 7320 663a 0a20 2020 2020 2020  4) as f:.       
-00013110: 2020 2020 2073 7a2c 2073 6861 3531 322c       sz, sha512,
-00013120: 205f 203d 2068 6173 6863 6f70 7928 705f   _ = hashcopy(p_
-00013130: 6461 7461 2c20 662c 2073 656c 662e 6172  data, f, self.ar
-00013140: 6773 2e73 5f77 725f 736c 7029 0a0a 2020  gs.s_wr_slp)..  
-00013150: 2020 2020 2020 6966 206c 696d 3a0a 2020        if lim:.  
-00013160: 2020 2020 2020 2020 2020 6c69 6d2e 6e75            lim.nu
-00013170: 7028 7365 6c66 2e69 7029 0a20 2020 2020  p(self.ip).     
-00013180: 2020 2020 2020 206c 696d 2e62 7570 2873         lim.bup(s
-00013190: 656c 662e 6970 2c20 737a 290a 2020 2020  elf.ip, sz).    
-000131a0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-000131b0: 2020 2020 2020 2020 2020 2020 206c 696d               lim
-000131c0: 2e63 686b 5f73 7a28 737a 290a 2020 2020  .chk_sz(sz).    
-000131d0: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131f0: 626f 732e 756e 6c69 6e6b 2866 7029 0a20  bos.unlink(fp). 
-00013200: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00013210: 6169 7365 0a0a 2020 2020 2020 2020 6e65  aise..        ne
-00013220: 775f 6c61 7374 6d6f 6420 3d20 626f 732e  w_lastmod = bos.
-00013230: 7374 6174 2866 7029 2e73 745f 6d74 696d  stat(fp).st_mtim
-00013240: 650a 2020 2020 2020 2020 6e65 775f 6c61  e.        new_la
-00013250: 7374 6d6f 6433 203d 2069 6e74 286e 6577  stmod3 = int(new
-00013260: 5f6c 6173 746d 6f64 202a 2031 3030 3029  _lastmod * 1000)
-00013270: 0a20 2020 2020 2020 2073 6861 3531 3220  .        sha512 
-00013280: 3d20 7368 6135 3132 5b3a 3536 5d0a 0a20  = sha512[:56].. 
-00013290: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-000132a0: 3d20 6a73 6f6e 2e64 756d 7073 280a 2020  = json.dumps(.  
-000132b0: 2020 2020 2020 2020 2020 7b22 6f6b 223a            {"ok":
-000132c0: 2054 7275 652c 2022 6c61 7374 6d6f 6422   True, "lastmod"
-000132d0: 3a20 6e65 775f 6c61 7374 6d6f 6433 2c20  : new_lastmod3, 
-000132e0: 2273 697a 6522 3a20 737a 2c20 2273 6861  "size": sz, "sha
-000132f0: 3531 3222 3a20 7368 6135 3132 7d0a 2020  512": sha512}.  
-00013300: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00013310: 7365 6c66 2e6c 6f67 2872 6573 706f 6e73  self.log(respons
-00013320: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00013330: 7061 7273 6572 2e64 726f 7028 290a 2020  parser.drop().  
-00013340: 2020 2020 2020 7365 6c66 2e72 6570 6c79        self.reply
-00013350: 2872 6573 706f 6e73 652e 656e 636f 6465  (response.encode
-00013360: 2822 7574 662d 3822 2929 0a20 2020 2020  ("utf-8")).     
-00013370: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00013380: 2020 2020 6465 6620 5f63 686b 5f6c 6173      def _chk_las
-00013390: 746d 6f64 2873 656c 662c 2066 696c 655f  tmod(self, file_
-000133a0: 7473 2029 2020 203a 0a20 2020 2020 2020  ts )   :.       
-000133b0: 2066 696c 655f 6c61 7374 6d6f 6420 3d20   file_lastmod = 
-000133c0: 666f 726d 6174 6461 7465 2866 696c 655f  formatdate(file_
-000133d0: 7473 2c20 7573 6567 6d74 3d54 7275 6529  ts, usegmt=True)
-000133e0: 0a20 2020 2020 2020 2063 6c69 5f6c 6173  .        cli_las
-000133f0: 746d 6f64 203d 2073 656c 662e 6865 6164  tmod = self.head
-00013400: 6572 732e 6765 7428 2269 662d 6d6f 6469  ers.get("if-modi
-00013410: 6669 6564 2d73 696e 6365 2229 0a20 2020  fied-since").   
-00013420: 2020 2020 2069 6620 636c 695f 6c61 7374       if cli_last
-00013430: 6d6f 643a 0a20 2020 2020 2020 2020 2020  mod:.           
-00013440: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00013450: 2020 2020 2020 2320 736f 6d65 2062 726f        # some bro
-00013460: 7773 6572 2061 7070 656e 6420 223b 206c  wser append "; l
-00013470: 656e 6774 683d 3537 3322 0a20 2020 2020  ength=573".     
-00013480: 2020 2020 2020 2020 2020 2063 6c69 5f6c             cli_l
-00013490: 6173 746d 6f64 203d 2063 6c69 5f6c 6173  astmod = cli_las
-000134a0: 746d 6f64 2e73 706c 6974 2822 3b22 295b  tmod.split(";")[
-000134b0: 305d 2e73 7472 6970 2829 0a20 2020 2020  0].strip().     
-000134c0: 2020 2020 2020 2020 2020 2063 6c69 5f64             cli_d
-000134d0: 7420 3d20 7061 7273 6564 6174 6528 636c  t = parsedate(cl
-000134e0: 695f 6c61 7374 6d6f 6429 0a20 2020 2020  i_lastmod).     
-000134f0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00013500: 7420 636c 695f 6474 0a20 2020 2020 2020  t cli_dt.       
-00013510: 2020 2020 2020 2020 2063 6c69 5f74 7320           cli_ts 
-00013520: 3d20 6361 6c65 6e64 6172 2e74 696d 6567  = calendar.timeg
-00013530: 6d28 636c 695f 6474 290a 2020 2020 2020  m(cli_dt).      
-00013540: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00013550: 2066 696c 655f 6c61 7374 6d6f 642c 2069   file_lastmod, i
-00013560: 6e74 2866 696c 655f 7473 2920 3e20 696e  nt(file_ts) > in
-00013570: 7428 636c 695f 7473 290a 2020 2020 2020  t(cli_ts).      
-00013580: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00013590: 6570 7469 6f6e 2061 7320 6578 3a0a 2020  eption as ex:.  
-000135a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000135b0: 6c66 2e6c 6f67 280a 2020 2020 2020 2020  lf.log(.        
-000135c0: 2020 2020 2020 2020 2020 2020 226c 6173              "las
-000135d0: 746d 6f64 207b 7d5c 6e72 656d 6f74 653a  tmod {}\nremote:
-000135e0: 205b 7b7d 5d5c 6e20 6c6f 6361 6c3a 205b   [{}]\n local: [
-000135f0: 7b7d 5d22 2e66 6f72 6d61 7428 0a20 2020  {}]".format(.   
-00013600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013610: 2020 2020 2072 6570 7228 6578 292c 2063       repr(ex), c
-00013620: 6c69 5f6c 6173 746d 6f64 2c20 6669 6c65  li_lastmod, file
-00013630: 5f6c 6173 746d 6f64 0a20 2020 2020 2020  _lastmod.       
-00013640: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00013650: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00013660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013670: 2072 6574 7572 6e20 6669 6c65 5f6c 6173   return file_las
-00013680: 746d 6f64 2c20 6669 6c65 5f6c 6173 746d  tmod, file_lastm
-00013690: 6f64 2021 3d20 636c 695f 6c61 7374 6d6f  od != cli_lastmo
-000136a0: 640a 0a20 2020 2020 2020 2072 6574 7572  d..        retur
-000136b0: 6e20 6669 6c65 5f6c 6173 746d 6f64 2c20  n file_lastmod, 
-000136c0: 5472 7565 0a0a 2020 2020 6465 6620 7478  True..    def tx
-000136d0: 5f66 696c 6528 7365 6c66 2c20 7265 715f  _file(self, req_
-000136e0: 7061 7468 2029 2020 3a0a 2020 2020 2020  path )  :.      
-000136f0: 2020 7374 6174 7573 203d 2032 3030 0a20    status = 200. 
-00013700: 2020 2020 2020 206c 6f67 6d73 6720 3d20         logmsg = 
-00013710: 227b 3a34 7d20 7b7d 2022 2e66 6f72 6d61  "{:4} {} ".forma
-00013720: 7428 2222 2c20 7365 6c66 2e72 6571 290a  t("", self.req).
-00013730: 2020 2020 2020 2020 6c6f 6774 6169 6c20          logtail 
-00013740: 3d20 2222 0a0a 2020 2020 2020 2020 230a  = ""..        #.
-00013750: 2020 2020 2020 2020 2320 6966 2072 6571          # if req
-00013760: 7565 7374 2069 7320 666f 7220 666f 6f2e  uest is for foo.
-00013770: 6a73 2c20 6368 6563 6b20 6966 2077 6520  js, check if we 
-00013780: 6861 7665 2066 6f6f 2e6a 732e 7b67 7a2c  have foo.js.{gz,
-00013790: 6272 7d0a 0a20 2020 2020 2020 2066 696c  br}..        fil
-000137a0: 655f 7473 203d 2030 0a20 2020 2020 2020  e_ts = 0.       
-000137b0: 2065 6469 7469 6f6e 7320 2020 203d 207b   editions    = {
-000137c0: 7d0a 2020 2020 2020 2020 666f 7220 6578  }.        for ex
-000137d0: 7420 696e 205b 2222 2c20 222e 677a 222c  t in ["", ".gz",
-000137e0: 2022 2e62 7222 5d3a 0a20 2020 2020 2020   ".br"]:.       
-000137f0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00013800: 2020 2020 2020 2020 2020 6673 5f70 6174            fs_pat
-00013810: 6820 3d20 7265 715f 7061 7468 202b 2065  h = req_path + e
-00013820: 7874 0a20 2020 2020 2020 2020 2020 2020  xt.             
-00013830: 2020 2073 7420 3d20 626f 732e 7374 6174     st = bos.stat
-00013840: 2866 735f 7061 7468 290a 2020 2020 2020  (fs_path).      
-00013850: 2020 2020 2020 2020 2020 6966 2073 7461            if sta
-00013860: 742e 535f 4953 4449 5228 7374 2e73 745f  t.S_ISDIR(st.st_
-00013870: 6d6f 6465 293a 0a20 2020 2020 2020 2020  mode):.         
-00013880: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00013890: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
-000138a0: 2020 2020 2069 6620 7374 6174 2e53 5f49       if stat.S_I
-000138b0: 5342 4c4b 2873 742e 7374 5f6d 6f64 6529  SBLK(st.st_mode)
-000138c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000138d0: 2020 2020 2020 6664 203d 2062 6f73 2e6f        fd = bos.o
-000138e0: 7065 6e28 6673 5f70 6174 682c 206f 732e  pen(fs_path, os.
-000138f0: 4f5f 5244 4f4e 4c59 290a 2020 2020 2020  O_RDONLY).      
-00013900: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00013910: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00013920: 2020 2020 2020 2020 2020 2073 7a20 3d20             sz = 
-00013930: 6f73 2e6c 7365 656b 2866 642c 2030 2c20  os.lseek(fd, 0, 
-00013940: 6f73 2e53 4545 4b5f 454e 4429 0a20 2020  os.SEEK_END).   
+00012bb0: 2020 2020 7372 765f 6c61 7374 6d6f 6420      srv_lastmod 
+00012bc0: 3d3d 2069 6e74 2863 6c69 5f6c 6173 746d  == int(cli_lastm
+00012bd0: 6f64 3320 2f20 3130 3030 290a 2020 2020  od3 / 1000).    
+00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bf0: 616e 6420 636c 695f 6c61 7374 6d6f 6433  and cli_lastmod3
+00012c00: 203e 2073 7276 5f6c 6173 746d 6f64 330a   > srv_lastmod3.
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 2020 2020 616e 6420 636c 695f 6c61 7374      and cli_last
+00012c30: 6d6f 6433 202d 2073 7276 5f6c 6173 746d  mod3 - srv_lastm
+00012c40: 6f64 3320 3c20 3130 3030 0a20 2020 2020  od3 < 1000.     
+00012c50: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00012c60: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00012c70: 2073 616d 655f 6c61 7374 6d6f 643a 0a20   same_lastmod:. 
+00012c80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00012c90: 6573 706f 6e73 6520 3d20 6a73 6f6e 2e64  esponse = json.d
+00012ca0: 756d 7073 280a 2020 2020 2020 2020 2020  umps(.          
+00012cb0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00012cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cd0: 2020 2020 226f 6b22 3a20 4661 6c73 652c      "ok": False,
+00012ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012cf0: 2020 2020 2020 2020 2022 6c61 7374 6d6f           "lastmo
+00012d00: 6422 3a20 7372 765f 6c61 7374 6d6f 6433  d": srv_lastmod3
+00012d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012d20: 2020 2020 2020 2020 2020 226e 6f77 223a            "now":
+00012d30: 2069 6e74 2874 696d 652e 7469 6d65 2829   int(time.time()
+00012d40: 202a 2031 3030 3029 2c0a 2020 2020 2020   * 1000),.      
+00012d50: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00012d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012d80: 2020 7365 6c66 2e6c 6f67 280a 2020 2020    self.log(.    
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 227b 7d20 2d20 7b7d 203d 207b 7d22 2e66  "{} - {} = {}".f
+00012db0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+00012dc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012dd0: 7276 5f6c 6173 746d 6f64 332c 2063 6c69  rv_lastmod3, cli
+00012de0: 5f6c 6173 746d 6f64 332c 2073 7276 5f6c  _lastmod3, srv_l
+00012df0: 6173 746d 6f64 3320 2d20 636c 695f 6c61  astmod3 - cli_la
+00012e00: 7374 6d6f 6433 0a20 2020 2020 2020 2020  stmod3.         
+00012e10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00012e20: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012e40: 656c 662e 6c6f 6728 7265 7370 6f6e 7365  elf.log(response
+00012e50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012e60: 2020 7365 6c66 2e70 6172 7365 722e 6472    self.parser.dr
+00012e70: 6f70 2829 0a20 2020 2020 2020 2020 2020  op().           
+00012e80: 2020 2020 2073 656c 662e 7265 706c 7928       self.reply(
+00012e90: 7265 7370 6f6e 7365 2e65 6e63 6f64 6528  response.encode(
+00012ea0: 2275 7466 2d38 2229 290a 2020 2020 2020  "utf-8")).      
+00012eb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00012ec0: 2054 7275 650a 0a20 2020 2020 2020 2020   True..         
+00012ed0: 2020 206d 6469 722c 206d 6669 6c65 203d     mdir, mfile =
+00012ee0: 206f 732e 7061 7468 2e73 706c 6974 2866   os.path.split(f
+00012ef0: 7029 0a20 2020 2020 2020 2020 2020 206d  p).            m
+00012f00: 6669 6c65 3220 3d20 227b 7d2e 7b3a 2e33  file2 = "{}.{:.3
+00012f10: 667d 2e6d 6422 2e66 6f72 6d61 7428 6d66  f}.md".format(mf
+00012f20: 696c 655b 3a2d 335d 2c20 7372 765f 6c61  ile[:-3], srv_la
+00012f30: 7374 6d6f 6429 0a20 2020 2020 2020 2020  stmod).         
+00012f40: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00012f50: 2020 2020 2020 2020 6470 203d 206f 732e          dp = os.
+00012f60: 7061 7468 2e6a 6f69 6e28 6d64 6972 2c20  path.join(mdir, 
+00012f70: 222e 6869 7374 2229 0a20 2020 2020 2020  ".hist").       
+00012f80: 2020 2020 2020 2020 2062 6f73 2e6d 6b64           bos.mkd
+00012f90: 6972 2864 7029 0a20 2020 2020 2020 2020  ir(dp).         
+00012fa0: 2020 2020 2020 2068 6964 6564 6972 2864         hidedir(d
+00012fb0: 7029 0a20 2020 2020 2020 2020 2020 2065  p).            e
+00012fc0: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+00012fd0: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00012fe0: 2020 2020 2020 2020 626f 732e 7265 6e61          bos.rena
+00012ff0: 6d65 2866 702c 206f 732e 7061 7468 2e6a  me(fp, os.path.j
+00013000: 6f69 6e28 6d64 6972 2c20 222e 6869 7374  oin(mdir, ".hist
+00013010: 222c 206d 6669 6c65 3229 290a 0a20 2020  ", mfile2))..   
+00013020: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+00013030: 2e70 6172 7365 722e 6765 6e0a 2020 2020  .parser.gen.    
+00013040: 2020 2020 705f 6669 656c 642c 205f 2c20      p_field, _, 
+00013050: 705f 6461 7461 203d 206e 6578 7428 7365  p_data = next(se
+00013060: 6c66 2e70 6172 7365 722e 6765 6e29 0a20  lf.parser.gen). 
+00013070: 2020 2020 2020 2069 6620 705f 6669 656c         if p_fiel
+00013080: 6420 213d 2022 626f 6479 223a 0a20 2020  d != "body":.   
+00013090: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
+000130a0: 6562 6b61 6328 3430 302c 2022 6578 7065  ebkac(400, "expe
+000130b0: 6374 6564 2062 6f64 792c 2067 6f74 207b  cted body, got {
+000130c0: 7d22 2e66 6f72 6d61 7428 705f 6669 656c  }".format(p_fiel
+000130d0: 6429 290a 0a20 2020 2020 2020 2069 6620  d))..        if 
+000130e0: 626f 732e 7061 7468 2e65 7869 7374 7328  bos.path.exists(
+000130f0: 6670 293a 0a20 2020 2020 2020 2020 2020  fp):.           
+00013100: 2062 6f73 2e75 6e6c 696e 6b28 6670 290a   bos.unlink(fp).
+00013110: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
+00013120: 656e 2866 7365 6e63 2866 7029 2c20 2277  en(fsenc(fp), "w
+00013130: 6222 2c20 3531 3220 2a20 3130 3234 2920  b", 512 * 1024) 
+00013140: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
+00013150: 2020 737a 2c20 7368 6135 3132 2c20 5f20    sz, sha512, _ 
+00013160: 3d20 6861 7368 636f 7079 2870 5f64 6174  = hashcopy(p_dat
+00013170: 612c 2066 2c20 7365 6c66 2e61 7267 732e  a, f, self.args.
+00013180: 735f 7772 5f73 6c70 290a 0a20 2020 2020  s_wr_slp)..     
+00013190: 2020 2069 6620 6c69 6d3a 0a20 2020 2020     if lim:.     
+000131a0: 2020 2020 2020 206c 696d 2e6e 7570 2873         lim.nup(s
+000131b0: 656c 662e 6970 290a 2020 2020 2020 2020  elf.ip).        
+000131c0: 2020 2020 6c69 6d2e 6275 7028 7365 6c66      lim.bup(self
+000131d0: 2e69 702c 2073 7a29 0a20 2020 2020 2020  .ip, sz).       
+000131e0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000131f0: 2020 2020 2020 2020 2020 6c69 6d2e 6368            lim.ch
+00013200: 6b5f 737a 2873 7a29 0a20 2020 2020 2020  k_sz(sz).       
+00013210: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+00013220: 2020 2020 2020 2020 2020 2020 2062 6f73               bos
+00013230: 2e75 6e6c 696e 6b28 6670 290a 2020 2020  .unlink(fp).    
+00013240: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00013250: 650a 0a20 2020 2020 2020 206e 6577 5f6c  e..        new_l
+00013260: 6173 746d 6f64 203d 2062 6f73 2e73 7461  astmod = bos.sta
+00013270: 7428 6670 292e 7374 5f6d 7469 6d65 0a20  t(fp).st_mtime. 
+00013280: 2020 2020 2020 206e 6577 5f6c 6173 746d         new_lastm
+00013290: 6f64 3320 3d20 696e 7428 6e65 775f 6c61  od3 = int(new_la
+000132a0: 7374 6d6f 6420 2a20 3130 3030 290a 2020  stmod * 1000).  
+000132b0: 2020 2020 2020 7368 6135 3132 203d 2073        sha512 = s
+000132c0: 6861 3531 325b 3a35 365d 0a0a 2020 2020  ha512[:56]..    
+000132d0: 2020 2020 7265 7370 6f6e 7365 203d 206a      response = j
+000132e0: 736f 6e2e 6475 6d70 7328 0a20 2020 2020  son.dumps(.     
+000132f0: 2020 2020 2020 207b 226f 6b22 3a20 5472         {"ok": Tr
+00013300: 7565 2c20 226c 6173 746d 6f64 223a 206e  ue, "lastmod": n
+00013310: 6577 5f6c 6173 746d 6f64 332c 2022 7369  ew_lastmod3, "si
+00013320: 7a65 223a 2073 7a2c 2022 7368 6135 3132  ze": sz, "sha512
+00013330: 223a 2073 6861 3531 327d 0a20 2020 2020  ": sha512}.     
+00013340: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00013350: 662e 6c6f 6728 7265 7370 6f6e 7365 290a  f.log(response).
+00013360: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
+00013370: 7365 722e 6472 6f70 2829 0a20 2020 2020  ser.drop().     
+00013380: 2020 2073 656c 662e 7265 706c 7928 7265     self.reply(re
+00013390: 7370 6f6e 7365 2e65 6e63 6f64 6528 2275  sponse.encode("u
+000133a0: 7466 2d38 2229 290a 2020 2020 2020 2020  tf-8")).        
+000133b0: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+000133c0: 2064 6566 205f 6368 6b5f 6c61 7374 6d6f   def _chk_lastmo
+000133d0: 6428 7365 6c66 2c20 6669 6c65 5f74 7320  d(self, file_ts 
+000133e0: 2920 2020 3a0a 2020 2020 2020 2020 6669  )   :.        fi
+000133f0: 6c65 5f6c 6173 746d 6f64 203d 2066 6f72  le_lastmod = for
+00013400: 6d61 7464 6174 6528 6669 6c65 5f74 732c  matdate(file_ts,
+00013410: 2075 7365 676d 743d 5472 7565 290a 2020   usegmt=True).  
+00013420: 2020 2020 2020 636c 695f 6c61 7374 6d6f        cli_lastmo
+00013430: 6420 3d20 7365 6c66 2e68 6561 6465 7273  d = self.headers
+00013440: 2e67 6574 2822 6966 2d6d 6f64 6966 6965  .get("if-modifie
+00013450: 642d 7369 6e63 6522 290a 2020 2020 2020  d-since").      
+00013460: 2020 6966 2063 6c69 5f6c 6173 746d 6f64    if cli_lastmod
+00013470: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
+00013480: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00013490: 2020 2023 2073 6f6d 6520 6272 6f77 7365     # some browse
+000134a0: 7220 6170 7065 6e64 2022 3b20 6c65 6e67  r append "; leng
+000134b0: 7468 3d35 3733 220a 2020 2020 2020 2020  th=573".        
+000134c0: 2020 2020 2020 2020 636c 695f 6c61 7374          cli_last
+000134d0: 6d6f 6420 3d20 636c 695f 6c61 7374 6d6f  mod = cli_lastmo
+000134e0: 642e 7370 6c69 7428 223b 2229 5b30 5d2e  d.split(";")[0].
+000134f0: 7374 7269 7028 290a 2020 2020 2020 2020  strip().        
+00013500: 2020 2020 2020 2020 636c 695f 6474 203d          cli_dt =
+00013510: 2070 6172 7365 6461 7465 2863 6c69 5f6c   parsedate(cli_l
+00013520: 6173 746d 6f64 290a 2020 2020 2020 2020  astmod).        
+00013530: 2020 2020 2020 2020 6173 7365 7274 2063          assert c
+00013540: 6c69 5f64 740a 2020 2020 2020 2020 2020  li_dt.          
+00013550: 2020 2020 2020 636c 695f 7473 203d 2063        cli_ts = c
+00013560: 616c 656e 6461 722e 7469 6d65 676d 2863  alendar.timegm(c
+00013570: 6c69 5f64 7429 0a20 2020 2020 2020 2020  li_dt).         
+00013580: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
+00013590: 6c65 5f6c 6173 746d 6f64 2c20 696e 7428  le_lastmod, int(
+000135a0: 6669 6c65 5f74 7329 203e 2069 6e74 2863  file_ts) > int(c
+000135b0: 6c69 5f74 7329 0a20 2020 2020 2020 2020  li_ts).         
+000135c0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+000135d0: 696f 6e20 6173 2065 783a 0a20 2020 2020  ion as ex:.     
+000135e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000135f0: 6c6f 6728 0a20 2020 2020 2020 2020 2020  log(.           
+00013600: 2020 2020 2020 2020 2022 6c61 7374 6d6f           "lastmo
+00013610: 6420 7b7d 5c6e 7265 6d6f 7465 3a20 5b7b  d {}\nremote: [{
+00013620: 7d5d 5c6e 206c 6f63 616c 3a20 5b7b 7d5d  }]\n local: [{}]
+00013630: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
+00013640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013650: 2020 7265 7072 2865 7829 2c20 636c 695f    repr(ex), cli_
+00013660: 6c61 7374 6d6f 642c 2066 696c 655f 6c61  lastmod, file_la
+00013670: 7374 6d6f 640a 2020 2020 2020 2020 2020  stmod.          
+00013680: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00013690: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000136a0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000136b0: 7475 726e 2066 696c 655f 6c61 7374 6d6f  turn file_lastmo
+000136c0: 642c 2066 696c 655f 6c61 7374 6d6f 6420  d, file_lastmod 
+000136d0: 213d 2063 6c69 5f6c 6173 746d 6f64 0a0a  != cli_lastmod..
+000136e0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+000136f0: 696c 655f 6c61 7374 6d6f 642c 2054 7275  ile_lastmod, Tru
+00013700: 650a 0a20 2020 2064 6566 2074 785f 6669  e..    def tx_fi
+00013710: 6c65 2873 656c 662c 2072 6571 5f70 6174  le(self, req_pat
+00013720: 6820 2920 203a 0a20 2020 2020 2020 2073  h )  :.        s
+00013730: 7461 7475 7320 3d20 3230 300a 2020 2020  tatus = 200.    
+00013740: 2020 2020 6c6f 676d 7367 203d 2022 7b3a      logmsg = "{:
+00013750: 347d 207b 7d20 222e 666f 726d 6174 2822  4} {} ".format("
+00013760: 222c 2073 656c 662e 7265 7129 0a20 2020  ", self.req).   
+00013770: 2020 2020 206c 6f67 7461 696c 203d 2022       logtail = "
+00013780: 220a 0a20 2020 2020 2020 2023 0a20 2020  "..        #.   
+00013790: 2020 2020 2023 2069 6620 7265 7175 6573       # if reques
+000137a0: 7420 6973 2066 6f72 2066 6f6f 2e6a 732c  t is for foo.js,
+000137b0: 2063 6865 636b 2069 6620 7765 2068 6176   check if we hav
+000137c0: 6520 666f 6f2e 6a73 2e7b 677a 2c62 727d  e foo.js.{gz,br}
+000137d0: 0a0a 2020 2020 2020 2020 6669 6c65 5f74  ..        file_t
+000137e0: 7320 3d20 300a 2020 2020 2020 2020 6564  s = 0.        ed
+000137f0: 6974 696f 6e73 2020 2020 3d20 7b7d 0a20  itions    = {}. 
+00013800: 2020 2020 2020 2066 6f72 2065 7874 2069         for ext i
+00013810: 6e20 5b22 222c 2022 2e67 7a22 2c20 222e  n ["", ".gz", ".
+00013820: 6272 225d 3a0a 2020 2020 2020 2020 2020  br"]:.          
+00013830: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00013840: 2020 2020 2020 2066 735f 7061 7468 203d         fs_path =
+00013850: 2072 6571 5f70 6174 6820 2b20 6578 740a   req_path + ext.
+00013860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013870: 7374 203d 2062 6f73 2e73 7461 7428 6673  st = bos.stat(fs
+00013880: 5f70 6174 6829 0a20 2020 2020 2020 2020  _path).         
+00013890: 2020 2020 2020 2069 6620 7374 6174 2e53         if stat.S
+000138a0: 5f49 5344 4952 2873 742e 7374 5f6d 6f64  _ISDIR(st.st_mod
+000138b0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+000138c0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+000138d0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000138e0: 2020 6966 2073 7461 742e 535f 4953 424c    if stat.S_ISBL
+000138f0: 4b28 7374 2e73 745f 6d6f 6465 293a 0a20  K(st.st_mode):. 
+00013900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013910: 2020 2066 6420 3d20 626f 732e 6f70 656e     fd = bos.open
+00013920: 2866 735f 7061 7468 2c20 6f73 2e4f 5f52  (fs_path, os.O_R
+00013930: 444f 4e4c 5929 0a20 2020 2020 2020 2020  DONLY).         
+00013940: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
 00013950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013960: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
-00013970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013980: 2020 6f73 2e63 6c6f 7365 2866 6429 0a20    os.close(fd). 
-00013990: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000139a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000139b0: 2020 2020 2020 2020 2073 7a20 3d20 7374           sz = st
-000139c0: 2e73 745f 7369 7a65 0a0a 2020 2020 2020  .st_size..      
-000139d0: 2020 2020 2020 2020 2020 6669 6c65 5f74            file_t
-000139e0: 7320 3d20 6d61 7828 6669 6c65 5f74 732c  s = max(file_ts,
-000139f0: 2069 6e74 2873 742e 7374 5f6d 7469 6d65   int(st.st_mtime
-00013a00: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00013a10: 2020 2065 6469 7469 6f6e 735b 6578 7420     editions[ext 
-00013a20: 6f72 2022 706c 6169 6e22 5d20 3d20 2866  or "plain"] = (f
-00013a30: 735f 7061 7468 2c20 737a 290a 2020 2020  s_path, sz).    
-00013a40: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-00013a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a60: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
-00013a70: 2069 6620 6e6f 7420 7365 6c66 2e76 7061   if not self.vpa
-00013a80: 7468 2e73 7461 7274 7377 6974 6828 222e  th.startswith(".
-00013a90: 6370 722f 2229 3a0a 2020 2020 2020 2020  cpr/"):.        
-00013aa0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-00013ab0: 2020 2020 2020 2069 6620 6e6f 7420 6564         if not ed
-00013ac0: 6974 696f 6e73 3a0a 2020 2020 2020 2020  itions:.        
-00013ad0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00013ae0: 7478 5f34 3034 2829 0a0a 2020 2020 2020  tx_404()..      
-00013af0: 2020 230a 2020 2020 2020 2020 2320 6966    #.        # if
-00013b00: 2d6d 6f64 6966 6965 640a 0a20 2020 2020  -modified..     
-00013b10: 2020 2066 696c 655f 6c61 7374 6d6f 642c     file_lastmod,
-00013b20: 2064 6f5f 7365 6e64 203d 2073 656c 662e   do_send = self.
-00013b30: 5f63 686b 5f6c 6173 746d 6f64 2866 696c  _chk_lastmod(fil
-00013b40: 655f 7473 290a 2020 2020 2020 2020 7365  e_ts).        se
-00013b50: 6c66 2e6f 7574 5f68 6561 6465 7273 5b22  lf.out_headers["
-00013b60: 4c61 7374 2d4d 6f64 6966 6965 6422 5d20  Last-Modified"] 
-00013b70: 3d20 6669 6c65 5f6c 6173 746d 6f64 0a20  = file_lastmod. 
-00013b80: 2020 2020 2020 2069 6620 6e6f 7420 646f         if not do
-00013b90: 5f73 656e 643a 0a20 2020 2020 2020 2020  _send:.         
-00013ba0: 2020 2073 7461 7475 7320 3d20 3330 340a     status = 304.
-00013bb0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-00013bc0: 2020 2023 2041 6363 6570 742d 456e 636f     # Accept-Enco
-00013bd0: 6469 6e67 2061 6e64 2055 4120 6465 6369  ding and UA deci
-00013be0: 6465 7320 7768 6963 6820 6564 6974 696f  des which editio
-00013bf0: 6e20 746f 2073 656e 640a 0a20 2020 2020  n to send..     
-00013c00: 2020 2064 6563 6f6d 7072 6573 7320 3d20     decompress = 
-00013c10: 4661 6c73 650a 2020 2020 2020 2020 7375  False.        su
-00013c20: 7070 6f72 7465 645f 6564 6974 696f 6e73  pported_editions
-00013c30: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00013c40: 2078 2e73 7472 6970 2829 0a20 2020 2020   x.strip().     
-00013c50: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
-00013c60: 7365 6c66 2e68 6561 6465 7273 2e67 6574  self.headers.get
-00013c70: 2822 6163 6365 7074 2d65 6e63 6f64 696e  ("accept-encodin
-00013c80: 6722 2c20 2222 292e 6c6f 7765 7228 292e  g", "").lower().
-00013c90: 7370 6c69 7428 222c 2229 0a20 2020 2020  split(",").     
-00013ca0: 2020 205d 0a20 2020 2020 2020 2069 6620     ].        if 
-00013cb0: 222e 6272 2220 696e 2065 6469 7469 6f6e  ".br" in edition
-00013cc0: 7320 616e 6420 2262 7222 2069 6e20 7375  s and "br" in su
-00013cd0: 7070 6f72 7465 645f 6564 6974 696f 6e73  pported_editions
-00013ce0: 3a0a 2020 2020 2020 2020 2020 2020 6973  :.            is
-00013cf0: 5f63 6f6d 7072 6573 7365 6420 3d20 5472  _compressed = Tr
-00013d00: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
-00013d10: 656c 6563 7465 645f 6564 6974 696f 6e20  elected_edition 
-00013d20: 3d20 222e 6272 220a 2020 2020 2020 2020  = ".br".        
-00013d30: 2020 2020 6673 5f70 6174 682c 2066 696c      fs_path, fil
-00013d40: 655f 737a 203d 2065 6469 7469 6f6e 735b  e_sz = editions[
-00013d50: 222e 6272 225d 0a20 2020 2020 2020 2020  ".br"].         
-00013d60: 2020 2073 656c 662e 6f75 745f 6865 6164     self.out_head
-00013d70: 6572 735b 2243 6f6e 7465 6e74 2d45 6e63  ers["Content-Enc
-00013d80: 6f64 696e 6722 5d20 3d20 2262 7222 0a20  oding"] = "br". 
-00013d90: 2020 2020 2020 2065 6c69 6620 222e 677a         elif ".gz
-00013da0: 2220 696e 2065 6469 7469 6f6e 733a 0a20  " in editions:. 
-00013db0: 2020 2020 2020 2020 2020 2069 735f 636f             is_co
-00013dc0: 6d70 7265 7373 6564 203d 2054 7275 650a  mpressed = True.
-00013dd0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-00013de0: 6374 6564 5f65 6469 7469 6f6e 203d 2022  cted_edition = "
-00013df0: 2e67 7a22 0a20 2020 2020 2020 2020 2020  .gz".           
-00013e00: 2066 735f 7061 7468 2c20 6669 6c65 5f73   fs_path, file_s
-00013e10: 7a20 3d20 6564 6974 696f 6e73 5b22 2e67  z = editions[".g
-00013e20: 7a22 5d0a 2020 2020 2020 2020 2020 2020  z"].            
-00013e30: 6966 2022 677a 6970 2220 6e6f 7420 696e  if "gzip" not in
-00013e40: 2073 7570 706f 7274 6564 5f65 6469 7469   supported_editi
-00013e50: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-00013e60: 2020 2020 2064 6563 6f6d 7072 6573 7320       decompress 
-00013e70: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-00013e80: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00013e90: 2020 2020 2020 2020 2069 6620 7265 2e6d           if re.m
-00013ea0: 6174 6368 2872 224d 5349 4520 5b34 2d36  atch(r"MSIE [4-6
-00013eb0: 5d5c 2e22 2c20 7365 6c66 2e75 6129 2061  ]\.", self.ua) a
-00013ec0: 6e64 2022 2053 5631 2220 6e6f 7420 696e  nd " SV1" not in
-00013ed0: 2073 656c 662e 7561 3a0a 2020 2020 2020   self.ua:.      
-00013ee0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00013ef0: 636f 6d70 7265 7373 203d 2054 7275 650a  compress = True.
-00013f00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013f10: 6e6f 7420 6465 636f 6d70 7265 7373 3a0a  not decompress:.
-00013f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f30: 7365 6c66 2e6f 7574 5f68 6561 6465 7273  self.out_headers
-00013f40: 5b22 436f 6e74 656e 742d 456e 636f 6469  ["Content-Encodi
-00013f50: 6e67 225d 203d 2022 677a 6970 220a 2020  ng"] = "gzip".  
-00013f60: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00013f70: 2020 2020 2020 2020 6973 5f63 6f6d 7072          is_compr
-00013f80: 6573 7365 6420 3d20 4661 6c73 650a 2020  essed = False.  
-00013f90: 2020 2020 2020 2020 2020 7365 6c65 6374            select
-00013fa0: 6564 5f65 6469 7469 6f6e 203d 2022 706c  ed_edition = "pl
-00013fb0: 6169 6e22 0a0a 2020 2020 2020 2020 7472  ain"..        tr
-00013fc0: 793a 0a20 2020 2020 2020 2020 2020 2066  y:.            f
-00013fd0: 735f 7061 7468 2c20 6669 6c65 5f73 7a20  s_path, file_sz 
-00013fe0: 3d20 6564 6974 696f 6e73 5b73 656c 6563  = editions[selec
-00013ff0: 7465 645f 6564 6974 696f 6e5d 0a20 2020  ted_edition].   
-00014000: 2020 2020 2020 2020 206c 6f67 6d73 6720           logmsg 
-00014010: 2b3d 2022 7b7d 2022 2e66 6f72 6d61 7428  += "{} ".format(
-00014020: 7365 6c65 6374 6564 5f65 6469 7469 6f6e  selected_edition
-00014030: 2e6c 7374 7269 7028 222e 2229 290a 2020  .lstrip(".")).  
-00014040: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-00014050: 2020 2020 2020 2020 2020 2320 636c 6965            # clie
-00014060: 6e74 2069 7320 6f6c 6420 616e 6420 7765  nt is old and we
-00014070: 206f 6e6c 7920 6861 7665 202e 6272 0a20   only have .br. 
-00014080: 2020 2020 2020 2020 2020 2023 2028 636f             # (co
-00014090: 756c 6420 6d61 6b65 2062 726f 746c 6920  uld make brotli 
-000140a0: 6120 6465 7020 746f 2066 6978 2074 6869  a dep to fix thi
-000140b0: 7320 6275 7420 6974 2773 206e 6f74 2077  s but it's not w
-000140c0: 6f72 7468 290a 2020 2020 2020 2020 2020  orth).          
-000140d0: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
-000140e0: 3034 290a 0a20 2020 2020 2020 2023 0a20  04)..        #. 
-000140f0: 2020 2020 2020 2023 2070 6172 7469 616c         # partial
-00014100: 0a0a 2020 2020 2020 2020 6c6f 7765 7220  ..        lower 
-00014110: 3d20 300a 2020 2020 2020 2020 7570 7065  = 0.        uppe
-00014120: 7220 3d20 6669 6c65 5f73 7a0a 2020 2020  r = file_sz.    
-00014130: 2020 2020 6872 616e 6765 203d 2073 656c      hrange = sel
-00014140: 662e 6865 6164 6572 732e 6765 7428 2272  f.headers.get("r
-00014150: 616e 6765 2229 0a0a 2020 2020 2020 2020  ange")..        
-00014160: 2320 6c65 7427 7320 6e6f 7420 7375 7070  # let's not supp
-00014170: 6f72 7420 3230 3620 7769 7468 2063 6f6d  ort 206 with com
-00014180: 7072 6573 7369 6f6e 0a20 2020 2020 2020  pression.       
-00014190: 2069 6620 646f 5f73 656e 6420 616e 6420   if do_send and 
-000141a0: 6e6f 7420 6973 5f63 6f6d 7072 6573 7365  not is_compresse
-000141b0: 6420 616e 6420 6872 616e 6765 2061 6e64  d and hrange and
-000141c0: 2066 696c 655f 737a 3a0a 2020 2020 2020   file_sz:.      
-000141d0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000141e0: 2020 2020 2020 2020 2020 2061 2c20 6220             a, b 
-000141f0: 3d20 6872 616e 6765 2e73 706c 6974 2822  = hrange.split("
-00014200: 3d22 2c20 3129 5b31 5d2e 7370 6c69 7428  =", 1)[1].split(
-00014210: 222d 2229 0a0a 2020 2020 2020 2020 2020  "-")..          
-00014220: 2020 2020 2020 6966 2061 2e73 7472 6970        if a.strip
-00014230: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014240: 2020 2020 2020 2020 6c6f 7765 7220 3d20          lower = 
-00014250: 696e 7428 612e 7374 7269 7028 2929 0a20  int(a.strip()). 
-00014260: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00014270: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00014280: 2020 2020 2020 2020 206c 6f77 6572 203d           lower =
-00014290: 2030 0a0a 2020 2020 2020 2020 2020 2020   0..            
-000142a0: 2020 2020 6966 2062 2e73 7472 6970 2829      if b.strip()
+00013960: 2020 2020 2020 2020 737a 203d 206f 732e          sz = os.
+00013970: 6c73 6565 6b28 6664 2c20 302c 206f 732e  lseek(fd, 0, os.
+00013980: 5345 454b 5f45 4e44 290a 2020 2020 2020  SEEK_END).      
+00013990: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+000139a0: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
+000139b0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000139c0: 732e 636c 6f73 6528 6664 290a 2020 2020  s.close(fd).    
+000139d0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000139e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000139f0: 2020 2020 2020 737a 203d 2073 742e 7374        sz = st.st
+00013a00: 5f73 697a 650a 0a20 2020 2020 2020 2020  _size..         
+00013a10: 2020 2020 2020 2066 696c 655f 7473 203d         file_ts =
+00013a20: 206d 6178 2866 696c 655f 7473 2c20 696e   max(file_ts, in
+00013a30: 7428 7374 2e73 745f 6d74 696d 6529 290a  t(st.st_mtime)).
+00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a50: 6564 6974 696f 6e73 5b65 7874 206f 7220  editions[ext or 
+00013a60: 2270 6c61 696e 225d 203d 2028 6673 5f70  "plain"] = (fs_p
+00013a70: 6174 682c 2073 7a29 0a20 2020 2020 2020  ath, sz).       
+00013a80: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+00013a90: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+00013aa0: 730a 2020 2020 2020 2020 2020 2020 6966  s.            if
+00013ab0: 206e 6f74 2073 656c 662e 7670 6174 682e   not self.vpath.
+00013ac0: 7374 6172 7473 7769 7468 2822 2e63 7072  startswith(".cpr
+00013ad0: 2f22 293a 0a20 2020 2020 2020 2020 2020  /"):.           
+00013ae0: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
+00013af0: 2020 2020 6966 206e 6f74 2065 6469 7469      if not editi
+00013b00: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+00013b10: 2072 6574 7572 6e20 7365 6c66 2e74 785f   return self.tx_
+00013b20: 3430 3428 290a 0a20 2020 2020 2020 2023  404()..        #
+00013b30: 0a20 2020 2020 2020 2023 2069 662d 6d6f  .        # if-mo
+00013b40: 6469 6669 6564 0a0a 2020 2020 2020 2020  dified..        
+00013b50: 6669 6c65 5f6c 6173 746d 6f64 2c20 646f  file_lastmod, do
+00013b60: 5f73 656e 6420 3d20 7365 6c66 2e5f 6368  _send = self._ch
+00013b70: 6b5f 6c61 7374 6d6f 6428 6669 6c65 5f74  k_lastmod(file_t
+00013b80: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
+00013b90: 6f75 745f 6865 6164 6572 735b 224c 6173  out_headers["Las
+00013ba0: 742d 4d6f 6469 6669 6564 225d 203d 2066  t-Modified"] = f
+00013bb0: 696c 655f 6c61 7374 6d6f 640a 2020 2020  ile_lastmod.    
+00013bc0: 2020 2020 6966 206e 6f74 2064 6f5f 7365      if not do_se
+00013bd0: 6e64 3a0a 2020 2020 2020 2020 2020 2020  nd:.            
+00013be0: 7374 6174 7573 203d 2033 3034 0a0a 2020  status = 304..  
+00013bf0: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
+00013c00: 2320 4163 6365 7074 2d45 6e63 6f64 696e  # Accept-Encodin
+00013c10: 6720 616e 6420 5541 2064 6563 6964 6573  g and UA decides
+00013c20: 2077 6869 6368 2065 6469 7469 6f6e 2074   which edition t
+00013c30: 6f20 7365 6e64 0a0a 2020 2020 2020 2020  o send..        
+00013c40: 6465 636f 6d70 7265 7373 203d 2046 616c  decompress = Fal
+00013c50: 7365 0a20 2020 2020 2020 2073 7570 706f  se.        suppo
+00013c60: 7274 6564 5f65 6469 7469 6f6e 7320 3d20  rted_editions = 
+00013c70: 5b0a 2020 2020 2020 2020 2020 2020 782e  [.            x.
+00013c80: 7374 7269 7028 290a 2020 2020 2020 2020  strip().        
+00013c90: 2020 2020 666f 7220 7820 696e 2073 656c      for x in sel
+00013ca0: 662e 6865 6164 6572 732e 6765 7428 2261  f.headers.get("a
+00013cb0: 6363 6570 742d 656e 636f 6469 6e67 222c  ccept-encoding",
+00013cc0: 2022 2229 2e6c 6f77 6572 2829 2e73 706c   "").lower().spl
+00013cd0: 6974 2822 2c22 290a 2020 2020 2020 2020  it(",").        
+00013ce0: 5d0a 2020 2020 2020 2020 6966 2022 2e62  ].        if ".b
+00013cf0: 7222 2069 6e20 6564 6974 696f 6e73 2061  r" in editions a
+00013d00: 6e64 2022 6272 2220 696e 2073 7570 706f  nd "br" in suppo
+00013d10: 7274 6564 5f65 6469 7469 6f6e 733a 0a20  rted_editions:. 
+00013d20: 2020 2020 2020 2020 2020 2069 735f 636f             is_co
+00013d30: 6d70 7265 7373 6564 203d 2054 7275 650a  mpressed = True.
+00013d40: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
+00013d50: 6374 6564 5f65 6469 7469 6f6e 203d 2022  cted_edition = "
+00013d60: 2e62 7222 0a20 2020 2020 2020 2020 2020  .br".           
+00013d70: 2066 735f 7061 7468 2c20 6669 6c65 5f73   fs_path, file_s
+00013d80: 7a20 3d20 6564 6974 696f 6e73 5b22 2e62  z = editions[".b
+00013d90: 7222 5d0a 2020 2020 2020 2020 2020 2020  r"].            
+00013da0: 7365 6c66 2e6f 7574 5f68 6561 6465 7273  self.out_headers
+00013db0: 5b22 436f 6e74 656e 742d 456e 636f 6469  ["Content-Encodi
+00013dc0: 6e67 225d 203d 2022 6272 220a 2020 2020  ng"] = "br".    
+00013dd0: 2020 2020 656c 6966 2022 2e67 7a22 2069      elif ".gz" i
+00013de0: 6e20 6564 6974 696f 6e73 3a0a 2020 2020  n editions:.    
+00013df0: 2020 2020 2020 2020 6973 5f63 6f6d 7072          is_compr
+00013e00: 6573 7365 6420 3d20 5472 7565 0a20 2020  essed = True.   
+00013e10: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
+00013e20: 645f 6564 6974 696f 6e20 3d20 222e 677a  d_edition = ".gz
+00013e30: 220a 2020 2020 2020 2020 2020 2020 6673  ".            fs
+00013e40: 5f70 6174 682c 2066 696c 655f 737a 203d  _path, file_sz =
+00013e50: 2065 6469 7469 6f6e 735b 222e 677a 225d   editions[".gz"]
+00013e60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013e70: 2267 7a69 7022 206e 6f74 2069 6e20 7375  "gzip" not in su
+00013e80: 7070 6f72 7465 645f 6564 6974 696f 6e73  pported_editions
+00013e90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013ea0: 2020 6465 636f 6d70 7265 7373 203d 2054    decompress = T
+00013eb0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+00013ec0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00013ed0: 2020 2020 2020 6966 2072 652e 6d61 7463        if re.matc
+00013ee0: 6828 7222 4d53 4945 205b 342d 365d 5c2e  h(r"MSIE [4-6]\.
+00013ef0: 222c 2073 656c 662e 7561 2920 616e 6420  ", self.ua) and 
+00013f00: 2220 5356 3122 206e 6f74 2069 6e20 7365  " SV1" not in se
+00013f10: 6c66 2e75 613a 0a20 2020 2020 2020 2020  lf.ua:.         
+00013f20: 2020 2020 2020 2020 2020 2064 6563 6f6d             decom
+00013f30: 7072 6573 7320 3d20 5472 7565 0a0a 2020  press = True..  
+00013f40: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00013f50: 2064 6563 6f6d 7072 6573 733a 0a20 2020   decompress:.   
+00013f60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013f70: 662e 6f75 745f 6865 6164 6572 735b 2243  f.out_headers["C
+00013f80: 6f6e 7465 6e74 2d45 6e63 6f64 696e 6722  ontent-Encoding"
+00013f90: 5d20 3d20 2267 7a69 7022 0a20 2020 2020  ] = "gzip".     
+00013fa0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00013fb0: 2020 2020 2069 735f 636f 6d70 7265 7373       is_compress
+00013fc0: 6564 203d 2046 616c 7365 0a20 2020 2020  ed = False.     
+00013fd0: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
+00013fe0: 6564 6974 696f 6e20 3d20 2270 6c61 696e  edition = "plain
+00013ff0: 220a 0a20 2020 2020 2020 2074 7279 3a0a  "..        try:.
+00014000: 2020 2020 2020 2020 2020 2020 6673 5f70              fs_p
+00014010: 6174 682c 2066 696c 655f 737a 203d 2065  ath, file_sz = e
+00014020: 6469 7469 6f6e 735b 7365 6c65 6374 6564  ditions[selected
+00014030: 5f65 6469 7469 6f6e 5d0a 2020 2020 2020  _edition].      
+00014040: 2020 2020 2020 6c6f 676d 7367 202b 3d20        logmsg += 
+00014050: 227b 7d20 222e 666f 726d 6174 2873 656c  "{} ".format(sel
+00014060: 6563 7465 645f 6564 6974 696f 6e2e 6c73  ected_edition.ls
+00014070: 7472 6970 2822 2e22 2929 0a20 2020 2020  trip(".")).     
+00014080: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+00014090: 2020 2020 2020 2023 2063 6c69 656e 7420         # client 
+000140a0: 6973 206f 6c64 2061 6e64 2077 6520 6f6e  is old and we on
+000140b0: 6c79 2068 6176 6520 2e62 720a 2020 2020  ly have .br.    
+000140c0: 2020 2020 2020 2020 2320 2863 6f75 6c64          # (could
+000140d0: 206d 616b 6520 6272 6f74 6c69 2061 2064   make brotli a d
+000140e0: 6570 2074 6f20 6669 7820 7468 6973 2062  ep to fix this b
+000140f0: 7574 2069 7427 7320 6e6f 7420 776f 7274  ut it's not wort
+00014100: 6829 0a20 2020 2020 2020 2020 2020 2072  h).            r
+00014110: 6169 7365 2050 6562 6b61 6328 3430 3429  aise Pebkac(404)
+00014120: 0a0a 2020 2020 2020 2020 230a 2020 2020  ..        #.    
+00014130: 2020 2020 2320 7061 7274 6961 6c0a 0a20      # partial.. 
+00014140: 2020 2020 2020 206c 6f77 6572 203d 2030         lower = 0
+00014150: 0a20 2020 2020 2020 2075 7070 6572 203d  .        upper =
+00014160: 2066 696c 655f 737a 0a20 2020 2020 2020   file_sz.       
+00014170: 2068 7261 6e67 6520 3d20 7365 6c66 2e68   hrange = self.h
+00014180: 6561 6465 7273 2e67 6574 2822 7261 6e67  eaders.get("rang
+00014190: 6522 290a 0a20 2020 2020 2020 2023 206c  e")..        # l
+000141a0: 6574 2773 206e 6f74 2073 7570 706f 7274  et's not support
+000141b0: 2032 3036 2077 6974 6820 636f 6d70 7265   206 with compre
+000141c0: 7373 696f 6e0a 2020 2020 2020 2020 6966  ssion.        if
+000141d0: 2064 6f5f 7365 6e64 2061 6e64 206e 6f74   do_send and not
+000141e0: 2069 735f 636f 6d70 7265 7373 6564 2061   is_compressed a
+000141f0: 6e64 2068 7261 6e67 6520 616e 6420 6669  nd hrange and fi
+00014200: 6c65 5f73 7a3a 0a20 2020 2020 2020 2020  le_sz:.         
+00014210: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00014220: 2020 2020 2020 2020 612c 2062 203d 2068          a, b = h
+00014230: 7261 6e67 652e 7370 6c69 7428 223d 222c  range.split("=",
+00014240: 2031 295b 315d 2e73 706c 6974 2822 2d22   1)[1].split("-"
+00014250: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00014260: 2020 2069 6620 612e 7374 7269 7028 293a     if a.strip():
+00014270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014280: 2020 2020 206c 6f77 6572 203d 2069 6e74       lower = int
+00014290: 2861 2e73 7472 6970 2829 290a 2020 2020  (a.strip()).    
+000142a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
 000142b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000142c0: 2020 2020 2020 7570 7065 7220 3d20 696e        upper = in
-000142d0: 7428 622e 7374 7269 7028 2929 202b 2031  t(b.strip()) + 1
-000142e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000142f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00014300: 2020 2020 2020 2020 2020 2075 7070 6572             upper
-00014310: 203d 2066 696c 655f 737a 0a0a 2020 2020   = file_sz..    
-00014320: 2020 2020 2020 2020 2020 2020 6966 2075              if u
-00014330: 7070 6572 203e 2066 696c 655f 737a 3a0a  pper > file_sz:.
-00014340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014350: 2020 2020 7570 7065 7220 3d20 6669 6c65      upper = file
-00014360: 5f73 7a0a 0a20 2020 2020 2020 2020 2020  _sz..           
-00014370: 2020 2020 2069 6620 6c6f 7765 7220 3c20       if lower < 
-00014380: 3020 6f72 206c 6f77 6572 203e 3d20 7570  0 or lower >= up
-00014390: 7065 723a 0a20 2020 2020 2020 2020 2020  per:.           
-000143a0: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
-000143b0: 7863 6570 7469 6f6e 2829 0a0a 2020 2020  xception()..    
-000143c0: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-000143d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143e0: 6572 7220 3d20 2269 6e76 616c 6964 2072  err = "invalid r
-000143f0: 616e 6765 2028 7b7d 292c 2073 697a 653d  ange ({}), size=
-00014400: 7b7d 222e 666f 726d 6174 2868 7261 6e67  {}".format(hrang
-00014410: 652c 2066 696c 655f 737a 290a 2020 2020  e, file_sz).    
-00014420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014430: 2e6c 6f75 645f 7265 706c 7928 0a20 2020  .loud_reply(.   
-00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014450: 2065 7272 2c0a 2020 2020 2020 2020 2020   err,.          
-00014460: 2020 2020 2020 2020 2020 7374 6174 7573            status
-00014470: 3d34 3136 2c0a 2020 2020 2020 2020 2020  =416,.          
-00014480: 2020 2020 2020 2020 2020 6865 6164 6572            header
-00014490: 733d 7b22 436f 6e74 656e 742d 5261 6e67  s={"Content-Rang
-000144a0: 6522 3a20 2262 7974 6573 202a 2f7b 7d22  e": "bytes */{}"
-000144b0: 2e66 6f72 6d61 7428 6669 6c65 5f73 7a29  .format(file_sz)
-000144c0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-000144d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000144e0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-000144f0: 0a0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00014500: 6174 7573 203d 2032 3036 0a20 2020 2020  atus = 206.     
-00014510: 2020 2020 2020 2073 656c 662e 6f75 745f         self.out_
-00014520: 6865 6164 6572 735b 2243 6f6e 7465 6e74  headers["Content
-00014530: 2d52 616e 6765 225d 203d 2022 6279 7465  -Range"] = "byte
-00014540: 7320 7b7d 2d7b 7d2f 7b7d 222e 666f 726d  s {}-{}/{}".form
-00014550: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
-00014560: 2020 2020 6c6f 7765 722c 2075 7070 6572      lower, upper
-00014570: 202d 2031 2c20 6669 6c65 5f73 7a0a 2020   - 1, file_sz.  
-00014580: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00014590: 2020 2020 2020 2020 206c 6f67 7461 696c           logtail
-000145a0: 202b 3d20 2220 5b5c 3033 335b 3336 6d7b   += " [\033[36m{
-000145b0: 7d2d 7b7d 5c30 3333 5b30 6d5d 222e 666f  }-{}\033[0m]".fo
-000145c0: 726d 6174 286c 6f77 6572 2c20 7570 7065  rmat(lower, uppe
-000145d0: 7229 0a0a 2020 2020 2020 2020 7573 655f  r)..        use_
-000145e0: 7365 6e64 6669 6c65 203d 2046 616c 7365  sendfile = False
-000145f0: 0a20 2020 2020 2020 2069 6620 6465 636f  .        if deco
-00014600: 6d70 7265 7373 3a0a 2020 2020 2020 2020  mpress:.        
-00014610: 2020 2020 6f70 656e 5f66 756e 6320 203d      open_func  =
-00014620: 2067 7a69 702e 6f70 656e 0a20 2020 2020   gzip.open.     
-00014630: 2020 2020 2020 206f 7065 6e5f 6172 6773         open_args
-00014640: 2020 3d20 5b66 7365 6e63 2866 735f 7061    = [fsenc(fs_pa
-00014650: 7468 292c 2022 7262 225d 0a20 2020 2020  th), "rb"].     
-00014660: 2020 2020 2020 2023 2043 6f6e 7465 6e74         # Content
-00014670: 2d4c 656e 6774 6820 3a3d 206f 7269 6769  -Length := origi
-00014680: 6e61 6c20 6669 6c65 2073 697a 650a 2020  nal file size.  
-00014690: 2020 2020 2020 2020 2020 7570 7065 7220            upper 
-000146a0: 3d20 677a 6970 5f6f 7269 675f 737a 2866  = gzip_orig_sz(f
-000146b0: 735f 7061 7468 290a 2020 2020 2020 2020  s_path).        
-000146c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000146d0: 2020 6f70 656e 5f66 756e 6320 3d20 6f70    open_func = op
-000146e0: 656e 0a20 2020 2020 2020 2020 2020 2023  en.            #
-000146f0: 2035 3132 206b 4220 6973 206f 7074 696d   512 kB is optim
-00014700: 616c 2066 6f72 2068 7567 6520 6669 6c65  al for huge file
-00014710: 732c 2075 7365 2036 346b 0a20 2020 2020  s, use 64k.     
-00014720: 2020 2020 2020 206f 7065 6e5f 6172 6773         open_args
-00014730: 203d 205b 6673 656e 6328 6673 5f70 6174   = [fsenc(fs_pat
-00014740: 6829 2c20 2272 6222 2c20 3634 202a 2031  h), "rb", 64 * 1
-00014750: 3032 345d 0a20 2020 2020 2020 2020 2020  024].           
-00014760: 2075 7365 5f73 656e 6466 696c 6520 3d20   use_sendfile = 
-00014770: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00014780: 2020 6e6f 7420 7365 6c66 2e74 6c73 2020    not self.tls  
-00014790: 230a 2020 2020 2020 2020 2020 2020 2020  #.              
-000147a0: 2020 616e 6420 6e6f 7420 7365 6c66 2e61    and not self.a
-000147b0: 7267 732e 6e6f 5f73 656e 6466 696c 650a  rgs.no_sendfile.
-000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147d0: 616e 6420 6861 7361 7474 7228 6f73 2c20  and hasattr(os, 
-000147e0: 2273 656e 6466 696c 6522 290a 2020 2020  "sendfile").    
-000147f0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00014800: 2020 2023 0a20 2020 2020 2020 2023 2073     #.        # s
-00014810: 656e 6420 7265 706c 790a 0a20 2020 2020  end reply..     
-00014820: 2020 2069 6620 6973 5f63 6f6d 7072 6573     if is_compres
-00014830: 7365 643a 0a20 2020 2020 2020 2020 2020  sed:.           
-00014840: 2073 656c 662e 6f75 745f 6865 6164 6572   self.out_header
-00014850: 735b 2243 6163 6865 2d43 6f6e 7472 6f6c  s["Cache-Control
-00014860: 225d 203d 2022 6d61 782d 6167 653d 3630  "] = "max-age=60
-00014870: 3438 3639 220a 2020 2020 2020 2020 656c  4869".        el
-00014880: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00014890: 7365 6c66 2e70 6572 6d69 745f 6361 6368  self.permit_cach
-000148a0: 696e 6728 290a 0a20 2020 2020 2020 2069  ing()..        i
-000148b0: 6620 2274 7874 2220 696e 2073 656c 662e  f "txt" in self.
-000148c0: 7570 6172 616d 3a0a 2020 2020 2020 2020  uparam:.        
-000148d0: 2020 2020 6d69 6d65 203d 2022 7465 7874      mime = "text
-000148e0: 2f70 6c61 696e 3b20 6368 6172 7365 743d  /plain; charset=
-000148f0: 7b7d 222e 666f 726d 6174 2873 656c 662e  {}".format(self.
-00014900: 7570 6172 616d 5b22 7478 7422 5d20 6f72  uparam["txt"] or
-00014910: 2022 7574 662d 3822 290a 2020 2020 2020   "utf-8").      
-00014920: 2020 656c 6966 2022 6d69 6d65 2220 696e    elif "mime" in
-00014930: 2073 656c 662e 7570 6172 616d 3a0a 2020   self.uparam:.  
-00014940: 2020 2020 2020 2020 2020 6d69 6d65 203d            mime =
-00014950: 2073 7472 2873 656c 662e 7570 6172 616d   str(self.uparam
-00014960: 2e67 6574 2822 6d69 6d65 2229 290a 2020  .get("mime")).  
-00014970: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00014980: 2020 2020 2020 2020 6d69 6d65 203d 2067          mime = g
-00014990: 7565 7373 5f6d 696d 6528 7265 715f 7061  uess_mime(req_pa
-000149a0: 7468 290a 0a20 2020 2020 2020 2073 656c  th)..        sel
-000149b0: 662e 6f75 745f 6865 6164 6572 735b 2241  f.out_headers["A
-000149c0: 6363 6570 742d 5261 6e67 6573 225d 203d  ccept-Ranges"] =
-000149d0: 2022 6279 7465 7322 0a20 2020 2020 2020   "bytes".       
-000149e0: 2073 656c 662e 7365 6e64 5f68 6561 6465   self.send_heade
-000149f0: 7273 286c 656e 6774 683d 7570 7065 7220  rs(length=upper 
-00014a00: 2d20 6c6f 7765 722c 2073 7461 7475 733d  - lower, status=
-00014a10: 7374 6174 7573 2c20 6d69 6d65 3d6d 696d  status, mime=mim
-00014a20: 6529 0a0a 2020 2020 2020 2020 6c6f 676d  e)..        logm
-00014a30: 7367 202b 3d20 756e 6963 6f64 6528 7374  sg += unicode(st
-00014a40: 6174 7573 2920 2b20 6c6f 6774 6169 6c0a  atus) + logtail.
-00014a50: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00014a60: 2e6d 6f64 6520 3d3d 2022 4845 4144 2220  .mode == "HEAD" 
-00014a70: 6f72 206e 6f74 2064 6f5f 7365 6e64 3a0a  or not do_send:.
-00014a80: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00014a90: 656c 662e 646f 5f6c 6f67 3a0a 2020 2020  elf.do_log:.    
-00014aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014ab0: 2e6c 6f67 286c 6f67 6d73 6729 0a0a 2020  .log(logmsg)..  
-00014ac0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014ad0: 2054 7275 650a 0a20 2020 2020 2020 2072   True..        r
-00014ae0: 6574 203d 2054 7275 650a 2020 2020 2020  et = True.      
-00014af0: 2020 7769 7468 206f 7065 6e5f 6675 6e63    with open_func
-00014b00: 282a 6f70 656e 5f61 7267 7329 2061 7320  (*open_args) as 
-00014b10: 663a 0a20 2020 2020 2020 2020 2020 2073  f:.            s
-00014b20: 656e 6466 756e 203d 2073 656e 6466 696c  endfun = sendfil
-00014b30: 655f 6b65 726e 2069 6620 7573 655f 7365  e_kern if use_se
-00014b40: 6e64 6669 6c65 2065 6c73 6520 7365 6e64  ndfile else send
-00014b50: 6669 6c65 5f70 790a 2020 2020 2020 2020  file_py.        
-00014b60: 2020 2020 7265 6d61 696e 7320 3d20 7365      remains = se
-00014b70: 6e64 6675 6e28 0a20 2020 2020 2020 2020  ndfun(.         
-00014b80: 2020 2020 2020 2073 656c 662e 6c6f 672c         self.log,
-00014b90: 206c 6f77 6572 2c20 7570 7065 722c 2066   lower, upper, f
-00014ba0: 2c20 7365 6c66 2e73 2c20 7365 6c66 2e61  , self.s, self.a
-00014bb0: 7267 732e 735f 7772 5f73 7a2c 2073 656c  rgs.s_wr_sz, sel
-00014bc0: 662e 6172 6773 2e73 5f77 725f 736c 700a  f.args.s_wr_slp.
-00014bd0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00014be0: 2020 2020 2020 2069 6620 7265 6d61 696e         if remain
-00014bf0: 7320 3e20 303a 0a20 2020 2020 2020 2020  s > 0:.         
-00014c00: 2020 206c 6f67 6d73 6720 2b3d 2022 205c     logmsg += " \
-00014c10: 3033 335b 3331 6d22 202b 2075 6e69 636f  033[31m" + unico
-00014c20: 6465 2875 7070 6572 202d 2072 656d 6169  de(upper - remai
-00014c30: 6e73 2920 2b20 225c 3033 335b 306d 220a  ns) + "\033[0m".
-00014c40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014c50: 2e6b 6565 7061 6c69 7665 203d 2046 616c  .keepalive = Fal
-00014c60: 7365 0a0a 2020 2020 2020 2020 7370 6420  se..        spd 
-00014c70: 3d20 7365 6c66 2e5f 7370 6428 2875 7070  = self._spd((upp
-00014c80: 6572 202d 206c 6f77 6572 2920 2d20 7265  er - lower) - re
-00014c90: 6d61 696e 7329 0a20 2020 2020 2020 2069  mains).        i
-00014ca0: 6620 7365 6c66 2e64 6f5f 6c6f 673a 0a20  f self.do_log:. 
-00014cb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014cc0: 6c6f 6728 227b 7d2c 2020 7b7d 222e 666f  log("{},  {}".fo
-00014cd0: 726d 6174 286c 6f67 6d73 672c 2073 7064  rmat(logmsg, spd
-00014ce0: 2929 0a0a 2020 2020 2020 2020 7265 7475  ))..        retu
-00014cf0: 726e 2072 6574 0a0a 2020 2020 6465 6620  rn ret..    def 
-00014d00: 7478 5f7a 6970 280a 2020 2020 2020 2020  tx_zip(.        
-00014d10: 7365 6c66 2c20 666d 7420 2c20 7561 7267  self, fmt , uarg
-00014d20: 202c 2076 6e20 2c20 7265 6d20 2c20 6974   , vn , rem , it
-00014d30: 656d 7320 2c20 646f 7473 200a 2020 2020  ems , dots .    
-00014d40: 2920 203a 0a20 2020 2020 2020 2069 6620  )  :.        if 
-00014d50: 7365 6c66 2e61 7267 732e 6e6f 5f7a 6970  self.args.no_zip
-00014d60: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00014d70: 6973 6520 5065 626b 6163 2834 3030 2c20  ise Pebkac(400, 
-00014d80: 226e 6f74 2065 6e61 626c 6564 2229 0a0a  "not enabled")..
-00014d90: 2020 2020 2020 2020 6c6f 676d 7367 203d          logmsg =
-00014da0: 2022 7b3a 347d 207b 7d20 222e 666f 726d   "{:4} {} ".form
-00014db0: 6174 2822 222c 2073 656c 662e 7265 7129  at("", self.req)
-00014dc0: 0a20 2020 2020 2020 2073 656c 662e 6b65  .        self.ke
-00014dd0: 6570 616c 6976 6520 3d20 4661 6c73 650a  epalive = False.
-00014de0: 0a20 2020 2020 2020 2069 6620 666d 7420  .        if fmt 
-00014df0: 3d3d 2022 7461 7222 3a0a 2020 2020 2020  == "tar":.      
-00014e00: 2020 2020 2020 6d69 6d65 203d 2022 6170        mime = "ap
-00014e10: 706c 6963 6174 696f 6e2f 782d 7461 7222  plication/x-tar"
-00014e20: 0a20 2020 2020 2020 2020 2020 2070 6163  .            pac
-00014e30: 6b65 7220 203d 2053 7472 6561 6d54 6172  ker  = StreamTar
-00014e40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00014e50: 2020 2020 2020 2020 2020 206d 696d 6520             mime 
-00014e60: 3d20 2261 7070 6c69 6361 7469 6f6e 2f7a  = "application/z
-00014e70: 6970 220a 2020 2020 2020 2020 2020 2020  ip".            
-00014e80: 7061 636b 6572 203d 2053 7472 6561 6d5a  packer = StreamZ
-00014e90: 6970 0a0a 2020 2020 2020 2020 666e 203d  ip..        fn =
-00014ea0: 2069 7465 6d73 5b30 5d20 6966 2069 7465   items[0] if ite
-00014eb0: 6d73 2061 6e64 2069 7465 6d73 5b30 5d20  ms and items[0] 
-00014ec0: 656c 7365 2073 656c 662e 7670 6174 680a  else self.vpath.
-00014ed0: 2020 2020 2020 2020 6966 2066 6e3a 0a20          if fn:. 
-00014ee0: 2020 2020 2020 2020 2020 2066 6e20 3d20             fn = 
-00014ef0: 666e 2e72 7374 7269 7028 222f 2229 2e73  fn.rstrip("/").s
-00014f00: 706c 6974 2822 2f22 295b 2d31 5d0a 2020  plit("/")[-1].  
-00014f10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00014f20: 2020 2020 2020 2020 666e 203d 2073 656c          fn = sel
-00014f30: 662e 686f 7374 2e73 706c 6974 2822 3a22  f.host.split(":"
-00014f40: 295b 305d 0a0a 2020 2020 2020 2020 7361  )[0]..        sa
-00014f50: 6665 203d 2028 7374 7269 6e67 2e61 7363  fe = (string.asc
-00014f60: 6969 5f6c 6574 7465 7273 202b 2073 7472  ii_letters + str
-00014f70: 696e 672e 6469 6769 7473 292e 7265 706c  ing.digits).repl
-00014f80: 6163 6528 2225 222c 2022 2229 0a20 2020  ace("%", "").   
-00014f90: 2020 2020 2061 666e 203d 2022 222e 6a6f       afn = "".jo
-00014fa0: 696e 285b 7820 6966 2078 2069 6e20 7361  in([x if x in sa
-00014fb0: 6665 2e72 6570 6c61 6365 2827 2227 2c20  fe.replace('"', 
-00014fc0: 2222 2920 656c 7365 2022 5f22 2066 6f72  "") else "_" for
-00014fd0: 2078 2069 6e20 666e 5d29 0a20 2020 2020   x in fn]).     
-00014fe0: 2020 2062 6173 6369 6920 3d20 756e 6963     bascii = unic
-00014ff0: 6f64 6528 7361 6665 292e 656e 636f 6465  ode(safe).encode
-00015000: 2822 7574 662d 3822 290a 2020 2020 2020  ("utf-8").      
-00015010: 2020 7a62 203d 2066 6e2e 656e 636f 6465    zb = fn.encode
-00015020: 2822 7574 662d 3822 2c20 2278 6d6c 6368  ("utf-8", "xmlch
-00015030: 6172 7265 6672 6570 6c61 6365 2229 0a20  arrefreplace"). 
-00015040: 2020 2020 2020 2069 6620 6e6f 7420 5059         if not PY
-00015050: 323a 0a20 2020 2020 2020 2020 2020 207a  2:.            z
-00015060: 626c 203d 205b 0a20 2020 2020 2020 2020  bl = [.         
-00015070: 2020 2020 2020 2063 6872 2878 292e 656e         chr(x).en
-00015080: 636f 6465 2822 7574 662d 3822 290a 2020  code("utf-8").  
-00015090: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000150a0: 2078 2069 6e20 6261 7363 6969 0a20 2020   x in bascii.   
-000150b0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000150c0: 6520 2225 7b3a 3032 787d 222e 666f 726d  e "%{:02x}".form
-000150d0: 6174 2878 292e 656e 636f 6465 2822 6173  at(x).encode("as
-000150e0: 6369 6922 290a 2020 2020 2020 2020 2020  cii").          
-000150f0: 2020 2020 2020 666f 7220 7820 696e 207a        for x in z
-00015100: 620a 2020 2020 2020 2020 2020 2020 5d0a  b.            ].
-00015110: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00015120: 2020 2020 2020 2020 2020 7a62 6c20 3d20            zbl = 
-00015130: 5b75 6e69 636f 6465 2878 2920 6966 2078  [unicode(x) if x
-00015140: 2069 6e20 6261 7363 6969 2065 6c73 6520   in bascii else 
-00015150: 2225 7b3a 3032 787d 222e 666f 726d 6174  "%{:02x}".format
-00015160: 286f 7264 2878 2929 2066 6f72 2078 2069  (ord(x)) for x i
-00015170: 6e20 7a62 5d0a 0a20 2020 2020 2020 2075  n zb]..        u
-00015180: 666e 203d 2062 2222 2e6a 6f69 6e28 7a62  fn = b"".join(zb
-00015190: 6c29 2e64 6563 6f64 6528 2261 7363 6969  l).decode("ascii
-000151a0: 2229 0a0a 2020 2020 2020 2020 6364 6973  ")..        cdis
-000151b0: 203d 2022 6174 7461 6368 6d65 6e74 3b20   = "attachment; 
-000151c0: 6669 6c65 6e61 6d65 3d5c 227b 7d2e 7b7d  filename=\"{}.{}
-000151d0: 5c22 3b20 6669 6c65 6e61 6d65 2a3d 5554  \"; filename*=UT
-000151e0: 462d 3827 277b 7d2e 7b7d 220a 2020 2020  F-8''{}.{}".    
-000151f0: 2020 2020 6364 6973 203d 2063 6469 732e      cdis = cdis.
-00015200: 666f 726d 6174 2861 666e 2c20 666d 742c  format(afn, fmt,
-00015210: 2075 666e 2c20 666d 7429 0a20 2020 2020   ufn, fmt).     
-00015220: 2020 2073 656c 662e 6c6f 6728 6364 6973     self.log(cdis
-00015230: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00015240: 656e 645f 6865 6164 6572 7328 4e6f 6e65  end_headers(None
-00015250: 2c20 6d69 6d65 3d6d 696d 652c 2068 6561  , mime=mime, hea
-00015260: 6465 7273 3d7b 2243 6f6e 7465 6e74 2d44  ders={"Content-D
-00015270: 6973 706f 7369 7469 6f6e 223a 2063 6469  isposition": cdi
-00015280: 737d 290a 0a20 2020 2020 2020 2066 6765  s})..        fge
-00015290: 6e20 3d20 766e 2e7a 6970 6765 6e28 0a20  n = vn.zipgen(. 
-000152a0: 2020 2020 2020 2020 2020 2072 656d 2c20             rem, 
-000152b0: 7365 7428 6974 656d 7329 2c20 7365 6c66  set(items), self
-000152c0: 2e75 6e61 6d65 2c20 4661 6c73 652c 2064  .uname, False, d
-000152d0: 6f74 732c 206e 6f74 2073 656c 662e 6172  ots, not self.ar
-000152e0: 6773 2e6e 6f5f 7363 616e 6469 720a 2020  gs.no_scandir.  
-000152f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00015300: 2320 666f 7220 6620 696e 2066 6765 6e3a  # for f in fgen:
-00015310: 2070 7269 6e74 2872 6570 7228 7b6b 3a20   print(repr({k: 
-00015320: 665b 6b5d 2066 6f72 206b 2069 6e20 5b22  f[k] for k in ["
-00015330: 7670 222c 2022 6170 225d 7d29 290a 2020  vp", "ap"]})).  
-00015340: 2020 2020 2020 6267 656e 203d 2070 6163        bgen = pac
-00015350: 6b65 7228 7365 6c66 2e6c 6f67 2c20 6667  ker(self.log, fg
-00015360: 656e 2c20 7574 6638 3d22 7574 6622 2069  en, utf8="utf" i
-00015370: 6e20 7561 7267 2c20 7072 655f 6372 633d  n uarg, pre_crc=
-00015380: 2263 7263 2220 696e 2075 6172 6729 0a20  "crc" in uarg). 
-00015390: 2020 2020 2020 2062 7365 6e74 203d 2030         bsent = 0
-000153a0: 0a20 2020 2020 2020 2066 6f72 2062 7566  .        for buf
-000153b0: 2069 6e20 6267 656e 2e67 656e 2829 3a0a   in bgen.gen():.
-000153c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000153d0: 6f74 2062 7566 3a0a 2020 2020 2020 2020  ot buf:.        
-000153e0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-000153f0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00015400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015410: 7365 6c66 2e73 2e73 656e 6461 6c6c 2862  self.s.sendall(b
-00015420: 7566 290a 2020 2020 2020 2020 2020 2020  uf).            
-00015430: 2020 2020 6273 656e 7420 2b3d 206c 656e      bsent += len
-00015440: 2862 7566 290a 2020 2020 2020 2020 2020  (buf).          
-00015450: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-00015460: 2020 2020 2020 2020 2020 6c6f 676d 7367            logmsg
-00015470: 202b 3d20 2220 5c30 3333 5b33 316d 2220   += " \033[31m" 
-00015480: 2b20 756e 6963 6f64 6528 6273 656e 7429  + unicode(bsent)
-00015490: 202b 2022 5c30 3333 5b30 6d22 0a20 2020   + "\033[0m".   
-000154a0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-000154b0: 616b 0a0a 2020 2020 2020 2020 7370 6420  ak..        spd 
-000154c0: 3d20 7365 6c66 2e5f 7370 6428 6273 656e  = self._spd(bsen
-000154d0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-000154e0: 6c6f 6728 227b 7d2c 2020 7b7d 222e 666f  log("{},  {}".fo
-000154f0: 726d 6174 286c 6f67 6d73 672c 2073 7064  rmat(logmsg, spd
-00015500: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-00015510: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
-00015520: 7478 5f69 636f 2873 656c 662c 2065 7874  tx_ico(self, ext
-00015530: 202c 2065 7861 6374 2020 3d20 4661 6c73   , exact  = Fals
-00015540: 6529 2020 3a0a 2020 2020 2020 2020 7365  e)  :.        se
-00015550: 6c66 2e70 6572 6d69 745f 6361 6368 696e  lf.permit_cachin
-00015560: 6728 290a 2020 2020 2020 2020 6966 2065  g().        if e
-00015570: 7874 2e65 6e64 7377 6974 6828 222f 2229  xt.endswith("/")
-00015580: 3a0a 2020 2020 2020 2020 2020 2020 6578  :.            ex
-00015590: 7420 3d20 2266 6f6c 6465 7222 0a20 2020  t = "folder".   
-000155a0: 2020 2020 2020 2020 2065 7861 6374 203d           exact =
-000155b0: 2054 7275 650a 0a20 2020 2020 2020 2062   True..        b
-000155c0: 6164 203d 2072 652e 636f 6d70 696c 6528  ad = re.compile(
-000155d0: 7222 5b5d 2829 7b7d 2f20 5b5d 7c5e 5b30  r"[](){}/ []|^[0
-000155e0: 2d39 5f2d 5d2a 2422 290a 2020 2020 2020  -9_-]*$").      
-000155f0: 2020 6e20 3d20 6578 742e 7370 6c69 7428    n = ext.split(
-00015600: 222e 2229 5b3a 3a2d 315d 0a20 2020 2020  ".")[::-1].     
-00015610: 2020 2069 6620 6e6f 7420 6578 6163 743a     if not exact:
-00015620: 0a20 2020 2020 2020 2020 2020 206e 203d  .            n =
-00015630: 206e 5b3a 2d31 5d0a 0a20 2020 2020 2020   n[:-1]..       
-00015640: 2065 7874 203d 2022 220a 2020 2020 2020   ext = "".      
-00015650: 2020 666f 7220 7620 696e 206e 3a0a 2020    for v in n:.  
-00015660: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00015670: 2876 2920 3e20 3720 6f72 2062 6164 2e73  (v) > 7 or bad.s
-00015680: 6561 7263 6828 7629 3a0a 2020 2020 2020  earch(v):.      
-00015690: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-000156a0: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
-000156b0: 203d 2022 7b7d 2e7b 7d22 2e66 6f72 6d61   = "{}.{}".forma
-000156c0: 7428 762c 2065 7874 290a 0a20 2020 2020  t(v, ext)..     
-000156d0: 2020 2065 7874 203d 2065 7874 2e72 7374     ext = ext.rst
-000156e0: 7269 7028 222e 2229 206f 7220 2275 6e6b  rip(".") or "unk
-000156f0: 220a 2020 2020 2020 2020 6966 206c 656e  ".        if len
-00015700: 2865 7874 2920 3e20 3131 3a0a 2020 2020  (ext) > 11:.    
-00015710: 2020 2020 2020 2020 6578 7420 3d20 22e2          ext = ".
-00015720: 8baf 2220 2b20 6578 745b 2d39 3a5d 0a0a  .." + ext[-9:]..
-00015730: 2020 2020 2020 2020 2320 6368 726f 6d65          # chrome
-00015740: 2063 616e 6e6f 7420 6861 6e64 6c65 206d   cannot handle m
-00015750: 6f72 6520 7468 616e 207e 3230 3030 2075  ore than ~2000 u
-00015760: 6e69 7175 6520 5356 4773 0a20 2020 2020  nique SVGs.     
-00015770: 2020 2063 6872 6f6d 6520 3d20 2220 7276     chrome = " rv
-00015780: 3a22 206e 6f74 2069 6e20 7365 6c66 2e75  :" not in self.u
-00015790: 610a 2020 2020 2020 2020 6d69 6d65 2c20  a.        mime, 
-000157a0: 6963 6f20 3d20 7365 6c66 2e69 636f 2e67  ico = self.ico.g
-000157b0: 6574 2865 7874 2c20 6e6f 7420 6578 6163  et(ext, not exac
-000157c0: 742c 2063 6872 6f6d 6529 0a0a 2020 2020  t, chrome)..    
-000157d0: 2020 2020 6c6d 203d 2066 6f72 6d61 7464      lm = formatd
-000157e0: 6174 6528 7365 6c66 2e45 2e74 302c 2075  ate(self.E.t0, u
-000157f0: 7365 676d 743d 5472 7565 290a 2020 2020  segmt=True).    
-00015800: 2020 2020 7365 6c66 2e72 6570 6c79 2869      self.reply(i
-00015810: 636f 2c20 6d69 6d65 3d6d 696d 652c 2068  co, mime=mime, h
-00015820: 6561 6465 7273 3d7b 224c 6173 742d 4d6f  eaders={"Last-Mo
-00015830: 6469 6669 6564 223a 206c 6d7d 290a 2020  dified": lm}).  
-00015840: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00015850: 650a 0a20 2020 2064 6566 2074 785f 6d64  e..    def tx_md
-00015860: 2873 656c 662c 2066 735f 7061 7468 2029  (self, fs_path )
-00015870: 2020 3a0a 2020 2020 2020 2020 6c6f 676d    :.        logm
-00015880: 7367 203d 2022 7b3a 347d 207b 7d20 222e  sg = "{:4} {} ".
-00015890: 666f 726d 6174 2822 222c 2073 656c 662e  format("", self.
-000158a0: 7265 7129 0a0a 2020 2020 2020 2020 6966  req)..        if
-000158b0: 206e 6f74 2073 656c 662e 6361 6e5f 7772   not self.can_wr
-000158c0: 6974 653a 0a20 2020 2020 2020 2020 2020  ite:.           
-000158d0: 2069 6620 2265 6469 7422 2069 6e20 7365   if "edit" in se
-000158e0: 6c66 2e75 7061 7261 6d20 6f72 2022 6564  lf.uparam or "ed
-000158f0: 6974 3222 2069 6e20 7365 6c66 2e75 7061  it2" in self.upa
-00015900: 7261 6d3a 0a20 2020 2020 2020 2020 2020  ram:.           
-00015910: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00015920: 2e74 785f 3430 3428 5472 7565 290a 0a20  .tx_404(True).. 
-00015930: 2020 2020 2020 2074 706c 203d 2022 6d64         tpl = "md
-00015940: 6522 2069 6620 2265 6469 7432 2220 696e  e" if "edit2" in
-00015950: 2073 656c 662e 7570 6172 616d 2065 6c73   self.uparam els
-00015960: 6520 226d 6422 0a20 2020 2020 2020 2068  e "md".        h
-00015970: 746d 6c5f 7061 7468 203d 206f 732e 7061  tml_path = os.pa
-00015980: 7468 2e6a 6f69 6e28 7365 6c66 2e45 2e6d  th.join(self.E.m
-00015990: 6f64 2c20 2277 6562 222c 2022 7b7d 2e68  od, "web", "{}.h
-000159a0: 746d 6c22 2e66 6f72 6d61 7428 7470 6c29  tml".format(tpl)
-000159b0: 290a 2020 2020 2020 2020 7465 6d70 6c61  ).        templa
-000159c0: 7465 203d 2073 656c 662e 6a32 6a28 7470  te = self.j2j(tp
-000159d0: 6c29 0a0a 2020 2020 2020 2020 7374 203d  l)..        st =
-000159e0: 2062 6f73 2e73 7461 7428 6673 5f70 6174   bos.stat(fs_pat
-000159f0: 6829 0a20 2020 2020 2020 2074 735f 6d64  h).        ts_md
-00015a00: 203d 2073 742e 7374 5f6d 7469 6d65 0a0a   = st.st_mtime..
-00015a10: 2020 2020 2020 2020 7374 203d 2062 6f73          st = bos
-00015a20: 2e73 7461 7428 6874 6d6c 5f70 6174 6829  .stat(html_path)
-00015a30: 0a20 2020 2020 2020 2074 735f 6874 6d6c  .        ts_html
-00015a40: 203d 2073 742e 7374 5f6d 7469 6d65 0a0a   = st.st_mtime..
-00015a50: 2020 2020 2020 2020 737a 5f6d 6420 3d20          sz_md = 
-00015a60: 300a 2020 2020 2020 2020 666f 7220 6275  0.        for bu
-00015a70: 6620 696e 2079 6965 6c64 6669 6c65 2866  f in yieldfile(f
-00015a80: 735f 7061 7468 293a 0a20 2020 2020 2020  s_path):.       
-00015a90: 2020 2020 2073 7a5f 6d64 202b 3d20 6c65       sz_md += le
-00015aa0: 6e28 6275 6629 0a20 2020 2020 2020 2020  n(buf).         
-00015ab0: 2020 2066 6f72 2063 2c20 7620 696e 205b     for c, v in [
-00015ac0: 2862 2226 222c 2034 292c 2028 6222 3c22  (b"&", 4), (b"<"
-00015ad0: 2c20 3329 2c20 2862 223e 222c 2033 295d  , 3), (b">", 3)]
-00015ae0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015af0: 2020 737a 5f6d 6420 2b3d 2028 6c65 6e28    sz_md += (len(
-00015b00: 6275 6629 202d 206c 656e 2862 7566 2e72  buf) - len(buf.r
-00015b10: 6570 6c61 6365 2863 2c20 6222 2229 2929  eplace(c, b"")))
-00015b20: 202a 2076 0a0a 2020 2020 2020 2020 6669   * v..        fi
-00015b30: 6c65 5f74 7320 3d20 696e 7428 6d61 7828  le_ts = int(max(
-00015b40: 7473 5f6d 642c 2074 735f 6874 6d6c 2c20  ts_md, ts_html, 
-00015b50: 7365 6c66 2e45 2e74 3029 290a 2020 2020  self.E.t0)).    
-00015b60: 2020 2020 6669 6c65 5f6c 6173 746d 6f64      file_lastmod
-00015b70: 2c20 646f 5f73 656e 6420 3d20 7365 6c66  , do_send = self
-00015b80: 2e5f 6368 6b5f 6c61 7374 6d6f 6428 6669  ._chk_lastmod(fi
-00015b90: 6c65 5f74 7329 0a20 2020 2020 2020 2073  le_ts).        s
-00015ba0: 656c 662e 6f75 745f 6865 6164 6572 735b  elf.out_headers[
-00015bb0: 224c 6173 742d 4d6f 6469 6669 6564 225d  "Last-Modified"]
-00015bc0: 203d 2066 696c 655f 6c61 7374 6d6f 640a   = file_lastmod.
-00015bd0: 2020 2020 2020 2020 7365 6c66 2e6f 7574          self.out
-00015be0: 5f68 6561 6465 7273 2e75 7064 6174 6528  _headers.update(
-00015bf0: 4e4f 5f43 4143 4845 290a 2020 2020 2020  NO_CACHE).      
-00015c00: 2020 7374 6174 7573 203d 2032 3030 2069    status = 200 i
-00015c10: 6620 646f 5f73 656e 6420 656c 7365 2033  f do_send else 3
-00015c20: 3034 0a0a 2020 2020 2020 2020 6172 675f  04..        arg_
-00015c30: 6261 7365 203d 2022 3f22 0a20 2020 2020  base = "?".     
-00015c40: 2020 2069 6620 226b 2220 696e 2073 656c     if "k" in sel
-00015c50: 662e 7570 6172 616d 3a0a 2020 2020 2020  f.uparam:.      
-00015c60: 2020 2020 2020 6172 675f 6261 7365 203d        arg_base =
-00015c70: 2022 3f6b 3d7b 7d26 222e 666f 726d 6174   "?k={}&".format
-00015c80: 2873 656c 662e 7570 6172 616d 5b22 6b22  (self.uparam["k"
-00015c90: 5d29 0a0a 2020 2020 2020 2020 626f 756e  ])..        boun
-00015ca0: 6461 7279 203d 2022 5c72 6f6c 6c5c 7469  dary = "\roll\ti
-00015cb0: 6465 220a 2020 2020 2020 2020 7461 7267  de".        targ
-00015cc0: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
-00015cd0: 2020 2272 223a 2073 656c 662e 6172 6773    "r": self.args
-00015ce0: 2e53 5220 6966 2073 656c 662e 6973 5f76  .SR if self.is_v
-00015cf0: 7072 6f78 6965 6420 656c 7365 2022 222c  proxied else "",
-00015d00: 0a20 2020 2020 2020 2020 2020 2022 7473  .            "ts
-00015d10: 223a 2073 656c 662e 636f 6e6e 2e68 7372  ": self.conn.hsr
-00015d20: 762e 6361 6368 6562 7573 7465 7228 292c  v.cachebuster(),
-00015d30: 0a20 2020 2020 2020 2020 2020 2022 7376  .            "sv
-00015d40: 636e 616d 6522 3a20 7365 6c66 2e61 7267  cname": self.arg
-00015d50: 732e 646f 6374 6974 6c65 2c0a 2020 2020  s.doctitle,.    
-00015d60: 2020 2020 2020 2020 2268 746d 6c5f 6865          "html_he
-00015d70: 6164 223a 2073 656c 662e 6874 6d6c 5f68  ad": self.html_h
-00015d80: 6561 642c 0a20 2020 2020 2020 2020 2020  ead,.           
-00015d90: 2022 6564 6974 223a 2022 6564 6974 2220   "edit": "edit" 
-00015da0: 696e 2073 656c 662e 7570 6172 616d 2c0a  in self.uparam,.
-00015db0: 2020 2020 2020 2020 2020 2020 2274 6974              "tit
-00015dc0: 6c65 223a 2068 746d 6c5f 6573 6361 7065  le": html_escape
-00015dd0: 2873 656c 662e 7670 6174 682c 2063 726c  (self.vpath, crl
-00015de0: 663d 5472 7565 292c 0a20 2020 2020 2020  f=True),.       
-00015df0: 2020 2020 2022 6c61 7374 6d6f 6422 3a20       "lastmod": 
-00015e00: 696e 7428 7473 5f6d 6420 2a20 3130 3030  int(ts_md * 1000
-00015e10: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
-00015e20: 6c61 6e67 223a 2073 656c 662e 6172 6773  lang": self.args
-00015e30: 2e6c 616e 672c 0a20 2020 2020 2020 2020  .lang,.         
-00015e40: 2020 2022 6661 7669 636f 223a 2073 656c     "favico": sel
-00015e50: 662e 6172 6773 2e66 6176 6963 6f2c 0a20  f.args.favico,. 
-00015e60: 2020 2020 2020 2020 2020 2022 6861 7665             "have
-00015e70: 5f65 6d70 223a 2073 656c 662e 6172 6773  _emp": self.args
-00015e80: 2e65 6d70 2c0a 2020 2020 2020 2020 2020  .emp,.          
-00015e90: 2020 226d 645f 6368 6b5f 7261 7465 223a    "md_chk_rate":
-00015ea0: 2073 656c 662e 6172 6773 2e6d 6372 2c0a   self.args.mcr,.
-00015eb0: 2020 2020 2020 2020 2020 2020 226d 6422              "md"
-00015ec0: 3a20 626f 756e 6461 7279 2c0a 2020 2020  : boundary,.    
-00015ed0: 2020 2020 2020 2020 2261 7267 5f62 6173          "arg_bas
-00015ee0: 6522 3a20 6172 675f 6261 7365 2c0a 2020  e": arg_base,.  
-00015ef0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00015f00: 7a73 203d 2074 656d 706c 6174 652e 7265  zs = template.re
-00015f10: 6e64 6572 282a 2a74 6172 6773 292e 656e  nder(**targs).en
-00015f20: 636f 6465 2822 7574 662d 3822 2c20 2272  code("utf-8", "r
-00015f30: 6570 6c61 6365 2229 0a20 2020 2020 2020  eplace").       
-00015f40: 2068 746d 6c20 3d20 7a73 2e73 706c 6974   html = zs.split
-00015f50: 2862 6f75 6e64 6172 792e 656e 636f 6465  (boundary.encode
-00015f60: 2822 7574 662d 3822 2929 0a20 2020 2020  ("utf-8")).     
-00015f70: 2020 2069 6620 6c65 6e28 6874 6d6c 2920     if len(html) 
-00015f80: 213d 2032 3a0a 2020 2020 2020 2020 2020  != 2:.          
-00015f90: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00015fa0: 6e28 2262 6f75 6e64 6172 7920 6170 7065  n("boundary appe
-00015fb0: 6172 7320 696e 2022 202b 2068 746d 6c5f  ars in " + html_
-00015fc0: 7061 7468 290a 0a20 2020 2020 2020 2073  path)..        s
-00015fd0: 656c 662e 7365 6e64 5f68 6561 6465 7273  elf.send_headers
-00015fe0: 2873 7a5f 6d64 202b 206c 656e 2868 746d  (sz_md + len(htm
-00015ff0: 6c5b 305d 2920 2b20 6c65 6e28 6874 6d6c  l[0]) + len(html
-00016000: 5b31 5d29 2c20 7374 6174 7573 290a 0a20  [1]), status).. 
-00016010: 2020 2020 2020 206c 6f67 6d73 6720 2b3d         logmsg +=
-00016020: 2075 6e69 636f 6465 2873 7461 7475 7329   unicode(status)
-00016030: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00016040: 2e6d 6f64 6520 3d3d 2022 4845 4144 2220  .mode == "HEAD" 
-00016050: 6f72 206e 6f74 2064 6f5f 7365 6e64 3a0a  or not do_send:.
-00016060: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00016070: 656c 662e 646f 5f6c 6f67 3a0a 2020 2020  elf.do_log:.    
-00016080: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016090: 2e6c 6f67 286c 6f67 6d73 6729 0a0a 2020  .log(logmsg)..  
-000160a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000160b0: 2054 7275 650a 0a20 2020 2020 2020 2074   True..        t
-000160c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-000160d0: 7365 6c66 2e73 2e73 656e 6461 6c6c 2868  self.s.sendall(h
-000160e0: 746d 6c5b 305d 290a 2020 2020 2020 2020  tml[0]).        
-000160f0: 2020 2020 666f 7220 6275 6620 696e 2079      for buf in y
-00016100: 6965 6c64 6669 6c65 2866 735f 7061 7468  ieldfile(fs_path
-00016110: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00016120: 2020 2073 656c 662e 732e 7365 6e64 616c     self.s.sendal
-00016130: 6c28 6874 6d6c 5f62 6573 6361 7065 2862  l(html_bescape(b
-00016140: 7566 2929 0a0a 2020 2020 2020 2020 2020  uf))..          
-00016150: 2020 7365 6c66 2e73 2e73 656e 6461 6c6c    self.s.sendall
-00016160: 2868 746d 6c5b 315d 290a 0a20 2020 2020  (html[1])..     
-00016170: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
-00016180: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
-00016190: 6c6f 676d 7367 202b 2022 205c 3033 335b  logmsg + " \033[
-000161a0: 3331 6d64 2f63 5c30 3333 5b30 6d22 290a  31md/c\033[0m").
-000161b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000161c0: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
-000161d0: 2020 6966 2073 656c 662e 646f 5f6c 6f67    if self.do_log
-000161e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000161f0: 6c66 2e6c 6f67 286c 6f67 6d73 6720 2b20  lf.log(logmsg + 
-00016200: 2220 2220 2b20 756e 6963 6f64 6528 6c65  " " + unicode(le
-00016210: 6e28 6874 6d6c 2929 290a 0a20 2020 2020  n(html)))..     
-00016220: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00016230: 2020 2020 6465 6620 7478 5f73 7663 7328      def tx_svcs(
-00016240: 7365 6c66 2920 203a 0a20 2020 2020 2020  self)  :.       
-00016250: 2061 6e61 6d65 203d 2072 652e 7375 6228   aname = re.sub(
-00016260: 225b 5e30 2d39 612d 7a41 2d5a 5d2b 222c  "[^0-9a-zA-Z]+",
-00016270: 2022 222c 2073 656c 662e 6172 6773 2e6e   "", self.args.n
-00016280: 616d 6529 206f 7220 2261 220a 2020 2020  ame) or "a".    
-00016290: 2020 2020 6570 203d 2073 656c 662e 686f      ep = self.ho
-000162a0: 7374 0a20 2020 2020 2020 2068 6f73 7420  st.        host 
-000162b0: 3d20 6570 2e73 706c 6974 2822 3a22 295b  = ep.split(":")[
-000162c0: 305d 0a20 2020 2020 2020 2068 706f 7274  0].        hport
-000162d0: 203d 2065 705b 6570 2e66 696e 6428 223a   = ep[ep.find(":
-000162e0: 2229 203a 5d20 6966 2022 3a22 2069 6e20  ") :] if ":" in 
-000162f0: 6570 2065 6c73 6520 2222 0a20 2020 2020  ep else "".     
-00016300: 2020 2072 6970 203d 2028 0a20 2020 2020     rip = (.     
-00016310: 2020 2020 2020 2068 6f73 740a 2020 2020         host.    
-00016320: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00016330: 6172 6773 2e72 636c 6f6e 655f 6d64 6e73  args.rclone_mdns
-00016340: 206f 7220 6e6f 7420 7365 6c66 2e61 7267   or not self.arg
-00016350: 732e 7a6d 0a20 2020 2020 2020 2020 2020  s.zm.           
-00016360: 2065 6c73 6520 7365 6c66 2e63 6f6e 6e2e   else self.conn.
-00016370: 6873 7276 2e6e 6d2e 6d61 7028 7365 6c66  hsrv.nm.map(self
-00016380: 2e69 7029 206f 7220 686f 7374 0a20 2020  .ip) or host.   
-00016390: 2020 2020 2029 0a20 2020 2020 2020 2076       ).        v
-000163a0: 7020 3d20 2873 656c 662e 7570 6172 616d  p = (self.uparam
-000163b0: 5b22 6863 225d 206f 7220 2222 292e 6c73  ["hc"] or "").ls
-000163c0: 7472 6970 2822 2f22 290a 2020 2020 2020  trip("/").      
-000163d0: 2020 6874 6d6c 203d 2073 656c 662e 6a32    html = self.j2
-000163e0: 7328 0a20 2020 2020 2020 2020 2020 2022  s(.            "
-000163f0: 7376 6373 222c 0a20 2020 2020 2020 2020  svcs",.         
-00016400: 2020 2061 7267 733d 7365 6c66 2e61 7267     args=self.arg
-00016410: 732c 0a20 2020 2020 2020 2020 2020 2061  s,.            a
-00016420: 6363 733d 626f 6f6c 2873 656c 662e 6173  ccs=bool(self.as
-00016430: 7276 2e61 6363 7429 2c0a 2020 2020 2020  rv.acct),.      
-00016440: 2020 2020 2020 733d 2273 2220 6966 2073        s="s" if s
-00016450: 656c 662e 6973 5f68 7474 7073 2065 6c73  elf.is_https els
-00016460: 6520 2222 2c0a 2020 2020 2020 2020 2020  e "",.          
-00016470: 2020 7269 703d 7269 702c 0a20 2020 2020    rip=rip,.     
-00016480: 2020 2020 2020 2065 703d 6570 2c0a 2020         ep=ep,.  
-00016490: 2020 2020 2020 2020 2020 7670 3d76 702c            vp=vp,
-000164a0: 0a20 2020 2020 2020 2020 2020 2072 7670  .            rvp
-000164b0: 3d76 6a6f 696e 2873 656c 662e 6172 6773  =vjoin(self.args
-000164c0: 2e52 2c20 7670 292c 0a20 2020 2020 2020  .R, vp),.       
-000164d0: 2020 2020 2068 6f73 743d 686f 7374 2c0a       host=host,.
-000164e0: 2020 2020 2020 2020 2020 2020 6870 6f72              hpor
-000164f0: 743d 6870 6f72 742c 0a20 2020 2020 2020  t=hport,.       
-00016500: 2020 2020 2061 6e61 6d65 3d61 6e61 6d65       aname=aname
-00016510: 2c0a 2020 2020 2020 2020 2020 2020 7077  ,.            pw
-00016520: 3d73 656c 662e 7077 206f 7220 2270 7722  =self.pw or "pw"
-00016530: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00016540: 2020 2020 7365 6c66 2e72 6570 6c79 2868      self.reply(h
-00016550: 746d 6c2e 656e 636f 6465 2822 7574 662d  tml.encode("utf-
-00016560: 3822 2929 0a20 2020 2020 2020 2072 6574  8")).        ret
-00016570: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
-00016580: 6620 7478 5f6d 6f75 6e74 7328 7365 6c66  f tx_mounts(self
-00016590: 2920 203a 0a20 2020 2020 2020 2073 7566  )  :.        suf
-000165a0: 203d 2073 656c 662e 7572 6c71 287b 7d2c   = self.urlq({},
-000165b0: 205b 2268 225d 290a 2020 2020 2020 2020   ["h"]).        
-000165c0: 6176 6f6c 203d 205b 7820 666f 7220 7820  avol = [x for x 
-000165d0: 696e 2073 656c 662e 7776 6f6c 2069 6620  in self.wvol if 
-000165e0: 7820 696e 2073 656c 662e 7276 6f6c 5d0a  x in self.rvol].
-000165f0: 2020 2020 2020 2020 7276 6f6c 2c20 7776          rvol, wv
-00016600: 6f6c 2c20 6176 6f6c 203d 205b 0a20 2020  ol, avol = [.   
-00016610: 2020 2020 2020 2020 205b 2822 2f22 202b           [("/" +
-00016620: 2078 292e 7273 7472 6970 2822 2f22 2920   x).rstrip("/") 
-00016630: 2b20 222f 2220 666f 7220 7820 696e 2079  + "/" for x in y
-00016640: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00016650: 7220 7920 696e 205b 7365 6c66 2e72 766f  r y in [self.rvo
-00016660: 6c2c 2073 656c 662e 7776 6f6c 2c20 6176  l, self.wvol, av
-00016670: 6f6c 5d0a 2020 2020 2020 2020 5d0a 0a20  ol].        ].. 
-00016680: 2020 2020 2020 2069 6620 6176 6f6c 2061         if avol a
-00016690: 6e64 206e 6f74 2073 656c 662e 6172 6773  nd not self.args
-000166a0: 2e6e 6f5f 7265 7363 616e 3a0a 2020 2020  .no_rescan:.    
-000166b0: 2020 2020 2020 2020 7820 3d20 7365 6c66          x = self
-000166c0: 2e63 6f6e 6e2e 6873 7276 2e62 726f 6b65  .conn.hsrv.broke
-000166d0: 722e 6173 6b28 2275 7032 6b2e 6765 745f  r.ask("up2k.get_
-000166e0: 7374 6174 6522 290a 2020 2020 2020 2020  state").        
-000166f0: 2020 2020 7673 203d 206a 736f 6e2e 6c6f      vs = json.lo
-00016700: 6164 7328 782e 6765 7428 2929 0a20 2020  ads(x.get()).   
-00016710: 2020 2020 2020 2020 2076 7374 6174 6520           vstate 
-00016720: 3d20 7b28 222f 2220 2b20 6b29 2e72 7374  = {("/" + k).rst
-00016730: 7269 7028 222f 2229 202b 2022 2f22 3a20  rip("/") + "/": 
-00016740: 7620 666f 7220 6b2c 2076 2069 6e20 7673  v for k, v in vs
-00016750: 5b22 766f 6c73 7461 7465 225d 2e69 7465  ["volstate"].ite
-00016760: 6d73 2829 7d0a 2020 2020 2020 2020 656c  ms()}.        el
-00016770: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00016780: 7673 7461 7465 203d 207b 7d0a 2020 2020  vstate = {}.    
-00016790: 2020 2020 2020 2020 7673 203d 207b 0a20          vs = {. 
-000167a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000167b0: 7363 616e 6e69 6e67 223a 204e 6f6e 652c  scanning": None,
-000167c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000167d0: 2022 6861 7368 7122 3a20 4e6f 6e65 2c0a   "hashq": None,.
-000167e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167f0: 2274 6167 7122 3a20 4e6f 6e65 2c0a 2020  "tagq": None,.  
-00016800: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-00016810: 7470 7122 3a20 4e6f 6e65 2c0a 2020 2020  tpq": None,.    
-00016820: 2020 2020 2020 2020 2020 2020 2264 6277              "dbw
-00016830: 7422 3a20 4e6f 6e65 2c0a 2020 2020 2020  t": None,.      
-00016840: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-00016850: 2066 6d74 203d 2073 656c 662e 7570 6172   fmt = self.upar
-00016860: 616d 2e67 6574 2822 6c73 222c 2022 2229  am.get("ls", "")
-00016870: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00016880: 666d 7420 616e 6420 2873 656c 662e 7561  fmt and (self.ua
-00016890: 2e73 7461 7274 7377 6974 6828 2263 7572  .startswith("cur
-000168a0: 6c2f 2229 206f 7220 7365 6c66 2e75 612e  l/") or self.ua.
-000168b0: 7374 6172 7473 7769 7468 2822 6665 7463  startswith("fetc
-000168c0: 6822 2929 3a0a 2020 2020 2020 2020 2020  h")):.          
-000168d0: 2020 666d 7420 3d20 2276 220a 0a20 2020    fmt = "v"..   
-000168e0: 2020 2020 2069 6620 666d 7420 696e 205b       if fmt in [
-000168f0: 2276 222c 2022 7422 2c20 2274 7874 225d  "v", "t", "txt"]
-00016900: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00016910: 2073 656c 662e 756e 616d 6520 3d3d 2022   self.uname == "
-00016920: 2a22 3a0a 2020 2020 2020 2020 2020 2020  *":.            
-00016930: 2020 2020 7478 7420 3d20 2268 6f77 6479      txt = "howdy
-00016940: 2073 7472 616e 6765 7220 2879 6f75 2772   stranger (you'r
-00016950: 6520 6e6f 7420 6c6f 6767 6564 2069 6e29  e not logged in)
-00016960: 220a 2020 2020 2020 2020 2020 2020 656c  ".            el
-00016970: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00016980: 2020 2020 7478 7420 3d20 2277 656c 636f      txt = "welco
-00016990: 6d65 2062 6163 6b20 7b7d 222e 666f 726d  me back {}".form
-000169a0: 6174 2873 656c 662e 756e 616d 6529 0a0a  at(self.uname)..
-000169b0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-000169c0: 7374 6174 653a 0a20 2020 2020 2020 2020  state:.         
-000169d0: 2020 2020 2020 2074 7874 202b 3d20 225c         txt += "\
-000169e0: 6e73 7461 7475 733a 220a 2020 2020 2020  nstatus:".      
-000169f0: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
-00016a00: 696e 205b 2273 6361 6e6e 696e 6722 2c20  in ["scanning", 
-00016a10: 2268 6173 6871 222c 2022 7461 6771 222c  "hashq", "tagq",
-00016a20: 2022 6d74 7071 222c 2022 6462 7774 225d   "mtpq", "dbwt"]
-00016a30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016a40: 2020 2020 2020 7478 7420 2b3d 2022 207b        txt += " {
-00016a50: 7d28 7b7d 2922 2e66 6f72 6d61 7428 6b2c  }({})".format(k,
-00016a60: 2076 735b 6b5d 290a 0a20 2020 2020 2020   vs[k])..       
-00016a70: 2020 2020 2069 6620 7276 6f6c 3a0a 2020       if rvol:.  
-00016a80: 2020 2020 2020 2020 2020 2020 2020 7478                tx
-00016a90: 7420 2b3d 2022 5c6e 796f 7520 6361 6e20  t += "\nyou can 
-00016aa0: 6272 6f77 7365 3a22 0a20 2020 2020 2020  browse:".       
-00016ab0: 2020 2020 2020 2020 2066 6f72 2076 2069           for v i
-00016ac0: 6e20 7276 6f6c 3a0a 2020 2020 2020 2020  n rvol:.        
-00016ad0: 2020 2020 2020 2020 2020 2020 7478 7420              txt 
-00016ae0: 2b3d 2022 5c6e 2020 2220 2b20 760a 0a20  += "\n  " + v.. 
-00016af0: 2020 2020 2020 2020 2020 2069 6620 7776             if wv
-00016b00: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
-00016b10: 2020 2020 7478 7420 2b3d 2022 5c6e 796f      txt += "\nyo
-00016b20: 7520 6361 6e20 7570 6c6f 6164 2074 6f3a  u can upload to:
-00016b30: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00016b40: 2020 666f 7220 7620 696e 2077 766f 6c3a    for v in wvol:
-00016b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016b60: 2020 2020 2074 7874 202b 3d20 225c 6e20       txt += "\n 
-00016b70: 2022 202b 2076 0a0a 2020 2020 2020 2020   " + v..        
-00016b80: 2020 2020 7a62 203d 2074 7874 2e65 6e63      zb = txt.enc
-00016b90: 6f64 6528 2275 7466 2d38 222c 2022 7265  ode("utf-8", "re
-00016ba0: 706c 6163 6522 2920 2b20 6222 5c6e 220a  place") + b"\n".
-00016bb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016bc0: 2e72 6570 6c79 287a 622c 206d 696d 653d  .reply(zb, mime=
-00016bd0: 2274 6578 742f 706c 6169 6e3b 2063 6861  "text/plain; cha
-00016be0: 7273 6574 3d75 7466 2d38 2229 0a20 2020  rset=utf-8").   
-00016bf0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00016c00: 5472 7565 0a0a 2020 2020 2020 2020 6874  True..        ht
-00016c10: 6d6c 203d 2073 656c 662e 6a32 7328 0a20  ml = self.j2s(. 
-00016c20: 2020 2020 2020 2020 2020 2022 7370 6c61             "spla
-00016c30: 7368 222c 0a20 2020 2020 2020 2020 2020  sh",.           
-00016c40: 2074 6869 733d 7365 6c66 2c0a 2020 2020   this=self,.    
-00016c50: 2020 2020 2020 2020 7176 7061 7468 3d71          qvpath=q
-00016c60: 756f 7465 7028 7365 6c66 2e76 7061 7468  uotep(self.vpath
-00016c70: 292c 0a20 2020 2020 2020 2020 2020 2072  ),.            r
-00016c80: 766f 6c3d 7276 6f6c 2c0a 2020 2020 2020  vol=rvol,.      
-00016c90: 2020 2020 2020 7776 6f6c 3d77 766f 6c2c        wvol=wvol,
-00016ca0: 0a20 2020 2020 2020 2020 2020 2061 766f  .            avo
-00016cb0: 6c3d 6176 6f6c 2c0a 2020 2020 2020 2020  l=avol,.        
-00016cc0: 2020 2020 7673 7461 7465 3d76 7374 6174      vstate=vstat
-00016cd0: 652c 0a20 2020 2020 2020 2020 2020 2073  e,.            s
-00016ce0: 6361 6e6e 696e 673d 7673 5b22 7363 616e  canning=vs["scan
-00016cf0: 6e69 6e67 225d 2c0a 2020 2020 2020 2020  ning"],.        
-00016d00: 2020 2020 6861 7368 713d 7673 5b22 6861      hashq=vs["ha
-00016d10: 7368 7122 5d2c 0a20 2020 2020 2020 2020  shq"],.         
-00016d20: 2020 2074 6167 713d 7673 5b22 7461 6771     tagq=vs["tagq
-00016d30: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-00016d40: 6d74 7071 3d76 735b 226d 7470 7122 5d2c  mtpq=vs["mtpq"],
-00016d50: 0a20 2020 2020 2020 2020 2020 2064 6277  .            dbw
-00016d60: 743d 7673 5b22 6462 7774 225d 2c0a 2020  t=vs["dbwt"],.  
-00016d70: 2020 2020 2020 2020 2020 7572 6c5f 7375            url_su
-00016d80: 663d 7375 662c 0a20 2020 2020 2020 2020  f=suf,.         
-00016d90: 2020 206b 3330 343d 7365 6c66 2e6b 3330     k304=self.k30
-00016da0: 3428 292c 0a20 2020 2020 2020 2020 2020  4(),.           
-00016db0: 2076 6572 3d53 5f56 4552 5349 4f4e 2069   ver=S_VERSION i
-00016dc0: 6620 7365 6c66 2e61 7267 732e 7665 7220  f self.args.ver 
-00016dd0: 656c 7365 2022 222c 0a20 2020 2020 2020  else "",.       
-00016de0: 2020 2020 2061 6874 7470 733d 2222 2069       ahttps="" i
-00016df0: 6620 7365 6c66 2e69 735f 6874 7470 7320  f self.is_https 
-00016e00: 656c 7365 2022 6874 7470 733a 2f2f 2220  else "https://" 
-00016e10: 2b20 7365 6c66 2e68 6f73 7420 2b20 7365  + self.host + se
-00016e20: 6c66 2e72 6571 2c0a 2020 2020 2020 2020  lf.req,.        
-00016e30: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-00016e40: 6570 6c79 2868 746d 6c2e 656e 636f 6465  eply(html.encode
-00016e50: 2822 7574 662d 3822 2929 0a20 2020 2020  ("utf-8")).     
-00016e60: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00016e70: 2020 2020 6465 6620 7365 745f 6b33 3034      def set_k304
-00016e80: 2873 656c 6629 2020 3a0a 2020 2020 2020  (self)  :.      
-00016e90: 2020 636b 203d 2067 656e 636f 6f6b 6965    ck = gencookie
-00016ea0: 2822 6b33 3034 222c 2073 656c 662e 7570  ("k304", self.up
-00016eb0: 6172 616d 5b22 6b33 3034 225d 2c20 7365  aram["k304"], se
-00016ec0: 6c66 2e61 7267 732e 522c 2046 616c 7365  lf.args.R, False
-00016ed0: 2c20 3836 3430 3020 2a20 3239 3929 0a20  , 86400 * 299). 
-00016ee0: 2020 2020 2020 2073 656c 662e 6f75 745f         self.out_
-00016ef0: 6865 6164 6572 6c69 7374 2e61 7070 656e  headerlist.appen
-00016f00: 6428 2822 5365 742d 436f 6f6b 6965 222c  d(("Set-Cookie",
-00016f10: 2063 6b29 290a 2020 2020 2020 2020 7365   ck)).        se
-00016f20: 6c66 2e72 6564 6972 6563 7428 2222 2c20  lf.redirect("", 
-00016f30: 223f 6823 6363 2229 0a20 2020 2020 2020  "?h#cc").       
-00016f40: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-00016f50: 2020 6465 6620 7365 745f 616d 5f6a 7328    def set_am_js(
-00016f60: 7365 6c66 2920 203a 0a20 2020 2020 2020  self)  :.       
-00016f70: 2076 203d 2022 6e22 2069 6620 7365 6c66   v = "n" if self
-00016f80: 2e75 7061 7261 6d5b 2261 6d5f 6a73 225d  .uparam["am_js"]
-00016f90: 203d 3d20 226e 2220 656c 7365 2022 7922   == "n" else "y"
-00016fa0: 0a20 2020 2020 2020 2063 6b20 3d20 6765  .        ck = ge
-00016fb0: 6e63 6f6f 6b69 6528 226a 7322 2c20 762c  ncookie("js", v,
-00016fc0: 2073 656c 662e 6172 6773 2e52 2c20 4661   self.args.R, Fa
-00016fd0: 6c73 652c 2038 3634 3030 202a 2032 3939  lse, 86400 * 299
-00016fe0: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-00016ff0: 7574 5f68 6561 6465 726c 6973 742e 6170  ut_headerlist.ap
-00017000: 7065 6e64 2828 2253 6574 2d43 6f6f 6b69  pend(("Set-Cooki
-00017010: 6522 2c20 636b 2929 0a20 2020 2020 2020  e", ck)).       
-00017020: 2073 656c 662e 7265 706c 7928 6222 7072   self.reply(b"pr
-00017030: 6f6d 6f74 6564 5c6e 2229 0a20 2020 2020  omoted\n").     
-00017040: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00017050: 2020 2020 6465 6620 7365 745f 6366 675f      def set_cfg_
-00017060: 7265 7365 7428 7365 6c66 2920 203a 0a20  reset(self)  :. 
-00017070: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-00017080: 2822 6b33 3034 222c 2022 6a73 222c 2022  ("k304", "js", "
-00017090: 6370 7077 6422 2c20 2263 7070 7773 2229  cppwd", "cppws")
-000170a0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-000170b0: 6f6b 6965 203d 2067 656e 636f 6f6b 6965  okie = gencookie
-000170c0: 286b 2c20 2278 222c 2073 656c 662e 6172  (k, "x", self.ar
-000170d0: 6773 2e52 2c20 4661 6c73 652c 204e 6f6e  gs.R, False, Non
-000170e0: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-000170f0: 656c 662e 6f75 745f 6865 6164 6572 6c69  elf.out_headerli
-00017100: 7374 2e61 7070 656e 6428 2822 5365 742d  st.append(("Set-
-00017110: 436f 6f6b 6965 222c 2063 6f6f 6b69 6529  Cookie", cookie)
-00017120: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00017130: 7265 6469 7265 6374 2822 222c 2022 3f68  redirect("", "?h
-00017140: 2363 6322 290a 2020 2020 2020 2020 7265  #cc").        re
-00017150: 7475 726e 2054 7275 650a 0a20 2020 2064  turn True..    d
-00017160: 6566 2074 785f 3430 3428 7365 6c66 2c20  ef tx_404(self, 
-00017170: 6973 5f34 3033 2020 3d20 4661 6c73 6529  is_403  = False)
-00017180: 2020 3a0a 2020 2020 2020 2020 7263 203d    :.        rc =
-00017190: 2034 3034 0a20 2020 2020 2020 2069 6620   404.        if 
-000171a0: 7365 6c66 2e61 7267 732e 7661 6775 655f  self.args.vague_
-000171b0: 3430 333a 0a20 2020 2020 2020 2020 2020  403:.           
-000171c0: 2074 203d 2027 3c68 3120 6964 3d22 6e22   t = '<h1 id="n"
-000171d0: 3e34 3034 206e 6f74 2066 6f75 6e64 2026  >404 not found &
-000171e0: 6e62 7370 3be2 9490 2820 c2b4 202d 6029  nbsp;...( .. -`)
-000171f0: e294 8c3c 2f68 313e 3c70 2069 643d 226f  ...</h1><p id="o
-00017200: 223e 6f72 206d 6179 6265 2079 6f75 2064  ">or maybe you d
-00017210: 6f6e 5c27 7420 6861 7665 2061 6363 6573  on\'t have acces
-00017220: 7320 2d2d 2074 7279 206c 6f67 6769 6e67  s -- try logging
-00017230: 2069 6e20 6f72 203c 6120 6872 6566 3d22   in or <a href="
-00017240: 7b7d 2f3f 6822 3e67 6f20 686f 6d65 3c2f  {}/?h">go home</
-00017250: 613e 3c2f 703e 270a 2020 2020 2020 2020  a></p>'.        
-00017260: 656c 6966 2069 735f 3430 333a 0a20 2020  elif is_403:.   
-00017270: 2020 2020 2020 2020 2074 203d 2027 3c68           t = '<h
-00017280: 3120 6964 3d22 7022 3e34 3033 2066 6f72  1 id="p">403 for
-00017290: 6269 6464 656e 6120 266e 6273 703b 7ee2  biddena &nbsp;~.
-000172a0: 94bb e294 81e2 94bb 3c2f 6831 3e3c 7020  ........</h1><p 
-000172b0: 6964 3d22 7122 3e79 6f75 5c27 6c6c 2068  id="q">you\'ll h
-000172c0: 6176 6520 746f 206c 6f67 2069 6e20 6f72  ave to log in or
-000172d0: 203c 6120 6872 6566 3d22 7b7d 2f3f 6822   <a href="{}/?h"
-000172e0: 3e67 6f20 686f 6d65 3c2f 613e 3c2f 703e  >go home</a></p>
-000172f0: 270a 2020 2020 2020 2020 2020 2020 7263  '.            rc
-00017300: 203d 2034 3033 0a20 2020 2020 2020 2065   = 403.        e
-00017310: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00017320: 2074 203d 2027 3c68 3120 6964 3d22 6e22   t = '<h1 id="n"
-00017330: 3e34 3034 206e 6f74 2066 6f75 6e64 2026  >404 not found &
-00017340: 6e62 7370 3be2 9490 2820 c2b4 202d 6029  nbsp;...( .. -`)
-00017350: e294 8c3c 2f68 313e 3c70 3e3c 6120 6964  ...</h1><p><a id
-00017360: 3d22 7222 2068 7265 663d 227b 7d2f 3f68  ="r" href="{}/?h
-00017370: 223e 676f 2068 6f6d 653c 2f61 3e3c 2f70  ">go home</a></p
-00017380: 3e27 0a0a 2020 2020 2020 2020 7420 3d20  >'..        t = 
-00017390: 742e 666f 726d 6174 2873 656c 662e 6172  t.format(self.ar
-000173a0: 6773 2e53 5229 0a20 2020 2020 2020 2068  gs.SR).        h
-000173b0: 746d 6c20 3d20 7365 6c66 2e6a 3273 2822  tml = self.j2s("
-000173c0: 7370 6c61 7368 222c 2074 6869 733d 7365  splash", this=se
-000173d0: 6c66 2c20 7176 7061 7468 3d71 756f 7465  lf, qvpath=quote
-000173e0: 7028 7365 6c66 2e76 7061 7468 292c 206d  p(self.vpath), m
-000173f0: 7367 3d74 290a 2020 2020 2020 2020 7365  sg=t).        se
-00017400: 6c66 2e72 6570 6c79 2868 746d 6c2e 656e  lf.reply(html.en
-00017410: 636f 6465 2822 7574 662d 3822 292c 2073  code("utf-8"), s
-00017420: 7461 7475 733d 7263 290a 2020 2020 2020  tatus=rc).      
-00017430: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
-00017440: 2020 2064 6566 2073 6361 6e76 6f6c 2873     def scanvol(s
-00017450: 656c 6629 2020 3a0a 2020 2020 2020 2020  elf)  :.        
-00017460: 6966 206e 6f74 2073 656c 662e 6361 6e5f  if not self.can_
-00017470: 7265 6164 206f 7220 6e6f 7420 7365 6c66  read or not self
-00017480: 2e63 616e 5f77 7269 7465 3a0a 2020 2020  .can_write:.    
-00017490: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
-000174a0: 626b 6163 2834 3033 2c20 226e 6f74 2061  bkac(403, "not a
-000174b0: 6c6c 6f77 6564 2066 6f72 2075 7365 7220  llowed for user 
-000174c0: 2220 2b20 7365 6c66 2e75 6e61 6d65 290a  " + self.uname).
-000174d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000174e0: 2e61 7267 732e 6e6f 5f72 6573 6361 6e3a  .args.no_rescan:
-000174f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00017500: 7365 2050 6562 6b61 6328 3430 332c 2022  se Pebkac(403, "
-00017510: 7468 6520 7265 7363 616e 2066 6561 7475  the rescan featu
-00017520: 7265 2069 7320 6469 7361 626c 6564 2069  re is disabled i
-00017530: 6e20 7365 7276 6572 2063 6f6e 6669 6722  n server config"
-00017540: 290a 0a20 2020 2020 2020 2076 6e2c 205f  )..        vn, _
-00017550: 203d 2073 656c 662e 6173 7276 2e76 6673   = self.asrv.vfs
-00017560: 2e67 6574 2873 656c 662e 7670 6174 682c  .get(self.vpath,
-00017570: 2073 656c 662e 756e 616d 652c 2054 7275   self.uname, Tru
-00017580: 652c 2054 7275 6529 0a0a 2020 2020 2020  e, True)..      
-00017590: 2020 6172 6773 203d 205b 7365 6c66 2e61    args = [self.a
-000175a0: 7372 762e 7666 732e 616c 6c5f 766f 6c73  srv.vfs.all_vols
-000175b0: 2c20 5b76 6e2e 7670 6174 685d 2c20 4661  , [vn.vpath], Fa
-000175c0: 6c73 652c 2054 7275 655d 0a0a 2020 2020  lse, True]..    
-000175d0: 2020 2020 7820 3d20 7365 6c66 2e63 6f6e      x = self.con
-000175e0: 6e2e 6873 7276 2e62 726f 6b65 722e 6173  n.hsrv.broker.as
-000175f0: 6b28 2275 7032 6b2e 7265 7363 616e 222c  k("up2k.rescan",
-00017600: 202a 6172 6773 290a 2020 2020 2020 2020   *args).        
-00017610: 6572 7220 3d20 782e 6765 7428 290a 2020  err = x.get().  
-00017620: 2020 2020 2020 6966 206e 6f74 2065 7272        if not err
-00017630: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00017640: 6c66 2e72 6564 6972 6563 7428 2222 2c20  lf.redirect("", 
-00017650: 223f 6822 290a 2020 2020 2020 2020 2020  "?h").          
-00017660: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
-00017670: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
-00017680: 6b61 6328 3530 302c 2065 7272 290a 0a20  kac(500, err).. 
-00017690: 2020 2064 6566 2068 616e 646c 655f 7265     def handle_re
-000176a0: 6c6f 6164 2873 656c 6629 2020 3a0a 2020  load(self)  :.  
-000176b0: 2020 2020 2020 6163 7420 3d20 7365 6c66        act = self
-000176c0: 2e75 7061 7261 6d2e 6765 7428 2272 656c  .uparam.get("rel
-000176d0: 6f61 6422 290a 2020 2020 2020 2020 6966  oad").        if
-000176e0: 2061 6374 2021 3d20 2263 6667 223a 0a20   act != "cfg":. 
-000176f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00017700: 2050 6562 6b61 6328 3430 302c 2022 6f6e   Pebkac(400, "on
-00017710: 6c79 2063 6f6e 6669 6720 6669 6c65 7320  ly config files 
-00017720: 2827 6366 6727 2920 6361 6e20 6265 2072  ('cfg') can be r
-00017730: 656c 6f61 6465 6420 726e 2229 0a0a 2020  eloaded rn")..  
-00017740: 2020 2020 2020 6966 206e 6f74 205b 7820        if not [x 
-00017750: 666f 7220 7820 696e 2073 656c 662e 7776  for x in self.wv
-00017760: 6f6c 2069 6620 7820 696e 2073 656c 662e  ol if x in self.
-00017770: 7276 6f6c 5d3a 0a20 2020 2020 2020 2020  rvol]:.         
-00017780: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
-00017790: 3430 332c 2022 6e6f 7420 616c 6c6f 7765  403, "not allowe
-000177a0: 6420 666f 7220 7573 6572 2022 202b 2073  d for user " + s
-000177b0: 656c 662e 756e 616d 6529 0a0a 2020 2020  elf.uname)..    
-000177c0: 2020 2020 6966 2073 656c 662e 6172 6773      if self.args
-000177d0: 2e6e 6f5f 7265 6c6f 6164 3a0a 2020 2020  .no_reload:.    
-000177e0: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
-000177f0: 626b 6163 2834 3033 2c20 2274 6865 2072  bkac(403, "the r
-00017800: 656c 6f61 6420 6665 6174 7572 6520 6973  eload feature is
-00017810: 2064 6973 6162 6c65 6420 696e 2073 6572   disabled in ser
-00017820: 7665 7220 636f 6e66 6967 2229 0a0a 2020  ver config")..  
-00017830: 2020 2020 2020 7820 3d20 7365 6c66 2e63        x = self.c
-00017840: 6f6e 6e2e 6873 7276 2e62 726f 6b65 722e  onn.hsrv.broker.
-00017850: 6173 6b28 2272 656c 6f61 6422 290a 2020  ask("reload").  
-00017860: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00017870: 662e 7265 6469 7265 6374 2822 222c 2022  f.redirect("", "
-00017880: 3f68 222c 2078 2e67 6574 2829 2c20 2272  ?h", x.get(), "r
-00017890: 6574 7572 6e20 746f 222c 2046 616c 7365  eturn to", False
-000178a0: 290a 0a20 2020 2064 6566 2074 785f 7374  )..    def tx_st
-000178b0: 6163 6b28 7365 6c66 2920 203a 0a20 2020  ack(self)  :.   
-000178c0: 2020 2020 2069 6620 6e6f 7420 5b78 2066       if not [x f
-000178d0: 6f72 2078 2069 6e20 7365 6c66 2e77 766f  or x in self.wvo
-000178e0: 6c20 6966 2078 2069 6e20 7365 6c66 2e72  l if x in self.r
-000178f0: 766f 6c5d 3a0a 2020 2020 2020 2020 2020  vol]:.          
-00017900: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
-00017910: 3033 2c20 226e 6f74 2061 6c6c 6f77 6564  03, "not allowed
-00017920: 2066 6f72 2075 7365 7220 2220 2b20 7365   for user " + se
-00017930: 6c66 2e75 6e61 6d65 290a 0a20 2020 2020  lf.uname)..     
-00017940: 2020 2069 6620 7365 6c66 2e61 7267 732e     if self.args.
-00017950: 6e6f 5f73 7461 636b 3a0a 2020 2020 2020  no_stack:.      
-00017960: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
-00017970: 6163 2834 3033 2c20 2274 6865 2073 7461  ac(403, "the sta
-00017980: 636b 6475 6d70 2066 6561 7475 7265 2069  ckdump feature i
-00017990: 7320 6469 7361 626c 6564 2069 6e20 7365  s disabled in se
-000179a0: 7276 6572 2063 6f6e 6669 6722 290a 0a20  rver config").. 
-000179b0: 2020 2020 2020 2072 6574 203d 2022 3c70         ret = "<p
-000179c0: 7265 3e7b 7d5c 6e7b 7d22 2e66 6f72 6d61  re>{}\n{}".forma
-000179d0: 7428 7469 6d65 2e74 696d 6528 292c 2068  t(time.time(), h
-000179e0: 746d 6c5f 6573 6361 7065 2861 6c6c 7472  tml_escape(alltr
-000179f0: 6163 6528 2929 290a 2020 2020 2020 2020  ace())).        
-00017a00: 7365 6c66 2e72 6570 6c79 2872 6574 2e65  self.reply(ret.e
-00017a10: 6e63 6f64 6528 2275 7466 2d38 2229 290a  ncode("utf-8")).
-00017a20: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00017a30: 7275 650a 0a20 2020 2064 6566 2074 785f  rue..    def tx_
-00017a40: 7472 6565 2873 656c 6629 2020 3a0a 2020  tree(self)  :.  
-00017a50: 2020 2020 2020 746f 7020 3d20 7365 6c66        top = self
-00017a60: 2e75 7061 7261 6d5b 2274 7265 6522 5d20  .uparam["tree"] 
-00017a70: 6f72 2022 220a 2020 2020 2020 2020 6473  or "".        ds
-00017a80: 7420 3d20 7365 6c66 2e76 7061 7468 0a20  t = self.vpath. 
-00017a90: 2020 2020 2020 2069 6620 746f 7020 696e         if top in
-00017aa0: 205b 222e 222c 2022 2e2e 225d 3a0a 2020   [".", ".."]:.  
-00017ab0: 2020 2020 2020 2020 2020 746f 7020 3d20            top = 
-00017ac0: 756e 646f 7428 7365 6c66 2e76 7061 7468  undot(self.vpath
-00017ad0: 202b 2022 2f22 202b 2074 6f70 290a 0a20   + "/" + top).. 
-00017ae0: 2020 2020 2020 2069 6620 746f 7020 3d3d         if top ==
-00017af0: 2064 7374 3a0a 2020 2020 2020 2020 2020   dst:.          
-00017b00: 2020 6473 7420 3d20 2222 0a20 2020 2020    dst = "".     
-00017b10: 2020 2065 6c69 6620 746f 703a 0a20 2020     elif top:.   
-00017b20: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00017b30: 6473 742e 7374 6172 7473 7769 7468 2874  dst.startswith(t
-00017b40: 6f70 202b 2022 2f22 293a 0a20 2020 2020  op + "/"):.     
-00017b50: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00017b60: 2050 6562 6b61 6328 3430 302c 2022 6172   Pebkac(400, "ar
-00017b70: 6720 6675 6e6b 2229 0a0a 2020 2020 2020  g funk")..      
-00017b80: 2020 2020 2020 6473 7420 3d20 6473 745b        dst = dst[
-00017b90: 6c65 6e28 746f 7029 202b 2031 203a 5d0a  len(top) + 1 :].
-00017ba0: 0a20 2020 2020 2020 2072 6574 203d 2073  .        ret = s
-00017bb0: 656c 662e 6765 6e5f 7472 6565 2874 6f70  elf.gen_tree(top
-00017bc0: 2c20 6473 7429 0a20 2020 2020 2020 2069  , dst).        i
-00017bd0: 6620 7365 6c66 2e69 735f 7670 726f 7869  f self.is_vproxi
-00017be0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-00017bf0: 7061 7265 6e74 7320 3d20 7365 6c66 2e61  parents = self.a
-00017c00: 7267 732e 522e 7370 6c69 7428 222f 2229  rgs.R.split("/")
-00017c10: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00017c20: 2070 6172 656e 7420 696e 2070 6172 656e   parent in paren
-00017c30: 7473 5b3a 3a2d 315d 3a0a 2020 2020 2020  ts[::-1]:.      
-00017c40: 2020 2020 2020 2020 2020 7265 7420 3d20            ret = 
-00017c50: 7b22 6b7b 7d22 2e66 6f72 6d61 7428 7061  {"k{}".format(pa
-00017c60: 7265 6e74 293a 2072 6574 2c20 2261 223a  rent): ret, "a":
-00017c70: 205b 5d7d 0a0a 2020 2020 2020 2020 7a73   []}..        zs
-00017c80: 203d 206a 736f 6e2e 6475 6d70 7328 7265   = json.dumps(re
-00017c90: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-00017ca0: 7265 706c 7928 7a73 2e65 6e63 6f64 6528  reply(zs.encode(
-00017cb0: 2275 7466 2d38 2229 2c20 6d69 6d65 3d22  "utf-8"), mime="
-00017cc0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00017cd0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00017ce0: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
-00017cf0: 6765 6e5f 7472 6565 2873 656c 662c 2074  gen_tree(self, t
-00017d00: 6f70 202c 2074 6172 6765 7420 2920 2020  op , target )   
-00017d10: 3a0a 2020 2020 2020 2020 7265 7420 2020  :.        ret   
-00017d20: 3d20 7b7d 0a20 2020 2020 2020 2065 7863  = {}.        exc
-00017d30: 6c20 3d20 4e6f 6e65 0a20 2020 2020 2020  l = None.       
-00017d40: 2069 6620 7461 7267 6574 3a0a 2020 2020   if target:.    
-00017d50: 2020 2020 2020 2020 6578 636c 2c20 7461          excl, ta
-00017d60: 7267 6574 203d 2028 7461 7267 6574 2e73  rget = (target.s
-00017d70: 706c 6974 2822 2f22 2c20 3129 202b 205b  plit("/", 1) + [
-00017d80: 2222 5d29 5b3a 325d 0a20 2020 2020 2020  ""])[:2].       
-00017d90: 2020 2020 2073 7562 203d 2073 656c 662e       sub = self.
-00017da0: 6765 6e5f 7472 6565 2822 2f22 2e6a 6f69  gen_tree("/".joi
-00017db0: 6e28 5b74 6f70 2c20 6578 636c 5d29 2e73  n([top, excl]).s
-00017dc0: 7472 6970 2822 2f22 292c 2074 6172 6765  trip("/"), targe
-00017dd0: 7429 0a20 2020 2020 2020 2020 2020 2072  t).            r
-00017de0: 6574 5b22 6b22 202b 2071 756f 7465 7028  et["k" + quotep(
-00017df0: 6578 636c 295d 203d 2073 7562 0a0a 2020  excl)] = sub..  
-00017e00: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00017e10: 2020 2020 2020 2076 6e2c 2072 656d 203d         vn, rem =
-00017e20: 2073 656c 662e 6173 7276 2e76 6673 2e67   self.asrv.vfs.g
-00017e30: 6574 2874 6f70 2c20 7365 6c66 2e75 6e61  et(top, self.una
-00017e40: 6d65 2c20 5472 7565 2c20 4661 6c73 6529  me, True, False)
-00017e50: 0a20 2020 2020 2020 2020 2020 2066 7372  .            fsr
-00017e60: 6f6f 742c 2076 6673 5f6c 732c 2076 6673  oot, vfs_ls, vfs
-00017e70: 5f76 6972 7420 3d20 766e 2e6c 7328 0a20  _virt = vn.ls(. 
-00017e80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00017e90: 656d 2c0a 2020 2020 2020 2020 2020 2020  em,.            
-00017ea0: 2020 2020 7365 6c66 2e75 6e61 6d65 2c0a      self.uname,.
-00017eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ec0: 6e6f 7420 7365 6c66 2e61 7267 732e 6e6f  not self.args.no
-00017ed0: 5f73 6361 6e64 6972 2c0a 2020 2020 2020  _scandir,.      
-00017ee0: 2020 2020 2020 2020 2020 5b5b 5472 7565            [[True
-00017ef0: 2c20 4661 6c73 655d 2c20 5b46 616c 7365  , False], [False
-00017f00: 2c20 5472 7565 5d5d 2c0a 2020 2020 2020  , True]],.      
-00017f10: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00017f20: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00017f30: 2020 2020 7666 735f 6c73 203d 205b 5d0a      vfs_ls = [].
-00017f40: 2020 2020 2020 2020 2020 2020 7666 735f              vfs_
-00017f50: 7669 7274 203d 207b 7d0a 2020 2020 2020  virt = {}.      
-00017f60: 2020 2020 2020 666f 7220 7620 696e 2073        for v in s
-00017f70: 656c 662e 7276 6f6c 3a0a 2020 2020 2020  elf.rvol:.      
-00017f80: 2020 2020 2020 2020 2020 6431 2c20 6432            d1, d2
-00017f90: 203d 2076 2e72 7370 6c69 7428 222f 222c   = v.rsplit("/",
-00017fa0: 2031 2920 6966 2022 2f22 2069 6e20 7620   1) if "/" in v 
-00017fb0: 656c 7365 205b 2222 2c20 765d 0a20 2020  else ["", v].   
-00017fc0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00017fd0: 6431 203d 3d20 746f 703a 0a20 2020 2020  d1 == top:.     
-00017fe0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00017ff0: 6673 5f76 6972 745b 6432 5d20 3d20 7365  fs_virt[d2] = se
-00018000: 6c66 2e61 7372 762e 7666 7320 2023 2074  lf.asrv.vfs  # t
-00018010: 7970 6563 686b 2c20 7661 6c75 6520 6e65  ypechk, value ne
-00018020: 7665 7220 7265 6164 0a0a 2020 2020 2020  ver read..      
-00018030: 2020 6469 7273 203d 205b 5d0a 0a20 2020    dirs = []..   
-00018040: 2020 2020 2064 6972 6e61 6d65 7320 3d20       dirnames = 
-00018050: 5b78 5b30 5d20 666f 7220 7820 696e 2076  [x[0] for x in v
-00018060: 6673 5f6c 7320 6966 2073 7461 742e 535f  fs_ls if stat.S_
-00018070: 4953 4449 5228 785b 315d 2e73 745f 6d6f  ISDIR(x[1].st_mo
-00018080: 6465 295d 0a0a 2020 2020 2020 2020 6966  de)]..        if
-00018090: 206e 6f74 2073 656c 662e 6172 6773 2e65   not self.args.e
-000180a0: 6420 6f72 2022 646f 7473 2220 6e6f 7420  d or "dots" not 
-000180b0: 696e 2073 656c 662e 7570 6172 616d 3a0a  in self.uparam:.
-000180c0: 2020 2020 2020 2020 2020 2020 6469 726e              dirn
-000180d0: 616d 6573 203d 2065 7863 6c75 6465 5f64  ames = exclude_d
-000180e0: 6f74 6669 6c65 7328 6469 726e 616d 6573  otfiles(dirnames
-000180f0: 290a 0a20 2020 2020 2020 2066 6f72 2066  )..        for f
-00018100: 6e20 696e 205b 7820 666f 7220 7820 696e  n in [x for x in
-00018110: 2064 6972 6e61 6d65 7320 6966 2078 2021   dirnames if x !
-00018120: 3d20 6578 636c 5d3a 0a20 2020 2020 2020  = excl]:.       
-00018130: 2020 2020 2064 6972 732e 6170 7065 6e64       dirs.append
-00018140: 2871 756f 7465 7028 666e 2929 0a0a 2020  (quotep(fn))..  
-00018150: 2020 2020 2020 666f 7220 7820 696e 2076        for x in v
-00018160: 6673 5f76 6972 743a 0a20 2020 2020 2020  fs_virt:.       
-00018170: 2020 2020 2069 6620 7820 213d 2065 7863       if x != exc
-00018180: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
-00018190: 2020 2064 6972 732e 6170 7065 6e64 2878     dirs.append(x
-000181a0: 290a 0a20 2020 2020 2020 2072 6574 5b22  )..        ret["
-000181b0: 6122 5d20 3d20 6469 7273 0a20 2020 2020  a"] = dirs.     
-000181c0: 2020 2072 6574 7572 6e20 7265 740a 0a20     return ret.. 
-000181d0: 2020 2064 6566 2074 785f 7570 7328 7365     def tx_ups(se
-000181e0: 6c66 2920 203a 0a20 2020 2020 2020 2069  lf)  :.        i
-000181f0: 6620 6e6f 7420 7365 6c66 2e61 7267 732e  f not self.args.
-00018200: 756e 706f 7374 3a0a 2020 2020 2020 2020  unpost:.        
-00018210: 2020 2020 7261 6973 6520 5065 626b 6163      raise Pebkac
-00018220: 2834 3033 2c20 2274 6865 2075 6e70 6f73  (403, "the unpos
-00018230: 7420 6665 6174 7572 6520 6973 2064 6973  t feature is dis
-00018240: 6162 6c65 6420 696e 2073 6572 7665 7220  abled in server 
-00018250: 636f 6e66 6967 2229 0a0a 2020 2020 2020  config")..      
-00018260: 2020 6964 7820 3d20 7365 6c66 2e63 6f6e    idx = self.con
-00018270: 6e2e 6765 745f 7532 6964 7828 290a 2020  n.get_u2idx().  
-00018280: 2020 2020 2020 6966 206e 6f74 2068 6173        if not has
-00018290: 6174 7472 2869 6478 2c20 2270 5f65 6e64  attr(idx, "p_end
-000182a0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000182b0: 7261 6973 6520 5065 626b 6163 2835 3030  raise Pebkac(500
-000182c0: 2c20 2273 716c 6974 6533 2069 7320 6e6f  , "sqlite3 is no
-000182d0: 7420 6176 6169 6c61 626c 6520 6f6e 2074  t available on t
-000182e0: 6865 2073 6572 7665 723b 2063 616e 6e6f  he server; canno
-000182f0: 7420 756e 706f 7374 2229 0a0a 2020 2020  t unpost")..    
-00018300: 2020 2020 6669 6c74 203d 2073 656c 662e      filt = self.
-00018310: 7570 6172 616d 2e67 6574 2822 6669 6c74  uparam.get("filt
-00018320: 6572 2229 0a20 2020 2020 2020 2066 696c  er").        fil
-00018330: 7420 3d20 756e 7175 6f74 6570 2866 696c  t = unquotep(fil
-00018340: 7420 6f72 2022 2229 0a20 2020 2020 2020  t or "").       
-00018350: 206c 6d20 3d20 2275 7073 205b 7b7d 5d22   lm = "ups [{}]"
-00018360: 2e66 6f72 6d61 7428 6669 6c74 290a 2020  .format(filt).  
-00018370: 2020 2020 2020 7365 6c66 2e6c 6f67 286c        self.log(l
-00018380: 6d29 0a0a 2020 2020 2020 2020 7265 7420  m)..        ret 
-00018390: 2020 3d20 5b5d 0a20 2020 2020 2020 2074    = [].        t
-000183a0: 3020 3d20 7469 6d65 2e74 696d 6528 290a  0 = time.time().
-000183b0: 2020 2020 2020 2020 6c69 6d20 3d20 7469          lim = ti
-000183c0: 6d65 2e74 696d 6528 2920 2d20 7365 6c66  me.time() - self
-000183d0: 2e61 7267 732e 756e 706f 7374 0a20 2020  .args.unpost.   
-000183e0: 2020 2020 2066 6b5f 766f 6c73 203d 207b       fk_vols = {
-000183f0: 0a20 2020 2020 2020 2020 2020 2076 6f6c  .            vol
-00018400: 3a20 766f 6c2e 666c 6167 735b 2266 6b22  : vol.flags["fk"
-00018410: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00018420: 7220 7670 2c20 766f 6c20 696e 2073 656c  r vp, vol in sel
-00018430: 662e 6173 7276 2e76 6673 2e61 6c6c 5f76  f.asrv.vfs.all_v
-00018440: 6f6c 732e 6974 656d 7328 290a 2020 2020  ols.items().    
-00018450: 2020 2020 2020 2020 6966 2022 666b 2220          if "fk" 
-00018460: 696e 2076 6f6c 2e66 6c61 6773 2061 6e64  in vol.flags and
-00018470: 2028 7670 2069 6e20 7365 6c66 2e72 766f   (vp in self.rvo
-00018480: 6c20 6f72 2076 7020 696e 2073 656c 662e  l or vp in self.
-00018490: 7570 766f 6c29 0a20 2020 2020 2020 207d  upvol).        }
-000184a0: 0a20 2020 2020 2020 2066 6f72 2076 6f6c  .        for vol
-000184b0: 2069 6e20 7365 6c66 2e61 7372 762e 7666   in self.asrv.vf
-000184c0: 732e 616c 6c5f 766f 6c73 2e76 616c 7565  s.all_vols.value
-000184d0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-000184e0: 2063 7572 203d 2069 6478 2e67 6574 5f63   cur = idx.get_c
-000184f0: 7572 2876 6f6c 2e72 6561 6c70 6174 6829  ur(vol.realpath)
-00018500: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00018510: 6e6f 7420 6375 723a 0a20 2020 2020 2020  not cur:.       
-00018520: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00018530: 650a 0a20 2020 2020 2020 2020 2020 206e  e..            n
-00018540: 666b 203d 2066 6b5f 766f 6c73 2e67 6574  fk = fk_vols.get
-00018550: 2876 6f6c 2c20 3029 0a0a 2020 2020 2020  (vol, 0)..      
-00018560: 2020 2020 2020 7120 3d20 2273 656c 6563        q = "selec
-00018570: 7420 737a 2c20 7264 2c20 666e 2c20 6174  t sz, rd, fn, at
-00018580: 2066 726f 6d20 7570 2077 6865 7265 2069   from up where i
-00018590: 703d 3f20 616e 6420 6174 3e3f 220a 2020  p=? and at>?".  
-000185a0: 2020 2020 2020 2020 2020 666f 7220 737a            for sz
-000185b0: 2c20 7264 2c20 666e 2c20 6174 2069 6e20  , rd, fn, at in 
-000185c0: 6375 722e 6578 6563 7574 6528 712c 2028  cur.execute(q, (
-000185d0: 7365 6c66 2e69 702c 206c 696d 2929 3a0a  self.ip, lim)):.
-000185e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185f0: 7670 203d 2022 2f22 202b 2022 2f22 2e6a  vp = "/" + "/".j
-00018600: 6f69 6e28 7820 666f 7220 7820 696e 205b  oin(x for x in [
-00018610: 766f 6c2e 7670 6174 682c 2072 642c 2066  vol.vpath, rd, f
-00018620: 6e5d 2069 6620 7829 0a20 2020 2020 2020  n] if x).       
-00018630: 2020 2020 2020 2020 2069 6620 6669 6c74           if filt
-00018640: 2061 6e64 2066 696c 7420 6e6f 7420 696e   and filt not in
-00018650: 2076 703a 0a20 2020 2020 2020 2020 2020   vp:.           
-00018660: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00018670: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
-00018680: 2020 2072 7620 3d20 7b22 7670 223a 2071     rv = {"vp": q
-00018690: 756f 7465 7028 7670 292c 2022 737a 223a  uotep(vp), "sz":
-000186a0: 2073 7a2c 2022 6174 223a 2061 742c 2022   sz, "at": at, "
-000186b0: 6e66 6b22 3a20 6e66 6b7d 0a20 2020 2020  nfk": nfk}.     
-000186c0: 2020 2020 2020 2020 2020 2069 6620 6e66             if nf
-000186d0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
-000186e0: 2020 2020 2020 2072 765b 2261 7022 5d20         rv["ap"] 
-000186f0: 3d20 766f 6c2e 6361 6e6f 6e69 6361 6c28  = vol.canonical(
-00018700: 766a 6f69 6e28 7264 2c20 666e 2929 0a0a  vjoin(rd, fn))..
+000142c0: 2020 2020 2020 6c6f 7765 7220 3d20 300a        lower = 0.
+000142d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000142e0: 2069 6620 622e 7374 7269 7028 293a 0a20   if b.strip():. 
+000142f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014300: 2020 2075 7070 6572 203d 2069 6e74 2862     upper = int(b
+00014310: 2e73 7472 6970 2829 2920 2b20 310a 2020  .strip()) + 1.  
+00014320: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00014330: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00014340: 2020 2020 2020 2020 7570 7065 7220 3d20          upper = 
+00014350: 6669 6c65 5f73 7a0a 0a20 2020 2020 2020  file_sz..       
+00014360: 2020 2020 2020 2020 2069 6620 7570 7065           if uppe
+00014370: 7220 3e20 6669 6c65 5f73 7a3a 0a20 2020  r > file_sz:.   
+00014380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014390: 2075 7070 6572 203d 2066 696c 655f 737a   upper = file_sz
+000143a0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000143b0: 2020 6966 206c 6f77 6572 203c 2030 206f    if lower < 0 o
+000143c0: 7220 6c6f 7765 7220 3e3d 2075 7070 6572  r lower >= upper
+000143d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000143e0: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+000143f0: 7074 696f 6e28 290a 0a20 2020 2020 2020  ption()..       
+00014400: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+00014410: 2020 2020 2020 2020 2020 2020 2065 7272               err
+00014420: 203d 2022 696e 7661 6c69 6420 7261 6e67   = "invalid rang
+00014430: 6520 287b 7d29 2c20 7369 7a65 3d7b 7d22  e ({}), size={}"
+00014440: 2e66 6f72 6d61 7428 6872 616e 6765 2c20  .format(hrange, 
+00014450: 6669 6c65 5f73 7a29 0a20 2020 2020 2020  file_sz).       
+00014460: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+00014470: 7564 5f72 6570 6c79 280a 2020 2020 2020  ud_reply(.      
+00014480: 2020 2020 2020 2020 2020 2020 2020 6572                er
+00014490: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+000144a0: 2020 2020 2020 2073 7461 7475 733d 3431         status=41
+000144b0: 362c 0a20 2020 2020 2020 2020 2020 2020  6,.             
+000144c0: 2020 2020 2020 2068 6561 6465 7273 3d7b         headers={
+000144d0: 2243 6f6e 7465 6e74 2d52 616e 6765 223a  "Content-Range":
+000144e0: 2022 6279 7465 7320 2a2f 7b7d 222e 666f   "bytes */{}".fo
+000144f0: 726d 6174 2866 696c 655f 737a 297d 2c0a  rmat(file_sz)},.
+00014500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014510: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014520: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+00014530: 2020 2020 2020 2020 2020 2073 7461 7475             statu
+00014540: 7320 3d20 3230 360a 2020 2020 2020 2020  s = 206.        
+00014550: 2020 2020 7365 6c66 2e6f 7574 5f68 6561      self.out_hea
+00014560: 6465 7273 5b22 436f 6e74 656e 742d 5261  ders["Content-Ra
+00014570: 6e67 6522 5d20 3d20 2262 7974 6573 207b  nge"] = "bytes {
+00014580: 7d2d 7b7d 2f7b 7d22 2e66 6f72 6d61 7428  }-{}/{}".format(
+00014590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000145a0: 206c 6f77 6572 2c20 7570 7065 7220 2d20   lower, upper - 
+000145b0: 312c 2066 696c 655f 737a 0a20 2020 2020  1, file_sz.     
+000145c0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000145d0: 2020 2020 2020 6c6f 6774 6169 6c20 2b3d        logtail +=
+000145e0: 2022 205b 5c30 3333 5b33 366d 7b7d 2d7b   " [\033[36m{}-{
+000145f0: 7d5c 3033 335b 306d 5d22 2e66 6f72 6d61  }\033[0m]".forma
+00014600: 7428 6c6f 7765 722c 2075 7070 6572 290a  t(lower, upper).
+00014610: 0a20 2020 2020 2020 2075 7365 5f73 656e  .        use_sen
+00014620: 6466 696c 6520 3d20 4661 6c73 650a 2020  dfile = False.  
+00014630: 2020 2020 2020 6966 2064 6563 6f6d 7072        if decompr
+00014640: 6573 733a 0a20 2020 2020 2020 2020 2020  ess:.           
+00014650: 206f 7065 6e5f 6675 6e63 2020 3d20 677a   open_func  = gz
+00014660: 6970 2e6f 7065 6e0a 2020 2020 2020 2020  ip.open.        
+00014670: 2020 2020 6f70 656e 5f61 7267 7320 203d      open_args  =
+00014680: 205b 6673 656e 6328 6673 5f70 6174 6829   [fsenc(fs_path)
+00014690: 2c20 2272 6222 5d0a 2020 2020 2020 2020  , "rb"].        
+000146a0: 2020 2020 2320 436f 6e74 656e 742d 4c65      # Content-Le
+000146b0: 6e67 7468 203a 3d20 6f72 6967 696e 616c  ngth := original
+000146c0: 2066 696c 6520 7369 7a65 0a20 2020 2020   file size.     
+000146d0: 2020 2020 2020 2075 7070 6572 203d 2067         upper = g
+000146e0: 7a69 705f 6f72 6967 5f73 7a28 6673 5f70  zip_orig_sz(fs_p
+000146f0: 6174 6829 0a20 2020 2020 2020 2065 6c73  ath).        els
+00014700: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+00014710: 7065 6e5f 6675 6e63 203d 206f 7065 6e0a  pen_func = open.
+00014720: 2020 2020 2020 2020 2020 2020 2320 3531              # 51
+00014730: 3220 6b42 2069 7320 6f70 7469 6d61 6c20  2 kB is optimal 
+00014740: 666f 7220 6875 6765 2066 696c 6573 2c20  for huge files, 
+00014750: 7573 6520 3634 6b0a 2020 2020 2020 2020  use 64k.        
+00014760: 2020 2020 6f70 656e 5f61 7267 7320 3d20      open_args = 
+00014770: 5b66 7365 6e63 2866 735f 7061 7468 292c  [fsenc(fs_path),
+00014780: 2022 7262 222c 2036 3420 2a20 3130 3234   "rb", 64 * 1024
+00014790: 5d0a 2020 2020 2020 2020 2020 2020 7573  ].            us
+000147a0: 655f 7365 6e64 6669 6c65 203d 2028 0a20  e_sendfile = (. 
+000147b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000147c0: 6f74 2073 656c 662e 746c 7320 2023 0a20  ot self.tls  #. 
+000147d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000147e0: 6e64 206e 6f74 2073 656c 662e 6172 6773  nd not self.args
+000147f0: 2e6e 6f5f 7365 6e64 6669 6c65 0a20 2020  .no_sendfile.   
+00014800: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00014810: 2068 6173 6174 7472 286f 732c 2022 7365   hasattr(os, "se
+00014820: 6e64 6669 6c65 2229 0a20 2020 2020 2020  ndfile").       
+00014830: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00014840: 230a 2020 2020 2020 2020 2320 7365 6e64  #.        # send
+00014850: 2072 6570 6c79 0a0a 2020 2020 2020 2020   reply..        
+00014860: 6966 2069 735f 636f 6d70 7265 7373 6564  if is_compressed
+00014870: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00014880: 6c66 2e6f 7574 5f68 6561 6465 7273 5b22  lf.out_headers["
+00014890: 4361 6368 652d 436f 6e74 726f 6c22 5d20  Cache-Control"] 
+000148a0: 3d20 226d 6178 2d61 6765 3d36 3034 3836  = "max-age=60486
+000148b0: 3922 0a20 2020 2020 2020 2065 6c73 653a  9".        else:
+000148c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000148d0: 662e 7065 726d 6974 5f63 6163 6869 6e67  f.permit_caching
+000148e0: 2829 0a0a 2020 2020 2020 2020 6966 2022  ()..        if "
+000148f0: 7478 7422 2069 6e20 7365 6c66 2e75 7061  txt" in self.upa
+00014900: 7261 6d3a 0a20 2020 2020 2020 2020 2020  ram:.           
+00014910: 206d 696d 6520 3d20 2274 6578 742f 706c   mime = "text/pl
+00014920: 6169 6e3b 2063 6861 7273 6574 3d7b 7d22  ain; charset={}"
+00014930: 2e66 6f72 6d61 7428 7365 6c66 2e75 7061  .format(self.upa
+00014940: 7261 6d5b 2274 7874 225d 206f 7220 2275  ram["txt"] or "u
+00014950: 7466 2d38 2229 0a20 2020 2020 2020 2065  tf-8").        e
+00014960: 6c69 6620 226d 696d 6522 2069 6e20 7365  lif "mime" in se
+00014970: 6c66 2e75 7061 7261 6d3a 0a20 2020 2020  lf.uparam:.     
+00014980: 2020 2020 2020 206d 696d 6520 3d20 7374         mime = st
+00014990: 7228 7365 6c66 2e75 7061 7261 6d2e 6765  r(self.uparam.ge
+000149a0: 7428 226d 696d 6522 2929 0a20 2020 2020  t("mime")).     
+000149b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000149c0: 2020 2020 206d 696d 6520 3d20 6775 6573       mime = gues
+000149d0: 735f 6d69 6d65 2872 6571 5f70 6174 6829  s_mime(req_path)
+000149e0: 0a0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
+000149f0: 7574 5f68 6561 6465 7273 5b22 4163 6365  ut_headers["Acce
+00014a00: 7074 2d52 616e 6765 7322 5d20 3d20 2262  pt-Ranges"] = "b
+00014a10: 7974 6573 220a 2020 2020 2020 2020 7365  ytes".        se
+00014a20: 6c66 2e73 656e 645f 6865 6164 6572 7328  lf.send_headers(
+00014a30: 6c65 6e67 7468 3d75 7070 6572 202d 206c  length=upper - l
+00014a40: 6f77 6572 2c20 7374 6174 7573 3d73 7461  ower, status=sta
+00014a50: 7475 732c 206d 696d 653d 6d69 6d65 290a  tus, mime=mime).
+00014a60: 0a20 2020 2020 2020 206c 6f67 6d73 6720  .        logmsg 
+00014a70: 2b3d 2075 6e69 636f 6465 2873 7461 7475  += unicode(statu
+00014a80: 7329 202b 206c 6f67 7461 696c 0a0a 2020  s) + logtail..  
+00014a90: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
+00014aa0: 6465 203d 3d20 2248 4541 4422 206f 7220  de == "HEAD" or 
+00014ab0: 6e6f 7420 646f 5f73 656e 643a 0a20 2020  not do_send:.   
+00014ac0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00014ad0: 2e64 6f5f 6c6f 673a 0a20 2020 2020 2020  .do_log:.       
+00014ae0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+00014af0: 6728 6c6f 676d 7367 290a 0a20 2020 2020  g(logmsg)..     
+00014b00: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00014b10: 7565 0a0a 2020 2020 2020 2020 7265 7420  ue..        ret 
+00014b20: 3d20 5472 7565 0a20 2020 2020 2020 2077  = True.        w
+00014b30: 6974 6820 6f70 656e 5f66 756e 6328 2a6f  ith open_func(*o
+00014b40: 7065 6e5f 6172 6773 2920 6173 2066 3a0a  pen_args) as f:.
+00014b50: 2020 2020 2020 2020 2020 2020 7365 6e64              send
+00014b60: 6675 6e20 3d20 7365 6e64 6669 6c65 5f6b  fun = sendfile_k
+00014b70: 6572 6e20 6966 2075 7365 5f73 656e 6466  ern if use_sendf
+00014b80: 696c 6520 656c 7365 2073 656e 6466 696c  ile else sendfil
+00014b90: 655f 7079 0a20 2020 2020 2020 2020 2020  e_py.           
+00014ba0: 2072 656d 6169 6e73 203d 2073 656e 6466   remains = sendf
+00014bb0: 756e 280a 2020 2020 2020 2020 2020 2020  un(.            
+00014bc0: 2020 2020 7365 6c66 2e6c 6f67 2c20 6c6f      self.log, lo
+00014bd0: 7765 722c 2075 7070 6572 2c20 662c 2073  wer, upper, f, s
+00014be0: 656c 662e 732c 2073 656c 662e 6172 6773  elf.s, self.args
+00014bf0: 2e73 5f77 725f 737a 2c20 7365 6c66 2e61  .s_wr_sz, self.a
+00014c00: 7267 732e 735f 7772 5f73 6c70 0a20 2020  rgs.s_wr_slp.   
+00014c10: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00014c20: 2020 2020 6966 2072 656d 6169 6e73 203e      if remains >
+00014c30: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00014c40: 6c6f 676d 7367 202b 3d20 2220 5c30 3333  logmsg += " \033
+00014c50: 5b33 316d 2220 2b20 756e 6963 6f64 6528  [31m" + unicode(
+00014c60: 7570 7065 7220 2d20 7265 6d61 696e 7329  upper - remains)
+00014c70: 202b 2022 5c30 3333 5b30 6d22 0a20 2020   + "\033[0m".   
+00014c80: 2020 2020 2020 2020 2073 656c 662e 6b65           self.ke
+00014c90: 6570 616c 6976 6520 3d20 4661 6c73 650a  epalive = False.
+00014ca0: 0a20 2020 2020 2020 2073 7064 203d 2073  .        spd = s
+00014cb0: 656c 662e 5f73 7064 2828 7570 7065 7220  elf._spd((upper 
+00014cc0: 2d20 6c6f 7765 7229 202d 2072 656d 6169  - lower) - remai
+00014cd0: 6e73 290a 2020 2020 2020 2020 6966 2073  ns).        if s
+00014ce0: 656c 662e 646f 5f6c 6f67 3a0a 2020 2020  elf.do_log:.    
+00014cf0: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+00014d00: 2822 7b7d 2c20 207b 7d22 2e66 6f72 6d61  ("{},  {}".forma
+00014d10: 7428 6c6f 676d 7367 2c20 7370 6429 290a  t(logmsg, spd)).
+00014d20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00014d30: 7265 740a 0a20 2020 2064 6566 2074 785f  ret..    def tx_
+00014d40: 7a69 7028 0a20 2020 2020 2020 2073 656c  zip(.        sel
+00014d50: 662c 2066 6d74 202c 2075 6172 6720 2c20  f, fmt , uarg , 
+00014d60: 766e 202c 2072 656d 202c 2069 7465 6d73  vn , rem , items
+00014d70: 202c 2064 6f74 7320 0a20 2020 2029 2020   , dots .    )  
+00014d80: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00014d90: 662e 6172 6773 2e6e 6f5f 7a69 703a 0a20  f.args.no_zip:. 
+00014da0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00014db0: 2050 6562 6b61 6328 3430 302c 2022 6e6f   Pebkac(400, "no
+00014dc0: 7420 656e 6162 6c65 6422 290a 0a20 2020  t enabled")..   
+00014dd0: 2020 2020 206c 6f67 6d73 6720 3d20 227b       logmsg = "{
+00014de0: 3a34 7d20 7b7d 2022 2e66 6f72 6d61 7428  :4} {} ".format(
+00014df0: 2222 2c20 7365 6c66 2e72 6571 290a 2020  "", self.req).  
+00014e00: 2020 2020 2020 7365 6c66 2e6b 6565 7061        self.keepa
+00014e10: 6c69 7665 203d 2046 616c 7365 0a0a 2020  live = False..  
+00014e20: 2020 2020 2020 6966 2066 6d74 203d 3d20        if fmt == 
+00014e30: 2274 6172 223a 0a20 2020 2020 2020 2020  "tar":.         
+00014e40: 2020 206d 696d 6520 3d20 2261 7070 6c69     mime = "appli
+00014e50: 6361 7469 6f6e 2f78 2d74 6172 220a 2020  cation/x-tar".  
+00014e60: 2020 2020 2020 2020 2020 7061 636b 6572            packer
+00014e70: 2020 3d20 5374 7265 616d 5461 720a 2020    = StreamTar.  
+00014e80: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00014e90: 2020 2020 2020 2020 6d69 6d65 203d 2022          mime = "
+00014ea0: 6170 706c 6963 6174 696f 6e2f 7a69 7022  application/zip"
+00014eb0: 0a20 2020 2020 2020 2020 2020 2070 6163  .            pac
+00014ec0: 6b65 7220 3d20 5374 7265 616d 5a69 700a  ker = StreamZip.
+00014ed0: 0a20 2020 2020 2020 2066 6e20 3d20 6974  .        fn = it
+00014ee0: 656d 735b 305d 2069 6620 6974 656d 7320  ems[0] if items 
+00014ef0: 616e 6420 6974 656d 735b 305d 2065 6c73  and items[0] els
+00014f00: 6520 7365 6c66 2e76 7061 7468 0a20 2020  e self.vpath.   
+00014f10: 2020 2020 2069 6620 666e 3a0a 2020 2020       if fn:.    
+00014f20: 2020 2020 2020 2020 666e 203d 2066 6e2e          fn = fn.
+00014f30: 7273 7472 6970 2822 2f22 292e 7370 6c69  rstrip("/").spli
+00014f40: 7428 222f 2229 5b2d 315d 0a20 2020 2020  t("/")[-1].     
+00014f50: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00014f60: 2020 2020 2066 6e20 3d20 7365 6c66 2e68       fn = self.h
+00014f70: 6f73 742e 7370 6c69 7428 223a 2229 5b30  ost.split(":")[0
+00014f80: 5d0a 0a20 2020 2020 2020 2073 6166 6520  ]..        safe 
+00014f90: 3d20 2873 7472 696e 672e 6173 6369 695f  = (string.ascii_
+00014fa0: 6c65 7474 6572 7320 2b20 7374 7269 6e67  letters + string
+00014fb0: 2e64 6967 6974 7329 2e72 6570 6c61 6365  .digits).replace
+00014fc0: 2822 2522 2c20 2222 290a 2020 2020 2020  ("%", "").      
+00014fd0: 2020 6166 6e20 3d20 2222 2e6a 6f69 6e28    afn = "".join(
+00014fe0: 5b78 2069 6620 7820 696e 2073 6166 652e  [x if x in safe.
+00014ff0: 7265 706c 6163 6528 2722 272c 2022 2229  replace('"', "")
+00015000: 2065 6c73 6520 225f 2220 666f 7220 7820   else "_" for x 
+00015010: 696e 2066 6e5d 290a 2020 2020 2020 2020  in fn]).        
+00015020: 6261 7363 6969 203d 2075 6e69 636f 6465  bascii = unicode
+00015030: 2873 6166 6529 2e65 6e63 6f64 6528 2275  (safe).encode("u
+00015040: 7466 2d38 2229 0a20 2020 2020 2020 207a  tf-8").        z
+00015050: 6220 3d20 666e 2e65 6e63 6f64 6528 2275  b = fn.encode("u
+00015060: 7466 2d38 222c 2022 786d 6c63 6861 7272  tf-8", "xmlcharr
+00015070: 6566 7265 706c 6163 6522 290a 2020 2020  efreplace").    
+00015080: 2020 2020 6966 206e 6f74 2050 5932 3a0a      if not PY2:.
+00015090: 2020 2020 2020 2020 2020 2020 7a62 6c20              zbl 
+000150a0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+000150b0: 2020 2020 6368 7228 7829 2e65 6e63 6f64      chr(x).encod
+000150c0: 6528 2275 7466 2d38 2229 0a20 2020 2020  e("utf-8").     
+000150d0: 2020 2020 2020 2020 2020 2069 6620 7820             if x 
+000150e0: 696e 2062 6173 6369 690a 2020 2020 2020  in bascii.      
+000150f0: 2020 2020 2020 2020 2020 656c 7365 2022            else "
+00015100: 257b 3a30 3278 7d22 2e66 6f72 6d61 7428  %{:02x}".format(
+00015110: 7829 2e65 6e63 6f64 6528 2261 7363 6969  x).encode("ascii
+00015120: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00015130: 2020 2066 6f72 2078 2069 6e20 7a62 0a20     for x in zb. 
+00015140: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00015150: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00015160: 2020 2020 2020 207a 626c 203d 205b 756e         zbl = [un
+00015170: 6963 6f64 6528 7829 2069 6620 7820 696e  icode(x) if x in
+00015180: 2062 6173 6369 6920 656c 7365 2022 257b   bascii else "%{
+00015190: 3a30 3278 7d22 2e66 6f72 6d61 7428 6f72  :02x}".format(or
+000151a0: 6428 7829 2920 666f 7220 7820 696e 207a  d(x)) for x in z
+000151b0: 625d 0a0a 2020 2020 2020 2020 7566 6e20  b]..        ufn 
+000151c0: 3d20 6222 222e 6a6f 696e 287a 626c 292e  = b"".join(zbl).
+000151d0: 6465 636f 6465 2822 6173 6369 6922 290a  decode("ascii").
+000151e0: 0a20 2020 2020 2020 2063 6469 7320 3d20  .        cdis = 
+000151f0: 2261 7474 6163 686d 656e 743b 2066 696c  "attachment; fil
+00015200: 656e 616d 653d 5c22 7b7d 2e7b 7d5c 223b  ename=\"{}.{}\";
+00015210: 2066 696c 656e 616d 652a 3d55 5446 2d38   filename*=UTF-8
+00015220: 2727 7b7d 2e7b 7d22 0a20 2020 2020 2020  ''{}.{}".       
+00015230: 2063 6469 7320 3d20 6364 6973 2e66 6f72   cdis = cdis.for
+00015240: 6d61 7428 6166 6e2c 2066 6d74 2c20 7566  mat(afn, fmt, uf
+00015250: 6e2c 2066 6d74 290a 2020 2020 2020 2020  n, fmt).        
+00015260: 7365 6c66 2e6c 6f67 2863 6469 7329 0a20  self.log(cdis). 
+00015270: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
+00015280: 5f68 6561 6465 7273 284e 6f6e 652c 206d  _headers(None, m
+00015290: 696d 653d 6d69 6d65 2c20 6865 6164 6572  ime=mime, header
+000152a0: 733d 7b22 436f 6e74 656e 742d 4469 7370  s={"Content-Disp
+000152b0: 6f73 6974 696f 6e22 3a20 6364 6973 7d29  osition": cdis})
+000152c0: 0a0a 2020 2020 2020 2020 6667 656e 203d  ..        fgen =
+000152d0: 2076 6e2e 7a69 7067 656e 280a 2020 2020   vn.zipgen(.    
+000152e0: 2020 2020 2020 2020 7265 6d2c 2073 6574          rem, set
+000152f0: 2869 7465 6d73 292c 2073 656c 662e 756e  (items), self.un
+00015300: 616d 652c 2046 616c 7365 2c20 646f 7473  ame, False, dots
+00015310: 2c20 6e6f 7420 7365 6c66 2e61 7267 732e  , not self.args.
+00015320: 6e6f 5f73 6361 6e64 6972 0a20 2020 2020  no_scandir.     
+00015330: 2020 2029 0a20 2020 2020 2020 2023 2066     ).        # f
+00015340: 6f72 2066 2069 6e20 6667 656e 3a20 7072  or f in fgen: pr
+00015350: 696e 7428 7265 7072 287b 6b3a 2066 5b6b  int(repr({k: f[k
+00015360: 5d20 666f 7220 6b20 696e 205b 2276 7022  ] for k in ["vp"
+00015370: 2c20 2261 7022 5d7d 2929 0a20 2020 2020  , "ap"]})).     
+00015380: 2020 2062 6765 6e20 3d20 7061 636b 6572     bgen = packer
+00015390: 2873 656c 662e 6c6f 672c 2066 6765 6e2c  (self.log, fgen,
+000153a0: 2075 7466 383d 2275 7466 2220 696e 2075   utf8="utf" in u
+000153b0: 6172 672c 2070 7265 5f63 7263 3d22 6372  arg, pre_crc="cr
+000153c0: 6322 2069 6e20 7561 7267 290a 2020 2020  c" in uarg).    
+000153d0: 2020 2020 6273 656e 7420 3d20 300a 2020      bsent = 0.  
+000153e0: 2020 2020 2020 666f 7220 6275 6620 696e        for buf in
+000153f0: 2062 6765 6e2e 6765 6e28 293a 0a20 2020   bgen.gen():.   
+00015400: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00015410: 6275 663a 0a20 2020 2020 2020 2020 2020  buf:.           
+00015420: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
+00015430: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00015440: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015450: 662e 732e 7365 6e64 616c 6c28 6275 6629  f.s.sendall(buf)
+00015460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015470: 2062 7365 6e74 202b 3d20 6c65 6e28 6275   bsent += len(bu
+00015480: 6629 0a20 2020 2020 2020 2020 2020 2065  f).            e
+00015490: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+000154a0: 2020 2020 2020 206c 6f67 6d73 6720 2b3d         logmsg +=
+000154b0: 2022 205c 3033 335b 3331 6d22 202b 2075   " \033[31m" + u
+000154c0: 6e69 636f 6465 2862 7365 6e74 2920 2b20  nicode(bsent) + 
+000154d0: 225c 3033 335b 306d 220a 2020 2020 2020  "\033[0m".      
+000154e0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+000154f0: 0a20 2020 2020 2020 2073 7064 203d 2073  .        spd = s
+00015500: 656c 662e 5f73 7064 2862 7365 6e74 290a  elf._spd(bsent).
+00015510: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+00015520: 2822 7b7d 2c20 207b 7d22 2e66 6f72 6d61  ("{},  {}".forma
+00015530: 7428 6c6f 676d 7367 2c20 7370 6429 290a  t(logmsg, spd)).
+00015540: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00015550: 7275 650a 0a20 2020 2064 6566 2074 785f  rue..    def tx_
+00015560: 6963 6f28 7365 6c66 2c20 6578 7420 2c20  ico(self, ext , 
+00015570: 6578 6163 7420 203d 2046 616c 7365 2920  exact  = False) 
+00015580: 203a 0a20 2020 2020 2020 2073 656c 662e   :.        self.
+00015590: 7065 726d 6974 5f63 6163 6869 6e67 2829  permit_caching()
+000155a0: 0a20 2020 2020 2020 2069 6620 6578 742e  .        if ext.
+000155b0: 656e 6473 7769 7468 2822 2f22 293a 0a20  endswith("/"):. 
+000155c0: 2020 2020 2020 2020 2020 2065 7874 203d             ext =
+000155d0: 2022 666f 6c64 6572 220a 2020 2020 2020   "folder".      
+000155e0: 2020 2020 2020 6578 6163 7420 3d20 5472        exact = Tr
+000155f0: 7565 0a0a 2020 2020 2020 2020 6261 6420  ue..        bad 
+00015600: 3d20 7265 2e63 6f6d 7069 6c65 2872 225b  = re.compile(r"[
+00015610: 5d28 297b 7d2f 205b 5d7c 5e5b 302d 395f  ](){}/ []|^[0-9_
+00015620: 2d5d 2a24 2229 0a20 2020 2020 2020 206e  -]*$").        n
+00015630: 203d 2065 7874 2e73 706c 6974 2822 2e22   = ext.split("."
+00015640: 295b 3a3a 2d31 5d0a 2020 2020 2020 2020  )[::-1].        
+00015650: 6966 206e 6f74 2065 7861 6374 3a0a 2020  if not exact:.  
+00015660: 2020 2020 2020 2020 2020 6e20 3d20 6e5b            n = n[
+00015670: 3a2d 315d 0a0a 2020 2020 2020 2020 6578  :-1]..        ex
+00015680: 7420 3d20 2222 0a20 2020 2020 2020 2066  t = "".        f
+00015690: 6f72 2076 2069 6e20 6e3a 0a20 2020 2020  or v in n:.     
+000156a0: 2020 2020 2020 2069 6620 6c65 6e28 7629         if len(v)
+000156b0: 203e 2037 206f 7220 6261 642e 7365 6172   > 7 or bad.sear
+000156c0: 6368 2876 293a 0a20 2020 2020 2020 2020  ch(v):.         
+000156d0: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+000156e0: 2020 2020 2020 2020 2020 6578 7420 3d20            ext = 
+000156f0: 227b 7d2e 7b7d 222e 666f 726d 6174 2876  "{}.{}".format(v
+00015700: 2c20 6578 7429 0a0a 2020 2020 2020 2020  , ext)..        
+00015710: 6578 7420 3d20 6578 742e 7273 7472 6970  ext = ext.rstrip
+00015720: 2822 2e22 2920 6f72 2022 756e 6b22 0a20  (".") or "unk". 
+00015730: 2020 2020 2020 2069 6620 6c65 6e28 6578         if len(ex
+00015740: 7429 203e 2031 313a 0a20 2020 2020 2020  t) > 11:.       
+00015750: 2020 2020 2065 7874 203d 2022 e28b af22       ext = "..."
+00015760: 202b 2065 7874 5b2d 393a 5d0a 0a20 2020   + ext[-9:]..   
+00015770: 2020 2020 2023 2063 6872 6f6d 6520 6361       # chrome ca
+00015780: 6e6e 6f74 2068 616e 646c 6520 6d6f 7265  nnot handle more
+00015790: 2074 6861 6e20 7e32 3030 3020 756e 6971   than ~2000 uniq
+000157a0: 7565 2053 5647 730a 2020 2020 2020 2020  ue SVGs.        
+000157b0: 6368 726f 6d65 203d 2022 2072 763a 2220  chrome = " rv:" 
+000157c0: 6e6f 7420 696e 2073 656c 662e 7561 0a20  not in self.ua. 
+000157d0: 2020 2020 2020 206d 696d 652c 2069 636f         mime, ico
+000157e0: 203d 2073 656c 662e 6963 6f2e 6765 7428   = self.ico.get(
+000157f0: 6578 742c 206e 6f74 2065 7861 6374 2c20  ext, not exact, 
+00015800: 6368 726f 6d65 290a 0a20 2020 2020 2020  chrome)..       
+00015810: 206c 6d20 3d20 666f 726d 6174 6461 7465   lm = formatdate
+00015820: 2873 656c 662e 452e 7430 2c20 7573 6567  (self.E.t0, useg
+00015830: 6d74 3d54 7275 6529 0a20 2020 2020 2020  mt=True).       
+00015840: 2073 656c 662e 7265 706c 7928 6963 6f2c   self.reply(ico,
+00015850: 206d 696d 653d 6d69 6d65 2c20 6865 6164   mime=mime, head
+00015860: 6572 733d 7b22 4c61 7374 2d4d 6f64 6966  ers={"Last-Modif
+00015870: 6965 6422 3a20 6c6d 7d29 0a20 2020 2020  ied": lm}).     
+00015880: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
+00015890: 2020 2020 6465 6620 7478 5f6d 6428 7365      def tx_md(se
+000158a0: 6c66 2c20 6673 5f70 6174 6820 2920 203a  lf, fs_path )  :
+000158b0: 0a20 2020 2020 2020 206c 6f67 6d73 6720  .        logmsg 
+000158c0: 3d20 227b 3a34 7d20 7b7d 2022 2e66 6f72  = "{:4} {} ".for
+000158d0: 6d61 7428 2222 2c20 7365 6c66 2e72 6571  mat("", self.req
+000158e0: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+000158f0: 7420 7365 6c66 2e63 616e 5f77 7269 7465  t self.can_write
+00015900: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00015910: 2022 6564 6974 2220 696e 2073 656c 662e   "edit" in self.
+00015920: 7570 6172 616d 206f 7220 2265 6469 7432  uparam or "edit2
+00015930: 2220 696e 2073 656c 662e 7570 6172 616d  " in self.uparam
+00015940: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015950: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
+00015960: 5f34 3034 2854 7275 6529 0a0a 2020 2020  _404(True)..    
+00015970: 2020 2020 7470 6c20 3d20 226d 6465 2220      tpl = "mde" 
+00015980: 6966 2022 6564 6974 3222 2069 6e20 7365  if "edit2" in se
+00015990: 6c66 2e75 7061 7261 6d20 656c 7365 2022  lf.uparam else "
+000159a0: 6d64 220a 2020 2020 2020 2020 6874 6d6c  md".        html
+000159b0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+000159c0: 6a6f 696e 2873 656c 662e 452e 6d6f 642c  join(self.E.mod,
+000159d0: 2022 7765 6222 2c20 227b 7d2e 6874 6d6c   "web", "{}.html
+000159e0: 222e 666f 726d 6174 2874 706c 2929 0a20  ".format(tpl)). 
+000159f0: 2020 2020 2020 2074 656d 706c 6174 6520         template 
+00015a00: 3d20 7365 6c66 2e6a 326a 2874 706c 290a  = self.j2j(tpl).
+00015a10: 0a20 2020 2020 2020 2073 7420 3d20 626f  .        st = bo
+00015a20: 732e 7374 6174 2866 735f 7061 7468 290a  s.stat(fs_path).
+00015a30: 2020 2020 2020 2020 7473 5f6d 6420 3d20          ts_md = 
+00015a40: 7374 2e73 745f 6d74 696d 650a 0a20 2020  st.st_mtime..   
+00015a50: 2020 2020 2073 7420 3d20 626f 732e 7374       st = bos.st
+00015a60: 6174 2868 746d 6c5f 7061 7468 290a 2020  at(html_path).  
+00015a70: 2020 2020 2020 7473 5f68 746d 6c20 3d20        ts_html = 
+00015a80: 7374 2e73 745f 6d74 696d 650a 0a20 2020  st.st_mtime..   
+00015a90: 2020 2020 2073 7a5f 6d64 203d 2030 0a20       sz_md = 0. 
+00015aa0: 2020 2020 2020 2066 6f72 2062 7566 2069         for buf i
+00015ab0: 6e20 7969 656c 6466 696c 6528 6673 5f70  n yieldfile(fs_p
+00015ac0: 6174 6829 3a0a 2020 2020 2020 2020 2020  ath):.          
+00015ad0: 2020 737a 5f6d 6420 2b3d 206c 656e 2862    sz_md += len(b
+00015ae0: 7566 290a 2020 2020 2020 2020 2020 2020  uf).            
+00015af0: 666f 7220 632c 2076 2069 6e20 5b28 6222  for c, v in [(b"
+00015b00: 2622 2c20 3429 2c20 2862 223c 222c 2033  &", 4), (b"<", 3
+00015b10: 292c 2028 6222 3e22 2c20 3329 5d3a 0a20  ), (b">", 3)]:. 
+00015b20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015b30: 7a5f 6d64 202b 3d20 286c 656e 2862 7566  z_md += (len(buf
+00015b40: 2920 2d20 6c65 6e28 6275 662e 7265 706c  ) - len(buf.repl
+00015b50: 6163 6528 632c 2062 2222 2929 2920 2a20  ace(c, b""))) * 
+00015b60: 760a 0a20 2020 2020 2020 2066 696c 655f  v..        file_
+00015b70: 7473 203d 2069 6e74 286d 6178 2874 735f  ts = int(max(ts_
+00015b80: 6d64 2c20 7473 5f68 746d 6c2c 2073 656c  md, ts_html, sel
+00015b90: 662e 452e 7430 2929 0a20 2020 2020 2020  f.E.t0)).       
+00015ba0: 2066 696c 655f 6c61 7374 6d6f 642c 2064   file_lastmod, d
+00015bb0: 6f5f 7365 6e64 203d 2073 656c 662e 5f63  o_send = self._c
+00015bc0: 686b 5f6c 6173 746d 6f64 2866 696c 655f  hk_lastmod(file_
+00015bd0: 7473 290a 2020 2020 2020 2020 7365 6c66  ts).        self
+00015be0: 2e6f 7574 5f68 6561 6465 7273 5b22 4c61  .out_headers["La
+00015bf0: 7374 2d4d 6f64 6966 6965 6422 5d20 3d20  st-Modified"] = 
+00015c00: 6669 6c65 5f6c 6173 746d 6f64 0a20 2020  file_lastmod.   
+00015c10: 2020 2020 2073 656c 662e 6f75 745f 6865       self.out_he
+00015c20: 6164 6572 732e 7570 6461 7465 284e 4f5f  aders.update(NO_
+00015c30: 4341 4348 4529 0a20 2020 2020 2020 2073  CACHE).        s
+00015c40: 7461 7475 7320 3d20 3230 3020 6966 2064  tatus = 200 if d
+00015c50: 6f5f 7365 6e64 2065 6c73 6520 3330 340a  o_send else 304.
+00015c60: 0a20 2020 2020 2020 2061 7267 5f62 6173  .        arg_bas
+00015c70: 6520 3d20 223f 220a 2020 2020 2020 2020  e = "?".        
+00015c80: 6966 2022 6b22 2069 6e20 7365 6c66 2e75  if "k" in self.u
+00015c90: 7061 7261 6d3a 0a20 2020 2020 2020 2020  param:.         
+00015ca0: 2020 2061 7267 5f62 6173 6520 3d20 223f     arg_base = "?
+00015cb0: 6b3d 7b7d 2622 2e66 6f72 6d61 7428 7365  k={}&".format(se
+00015cc0: 6c66 2e75 7061 7261 6d5b 226b 225d 290a  lf.uparam["k"]).
+00015cd0: 0a20 2020 2020 2020 2062 6f75 6e64 6172  .        boundar
+00015ce0: 7920 3d20 225c 726f 6c6c 5c74 6964 6522  y = "\roll\tide"
+00015cf0: 0a20 2020 2020 2020 2074 6172 6773 203d  .        targs =
+00015d00: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00015d10: 7222 3a20 7365 6c66 2e61 7267 732e 5352  r": self.args.SR
+00015d20: 2069 6620 7365 6c66 2e69 735f 7670 726f   if self.is_vpro
+00015d30: 7869 6564 2065 6c73 6520 2222 2c0a 2020  xied else "",.  
+00015d40: 2020 2020 2020 2020 2020 2274 7322 3a20            "ts": 
+00015d50: 7365 6c66 2e63 6f6e 6e2e 6873 7276 2e63  self.conn.hsrv.c
+00015d60: 6163 6865 6275 7374 6572 2829 2c0a 2020  achebuster(),.  
+00015d70: 2020 2020 2020 2020 2020 2273 7663 6e61            "svcna
+00015d80: 6d65 223a 2073 656c 662e 6172 6773 2e64  me": self.args.d
+00015d90: 6f63 7469 746c 652c 0a20 2020 2020 2020  octitle,.       
+00015da0: 2020 2020 2022 6874 6d6c 5f68 6561 6422       "html_head"
+00015db0: 3a20 7365 6c66 2e68 746d 6c5f 6865 6164  : self.html_head
+00015dc0: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00015dd0: 6469 7422 3a20 2265 6469 7422 2069 6e20  dit": "edit" in 
+00015de0: 7365 6c66 2e75 7061 7261 6d2c 0a20 2020  self.uparam,.   
+00015df0: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
+00015e00: 3a20 6874 6d6c 5f65 7363 6170 6528 7365  : html_escape(se
+00015e10: 6c66 2e76 7061 7468 2c20 6372 6c66 3d54  lf.vpath, crlf=T
+00015e20: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
+00015e30: 2020 226c 6173 746d 6f64 223a 2069 6e74    "lastmod": int
+00015e40: 2874 735f 6d64 202a 2031 3030 3029 2c0a  (ts_md * 1000),.
+00015e50: 2020 2020 2020 2020 2020 2020 226c 616e              "lan
+00015e60: 6722 3a20 7365 6c66 2e61 7267 732e 6c61  g": self.args.la
+00015e70: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
+00015e80: 2266 6176 6963 6f22 3a20 7365 6c66 2e61  "favico": self.a
+00015e90: 7267 732e 6661 7669 636f 2c0a 2020 2020  rgs.favico,.    
+00015ea0: 2020 2020 2020 2020 2268 6176 655f 656d          "have_em
+00015eb0: 7022 3a20 7365 6c66 2e61 7267 732e 656d  p": self.args.em
+00015ec0: 702c 0a20 2020 2020 2020 2020 2020 2022  p,.            "
+00015ed0: 6d64 5f63 686b 5f72 6174 6522 3a20 7365  md_chk_rate": se
+00015ee0: 6c66 2e61 7267 732e 6d63 722c 0a20 2020  lf.args.mcr,.   
+00015ef0: 2020 2020 2020 2020 2022 6d64 223a 2062           "md": b
+00015f00: 6f75 6e64 6172 792c 0a20 2020 2020 2020  oundary,.       
+00015f10: 2020 2020 2022 6172 675f 6261 7365 223a       "arg_base":
+00015f20: 2061 7267 5f62 6173 652c 0a20 2020 2020   arg_base,.     
+00015f30: 2020 207d 0a20 2020 2020 2020 207a 7320     }.        zs 
+00015f40: 3d20 7465 6d70 6c61 7465 2e72 656e 6465  = template.rende
+00015f50: 7228 2a2a 7461 7267 7329 2e65 6e63 6f64  r(**targs).encod
+00015f60: 6528 2275 7466 2d38 222c 2022 7265 706c  e("utf-8", "repl
+00015f70: 6163 6522 290a 2020 2020 2020 2020 6874  ace").        ht
+00015f80: 6d6c 203d 207a 732e 7370 6c69 7428 626f  ml = zs.split(bo
+00015f90: 756e 6461 7279 2e65 6e63 6f64 6528 2275  undary.encode("u
+00015fa0: 7466 2d38 2229 290a 2020 2020 2020 2020  tf-8")).        
+00015fb0: 6966 206c 656e 2868 746d 6c29 2021 3d20  if len(html) != 
+00015fc0: 323a 0a20 2020 2020 2020 2020 2020 2072  2:.            r
+00015fd0: 6169 7365 2045 7863 6570 7469 6f6e 2822  aise Exception("
+00015fe0: 626f 756e 6461 7279 2061 7070 6561 7273  boundary appears
+00015ff0: 2069 6e20 2220 2b20 6874 6d6c 5f70 6174   in " + html_pat
+00016000: 6829 0a0a 2020 2020 2020 2020 7365 6c66  h)..        self
+00016010: 2e73 656e 645f 6865 6164 6572 7328 737a  .send_headers(sz
+00016020: 5f6d 6420 2b20 6c65 6e28 6874 6d6c 5b30  _md + len(html[0
+00016030: 5d29 202b 206c 656e 2868 746d 6c5b 315d  ]) + len(html[1]
+00016040: 292c 2073 7461 7475 7329 0a0a 2020 2020  ), status)..    
+00016050: 2020 2020 6c6f 676d 7367 202b 3d20 756e      logmsg += un
+00016060: 6963 6f64 6528 7374 6174 7573 290a 2020  icode(status).  
+00016070: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
+00016080: 6465 203d 3d20 2248 4541 4422 206f 7220  de == "HEAD" or 
+00016090: 6e6f 7420 646f 5f73 656e 643a 0a20 2020  not do_send:.   
+000160a0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000160b0: 2e64 6f5f 6c6f 673a 0a20 2020 2020 2020  .do_log:.       
+000160c0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+000160d0: 6728 6c6f 676d 7367 290a 0a20 2020 2020  g(logmsg)..     
+000160e0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000160f0: 7565 0a0a 2020 2020 2020 2020 7472 793a  ue..        try:
+00016100: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00016110: 662e 732e 7365 6e64 616c 6c28 6874 6d6c  f.s.sendall(html
+00016120: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+00016130: 2066 6f72 2062 7566 2069 6e20 7969 656c   for buf in yiel
+00016140: 6466 696c 6528 6673 5f70 6174 6829 3a0a  dfile(fs_path):.
+00016150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016160: 7365 6c66 2e73 2e73 656e 6461 6c6c 2868  self.s.sendall(h
+00016170: 746d 6c5f 6265 7363 6170 6528 6275 6629  tml_bescape(buf)
+00016180: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00016190: 656c 662e 732e 7365 6e64 616c 6c28 6874  elf.s.sendall(ht
+000161a0: 6d6c 5b31 5d29 0a0a 2020 2020 2020 2020  ml[1])..        
+000161b0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+000161c0: 2020 2020 7365 6c66 2e6c 6f67 286c 6f67      self.log(log
+000161d0: 6d73 6720 2b20 2220 5c30 3333 5b33 316d  msg + " \033[31m
+000161e0: 642f 635c 3033 335b 306d 2229 0a20 2020  d/c\033[0m").   
+000161f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00016200: 4661 6c73 650a 0a20 2020 2020 2020 2069  False..        i
+00016210: 6620 7365 6c66 2e64 6f5f 6c6f 673a 0a20  f self.do_log:. 
+00016220: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016230: 6c6f 6728 6c6f 676d 7367 202b 2022 2022  log(logmsg + " "
+00016240: 202b 2075 6e69 636f 6465 286c 656e 2868   + unicode(len(h
+00016250: 746d 6c29 2929 0a0a 2020 2020 2020 2020  tml)))..        
+00016260: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+00016270: 2064 6566 2074 785f 7376 6373 2873 656c   def tx_svcs(sel
+00016280: 6629 2020 3a0a 2020 2020 2020 2020 616e  f)  :.        an
+00016290: 616d 6520 3d20 7265 2e73 7562 2822 5b5e  ame = re.sub("[^
+000162a0: 302d 3961 2d7a 412d 5a5d 2b22 2c20 2222  0-9a-zA-Z]+", ""
+000162b0: 2c20 7365 6c66 2e61 7267 732e 6e61 6d65  , self.args.name
+000162c0: 2920 6f72 2022 6122 0a20 2020 2020 2020  ) or "a".       
+000162d0: 2065 7020 3d20 7365 6c66 2e68 6f73 740a   ep = self.host.
+000162e0: 2020 2020 2020 2020 686f 7374 203d 2065          host = e
+000162f0: 702e 7370 6c69 7428 223a 2229 5b30 5d0a  p.split(":")[0].
+00016300: 2020 2020 2020 2020 6870 6f72 7420 3d20          hport = 
+00016310: 6570 5b65 702e 6669 6e64 2822 3a22 2920  ep[ep.find(":") 
+00016320: 3a5d 2069 6620 223a 2220 696e 2065 7020  :] if ":" in ep 
+00016330: 656c 7365 2022 220a 2020 2020 2020 2020  else "".        
+00016340: 7269 7020 3d20 280a 2020 2020 2020 2020  rip = (.        
+00016350: 2020 2020 686f 7374 0a20 2020 2020 2020      host.       
+00016360: 2020 2020 2069 6620 7365 6c66 2e61 7267       if self.arg
+00016370: 732e 7263 6c6f 6e65 5f6d 646e 7320 6f72  s.rclone_mdns or
+00016380: 206e 6f74 2073 656c 662e 6172 6773 2e7a   not self.args.z
+00016390: 6d0a 2020 2020 2020 2020 2020 2020 656c  m.            el
+000163a0: 7365 2073 656c 662e 636f 6e6e 2e68 7372  se self.conn.hsr
+000163b0: 762e 6e6d 2e6d 6170 2873 656c 662e 6970  v.nm.map(self.ip
+000163c0: 2920 6f72 2068 6f73 740a 2020 2020 2020  ) or host.      
+000163d0: 2020 290a 2020 2020 2020 2020 7670 203d    ).        vp =
+000163e0: 2028 7365 6c66 2e75 7061 7261 6d5b 2268   (self.uparam["h
+000163f0: 6322 5d20 6f72 2022 2229 2e6c 7374 7269  c"] or "").lstri
+00016400: 7028 222f 2229 0a20 2020 2020 2020 2068  p("/").        h
+00016410: 746d 6c20 3d20 7365 6c66 2e6a 3273 280a  tml = self.j2s(.
+00016420: 2020 2020 2020 2020 2020 2020 2273 7663              "svc
+00016430: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00016440: 6172 6773 3d73 656c 662e 6172 6773 2c0a  args=self.args,.
+00016450: 2020 2020 2020 2020 2020 2020 6163 6373              accs
+00016460: 3d62 6f6f 6c28 7365 6c66 2e61 7372 762e  =bool(self.asrv.
+00016470: 6163 6374 292c 0a20 2020 2020 2020 2020  acct),.         
+00016480: 2020 2073 3d22 7322 2069 6620 7365 6c66     s="s" if self
+00016490: 2e69 735f 6874 7470 7320 656c 7365 2022  .is_https else "
+000164a0: 222c 0a20 2020 2020 2020 2020 2020 2072  ",.            r
+000164b0: 6970 3d72 6970 2c0a 2020 2020 2020 2020  ip=rip,.        
+000164c0: 2020 2020 6570 3d65 702c 0a20 2020 2020      ep=ep,.     
+000164d0: 2020 2020 2020 2076 703d 7670 2c0a 2020         vp=vp,.  
+000164e0: 2020 2020 2020 2020 2020 7276 703d 766a            rvp=vj
+000164f0: 6f69 6e28 7365 6c66 2e61 7267 732e 522c  oin(self.args.R,
+00016500: 2076 7029 2c0a 2020 2020 2020 2020 2020   vp),.          
+00016510: 2020 686f 7374 3d68 6f73 742c 0a20 2020    host=host,.   
+00016520: 2020 2020 2020 2020 2068 706f 7274 3d68           hport=h
+00016530: 706f 7274 2c0a 2020 2020 2020 2020 2020  port,.          
+00016540: 2020 616e 616d 653d 616e 616d 652c 0a20    aname=aname,. 
+00016550: 2020 2020 2020 2020 2020 2070 773d 7365             pw=se
+00016560: 6c66 2e70 7720 6f72 2022 7077 222c 0a20  lf.pw or "pw",. 
+00016570: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00016580: 2073 656c 662e 7265 706c 7928 6874 6d6c   self.reply(html
+00016590: 2e65 6e63 6f64 6528 2275 7466 2d38 2229  .encode("utf-8")
+000165a0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000165b0: 2054 7275 650a 0a20 2020 2064 6566 2074   True..    def t
+000165c0: 785f 6d6f 756e 7473 2873 656c 6629 2020  x_mounts(self)  
+000165d0: 3a0a 2020 2020 2020 2020 7375 6620 3d20  :.        suf = 
+000165e0: 7365 6c66 2e75 726c 7128 7b7d 2c20 5b22  self.urlq({}, ["
+000165f0: 6822 5d29 0a20 2020 2020 2020 2061 766f  h"]).        avo
+00016600: 6c20 3d20 5b78 2066 6f72 2078 2069 6e20  l = [x for x in 
+00016610: 7365 6c66 2e77 766f 6c20 6966 2078 2069  self.wvol if x i
+00016620: 6e20 7365 6c66 2e72 766f 6c5d 0a20 2020  n self.rvol].   
+00016630: 2020 2020 2072 766f 6c2c 2077 766f 6c2c       rvol, wvol,
+00016640: 2061 766f 6c20 3d20 5b0a 2020 2020 2020   avol = [.      
+00016650: 2020 2020 2020 5b28 222f 2220 2b20 7829        [("/" + x)
+00016660: 2e72 7374 7269 7028 222f 2229 202b 2022  .rstrip("/") + "
+00016670: 2f22 2066 6f72 2078 2069 6e20 795d 0a20  /" for x in y]. 
+00016680: 2020 2020 2020 2020 2020 2066 6f72 2079             for y
+00016690: 2069 6e20 5b73 656c 662e 7276 6f6c 2c20   in [self.rvol, 
+000166a0: 7365 6c66 2e77 766f 6c2c 2061 766f 6c5d  self.wvol, avol]
+000166b0: 0a20 2020 2020 2020 205d 0a0a 2020 2020  .        ]..    
+000166c0: 2020 2020 6966 2061 766f 6c20 616e 6420      if avol and 
+000166d0: 6e6f 7420 7365 6c66 2e61 7267 732e 6e6f  not self.args.no
+000166e0: 5f72 6573 6361 6e3a 0a20 2020 2020 2020  _rescan:.       
+000166f0: 2020 2020 2078 203d 2073 656c 662e 636f       x = self.co
+00016700: 6e6e 2e68 7372 762e 6272 6f6b 6572 2e61  nn.hsrv.broker.a
+00016710: 736b 2822 7570 326b 2e67 6574 5f73 7461  sk("up2k.get_sta
+00016720: 7465 2229 0a20 2020 2020 2020 2020 2020  te").           
+00016730: 2076 7320 3d20 6a73 6f6e 2e6c 6f61 6473   vs = json.loads
+00016740: 2878 2e67 6574 2829 290a 2020 2020 2020  (x.get()).      
+00016750: 2020 2020 2020 7673 7461 7465 203d 207b        vstate = {
+00016760: 2822 2f22 202b 206b 292e 7273 7472 6970  ("/" + k).rstrip
+00016770: 2822 2f22 2920 2b20 222f 223a 2076 2066  ("/") + "/": v f
+00016780: 6f72 206b 2c20 7620 696e 2076 735b 2276  or k, v in vs["v
+00016790: 6f6c 7374 6174 6522 5d2e 6974 656d 7328  olstate"].items(
+000167a0: 297d 0a20 2020 2020 2020 2065 6c73 653a  )}.        else:
+000167b0: 0a20 2020 2020 2020 2020 2020 2076 7374  .            vst
+000167c0: 6174 6520 3d20 7b7d 0a20 2020 2020 2020  ate = {}.       
+000167d0: 2020 2020 2076 7320 3d20 7b0a 2020 2020       vs = {.    
+000167e0: 2020 2020 2020 2020 2020 2020 2273 6361              "sca
+000167f0: 6e6e 696e 6722 3a20 4e6f 6e65 2c0a 2020  nning": None,.  
+00016800: 2020 2020 2020 2020 2020 2020 2020 2268                "h
+00016810: 6173 6871 223a 204e 6f6e 652c 0a20 2020  ashq": None,.   
+00016820: 2020 2020 2020 2020 2020 2020 2022 7461               "ta
+00016830: 6771 223a 204e 6f6e 652c 0a20 2020 2020  gq": None,.     
+00016840: 2020 2020 2020 2020 2020 2022 6d74 7071             "mtpq
+00016850: 223a 204e 6f6e 652c 0a20 2020 2020 2020  ": None,.       
+00016860: 2020 2020 2020 2020 2022 6462 7774 223a           "dbwt":
+00016870: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00016880: 2020 207d 0a0a 2020 2020 2020 2020 666d     }..        fm
+00016890: 7420 3d20 7365 6c66 2e75 7061 7261 6d2e  t = self.uparam.
+000168a0: 6765 7428 226c 7322 2c20 2222 290a 2020  get("ls", "").  
+000168b0: 2020 2020 2020 6966 206e 6f74 2066 6d74        if not fmt
+000168c0: 2061 6e64 2028 7365 6c66 2e75 612e 7374   and (self.ua.st
+000168d0: 6172 7473 7769 7468 2822 6375 726c 2f22  artswith("curl/"
+000168e0: 2920 6f72 2073 656c 662e 7561 2e73 7461  ) or self.ua.sta
+000168f0: 7274 7377 6974 6828 2266 6574 6368 2229  rtswith("fetch")
+00016900: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+00016910: 6d74 203d 2022 7622 0a0a 2020 2020 2020  mt = "v"..      
+00016920: 2020 6966 2066 6d74 2069 6e20 5b22 7622    if fmt in ["v"
+00016930: 2c20 2274 222c 2022 7478 7422 5d3a 0a20  , "t", "txt"]:. 
+00016940: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00016950: 6c66 2e75 6e61 6d65 203d 3d20 222a 223a  lf.uname == "*":
+00016960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016970: 2074 7874 203d 2022 686f 7764 7920 7374   txt = "howdy st
+00016980: 7261 6e67 6572 2028 796f 7527 7265 206e  ranger (you're n
+00016990: 6f74 206c 6f67 6765 6420 696e 2922 0a20  ot logged in)". 
+000169a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000169b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000169c0: 2074 7874 203d 2022 7765 6c63 6f6d 6520   txt = "welcome 
+000169d0: 6261 636b 207b 7d22 2e66 6f72 6d61 7428  back {}".format(
+000169e0: 7365 6c66 2e75 6e61 6d65 290a 0a20 2020  self.uname)..   
+000169f0: 2020 2020 2020 2020 2069 6620 7673 7461           if vsta
+00016a00: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
+00016a10: 2020 2020 7478 7420 2b3d 2022 5c6e 7374      txt += "\nst
+00016a20: 6174 7573 3a22 0a20 2020 2020 2020 2020  atus:".         
+00016a30: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00016a40: 5b22 7363 616e 6e69 6e67 222c 2022 6861  ["scanning", "ha
+00016a50: 7368 7122 2c20 2274 6167 7122 2c20 226d  shq", "tagq", "m
+00016a60: 7470 7122 2c20 2264 6277 7422 5d3a 0a20  tpq", "dbwt"]:. 
+00016a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a80: 2020 2074 7874 202b 3d20 2220 7b7d 287b     txt += " {}({
+00016a90: 7d29 222e 666f 726d 6174 286b 2c20 7673  })".format(k, vs
+00016aa0: 5b6b 5d29 0a0a 2020 2020 2020 2020 2020  [k])..          
+00016ab0: 2020 6966 2072 766f 6c3a 0a20 2020 2020    if rvol:.     
+00016ac0: 2020 2020 2020 2020 2020 2074 7874 202b             txt +
+00016ad0: 3d20 225c 6e79 6f75 2063 616e 2062 726f  = "\nyou can bro
+00016ae0: 7773 653a 220a 2020 2020 2020 2020 2020  wse:".          
+00016af0: 2020 2020 2020 666f 7220 7620 696e 2072        for v in r
+00016b00: 766f 6c3a 0a20 2020 2020 2020 2020 2020  vol:.           
+00016b10: 2020 2020 2020 2020 2074 7874 202b 3d20           txt += 
+00016b20: 225c 6e20 2022 202b 2076 0a0a 2020 2020  "\n  " + v..    
+00016b30: 2020 2020 2020 2020 6966 2077 766f 6c3a          if wvol:
+00016b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016b50: 2074 7874 202b 3d20 225c 6e79 6f75 2063   txt += "\nyou c
+00016b60: 616e 2075 706c 6f61 6420 746f 3a22 0a20  an upload to:". 
+00016b70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00016b80: 6f72 2076 2069 6e20 7776 6f6c 3a0a 2020  or v in wvol:.  
+00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ba0: 2020 7478 7420 2b3d 2022 5c6e 2020 2220    txt += "\n  " 
+00016bb0: 2b20 760a 0a20 2020 2020 2020 2020 2020  + v..           
+00016bc0: 207a 6220 3d20 7478 742e 656e 636f 6465   zb = txt.encode
+00016bd0: 2822 7574 662d 3822 2c20 2272 6570 6c61  ("utf-8", "repla
+00016be0: 6365 2229 202b 2062 225c 6e22 0a20 2020  ce") + b"\n".   
+00016bf0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00016c00: 706c 7928 7a62 2c20 6d69 6d65 3d22 7465  ply(zb, mime="te
+00016c10: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
+00016c20: 743d 7574 662d 3822 290a 2020 2020 2020  t=utf-8").      
+00016c30: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00016c40: 650a 0a20 2020 2020 2020 2068 746d 6c20  e..        html 
+00016c50: 3d20 7365 6c66 2e6a 3273 280a 2020 2020  = self.j2s(.    
+00016c60: 2020 2020 2020 2020 2273 706c 6173 6822          "splash"
+00016c70: 2c0a 2020 2020 2020 2020 2020 2020 7468  ,.            th
+00016c80: 6973 3d73 656c 662c 0a20 2020 2020 2020  is=self,.       
+00016c90: 2020 2020 2071 7670 6174 683d 7175 6f74       qvpath=quot
+00016ca0: 6570 2873 656c 662e 7670 6174 6829 2c0a  ep(self.vpath),.
+00016cb0: 2020 2020 2020 2020 2020 2020 7276 6f6c              rvol
+00016cc0: 3d72 766f 6c2c 0a20 2020 2020 2020 2020  =rvol,.         
+00016cd0: 2020 2077 766f 6c3d 7776 6f6c 2c0a 2020     wvol=wvol,.  
+00016ce0: 2020 2020 2020 2020 2020 6176 6f6c 3d61            avol=a
+00016cf0: 766f 6c2c 0a20 2020 2020 2020 2020 2020  vol,.           
+00016d00: 2076 7374 6174 653d 7673 7461 7465 2c0a   vstate=vstate,.
+00016d10: 2020 2020 2020 2020 2020 2020 7363 616e              scan
+00016d20: 6e69 6e67 3d76 735b 2273 6361 6e6e 696e  ning=vs["scannin
+00016d30: 6722 5d2c 0a20 2020 2020 2020 2020 2020  g"],.           
+00016d40: 2068 6173 6871 3d76 735b 2268 6173 6871   hashq=vs["hashq
+00016d50: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+00016d60: 7461 6771 3d76 735b 2274 6167 7122 5d2c  tagq=vs["tagq"],
+00016d70: 0a20 2020 2020 2020 2020 2020 206d 7470  .            mtp
+00016d80: 713d 7673 5b22 6d74 7071 225d 2c0a 2020  q=vs["mtpq"],.  
+00016d90: 2020 2020 2020 2020 2020 6462 7774 3d76            dbwt=v
+00016da0: 735b 2264 6277 7422 5d2c 0a20 2020 2020  s["dbwt"],.     
+00016db0: 2020 2020 2020 2075 726c 5f73 7566 3d73         url_suf=s
+00016dc0: 7566 2c0a 2020 2020 2020 2020 2020 2020  uf,.            
+00016dd0: 6b33 3034 3d73 656c 662e 6b33 3034 2829  k304=self.k304()
+00016de0: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+00016df0: 723d 535f 5645 5253 494f 4e20 6966 2073  r=S_VERSION if s
+00016e00: 656c 662e 6172 6773 2e76 6572 2065 6c73  elf.args.ver els
+00016e10: 6520 2222 2c0a 2020 2020 2020 2020 2020  e "",.          
+00016e20: 2020 6168 7474 7073 3d22 2220 6966 2073    ahttps="" if s
+00016e30: 656c 662e 6973 5f68 7474 7073 2065 6c73  elf.is_https els
+00016e40: 6520 2268 7474 7073 3a2f 2f22 202b 2073  e "https://" + s
+00016e50: 656c 662e 686f 7374 202b 2073 656c 662e  elf.host + self.
+00016e60: 7265 712c 0a20 2020 2020 2020 2029 0a20  req,.        ). 
+00016e70: 2020 2020 2020 2073 656c 662e 7265 706c         self.repl
+00016e80: 7928 6874 6d6c 2e65 6e63 6f64 6528 2275  y(html.encode("u
+00016e90: 7466 2d38 2229 290a 2020 2020 2020 2020  tf-8")).        
+00016ea0: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+00016eb0: 2064 6566 2073 6574 5f6b 3330 3428 7365   def set_k304(se
+00016ec0: 6c66 2920 203a 0a20 2020 2020 2020 2063  lf)  :.        c
+00016ed0: 6b20 3d20 6765 6e63 6f6f 6b69 6528 226b  k = gencookie("k
+00016ee0: 3330 3422 2c20 7365 6c66 2e75 7061 7261  304", self.upara
+00016ef0: 6d5b 226b 3330 3422 5d2c 2073 656c 662e  m["k304"], self.
+00016f00: 6172 6773 2e52 2c20 4661 6c73 652c 2038  args.R, False, 8
+00016f10: 3634 3030 202a 2032 3939 290a 2020 2020  6400 * 299).    
+00016f20: 2020 2020 7365 6c66 2e6f 7574 5f68 6561      self.out_hea
+00016f30: 6465 726c 6973 742e 6170 7065 6e64 2828  derlist.append((
+00016f40: 2253 6574 2d43 6f6f 6b69 6522 2c20 636b  "Set-Cookie", ck
+00016f50: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00016f60: 7265 6469 7265 6374 2822 222c 2022 3f68  redirect("", "?h
+00016f70: 2363 6322 290a 2020 2020 2020 2020 7265  #cc").        re
+00016f80: 7475 726e 2054 7275 650a 0a20 2020 2064  turn True..    d
+00016f90: 6566 2073 6574 636b 2873 656c 6629 2020  ef setck(self)  
+00016fa0: 3a0a 2020 2020 2020 2020 6b2c 2076 203d  :.        k, v =
+00016fb0: 2073 656c 662e 7570 6172 616d 5b22 7365   self.uparam["se
+00016fc0: 7463 6b22 5d2e 7370 6c69 7428 223d 222c  tck"].split("=",
+00016fd0: 2031 290a 2020 2020 2020 2020 7420 3d20   1).        t = 
+00016fe0: 4e6f 6e65 2069 6620 7620 3d3d 2022 2220  None if v == "" 
+00016ff0: 656c 7365 2038 3634 3030 202a 2032 3939  else 86400 * 299
+00017000: 0a20 2020 2020 2020 2063 6b20 3d20 6765  .        ck = ge
+00017010: 6e63 6f6f 6b69 6528 6b2c 2076 2c20 7365  ncookie(k, v, se
+00017020: 6c66 2e61 7267 732e 522c 2046 616c 7365  lf.args.R, False
+00017030: 2c20 7429 0a20 2020 2020 2020 2073 656c  , t).        sel
+00017040: 662e 6f75 745f 6865 6164 6572 6c69 7374  f.out_headerlist
+00017050: 2e61 7070 656e 6428 2822 5365 742d 436f  .append(("Set-Co
+00017060: 6f6b 6965 222c 2063 6b29 290a 2020 2020  okie", ck)).    
+00017070: 2020 2020 7365 6c66 2e72 6570 6c79 2862      self.reply(b
+00017080: 226f 375c 6e22 290a 2020 2020 2020 2020  "o7\n").        
+00017090: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+000170a0: 2064 6566 2073 6574 5f63 6667 5f72 6573   def set_cfg_res
+000170b0: 6574 2873 656c 6629 2020 3a0a 2020 2020  et(self)  :.    
+000170c0: 2020 2020 666f 7220 6b20 696e 2028 226b      for k in ("k
+000170d0: 3330 3422 2c20 226a 7322 2c20 2269 6478  304", "js", "idx
+000170e0: 6822 2c20 2263 7070 7764 222c 2022 6370  h", "cppwd", "cp
+000170f0: 7077 7322 293a 0a20 2020 2020 2020 2020  pws"):.         
+00017100: 2020 2063 6f6f 6b69 6520 3d20 6765 6e63     cookie = genc
+00017110: 6f6f 6b69 6528 6b2c 2022 7822 2c20 7365  ookie(k, "x", se
+00017120: 6c66 2e61 7267 732e 522c 2046 616c 7365  lf.args.R, False
+00017130: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
+00017140: 2020 2020 7365 6c66 2e6f 7574 5f68 6561      self.out_hea
+00017150: 6465 726c 6973 742e 6170 7065 6e64 2828  derlist.append((
+00017160: 2253 6574 2d43 6f6f 6b69 6522 2c20 636f  "Set-Cookie", co
+00017170: 6f6b 6965 2929 0a0a 2020 2020 2020 2020  okie))..        
+00017180: 7365 6c66 2e72 6564 6972 6563 7428 2222  self.redirect(""
+00017190: 2c20 223f 6823 6363 2229 0a20 2020 2020  , "?h#cc").     
+000171a0: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
+000171b0: 2020 2020 6465 6620 7478 5f34 3034 2873      def tx_404(s
+000171c0: 656c 662c 2069 735f 3430 3320 203d 2046  elf, is_403  = F
+000171d0: 616c 7365 2920 203a 0a20 2020 2020 2020  alse)  :.       
+000171e0: 2072 6320 3d20 3430 340a 2020 2020 2020   rc = 404.      
+000171f0: 2020 6966 2073 656c 662e 6172 6773 2e76    if self.args.v
+00017200: 6167 7565 5f34 3033 3a0a 2020 2020 2020  ague_403:.      
+00017210: 2020 2020 2020 7420 3d20 273c 6831 2069        t = '<h1 i
+00017220: 643d 226e 223e 3430 3420 6e6f 7420 666f  d="n">404 not fo
+00017230: 756e 6420 266e 6273 703b e294 9028 20c2  und &nbsp;...( .
+00017240: b420 2d60 29e2 948c 3c2f 6831 3e3c 7020  . -`)...</h1><p 
+00017250: 6964 3d22 6f22 3e6f 7220 6d61 7962 6520  id="o">or maybe 
+00017260: 796f 7520 646f 6e5c 2774 2068 6176 6520  you don\'t have 
+00017270: 6163 6365 7373 202d 2d20 7472 7920 6c6f  access -- try lo
+00017280: 6767 696e 6720 696e 206f 7220 3c61 2068  gging in or <a h
+00017290: 7265 663d 227b 7d2f 3f68 223e 676f 2068  ref="{}/?h">go h
+000172a0: 6f6d 653c 2f61 3e3c 2f70 3e27 0a20 2020  ome</a></p>'.   
+000172b0: 2020 2020 2065 6c69 6620 6973 5f34 3033       elif is_403
+000172c0: 3a0a 2020 2020 2020 2020 2020 2020 7420  :.            t 
+000172d0: 3d20 273c 6831 2069 643d 2270 223e 3430  = '<h1 id="p">40
+000172e0: 3320 666f 7262 6964 6465 6e61 2026 6e62  3 forbiddena &nb
+000172f0: 7370 3b7e e294 bbe2 9481 e294 bb3c 2f68  sp;~.........</h
+00017300: 313e 3c70 2069 643d 2271 223e 796f 755c  1><p id="q">you\
+00017310: 276c 6c20 6861 7665 2074 6f20 6c6f 6720  'll have to log 
+00017320: 696e 206f 7220 3c61 2068 7265 663d 227b  in or <a href="{
+00017330: 7d2f 3f68 223e 676f 2068 6f6d 653c 2f61  }/?h">go home</a
+00017340: 3e3c 2f70 3e27 0a20 2020 2020 2020 2020  ></p>'.         
+00017350: 2020 2072 6320 3d20 3430 330a 2020 2020     rc = 403.    
+00017360: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00017370: 2020 2020 2020 7420 3d20 273c 6831 2069        t = '<h1 i
+00017380: 643d 226e 223e 3430 3420 6e6f 7420 666f  d="n">404 not fo
+00017390: 756e 6420 266e 6273 703b e294 9028 20c2  und &nbsp;...( .
+000173a0: b420 2d60 29e2 948c 3c2f 6831 3e3c 703e  . -`)...</h1><p>
+000173b0: 3c61 2069 643d 2272 2220 6872 6566 3d22  <a id="r" href="
+000173c0: 7b7d 2f3f 6822 3e67 6f20 686f 6d65 3c2f  {}/?h">go home</
+000173d0: 613e 3c2f 703e 270a 0a20 2020 2020 2020  a></p>'..       
+000173e0: 2074 203d 2074 2e66 6f72 6d61 7428 7365   t = t.format(se
+000173f0: 6c66 2e61 7267 732e 5352 290a 2020 2020  lf.args.SR).    
+00017400: 2020 2020 6874 6d6c 203d 2073 656c 662e      html = self.
+00017410: 6a32 7328 2273 706c 6173 6822 2c20 7468  j2s("splash", th
+00017420: 6973 3d73 656c 662c 2071 7670 6174 683d  is=self, qvpath=
+00017430: 7175 6f74 6570 2873 656c 662e 7670 6174  quotep(self.vpat
+00017440: 6829 2c20 6d73 673d 7429 0a20 2020 2020  h), msg=t).     
+00017450: 2020 2073 656c 662e 7265 706c 7928 6874     self.reply(ht
+00017460: 6d6c 2e65 6e63 6f64 6528 2275 7466 2d38  ml.encode("utf-8
+00017470: 2229 2c20 7374 6174 7573 3d72 6329 0a20  "), status=rc). 
+00017480: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00017490: 7565 0a0a 2020 2020 6465 6620 7363 616e  ue..    def scan
+000174a0: 766f 6c28 7365 6c66 2920 203a 0a20 2020  vol(self)  :.   
+000174b0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+000174c0: 2e63 616e 5f72 6561 6420 6f72 206e 6f74  .can_read or not
+000174d0: 2073 656c 662e 6361 6e5f 7772 6974 653a   self.can_write:
+000174e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000174f0: 7365 2050 6562 6b61 6328 3430 332c 2022  se Pebkac(403, "
+00017500: 6e6f 7420 616c 6c6f 7765 6420 666f 7220  not allowed for 
+00017510: 7573 6572 2022 202b 2073 656c 662e 756e  user " + self.un
+00017520: 616d 6529 0a0a 2020 2020 2020 2020 6966  ame)..        if
+00017530: 2073 656c 662e 6172 6773 2e6e 6f5f 7265   self.args.no_re
+00017540: 7363 616e 3a0a 2020 2020 2020 2020 2020  scan:.          
+00017550: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
+00017560: 3033 2c20 2274 6865 2072 6573 6361 6e20  03, "the rescan 
+00017570: 6665 6174 7572 6520 6973 2064 6973 6162  feature is disab
+00017580: 6c65 6420 696e 2073 6572 7665 7220 636f  led in server co
+00017590: 6e66 6967 2229 0a0a 2020 2020 2020 2020  nfig")..        
+000175a0: 766e 2c20 5f20 3d20 7365 6c66 2e61 7372  vn, _ = self.asr
+000175b0: 762e 7666 732e 6765 7428 7365 6c66 2e76  v.vfs.get(self.v
+000175c0: 7061 7468 2c20 7365 6c66 2e75 6e61 6d65  path, self.uname
+000175d0: 2c20 5472 7565 2c20 5472 7565 290a 0a20  , True, True).. 
+000175e0: 2020 2020 2020 2061 7267 7320 3d20 5b73         args = [s
+000175f0: 656c 662e 6173 7276 2e76 6673 2e61 6c6c  elf.asrv.vfs.all
+00017600: 5f76 6f6c 732c 205b 766e 2e76 7061 7468  _vols, [vn.vpath
+00017610: 5d2c 2046 616c 7365 2c20 5472 7565 5d0a  ], False, True].
+00017620: 0a20 2020 2020 2020 2078 203d 2073 656c  .        x = sel
+00017630: 662e 636f 6e6e 2e68 7372 762e 6272 6f6b  f.conn.hsrv.brok
+00017640: 6572 2e61 736b 2822 7570 326b 2e72 6573  er.ask("up2k.res
+00017650: 6361 6e22 2c20 2a61 7267 7329 0a20 2020  can", *args).   
+00017660: 2020 2020 2065 7272 203d 2078 2e67 6574       err = x.get
+00017670: 2829 0a20 2020 2020 2020 2069 6620 6e6f  ().        if no
+00017680: 7420 6572 723a 0a20 2020 2020 2020 2020  t err:.         
+00017690: 2020 2073 656c 662e 7265 6469 7265 6374     self.redirect
+000176a0: 2822 222c 2022 3f68 2229 0a20 2020 2020  ("", "?h").     
+000176b0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000176c0: 7565 0a0a 2020 2020 2020 2020 7261 6973  ue..        rais
+000176d0: 6520 5065 626b 6163 2835 3030 2c20 6572  e Pebkac(500, er
+000176e0: 7229 0a0a 2020 2020 6465 6620 6861 6e64  r)..    def hand
+000176f0: 6c65 5f72 656c 6f61 6428 7365 6c66 2920  le_reload(self) 
+00017700: 203a 0a20 2020 2020 2020 2061 6374 203d   :.        act =
+00017710: 2073 656c 662e 7570 6172 616d 2e67 6574   self.uparam.get
+00017720: 2822 7265 6c6f 6164 2229 0a20 2020 2020  ("reload").     
+00017730: 2020 2069 6620 6163 7420 213d 2022 6366     if act != "cf
+00017740: 6722 3a0a 2020 2020 2020 2020 2020 2020  g":.            
+00017750: 7261 6973 6520 5065 626b 6163 2834 3030  raise Pebkac(400
+00017760: 2c20 226f 6e6c 7920 636f 6e66 6967 2066  , "only config f
+00017770: 696c 6573 2028 2763 6667 2729 2063 616e  iles ('cfg') can
+00017780: 2062 6520 7265 6c6f 6164 6564 2072 6e22   be reloaded rn"
+00017790: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+000177a0: 7420 5b78 2066 6f72 2078 2069 6e20 7365  t [x for x in se
+000177b0: 6c66 2e77 766f 6c20 6966 2078 2069 6e20  lf.wvol if x in 
+000177c0: 7365 6c66 2e72 766f 6c5d 3a0a 2020 2020  self.rvol]:.    
+000177d0: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
+000177e0: 626b 6163 2834 3033 2c20 226e 6f74 2061  bkac(403, "not a
+000177f0: 6c6c 6f77 6564 2066 6f72 2075 7365 7220  llowed for user 
+00017800: 2220 2b20 7365 6c66 2e75 6e61 6d65 290a  " + self.uname).
+00017810: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00017820: 2e61 7267 732e 6e6f 5f72 656c 6f61 643a  .args.no_reload:
+00017830: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00017840: 7365 2050 6562 6b61 6328 3430 332c 2022  se Pebkac(403, "
+00017850: 7468 6520 7265 6c6f 6164 2066 6561 7475  the reload featu
+00017860: 7265 2069 7320 6469 7361 626c 6564 2069  re is disabled i
+00017870: 6e20 7365 7276 6572 2063 6f6e 6669 6722  n server config"
+00017880: 290a 0a20 2020 2020 2020 2078 203d 2073  )..        x = s
+00017890: 656c 662e 636f 6e6e 2e68 7372 762e 6272  elf.conn.hsrv.br
+000178a0: 6f6b 6572 2e61 736b 2822 7265 6c6f 6164  oker.ask("reload
+000178b0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+000178c0: 6e20 7365 6c66 2e72 6564 6972 6563 7428  n self.redirect(
+000178d0: 2222 2c20 223f 6822 2c20 782e 6765 7428  "", "?h", x.get(
+000178e0: 292c 2022 7265 7475 726e 2074 6f22 2c20  ), "return to", 
+000178f0: 4661 6c73 6529 0a0a 2020 2020 6465 6620  False)..    def 
+00017900: 7478 5f73 7461 636b 2873 656c 6629 2020  tx_stack(self)  
+00017910: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00017920: 205b 7820 666f 7220 7820 696e 2073 656c   [x for x in sel
+00017930: 662e 7776 6f6c 2069 6620 7820 696e 2073  f.wvol if x in s
+00017940: 656c 662e 7276 6f6c 5d3a 0a20 2020 2020  elf.rvol]:.     
+00017950: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
+00017960: 6b61 6328 3430 332c 2022 6e6f 7420 616c  kac(403, "not al
+00017970: 6c6f 7765 6420 666f 7220 7573 6572 2022  lowed for user "
+00017980: 202b 2073 656c 662e 756e 616d 6529 0a0a   + self.uname)..
+00017990: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000179a0: 6172 6773 2e6e 6f5f 7374 6163 6b3a 0a20  args.no_stack:. 
+000179b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000179c0: 2050 6562 6b61 6328 3430 332c 2022 7468   Pebkac(403, "th
+000179d0: 6520 7374 6163 6b64 756d 7020 6665 6174  e stackdump feat
+000179e0: 7572 6520 6973 2064 6973 6162 6c65 6420  ure is disabled 
+000179f0: 696e 2073 6572 7665 7220 636f 6e66 6967  in server config
+00017a00: 2229 0a0a 2020 2020 2020 2020 7265 7420  ")..        ret 
+00017a10: 3d20 223c 7072 653e 7b7d 5c6e 7b7d 222e  = "<pre>{}\n{}".
+00017a20: 666f 726d 6174 2874 696d 652e 7469 6d65  format(time.time
+00017a30: 2829 2c20 6874 6d6c 5f65 7363 6170 6528  (), html_escape(
+00017a40: 616c 6c74 7261 6365 2829 2929 0a20 2020  alltrace())).   
+00017a50: 2020 2020 2073 656c 662e 7265 706c 7928       self.reply(
+00017a60: 7265 742e 656e 636f 6465 2822 7574 662d  ret.encode("utf-
+00017a70: 3822 2929 0a20 2020 2020 2020 2072 6574  8")).        ret
+00017a80: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
+00017a90: 6620 7478 5f74 7265 6528 7365 6c66 2920  f tx_tree(self) 
+00017aa0: 203a 0a20 2020 2020 2020 2074 6f70 203d   :.        top =
+00017ab0: 2073 656c 662e 7570 6172 616d 5b22 7472   self.uparam["tr
+00017ac0: 6565 225d 206f 7220 2222 0a20 2020 2020  ee"] or "".     
+00017ad0: 2020 2064 7374 203d 2073 656c 662e 7670     dst = self.vp
+00017ae0: 6174 680a 2020 2020 2020 2020 6966 2074  ath.        if t
+00017af0: 6f70 2069 6e20 5b22 2e22 2c20 222e 2e22  op in [".", ".."
+00017b00: 5d3a 0a20 2020 2020 2020 2020 2020 2074  ]:.            t
+00017b10: 6f70 203d 2075 6e64 6f74 2873 656c 662e  op = undot(self.
+00017b20: 7670 6174 6820 2b20 222f 2220 2b20 746f  vpath + "/" + to
+00017b30: 7029 0a0a 2020 2020 2020 2020 6966 2074  p)..        if t
+00017b40: 6f70 203d 3d20 6473 743a 0a20 2020 2020  op == dst:.     
+00017b50: 2020 2020 2020 2064 7374 203d 2022 220a         dst = "".
+00017b60: 2020 2020 2020 2020 656c 6966 2074 6f70          elif top
+00017b70: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00017b80: 206e 6f74 2064 7374 2e73 7461 7274 7377   not dst.startsw
+00017b90: 6974 6828 746f 7020 2b20 222f 2229 3a0a  ith(top + "/"):.
+00017ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bb0: 7261 6973 6520 5065 626b 6163 2834 3030  raise Pebkac(400
+00017bc0: 2c20 2261 7267 2066 756e 6b22 290a 0a20  , "arg funk").. 
+00017bd0: 2020 2020 2020 2020 2020 2064 7374 203d             dst =
+00017be0: 2064 7374 5b6c 656e 2874 6f70 2920 2b20   dst[len(top) + 
+00017bf0: 3120 3a5d 0a0a 2020 2020 2020 2020 7265  1 :]..        re
+00017c00: 7420 3d20 7365 6c66 2e67 656e 5f74 7265  t = self.gen_tre
+00017c10: 6528 746f 702c 2064 7374 290a 2020 2020  e(top, dst).    
+00017c20: 2020 2020 6966 2073 656c 662e 6973 5f76      if self.is_v
+00017c30: 7072 6f78 6965 643a 0a20 2020 2020 2020  proxied:.       
+00017c40: 2020 2020 2070 6172 656e 7473 203d 2073       parents = s
+00017c50: 656c 662e 6172 6773 2e52 2e73 706c 6974  elf.args.R.split
+00017c60: 2822 2f22 290a 2020 2020 2020 2020 2020  ("/").          
+00017c70: 2020 666f 7220 7061 7265 6e74 2069 6e20    for parent in 
+00017c80: 7061 7265 6e74 735b 3a3a 2d31 5d3a 0a20  parents[::-1]:. 
+00017c90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00017ca0: 6574 203d 207b 226b 7b7d 222e 666f 726d  et = {"k{}".form
+00017cb0: 6174 2870 6172 656e 7429 3a20 7265 742c  at(parent): ret,
+00017cc0: 2022 6122 3a20 5b5d 7d0a 0a20 2020 2020   "a": []}..     
+00017cd0: 2020 207a 7320 3d20 6a73 6f6e 2e64 756d     zs = json.dum
+00017ce0: 7073 2872 6574 290a 2020 2020 2020 2020  ps(ret).        
+00017cf0: 7365 6c66 2e72 6570 6c79 287a 732e 656e  self.reply(zs.en
+00017d00: 636f 6465 2822 7574 662d 3822 292c 206d  code("utf-8"), m
+00017d10: 696d 653d 2261 7070 6c69 6361 7469 6f6e  ime="application
+00017d20: 2f6a 736f 6e22 290a 2020 2020 2020 2020  /json").        
+00017d30: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+00017d40: 2064 6566 2067 656e 5f74 7265 6528 7365   def gen_tree(se
+00017d50: 6c66 2c20 746f 7020 2c20 7461 7267 6574  lf, top , target
+00017d60: 2029 2020 203a 0a20 2020 2020 2020 2072   )   :.        r
+00017d70: 6574 2020 203d 207b 7d0a 2020 2020 2020  et   = {}.      
+00017d80: 2020 6578 636c 203d 204e 6f6e 650a 2020    excl = None.  
+00017d90: 2020 2020 2020 6966 2074 6172 6765 743a        if target:
+00017da0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00017db0: 6c2c 2074 6172 6765 7420 3d20 2874 6172  l, target = (tar
+00017dc0: 6765 742e 7370 6c69 7428 222f 222c 2031  get.split("/", 1
+00017dd0: 2920 2b20 5b22 225d 295b 3a32 5d0a 2020  ) + [""])[:2].  
+00017de0: 2020 2020 2020 2020 2020 7375 6220 3d20            sub = 
+00017df0: 7365 6c66 2e67 656e 5f74 7265 6528 222f  self.gen_tree("/
+00017e00: 222e 6a6f 696e 285b 746f 702c 2065 7863  ".join([top, exc
+00017e10: 6c5d 292e 7374 7269 7028 222f 2229 2c20  l]).strip("/"), 
+00017e20: 7461 7267 6574 290a 2020 2020 2020 2020  target).        
+00017e30: 2020 2020 7265 745b 226b 2220 2b20 7175      ret["k" + qu
+00017e40: 6f74 6570 2865 7863 6c29 5d20 3d20 7375  otep(excl)] = su
+00017e50: 620a 0a20 2020 2020 2020 2074 7279 3a0a  b..        try:.
+00017e60: 2020 2020 2020 2020 2020 2020 766e 2c20              vn, 
+00017e70: 7265 6d20 3d20 7365 6c66 2e61 7372 762e  rem = self.asrv.
+00017e80: 7666 732e 6765 7428 746f 702c 2073 656c  vfs.get(top, sel
+00017e90: 662e 756e 616d 652c 2054 7275 652c 2046  f.uname, True, F
+00017ea0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00017eb0: 2020 6673 726f 6f74 2c20 7666 735f 6c73    fsroot, vfs_ls
+00017ec0: 2c20 7666 735f 7669 7274 203d 2076 6e2e  , vfs_virt = vn.
+00017ed0: 6c73 280a 2020 2020 2020 2020 2020 2020  ls(.            
+00017ee0: 2020 2020 7265 6d2c 0a20 2020 2020 2020      rem,.       
+00017ef0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00017f00: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00017f10: 2020 2020 206e 6f74 2073 656c 662e 6172       not self.ar
+00017f20: 6773 2e6e 6f5f 7363 616e 6469 722c 0a20  gs.no_scandir,. 
+00017f30: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00017f40: 5b54 7275 652c 2046 616c 7365 5d2c 205b  [True, False], [
+00017f50: 4661 6c73 652c 2054 7275 655d 5d2c 0a20  False, True]],. 
+00017f60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00017f70: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+00017f80: 2020 2020 2020 2020 2076 6673 5f6c 7320           vfs_ls 
+00017f90: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00017fa0: 2076 6673 5f76 6972 7420 3d20 7b7d 0a20   vfs_virt = {}. 
+00017fb0: 2020 2020 2020 2020 2020 2066 6f72 2076             for v
+00017fc0: 2069 6e20 7365 6c66 2e72 766f 6c3a 0a20   in self.rvol:. 
+00017fd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00017fe0: 312c 2064 3220 3d20 762e 7273 706c 6974  1, d2 = v.rsplit
+00017ff0: 2822 2f22 2c20 3129 2069 6620 222f 2220  ("/", 1) if "/" 
+00018000: 696e 2076 2065 6c73 6520 5b22 222c 2076  in v else ["", v
+00018010: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00018020: 2020 6966 2064 3120 3d3d 2074 6f70 3a0a    if d1 == top:.
+00018030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018040: 2020 2020 7666 735f 7669 7274 5b64 325d      vfs_virt[d2]
+00018050: 203d 2073 656c 662e 6173 7276 2e76 6673   = self.asrv.vfs
+00018060: 2020 2320 7479 7065 6368 6b2c 2076 616c    # typechk, val
+00018070: 7565 206e 6576 6572 2072 6561 640a 0a20  ue never read.. 
+00018080: 2020 2020 2020 2064 6972 7320 3d20 5b5d         dirs = []
+00018090: 0a0a 2020 2020 2020 2020 6469 726e 616d  ..        dirnam
+000180a0: 6573 203d 205b 785b 305d 2066 6f72 2078  es = [x[0] for x
+000180b0: 2069 6e20 7666 735f 6c73 2069 6620 7374   in vfs_ls if st
+000180c0: 6174 2e53 5f49 5344 4952 2878 5b31 5d2e  at.S_ISDIR(x[1].
+000180d0: 7374 5f6d 6f64 6529 5d0a 0a20 2020 2020  st_mode)]..     
+000180e0: 2020 2069 6620 6e6f 7420 7365 6c66 2e61     if not self.a
+000180f0: 7267 732e 6564 206f 7220 2264 6f74 7322  rgs.ed or "dots"
+00018100: 206e 6f74 2069 6e20 7365 6c66 2e75 7061   not in self.upa
+00018110: 7261 6d3a 0a20 2020 2020 2020 2020 2020  ram:.           
+00018120: 2064 6972 6e61 6d65 7320 3d20 6578 636c   dirnames = excl
+00018130: 7564 655f 646f 7466 696c 6573 2864 6972  ude_dotfiles(dir
+00018140: 6e61 6d65 7329 0a0a 2020 2020 2020 2020  names)..        
+00018150: 666f 7220 666e 2069 6e20 5b78 2066 6f72  for fn in [x for
+00018160: 2078 2069 6e20 6469 726e 616d 6573 2069   x in dirnames i
+00018170: 6620 7820 213d 2065 7863 6c5d 3a0a 2020  f x != excl]:.  
+00018180: 2020 2020 2020 2020 2020 6469 7273 2e61            dirs.a
+00018190: 7070 656e 6428 7175 6f74 6570 2866 6e29  ppend(quotep(fn)
+000181a0: 290a 0a20 2020 2020 2020 2066 6f72 2078  )..        for x
+000181b0: 2069 6e20 7666 735f 7669 7274 3a0a 2020   in vfs_virt:.  
+000181c0: 2020 2020 2020 2020 2020 6966 2078 2021            if x !
+000181d0: 3d20 6578 636c 3a0a 2020 2020 2020 2020  = excl:.        
+000181e0: 2020 2020 2020 2020 6469 7273 2e61 7070          dirs.app
+000181f0: 656e 6428 7829 0a0a 2020 2020 2020 2020  end(x)..        
+00018200: 7265 745b 2261 225d 203d 2064 6972 730a  ret["a"] = dirs.
+00018210: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00018220: 6574 0a0a 2020 2020 6465 6620 7478 5f75  et..    def tx_u
+00018230: 7073 2873 656c 6629 2020 3a0a 2020 2020  ps(self)  :.    
+00018240: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00018250: 6172 6773 2e75 6e70 6f73 743a 0a20 2020  args.unpost:.   
+00018260: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
+00018270: 6562 6b61 6328 3430 332c 2022 7468 6520  ebkac(403, "the 
+00018280: 756e 706f 7374 2066 6561 7475 7265 2069  unpost feature i
+00018290: 7320 6469 7361 626c 6564 2069 6e20 7365  s disabled in se
+000182a0: 7276 6572 2063 6f6e 6669 6722 290a 0a20  rver config").. 
+000182b0: 2020 2020 2020 2069 6478 203d 2073 656c         idx = sel
+000182c0: 662e 636f 6e6e 2e67 6574 5f75 3269 6478  f.conn.get_u2idx
+000182d0: 2829 0a20 2020 2020 2020 2069 6620 6e6f  ().        if no
+000182e0: 7420 6861 7361 7474 7228 6964 782c 2022  t hasattr(idx, "
+000182f0: 705f 656e 6422 293a 0a20 2020 2020 2020  p_end"):.       
+00018300: 2020 2020 2072 6169 7365 2050 6562 6b61       raise Pebka
+00018310: 6328 3530 302c 2022 7371 6c69 7465 3320  c(500, "sqlite3 
+00018320: 6973 206e 6f74 2061 7661 696c 6162 6c65  is not available
+00018330: 206f 6e20 7468 6520 7365 7276 6572 3b20   on the server; 
+00018340: 6361 6e6e 6f74 2075 6e70 6f73 7422 290a  cannot unpost").
+00018350: 0a20 2020 2020 2020 2066 696c 7420 3d20  .        filt = 
+00018360: 7365 6c66 2e75 7061 7261 6d2e 6765 7428  self.uparam.get(
+00018370: 2266 696c 7465 7222 290a 2020 2020 2020  "filter").      
+00018380: 2020 6669 6c74 203d 2075 6e71 756f 7465    filt = unquote
+00018390: 7028 6669 6c74 206f 7220 2222 290a 2020  p(filt or "").  
+000183a0: 2020 2020 2020 6c6d 203d 2022 7570 7320        lm = "ups 
+000183b0: 5b7b 7d5d 222e 666f 726d 6174 2866 696c  [{}]".format(fil
+000183c0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+000183d0: 6c6f 6728 6c6d 290a 0a20 2020 2020 2020  log(lm)..       
+000183e0: 2072 6574 2020 203d 205b 5d0a 2020 2020   ret   = [].    
+000183f0: 2020 2020 7430 203d 2074 696d 652e 7469      t0 = time.ti
+00018400: 6d65 2829 0a20 2020 2020 2020 206c 696d  me().        lim
+00018410: 203d 2074 696d 652e 7469 6d65 2829 202d   = time.time() -
+00018420: 2073 656c 662e 6172 6773 2e75 6e70 6f73   self.args.unpos
+00018430: 740a 2020 2020 2020 2020 666b 5f76 6f6c  t.        fk_vol
+00018440: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+00018450: 2020 766f 6c3a 2076 6f6c 2e66 6c61 6773    vol: vol.flags
+00018460: 5b22 666b 225d 0a20 2020 2020 2020 2020  ["fk"].         
+00018470: 2020 2066 6f72 2076 702c 2076 6f6c 2069     for vp, vol i
+00018480: 6e20 7365 6c66 2e61 7372 762e 7666 732e  n self.asrv.vfs.
+00018490: 616c 6c5f 766f 6c73 2e69 7465 6d73 2829  all_vols.items()
+000184a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000184b0: 2266 6b22 2069 6e20 766f 6c2e 666c 6167  "fk" in vol.flag
+000184c0: 7320 616e 6420 2876 7020 696e 2073 656c  s and (vp in sel
+000184d0: 662e 7276 6f6c 206f 7220 7670 2069 6e20  f.rvol or vp in 
+000184e0: 7365 6c66 2e75 7076 6f6c 290a 2020 2020  self.upvol).    
+000184f0: 2020 2020 7d0a 2020 2020 2020 2020 666f      }.        fo
+00018500: 7220 766f 6c20 696e 2073 656c 662e 6173  r vol in self.as
+00018510: 7276 2e76 6673 2e61 6c6c 5f76 6f6c 732e  rv.vfs.all_vols.
+00018520: 7661 6c75 6573 2829 3a0a 2020 2020 2020  values():.      
+00018530: 2020 2020 2020 6375 7220 3d20 6964 782e        cur = idx.
+00018540: 6765 745f 6375 7228 766f 6c2e 7265 616c  get_cur(vol.real
+00018550: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+00018560: 2020 6966 206e 6f74 2063 7572 3a0a 2020    if not cur:.  
+00018570: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00018580: 6e74 696e 7565 0a0a 2020 2020 2020 2020  ntinue..        
+00018590: 2020 2020 6e66 6b20 3d20 666b 5f76 6f6c      nfk = fk_vol
+000185a0: 732e 6765 7428 766f 6c2c 2030 290a 0a20  s.get(vol, 0).. 
+000185b0: 2020 2020 2020 2020 2020 2071 203d 2022             q = "
+000185c0: 7365 6c65 6374 2073 7a2c 2072 642c 2066  select sz, rd, f
+000185d0: 6e2c 2061 7420 6672 6f6d 2075 7020 7768  n, at from up wh
+000185e0: 6572 6520 6970 3d3f 2061 6e64 2061 743e  ere ip=? and at>
+000185f0: 3f22 0a20 2020 2020 2020 2020 2020 2066  ?".            f
+00018600: 6f72 2073 7a2c 2072 642c 2066 6e2c 2061  or sz, rd, fn, a
+00018610: 7420 696e 2063 7572 2e65 7865 6375 7465  t in cur.execute
+00018620: 2871 2c20 2873 656c 662e 6970 2c20 6c69  (q, (self.ip, li
+00018630: 6d29 293a 0a20 2020 2020 2020 2020 2020  m)):.           
+00018640: 2020 2020 2076 7020 3d20 222f 2220 2b20       vp = "/" + 
+00018650: 222f 222e 6a6f 696e 2878 2066 6f72 2078  "/".join(x for x
+00018660: 2069 6e20 5b76 6f6c 2e76 7061 7468 2c20   in [vol.vpath, 
+00018670: 7264 2c20 666e 5d20 6966 2078 290a 2020  rd, fn] if x).  
+00018680: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00018690: 2066 696c 7420 616e 6420 6669 6c74 206e   filt and filt n
+000186a0: 6f74 2069 6e20 7670 3a0a 2020 2020 2020  ot in vp:.      
+000186b0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000186c0: 6e74 696e 7565 0a0a 2020 2020 2020 2020  ntinue..        
+000186d0: 2020 2020 2020 2020 7276 203d 207b 2276          rv = {"v
+000186e0: 7022 3a20 7175 6f74 6570 2876 7029 2c20  p": quotep(vp), 
+000186f0: 2273 7a22 3a20 737a 2c20 2261 7422 3a20  "sz": sz, "at": 
+00018700: 6174 2c20 226e 666b 223a 206e 666b 7d0a  at, "nfk": nfk}.
 00018710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018720: 7265 742e 6170 7065 6e64 2872 7629 0a20  ret.append(rv). 
-00018730: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00018740: 6620 6c65 6e28 7265 7429 203e 2033 3030  f len(ret) > 300
-00018750: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-00018760: 2020 2020 2020 2072 6574 2e73 6f72 7428         ret.sort(
-00018770: 6b65 793d 6c61 6d62 6461 2078 3a20 785b  key=lambda x: x[
-00018780: 2261 7422 5d2c 2072 6576 6572 7365 3d54  "at"], reverse=T
-00018790: 7275 6529 2020 2320 7479 7065 3a20 6967  rue)  # type: ig
-000187a0: 6e6f 7265 0a20 2020 2020 2020 2020 2020  nore.           
-000187b0: 2020 2020 2020 2020 2072 6574 203d 2072           ret = r
-000187c0: 6574 5b3a 3230 3030 5d0a 0a20 2020 2020  et[:2000]..     
-000187d0: 2020 2072 6574 2e73 6f72 7428 6b65 793d     ret.sort(key=
-000187e0: 6c61 6d62 6461 2078 3a20 785b 2261 7422  lambda x: x["at"
-000187f0: 5d2c 2072 6576 6572 7365 3d54 7275 6529  ], reverse=True)
-00018800: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-00018810: 0a20 2020 2020 2020 206e 203d 2030 0a20  .        n = 0. 
-00018820: 2020 2020 2020 2066 6f72 2072 7620 696e         for rv in
-00018830: 2072 6574 5b3a 3131 3030 305d 3a0a 2020   ret[:11000]:.  
-00018840: 2020 2020 2020 2020 2020 6e66 6b20 3d20            nfk = 
-00018850: 7276 2e70 6f70 2822 6e66 6b22 290a 2020  rv.pop("nfk").  
-00018860: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00018870: 206e 666b 3a0a 2020 2020 2020 2020 2020   nfk:.          
-00018880: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
-00018890: 2020 2020 2020 2020 2020 2020 6170 203d              ap =
-000188a0: 2072 762e 706f 7028 2261 7022 290a 2020   rv.pop("ap").  
-000188b0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-000188c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000188d0: 7420 3d20 626f 732e 7374 6174 2861 7029  t = bos.stat(ap)
-000188e0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-000188f0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-00018900: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-00018910: 2020 2020 2020 2020 2020 2066 6b20 3d20             fk = 
-00018920: 7365 6c66 2e67 656e 5f66 6b28 0a20 2020  self.gen_fk(.   
-00018930: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018940: 662e 6172 6773 2e66 6b5f 7361 6c74 2c20  f.args.fk_salt, 
-00018950: 6170 2c20 7374 2e73 745f 7369 7a65 2c20  ap, st.st_size, 
-00018960: 3020 6966 2041 4e59 5749 4e20 656c 7365  0 if ANYWIN else
-00018970: 2073 742e 7374 5f69 6e6f 0a20 2020 2020   st.st_ino.     
-00018980: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00018990: 2020 2020 2072 765b 2276 7022 5d20 2b3d       rv["vp"] +=
-000189a0: 2022 3f6b 3d22 202b 2066 6b5b 3a6e 666b   "?k=" + fk[:nfk
-000189b0: 5d0a 0a20 2020 2020 2020 2020 2020 206e  ]..            n
-000189c0: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
-000189d0: 2020 6966 206e 203e 2032 3030 303a 0a20    if n > 2000:. 
-000189e0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-000189f0: 7265 616b 0a0a 2020 2020 2020 2020 7265  reak..        re
-00018a00: 7420 3d20 7265 745b 3a32 3030 305d 0a0a  t = ret[:2000]..
-00018a10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00018a20: 6973 5f76 7072 6f78 6965 643a 0a20 2020  is_vproxied:.   
-00018a30: 2020 2020 2020 2020 2066 6f72 2076 2069           for v i
-00018a40: 6e20 7265 743a 0a20 2020 2020 2020 2020  n ret:.         
-00018a50: 2020 2020 2020 2076 5b22 7670 225d 203d         v["vp"] =
-00018a60: 2073 656c 662e 6172 6773 2e53 5220 2b20   self.args.SR + 
-00018a70: 765b 2276 7022 5d0a 0a20 2020 2020 2020  v["vp"]..       
-00018a80: 206a 7478 7420 3d20 6a73 6f6e 2e64 756d   jtxt = json.dum
-00018a90: 7073 2872 6574 2c20 696e 6465 6e74 3d32  ps(ret, indent=2
-00018aa0: 2c20 736f 7274 5f6b 6579 733d 5472 7565  , sort_keys=True
-00018ab0: 292e 656e 636f 6465 2822 7574 662d 3822  ).encode("utf-8"
-00018ac0: 2c20 2272 6570 6c61 6365 2229 0a20 2020  , "replace").   
-00018ad0: 2020 2020 2073 656c 662e 6c6f 6728 227b       self.log("{
-00018ae0: 7d20 237b 7d20 7b3a 2e32 667d 7365 6322  } #{} {:.2f}sec"
-00018af0: 2e66 6f72 6d61 7428 6c6d 2c20 6c65 6e28  .format(lm, len(
-00018b00: 7265 7429 2c20 7469 6d65 2e74 696d 6528  ret), time.time(
-00018b10: 2920 2d20 7430 2929 0a20 2020 2020 2020  ) - t0)).       
-00018b20: 2073 656c 662e 7265 706c 7928 6a74 7874   self.reply(jtxt
-00018b30: 2c20 6d69 6d65 3d22 6170 706c 6963 6174  , mime="applicat
-00018b40: 696f 6e2f 6a73 6f6e 2229 0a20 2020 2020  ion/json").     
-00018b50: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00018b60: 2020 2020 6465 6620 6861 6e64 6c65 5f72      def handle_r
-00018b70: 6d28 7365 6c66 2c20 7265 7120 2920 203a  m(self, req )  :
-00018b80: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00018b90: 7265 7120 616e 6420 6e6f 7420 7365 6c66  req and not self
-00018ba0: 2e63 616e 5f64 656c 6574 653a 0a20 2020  .can_delete:.   
-00018bb0: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
-00018bc0: 6562 6b61 6328 3430 332c 2022 6e6f 7420  ebkac(403, "not 
-00018bd0: 616c 6c6f 7765 6420 666f 7220 7573 6572  allowed for user
-00018be0: 2022 202b 2073 656c 662e 756e 616d 6529   " + self.uname)
-00018bf0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00018c00: 662e 6172 6773 2e6e 6f5f 6465 6c3a 0a20  f.args.no_del:. 
-00018c10: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00018c20: 2050 6562 6b61 6328 3430 332c 2022 7468   Pebkac(403, "th
-00018c30: 6520 6465 6c65 7465 2066 6561 7475 7265  e delete feature
-00018c40: 2069 7320 6469 7361 626c 6564 2069 6e20   is disabled in 
-00018c50: 7365 7276 6572 2063 6f6e 6669 6722 290a  server config").
-00018c60: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00018c70: 7265 713a 0a20 2020 2020 2020 2020 2020  req:.           
-00018c80: 2072 6571 203d 205b 7365 6c66 2e76 7061   req = [self.vpa
-00018c90: 7468 5d0a 2020 2020 2020 2020 656c 6966  th].        elif
-00018ca0: 2073 656c 662e 6973 5f76 7072 6f78 6965   self.is_vproxie
-00018cb0: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
-00018cc0: 6571 203d 205b 785b 6c65 6e28 7365 6c66  eq = [x[len(self
-00018cd0: 2e61 7267 732e 5352 2920 3a5d 2066 6f72  .args.SR) :] for
-00018ce0: 2078 2069 6e20 7265 715d 0a0a 2020 2020   x in req]..    
-00018cf0: 2020 2020 6e6c 696d 203d 2069 6e74 2873      nlim = int(s
-00018d00: 656c 662e 7570 6172 616d 2e67 6574 2822  elf.uparam.get("
-00018d10: 6c69 6d22 2920 6f72 2030 290a 2020 2020  lim") or 0).    
-00018d20: 2020 2020 6c69 6d20 3d20 5b6e 6c69 6d2c      lim = [nlim,
-00018d30: 206e 6c69 6d5d 2069 6620 6e6c 696d 2065   nlim] if nlim e
-00018d40: 6c73 6520 5b5d 0a0a 2020 2020 2020 2020  lse []..        
-00018d50: 7820 3d20 7365 6c66 2e63 6f6e 6e2e 6873  x = self.conn.hs
-00018d60: 7276 2e62 726f 6b65 722e 6173 6b28 2275  rv.broker.ask("u
-00018d70: 7032 6b2e 6861 6e64 6c65 5f72 6d22 2c20  p2k.handle_rm", 
-00018d80: 7365 6c66 2e75 6e61 6d65 2c20 7365 6c66  self.uname, self
-00018d90: 2e69 702c 2072 6571 2c20 6c69 6d29 0a20  .ip, req, lim). 
-00018da0: 2020 2020 2020 2073 656c 662e 6c6f 7564         self.loud
-00018db0: 5f72 6570 6c79 2878 2e67 6574 2829 290a  _reply(x.get()).
-00018dc0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00018dd0: 7275 650a 0a20 2020 2064 6566 2068 616e  rue..    def han
-00018de0: 646c 655f 6d76 2873 656c 6629 2020 3a0a  dle_mv(self)  :.
-00018df0: 2020 2020 2020 2020 2320 6675 6c6c 2070          # full p
-00018e00: 6174 6820 6f66 206e 6577 206c 6f63 2028  ath of new loc (
-00018e10: 696e 636c 2066 696c 656e 616d 6529 0a20  incl filename). 
-00018e20: 2020 2020 2020 2064 7374 203d 2073 656c         dst = sel
-00018e30: 662e 7570 6172 616d 2e67 6574 2822 6d6f  f.uparam.get("mo
-00018e40: 7665 2229 0a0a 2020 2020 2020 2020 6966  ve")..        if
-00018e50: 2073 656c 662e 6973 5f76 7072 6f78 6965   self.is_vproxie
-00018e60: 6420 616e 6420 6473 7420 616e 6420 6473  d and dst and ds
-00018e70: 742e 7374 6172 7473 7769 7468 2873 656c  t.startswith(sel
-00018e80: 662e 6172 6773 2e53 5229 3a0a 2020 2020  f.args.SR):.    
-00018e90: 2020 2020 2020 2020 6473 7420 3d20 6473          dst = ds
-00018ea0: 745b 6c65 6e28 7365 6c66 2e61 7267 732e  t[len(self.args.
-00018eb0: 5253 2920 3a5d 0a0a 2020 2020 2020 2020  RS) :]..        
-00018ec0: 6966 206e 6f74 2064 7374 3a0a 2020 2020  if not dst:.    
-00018ed0: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
-00018ee0: 626b 6163 2834 3030 2c20 226e 6565 6420  bkac(400, "need 
-00018ef0: 6473 7420 7670 6174 6822 290a 0a20 2020  dst vpath")..   
-00018f00: 2020 2020 2023 2078 2d77 7777 2d66 6f72       # x-www-for
-00018f10: 6d2d 7572 6c65 6e63 6f64 6564 2028 7572  m-urlencoded (ur
-00018f20: 6c20 7175 6572 7920 7061 7274 2920 7573  l query part) us
-00018f30: 6573 0a20 2020 2020 2020 2023 2065 6974  es.        # eit
-00018f40: 6865 7220 2b20 6f72 2025 3230 2066 6f72  her + or %20 for
-00018f50: 2030 7832 3020 736f 2068 616e 646c 6520   0x20 so handle 
-00018f60: 626f 7468 0a20 2020 2020 2020 2064 7374  both.        dst
-00018f70: 203d 2075 6e71 756f 7465 7028 6473 742e   = unquotep(dst.
-00018f80: 7265 706c 6163 6528 222b 222c 2022 2022  replace("+", " "
-00018f90: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-00018fa0: 6e20 7365 6c66 2e5f 6d76 2873 656c 662e  n self._mv(self.
-00018fb0: 7670 6174 682c 2064 7374 290a 0a20 2020  vpath, dst)..   
-00018fc0: 2064 6566 205f 6d76 2873 656c 662c 2076   def _mv(self, v
-00018fd0: 7372 6320 2c20 7664 7374 2029 2020 3a0a  src , vdst )  :.
-00018fe0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00018ff0: 656c 662e 6361 6e5f 6d6f 7665 3a0a 2020  elf.can_move:.  
-00019000: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00019010: 5065 626b 6163 2834 3033 2c20 226e 6f74  Pebkac(403, "not
-00019020: 2061 6c6c 6f77 6564 2066 6f72 2075 7365   allowed for use
-00019030: 7220 2220 2b20 7365 6c66 2e75 6e61 6d65  r " + self.uname
-00019040: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00019050: 6c66 2e61 7267 732e 6e6f 5f6d 763a 0a20  lf.args.no_mv:. 
-00019060: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00019070: 2050 6562 6b61 6328 3430 332c 2022 7468   Pebkac(403, "th
-00019080: 6520 7265 6e61 6d65 2f6d 6f76 6520 6665  e rename/move fe
-00019090: 6174 7572 6520 6973 2064 6973 6162 6c65  ature is disable
-000190a0: 6420 696e 2073 6572 7665 7220 636f 6e66  d in server conf
-000190b0: 6967 2229 0a0a 2020 2020 2020 2020 7820  ig")..        x 
-000190c0: 3d20 7365 6c66 2e63 6f6e 6e2e 6873 7276  = self.conn.hsrv
-000190d0: 2e62 726f 6b65 722e 6173 6b28 2275 7032  .broker.ask("up2
-000190e0: 6b2e 6861 6e64 6c65 5f6d 7622 2c20 7365  k.handle_mv", se
-000190f0: 6c66 2e75 6e61 6d65 2c20 7673 7263 2c20  lf.uname, vsrc, 
-00019100: 7664 7374 290a 2020 2020 2020 2020 7365  vdst).        se
-00019110: 6c66 2e6c 6f75 645f 7265 706c 7928 782e  lf.loud_reply(x.
-00019120: 6765 7428 292c 2073 7461 7475 733d 3230  get(), status=20
-00019130: 3129 0a20 2020 2020 2020 2072 6574 7572  1).        retur
-00019140: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
-00019150: 7478 5f6c 7328 7365 6c66 2c20 6c73 2020  tx_ls(self, ls  
-00019160: 2920 203a 0a20 2020 2020 2020 2064 6972  )  :.        dir
-00019170: 7320 3d20 6c73 5b22 6469 7273 225d 0a20  s = ls["dirs"]. 
-00019180: 2020 2020 2020 2066 696c 6573 203d 206c         files = l
-00019190: 735b 2266 696c 6573 225d 0a20 2020 2020  s["files"].     
-000191a0: 2020 2061 7267 203d 2073 656c 662e 7570     arg = self.up
-000191b0: 6172 616d 5b22 6c73 225d 0a20 2020 2020  aram["ls"].     
-000191c0: 2020 2069 6620 6172 6720 696e 205b 2276     if arg in ["v
-000191d0: 222c 2022 7422 2c20 2274 7874 225d 3a0a  ", "t", "txt"]:.
-000191e0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000191f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019200: 2062 6967 6765 7374 203d 206d 6178 286c   biggest = max(l
-00019210: 735b 2266 696c 6573 225d 202b 206c 735b  s["files"] + ls[
-00019220: 2264 6972 7322 5d2c 206b 6579 3d69 7465  "dirs"], key=ite
-00019230: 6d67 6574 7465 7228 2273 7a22 2929 5b22  mgetter("sz"))["
-00019240: 737a 225d 0a20 2020 2020 2020 2020 2020  sz"].           
-00019250: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00019260: 2020 2020 2020 2020 2062 6967 6765 7374           biggest
-00019270: 203d 2030 0a0a 2020 2020 2020 2020 2020   = 0..          
-00019280: 2020 6966 2061 7267 203d 3d20 2276 223a    if arg == "v":
-00019290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000192a0: 2066 6d74 203d 2022 5c30 3333 5b30 3b37   fmt = "\033[0;7
-000192b0: 3b33 366d 7b7b 7d7d 7b7b 3a3e 7b7d 7d7d  ;36m{{}}{{:>{}}}
-000192c0: 5c30 3333 5b30 6d20 7b7b 7d7d 220a 2020  \033[0m {{}}".  
-000192d0: 2020 2020 2020 2020 2020 2020 2020 6e66                nf
-000192e0: 6d74 203d 2022 7b7d 220a 2020 2020 2020  mt = "{}".      
-000192f0: 2020 2020 2020 2020 2020 6269 6767 6573            bigges
-00019300: 7420 3d20 300a 2020 2020 2020 2020 2020  t = 0.          
-00019310: 2020 2020 2020 6632 203d 2022 222e 6a6f        f2 = "".jo
-00019320: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
-00019330: 2020 2020 2020 2020 227b 7d7b 7b7d 7d22          "{}{{}}"
-00019340: 2e66 6f72 6d61 7428 7829 0a20 2020 2020  .format(x).     
-00019350: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00019360: 6f72 2078 2069 6e20 5b0a 2020 2020 2020  or x in [.      
-00019370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019380: 2020 225c 3033 335b 376d 222c 0a20 2020    "\033[7m",.   
-00019390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193a0: 2020 2020 2022 5c30 3333 5b32 376d 222c       "\033[27m",
-000193b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000193c0: 2020 2020 2020 2020 2022 222c 0a20 2020           "",.   
-000193d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193e0: 2020 2020 2022 5c30 3333 5b30 3b31 6d22       "\033[0;1m"
-000193f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019400: 2020 2020 2020 2020 2020 225c 3033 335b            "\033[
-00019410: 303b 3336 6d22 2c0a 2020 2020 2020 2020  0;36m",.        
-00019420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019430: 225c 3033 335b 306d 222c 0a20 2020 2020  "\033[0m",.     
-00019440: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00019450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019460: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00019470: 2020 2063 7461 6220 3d20 7b22 4222 3a20     ctab = {"B": 
-00019480: 362c 2022 4b22 3a20 352c 2022 4d22 3a20  6, "K": 5, "M": 
-00019490: 312c 2022 4722 3a20 337d 0a20 2020 2020  1, "G": 3}.     
-000194a0: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
-000194b0: 7374 2069 6e20 5b64 6972 732c 2066 696c  st in [dirs, fil
-000194c0: 6573 5d3a 0a20 2020 2020 2020 2020 2020  es]:.           
-000194d0: 2020 2020 2020 2020 2066 6f72 2078 2069           for x i
-000194e0: 6e20 6c73 743a 0a20 2020 2020 2020 2020  n lst:.         
-000194f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00019500: 203d 2078 5b22 6474 225d 2e72 6570 6c61   = x["dt"].repla
-00019510: 6365 2822 2d22 2c20 2220 2229 2e72 6570  ce("-", " ").rep
-00019520: 6c61 6365 2822 3a22 2c20 2220 2229 2e73  lace(":", " ").s
-00019530: 706c 6974 2822 2022 290a 2020 2020 2020  plit(" ").      
+00018720: 6966 206e 666b 3a0a 2020 2020 2020 2020  if nfk:.        
+00018730: 2020 2020 2020 2020 2020 2020 7276 5b22              rv["
+00018740: 6170 225d 203d 2076 6f6c 2e63 616e 6f6e  ap"] = vol.canon
+00018750: 6963 616c 2876 6a6f 696e 2872 642c 2066  ical(vjoin(rd, f
+00018760: 6e29 290a 0a20 2020 2020 2020 2020 2020  n))..           
+00018770: 2020 2020 2072 6574 2e61 7070 656e 6428       ret.append(
+00018780: 7276 290a 2020 2020 2020 2020 2020 2020  rv).            
+00018790: 2020 2020 6966 206c 656e 2872 6574 2920      if len(ret) 
+000187a0: 3e20 3330 3030 3a0a 2020 2020 2020 2020  > 3000:.        
+000187b0: 2020 2020 2020 2020 2020 2020 7265 742e              ret.
+000187c0: 736f 7274 286b 6579 3d6c 616d 6264 6120  sort(key=lambda 
+000187d0: 783a 2078 5b22 6174 225d 2c20 7265 7665  x: x["at"], reve
+000187e0: 7273 653d 5472 7565 2920 2023 2074 7970  rse=True)  # typ
+000187f0: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
+00018800: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00018810: 7420 3d20 7265 745b 3a32 3030 305d 0a0a  t = ret[:2000]..
+00018820: 2020 2020 2020 2020 7265 742e 736f 7274          ret.sort
+00018830: 286b 6579 3d6c 616d 6264 6120 783a 2078  (key=lambda x: x
+00018840: 5b22 6174 225d 2c20 7265 7665 7273 653d  ["at"], reverse=
+00018850: 5472 7565 2920 2023 2074 7970 653a 2069  True)  # type: i
+00018860: 676e 6f72 650a 2020 2020 2020 2020 6e20  gnore.        n 
+00018870: 3d20 300a 2020 2020 2020 2020 666f 7220  = 0.        for 
+00018880: 7276 2069 6e20 7265 745b 3a31 3130 3030  rv in ret[:11000
+00018890: 5d3a 0a20 2020 2020 2020 2020 2020 206e  ]:.            n
+000188a0: 666b 203d 2072 762e 706f 7028 226e 666b  fk = rv.pop("nfk
+000188b0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+000188c0: 6620 6e6f 7420 6e66 6b3a 0a20 2020 2020  f not nfk:.     
+000188d0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+000188e0: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
+000188f0: 2061 7020 3d20 7276 2e70 6f70 2822 6170   ap = rv.pop("ap
+00018900: 2229 0a20 2020 2020 2020 2020 2020 2074  ").            t
+00018910: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00018920: 2020 2020 7374 203d 2062 6f73 2e73 7461      st = bos.sta
+00018930: 7428 6170 290a 2020 2020 2020 2020 2020  t(ap).          
+00018940: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+00018950: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00018960: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+00018970: 666b 203d 2073 656c 662e 6765 6e5f 666b  fk = self.gen_fk
+00018980: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00018990: 2020 7365 6c66 2e61 7267 732e 666b 5f73    self.args.fk_s
+000189a0: 616c 742c 2061 702c 2073 742e 7374 5f73  alt, ap, st.st_s
+000189b0: 697a 652c 2030 2069 6620 414e 5957 494e  ize, 0 if ANYWIN
+000189c0: 2065 6c73 6520 7374 2e73 745f 696e 6f0a   else st.st_ino.
+000189d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000189e0: 2020 2020 2020 2020 2020 7276 5b22 7670            rv["vp
+000189f0: 225d 202b 3d20 223f 6b3d 2220 2b20 666b  "] += "?k=" + fk
+00018a00: 5b3a 6e66 6b5d 0a0a 2020 2020 2020 2020  [:nfk]..        
+00018a10: 2020 2020 6e20 2b3d 2031 0a20 2020 2020      n += 1.     
+00018a20: 2020 2020 2020 2069 6620 6e20 3e20 3230         if n > 20
+00018a30: 3030 3a0a 2020 2020 2020 2020 2020 2020  00:.            
+00018a40: 2020 2020 6272 6561 6b0a 0a20 2020 2020      break..     
+00018a50: 2020 2072 6574 203d 2072 6574 5b3a 3230     ret = ret[:20
+00018a60: 3030 5d0a 0a20 2020 2020 2020 2069 6620  00]..        if 
+00018a70: 7365 6c66 2e69 735f 7670 726f 7869 6564  self.is_vproxied
+00018a80: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00018a90: 7220 7620 696e 2072 6574 3a0a 2020 2020  r v in ret:.    
+00018aa0: 2020 2020 2020 2020 2020 2020 765b 2276              v["v
+00018ab0: 7022 5d20 3d20 7365 6c66 2e61 7267 732e  p"] = self.args.
+00018ac0: 5352 202b 2076 5b22 7670 225d 0a0a 2020  SR + v["vp"]..  
+00018ad0: 2020 2020 2020 6a74 7874 203d 206a 736f        jtxt = jso
+00018ae0: 6e2e 6475 6d70 7328 7265 742c 2069 6e64  n.dumps(ret, ind
+00018af0: 656e 743d 322c 2073 6f72 745f 6b65 7973  ent=2, sort_keys
+00018b00: 3d54 7275 6529 2e65 6e63 6f64 6528 2275  =True).encode("u
+00018b10: 7466 2d38 222c 2022 7265 706c 6163 6522  tf-8", "replace"
+00018b20: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00018b30: 6f67 2822 7b7d 2023 7b7d 207b 3a2e 3266  og("{} #{} {:.2f
+00018b40: 7d73 6563 222e 666f 726d 6174 286c 6d2c  }sec".format(lm,
+00018b50: 206c 656e 2872 6574 292c 2074 696d 652e   len(ret), time.
+00018b60: 7469 6d65 2829 202d 2074 3029 290a 2020  time() - t0)).  
+00018b70: 2020 2020 2020 7365 6c66 2e72 6570 6c79        self.reply
+00018b80: 286a 7478 742c 206d 696d 653d 2261 7070  (jtxt, mime="app
+00018b90: 6c69 6361 7469 6f6e 2f6a 736f 6e22 290a  lication/json").
+00018ba0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00018bb0: 7275 650a 0a20 2020 2064 6566 2068 616e  rue..    def han
+00018bc0: 646c 655f 726d 2873 656c 662c 2072 6571  dle_rm(self, req
+00018bd0: 2029 2020 3a0a 2020 2020 2020 2020 6966   )  :.        if
+00018be0: 206e 6f74 2072 6571 2061 6e64 206e 6f74   not req and not
+00018bf0: 2073 656c 662e 6361 6e5f 6465 6c65 7465   self.can_delete
+00018c00: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00018c10: 6973 6520 5065 626b 6163 2834 3033 2c20  ise Pebkac(403, 
+00018c20: 226e 6f74 2061 6c6c 6f77 6564 2066 6f72  "not allowed for
+00018c30: 2075 7365 7220 2220 2b20 7365 6c66 2e75   user " + self.u
+00018c40: 6e61 6d65 290a 0a20 2020 2020 2020 2069  name)..        i
+00018c50: 6620 7365 6c66 2e61 7267 732e 6e6f 5f64  f self.args.no_d
+00018c60: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
+00018c70: 7261 6973 6520 5065 626b 6163 2834 3033  raise Pebkac(403
+00018c80: 2c20 2274 6865 2064 656c 6574 6520 6665  , "the delete fe
+00018c90: 6174 7572 6520 6973 2064 6973 6162 6c65  ature is disable
+00018ca0: 6420 696e 2073 6572 7665 7220 636f 6e66  d in server conf
+00018cb0: 6967 2229 0a0a 2020 2020 2020 2020 6966  ig")..        if
+00018cc0: 206e 6f74 2072 6571 3a0a 2020 2020 2020   not req:.      
+00018cd0: 2020 2020 2020 7265 7120 3d20 5b73 656c        req = [sel
+00018ce0: 662e 7670 6174 685d 0a20 2020 2020 2020  f.vpath].       
+00018cf0: 2065 6c69 6620 7365 6c66 2e69 735f 7670   elif self.is_vp
+00018d00: 726f 7869 6564 3a0a 2020 2020 2020 2020  roxied:.        
+00018d10: 2020 2020 7265 7120 3d20 5b78 5b6c 656e      req = [x[len
+00018d20: 2873 656c 662e 6172 6773 2e53 5229 203a  (self.args.SR) :
+00018d30: 5d20 666f 7220 7820 696e 2072 6571 5d0a  ] for x in req].
+00018d40: 0a20 2020 2020 2020 206e 6c69 6d20 3d20  .        nlim = 
+00018d50: 696e 7428 7365 6c66 2e75 7061 7261 6d2e  int(self.uparam.
+00018d60: 6765 7428 226c 696d 2229 206f 7220 3029  get("lim") or 0)
+00018d70: 0a20 2020 2020 2020 206c 696d 203d 205b  .        lim = [
+00018d80: 6e6c 696d 2c20 6e6c 696d 5d20 6966 206e  nlim, nlim] if n
+00018d90: 6c69 6d20 656c 7365 205b 5d0a 0a20 2020  lim else []..   
+00018da0: 2020 2020 2078 203d 2073 656c 662e 636f       x = self.co
+00018db0: 6e6e 2e68 7372 762e 6272 6f6b 6572 2e61  nn.hsrv.broker.a
+00018dc0: 736b 2822 7570 326b 2e68 616e 646c 655f  sk("up2k.handle_
+00018dd0: 726d 222c 2073 656c 662e 756e 616d 652c  rm", self.uname,
+00018de0: 2073 656c 662e 6970 2c20 7265 712c 206c   self.ip, req, l
+00018df0: 696d 290a 2020 2020 2020 2020 7365 6c66  im).        self
+00018e00: 2e6c 6f75 645f 7265 706c 7928 782e 6765  .loud_reply(x.ge
+00018e10: 7428 2929 0a20 2020 2020 2020 2072 6574  t()).        ret
+00018e20: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
+00018e30: 6620 6861 6e64 6c65 5f6d 7628 7365 6c66  f handle_mv(self
+00018e40: 2920 203a 0a20 2020 2020 2020 2023 2066  )  :.        # f
+00018e50: 756c 6c20 7061 7468 206f 6620 6e65 7720  ull path of new 
+00018e60: 6c6f 6320 2869 6e63 6c20 6669 6c65 6e61  loc (incl filena
+00018e70: 6d65 290a 2020 2020 2020 2020 6473 7420  me).        dst 
+00018e80: 3d20 7365 6c66 2e75 7061 7261 6d2e 6765  = self.uparam.ge
+00018e90: 7428 226d 6f76 6522 290a 0a20 2020 2020  t("move")..     
+00018ea0: 2020 2069 6620 7365 6c66 2e69 735f 7670     if self.is_vp
+00018eb0: 726f 7869 6564 2061 6e64 2064 7374 2061  roxied and dst a
+00018ec0: 6e64 2064 7374 2e73 7461 7274 7377 6974  nd dst.startswit
+00018ed0: 6828 7365 6c66 2e61 7267 732e 5352 293a  h(self.args.SR):
+00018ee0: 0a20 2020 2020 2020 2020 2020 2064 7374  .            dst
+00018ef0: 203d 2064 7374 5b6c 656e 2873 656c 662e   = dst[len(self.
+00018f00: 6172 6773 2e52 5329 203a 5d0a 0a20 2020  args.RS) :]..   
+00018f10: 2020 2020 2069 6620 6e6f 7420 6473 743a       if not dst:
+00018f20: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00018f30: 7365 2050 6562 6b61 6328 3430 302c 2022  se Pebkac(400, "
+00018f40: 6e65 6564 2064 7374 2076 7061 7468 2229  need dst vpath")
+00018f50: 0a0a 2020 2020 2020 2020 2320 782d 7777  ..        # x-ww
+00018f60: 772d 666f 726d 2d75 726c 656e 636f 6465  w-form-urlencode
+00018f70: 6420 2875 726c 2071 7565 7279 2070 6172  d (url query par
+00018f80: 7429 2075 7365 730a 2020 2020 2020 2020  t) uses.        
+00018f90: 2320 6569 7468 6572 202b 206f 7220 2532  # either + or %2
+00018fa0: 3020 666f 7220 3078 3230 2073 6f20 6861  0 for 0x20 so ha
+00018fb0: 6e64 6c65 2062 6f74 680a 2020 2020 2020  ndle both.      
+00018fc0: 2020 6473 7420 3d20 756e 7175 6f74 6570    dst = unquotep
+00018fd0: 2864 7374 2e72 6570 6c61 6365 2822 2b22  (dst.replace("+"
+00018fe0: 2c20 2220 2229 290a 2020 2020 2020 2020  , " ")).        
+00018ff0: 7265 7475 726e 2073 656c 662e 5f6d 7628  return self._mv(
+00019000: 7365 6c66 2e76 7061 7468 2c20 6473 7429  self.vpath, dst)
+00019010: 0a0a 2020 2020 6465 6620 5f6d 7628 7365  ..    def _mv(se
+00019020: 6c66 2c20 7673 7263 202c 2076 6473 7420  lf, vsrc , vdst 
+00019030: 2920 203a 0a20 2020 2020 2020 2069 6620  )  :.        if 
+00019040: 6e6f 7420 7365 6c66 2e63 616e 5f6d 6f76  not self.can_mov
+00019050: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00019060: 6169 7365 2050 6562 6b61 6328 3430 332c  aise Pebkac(403,
+00019070: 2022 6e6f 7420 616c 6c6f 7765 6420 666f   "not allowed fo
+00019080: 7220 7573 6572 2022 202b 2073 656c 662e  r user " + self.
+00019090: 756e 616d 6529 0a0a 2020 2020 2020 2020  uname)..        
+000190a0: 6966 2073 656c 662e 6172 6773 2e6e 6f5f  if self.args.no_
+000190b0: 6d76 3a0a 2020 2020 2020 2020 2020 2020  mv:.            
+000190c0: 7261 6973 6520 5065 626b 6163 2834 3033  raise Pebkac(403
+000190d0: 2c20 2274 6865 2072 656e 616d 652f 6d6f  , "the rename/mo
+000190e0: 7665 2066 6561 7475 7265 2069 7320 6469  ve feature is di
+000190f0: 7361 626c 6564 2069 6e20 7365 7276 6572  sabled in server
+00019100: 2063 6f6e 6669 6722 290a 0a20 2020 2020   config")..     
+00019110: 2020 2078 203d 2073 656c 662e 636f 6e6e     x = self.conn
+00019120: 2e68 7372 762e 6272 6f6b 6572 2e61 736b  .hsrv.broker.ask
+00019130: 2822 7570 326b 2e68 616e 646c 655f 6d76  ("up2k.handle_mv
+00019140: 222c 2073 656c 662e 756e 616d 652c 2076  ", self.uname, v
+00019150: 7372 632c 2076 6473 7429 0a20 2020 2020  src, vdst).     
+00019160: 2020 2073 656c 662e 6c6f 7564 5f72 6570     self.loud_rep
+00019170: 6c79 2878 2e67 6574 2829 2c20 7374 6174  ly(x.get(), stat
+00019180: 7573 3d32 3031 290a 2020 2020 2020 2020  us=201).        
+00019190: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+000191a0: 2064 6566 2074 785f 6c73 2873 656c 662c   def tx_ls(self,
+000191b0: 206c 7320 2029 2020 3a0a 2020 2020 2020   ls  )  :.      
+000191c0: 2020 6469 7273 203d 206c 735b 2264 6972    dirs = ls["dir
+000191d0: 7322 5d0a 2020 2020 2020 2020 6669 6c65  s"].        file
+000191e0: 7320 3d20 6c73 5b22 6669 6c65 7322 5d0a  s = ls["files"].
+000191f0: 2020 2020 2020 2020 6172 6720 3d20 7365          arg = se
+00019200: 6c66 2e75 7061 7261 6d5b 226c 7322 5d0a  lf.uparam["ls"].
+00019210: 2020 2020 2020 2020 6966 2061 7267 2069          if arg i
+00019220: 6e20 5b22 7622 2c20 2274 222c 2022 7478  n ["v", "t", "tx
+00019230: 7422 5d3a 0a20 2020 2020 2020 2020 2020  t"]:.           
+00019240: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00019250: 2020 2020 2020 6269 6767 6573 7420 3d20        biggest = 
+00019260: 6d61 7828 6c73 5b22 6669 6c65 7322 5d20  max(ls["files"] 
+00019270: 2b20 6c73 5b22 6469 7273 225d 2c20 6b65  + ls["dirs"], ke
+00019280: 793d 6974 656d 6765 7474 6572 2822 737a  y=itemgetter("sz
+00019290: 2229 295b 2273 7a22 5d0a 2020 2020 2020  "))["sz"].      
+000192a0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+000192b0: 2020 2020 2020 2020 2020 2020 2020 6269                bi
+000192c0: 6767 6573 7420 3d20 300a 0a20 2020 2020  ggest = 0..     
+000192d0: 2020 2020 2020 2069 6620 6172 6720 3d3d         if arg ==
+000192e0: 2022 7622 3a0a 2020 2020 2020 2020 2020   "v":.          
+000192f0: 2020 2020 2020 666d 7420 3d20 225c 3033        fmt = "\03
+00019300: 335b 303b 373b 3336 6d7b 7b7d 7d7b 7b3a  3[0;7;36m{{}}{{:
+00019310: 3e7b 7d7d 7d5c 3033 335b 306d 207b 7b7d  >{}}}\033[0m {{}
+00019320: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+00019330: 2020 206e 666d 7420 3d20 227b 7d22 0a20     nfmt = "{}". 
+00019340: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00019350: 6967 6765 7374 203d 2030 0a20 2020 2020  iggest = 0.     
+00019360: 2020 2020 2020 2020 2020 2066 3220 3d20             f2 = 
+00019370: 2222 2e6a 6f69 6e28 0a20 2020 2020 2020  "".join(.       
+00019380: 2020 2020 2020 2020 2020 2020 2022 7b7d               "{}
+00019390: 7b7b 7d7d 222e 666f 726d 6174 2878 290a  {{}}".format(x).
+000193a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193b0: 2020 2020 666f 7220 7820 696e 205b 0a20      for x in [. 
+000193c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193d0: 2020 2020 2020 2022 5c30 3333 5b37 6d22         "\033[7m"
+000193e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000193f0: 2020 2020 2020 2020 2020 225c 3033 335b            "\033[
+00019400: 3237 6d22 2c0a 2020 2020 2020 2020 2020  27m",.          
+00019410: 2020 2020 2020 2020 2020 2020 2020 2222                ""
+00019420: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00019430: 2020 2020 2020 2020 2020 225c 3033 335b            "\033[
+00019440: 303b 316d 222c 0a20 2020 2020 2020 2020  0;1m",.         
+00019450: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00019460: 5c30 3333 5b30 3b33 366d 222c 0a20 2020  \033[0;36m",.   
+00019470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019480: 2020 2020 2022 5c30 3333 5b30 6d22 2c0a       "\033[0m",.
+00019490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194a0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+000194b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000194c0: 2020 2020 2020 2020 6374 6162 203d 207b          ctab = {
+000194d0: 2242 223a 2036 2c20 224b 223a 2035 2c20  "B": 6, "K": 5, 
+000194e0: 224d 223a 2031 2c20 2247 223a 2033 7d0a  "M": 1, "G": 3}.
+000194f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019500: 666f 7220 6c73 7420 696e 205b 6469 7273  for lst in [dirs
+00019510: 2c20 6669 6c65 735d 3a0a 2020 2020 2020  , files]:.      
+00019520: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00019530: 7220 7820 696e 206c 7374 3a0a 2020 2020  r x in lst:.    
 00019540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019550: 2020 785b 2264 7422 5d20 3d20 6632 2e66    x["dt"] = f2.f
-00019560: 6f72 6d61 7428 2a6c 6973 7428 6129 290a  ormat(*list(a)).
-00019570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019580: 2020 2020 2020 2020 737a 203d 2068 756d          sz = hum
-00019590: 616e 7369 7a65 2878 5b22 737a 225d 2c20  ansize(x["sz"], 
-000195a0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-000195b0: 2020 2020 2020 2020 2020 2020 2020 785b                x[
-000195c0: 2273 7a22 5d20 3d20 225c 3033 335b 303b  "sz"] = "\033[0;
-000195d0: 337b 7d6d 207b 3a3e 357d 222e 666f 726d  3{}m {:>5}".form
-000195e0: 6174 2863 7461 622e 6765 7428 737a 5b2d  at(ctab.get(sz[-
-000195f0: 313a 5d2c 2030 292c 2073 7a29 0a20 2020  1:], 0), sz).   
-00019600: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00019610: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00019620: 6d74 203d 2022 7b7b 7d7d 2020 7b7b 3a7b  mt = "{{}}  {{:{
-00019630: 7d2c 7d7d 2020 7b7b 7d7d 220a 2020 2020  },}}  {{}}".    
-00019640: 2020 2020 2020 2020 2020 2020 6e66 6d74              nfmt
-00019650: 203d 2022 7b3a 2c7d 220a 0a20 2020 2020   = "{:,}"..     
-00019660: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
-00019670: 6469 7273 3a0a 2020 2020 2020 2020 2020  dirs:.          
-00019680: 2020 2020 2020 6e20 3d20 785b 226e 616d        n = x["nam
-00019690: 6522 5d20 2b20 222f 220a 2020 2020 2020  e"] + "/".      
-000196a0: 2020 2020 2020 2020 2020 6966 2061 7267            if arg
-000196b0: 203d 3d20 2276 223a 0a20 2020 2020 2020   == "v":.       
-000196c0: 2020 2020 2020 2020 2020 2020 206e 203d               n =
-000196d0: 2022 5c30 3333 5b39 346d 2220 2b20 6e0a   "\033[94m" + n.
-000196e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000196f0: 2078 5b22 6e61 6d65 225d 203d 206e 0a0a   x["name"] = n..
-00019700: 2020 2020 2020 2020 2020 2020 666d 7420              fmt 
-00019710: 3d20 666d 742e 666f 726d 6174 286c 656e  = fmt.format(len
-00019720: 286e 666d 742e 666f 726d 6174 2862 6967  (nfmt.format(big
-00019730: 6765 7374 2929 290a 2020 2020 2020 2020  gest))).        
-00019740: 2020 2020 7265 746c 203d 205b 0a20 2020      retl = [.   
-00019750: 2020 2020 2020 2020 2020 2020 2022 2320               "# 
-00019760: 7b7d 3a20 7b7d 222e 666f 726d 6174 2878  {}: {}".format(x
-00019770: 2c20 6c73 5b78 5d29 0a20 2020 2020 2020  , ls[x]).       
-00019780: 2020 2020 2020 2020 2066 6f72 2078 2069           for x i
-00019790: 6e20 5b22 6163 6374 222c 2022 7065 726d  n ["acct", "perm
-000197a0: 7322 2c20 2273 7276 696e 6622 5d0a 2020  s", "srvinf"].  
-000197b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000197c0: 2078 2069 6e20 6c73 0a20 2020 2020 2020   x in ls.       
-000197d0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-000197e0: 2020 2072 6574 6c20 2b3d 205b 0a20 2020     retl += [.   
-000197f0: 2020 2020 2020 2020 2020 2020 2066 6d74               fmt
-00019800: 2e66 6f72 6d61 7428 785b 2264 7422 5d2c  .format(x["dt"],
-00019810: 2078 5b22 737a 225d 2c20 785b 226e 616d   x["sz"], x["nam
-00019820: 6522 5d29 0a20 2020 2020 2020 2020 2020  e"]).           
-00019830: 2020 2020 2066 6f72 2079 2069 6e20 5b64       for y in [d
-00019840: 6972 732c 2066 696c 6573 5d0a 2020 2020  irs, files].    
-00019850: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00019860: 7820 696e 2079 0a20 2020 2020 2020 2020  x in y.         
-00019870: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
-00019880: 2072 6574 203d 2022 5c6e 222e 6a6f 696e   ret = "\n".join
-00019890: 2872 6574 6c29 0a20 2020 2020 2020 2020  (retl).         
-000198a0: 2020 206d 696d 6520 3d20 2274 6578 742f     mime = "text/
-000198b0: 706c 6169 6e3b 2063 6861 7273 6574 3d75  plain; charset=u
-000198c0: 7466 2d38 220a 2020 2020 2020 2020 656c  tf-8".        el
-000198d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000198e0: 5b78 2e70 6f70 286b 2920 666f 7220 6b20  [x.pop(k) for k 
-000198f0: 696e 205b 226e 616d 6522 2c20 2264 7422  in ["name", "dt"
-00019900: 5d20 666f 7220 7920 696e 205b 6469 7273  ] for y in [dirs
-00019910: 2c20 6669 6c65 735d 2066 6f72 2078 2069  , files] for x i
-00019920: 6e20 795d 0a0a 2020 2020 2020 2020 2020  n y]..          
-00019930: 2020 7265 7420 3d20 6a73 6f6e 2e64 756d    ret = json.dum
-00019940: 7073 286c 7329 0a20 2020 2020 2020 2020  ps(ls).         
-00019950: 2020 206d 696d 6520 3d20 2261 7070 6c69     mime = "appli
-00019960: 6361 7469 6f6e 2f6a 736f 6e22 0a0a 2020  cation/json"..  
-00019970: 2020 2020 2020 7265 7420 2b3d 2022 5c6e        ret += "\n
-00019980: 5c30 3333 5b30 6d22 2069 6620 6172 6720  \033[0m" if arg 
-00019990: 3d3d 2022 7622 2065 6c73 6520 225c 6e22  == "v" else "\n"
-000199a0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-000199b0: 706c 7928 7265 742e 656e 636f 6465 2822  ply(ret.encode("
-000199c0: 7574 662d 3822 2c20 2272 6570 6c61 6365  utf-8", "replace
-000199d0: 2229 2c20 6d69 6d65 3d6d 696d 6529 0a20  "), mime=mime). 
-000199e0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000199f0: 7565 0a0a 2020 2020 6465 6620 7478 5f62  ue..    def tx_b
-00019a00: 726f 7773 6572 2873 656c 6629 2020 3a0a  rowser(self)  :.
-00019a10: 2020 2020 2020 2020 7670 6174 6820 3d20          vpath = 
-00019a20: 2222 0a20 2020 2020 2020 2076 706e 6f64  "".        vpnod
-00019a30: 6573 203d 205b 5b22 222c 2022 2f22 5d5d  es = [["", "/"]]
-00019a40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00019a50: 2e76 7061 7468 3a0a 2020 2020 2020 2020  .vpath:.        
-00019a60: 2020 2020 666f 7220 6e6f 6465 2069 6e20      for node in 
-00019a70: 7365 6c66 2e76 7061 7468 2e73 706c 6974  self.vpath.split
-00019a80: 2822 2f22 293a 0a20 2020 2020 2020 2020  ("/"):.         
-00019a90: 2020 2020 2020 2069 6620 6e6f 7420 7670         if not vp
-00019aa0: 6174 683a 0a20 2020 2020 2020 2020 2020  ath:.           
-00019ab0: 2020 2020 2020 2020 2076 7061 7468 203d           vpath =
-00019ac0: 206e 6f64 650a 2020 2020 2020 2020 2020   node.          
-00019ad0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00019ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019af0: 7670 6174 6820 2b3d 2022 2f22 202b 206e  vpath += "/" + n
-00019b00: 6f64 650a 0a20 2020 2020 2020 2020 2020  ode..           
-00019b10: 2020 2020 2076 706e 6f64 6573 2e61 7070       vpnodes.app
-00019b20: 656e 6428 5b71 756f 7465 7028 7670 6174  end([quotep(vpat
-00019b30: 6829 202b 2022 2f22 2c20 6874 6d6c 5f65  h) + "/", html_e
-00019b40: 7363 6170 6528 6e6f 6465 2c20 6372 6c66  scape(node, crlf
-00019b50: 3d54 7275 6529 5d29 0a0a 2020 2020 2020  =True)])..      
-00019b60: 2020 766e 2c20 7265 6d20 3d20 7365 6c66    vn, rem = self
-00019b70: 2e61 7372 762e 7666 732e 6765 7428 7365  .asrv.vfs.get(se
-00019b80: 6c66 2e76 7061 7468 2c20 7365 6c66 2e75  lf.vpath, self.u
-00019b90: 6e61 6d65 2c20 4661 6c73 652c 2046 616c  name, False, Fal
-00019ba0: 7365 290a 2020 2020 2020 2020 6162 7370  se).        absp
-00019bb0: 6174 6820 3d20 766e 2e64 6361 6e6f 6e69  ath = vn.dcanoni
-00019bc0: 6361 6c28 7265 6d29 0a20 2020 2020 2020  cal(rem).       
-00019bd0: 2064 6276 2c20 7672 656d 203d 2076 6e2e   dbv, vrem = vn.
-00019be0: 6765 745f 6462 7628 7265 6d29 0a0a 2020  get_dbv(rem)..  
-00019bf0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00019c00: 2020 2020 2020 2073 7420 3d20 626f 732e         st = bos.
-00019c10: 7374 6174 2861 6273 7061 7468 290a 2020  stat(abspath).  
-00019c20: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-00019c30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00019c40: 2073 656c 662e 7478 5f34 3034 2829 0a0a   self.tx_404()..
-00019c50: 2020 2020 2020 2020 6966 2072 656d 2e73          if rem.s
-00019c60: 7461 7274 7377 6974 6828 222e 6869 7374  tartswith(".hist
-00019c70: 2f75 7032 6b2e 2229 206f 7220 280a 2020  /up2k.") or (.  
-00019c80: 2020 2020 2020 2020 2020 7265 6d2e 656e            rem.en
-00019c90: 6473 7769 7468 2822 2f64 6972 2e74 7874  dswith("/dir.txt
-00019ca0: 2229 2061 6e64 2072 656d 2e73 7461 7274  ") and rem.start
-00019cb0: 7377 6974 6828 222e 6869 7374 2f74 682f  swith(".hist/th/
-00019cc0: 2229 0a20 2020 2020 2020 2029 3a0a 2020  ").        ):.  
-00019cd0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00019ce0: 5065 626b 6163 2834 3033 290a 0a20 2020  Pebkac(403)..   
-00019cf0: 2020 2020 2065 3264 203d 2022 6532 6422       e2d = "e2d"
-00019d00: 2069 6e20 766e 2e66 6c61 6773 0a20 2020   in vn.flags.   
-00019d10: 2020 2020 2065 3274 203d 2022 6532 7422       e2t = "e2t"
-00019d20: 2069 6e20 766e 2e66 6c61 6773 0a0a 2020   in vn.flags..  
-00019d30: 2020 2020 2020 7365 6c66 2e68 746d 6c5f        self.html_
-00019d40: 6865 6164 203d 2076 6e2e 666c 6167 732e  head = vn.flags.
-00019d50: 6765 7428 2268 746d 6c5f 6865 6164 222c  get("html_head",
-00019d60: 2022 2229 0a20 2020 2020 2020 2069 6620   "").        if 
-00019d70: 766e 2e66 6c61 6773 2e67 6574 2822 6e6f  vn.flags.get("no
-00019d80: 726f 626f 7473 2229 206f 7220 2262 2220  robots") or "b" 
-00019d90: 696e 2073 656c 662e 7570 6172 616d 3a0a  in self.uparam:.
-00019da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019db0: 2e6f 7574 5f68 6561 6465 7273 5b22 582d  .out_headers["X-
-00019dc0: 526f 626f 7473 2d54 6167 225d 203d 2022  Robots-Tag"] = "
-00019dd0: 6e6f 696e 6465 782c 206e 6f66 6f6c 6c6f  noindex, nofollo
-00019de0: 7722 0a20 2020 2020 2020 2065 6c73 653a  w".        else:
-00019df0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00019e00: 662e 6f75 745f 6865 6164 6572 732e 706f  f.out_headers.po
-00019e10: 7028 2258 2d52 6f62 6f74 732d 5461 6722  p("X-Robots-Tag"
-00019e20: 2c20 4e6f 6e65 290a 0a20 2020 2020 2020  , None)..       
-00019e30: 2069 735f 6469 7220 3d20 7374 6174 2e53   is_dir = stat.S
-00019e40: 5f49 5344 4952 2873 742e 7374 5f6d 6f64  _ISDIR(st.st_mod
-00019e50: 6529 0a20 2020 2020 2020 2069 6375 7220  e).        icur 
-00019e60: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-00019e70: 6620 6532 7420 6f72 2028 6532 6420 616e  f e2t or (e2d an
-00019e80: 6420 6973 5f64 6972 293a 0a20 2020 2020  d is_dir):.     
-00019e90: 2020 2020 2020 2069 6478 203d 2073 656c         idx = sel
-00019ea0: 662e 636f 6e6e 2e67 6574 5f75 3269 6478  f.conn.get_u2idx
-00019eb0: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-00019ec0: 6375 7220 3d20 6964 782e 6765 745f 6375  cur = idx.get_cu
-00019ed0: 7228 6462 762e 7265 616c 7061 7468 290a  r(dbv.realpath).
-00019ee0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00019ef0: 2e63 616e 5f72 6561 643a 0a20 2020 2020  .can_read:.     
-00019f00: 2020 2020 2020 2074 685f 666d 7420 3d20         th_fmt = 
-00019f10: 7365 6c66 2e75 7061 7261 6d2e 6765 7428  self.uparam.get(
-00019f20: 2274 6822 290a 2020 2020 2020 2020 2020  "th").          
-00019f30: 2020 6966 2074 685f 666d 7420 6973 206e    if th_fmt is n
-00019f40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00019f50: 2020 2020 2020 2020 2069 6620 6973 5f64           if is_d
-00019f60: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
-00019f70: 2020 2020 2020 2020 7672 656d 203d 2076          vrem = v
-00019f80: 7265 6d2e 7273 7472 6970 2822 2f22 290a  rem.rstrip("/").
-00019f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fa0: 2020 2020 6966 2069 6375 7220 616e 6420      if icur and 
-00019fb0: 7672 656d 3a0a 2020 2020 2020 2020 2020  vrem:.          
-00019fc0: 2020 2020 2020 2020 2020 2020 2020 7120                q 
-00019fd0: 3d20 2273 656c 6563 7420 666e 2066 726f  = "select fn fro
-00019fe0: 6d20 6376 2077 6865 7265 2072 643d 3f20  m cv where rd=? 
-00019ff0: 616e 6420 646e 3d3f 220a 2020 2020 2020  and dn=?".      
-0001a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a010: 2020 6372 642c 2063 646e 203d 2076 7265    crd, cdn = vre
-0001a020: 6d2e 7273 706c 6974 2822 2f22 2c20 3129  m.rsplit("/", 1)
-0001a030: 2069 6620 222f 2220 696e 2076 7265 6d20   if "/" in vrem 
-0001a040: 656c 7365 2028 2222 2c20 7672 656d 290a  else ("", vrem).
+00019550: 2020 2020 6120 3d20 785b 2264 7422 5d2e      a = x["dt"].
+00019560: 7265 706c 6163 6528 222d 222c 2022 2022  replace("-", " "
+00019570: 292e 7265 706c 6163 6528 223a 222c 2022  ).replace(":", "
+00019580: 2022 292e 7370 6c69 7428 2220 2229 0a20   ").split(" "). 
+00019590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195a0: 2020 2020 2020 2078 5b22 6474 225d 203d         x["dt"] =
+000195b0: 2066 322e 666f 726d 6174 282a 6c69 7374   f2.format(*list
+000195c0: 2861 2929 0a20 2020 2020 2020 2020 2020  (a)).           
+000195d0: 2020 2020 2020 2020 2020 2020 2073 7a20               sz 
+000195e0: 3d20 6875 6d61 6e73 697a 6528 785b 2273  = humansize(x["s
+000195f0: 7a22 5d2c 2054 7275 6529 0a20 2020 2020  z"], True).     
+00019600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019610: 2020 2078 5b22 737a 225d 203d 2022 5c30     x["sz"] = "\0
+00019620: 3333 5b30 3b33 7b7d 6d20 7b3a 3e35 7d22  33[0;3{}m {:>5}"
+00019630: 2e66 6f72 6d61 7428 6374 6162 2e67 6574  .format(ctab.get
+00019640: 2873 7a5b 2d31 3a5d 2c20 3029 2c20 737a  (sz[-1:], 0), sz
+00019650: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00019660: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00019670: 2020 2020 666d 7420 3d20 227b 7b7d 7d20      fmt = "{{}} 
+00019680: 207b 7b3a 7b7d 2c7d 7d20 207b 7b7d 7d22   {{:{},}}  {{}}"
+00019690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000196a0: 206e 666d 7420 3d20 227b 3a2c 7d22 0a0a   nfmt = "{:,}"..
+000196b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000196c0: 7820 696e 2064 6972 733a 0a20 2020 2020  x in dirs:.     
+000196d0: 2020 2020 2020 2020 2020 206e 203d 2078             n = x
+000196e0: 5b22 6e61 6d65 225d 202b 2022 2f22 0a20  ["name"] + "/". 
+000196f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00019700: 6620 6172 6720 3d3d 2022 7622 3a0a 2020  f arg == "v":.  
+00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019720: 2020 6e20 3d20 225c 3033 335b 3934 6d22    n = "\033[94m"
+00019730: 202b 206e 0a0a 2020 2020 2020 2020 2020   + n..          
+00019740: 2020 2020 2020 785b 226e 616d 6522 5d20        x["name"] 
+00019750: 3d20 6e0a 0a20 2020 2020 2020 2020 2020  = n..           
+00019760: 2066 6d74 203d 2066 6d74 2e66 6f72 6d61   fmt = fmt.forma
+00019770: 7428 6c65 6e28 6e66 6d74 2e66 6f72 6d61  t(len(nfmt.forma
+00019780: 7428 6269 6767 6573 7429 2929 0a20 2020  t(biggest))).   
+00019790: 2020 2020 2020 2020 2072 6574 6c20 3d20           retl = 
+000197a0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+000197b0: 2020 2223 207b 7d3a 207b 7d22 2e66 6f72    "# {}: {}".for
+000197c0: 6d61 7428 782c 206c 735b 785d 290a 2020  mat(x, ls[x]).  
+000197d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000197e0: 7220 7820 696e 205b 2261 6363 7422 2c20  r x in ["acct", 
+000197f0: 2270 6572 6d73 222c 2022 7372 7669 6e66  "perms", "srvinf
+00019800: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00019810: 2020 2069 6620 7820 696e 206c 730a 2020     if x in ls.  
+00019820: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00019830: 2020 2020 2020 2020 7265 746c 202b 3d20          retl += 
+00019840: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00019850: 2020 666d 742e 666f 726d 6174 2878 5b22    fmt.format(x["
+00019860: 6474 225d 2c20 785b 2273 7a22 5d2c 2078  dt"], x["sz"], x
+00019870: 5b22 6e61 6d65 225d 290a 2020 2020 2020  ["name"]).      
+00019880: 2020 2020 2020 2020 2020 666f 7220 7920            for y 
+00019890: 696e 205b 6469 7273 2c20 6669 6c65 735d  in [dirs, files]
+000198a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000198b0: 2066 6f72 2078 2069 6e20 790a 2020 2020   for x in y.    
+000198c0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+000198d0: 2020 2020 2020 7265 7420 3d20 225c 6e22        ret = "\n"
+000198e0: 2e6a 6f69 6e28 7265 746c 290a 2020 2020  .join(retl).    
+000198f0: 2020 2020 2020 2020 6d69 6d65 203d 2022          mime = "
+00019900: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
+00019910: 7365 743d 7574 662d 3822 0a20 2020 2020  set=utf-8".     
+00019920: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00019930: 2020 2020 205b 782e 706f 7028 6b29 2066       [x.pop(k) f
+00019940: 6f72 206b 2069 6e20 5b22 6e61 6d65 222c  or k in ["name",
+00019950: 2022 6474 225d 2066 6f72 2079 2069 6e20   "dt"] for y in 
+00019960: 5b64 6972 732c 2066 696c 6573 5d20 666f  [dirs, files] fo
+00019970: 7220 7820 696e 2079 5d0a 0a20 2020 2020  r x in y]..     
+00019980: 2020 2020 2020 2072 6574 203d 206a 736f         ret = jso
+00019990: 6e2e 6475 6d70 7328 6c73 290a 2020 2020  n.dumps(ls).    
+000199a0: 2020 2020 2020 2020 6d69 6d65 203d 2022          mime = "
+000199b0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+000199c0: 220a 0a20 2020 2020 2020 2072 6574 202b  "..        ret +
+000199d0: 3d20 225c 6e5c 3033 335b 306d 2220 6966  = "\n\033[0m" if
+000199e0: 2061 7267 203d 3d20 2276 2220 656c 7365   arg == "v" else
+000199f0: 2022 5c6e 220a 2020 2020 2020 2020 7365   "\n".        se
+00019a00: 6c66 2e72 6570 6c79 2872 6574 2e65 6e63  lf.reply(ret.enc
+00019a10: 6f64 6528 2275 7466 2d38 222c 2022 7265  ode("utf-8", "re
+00019a20: 706c 6163 6522 292c 206d 696d 653d 6d69  place"), mime=mi
+00019a30: 6d65 290a 2020 2020 2020 2020 7265 7475  me).        retu
+00019a40: 726e 2054 7275 650a 0a20 2020 2064 6566  rn True..    def
+00019a50: 2074 785f 6272 6f77 7365 7228 7365 6c66   tx_browser(self
+00019a60: 2920 203a 0a20 2020 2020 2020 2076 7061  )  :.        vpa
+00019a70: 7468 203d 2022 220a 2020 2020 2020 2020  th = "".        
+00019a80: 7670 6e6f 6465 7320 3d20 5b5b 2222 2c20  vpnodes = [["", 
+00019a90: 222f 225d 5d0a 2020 2020 2020 2020 6966  "/"]].        if
+00019aa0: 2073 656c 662e 7670 6174 683a 0a20 2020   self.vpath:.   
+00019ab0: 2020 2020 2020 2020 2066 6f72 206e 6f64           for nod
+00019ac0: 6520 696e 2073 656c 662e 7670 6174 682e  e in self.vpath.
+00019ad0: 7370 6c69 7428 222f 2229 3a0a 2020 2020  split("/"):.    
+00019ae0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00019af0: 6f74 2076 7061 7468 3a0a 2020 2020 2020  ot vpath:.      
+00019b00: 2020 2020 2020 2020 2020 2020 2020 7670                vp
+00019b10: 6174 6820 3d20 6e6f 6465 0a20 2020 2020  ath = node.     
+00019b20: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00019b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019b40: 2020 2020 2076 7061 7468 202b 3d20 222f       vpath += "/
+00019b50: 2220 2b20 6e6f 6465 0a0a 2020 2020 2020  " + node..      
+00019b60: 2020 2020 2020 2020 2020 7670 6e6f 6465            vpnode
+00019b70: 732e 6170 7065 6e64 285b 7175 6f74 6570  s.append([quotep
+00019b80: 2876 7061 7468 2920 2b20 222f 222c 2068  (vpath) + "/", h
+00019b90: 746d 6c5f 6573 6361 7065 286e 6f64 652c  tml_escape(node,
+00019ba0: 2063 726c 663d 5472 7565 295d 290a 0a20   crlf=True)]).. 
+00019bb0: 2020 2020 2020 2076 6e2c 2072 656d 203d         vn, rem =
+00019bc0: 2073 656c 662e 6173 7276 2e76 6673 2e67   self.asrv.vfs.g
+00019bd0: 6574 2873 656c 662e 7670 6174 682c 2073  et(self.vpath, s
+00019be0: 656c 662e 756e 616d 652c 2046 616c 7365  elf.uname, False
+00019bf0: 2c20 4661 6c73 6529 0a20 2020 2020 2020  , False).       
+00019c00: 2061 6273 7061 7468 203d 2076 6e2e 6463   abspath = vn.dc
+00019c10: 616e 6f6e 6963 616c 2872 656d 290a 2020  anonical(rem).  
+00019c20: 2020 2020 2020 6462 762c 2076 7265 6d20        dbv, vrem 
+00019c30: 3d20 766e 2e67 6574 5f64 6276 2872 656d  = vn.get_dbv(rem
+00019c40: 290a 0a20 2020 2020 2020 2074 7279 3a0a  )..        try:.
+00019c50: 2020 2020 2020 2020 2020 2020 7374 203d              st =
+00019c60: 2062 6f73 2e73 7461 7428 6162 7370 6174   bos.stat(abspat
+00019c70: 6829 0a20 2020 2020 2020 2065 7863 6570  h).        excep
+00019c80: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+00019c90: 6574 7572 6e20 7365 6c66 2e74 785f 3430  eturn self.tx_40
+00019ca0: 3428 290a 0a20 2020 2020 2020 2069 6620  4()..        if 
+00019cb0: 7265 6d2e 7374 6172 7473 7769 7468 2822  rem.startswith("
+00019cc0: 2e68 6973 742f 7570 326b 2e22 2920 6f72  .hist/up2k.") or
+00019cd0: 2028 0a20 2020 2020 2020 2020 2020 2072   (.            r
+00019ce0: 656d 2e65 6e64 7377 6974 6828 222f 6469  em.endswith("/di
+00019cf0: 722e 7478 7422 2920 616e 6420 7265 6d2e  r.txt") and rem.
+00019d00: 7374 6172 7473 7769 7468 2822 2e68 6973  startswith(".his
+00019d10: 742f 7468 2f22 290a 2020 2020 2020 2020  t/th/").        
+00019d20: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00019d30: 6169 7365 2050 6562 6b61 6328 3430 3329  aise Pebkac(403)
+00019d40: 0a0a 2020 2020 2020 2020 6532 6420 3d20  ..        e2d = 
+00019d50: 2265 3264 2220 696e 2076 6e2e 666c 6167  "e2d" in vn.flag
+00019d60: 730a 2020 2020 2020 2020 6532 7420 3d20  s.        e2t = 
+00019d70: 2265 3274 2220 696e 2076 6e2e 666c 6167  "e2t" in vn.flag
+00019d80: 730a 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+00019d90: 6874 6d6c 5f68 6561 6420 3d20 766e 2e66  html_head = vn.f
+00019da0: 6c61 6773 2e67 6574 2822 6874 6d6c 5f68  lags.get("html_h
+00019db0: 6561 6422 2c20 2222 290a 2020 2020 2020  ead", "").      
+00019dc0: 2020 6966 2076 6e2e 666c 6167 732e 6765    if vn.flags.ge
+00019dd0: 7428 226e 6f72 6f62 6f74 7322 2920 6f72  t("norobots") or
+00019de0: 2022 6222 2069 6e20 7365 6c66 2e75 7061   "b" in self.upa
+00019df0: 7261 6d3a 0a20 2020 2020 2020 2020 2020  ram:.           
+00019e00: 2073 656c 662e 6f75 745f 6865 6164 6572   self.out_header
+00019e10: 735b 2258 2d52 6f62 6f74 732d 5461 6722  s["X-Robots-Tag"
+00019e20: 5d20 3d20 226e 6f69 6e64 6578 2c20 6e6f  ] = "noindex, no
+00019e30: 666f 6c6c 6f77 220a 2020 2020 2020 2020  follow".        
+00019e40: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00019e50: 2020 7365 6c66 2e6f 7574 5f68 6561 6465    self.out_heade
+00019e60: 7273 2e70 6f70 2822 582d 526f 626f 7473  rs.pop("X-Robots
+00019e70: 2d54 6167 222c 204e 6f6e 6529 0a0a 2020  -Tag", None)..  
+00019e80: 2020 2020 2020 6973 5f64 6972 203d 2073        is_dir = s
+00019e90: 7461 742e 535f 4953 4449 5228 7374 2e73  tat.S_ISDIR(st.s
+00019ea0: 745f 6d6f 6465 290a 2020 2020 2020 2020  t_mode).        
+00019eb0: 6963 7572 203d 204e 6f6e 650a 2020 2020  icur = None.    
+00019ec0: 2020 2020 6966 2065 3274 206f 7220 2865      if e2t or (e
+00019ed0: 3264 2061 6e64 2069 735f 6469 7229 3a0a  2d and is_dir):.
+00019ee0: 2020 2020 2020 2020 2020 2020 6964 7820              idx 
+00019ef0: 3d20 7365 6c66 2e63 6f6e 6e2e 6765 745f  = self.conn.get_
+00019f00: 7532 6964 7828 290a 2020 2020 2020 2020  u2idx().        
+00019f10: 2020 2020 6963 7572 203d 2069 6478 2e67      icur = idx.g
+00019f20: 6574 5f63 7572 2864 6276 2e72 6561 6c70  et_cur(dbv.realp
+00019f30: 6174 6829 0a0a 2020 2020 2020 2020 6966  ath)..        if
+00019f40: 2073 656c 662e 6361 6e5f 7265 6164 3a0a   self.can_read:.
+00019f50: 2020 2020 2020 2020 2020 2020 7468 5f66              th_f
+00019f60: 6d74 203d 2073 656c 662e 7570 6172 616d  mt = self.uparam
+00019f70: 2e67 6574 2822 7468 2229 0a20 2020 2020  .get("th").     
+00019f80: 2020 2020 2020 2069 6620 7468 5f66 6d74         if th_fmt
+00019f90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00019fa0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00019fb0: 2069 735f 6469 723a 0a20 2020 2020 2020   is_dir:.       
+00019fc0: 2020 2020 2020 2020 2020 2020 2076 7265               vre
+00019fd0: 6d20 3d20 7672 656d 2e72 7374 7269 7028  m = vrem.rstrip(
+00019fe0: 222f 2229 0a20 2020 2020 2020 2020 2020  "/").           
+00019ff0: 2020 2020 2020 2020 2069 6620 6963 7572           if icur
+0001a000: 2061 6e64 2076 7265 6d3a 0a20 2020 2020   and vrem:.     
+0001a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a020: 2020 2071 203d 2022 7365 6c65 6374 2066     q = "select f
+0001a030: 6e20 6672 6f6d 2063 7620 7768 6572 6520  n from cv where 
+0001a040: 7264 3d3f 2061 6e64 2064 6e3d 3f22 0a20  rd=? and dn=?". 
 0001a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a060: 2020 2020 2020 2020 2320 6e6f 206d 6f6a          # no moj
-0001a070: 6962 616b 6520 7375 7070 6f72 743a 0a20  ibake support:. 
-0001a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a090: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0001a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a0b0: 2020 2020 2020 2020 6366 6e20 3d20 6963          cfn = ic
-0001a0c0: 7572 2e65 7865 6375 7465 2871 2c20 2863  ur.execute(q, (c
-0001a0d0: 7264 2c20 6364 6e29 292e 6665 7463 686f  rd, cdn)).fetcho
-0001a0e0: 6e65 2829 0a20 2020 2020 2020 2020 2020  ne().           
-0001a0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a100: 2069 6620 6366 6e3a 0a20 2020 2020 2020   if cfn:.       
-0001a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a120: 2020 2020 2020 2020 2066 6e20 3d20 6366           fn = cf
-0001a130: 6e5b 305d 0a20 2020 2020 2020 2020 2020  n[0].           
+0001a060: 2020 2020 2020 2063 7264 2c20 6364 6e20         crd, cdn 
+0001a070: 3d20 7672 656d 2e72 7370 6c69 7428 222f  = vrem.rsplit("/
+0001a080: 222c 2031 2920 6966 2022 2f22 2069 6e20  ", 1) if "/" in 
+0001a090: 7672 656d 2065 6c73 6520 2822 222c 2076  vrem else ("", v
+0001a0a0: 7265 6d29 0a20 2020 2020 2020 2020 2020  rem).           
+0001a0b0: 2020 2020 2020 2020 2020 2020 2023 206e               # n
+0001a0c0: 6f20 6d6f 6a69 6261 6b65 2073 7570 706f  o mojibake suppo
+0001a0d0: 7274 3a0a 2020 2020 2020 2020 2020 2020  rt:.            
+0001a0e0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0001a0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a100: 2020 2020 2020 2020 2020 2020 2063 666e               cfn
+0001a110: 203d 2069 6375 722e 6578 6563 7574 6528   = icur.execute(
+0001a120: 712c 2028 6372 642c 2063 646e 2929 2e66  q, (crd, cdn)).f
+0001a130: 6574 6368 6f6e 6528 290a 2020 2020 2020  etchone().      
 0001a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a150: 2020 2020 2066 7020 3d20 6f73 2e70 6174       fp = os.pat
-0001a160: 682e 6a6f 696e 2861 6273 7061 7468 2c20  h.join(abspath, 
-0001a170: 666e 290a 2020 2020 2020 2020 2020 2020  fn).            
-0001a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a190: 2020 2020 6966 2062 6f73 2e70 6174 682e      if bos.path.
-0001a1a0: 6578 6973 7473 2866 7029 3a0a 2020 2020  exists(fp):.    
-0001a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1d0: 7672 656d 203d 2022 7b7d 2f7b 7d22 2e66  vrem = "{}/{}".f
-0001a1e0: 6f72 6d61 7428 7672 656d 2c20 666e 292e  ormat(vrem, fn).
-0001a1f0: 7374 7269 7028 222f 2229 0a20 2020 2020  strip("/").     
-0001a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a210: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001a220: 735f 6469 7220 3d20 4661 6c73 650a 2020  s_dir = False.  
-0001a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a240: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+0001a150: 2020 2020 2020 6966 2063 666e 3a0a 2020        if cfn:.  
+0001a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a170: 2020 2020 2020 2020 2020 2020 2020 666e                fn
+0001a180: 203d 2063 666e 5b30 5d0a 2020 2020 2020   = cfn[0].      
+0001a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1a0: 2020 2020 2020 2020 2020 6670 203d 206f            fp = o
+0001a1b0: 732e 7061 7468 2e6a 6f69 6e28 6162 7370  s.path.join(absp
+0001a1c0: 6174 682c 2066 6e29 0a20 2020 2020 2020  ath, fn).       
+0001a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1e0: 2020 2020 2020 2020 2069 6620 626f 732e           if bos.
+0001a1f0: 7061 7468 2e65 7869 7374 7328 6670 293a  path.exists(fp):
+0001a200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a220: 2020 2020 2076 7265 6d20 3d20 227b 7d2f       vrem = "{}/
+0001a230: 7b7d 222e 666f 726d 6174 2876 7265 6d2c  {}".format(vrem,
+0001a240: 2066 6e29 2e73 7472 6970 2822 2f22 290a   fn).strip("/").
 0001a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a260: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
-0001a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a280: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2a0: 2066 6f72 2066 6e20 696e 2073 656c 662e   for fn in self.
-0001a2b0: 6172 6773 2e74 685f 636f 7665 7273 3a0a  args.th_covers:.
-0001a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2d0: 2020 2020 2020 2020 2020 2020 6670 203d              fp =
-0001a2e0: 206f 732e 7061 7468 2e6a 6f69 6e28 6162   os.path.join(ab
-0001a2f0: 7370 6174 682c 2066 6e29 0a20 2020 2020  spath, fn).     
-0001a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a310: 2020 2020 2020 2069 6620 626f 732e 7061         if bos.pa
-0001a320: 7468 2e65 7869 7374 7328 6670 293a 0a20  th.exists(fp):. 
-0001a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a340: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0001a350: 7265 6d20 3d20 227b 7d2f 7b7d 222e 666f  rem = "{}/{}".fo
-0001a360: 726d 6174 2876 7265 6d2c 2066 6e29 2e73  rmat(vrem, fn).s
-0001a370: 7472 6970 2822 2f22 290a 2020 2020 2020  trip("/").      
-0001a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a390: 2020 2020 2020 2020 2020 6973 5f64 6972            is_dir
-0001a3a0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-0001a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3c0: 2020 2020 2020 2020 2062 7265 616b 0a0a           break..
+0001a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a270: 2020 2020 6973 5f64 6972 203d 2046 616c      is_dir = Fal
+0001a280: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+0001a290: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0001a2a0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0001a2b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001a2c0: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+0001a2d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2f0: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
+0001a300: 7365 6c66 2e61 7267 732e 7468 5f63 6f76  self.args.th_cov
+0001a310: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+0001a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a330: 2066 7020 3d20 6f73 2e70 6174 682e 6a6f   fp = os.path.jo
+0001a340: 696e 2861 6273 7061 7468 2c20 666e 290a  in(abspath, fn).
+0001a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a360: 2020 2020 2020 2020 2020 2020 6966 2062              if b
+0001a370: 6f73 2e70 6174 682e 6578 6973 7473 2866  os.path.exists(f
+0001a380: 7029 3a0a 2020 2020 2020 2020 2020 2020  p):.            
+0001a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3a0: 2020 2020 7672 656d 203d 2022 7b7d 2f7b      vrem = "{}/{
+0001a3b0: 7d22 2e66 6f72 6d61 7428 7672 656d 2c20  }".format(vrem, 
+0001a3c0: 666e 292e 7374 7269 7028 222f 2229 0a20  fn).strip("/"). 
 0001a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3e0: 2020 2020 6966 2069 735f 6469 723a 0a20      if is_dir:. 
-0001a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a400: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001a410: 6c66 2e74 785f 6963 6f28 2261 2e66 6f6c  lf.tx_ico("a.fol
-0001a420: 6465 7222 290a 0a20 2020 2020 2020 2020  der")..         
-0001a430: 2020 2020 2020 2074 6870 203d 204e 6f6e         thp = Non
-0001a440: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0001a450: 2020 6966 2073 656c 662e 7468 756d 6263    if self.thumbc
-0001a460: 6c69 3a0a 2020 2020 2020 2020 2020 2020  li:.            
-0001a470: 2020 2020 2020 2020 7468 7020 3d20 7365          thp = se
-0001a480: 6c66 2e74 6875 6d62 636c 692e 6765 7428  lf.thumbcli.get(
-0001a490: 6462 762c 2076 7265 6d2c 2069 6e74 2873  dbv, vrem, int(s
-0001a4a0: 742e 7374 5f6d 7469 6d65 292c 2074 685f  t.st_mtime), th_
-0001a4b0: 666d 7429 0a0a 2020 2020 2020 2020 2020  fmt)..          
-0001a4c0: 2020 2020 2020 6966 2074 6870 3a0a 2020        if thp:.  
-0001a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4e0: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
-0001a4f0: 5f66 696c 6528 7468 7029 0a0a 2020 2020  _file(thp)..    
-0001a500: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-0001a510: 685f 666d 7420 3d3d 2022 7022 3a0a 2020  h_fmt == "p":.  
-0001a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a530: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
-0001a540: 3034 290a 0a20 2020 2020 2020 2020 2020  04)..           
-0001a550: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001a560: 2e74 785f 6963 6f28 7265 6d29 0a0a 2020  .tx_ico(rem)..  
-0001a570: 2020 2020 2020 6966 206e 6f74 2069 735f        if not is_
-0001a580: 6469 7220 616e 6420 2873 656c 662e 6361  dir and (self.ca
-0001a590: 6e5f 7265 6164 206f 7220 7365 6c66 2e63  n_read or self.c
-0001a5a0: 616e 5f67 6574 293a 0a20 2020 2020 2020  an_get):.       
-0001a5b0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-0001a5c0: 2e63 616e 5f72 6561 6420 616e 6420 2266  .can_read and "f
-0001a5d0: 6b22 2069 6e20 766e 2e66 6c61 6773 3a0a  k" in vn.flags:.
-0001a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5f0: 636f 7272 6563 7420 3d20 7365 6c66 2e67  correct = self.g
-0001a600: 656e 5f66 6b28 0a20 2020 2020 2020 2020  en_fk(.         
-0001a610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a620: 6172 6773 2e66 6b5f 7361 6c74 2c20 6162  args.fk_salt, ab
-0001a630: 7370 6174 682c 2073 742e 7374 5f73 697a  spath, st.st_siz
-0001a640: 652c 2030 2069 6620 414e 5957 494e 2065  e, 0 if ANYWIN e
-0001a650: 6c73 6520 7374 2e73 745f 696e 6f0a 2020  lse st.st_ino.  
-0001a660: 2020 2020 2020 2020 2020 2020 2020 295b                )[
-0001a670: 3a20 766e 2e66 6c61 6773 5b22 666b 225d  : vn.flags["fk"]
-0001a680: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001a690: 2020 676f 7420 3d20 7365 6c66 2e75 7061    got = self.upa
-0001a6a0: 7261 6d2e 6765 7428 226b 2229 0a20 2020  ram.get("k").   
-0001a6b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001a6c0: 676f 7420 213d 2063 6f72 7265 6374 3a0a  got != correct:.
-0001a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6e0: 2020 2020 7365 6c66 2e6c 6f67 2822 7772      self.log("wr
-0001a6f0: 6f6e 6720 6669 6c65 6b65 792c 2077 616e  ong filekey, wan
-0001a700: 7420 7b7d 2c20 676f 7420 7b7d 222e 666f  t {}, got {}".fo
-0001a710: 726d 6174 2863 6f72 7265 6374 2c20 676f  rmat(correct, go
-0001a720: 7429 290a 2020 2020 2020 2020 2020 2020  t)).            
-0001a730: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001a740: 656c 662e 7478 5f34 3034 2829 0a0a 2020  elf.tx_404()..  
-0001a750: 2020 2020 2020 2020 2020 6966 2061 6273            if abs
-0001a760: 7061 7468 2e65 6e64 7377 6974 6828 222e  path.endswith(".
-0001a770: 6d64 2229 2061 6e64 2028 0a20 2020 2020  md") and (.     
-0001a780: 2020 2020 2020 2020 2020 2022 7622 2069             "v" i
-0001a790: 6e20 7365 6c66 2e75 7061 7261 6d20 6f72  n self.uparam or
-0001a7a0: 2022 6564 6974 2220 696e 2073 656c 662e   "edit" in self.
-0001a7b0: 7570 6172 616d 206f 7220 2265 6469 7432  uparam or "edit2
-0001a7c0: 2220 696e 2073 656c 662e 7570 6172 616d  " in self.uparam
-0001a7d0: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
-0001a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7f0: 7265 7475 726e 2073 656c 662e 7478 5f6d  return self.tx_m
-0001a800: 6428 6162 7370 6174 6829 0a0a 2020 2020  d(abspath)..    
-0001a810: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001a820: 656c 662e 7478 5f66 696c 6528 6162 7370  elf.tx_file(absp
-0001a830: 6174 6829 0a0a 2020 2020 2020 2020 656c  ath)..        el
-0001a840: 6966 2069 735f 6469 7220 616e 6420 6e6f  if is_dir and no
-0001a850: 7420 7365 6c66 2e63 616e 5f72 6561 6420  t self.can_read 
-0001a860: 616e 6420 6e6f 7420 7365 6c66 2e63 616e  and not self.can
-0001a870: 5f77 7269 7465 3a0a 2020 2020 2020 2020  _write:.        
-0001a880: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001a890: 7478 5f34 3034 2854 7275 6529 0a0a 2020  tx_404(True)..  
-0001a8a0: 2020 2020 2020 7372 765f 696e 666f 203d        srv_info =
-0001a8b0: 205b 5d0a 0a20 2020 2020 2020 2074 7279   []..        try
-0001a8c0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0001a8d0: 206e 6f74 2073 656c 662e 6172 6773 2e6e   not self.args.n
-0001a8e0: 6968 3a0a 2020 2020 2020 2020 2020 2020  ih:.            
-0001a8f0: 2020 2020 7372 765f 696e 666f 2e61 7070      srv_info.app
-0001a900: 656e 6428 7365 6c66 2e61 7267 732e 6e61  end(self.args.na
-0001a910: 6d65 290a 2020 2020 2020 2020 6578 6365  me).        exce
-0001a920: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-0001a930: 7365 6c66 2e6c 6f67 2822 2377 6f77 2023  self.log("#wow #
-0001a940: 7768 6f61 2229 0a0a 2020 2020 2020 2020  whoa")..        
-0001a950: 6966 206e 6f74 2073 656c 662e 6172 6773  if not self.args
-0001a960: 2e6e 6964 3a0a 2020 2020 2020 2020 2020  .nid:.          
-0001a970: 2020 6672 6565 2c20 746f 7461 6c20 3d20    free, total = 
-0001a980: 6765 745f 6466 2861 6273 7061 7468 290a  get_df(abspath).
-0001a990: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-0001a9a0: 6f74 616c 2069 7320 6e6f 7420 4e6f 6e65  otal is not None
-0001a9b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001a9c0: 2020 6831 203d 2068 756d 616e 7369 7a65    h1 = humansize
-0001a9d0: 2866 7265 6520 6f72 2030 290a 2020 2020  (free or 0).    
-0001a9e0: 2020 2020 2020 2020 2020 2020 6832 203d              h2 =
-0001a9f0: 2068 756d 616e 7369 7a65 2874 6f74 616c   humansize(total
-0001aa00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001aa10: 2020 7372 765f 696e 666f 2e61 7070 656e    srv_info.appen
-0001aa20: 6428 227b 7d20 6672 6565 206f 6620 7b7d  d("{} free of {}
-0001aa30: 222e 666f 726d 6174 2868 312c 2068 3229  ".format(h1, h2)
-0001aa40: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0001aa50: 6966 2066 7265 6520 6973 206e 6f74 204e  if free is not N
-0001aa60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001aa70: 2020 2020 2073 7276 5f69 6e66 6f2e 6170       srv_info.ap
-0001aa80: 7065 6e64 2868 756d 616e 7369 7a65 2866  pend(humansize(f
-0001aa90: 7265 652c 2054 7275 6529 202b 2022 2066  ree, True) + " f
-0001aaa0: 7265 6522 290a 0a20 2020 2020 2020 2073  ree")..        s
-0001aab0: 7276 5f69 6e66 6f74 203d 2022 3c2f 7370  rv_infot = "</sp
-0001aac0: 616e 3e20 2f2f 203c 7370 616e 3e22 2e6a  an> // <span>".j
-0001aad0: 6f69 6e28 7372 765f 696e 666f 290a 0a20  oin(srv_info).. 
-0001aae0: 2020 2020 2020 2070 6572 6d73 203d 205b         perms = [
-0001aaf0: 5d0a 2020 2020 2020 2020 6966 2073 656c  ].        if sel
-0001ab00: 662e 6361 6e5f 7265 6164 3a0a 2020 2020  f.can_read:.    
-0001ab10: 2020 2020 2020 2020 7065 726d 732e 6170          perms.ap
-0001ab20: 7065 6e64 2822 7265 6164 2229 0a20 2020  pend("read").   
-0001ab30: 2020 2020 2069 6620 7365 6c66 2e63 616e       if self.can
-0001ab40: 5f77 7269 7465 3a0a 2020 2020 2020 2020  _write:.        
-0001ab50: 2020 2020 7065 726d 732e 6170 7065 6e64      perms.append
-0001ab60: 2822 7772 6974 6522 290a 2020 2020 2020  ("write").      
-0001ab70: 2020 6966 2073 656c 662e 6361 6e5f 6d6f    if self.can_mo
-0001ab80: 7665 3a0a 2020 2020 2020 2020 2020 2020  ve:.            
-0001ab90: 7065 726d 732e 6170 7065 6e64 2822 6d6f  perms.append("mo
-0001aba0: 7665 2229 0a20 2020 2020 2020 2069 6620  ve").        if 
-0001abb0: 7365 6c66 2e63 616e 5f64 656c 6574 653a  self.can_delete:
-0001abc0: 0a20 2020 2020 2020 2020 2020 2070 6572  .            per
-0001abd0: 6d73 2e61 7070 656e 6428 2264 656c 6574  ms.append("delet
-0001abe0: 6522 290a 2020 2020 2020 2020 6966 2073  e").        if s
-0001abf0: 656c 662e 6361 6e5f 6765 743a 0a20 2020  elf.can_get:.   
-0001ac00: 2020 2020 2020 2020 2070 6572 6d73 2e61           perms.a
-0001ac10: 7070 656e 6428 2267 6574 2229 0a20 2020  ppend("get").   
-0001ac20: 2020 2020 2069 6620 7365 6c66 2e63 616e       if self.can
-0001ac30: 5f75 7067 6574 3a0a 2020 2020 2020 2020  _upget:.        
-0001ac40: 2020 2020 7065 726d 732e 6170 7065 6e64      perms.append
-0001ac50: 2822 7570 6765 7422 290a 0a20 2020 2020  ("upget")..     
-0001ac60: 2020 2075 726c 5f73 7566 203d 2073 656c     url_suf = sel
-0001ac70: 662e 7572 6c71 287b 7d2c 205b 226b 225d  f.urlq({}, ["k"]
-0001ac80: 290a 2020 2020 2020 2020 6973 5f6c 7320  ).        is_ls 
-0001ac90: 3d20 226c 7322 2069 6e20 7365 6c66 2e75  = "ls" in self.u
-0001aca0: 7061 7261 6d0a 2020 2020 2020 2020 6973  param.        is
-0001acb0: 5f6a 7320 3d20 7365 6c66 2e61 7267 732e  _js = self.args.
-0001acc0: 666f 7263 655f 6a73 206f 7220 7365 6c66  force_js or self
-0001acd0: 2e63 6f6f 6b69 6573 2e67 6574 2822 6a73  .cookies.get("js
-0001ace0: 2229 203d 3d20 2279 220a 0a20 2020 2020  ") == "y"..     
-0001acf0: 2020 2069 6620 6e6f 7420 6973 5f6c 7320     if not is_ls 
-0001ad00: 616e 6420 2873 656c 662e 7561 2e73 7461  and (self.ua.sta
-0001ad10: 7274 7377 6974 6828 2263 7572 6c2f 2229  rtswith("curl/")
-0001ad20: 206f 7220 7365 6c66 2e75 612e 7374 6172   or self.ua.star
-0001ad30: 7473 7769 7468 2822 6665 7463 6822 2929  tswith("fetch"))
-0001ad40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0001ad50: 6c66 2e75 7061 7261 6d5b 226c 7322 5d20  lf.uparam["ls"] 
-0001ad60: 3d20 2276 220a 2020 2020 2020 2020 2020  = "v".          
-0001ad70: 2020 6973 5f6c 7320 3d20 5472 7565 0a0a    is_ls = True..
-0001ad80: 2020 2020 2020 2020 7470 6c20 3d20 2262          tpl = "b
-0001ad90: 726f 7773 6572 220a 2020 2020 2020 2020  rowser".        
-0001ada0: 6966 2022 6222 2069 6e20 7365 6c66 2e75  if "b" in self.u
-0001adb0: 7061 7261 6d3a 0a20 2020 2020 2020 2020  param:.         
-0001adc0: 2020 2074 706c 203d 2022 6272 6f77 7365     tpl = "browse
-0001add0: 7232 220a 2020 2020 2020 2020 2020 2020  r2".            
-0001ade0: 6973 5f6a 7320 3d20 4661 6c73 650a 0a20  is_js = False.. 
-0001adf0: 2020 2020 2020 206c 6f67 7565 7320 3d20         logues = 
-0001ae00: 5b22 222c 2022 225d 0a20 2020 2020 2020  ["", ""].       
-0001ae10: 2069 6620 6e6f 7420 7365 6c66 2e61 7267   if not self.arg
-0001ae20: 732e 6e6f 5f6c 6f67 7565 733a 0a20 2020  s.no_logues:.   
-0001ae30: 2020 2020 2020 2020 2066 6f72 206e 2c20           for n, 
-0001ae40: 666e 2069 6e20 656e 756d 6572 6174 6528  fn in enumerate(
-0001ae50: 5b22 2e70 726f 6c6f 6775 652e 6874 6d6c  [".prologue.html
-0001ae60: 222c 2022 2e65 7069 6c6f 6775 652e 6874  ", ".epilogue.ht
-0001ae70: 6d6c 225d 293a 0a20 2020 2020 2020 2020  ml"]):.         
-0001ae80: 2020 2020 2020 2066 6e20 3d20 6f73 2e70         fn = os.p
-0001ae90: 6174 682e 6a6f 696e 2861 6273 7061 7468  ath.join(abspath
-0001aea0: 2c20 666e 290a 2020 2020 2020 2020 2020  , fn).          
-0001aeb0: 2020 2020 2020 6966 2062 6f73 2e70 6174        if bos.pat
-0001aec0: 682e 6578 6973 7473 2866 6e29 3a0a 2020  h.exists(fn):.  
-0001aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aee0: 2020 7769 7468 206f 7065 6e28 6673 656e    with open(fsen
-0001aef0: 6328 666e 292c 2022 7262 2229 2061 7320  c(fn), "rb") as 
-0001af00: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-0001af10: 2020 2020 2020 2020 2020 206c 6f67 7565             logue
-0001af20: 735b 6e5d 203d 2066 2e72 6561 6428 292e  s[n] = f.read().
-0001af30: 6465 636f 6465 2822 7574 662d 3822 290a  decode("utf-8").
-0001af40: 0a20 2020 2020 2020 2072 6561 646d 6520  .        readme 
-0001af50: 3d20 2222 0a20 2020 2020 2020 2069 6620  = "".        if 
-0001af60: 6e6f 7420 7365 6c66 2e61 7267 732e 6e6f  not self.args.no
-0001af70: 5f72 6561 646d 6520 616e 6420 6e6f 7420  _readme and not 
-0001af80: 6c6f 6775 6573 5b31 5d3a 0a20 2020 2020  logues[1]:.     
-0001af90: 2020 2020 2020 2066 6f72 2066 6e20 696e         for fn in
-0001afa0: 205b 2252 4541 444d 452e 6d64 222c 2022   ["README.md", "
-0001afb0: 7265 6164 6d65 2e6d 6422 5d3a 0a20 2020  readme.md"]:.   
-0001afc0: 2020 2020 2020 2020 2020 2020 2066 6e20               fn 
-0001afd0: 3d20 6f73 2e70 6174 682e 6a6f 696e 2861  = os.path.join(a
-0001afe0: 6273 7061 7468 2c20 666e 290a 2020 2020  bspath, fn).    
-0001aff0: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0001b000: 6f73 2e70 6174 682e 6973 6669 6c65 2866  os.path.isfile(f
-0001b010: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-0001b020: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-0001b030: 6e28 6673 656e 6328 666e 292c 2022 7262  n(fsenc(fn), "rb
-0001b040: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
-0001b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b060: 2072 6561 646d 6520 3d20 662e 7265 6164   readme = f.read
-0001b070: 2829 2e64 6563 6f64 6528 2275 7466 2d38  ().decode("utf-8
-0001b080: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0001b090: 2020 2020 2020 2020 2020 2062 7265 616b             break
-0001b0a0: 0a0a 2020 2020 2020 2020 7666 203d 2076  ..        vf = v
-0001b0b0: 6e2e 666c 6167 730a 2020 2020 2020 2020  n.flags.        
-0001b0c0: 6c73 5f72 6574 203d 207b 0a20 2020 2020  ls_ret = {.     
-0001b0d0: 2020 2020 2020 2022 6469 7273 223a 205b         "dirs": [
-0001b0e0: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
-0001b0f0: 6669 6c65 7322 3a20 5b5d 2c0a 2020 2020  files": [],.    
-0001b100: 2020 2020 2020 2020 2274 6167 6c69 7374          "taglist
-0001b110: 223a 205b 5d2c 0a20 2020 2020 2020 2020  ": [],.         
-0001b120: 2020 2022 7372 7669 6e66 223a 2073 7276     "srvinf": srv
-0001b130: 5f69 6e66 6f74 2c0a 2020 2020 2020 2020  _infot,.        
-0001b140: 2020 2020 2261 6363 7422 3a20 7365 6c66      "acct": self
-0001b150: 2e75 6e61 6d65 2c0a 2020 2020 2020 2020  .uname,.        
-0001b160: 2020 2020 2269 6478 223a 2065 3264 2c0a      "idx": e2d,.
-0001b170: 2020 2020 2020 2020 2020 2020 2269 7461              "ita
-0001b180: 6722 3a20 6532 742c 0a20 2020 2020 2020  g": e2t,.       
-0001b190: 2020 2020 2022 6c69 6665 7469 6d65 223a       "lifetime":
-0001b1a0: 2076 6e2e 666c 6167 732e 6765 7428 226c   vn.flags.get("l
-0001b1b0: 6966 6574 696d 6522 2920 6f72 2030 2c0a  ifetime") or 0,.
-0001b1c0: 2020 2020 2020 2020 2020 2020 2266 7261              "fra
-0001b1d0: 6e64 223a 2062 6f6f 6c28 766e 2e66 6c61  nd": bool(vn.fla
-0001b1e0: 6773 2e67 6574 2822 7261 6e64 2229 292c  gs.get("rand")),
-0001b1f0: 0a20 2020 2020 2020 2020 2020 2022 7065  .            "pe
-0001b200: 726d 7322 3a20 7065 726d 732c 0a20 2020  rms": perms,.   
-0001b210: 2020 2020 2020 2020 2022 6c6f 6775 6573           "logues
-0001b220: 223a 206c 6f67 7565 732c 0a20 2020 2020  ": logues,.     
-0001b230: 2020 2020 2020 2022 7265 6164 6d65 223a         "readme":
-0001b240: 2072 6561 646d 652c 0a20 2020 2020 2020   readme,.       
-0001b250: 207d 0a20 2020 2020 2020 206a 3261 203d   }.        j2a =
-0001b260: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-0001b270: 7664 6972 223a 2071 756f 7465 7028 7365  vdir": quotep(se
-0001b280: 6c66 2e76 7061 7468 292c 0a20 2020 2020  lf.vpath),.     
-0001b290: 2020 2020 2020 2022 7670 6e6f 6465 7322         "vpnodes"
-0001b2a0: 3a20 7670 6e6f 6465 732c 0a20 2020 2020  : vpnodes,.     
-0001b2b0: 2020 2020 2020 2022 6669 6c65 7322 3a20         "files": 
-0001b2c0: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
-0001b2d0: 226c 7330 223a 204e 6f6e 652c 0a20 2020  "ls0": None,.   
-0001b2e0: 2020 2020 2020 2020 2022 6163 6374 223a           "acct":
-0001b2f0: 2073 656c 662e 756e 616d 652c 0a20 2020   self.uname,.   
-0001b300: 2020 2020 2020 2020 2022 7065 726d 7322           "perms"
-0001b310: 3a20 6a73 6f6e 2e64 756d 7073 2870 6572  : json.dumps(per
-0001b320: 6d73 292c 0a20 2020 2020 2020 2020 2020  ms),.           
-0001b330: 2022 6c69 6665 7469 6d65 223a 206c 735f   "lifetime": ls_
-0001b340: 7265 745b 226c 6966 6574 696d 6522 5d2c  ret["lifetime"],
-0001b350: 0a20 2020 2020 2020 2020 2020 2022 6672  .            "fr
-0001b360: 616e 6422 3a20 626f 6f6c 2876 6e2e 666c  and": bool(vn.fl
-0001b370: 6167 732e 6765 7428 2272 616e 6422 2929  ags.get("rand"))
-0001b380: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
-0001b390: 6167 6c69 7374 223a 205b 5d2c 0a20 2020  aglist": [],.   
-0001b3a0: 2020 2020 2020 2020 2022 6465 665f 6863           "def_hc
-0001b3b0: 6f6c 7322 3a20 5b5d 2c0a 2020 2020 2020  ols": [],.      
-0001b3c0: 2020 2020 2020 2268 6176 655f 656d 7022        "have_emp"
-0001b3d0: 3a20 7365 6c66 2e61 7267 732e 656d 702c  : self.args.emp,
-0001b3e0: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
-0001b3f0: 7665 5f75 7032 6b5f 6964 7822 3a20 6532  ve_up2k_idx": e2
-0001b400: 642c 0a20 2020 2020 2020 2020 2020 2022  d,.            "
-0001b410: 6861 7665 5f74 6167 735f 6964 7822 3a20  have_tags_idx": 
-0001b420: 6532 742c 0a20 2020 2020 2020 2020 2020  e2t,.           
-0001b430: 2022 6861 7665 5f61 636f 6465 223a 2028   "have_acode": (
-0001b440: 6e6f 7420 7365 6c66 2e61 7267 732e 6e6f  not self.args.no
-0001b450: 5f61 636f 6465 292c 0a20 2020 2020 2020  _acode),.       
-0001b460: 2020 2020 2022 6861 7665 5f6d 7622 3a20       "have_mv": 
-0001b470: 286e 6f74 2073 656c 662e 6172 6773 2e6e  (not self.args.n
-0001b480: 6f5f 6d76 292c 0a20 2020 2020 2020 2020  o_mv),.         
-0001b490: 2020 2022 6861 7665 5f64 656c 223a 2028     "have_del": (
-0001b4a0: 6e6f 7420 7365 6c66 2e61 7267 732e 6e6f  not self.args.no
-0001b4b0: 5f64 656c 292c 0a20 2020 2020 2020 2020  _del),.         
-0001b4c0: 2020 2022 6861 7665 5f7a 6970 223a 2028     "have_zip": (
-0001b4d0: 6e6f 7420 7365 6c66 2e61 7267 732e 6e6f  not self.args.no
-0001b4e0: 5f7a 6970 292c 0a20 2020 2020 2020 2020  _zip),.         
-0001b4f0: 2020 2022 6861 7665 5f75 6e70 6f73 7422     "have_unpost"
-0001b500: 3a20 696e 7428 7365 6c66 2e61 7267 732e  : int(self.args.
-0001b510: 756e 706f 7374 292c 0a20 2020 2020 2020  unpost),.       
-0001b520: 2020 2020 2022 6861 7665 5f62 5f75 223a       "have_b_u":
-0001b530: 2028 7365 6c66 2e63 616e 5f77 7269 7465   (self.can_write
-0001b540: 2061 6e64 2073 656c 662e 7570 6172 616d   and self.uparam
-0001b550: 2e67 6574 2822 6222 2920 3d3d 2022 7522  .get("b") == "u"
-0001b560: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
-0001b570: 7362 5f6d 6422 3a20 2222 2069 6620 226e  sb_md": "" if "n
-0001b580: 6f5f 7362 5f6d 6422 2069 6e20 7666 2065  o_sb_md" in vf e
-0001b590: 6c73 6520 2876 662e 6765 7428 226d 645f  lse (vf.get("md_
-0001b5a0: 7362 6622 2920 6f72 2022 7922 292c 0a20  sbf") or "y"),. 
-0001b5b0: 2020 2020 2020 2020 2020 2022 7362 5f6c             "sb_l
-0001b5c0: 6722 3a20 2222 2069 6620 226e 6f5f 7362  g": "" if "no_sb
-0001b5d0: 5f6c 6722 2069 6e20 7666 2065 6c73 6520  _lg" in vf else 
-0001b5e0: 2876 662e 6765 7428 226c 675f 7362 6622  (vf.get("lg_sbf"
-0001b5f0: 2920 6f72 2022 7922 292c 0a20 2020 2020  ) or "y"),.     
-0001b600: 2020 2020 2020 2022 7572 6c5f 7375 6622         "url_suf"
-0001b610: 3a20 7572 6c5f 7375 662c 0a20 2020 2020  : url_suf,.     
-0001b620: 2020 2020 2020 2022 6c6f 6775 6573 223a         "logues":
-0001b630: 206c 6f67 7565 732c 0a20 2020 2020 2020   logues,.       
-0001b640: 2020 2020 2022 7265 6164 6d65 223a 2072       "readme": r
-0001b650: 6561 646d 652c 0a20 2020 2020 2020 2020  eadme,.         
-0001b660: 2020 2022 7469 746c 6522 3a20 6874 6d6c     "title": html
-0001b670: 5f65 7363 6170 6528 7365 6c66 2e76 7061  _escape(self.vpa
-0001b680: 7468 2c20 6372 6c66 3d54 7275 6529 206f  th, crlf=True) o
-0001b690: 7220 22f0 9f92 bef0 9f8e 8922 2c0a 2020  r "........",.  
-0001b6a0: 2020 2020 2020 2020 2020 2273 7276 5f69            "srv_i
-0001b6b0: 6e66 6f22 3a20 7372 765f 696e 666f 742c  nfo": srv_infot,
-0001b6c0: 0a20 2020 2020 2020 2020 2020 2022 6474  .            "dt
-0001b6d0: 6865 6d65 223a 2073 656c 662e 6172 6773  heme": self.args
-0001b6e0: 2e74 6865 6d65 2c0a 2020 2020 2020 2020  .theme,.        
-0001b6f0: 2020 2020 2274 6865 6d65 7322 3a20 7365      "themes": se
-0001b700: 6c66 2e61 7267 732e 7468 656d 6573 2c0a  lf.args.themes,.
-0001b710: 2020 2020 2020 2020 2020 2020 2274 7572              "tur
-0001b720: 626f 6c76 6c22 3a20 7365 6c66 2e61 7267  bolvl": self.arg
-0001b730: 732e 7475 7262 6f2c 0a20 2020 2020 2020  s.turbo,.       
-0001b740: 2020 2020 2022 7532 736f 7274 223a 2073       "u2sort": s
-0001b750: 656c 662e 6172 6773 2e75 3273 6f72 742c  elf.args.u2sort,
-0001b760: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-0001b770: 2020 2020 6966 2073 656c 662e 6172 6773      if self.args
-0001b780: 2e6a 735f 6272 6f77 7365 723a 0a20 2020  .js_browser:.   
-0001b790: 2020 2020 2020 2020 206a 3261 5b22 6a73           j2a["js
-0001b7a0: 225d 203d 2073 656c 662e 6172 6773 2e6a  "] = self.args.j
-0001b7b0: 735f 6272 6f77 7365 720a 0a20 2020 2020  s_browser..     
-0001b7c0: 2020 2069 6620 7365 6c66 2e61 7267 732e     if self.args.
-0001b7d0: 6373 735f 6272 6f77 7365 723a 0a20 2020  css_browser:.   
-0001b7e0: 2020 2020 2020 2020 206a 3261 5b22 6373           j2a["cs
-0001b7f0: 7322 5d20 3d20 7365 6c66 2e61 7267 732e  s"] = self.args.
-0001b800: 6373 735f 6272 6f77 7365 720a 0a20 2020  css_browser..   
-0001b810: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-0001b820: 2e63 6f6e 6e2e 6873 7276 2e70 7269 736d  .conn.hsrv.prism
-0001b830: 3a0a 2020 2020 2020 2020 2020 2020 6a32  :.            j2
-0001b840: 615b 226e 6f5f 7072 6973 6d22 5d20 3d20  a["no_prism"] = 
-0001b850: 5472 7565 0a0a 2020 2020 2020 2020 6966  True..        if
-0001b860: 206e 6f74 2073 656c 662e 6361 6e5f 7265   not self.can_re
-0001b870: 6164 3a0a 2020 2020 2020 2020 2020 2020  ad:.            
-0001b880: 6966 2069 735f 6c73 3a0a 2020 2020 2020  if is_ls:.      
-0001b890: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001b8a0: 2073 656c 662e 7478 5f6c 7328 6c73 5f72   self.tx_ls(ls_r
-0001b8b0: 6574 290a 0a20 2020 2020 2020 2020 2020  et)..           
-0001b8c0: 2069 6620 6e6f 7420 7374 6174 2e53 5f49   if not stat.S_I
-0001b8d0: 5344 4952 2873 742e 7374 5f6d 6f64 6529  SDIR(st.st_mode)
-0001b8e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001b8f0: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
-0001b900: 5f34 3034 2854 7275 6529 0a0a 2020 2020  _404(True)..    
-0001b910: 2020 2020 2020 2020 6966 2022 7a69 7022          if "zip"
-0001b920: 2069 6e20 7365 6c66 2e75 7061 7261 6d20   in self.uparam 
-0001b930: 6f72 2022 7461 7222 2069 6e20 7365 6c66  or "tar" in self
-0001b940: 2e75 7061 7261 6d3a 0a20 2020 2020 2020  .uparam:.       
-0001b950: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
-0001b960: 6562 6b61 6328 3430 3329 0a0a 2020 2020  ebkac(403)..    
-0001b970: 2020 2020 2020 2020 6874 6d6c 203d 2073          html = s
-0001b980: 656c 662e 6a32 7328 7470 6c2c 202a 2a6a  elf.j2s(tpl, **j
-0001b990: 3261 290a 2020 2020 2020 2020 2020 2020  2a).            
-0001b9a0: 7365 6c66 2e72 6570 6c79 2868 746d 6c2e  self.reply(html.
-0001b9b0: 656e 636f 6465 2822 7574 662d 3822 2c20  encode("utf-8", 
-0001b9c0: 2272 6570 6c61 6365 2229 290a 2020 2020  "replace")).    
-0001b9d0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0001b9e0: 7275 650a 0a20 2020 2020 2020 2066 6f72  rue..        for
-0001b9f0: 206b 2069 6e20 5b22 7a69 7022 2c20 2274   k in ["zip", "t
-0001ba00: 6172 225d 3a0a 2020 2020 2020 2020 2020  ar"]:.          
-0001ba10: 2020 7620 3d20 7365 6c66 2e75 7061 7261    v = self.upara
-0001ba20: 6d2e 6765 7428 6b29 0a20 2020 2020 2020  m.get(k).       
-0001ba30: 2020 2020 2069 6620 7620 6973 206e 6f74       if v is not
-0001ba40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001ba50: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001ba60: 6c66 2e74 785f 7a69 7028 6b2c 2076 2c20  lf.tx_zip(k, v, 
-0001ba70: 766e 2c20 7265 6d2c 205b 5d2c 2073 656c  vn, rem, [], sel
-0001ba80: 662e 6172 6773 2e65 6429 0a0a 2020 2020  f.args.ed)..    
-0001ba90: 2020 2020 6673 726f 6f74 2c20 7666 735f      fsroot, vfs_
-0001baa0: 6c73 2c20 7666 735f 7669 7274 203d 2076  ls, vfs_virt = v
-0001bab0: 6e2e 6c73 280a 2020 2020 2020 2020 2020  n.ls(.          
-0001bac0: 2020 7265 6d2c 2073 656c 662e 756e 616d    rem, self.unam
-0001bad0: 652c 206e 6f74 2073 656c 662e 6172 6773  e, not self.args
-0001bae0: 2e6e 6f5f 7363 616e 6469 722c 205b 5b54  .no_scandir, [[T
-0001baf0: 7275 652c 2046 616c 7365 5d2c 205b 4661  rue, False], [Fa
-0001bb00: 6c73 652c 2054 7275 655d 5d0a 2020 2020  lse, True]].    
-0001bb10: 2020 2020 290a 2020 2020 2020 2020 7374      ).        st
-0001bb20: 6174 7320 3d20 7b6b 3a20 7620 666f 7220  ats = {k: v for 
-0001bb30: 6b2c 2076 2069 6e20 7666 735f 6c73 7d0a  k, v in vfs_ls}.
-0001bb40: 2020 2020 2020 2020 6c73 5f6e 616d 6573          ls_names
-0001bb50: 203d 205b 785b 305d 2066 6f72 2078 2069   = [x[0] for x i
-0001bb60: 6e20 7666 735f 6c73 5d0a 2020 2020 2020  n vfs_ls].      
-0001bb70: 2020 6c73 5f6e 616d 6573 2e65 7874 656e    ls_names.exten
-0001bb80: 6428 6c69 7374 2876 6673 5f76 6972 742e  d(list(vfs_virt.
-0001bb90: 6b65 7973 2829 2929 0a0a 2020 2020 2020  keys()))..      
-0001bba0: 2020 2320 6368 6563 6b20 666f 7220 6f6c    # check for ol
-0001bbb0: 6420 7665 7273 696f 6e73 206f 6620 6669  d versions of fi
-0001bbc0: 6c65 732c 0a20 2020 2020 2020 2023 205b  les,.        # [
-0001bbd0: 6e75 6d2d 6261 636b 7570 732c 206d 6f73  num-backups, mos
-0001bbe0: 742d 7265 6365 6e74 2c20 6869 7374 2d70  t-recent, hist-p
-0001bbf0: 6174 685d 0a20 2020 2020 2020 2068 6973  ath].        his
-0001bc00: 7420 2020 2020 3d20 7b7d 0a20 2020 2020  t     = {}.     
-0001bc10: 2020 2068 6973 7464 6972 203d 206f 732e     histdir = os.
-0001bc20: 7061 7468 2e6a 6f69 6e28 6673 726f 6f74  path.join(fsroot
-0001bc30: 2c20 222e 6869 7374 2229 0a20 2020 2020  , ".hist").     
-0001bc40: 2020 2070 746e 203d 2072 652e 636f 6d70     ptn = re.comp
-0001bc50: 696c 6528 7222 282e 2a29 5c2e 285b 302d  ile(r"(.*)\.([0-
-0001bc60: 395d 2b5c 2e5b 302d 395d 7b33 7d29 285c  9]+\.[0-9]{3})(\
-0001bc70: 2e5b 5e5c 2e5d 2b29 2422 290a 2020 2020  .[^\.]+)$").    
-0001bc80: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0001bc90: 2020 2020 2066 6f72 2068 666e 2069 6e20       for hfn in 
-0001bca0: 626f 732e 6c69 7374 6469 7228 6869 7374  bos.listdir(hist
-0001bcb0: 6469 7229 3a0a 2020 2020 2020 2020 2020  dir):.          
-0001bcc0: 2020 2020 2020 6d20 3d20 7074 6e2e 6d61        m = ptn.ma
-0001bcd0: 7463 6828 6866 6e29 0a20 2020 2020 2020  tch(hfn).       
-0001bce0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0001bcf0: 6d3a 0a20 2020 2020 2020 2020 2020 2020  m:.             
-0001bd00: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-0001bd10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bd20: 2066 6e20 3d20 6d2e 6772 6f75 7028 3129   fn = m.group(1)
-0001bd30: 202b 206d 2e67 726f 7570 2833 290a 2020   + m.group(3).  
-0001bd40: 2020 2020 2020 2020 2020 2020 2020 6e2c                n,
-0001bd50: 2074 732c 205f 203d 2068 6973 742e 6765   ts, _ = hist.ge
-0001bd60: 7428 666e 2c20 2830 2c20 302c 2022 2229  t(fn, (0, 0, "")
-0001bd70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001bd80: 2020 6869 7374 5b66 6e5d 203d 2028 6e20    hist[fn] = (n 
-0001bd90: 2b20 312c 206d 6178 2874 732c 2066 6c6f  + 1, max(ts, flo
-0001bda0: 6174 286d 2e67 726f 7570 2832 2929 292c  at(m.group(2))),
-0001bdb0: 2068 666e 290a 2020 2020 2020 2020 6578   hfn).        ex
-0001bdc0: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
-0001bdd0: 2020 7061 7373 0a0a 2020 2020 2020 2020    pass..        
-0001bde0: 2320 7368 6f77 2064 6f74 6669 6c65 7320  # show dotfiles 
-0001bdf0: 6966 2070 6572 6d69 7474 6564 2061 6e64  if permitted and
-0001be00: 2072 6571 7565 7374 6564 0a20 2020 2020   requested.     
-0001be10: 2020 2069 6620 6e6f 7420 7365 6c66 2e61     if not self.a
-0001be20: 7267 732e 6564 206f 7220 2264 6f74 7322  rgs.ed or "dots"
-0001be30: 206e 6f74 2069 6e20 7365 6c66 2e75 7061   not in self.upa
-0001be40: 7261 6d3a 0a20 2020 2020 2020 2020 2020  ram:.           
-0001be50: 206c 735f 6e61 6d65 7320 3d20 6578 636c   ls_names = excl
-0001be60: 7564 655f 646f 7466 696c 6573 286c 735f  ude_dotfiles(ls_
-0001be70: 6e61 6d65 7329 0a0a 2020 2020 2020 2020  names)..        
-0001be80: 6164 645f 666b 203d 2076 6e2e 666c 6167  add_fk = vn.flag
-0001be90: 732e 6765 7428 2266 6b22 290a 0a20 2020  s.get("fk")..   
-0001bea0: 2020 2020 2064 6972 7320 3d20 5b5d 0a20       dirs = []. 
-0001beb0: 2020 2020 2020 2066 696c 6573 203d 205b         files = [
-0001bec0: 5d0a 2020 2020 2020 2020 666f 7220 666e  ].        for fn
-0001bed0: 2069 6e20 6c73 5f6e 616d 6573 3a0a 2020   in ls_names:.  
-0001bee0: 2020 2020 2020 2020 2020 6261 7365 203d            base =
-0001bef0: 2022 220a 2020 2020 2020 2020 2020 2020   "".            
-0001bf00: 6872 6566 203d 2066 6e0a 2020 2020 2020  href = fn.      
-0001bf10: 2020 2020 2020 6966 206e 6f74 2069 735f        if not is_
-0001bf20: 6c73 2061 6e64 206e 6f74 2069 735f 6a73  ls and not is_js
-0001bf30: 2061 6e64 206e 6f74 2073 656c 662e 7472   and not self.tr
-0001bf40: 6169 6c69 6e67 5f73 6c61 7368 2061 6e64  ailing_slash and
-0001bf50: 2076 7061 7468 3a0a 2020 2020 2020 2020   vpath:.        
-0001bf60: 2020 2020 2020 2020 6261 7365 203d 2022          base = "
-0001bf70: 2f22 202b 2076 7061 7468 202b 2022 2f22  /" + vpath + "/"
-0001bf80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bf90: 2068 7265 6620 3d20 6261 7365 202b 2066   href = base + f
-0001bfa0: 6e0a 0a20 2020 2020 2020 2020 2020 2069  n..            i
-0001bfb0: 6620 666e 2069 6e20 7666 735f 7669 7274  f fn in vfs_virt
-0001bfc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001bfd0: 2020 6673 7061 7468 203d 2076 6673 5f76    fspath = vfs_v
-0001bfe0: 6972 745b 666e 5d2e 7265 616c 7061 7468  irt[fn].realpath
-0001bff0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001c000: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001c010: 2020 2066 7370 6174 6820 3d20 6673 726f     fspath = fsro
-0001c020: 6f74 202b 2022 2f22 202b 2066 6e0a 0a20  ot + "/" + fn.. 
-0001c030: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0001c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c050: 696e 6620 3d20 7374 6174 732e 6765 7428  inf = stats.get(
-0001c060: 666e 2920 6f72 2062 6f73 2e73 7461 7428  fn) or bos.stat(
-0001c070: 6673 7061 7468 290a 2020 2020 2020 2020  fspath).        
-0001c080: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-0001c090: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001c0a0: 2e6c 6f67 2822 6272 6f6b 656e 2073 796d  .log("broken sym
-0001c0b0: 6c69 6e6b 3a20 7b7d 222e 666f 726d 6174  link: {}".format
-0001c0c0: 2872 6570 7228 6673 7061 7468 2929 290a  (repr(fspath))).
-0001c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c0e0: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
-0001c0f0: 2020 2020 2020 6973 5f64 6972 203d 2073        is_dir = s
-0001c100: 7461 742e 535f 4953 4449 5228 696e 662e  tat.S_ISDIR(inf.
-0001c110: 7374 5f6d 6f64 6529 0a20 2020 2020 2020  st_mode).       
-0001c120: 2020 2020 2069 6620 6973 5f64 6972 3a0a       if is_dir:.
-0001c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c140: 6872 6566 202b 3d20 222f 220a 2020 2020  href += "/".    
-0001c150: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0001c160: 656c 662e 6172 6773 2e6e 6f5f 7a69 703a  elf.args.no_zip:
-0001c170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c180: 2020 2020 206d 6172 6769 6e20 3d20 2244       margin = "D
-0001c190: 4952 220a 2020 2020 2020 2020 2020 2020  IR".            
-0001c1a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001c1b0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0001c1c0: 7267 696e 203d 2027 3c61 2068 7265 663d  rgin = '<a href=
-0001c1d0: 227b 7d3f 7a69 7022 2072 656c 3d22 6e6f  "{}?zip" rel="no
-0001c1e0: 666f 6c6c 6f77 223e 7a69 703c 2f61 3e27  follow">zip</a>'
-0001c1f0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-0001c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c210: 2071 756f 7465 7028 6872 6566 290a 2020   quotep(href).  
-0001c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c230: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001c240: 656c 6966 2066 6e20 696e 2068 6973 743a  elif fn in hist:
-0001c250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c260: 206d 6172 6769 6e20 3d20 273c 6120 6872   margin = '<a hr
-0001c270: 6566 3d22 7b7d 2e68 6973 742f 7b7d 223e  ef="{}.hist/{}">
-0001c280: 237b 7d3c 2f61 3e27 2e66 6f72 6d61 7428  #{}</a>'.format(
-0001c290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c2a0: 2020 2020 2062 6173 652c 2068 746d 6c5f       base, html_
-0001c2b0: 6573 6361 7065 2868 6973 745b 666e 5d5b  escape(hist[fn][
-0001c2c0: 325d 2c20 7175 6f74 3d54 7275 652c 2063  2], quot=True, c
-0001c2d0: 726c 663d 5472 7565 292c 2068 6973 745b  rlf=True), hist[
-0001c2e0: 666e 5d5b 305d 0a20 2020 2020 2020 2020  fn][0].         
-0001c2f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001c300: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001c310: 2020 2020 2020 2020 2020 206d 6172 6769             margi
-0001c320: 6e20 3d20 222d 220a 0a20 2020 2020 2020  n = "-"..       
-0001c330: 2020 2020 2073 7a20 3d20 696e 662e 7374       sz = inf.st
-0001c340: 5f73 697a 650a 2020 2020 2020 2020 2020  _size.          
-0001c350: 2020 7a64 203d 2064 6174 6574 696d 652e    zd = datetime.
-0001c360: 7574 6366 726f 6d74 696d 6573 7461 6d70  utcfromtimestamp
-0001c370: 2869 6e66 2e73 745f 6d74 696d 6529 0a20  (inf.st_mtime). 
-0001c380: 2020 2020 2020 2020 2020 2064 7420 3d20             dt = 
-0001c390: 7a64 2e73 7472 6674 696d 6528 2225 592d  zd.strftime("%Y-
-0001c3a0: 256d 2d25 6420 2548 3a25 4d3a 2553 2229  %m-%d %H:%M:%S")
-0001c3b0: 0a0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-0001c3c0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0001c3d0: 2020 2065 7874 203d 2022 2d2d 2d22 2069     ext = "---" i
-0001c3e0: 6620 6973 5f64 6972 2065 6c73 6520 666e  f is_dir else fn
-0001c3f0: 2e72 7370 6c69 7428 222e 222c 2031 295b  .rsplit(".", 1)[
-0001c400: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
-0001c410: 2020 2069 6620 6c65 6e28 6578 7429 203e     if len(ext) >
-0001c420: 2031 363a 0a20 2020 2020 2020 2020 2020   16:.           
-0001c430: 2020 2020 2020 2020 2065 7874 203d 2065           ext = e
-0001c440: 7874 5b3a 3136 5d0a 2020 2020 2020 2020  xt[:16].        
-0001c450: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-0001c460: 2020 2020 2020 2020 2020 2020 6578 7420              ext 
-0001c470: 3d20 2225 220a 0a20 2020 2020 2020 2020  = "%"..         
-0001c480: 2020 2069 6620 6164 645f 666b 3a0a 2020     if add_fk:.  
-0001c490: 2020 2020 2020 2020 2020 2020 2020 6872                hr
-0001c4a0: 6566 203d 2022 7b7d 3f6b 3d7b 7d22 2e66  ef = "{}?k={}".f
-0001c4b0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-0001c4c0: 2020 2020 2020 2020 2020 2071 756f 7465             quote
-0001c4d0: 7028 6872 6566 292c 0a20 2020 2020 2020  p(href),.       
-0001c4e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001c4f0: 662e 6765 6e5f 666b 280a 2020 2020 2020  f.gen_fk(.      
-0001c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c510: 2020 7365 6c66 2e61 7267 732e 666b 5f73    self.args.fk_s
-0001c520: 616c 742c 2066 7370 6174 682c 2073 7a2c  alt, fspath, sz,
-0001c530: 2030 2069 6620 414e 5957 494e 2065 6c73   0 if ANYWIN els
-0001c540: 6520 696e 662e 7374 5f69 6e6f 0a20 2020  e inf.st_ino.   
-0001c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c560: 2029 5b3a 6164 645f 666b 5d2c 0a20 2020   )[:add_fk],.   
-0001c570: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001c580: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001c590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c5a0: 2068 7265 6620 3d20 7175 6f74 6570 2868   href = quotep(h
-0001c5b0: 7265 6629 0a0a 2020 2020 2020 2020 2020  ref)..          
-0001c5c0: 2020 6974 656d 203d 207b 0a20 2020 2020    item = {.     
-0001c5d0: 2020 2020 2020 2020 2020 2022 6c65 6164             "lead
-0001c5e0: 223a 206d 6172 6769 6e2c 0a20 2020 2020  ": margin,.     
-0001c5f0: 2020 2020 2020 2020 2020 2022 6872 6566             "href
-0001c600: 223a 2068 7265 662c 0a20 2020 2020 2020  ": href,.       
-0001c610: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-0001c620: 2066 6e2c 0a20 2020 2020 2020 2020 2020   fn,.           
-0001c630: 2020 2020 2022 737a 223a 2073 7a2c 0a20       "sz": sz,. 
-0001c640: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001c650: 6578 7422 3a20 6578 742c 0a20 2020 2020  ext": ext,.     
-0001c660: 2020 2020 2020 2020 2020 2022 6474 223a             "dt":
-0001c670: 2064 742c 0a20 2020 2020 2020 2020 2020   dt,.           
-0001c680: 2020 2020 2022 7473 223a 2069 6e74 2869       "ts": int(i
-0001c690: 6e66 2e73 745f 6d74 696d 6529 2c0a 2020  nf.st_mtime),.  
-0001c6a0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-0001c6b0: 2020 2020 2020 2020 6966 2069 735f 6469          if is_di
-0001c6c0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0001c6d0: 2020 2064 6972 732e 6170 7065 6e64 2869     dirs.append(i
-0001c6e0: 7465 6d29 0a20 2020 2020 2020 2020 2020  tem).           
-0001c6f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001c700: 2020 2020 2020 2066 696c 6573 2e61 7070         files.app
-0001c710: 656e 6428 6974 656d 290a 2020 2020 2020  end(item).      
-0001c720: 2020 2020 2020 2020 2020 6974 656d 5b22            item["
-0001c730: 7264 225d 203d 2072 656d 0a0a 2020 2020  rd"] = rem..    
-0001c740: 2020 2020 7461 6773 6574 2020 3d20 7365      tagset  = se
-0001c750: 7428 290a 2020 2020 2020 2020 666f 7220  t().        for 
-0001c760: 6665 2069 6e20 6669 6c65 733a 0a20 2020  fe in files:.   
-0001c770: 2020 2020 2020 2020 2066 6e20 3d20 6665           fn = fe
-0001c780: 5b22 6e61 6d65 225d 0a20 2020 2020 2020  ["name"].       
-0001c790: 2020 2020 2072 6420 3d20 6665 5b22 7264       rd = fe["rd
-0001c7a0: 225d 0a20 2020 2020 2020 2020 2020 2064  "].            d
-0001c7b0: 656c 2066 655b 2272 6422 5d0a 2020 2020  el fe["rd"].    
-0001c7c0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-0001c7d0: 6375 723a 0a20 2020 2020 2020 2020 2020  cur:.           
-0001c7e0: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-0001c7f0: 2020 2020 2020 2020 2020 2069 6620 766e             if vn
-0001c800: 2021 3d20 6462 763a 0a20 2020 2020 2020   != dbv:.       
-0001c810: 2020 2020 2020 2020 205f 2c20 7264 203d           _, rd =
-0001c820: 2076 6e2e 6765 745f 6462 7628 7264 290a   vn.get_dbv(rd).
-0001c830: 0a20 2020 2020 2020 2020 2020 2071 203d  .            q =
-0001c840: 2022 7365 6c65 6374 206d 742e 6b2c 206d   "select mt.k, m
-0001c850: 742e 7620 6672 6f6d 2075 7020 696e 6e65  t.v from up inne
-0001c860: 7220 6a6f 696e 206d 7420 6f6e 206d 742e  r join mt on mt.
-0001c870: 7720 3d20 7375 6273 7472 2875 702e 772c  w = substr(up.w,
-0001c880: 312c 3136 2920 7768 6572 6520 7570 2e72  1,16) where up.r
-0001c890: 6420 3d20 3f20 616e 6420 7570 2e66 6e20  d = ? and up.fn 
-0001c8a0: 3d20 3f20 616e 6420 2b6d 742e 6b20 213d  = ? and +mt.k !=
-0001c8b0: 2027 7827 220a 2020 2020 2020 2020 2020   'x'".          
-0001c8c0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0001c8d0: 2020 2020 2020 2072 203d 2069 6375 722e         r = icur.
-0001c8e0: 6578 6563 7574 6528 712c 2028 7264 2c20  execute(q, (rd, 
-0001c8f0: 666e 2929 0a20 2020 2020 2020 2020 2020  fn)).           
-0001c900: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0001c910: 6e20 6173 2065 783a 0a20 2020 2020 2020  n as ex:.       
-0001c920: 2020 2020 2020 2020 2069 6620 2264 6174           if "dat
-0001c930: 6162 6173 6520 6973 206c 6f63 6b65 6422  abase is locked"
-0001c940: 2069 6e20 7374 7228 6578 293a 0a20 2020   in str(ex):.   
-0001c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c960: 2062 7265 616b 0a0a 2020 2020 2020 2020   break..        
-0001c970: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0001c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c990: 2061 7267 7320 3d20 7333 656e 6328 6964   args = s3enc(id
-0001c9a0: 782e 6d65 6d5f 6375 722c 2072 642c 2066  x.mem_cur, rd, f
-0001c9b0: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-0001c9c0: 2020 2020 2020 2072 203d 2069 6375 722e         r = icur.
-0001c9d0: 6578 6563 7574 6528 712c 2061 7267 7329  execute(q, args)
-0001c9e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c9f0: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-0001ca00: 2020 2020 2020 2020 2020 2020 2074 203d               t =
-0001ca10: 2022 7461 6720 7265 6164 2065 7272 6f72   "tag read error
-0001ca20: 2c20 7b7d 2f7b 7d5c 6e7b 7d22 0a20 2020  , {}/{}\n{}".   
-0001ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca40: 2073 656c 662e 6c6f 6728 742e 666f 726d   self.log(t.form
-0001ca50: 6174 2872 642c 2066 6e2c 206d 696e 5f65  at(rd, fn, min_e
-0001ca60: 7828 2929 290a 2020 2020 2020 2020 2020  x())).          
-0001ca70: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-0001ca80: 0a20 2020 2020 2020 2020 2020 2066 655b  .            fe[
-0001ca90: 2274 6167 7322 5d20 3d20 7b6b 3a20 7620  "tags"] = {k: v 
-0001caa0: 666f 7220 6b2c 2076 2069 6e20 727d 0a20  for k, v in r}. 
-0001cab0: 2020 2020 2020 2020 2020 205f 203d 205b             _ = [
-0001cac0: 7461 6773 6574 2e61 6464 286b 2920 666f  tagset.add(k) fo
-0001cad0: 7220 6b20 696e 2066 655b 2274 6167 7322  r k in fe["tags"
-0001cae0: 5d5d 0a0a 2020 2020 2020 2020 6966 2069  ]]..        if i
-0001caf0: 6375 723a 0a20 2020 2020 2020 2020 2020  cur:.           
-0001cb00: 2074 6167 6c69 7374 203d 205b 6b20 666f   taglist = [k fo
-0001cb10: 7220 6b20 696e 2076 6e2e 666c 6167 732e  r k in vn.flags.
-0001cb20: 6765 7428 226d 7465 222c 2022 2229 2e73  get("mte", "").s
-0001cb30: 706c 6974 2822 2c22 2920 6966 206b 2069  plit(",") if k i
-0001cb40: 6e20 7461 6773 6574 5d0a 2020 2020 2020  n tagset].      
-0001cb50: 2020 2020 2020 666f 7220 6665 2069 6e20        for fe in 
-0001cb60: 6469 7273 3a0a 2020 2020 2020 2020 2020  dirs:.          
-0001cb70: 2020 2020 2020 6665 5b22 7461 6773 225d        fe["tags"]
-0001cb80: 203d 207b 7d0a 2020 2020 2020 2020 656c   = {}.        el
-0001cb90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001cba0: 7461 676c 6973 7420 3d20 6c69 7374 2874  taglist = list(t
-0001cbb0: 6167 7365 7429 0a0a 2020 2020 2020 2020  agset)..        
-0001cbc0: 6966 2069 735f 6c73 3a0a 2020 2020 2020  if is_ls:.      
-0001cbd0: 2020 2020 2020 6c73 5f72 6574 5b22 6469        ls_ret["di
-0001cbe0: 7273 225d 203d 2064 6972 730a 2020 2020  rs"] = dirs.    
-0001cbf0: 2020 2020 2020 2020 6c73 5f72 6574 5b22          ls_ret["
-0001cc00: 6669 6c65 7322 5d20 3d20 6669 6c65 730a  files"] = files.
-0001cc10: 2020 2020 2020 2020 2020 2020 6c73 5f72              ls_r
-0001cc20: 6574 5b22 7461 676c 6973 7422 5d20 3d20  et["taglist"] = 
-0001cc30: 7461 676c 6973 740a 2020 2020 2020 2020  taglist.        
-0001cc40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001cc50: 7478 5f6c 7328 6c73 5f72 6574 290a 0a20  tx_ls(ls_ret).. 
-0001cc60: 2020 2020 2020 2064 6f63 203d 2073 656c         doc = sel
-0001cc70: 662e 7570 6172 616d 2e67 6574 2822 646f  f.uparam.get("do
-0001cc80: 6322 2920 6966 2073 656c 662e 6361 6e5f  c") if self.can_
-0001cc90: 7265 6164 2065 6c73 6520 4e6f 6e65 0a20  read else None. 
-0001cca0: 2020 2020 2020 2069 6620 646f 633a 0a20         if doc:. 
-0001ccb0: 2020 2020 2020 2020 2020 2064 6f63 203d             doc =
-0001ccc0: 2075 6e71 756f 7465 7028 646f 632e 7265   unquotep(doc.re
-0001ccd0: 706c 6163 6528 222b 222c 2022 2022 292e  place("+", " ").
-0001cce0: 7370 6c69 7428 223f 2229 5b30 5d29 0a20  split("?")[0]). 
-0001ccf0: 2020 2020 2020 2020 2020 206a 3261 5b22             j2a["
-0001cd00: 646f 636e 616d 6522 5d20 3d20 646f 630a  docname"] = doc.
-0001cd10: 2020 2020 2020 2020 2020 2020 646f 6374              doct
-0001cd20: 7874 203d 204e 6f6e 650a 2020 2020 2020  xt = None.      
-0001cd30: 2020 2020 2020 6966 206e 6578 7428 2878        if next((x
-0001cd40: 2066 6f72 2078 2069 6e20 6669 6c65 7320   for x in files 
-0001cd50: 6966 2078 5b22 6e61 6d65 225d 203d 3d20  if x["name"] == 
-0001cd60: 646f 6329 2c20 4e6f 6e65 293a 0a20 2020  doc), None):.   
-0001cd70: 2020 2020 2020 2020 2020 2020 2064 6f63               doc
-0001cd80: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-0001cd90: 6f69 6e28 6162 7370 6174 682c 2064 6f63  oin(abspath, doc
-0001cda0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001cdb0: 2020 737a 203d 2062 6f73 2e70 6174 682e    sz = bos.path.
-0001cdc0: 6765 7473 697a 6528 646f 6370 6174 6829  getsize(docpath)
-0001cdd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001cde0: 2069 6620 737a 203c 2031 3032 3420 2a20   if sz < 1024 * 
-0001cdf0: 7365 6c66 2e61 7267 732e 7478 745f 6d61  self.args.txt_ma
-0001ce00: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
-0001ce10: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-0001ce20: 2866 7365 6e63 2864 6f63 7061 7468 292c  (fsenc(docpath),
-0001ce30: 2022 7262 2229 2061 7320 663a 0a20 2020   "rb") as f:.   
-0001ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ce50: 2020 2020 2064 6f63 7478 7420 3d20 662e       doctxt = f.
-0001ce60: 7265 6164 2829 2e64 6563 6f64 6528 2275  read().decode("u
-0001ce70: 7466 2d38 222c 2022 7265 706c 6163 6522  tf-8", "replace"
-0001ce80: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0001ce90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001cea0: 2020 2020 7365 6c66 2e6c 6f67 2822 646f      self.log("do
-0001ceb0: 6320 3430 343a 205b 7b7d 5d22 2e66 6f72  c 404: [{}]".for
-0001cec0: 6d61 7428 646f 6329 2c20 633d 3629 0a20  mat(doc), c=6). 
-0001ced0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001cee0: 6f63 7478 7420 3d20 2228 2074 6578 7466  octxt = "( textf
-0001cef0: 696c 6520 6e6f 7420 666f 756e 6420 2922  ile not found )"
-0001cf00: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001cf10: 2064 6f63 7478 7420 6973 206e 6f74 204e   doctxt is not N
-0001cf20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001cf30: 2020 2020 206a 3261 5b22 646f 6322 5d20       j2a["doc"] 
-0001cf40: 3d20 646f 6374 7874 0a0a 2020 2020 2020  = doctxt..      
-0001cf50: 2020 666f 7220 6420 696e 2064 6972 733a    for d in dirs:
-0001cf60: 0a20 2020 2020 2020 2020 2020 2064 5b22  .            d["
-0001cf70: 6e61 6d65 225d 202b 3d20 222f 220a 0a20  name"] += "/".. 
-0001cf80: 2020 2020 2020 2064 6972 732e 736f 7274         dirs.sort
-0001cf90: 286b 6579 3d69 7465 6d67 6574 7465 7228  (key=itemgetter(
-0001cfa0: 226e 616d 6522 2929 0a0a 2020 2020 2020  "name"))..      
-0001cfb0: 2020 6966 2069 735f 6a73 3a0a 2020 2020    if is_js:.    
-0001cfc0: 2020 2020 2020 2020 6a32 615b 226c 7330          j2a["ls0
-0001cfd0: 225d 203d 207b 2264 6972 7322 3a20 6469  "] = {"dirs": di
-0001cfe0: 7273 2c20 2266 696c 6573 223a 2066 696c  rs, "files": fil
-0001cff0: 6573 2c20 2274 6167 6c69 7374 223a 2074  es, "taglist": t
-0001d000: 6167 6c69 7374 7d0a 2020 2020 2020 2020  aglist}.        
-0001d010: 2020 2020 6a32 615b 2266 696c 6573 225d      j2a["files"]
-0001d020: 203d 205b 5d0a 2020 2020 2020 2020 656c   = [].        el
-0001d030: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001d040: 6a32 615b 2266 696c 6573 225d 203d 2064  j2a["files"] = d
-0001d050: 6972 7320 2b20 6669 6c65 730a 0a20 2020  irs + files..   
-0001d060: 2020 2020 206a 3261 5b22 7461 676c 6973       j2a["taglis
-0001d070: 7422 5d20 3d20 7461 676c 6973 740a 2020  t"] = taglist.  
-0001d080: 2020 2020 2020 6a32 615b 2274 7874 5f65        j2a["txt_e
-0001d090: 7874 225d 203d 2073 656c 662e 6172 6773  xt"] = self.args
-0001d0a0: 2e74 6578 7466 696c 6573 2e72 6570 6c61  .textfiles.repla
-0001d0b0: 6365 2822 2c22 2c20 2220 2229 0a0a 2020  ce(",", " ")..  
-0001d0c0: 2020 2020 2020 6966 2022 6d74 6822 2069        if "mth" i
-0001d0d0: 6e20 766e 2e66 6c61 6773 3a0a 2020 2020  n vn.flags:.    
-0001d0e0: 2020 2020 2020 2020 6a32 615b 2264 6566          j2a["def
-0001d0f0: 5f68 636f 6c73 225d 203d 2076 6e2e 666c  _hcols"] = vn.fl
-0001d100: 6167 735b 226d 7468 225d 2e73 706c 6974  ags["mth"].split
-0001d110: 2822 2c22 290a 0a20 2020 2020 2020 2068  (",")..        h
-0001d120: 746d 6c20 3d20 7365 6c66 2e6a 3273 2874  tml = self.j2s(t
-0001d130: 706c 2c20 2a2a 6a32 6129 0a20 2020 2020  pl, **j2a).     
-0001d140: 2020 2073 656c 662e 7265 706c 7928 6874     self.reply(ht
-0001d150: 6d6c 2e65 6e63 6f64 6528 2275 7466 2d38  ml.encode("utf-8
-0001d160: 222c 2022 7265 706c 6163 6522 2929 0a20  ", "replace")). 
-0001d170: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0001d180: 7565 0a                                  ue.
+0001a3e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a3f0: 735f 6469 7220 3d20 4661 6c73 650a 2020  s_dir = False.  
+0001a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a410: 2020 2020 2020 2020 2020 2020 2020 6272                br
+0001a420: 6561 6b0a 0a20 2020 2020 2020 2020 2020  eak..           
+0001a430: 2020 2020 2020 2020 2069 6620 6973 5f64           if is_d
+0001a440: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
+0001a450: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001a460: 726e 2073 656c 662e 7478 5f69 636f 2822  rn self.tx_ico("
+0001a470: 612e 666f 6c64 6572 2229 0a0a 2020 2020  a.folder")..    
+0001a480: 2020 2020 2020 2020 2020 2020 7468 7020              thp 
+0001a490: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0001a4a0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+0001a4b0: 6875 6d62 636c 693a 0a20 2020 2020 2020  humbcli:.       
+0001a4c0: 2020 2020 2020 2020 2020 2020 2074 6870               thp
+0001a4d0: 203d 2073 656c 662e 7468 756d 6263 6c69   = self.thumbcli
+0001a4e0: 2e67 6574 2864 6276 2c20 7672 656d 2c20  .get(dbv, vrem, 
+0001a4f0: 696e 7428 7374 2e73 745f 6d74 696d 6529  int(st.st_mtime)
+0001a500: 2c20 7468 5f66 6d74 290a 0a20 2020 2020  , th_fmt)..     
+0001a510: 2020 2020 2020 2020 2020 2069 6620 7468             if th
+0001a520: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+0001a530: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001a540: 6c66 2e74 785f 6669 6c65 2874 6870 290a  lf.tx_file(thp).
+0001a550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a560: 2069 6620 7468 5f66 6d74 203d 3d20 2270   if th_fmt == "p
+0001a570: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0001a580: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
+0001a590: 6b61 6328 3430 3429 0a0a 2020 2020 2020  kac(404)..      
+0001a5a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001a5b0: 2073 656c 662e 7478 5f69 636f 2872 656d   self.tx_ico(rem
+0001a5c0: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+0001a5d0: 7420 6973 5f64 6972 2061 6e64 2028 7365  t is_dir and (se
+0001a5e0: 6c66 2e63 616e 5f72 6561 6420 6f72 2073  lf.can_read or s
+0001a5f0: 656c 662e 6361 6e5f 6765 7429 3a0a 2020  elf.can_get):.  
+0001a600: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0001a610: 2073 656c 662e 6361 6e5f 7265 6164 2061   self.can_read a
+0001a620: 6e64 2022 666b 2220 696e 2076 6e2e 666c  nd "fk" in vn.fl
+0001a630: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
+0001a640: 2020 2020 2063 6f72 7265 6374 203d 2073       correct = s
+0001a650: 656c 662e 6765 6e5f 666b 280a 2020 2020  elf.gen_fk(.    
+0001a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a670: 7365 6c66 2e61 7267 732e 666b 5f73 616c  self.args.fk_sal
+0001a680: 742c 2061 6273 7061 7468 2c20 7374 2e73  t, abspath, st.s
+0001a690: 745f 7369 7a65 2c20 3020 6966 2041 4e59  t_size, 0 if ANY
+0001a6a0: 5749 4e20 656c 7365 2073 742e 7374 5f69  WIN else st.st_i
+0001a6b0: 6e6f 0a20 2020 2020 2020 2020 2020 2020  no.             
+0001a6c0: 2020 2029 5b3a 2076 6e2e 666c 6167 735b     )[: vn.flags[
+0001a6d0: 2266 6b22 5d5d 0a20 2020 2020 2020 2020  "fk"]].         
+0001a6e0: 2020 2020 2020 2067 6f74 203d 2073 656c         got = sel
+0001a6f0: 662e 7570 6172 616d 2e67 6574 2822 6b22  f.uparam.get("k"
+0001a700: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001a710: 2020 6966 2067 6f74 2021 3d20 636f 7272    if got != corr
+0001a720: 6563 743a 0a20 2020 2020 2020 2020 2020  ect:.           
+0001a730: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+0001a740: 6728 2277 726f 6e67 2066 696c 656b 6579  g("wrong filekey
+0001a750: 2c20 7761 6e74 207b 7d2c 2067 6f74 207b  , want {}, got {
+0001a760: 7d22 2e66 6f72 6d61 7428 636f 7272 6563  }".format(correc
+0001a770: 742c 2067 6f74 2929 0a20 2020 2020 2020  t, got)).       
+0001a780: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0001a790: 7572 6e20 7365 6c66 2e74 785f 3430 3428  urn self.tx_404(
+0001a7a0: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0001a7b0: 6620 6162 7370 6174 682e 656e 6473 7769  f abspath.endswi
+0001a7c0: 7468 2822 2e6d 6422 2920 616e 6420 280a  th(".md") and (.
+0001a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7e0: 2276 2220 696e 2073 656c 662e 7570 6172  "v" in self.upar
+0001a7f0: 616d 206f 7220 2265 6469 7422 2069 6e20  am or "edit" in 
+0001a800: 7365 6c66 2e75 7061 7261 6d20 6f72 2022  self.uparam or "
+0001a810: 6564 6974 3222 2069 6e20 7365 6c66 2e75  edit2" in self.u
+0001a820: 7061 7261 6d0a 2020 2020 2020 2020 2020  param.          
+0001a830: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+0001a840: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001a850: 2e74 785f 6d64 2861 6273 7061 7468 290a  .tx_md(abspath).
+0001a860: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001a870: 7572 6e20 7365 6c66 2e74 785f 6669 6c65  urn self.tx_file
+0001a880: 2861 6273 7061 7468 290a 0a20 2020 2020  (abspath)..     
+0001a890: 2020 2065 6c69 6620 6973 5f64 6972 2061     elif is_dir a
+0001a8a0: 6e64 206e 6f74 2073 656c 662e 6361 6e5f  nd not self.can_
+0001a8b0: 7265 6164 2061 6e64 206e 6f74 2073 656c  read and not sel
+0001a8c0: 662e 6361 6e5f 7772 6974 653a 0a20 2020  f.can_write:.   
+0001a8d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001a8e0: 7365 6c66 2e74 785f 3430 3428 5472 7565  self.tx_404(True
+0001a8f0: 290a 0a20 2020 2020 2020 2073 7276 5f69  )..        srv_i
+0001a900: 6e66 6f20 3d20 5b5d 0a0a 2020 2020 2020  nfo = []..      
+0001a910: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0001a920: 2020 2069 6620 6e6f 7420 7365 6c66 2e61     if not self.a
+0001a930: 7267 732e 6e69 683a 0a20 2020 2020 2020  rgs.nih:.       
+0001a940: 2020 2020 2020 2020 2073 7276 5f69 6e66           srv_inf
+0001a950: 6f2e 6170 7065 6e64 2873 656c 662e 6172  o.append(self.ar
+0001a960: 6773 2e6e 616d 6529 0a20 2020 2020 2020  gs.name).       
+0001a970: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+0001a980: 2020 2020 2073 656c 662e 6c6f 6728 2223       self.log("#
+0001a990: 776f 7720 2377 686f 6122 290a 0a20 2020  wow #whoa")..   
+0001a9a0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0001a9b0: 2e61 7267 732e 6e69 643a 0a20 2020 2020  .args.nid:.     
+0001a9c0: 2020 2020 2020 2066 7265 652c 2074 6f74         free, tot
+0001a9d0: 616c 203d 2067 6574 5f64 6628 6162 7370  al = get_df(absp
+0001a9e0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+0001a9f0: 2069 6620 746f 7461 6c20 6973 206e 6f74   if total is not
+0001aa00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001aa10: 2020 2020 2020 2068 3120 3d20 6875 6d61         h1 = huma
+0001aa20: 6e73 697a 6528 6672 6565 206f 7220 3029  nsize(free or 0)
+0001aa30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001aa40: 2068 3220 3d20 6875 6d61 6e73 697a 6528   h2 = humansize(
+0001aa50: 746f 7461 6c29 0a20 2020 2020 2020 2020  total).         
+0001aa60: 2020 2020 2020 2073 7276 5f69 6e66 6f2e         srv_info.
+0001aa70: 6170 7065 6e64 2822 7b7d 2066 7265 6520  append("{} free 
+0001aa80: 6f66 207b 7d22 2e66 6f72 6d61 7428 6831  of {}".format(h1
+0001aa90: 2c20 6832 2929 0a20 2020 2020 2020 2020  , h2)).         
+0001aaa0: 2020 2065 6c69 6620 6672 6565 2069 7320     elif free is 
+0001aab0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0001aac0: 2020 2020 2020 2020 2020 7372 765f 696e            srv_in
+0001aad0: 666f 2e61 7070 656e 6428 6875 6d61 6e73  fo.append(humans
+0001aae0: 697a 6528 6672 6565 2c20 5472 7565 2920  ize(free, True) 
+0001aaf0: 2b20 2220 6672 6565 2229 0a0a 2020 2020  + " free")..    
+0001ab00: 2020 2020 7372 765f 696e 666f 7420 3d20      srv_infot = 
+0001ab10: 223c 2f73 7061 6e3e 202f 2f20 3c73 7061  "</span> // <spa
+0001ab20: 6e3e 222e 6a6f 696e 2873 7276 5f69 6e66  n>".join(srv_inf
+0001ab30: 6f29 0a0a 2020 2020 2020 2020 7065 726d  o)..        perm
+0001ab40: 7320 3d20 5b5d 0a20 2020 2020 2020 2069  s = [].        i
+0001ab50: 6620 7365 6c66 2e63 616e 5f72 6561 643a  f self.can_read:
+0001ab60: 0a20 2020 2020 2020 2020 2020 2070 6572  .            per
+0001ab70: 6d73 2e61 7070 656e 6428 2272 6561 6422  ms.append("read"
+0001ab80: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0001ab90: 662e 6361 6e5f 7772 6974 653a 0a20 2020  f.can_write:.   
+0001aba0: 2020 2020 2020 2020 2070 6572 6d73 2e61           perms.a
+0001abb0: 7070 656e 6428 2277 7269 7465 2229 0a20  ppend("write"). 
+0001abc0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0001abd0: 616e 5f6d 6f76 653a 0a20 2020 2020 2020  an_move:.       
+0001abe0: 2020 2020 2070 6572 6d73 2e61 7070 656e       perms.appen
+0001abf0: 6428 226d 6f76 6522 290a 2020 2020 2020  d("move").      
+0001ac00: 2020 6966 2073 656c 662e 6361 6e5f 6465    if self.can_de
+0001ac10: 6c65 7465 3a0a 2020 2020 2020 2020 2020  lete:.          
+0001ac20: 2020 7065 726d 732e 6170 7065 6e64 2822    perms.append("
+0001ac30: 6465 6c65 7465 2229 0a20 2020 2020 2020  delete").       
+0001ac40: 2069 6620 7365 6c66 2e63 616e 5f67 6574   if self.can_get
+0001ac50: 3a0a 2020 2020 2020 2020 2020 2020 7065  :.            pe
+0001ac60: 726d 732e 6170 7065 6e64 2822 6765 7422  rms.append("get"
+0001ac70: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0001ac80: 662e 6361 6e5f 7570 6765 743a 0a20 2020  f.can_upget:.   
+0001ac90: 2020 2020 2020 2020 2070 6572 6d73 2e61           perms.a
+0001aca0: 7070 656e 6428 2275 7067 6574 2229 0a0a  ppend("upget")..
+0001acb0: 2020 2020 2020 2020 7572 6c5f 7375 6620          url_suf 
+0001acc0: 3d20 7365 6c66 2e75 726c 7128 7b7d 2c20  = self.urlq({}, 
+0001acd0: 5b22 6b22 5d29 0a20 2020 2020 2020 2069  ["k"]).        i
+0001ace0: 735f 6c73 203d 2022 6c73 2220 696e 2073  s_ls = "ls" in s
+0001acf0: 656c 662e 7570 6172 616d 0a20 2020 2020  elf.uparam.     
+0001ad00: 2020 2069 735f 6a73 203d 2073 656c 662e     is_js = self.
+0001ad10: 6172 6773 2e66 6f72 6365 5f6a 7320 6f72  args.force_js or
+0001ad20: 2073 656c 662e 636f 6f6b 6965 732e 6765   self.cookies.ge
+0001ad30: 7428 226a 7322 2920 3d3d 2022 7922 0a0a  t("js") == "y"..
+0001ad40: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+0001ad50: 735f 6c73 2061 6e64 2028 7365 6c66 2e75  s_ls and (self.u
+0001ad60: 612e 7374 6172 7473 7769 7468 2822 6375  a.startswith("cu
+0001ad70: 726c 2f22 2920 6f72 2073 656c 662e 7561  rl/") or self.ua
+0001ad80: 2e73 7461 7274 7377 6974 6828 2266 6574  .startswith("fet
+0001ad90: 6368 2229 293a 0a20 2020 2020 2020 2020  ch")):.         
+0001ada0: 2020 2073 656c 662e 7570 6172 616d 5b22     self.uparam["
+0001adb0: 6c73 225d 203d 2022 7622 0a20 2020 2020  ls"] = "v".     
+0001adc0: 2020 2020 2020 2069 735f 6c73 203d 2054         is_ls = T
+0001add0: 7275 650a 0a20 2020 2020 2020 2074 706c  rue..        tpl
+0001ade0: 203d 2022 6272 6f77 7365 7222 0a20 2020   = "browser".   
+0001adf0: 2020 2020 2069 6620 2262 2220 696e 2073       if "b" in s
+0001ae00: 656c 662e 7570 6172 616d 3a0a 2020 2020  elf.uparam:.    
+0001ae10: 2020 2020 2020 2020 7470 6c20 3d20 2262          tpl = "b
+0001ae20: 726f 7773 6572 3222 0a20 2020 2020 2020  rowser2".       
+0001ae30: 2020 2020 2069 735f 6a73 203d 2046 616c       is_js = Fal
+0001ae40: 7365 0a0a 2020 2020 2020 2020 6c6f 6775  se..        logu
+0001ae50: 6573 203d 205b 2222 2c20 2222 5d0a 2020  es = ["", ""].  
+0001ae60: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+0001ae70: 662e 6172 6773 2e6e 6f5f 6c6f 6775 6573  f.args.no_logues
+0001ae80: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+0001ae90: 7220 6e2c 2066 6e20 696e 2065 6e75 6d65  r n, fn in enume
+0001aea0: 7261 7465 285b 222e 7072 6f6c 6f67 7565  rate([".prologue
+0001aeb0: 2e68 746d 6c22 2c20 222e 6570 696c 6f67  .html", ".epilog
+0001aec0: 7565 2e68 746d 6c22 5d29 3a0a 2020 2020  ue.html"]):.    
+0001aed0: 2020 2020 2020 2020 2020 2020 666e 203d              fn =
+0001aee0: 206f 732e 7061 7468 2e6a 6f69 6e28 6162   os.path.join(ab
+0001aef0: 7370 6174 682c 2066 6e29 0a20 2020 2020  spath, fn).     
+0001af00: 2020 2020 2020 2020 2020 2069 6620 626f             if bo
+0001af10: 732e 7061 7468 2e65 7869 7374 7328 666e  s.path.exists(fn
+0001af20: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001af30: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+0001af40: 2866 7365 6e63 2866 6e29 2c20 2272 6222  (fsenc(fn), "rb"
+0001af50: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+0001af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af70: 6c6f 6775 6573 5b6e 5d20 3d20 662e 7265  logues[n] = f.re
+0001af80: 6164 2829 2e64 6563 6f64 6528 2275 7466  ad().decode("utf
+0001af90: 2d38 2229 0a0a 2020 2020 2020 2020 7265  -8")..        re
+0001afa0: 6164 6d65 203d 2022 220a 2020 2020 2020  adme = "".      
+0001afb0: 2020 6966 206e 6f74 2073 656c 662e 6172    if not self.ar
+0001afc0: 6773 2e6e 6f5f 7265 6164 6d65 2061 6e64  gs.no_readme and
+0001afd0: 206e 6f74 206c 6f67 7565 735b 315d 3a0a   not logues[1]:.
+0001afe0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001aff0: 666e 2069 6e20 5b22 5245 4144 4d45 2e6d  fn in ["README.m
+0001b000: 6422 2c20 2272 6561 646d 652e 6d64 225d  d", "readme.md"]
+0001b010: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b020: 2020 666e 203d 206f 732e 7061 7468 2e6a    fn = os.path.j
+0001b030: 6f69 6e28 6162 7370 6174 682c 2066 6e29  oin(abspath, fn)
+0001b040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b050: 2069 6620 626f 732e 7061 7468 2e69 7366   if bos.path.isf
+0001b060: 696c 6528 666e 293a 0a20 2020 2020 2020  ile(fn):.       
+0001b070: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+0001b080: 6820 6f70 656e 2866 7365 6e63 2866 6e29  h open(fsenc(fn)
+0001b090: 2c20 2272 6222 2920 6173 2066 3a0a 2020  , "rb") as f:.  
+0001b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0b0: 2020 2020 2020 7265 6164 6d65 203d 2066        readme = f
+0001b0c0: 2e72 6561 6428 292e 6465 636f 6465 2822  .read().decode("
+0001b0d0: 7574 662d 3822 290a 2020 2020 2020 2020  utf-8").        
+0001b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0f0: 6272 6561 6b0a 0a20 2020 2020 2020 2076  break..        v
+0001b100: 6620 3d20 766e 2e66 6c61 6773 0a20 2020  f = vn.flags.   
+0001b110: 2020 2020 206c 735f 7265 7420 3d20 7b0a       ls_ret = {.
+0001b120: 2020 2020 2020 2020 2020 2020 2264 6972              "dir
+0001b130: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
+0001b140: 2020 2020 2266 696c 6573 223a 205b 5d2c      "files": [],
+0001b150: 0a20 2020 2020 2020 2020 2020 2022 7461  .            "ta
+0001b160: 676c 6973 7422 3a20 5b5d 2c0a 2020 2020  glist": [],.    
+0001b170: 2020 2020 2020 2020 2273 7276 696e 6622          "srvinf"
+0001b180: 3a20 7372 765f 696e 666f 742c 0a20 2020  : srv_infot,.   
+0001b190: 2020 2020 2020 2020 2022 6163 6374 223a           "acct":
+0001b1a0: 2073 656c 662e 756e 616d 652c 0a20 2020   self.uname,.   
+0001b1b0: 2020 2020 2020 2020 2022 6964 7822 3a20           "idx": 
+0001b1c0: 6532 642c 0a20 2020 2020 2020 2020 2020  e2d,.           
+0001b1d0: 2022 6974 6167 223a 2065 3274 2c0a 2020   "itag": e2t,.  
+0001b1e0: 2020 2020 2020 2020 2020 226c 6966 6574            "lifet
+0001b1f0: 696d 6522 3a20 766e 2e66 6c61 6773 2e67  ime": vn.flags.g
+0001b200: 6574 2822 6c69 6665 7469 6d65 2229 206f  et("lifetime") o
+0001b210: 7220 302c 0a20 2020 2020 2020 2020 2020  r 0,.           
+0001b220: 2022 6672 616e 6422 3a20 626f 6f6c 2876   "frand": bool(v
+0001b230: 6e2e 666c 6167 732e 6765 7428 2272 616e  n.flags.get("ran
+0001b240: 6422 2929 2c0a 2020 2020 2020 2020 2020  d")),.          
+0001b250: 2020 2270 6572 6d73 223a 2070 6572 6d73    "perms": perms
+0001b260: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
+0001b270: 6f67 7565 7322 3a20 6c6f 6775 6573 2c0a  ogues": logues,.
+0001b280: 2020 2020 2020 2020 2020 2020 2272 6561              "rea
+0001b290: 646d 6522 3a20 7265 6164 6d65 2c0a 2020  dme": readme,.  
+0001b2a0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0001b2b0: 6a32 6120 3d20 7b0a 2020 2020 2020 2020  j2a = {.        
+0001b2c0: 2020 2020 2276 6469 7222 3a20 7175 6f74      "vdir": quot
+0001b2d0: 6570 2873 656c 662e 7670 6174 6829 2c0a  ep(self.vpath),.
+0001b2e0: 2020 2020 2020 2020 2020 2020 2276 706e              "vpn
+0001b2f0: 6f64 6573 223a 2076 706e 6f64 6573 2c0a  odes": vpnodes,.
+0001b300: 2020 2020 2020 2020 2020 2020 2266 696c              "fil
+0001b310: 6573 223a 205b 5d2c 0a20 2020 2020 2020  es": [],.       
+0001b320: 2020 2020 2022 6c73 3022 3a20 4e6f 6e65       "ls0": None
+0001b330: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
+0001b340: 6363 7422 3a20 7365 6c66 2e75 6e61 6d65  cct": self.uname
+0001b350: 2c0a 2020 2020 2020 2020 2020 2020 2270  ,.            "p
+0001b360: 6572 6d73 223a 206a 736f 6e2e 6475 6d70  erms": json.dump
+0001b370: 7328 7065 726d 7329 2c0a 2020 2020 2020  s(perms),.      
+0001b380: 2020 2020 2020 226c 6966 6574 696d 6522        "lifetime"
+0001b390: 3a20 6c73 5f72 6574 5b22 6c69 6665 7469  : ls_ret["lifeti
+0001b3a0: 6d65 225d 2c0a 2020 2020 2020 2020 2020  me"],.          
+0001b3b0: 2020 2266 7261 6e64 223a 2062 6f6f 6c28    "frand": bool(
+0001b3c0: 766e 2e66 6c61 6773 2e67 6574 2822 7261  vn.flags.get("ra
+0001b3d0: 6e64 2229 292c 0a20 2020 2020 2020 2020  nd")),.         
+0001b3e0: 2020 2022 7461 676c 6973 7422 3a20 5b5d     "taglist": []
+0001b3f0: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
+0001b400: 6566 5f68 636f 6c73 223a 205b 5d2c 0a20  ef_hcols": [],. 
+0001b410: 2020 2020 2020 2020 2020 2022 6861 7665             "have
+0001b420: 5f65 6d70 223a 2073 656c 662e 6172 6773  _emp": self.args
+0001b430: 2e65 6d70 2c0a 2020 2020 2020 2020 2020  .emp,.          
+0001b440: 2020 2268 6176 655f 7570 326b 5f69 6478    "have_up2k_idx
+0001b450: 223a 2065 3264 2c0a 2020 2020 2020 2020  ": e2d,.        
+0001b460: 2020 2020 2268 6176 655f 7461 6773 5f69      "have_tags_i
+0001b470: 6478 223a 2065 3274 2c0a 2020 2020 2020  dx": e2t,.      
+0001b480: 2020 2020 2020 2268 6176 655f 6163 6f64        "have_acod
+0001b490: 6522 3a20 286e 6f74 2073 656c 662e 6172  e": (not self.ar
+0001b4a0: 6773 2e6e 6f5f 6163 6f64 6529 2c0a 2020  gs.no_acode),.  
+0001b4b0: 2020 2020 2020 2020 2020 2268 6176 655f            "have_
+0001b4c0: 6d76 223a 2028 6e6f 7420 7365 6c66 2e61  mv": (not self.a
+0001b4d0: 7267 732e 6e6f 5f6d 7629 2c0a 2020 2020  rgs.no_mv),.    
+0001b4e0: 2020 2020 2020 2020 2268 6176 655f 6465          "have_de
+0001b4f0: 6c22 3a20 286e 6f74 2073 656c 662e 6172  l": (not self.ar
+0001b500: 6773 2e6e 6f5f 6465 6c29 2c0a 2020 2020  gs.no_del),.    
+0001b510: 2020 2020 2020 2020 2268 6176 655f 7a69          "have_zi
+0001b520: 7022 3a20 286e 6f74 2073 656c 662e 6172  p": (not self.ar
+0001b530: 6773 2e6e 6f5f 7a69 7029 2c0a 2020 2020  gs.no_zip),.    
+0001b540: 2020 2020 2020 2020 2268 6176 655f 756e          "have_un
+0001b550: 706f 7374 223a 2069 6e74 2873 656c 662e  post": int(self.
+0001b560: 6172 6773 2e75 6e70 6f73 7429 2c0a 2020  args.unpost),.  
+0001b570: 2020 2020 2020 2020 2020 2268 6176 655f            "have_
+0001b580: 625f 7522 3a20 2873 656c 662e 6361 6e5f  b_u": (self.can_
+0001b590: 7772 6974 6520 616e 6420 7365 6c66 2e75  write and self.u
+0001b5a0: 7061 7261 6d2e 6765 7428 2262 2229 203d  param.get("b") =
+0001b5b0: 3d20 2275 2229 2c0a 2020 2020 2020 2020  = "u"),.        
+0001b5c0: 2020 2020 2273 625f 6d64 223a 2022 2220      "sb_md": "" 
+0001b5d0: 6966 2022 6e6f 5f73 625f 6d64 2220 696e  if "no_sb_md" in
+0001b5e0: 2076 6620 656c 7365 2028 7666 2e67 6574   vf else (vf.get
+0001b5f0: 2822 6d64 5f73 6266 2229 206f 7220 2279  ("md_sbf") or "y
+0001b600: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+0001b610: 2273 625f 6c67 223a 2022 2220 6966 2022  "sb_lg": "" if "
+0001b620: 6e6f 5f73 625f 6c67 2220 696e 2076 6620  no_sb_lg" in vf 
+0001b630: 656c 7365 2028 7666 2e67 6574 2822 6c67  else (vf.get("lg
+0001b640: 5f73 6266 2229 206f 7220 2279 2229 2c0a  _sbf") or "y"),.
+0001b650: 2020 2020 2020 2020 2020 2020 2275 726c              "url
+0001b660: 5f73 7566 223a 2075 726c 5f73 7566 2c0a  _suf": url_suf,.
+0001b670: 2020 2020 2020 2020 2020 2020 226c 6f67              "log
+0001b680: 7565 7322 3a20 6c6f 6775 6573 2c0a 2020  ues": logues,.  
+0001b690: 2020 2020 2020 2020 2020 2272 6561 646d            "readm
+0001b6a0: 6522 3a20 7265 6164 6d65 2c0a 2020 2020  e": readme,.    
+0001b6b0: 2020 2020 2020 2020 2274 6974 6c65 223a          "title":
+0001b6c0: 2068 746d 6c5f 6573 6361 7065 2873 656c   html_escape(sel
+0001b6d0: 662e 7670 6174 682c 2063 726c 663d 5472  f.vpath, crlf=Tr
+0001b6e0: 7565 2920 6f72 2022 f09f 92be f09f 8e89  ue) or "........
+0001b6f0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+0001b700: 7372 765f 696e 666f 223a 2073 7276 5f69  srv_info": srv_i
+0001b710: 6e66 6f74 2c0a 2020 2020 2020 2020 2020  nfot,.          
+0001b720: 2020 2264 7468 656d 6522 3a20 7365 6c66    "dtheme": self
+0001b730: 2e61 7267 732e 7468 656d 652c 0a20 2020  .args.theme,.   
+0001b740: 2020 2020 2020 2020 2022 7468 656d 6573           "themes
+0001b750: 223a 2073 656c 662e 6172 6773 2e74 6865  ": self.args.the
+0001b760: 6d65 732c 0a20 2020 2020 2020 2020 2020  mes,.           
+0001b770: 2022 7475 7262 6f6c 766c 223a 2073 656c   "turbolvl": sel
+0001b780: 662e 6172 6773 2e74 7572 626f 2c0a 2020  f.args.turbo,.  
+0001b790: 2020 2020 2020 2020 2020 2269 6478 6822            "idxh"
+0001b7a0: 3a20 696e 7428 7365 6c66 2e61 7267 732e  : int(self.args.
+0001b7b0: 6968 292c 0a20 2020 2020 2020 2020 2020  ih),.           
+0001b7c0: 2022 7532 736f 7274 223a 2073 656c 662e   "u2sort": self.
+0001b7d0: 6172 6773 2e75 3273 6f72 742c 0a20 2020  args.u2sort,.   
+0001b7e0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+0001b7f0: 6966 2073 656c 662e 6172 6773 2e6a 735f  if self.args.js_
+0001b800: 6272 6f77 7365 723a 0a20 2020 2020 2020  browser:.       
+0001b810: 2020 2020 206a 3261 5b22 6a73 225d 203d       j2a["js"] =
+0001b820: 2073 656c 662e 6172 6773 2e6a 735f 6272   self.args.js_br
+0001b830: 6f77 7365 720a 0a20 2020 2020 2020 2069  owser..        i
+0001b840: 6620 7365 6c66 2e61 7267 732e 6373 735f  f self.args.css_
+0001b850: 6272 6f77 7365 723a 0a20 2020 2020 2020  browser:.       
+0001b860: 2020 2020 206a 3261 5b22 6373 7322 5d20       j2a["css"] 
+0001b870: 3d20 7365 6c66 2e61 7267 732e 6373 735f  = self.args.css_
+0001b880: 6272 6f77 7365 720a 0a20 2020 2020 2020  browser..       
+0001b890: 2069 6620 6e6f 7420 7365 6c66 2e63 6f6e   if not self.con
+0001b8a0: 6e2e 6873 7276 2e70 7269 736d 3a0a 2020  n.hsrv.prism:.  
+0001b8b0: 2020 2020 2020 2020 2020 6a32 615b 226e            j2a["n
+0001b8c0: 6f5f 7072 6973 6d22 5d20 3d20 5472 7565  o_prism"] = True
+0001b8d0: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+0001b8e0: 2073 656c 662e 6361 6e5f 7265 6164 3a0a   self.can_read:.
+0001b8f0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0001b900: 735f 6c73 3a0a 2020 2020 2020 2020 2020  s_ls:.          
+0001b910: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001b920: 662e 7478 5f6c 7328 6c73 5f72 6574 290a  f.tx_ls(ls_ret).
+0001b930: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001b940: 6e6f 7420 7374 6174 2e53 5f49 5344 4952  not stat.S_ISDIR
+0001b950: 2873 742e 7374 5f6d 6f64 6529 3a0a 2020  (st.st_mode):.  
+0001b960: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001b970: 7475 726e 2073 656c 662e 7478 5f34 3034  turn self.tx_404
+0001b980: 2854 7275 6529 0a0a 2020 2020 2020 2020  (True)..        
+0001b990: 2020 2020 6966 2022 7a69 7022 2069 6e20      if "zip" in 
+0001b9a0: 7365 6c66 2e75 7061 7261 6d20 6f72 2022  self.uparam or "
+0001b9b0: 7461 7222 2069 6e20 7365 6c66 2e75 7061  tar" in self.upa
+0001b9c0: 7261 6d3a 0a20 2020 2020 2020 2020 2020  ram:.           
+0001b9d0: 2020 2020 2072 6169 7365 2050 6562 6b61       raise Pebka
+0001b9e0: 6328 3430 3329 0a0a 2020 2020 2020 2020  c(403)..        
+0001b9f0: 2020 2020 6874 6d6c 203d 2073 656c 662e      html = self.
+0001ba00: 6a32 7328 7470 6c2c 202a 2a6a 3261 290a  j2s(tpl, **j2a).
+0001ba10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001ba20: 2e72 6570 6c79 2868 746d 6c2e 656e 636f  .reply(html.enco
+0001ba30: 6465 2822 7574 662d 3822 2c20 2272 6570  de("utf-8", "rep
+0001ba40: 6c61 6365 2229 290a 2020 2020 2020 2020  lace")).        
+0001ba50: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0001ba60: 0a20 2020 2020 2020 2066 6f72 206b 2069  .        for k i
+0001ba70: 6e20 5b22 7a69 7022 2c20 2274 6172 225d  n ["zip", "tar"]
+0001ba80: 3a0a 2020 2020 2020 2020 2020 2020 7620  :.            v 
+0001ba90: 3d20 7365 6c66 2e75 7061 7261 6d2e 6765  = self.uparam.ge
+0001baa0: 7428 6b29 0a20 2020 2020 2020 2020 2020  t(k).           
+0001bab0: 2069 6620 7620 6973 206e 6f74 204e 6f6e   if v is not Non
+0001bac0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001bad0: 2020 2072 6574 7572 6e20 7365 6c66 2e74     return self.t
+0001bae0: 785f 7a69 7028 6b2c 2076 2c20 766e 2c20  x_zip(k, v, vn, 
+0001baf0: 7265 6d2c 205b 5d2c 2073 656c 662e 6172  rem, [], self.ar
+0001bb00: 6773 2e65 6429 0a0a 2020 2020 2020 2020  gs.ed)..        
+0001bb10: 6673 726f 6f74 2c20 7666 735f 6c73 2c20  fsroot, vfs_ls, 
+0001bb20: 7666 735f 7669 7274 203d 2076 6e2e 6c73  vfs_virt = vn.ls
+0001bb30: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+0001bb40: 6d2c 2073 656c 662e 756e 616d 652c 206e  m, self.uname, n
+0001bb50: 6f74 2073 656c 662e 6172 6773 2e6e 6f5f  ot self.args.no_
+0001bb60: 7363 616e 6469 722c 205b 5b54 7275 652c  scandir, [[True,
+0001bb70: 2046 616c 7365 5d2c 205b 4661 6c73 652c   False], [False,
+0001bb80: 2054 7275 655d 5d0a 2020 2020 2020 2020   True]].        
+0001bb90: 290a 2020 2020 2020 2020 7374 6174 7320  ).        stats 
+0001bba0: 3d20 7b6b 3a20 7620 666f 7220 6b2c 2076  = {k: v for k, v
+0001bbb0: 2069 6e20 7666 735f 6c73 7d0a 2020 2020   in vfs_ls}.    
+0001bbc0: 2020 2020 6c73 5f6e 616d 6573 203d 205b      ls_names = [
+0001bbd0: 785b 305d 2066 6f72 2078 2069 6e20 7666  x[0] for x in vf
+0001bbe0: 735f 6c73 5d0a 2020 2020 2020 2020 6c73  s_ls].        ls
+0001bbf0: 5f6e 616d 6573 2e65 7874 656e 6428 6c69  _names.extend(li
+0001bc00: 7374 2876 6673 5f76 6972 742e 6b65 7973  st(vfs_virt.keys
+0001bc10: 2829 2929 0a0a 2020 2020 2020 2020 2320  ()))..        # 
+0001bc20: 6368 6563 6b20 666f 7220 6f6c 6420 7665  check for old ve
+0001bc30: 7273 696f 6e73 206f 6620 6669 6c65 732c  rsions of files,
+0001bc40: 0a20 2020 2020 2020 2023 205b 6e75 6d2d  .        # [num-
+0001bc50: 6261 636b 7570 732c 206d 6f73 742d 7265  backups, most-re
+0001bc60: 6365 6e74 2c20 6869 7374 2d70 6174 685d  cent, hist-path]
+0001bc70: 0a20 2020 2020 2020 2068 6973 7420 2020  .        hist   
+0001bc80: 2020 3d20 7b7d 0a20 2020 2020 2020 2068    = {}.        h
+0001bc90: 6973 7464 6972 203d 206f 732e 7061 7468  istdir = os.path
+0001bca0: 2e6a 6f69 6e28 6673 726f 6f74 2c20 222e  .join(fsroot, ".
+0001bcb0: 6869 7374 2229 0a20 2020 2020 2020 2070  hist").        p
+0001bcc0: 746e 203d 2072 652e 636f 6d70 696c 6528  tn = re.compile(
+0001bcd0: 7222 282e 2a29 5c2e 285b 302d 395d 2b5c  r"(.*)\.([0-9]+\
+0001bce0: 2e5b 302d 395d 7b33 7d29 285c 2e5b 5e5c  .[0-9]{3})(\.[^\
+0001bcf0: 2e5d 2b29 2422 290a 2020 2020 2020 2020  .]+)$").        
+0001bd00: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0001bd10: 2066 6f72 2068 666e 2069 6e20 626f 732e   for hfn in bos.
+0001bd20: 6c69 7374 6469 7228 6869 7374 6469 7229  listdir(histdir)
+0001bd30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001bd40: 2020 6d20 3d20 7074 6e2e 6d61 7463 6828    m = ptn.match(
+0001bd50: 6866 6e29 0a20 2020 2020 2020 2020 2020  hfn).           
+0001bd60: 2020 2020 2069 6620 6e6f 7420 6d3a 0a20       if not m:. 
+0001bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd80: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
+0001bd90: 2020 2020 2020 2020 2020 2020 2066 6e20               fn 
+0001bda0: 3d20 6d2e 6772 6f75 7028 3129 202b 206d  = m.group(1) + m
+0001bdb0: 2e67 726f 7570 2833 290a 2020 2020 2020  .group(3).      
+0001bdc0: 2020 2020 2020 2020 2020 6e2c 2074 732c            n, ts,
+0001bdd0: 205f 203d 2068 6973 742e 6765 7428 666e   _ = hist.get(fn
+0001bde0: 2c20 2830 2c20 302c 2022 2229 290a 2020  , (0, 0, "")).  
+0001bdf0: 2020 2020 2020 2020 2020 2020 2020 6869                hi
+0001be00: 7374 5b66 6e5d 203d 2028 6e20 2b20 312c  st[fn] = (n + 1,
+0001be10: 206d 6178 2874 732c 2066 6c6f 6174 286d   max(ts, float(m
+0001be20: 2e67 726f 7570 2832 2929 292c 2068 666e  .group(2))), hfn
+0001be30: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+0001be40: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+0001be50: 7373 0a0a 2020 2020 2020 2020 2320 7368  ss..        # sh
+0001be60: 6f77 2064 6f74 6669 6c65 7320 6966 2070  ow dotfiles if p
+0001be70: 6572 6d69 7474 6564 2061 6e64 2072 6571  ermitted and req
+0001be80: 7565 7374 6564 0a20 2020 2020 2020 2069  uested.        i
+0001be90: 6620 6e6f 7420 7365 6c66 2e61 7267 732e  f not self.args.
+0001bea0: 6564 206f 7220 2264 6f74 7322 206e 6f74  ed or "dots" not
+0001beb0: 2069 6e20 7365 6c66 2e75 7061 7261 6d3a   in self.uparam:
+0001bec0: 0a20 2020 2020 2020 2020 2020 206c 735f  .            ls_
+0001bed0: 6e61 6d65 7320 3d20 6578 636c 7564 655f  names = exclude_
+0001bee0: 646f 7466 696c 6573 286c 735f 6e61 6d65  dotfiles(ls_name
+0001bef0: 7329 0a0a 2020 2020 2020 2020 6164 645f  s)..        add_
+0001bf00: 666b 203d 2076 6e2e 666c 6167 732e 6765  fk = vn.flags.ge
+0001bf10: 7428 2266 6b22 290a 0a20 2020 2020 2020  t("fk")..       
+0001bf20: 2064 6972 7320 3d20 5b5d 0a20 2020 2020   dirs = [].     
+0001bf30: 2020 2066 696c 6573 203d 205b 5d0a 2020     files = [].  
+0001bf40: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
+0001bf50: 6c73 5f6e 616d 6573 3a0a 2020 2020 2020  ls_names:.      
+0001bf60: 2020 2020 2020 6261 7365 203d 2022 220a        base = "".
+0001bf70: 2020 2020 2020 2020 2020 2020 6872 6566              href
+0001bf80: 203d 2066 6e0a 2020 2020 2020 2020 2020   = fn.          
+0001bf90: 2020 6966 206e 6f74 2069 735f 6c73 2061    if not is_ls a
+0001bfa0: 6e64 206e 6f74 2069 735f 6a73 2061 6e64  nd not is_js and
+0001bfb0: 206e 6f74 2073 656c 662e 7472 6169 6c69   not self.traili
+0001bfc0: 6e67 5f73 6c61 7368 2061 6e64 2076 7061  ng_slash and vpa
+0001bfd0: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
+0001bfe0: 2020 2020 6261 7365 203d 2022 2f22 202b      base = "/" +
+0001bff0: 2076 7061 7468 202b 2022 2f22 0a20 2020   vpath + "/".   
+0001c000: 2020 2020 2020 2020 2020 2020 2068 7265               hre
+0001c010: 6620 3d20 6261 7365 202b 2066 6e0a 0a20  f = base + fn.. 
+0001c020: 2020 2020 2020 2020 2020 2069 6620 666e             if fn
+0001c030: 2069 6e20 7666 735f 7669 7274 3a0a 2020   in vfs_virt:.  
+0001c040: 2020 2020 2020 2020 2020 2020 2020 6673                fs
+0001c050: 7061 7468 203d 2076 6673 5f76 6972 745b  path = vfs_virt[
+0001c060: 666e 5d2e 7265 616c 7061 7468 0a20 2020  fn].realpath.   
+0001c070: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0001c080: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001c090: 7370 6174 6820 3d20 6673 726f 6f74 202b  spath = fsroot +
+0001c0a0: 2022 2f22 202b 2066 6e0a 0a20 2020 2020   "/" + fn..     
+0001c0b0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0001c0c0: 2020 2020 2020 2020 2020 2020 696e 6620              inf 
+0001c0d0: 3d20 7374 6174 732e 6765 7428 666e 2920  = stats.get(fn) 
+0001c0e0: 6f72 2062 6f73 2e73 7461 7428 6673 7061  or bos.stat(fspa
+0001c0f0: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
+0001c100: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+0001c110: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+0001c120: 2822 6272 6f6b 656e 2073 796d 6c69 6e6b  ("broken symlink
+0001c130: 3a20 7b7d 222e 666f 726d 6174 2872 6570  : {}".format(rep
+0001c140: 7228 6673 7061 7468 2929 290a 2020 2020  r(fspath))).    
+0001c150: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0001c160: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
+0001c170: 2020 6973 5f64 6972 203d 2073 7461 742e    is_dir = stat.
+0001c180: 535f 4953 4449 5228 696e 662e 7374 5f6d  S_ISDIR(inf.st_m
+0001c190: 6f64 6529 0a20 2020 2020 2020 2020 2020  ode).           
+0001c1a0: 2069 6620 6973 5f64 6972 3a0a 2020 2020   if is_dir:.    
+0001c1b0: 2020 2020 2020 2020 2020 2020 6872 6566              href
+0001c1c0: 202b 3d20 222f 220a 2020 2020 2020 2020   += "/".        
+0001c1d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001c1e0: 6172 6773 2e6e 6f5f 7a69 703a 0a20 2020  args.no_zip:.   
+0001c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c200: 206d 6172 6769 6e20 3d20 2244 4952 220a   margin = "DIR".
+0001c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c220: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001c230: 2020 2020 2020 2020 2020 6d61 7267 696e            margin
+0001c240: 203d 2027 3c61 2068 7265 663d 227b 7d3f   = '<a href="{}?
+0001c250: 7a69 7022 2072 656c 3d22 6e6f 666f 6c6c  zip" rel="nofoll
+0001c260: 6f77 223e 7a69 703c 2f61 3e27 2e66 6f72  ow">zip</a>'.for
+0001c270: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+0001c280: 2020 2020 2020 2020 2020 2020 2071 756f               quo
+0001c290: 7465 7028 6872 6566 290a 2020 2020 2020  tep(href).      
+0001c2a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0001c2b0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0001c2c0: 2066 6e20 696e 2068 6973 743a 0a20 2020   fn in hist:.   
+0001c2d0: 2020 2020 2020 2020 2020 2020 206d 6172               mar
+0001c2e0: 6769 6e20 3d20 273c 6120 6872 6566 3d22  gin = '<a href="
+0001c2f0: 7b7d 2e68 6973 742f 7b7d 223e 237b 7d3c  {}.hist/{}">#{}<
+0001c300: 2f61 3e27 2e66 6f72 6d61 7428 0a20 2020  /a>'.format(.   
+0001c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c320: 2062 6173 652c 2068 746d 6c5f 6573 6361   base, html_esca
+0001c330: 7065 2868 6973 745b 666e 5d5b 325d 2c20  pe(hist[fn][2], 
+0001c340: 7175 6f74 3d54 7275 652c 2063 726c 663d  quot=True, crlf=
+0001c350: 5472 7565 292c 2068 6973 745b 666e 5d5b  True), hist[fn][
+0001c360: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+0001c370: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0001c380: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001c390: 2020 2020 2020 206d 6172 6769 6e20 3d20         margin = 
+0001c3a0: 222d 220a 0a20 2020 2020 2020 2020 2020  "-"..           
+0001c3b0: 2073 7a20 3d20 696e 662e 7374 5f73 697a   sz = inf.st_siz
+0001c3c0: 650a 2020 2020 2020 2020 2020 2020 7a64  e.            zd
+0001c3d0: 203d 2064 6174 6574 696d 652e 7574 6366   = datetime.utcf
+0001c3e0: 726f 6d74 696d 6573 7461 6d70 2869 6e66  romtimestamp(inf
+0001c3f0: 2e73 745f 6d74 696d 6529 0a20 2020 2020  .st_mtime).     
+0001c400: 2020 2020 2020 2064 7420 3d20 7a64 2e73         dt = zd.s
+0001c410: 7472 6674 696d 6528 2225 592d 256d 2d25  trftime("%Y-%m-%
+0001c420: 6420 2548 3a25 4d3a 2553 2229 0a0a 2020  d %H:%M:%S")..  
+0001c430: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+0001c440: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001c450: 7874 203d 2022 2d2d 2d22 2069 6620 6973  xt = "---" if is
+0001c460: 5f64 6972 2065 6c73 6520 666e 2e72 7370  _dir else fn.rsp
+0001c470: 6c69 7428 222e 222c 2031 295b 315d 0a20  lit(".", 1)[1]. 
+0001c480: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001c490: 6620 6c65 6e28 6578 7429 203e 2031 363a  f len(ext) > 16:
+0001c4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c4b0: 2020 2020 2065 7874 203d 2065 7874 5b3a       ext = ext[:
+0001c4c0: 3136 5d0a 2020 2020 2020 2020 2020 2020  16].            
+0001c4d0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+0001c4e0: 2020 2020 2020 2020 6578 7420 3d20 2225          ext = "%
+0001c4f0: 220a 0a20 2020 2020 2020 2020 2020 2069  "..            i
+0001c500: 6620 6164 645f 666b 3a0a 2020 2020 2020  f add_fk:.      
+0001c510: 2020 2020 2020 2020 2020 6872 6566 203d            href =
+0001c520: 2022 7b7d 3f6b 3d7b 7d22 2e66 6f72 6d61   "{}?k={}".forma
+0001c530: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0001c540: 2020 2020 2020 2071 756f 7465 7028 6872         quotep(hr
+0001c550: 6566 292c 0a20 2020 2020 2020 2020 2020  ef),.           
+0001c560: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+0001c570: 6e5f 666b 280a 2020 2020 2020 2020 2020  n_fk(.          
+0001c580: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001c590: 6c66 2e61 7267 732e 666b 5f73 616c 742c  lf.args.fk_salt,
+0001c5a0: 2066 7370 6174 682c 2073 7a2c 2030 2069   fspath, sz, 0 i
+0001c5b0: 6620 414e 5957 494e 2065 6c73 6520 696e  f ANYWIN else in
+0001c5c0: 662e 7374 5f69 6e6f 0a20 2020 2020 2020  f.st_ino.       
+0001c5d0: 2020 2020 2020 2020 2020 2020 2029 5b3a               )[:
+0001c5e0: 6164 645f 666b 5d2c 0a20 2020 2020 2020  add_fk],.       
+0001c5f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0001c600: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001c610: 2020 2020 2020 2020 2020 2020 2068 7265               hre
+0001c620: 6620 3d20 7175 6f74 6570 2868 7265 6629  f = quotep(href)
+0001c630: 0a0a 2020 2020 2020 2020 2020 2020 6974  ..            it
+0001c640: 656d 203d 207b 0a20 2020 2020 2020 2020  em = {.         
+0001c650: 2020 2020 2020 2022 6c65 6164 223a 206d         "lead": m
+0001c660: 6172 6769 6e2c 0a20 2020 2020 2020 2020  argin,.         
+0001c670: 2020 2020 2020 2022 6872 6566 223a 2068         "href": h
+0001c680: 7265 662c 0a20 2020 2020 2020 2020 2020  ref,.           
+0001c690: 2020 2020 2022 6e61 6d65 223a 2066 6e2c       "name": fn,
+0001c6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c6b0: 2022 737a 223a 2073 7a2c 0a20 2020 2020   "sz": sz,.     
+0001c6c0: 2020 2020 2020 2020 2020 2022 6578 7422             "ext"
+0001c6d0: 3a20 6578 742c 0a20 2020 2020 2020 2020  : ext,.         
+0001c6e0: 2020 2020 2020 2022 6474 223a 2064 742c         "dt": dt,
+0001c6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c700: 2022 7473 223a 2069 6e74 2869 6e66 2e73   "ts": int(inf.s
+0001c710: 745f 6d74 696d 6529 2c0a 2020 2020 2020  t_mtime),.      
+0001c720: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0001c730: 2020 2020 6966 2069 735f 6469 723a 0a20      if is_dir:. 
+0001c740: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001c750: 6972 732e 6170 7065 6e64 2869 7465 6d29  irs.append(item)
+0001c760: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0001c770: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001c780: 2020 2066 696c 6573 2e61 7070 656e 6428     files.append(
+0001c790: 6974 656d 290a 2020 2020 2020 2020 2020  item).          
+0001c7a0: 2020 2020 2020 6974 656d 5b22 7264 225d        item["rd"]
+0001c7b0: 203d 2072 656d 0a0a 2020 2020 2020 2020   = rem..        
+0001c7c0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
+0001c7d0: 2073 656c 662e 636f 6f6b 6965 732e 6765   self.cookies.ge
+0001c7e0: 7428 2269 6478 6822 2920 3d3d 2022 7922  t("idxh") == "y"
+0001c7f0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001c800: 2022 6c73 2220 6e6f 7420 696e 2073 656c   "ls" not in sel
+0001c810: 662e 7570 6172 616d 0a20 2020 2020 2020  f.uparam.       
+0001c820: 2020 2020 2061 6e64 2022 7622 206e 6f74       and "v" not
+0001c830: 2069 6e20 7365 6c66 2e75 7061 7261 6d0a   in self.uparam.
+0001c840: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+0001c850: 2020 2020 2020 2069 6478 5f68 746d 6c20         idx_html 
+0001c860: 3d20 7365 7428 5b22 696e 6465 782e 6874  = set(["index.ht
+0001c870: 6d22 2c20 2269 6e64 6578 2e68 746d 6c22  m", "index.html"
+0001c880: 5d29 0a20 2020 2020 2020 2020 2020 2066  ]).            f
+0001c890: 6f72 2069 7465 6d20 696e 2066 696c 6573  or item in files
+0001c8a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001c8b0: 2020 6966 2069 7465 6d5b 226e 616d 6522    if item["name"
+0001c8c0: 5d20 696e 2069 6478 5f68 746d 6c3a 0a20  ] in idx_html:. 
+0001c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c8e0: 2020 2023 2064 6f20 6675 6c6c 2072 6573     # do full res
+0001c8f0: 6f6c 7665 2069 6e20 6361 7365 206f 6620  olve in case of 
+0001c900: 7368 6164 6f77 6564 2066 696c 650a 2020  shadowed file.  
+0001c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c920: 2020 7670 203d 2076 6a6f 696e 2873 656c    vp = vjoin(sel
+0001c930: 662e 7670 6174 682e 7370 6c69 7428 223f  f.vpath.split("?
+0001c940: 2229 5b30 5d2c 2069 7465 6d5b 226e 616d  ")[0], item["nam
+0001c950: 6522 5d29 0a20 2020 2020 2020 2020 2020  e"]).           
+0001c960: 2020 2020 2020 2020 2076 6e2c 2072 656d           vn, rem
+0001c970: 203d 2073 656c 662e 6173 7276 2e76 6673   = self.asrv.vfs
+0001c980: 2e67 6574 2876 702c 2073 656c 662e 756e  .get(vp, self.un
+0001c990: 616d 652c 2054 7275 652c 2046 616c 7365  ame, True, False
+0001c9a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001c9b0: 2020 2020 2020 6170 203d 2076 6e2e 6361        ap = vn.ca
+0001c9c0: 6e6f 6e69 6361 6c28 7265 6d29 0a20 2020  nonical(rem).   
+0001c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c9e0: 2072 6574 7572 6e20 7365 6c66 2e74 785f   return self.tx_
+0001c9f0: 6669 6c65 2861 7029 2020 2320 6973 206e  file(ap)  # is n
+0001ca00: 6f2d 6361 6368 650a 0a20 2020 2020 2020  o-cache..       
+0001ca10: 2074 6167 7365 7420 203d 2073 6574 2829   tagset  = set()
+0001ca20: 0a20 2020 2020 2020 2066 6f72 2066 6520  .        for fe 
+0001ca30: 696e 2066 696c 6573 3a0a 2020 2020 2020  in files:.      
+0001ca40: 2020 2020 2020 666e 203d 2066 655b 226e        fn = fe["n
+0001ca50: 616d 6522 5d0a 2020 2020 2020 2020 2020  ame"].          
+0001ca60: 2020 7264 203d 2066 655b 2272 6422 5d0a    rd = fe["rd"].
+0001ca70: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
+0001ca80: 6665 5b22 7264 225d 0a20 2020 2020 2020  fe["rd"].       
+0001ca90: 2020 2020 2069 6620 6e6f 7420 6963 7572       if not icur
+0001caa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001cab0: 2020 636f 6e74 696e 7565 0a0a 2020 2020    continue..    
+0001cac0: 2020 2020 2020 2020 6966 2076 6e20 213d          if vn !=
+0001cad0: 2064 6276 3a0a 2020 2020 2020 2020 2020   dbv:.          
+0001cae0: 2020 2020 2020 5f2c 2072 6420 3d20 766e        _, rd = vn
+0001caf0: 2e67 6574 5f64 6276 2872 6429 0a0a 2020  .get_dbv(rd)..  
+0001cb00: 2020 2020 2020 2020 2020 7120 3d20 2273            q = "s
+0001cb10: 656c 6563 7420 6d74 2e6b 2c20 6d74 2e76  elect mt.k, mt.v
+0001cb20: 2066 726f 6d20 7570 2069 6e6e 6572 206a   from up inner j
+0001cb30: 6f69 6e20 6d74 206f 6e20 6d74 2e77 203d  oin mt on mt.w =
+0001cb40: 2073 7562 7374 7228 7570 2e77 2c31 2c31   substr(up.w,1,1
+0001cb50: 3629 2077 6865 7265 2075 702e 7264 203d  6) where up.rd =
+0001cb60: 203f 2061 6e64 2075 702e 666e 203d 203f   ? and up.fn = ?
+0001cb70: 2061 6e64 202b 6d74 2e6b 2021 3d20 2778   and +mt.k != 'x
+0001cb80: 2722 0a20 2020 2020 2020 2020 2020 2074  '".            t
+0001cb90: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0001cba0: 2020 2020 7220 3d20 6963 7572 2e65 7865      r = icur.exe
+0001cbb0: 6375 7465 2871 2c20 2872 642c 2066 6e29  cute(q, (rd, fn)
+0001cbc0: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+0001cbd0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+0001cbe0: 7320 6578 3a0a 2020 2020 2020 2020 2020  s ex:.          
+0001cbf0: 2020 2020 2020 6966 2022 6461 7461 6261        if "databa
+0001cc00: 7365 2069 7320 6c6f 636b 6564 2220 696e  se is locked" in
+0001cc10: 2073 7472 2865 7829 3a0a 2020 2020 2020   str(ex):.      
+0001cc20: 2020 2020 2020 2020 2020 2020 2020 6272                br
+0001cc30: 6561 6b0a 0a20 2020 2020 2020 2020 2020  eak..           
+0001cc40: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0001cc50: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+0001cc60: 6773 203d 2073 3365 6e63 2869 6478 2e6d  gs = s3enc(idx.m
+0001cc70: 656d 5f63 7572 2c20 7264 2c20 666e 290a  em_cur, rd, fn).
+0001cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cc90: 2020 2020 7220 3d20 6963 7572 2e65 7865      r = icur.exe
+0001cca0: 6375 7465 2871 2c20 6172 6773 290a 2020  cute(q, args).  
+0001ccb0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0001ccc0: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+0001ccd0: 2020 2020 2020 2020 2020 7420 3d20 2274            t = "t
+0001cce0: 6167 2072 6561 6420 6572 726f 722c 207b  ag read error, {
+0001ccf0: 7d2f 7b7d 5c6e 7b7d 220a 2020 2020 2020  }/{}\n{}".      
+0001cd00: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001cd10: 6c66 2e6c 6f67 2874 2e66 6f72 6d61 7428  lf.log(t.format(
+0001cd20: 7264 2c20 666e 2c20 6d69 6e5f 6578 2829  rd, fn, min_ex()
+0001cd30: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0001cd40: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+0001cd50: 2020 2020 2020 2020 2020 6665 5b22 7461            fe["ta
+0001cd60: 6773 225d 203d 207b 6b3a 2076 2066 6f72  gs"] = {k: v for
+0001cd70: 206b 2c20 7620 696e 2072 7d0a 2020 2020   k, v in r}.    
+0001cd80: 2020 2020 2020 2020 5f20 3d20 5b74 6167          _ = [tag
+0001cd90: 7365 742e 6164 6428 6b29 2066 6f72 206b  set.add(k) for k
+0001cda0: 2069 6e20 6665 5b22 7461 6773 225d 5d0a   in fe["tags"]].
+0001cdb0: 0a20 2020 2020 2020 2069 6620 6963 7572  .        if icur
+0001cdc0: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
+0001cdd0: 676c 6973 7420 3d20 5b6b 2066 6f72 206b  glist = [k for k
+0001cde0: 2069 6e20 766e 2e66 6c61 6773 2e67 6574   in vn.flags.get
+0001cdf0: 2822 6d74 6522 2c20 2222 292e 7370 6c69  ("mte", "").spli
+0001ce00: 7428 222c 2229 2069 6620 6b20 696e 2074  t(",") if k in t
+0001ce10: 6167 7365 745d 0a20 2020 2020 2020 2020  agset].         
+0001ce20: 2020 2066 6f72 2066 6520 696e 2064 6972     for fe in dir
+0001ce30: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0001ce40: 2020 2066 655b 2274 6167 7322 5d20 3d20     fe["tags"] = 
+0001ce50: 7b7d 0a20 2020 2020 2020 2065 6c73 653a  {}.        else:
+0001ce60: 0a20 2020 2020 2020 2020 2020 2074 6167  .            tag
+0001ce70: 6c69 7374 203d 206c 6973 7428 7461 6773  list = list(tags
+0001ce80: 6574 290a 0a20 2020 2020 2020 2069 6620  et)..        if 
+0001ce90: 6973 5f6c 733a 0a20 2020 2020 2020 2020  is_ls:.         
+0001cea0: 2020 206c 735f 7265 745b 2264 6972 7322     ls_ret["dirs"
+0001ceb0: 5d20 3d20 6469 7273 0a20 2020 2020 2020  ] = dirs.       
+0001cec0: 2020 2020 206c 735f 7265 745b 2266 696c       ls_ret["fil
+0001ced0: 6573 225d 203d 2066 696c 6573 0a20 2020  es"] = files.   
+0001cee0: 2020 2020 2020 2020 206c 735f 7265 745b           ls_ret[
+0001cef0: 2274 6167 6c69 7374 225d 203d 2074 6167  "taglist"] = tag
+0001cf00: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
+0001cf10: 2072 6574 7572 6e20 7365 6c66 2e74 785f   return self.tx_
+0001cf20: 6c73 286c 735f 7265 7429 0a0a 2020 2020  ls(ls_ret)..    
+0001cf30: 2020 2020 646f 6320 3d20 7365 6c66 2e75      doc = self.u
+0001cf40: 7061 7261 6d2e 6765 7428 2264 6f63 2229  param.get("doc")
+0001cf50: 2069 6620 7365 6c66 2e63 616e 5f72 6561   if self.can_rea
+0001cf60: 6420 656c 7365 204e 6f6e 650a 2020 2020  d else None.    
+0001cf70: 2020 2020 6966 2064 6f63 3a0a 2020 2020      if doc:.    
+0001cf80: 2020 2020 2020 2020 646f 6320 3d20 756e          doc = un
+0001cf90: 7175 6f74 6570 2864 6f63 2e72 6570 6c61  quotep(doc.repla
+0001cfa0: 6365 2822 2b22 2c20 2220 2229 2e73 706c  ce("+", " ").spl
+0001cfb0: 6974 2822 3f22 295b 305d 290a 2020 2020  it("?")[0]).    
+0001cfc0: 2020 2020 2020 2020 6a32 615b 2264 6f63          j2a["doc
+0001cfd0: 6e61 6d65 225d 203d 2064 6f63 0a20 2020  name"] = doc.   
+0001cfe0: 2020 2020 2020 2020 2064 6f63 7478 7420           doctxt 
+0001cff0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0001d000: 2020 2069 6620 6e65 7874 2828 7820 666f     if next((x fo
+0001d010: 7220 7820 696e 2066 696c 6573 2069 6620  r x in files if 
+0001d020: 785b 226e 616d 6522 5d20 3d3d 2064 6f63  x["name"] == doc
+0001d030: 292c 204e 6f6e 6529 3a0a 2020 2020 2020  ), None):.      
+0001d040: 2020 2020 2020 2020 2020 646f 6370 6174            docpat
+0001d050: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+0001d060: 2861 6273 7061 7468 2c20 646f 6329 0a20  (abspath, doc). 
+0001d070: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001d080: 7a20 3d20 626f 732e 7061 7468 2e67 6574  z = bos.path.get
+0001d090: 7369 7a65 2864 6f63 7061 7468 290a 2020  size(docpath).  
+0001d0a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001d0b0: 2073 7a20 3c20 3130 3234 202a 2073 656c   sz < 1024 * sel
+0001d0c0: 662e 6172 6773 2e74 7874 5f6d 6178 3a0a  f.args.txt_max:.
+0001d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d0e0: 2020 2020 7769 7468 206f 7065 6e28 6673      with open(fs
+0001d0f0: 656e 6328 646f 6370 6174 6829 2c20 2272  enc(docpath), "r
+0001d100: 6222 2920 6173 2066 3a0a 2020 2020 2020  b") as f:.      
+0001d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d120: 2020 646f 6374 7874 203d 2066 2e72 6561    doctxt = f.rea
+0001d130: 6428 292e 6465 636f 6465 2822 7574 662d  d().decode("utf-
+0001d140: 3822 2c20 2272 6570 6c61 6365 2229 0a20  8", "replace"). 
+0001d150: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001d160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d170: 2073 656c 662e 6c6f 6728 2264 6f63 2034   self.log("doc 4
+0001d180: 3034 3a20 5b7b 7d5d 222e 666f 726d 6174  04: [{}]".format
+0001d190: 2864 6f63 292c 2063 3d36 290a 2020 2020  (doc), c=6).    
+0001d1a0: 2020 2020 2020 2020 2020 2020 646f 6374              doct
+0001d1b0: 7874 203d 2022 2820 7465 7874 6669 6c65  xt = "( textfile
+0001d1c0: 206e 6f74 2066 6f75 6e64 2029 220a 0a20   not found )".. 
+0001d1d0: 2020 2020 2020 2020 2020 2069 6620 646f             if do
+0001d1e0: 6374 7874 2069 7320 6e6f 7420 4e6f 6e65  ctxt is not None
+0001d1f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001d200: 2020 6a32 615b 2264 6f63 225d 203d 2064    j2a["doc"] = d
+0001d210: 6f63 7478 740a 0a20 2020 2020 2020 2066  octxt..        f
+0001d220: 6f72 2064 2069 6e20 6469 7273 3a0a 2020  or d in dirs:.  
+0001d230: 2020 2020 2020 2020 2020 645b 226e 616d            d["nam
+0001d240: 6522 5d20 2b3d 2022 2f22 0a0a 2020 2020  e"] += "/"..    
+0001d250: 2020 2020 6469 7273 2e73 6f72 7428 6b65      dirs.sort(ke
+0001d260: 793d 6974 656d 6765 7474 6572 2822 6e61  y=itemgetter("na
+0001d270: 6d65 2229 290a 0a20 2020 2020 2020 2069  me"))..        i
+0001d280: 6620 6973 5f6a 733a 0a20 2020 2020 2020  f is_js:.       
+0001d290: 2020 2020 206a 3261 5b22 6c73 3022 5d20       j2a["ls0"] 
+0001d2a0: 3d20 7b22 6469 7273 223a 2064 6972 732c  = {"dirs": dirs,
+0001d2b0: 2022 6669 6c65 7322 3a20 6669 6c65 732c   "files": files,
+0001d2c0: 2022 7461 676c 6973 7422 3a20 7461 676c   "taglist": tagl
+0001d2d0: 6973 747d 0a20 2020 2020 2020 2020 2020  ist}.           
+0001d2e0: 206a 3261 5b22 6669 6c65 7322 5d20 3d20   j2a["files"] = 
+0001d2f0: 5b5d 0a20 2020 2020 2020 2065 6c73 653a  [].        else:
+0001d300: 0a20 2020 2020 2020 2020 2020 206a 3261  .            j2a
+0001d310: 5b22 6669 6c65 7322 5d20 3d20 6469 7273  ["files"] = dirs
+0001d320: 202b 2066 696c 6573 0a0a 2020 2020 2020   + files..      
+0001d330: 2020 6a32 615b 2274 6167 6c69 7374 225d    j2a["taglist"]
+0001d340: 203d 2074 6167 6c69 7374 0a20 2020 2020   = taglist.     
+0001d350: 2020 206a 3261 5b22 7478 745f 6578 7422     j2a["txt_ext"
+0001d360: 5d20 3d20 7365 6c66 2e61 7267 732e 7465  ] = self.args.te
+0001d370: 7874 6669 6c65 732e 7265 706c 6163 6528  xtfiles.replace(
+0001d380: 222c 222c 2022 2022 290a 0a20 2020 2020  ",", " ")..     
+0001d390: 2020 2069 6620 226d 7468 2220 696e 2076     if "mth" in v
+0001d3a0: 6e2e 666c 6167 733a 0a20 2020 2020 2020  n.flags:.       
+0001d3b0: 2020 2020 206a 3261 5b22 6465 665f 6863       j2a["def_hc
+0001d3c0: 6f6c 7322 5d20 3d20 766e 2e66 6c61 6773  ols"] = vn.flags
+0001d3d0: 5b22 6d74 6822 5d2e 7370 6c69 7428 222c  ["mth"].split(",
+0001d3e0: 2229 0a0a 2020 2020 2020 2020 6874 6d6c  ")..        html
+0001d3f0: 203d 2073 656c 662e 6a32 7328 7470 6c2c   = self.j2s(tpl,
+0001d400: 202a 2a6a 3261 290a 2020 2020 2020 2020   **j2a).        
+0001d410: 7365 6c66 2e72 6570 6c79 2868 746d 6c2e  self.reply(html.
+0001d420: 656e 636f 6465 2822 7574 662d 3822 2c20  encode("utf-8", 
+0001d430: 2272 6570 6c61 6365 2229 290a 2020 2020  "replace")).    
+0001d440: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
```

### Comparing `copyparty-1.6.8/copyparty/httpconn.py` & `copyparty-1.6.9/copyparty/httpconn.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/httpsrv.py` & `copyparty-1.6.9/copyparty/httpsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/ico.py` & `copyparty-1.6.9/copyparty/ico.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/mdns.py` & `copyparty-1.6.9/copyparty/mdns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/mtag.py` & `copyparty-1.6.9/copyparty/mtag.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/multicast.py` & `copyparty-1.6.9/copyparty/multicast.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/res/COPYING.txt` & `copyparty-1.6.9/copyparty/res/COPYING.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/res/insecure.pem` & `copyparty-1.6.9/copyparty/res/insecure.pem`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/smbd.py` & `copyparty-1.6.9/copyparty/smbd.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/ssdp.py` & `copyparty-1.6.9/copyparty/ssdp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/star.py` & `copyparty-1.6.9/copyparty/star.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/dnslib/bimap.py` & `copyparty-1.6.9/copyparty/stolen/dnslib/bimap.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/dnslib/buffer.py` & `copyparty-1.6.9/copyparty/stolen/dnslib/buffer.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/dnslib/dns.py` & `copyparty-1.6.9/copyparty/stolen/dnslib/dns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/dnslib/label.py` & `copyparty-1.6.9/copyparty/stolen/dnslib/label.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/dnslib/lex.py` & `copyparty-1.6.9/copyparty/stolen/dnslib/lex.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/dnslib/ranges.py` & `copyparty-1.6.9/copyparty/stolen/dnslib/ranges.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/ifaddr/_posix.py` & `copyparty-1.6.9/copyparty/stolen/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/ifaddr/_shared.py` & `copyparty-1.6.9/copyparty/stolen/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/ifaddr/_win32.py` & `copyparty-1.6.9/copyparty/stolen/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/qrcodegen.py` & `copyparty-1.6.9/copyparty/stolen/qrcodegen.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/stolen/surrogateescape.py` & `copyparty-1.6.9/copyparty/stolen/surrogateescape.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/sutil.py` & `copyparty-1.6.9/copyparty/sutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/svchub.py` & `copyparty-1.6.9/copyparty/svchub.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/szip.py` & `copyparty-1.6.9/copyparty/szip.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/tcpsrv.py` & `copyparty-1.6.9/copyparty/tcpsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/th_cli.py` & `copyparty-1.6.9/copyparty/th_cli.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/th_srv.py` & `copyparty-1.6.9/copyparty/th_srv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/u2idx.py` & `copyparty-1.6.9/copyparty/u2idx.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,18 +113,18 @@
             self.log("opened {}".format(db_path))
 
         self.cur[ptop] = cur
         return cur
 
     def search(
         self, vols    , uq , lim 
-    )    :
+    )     :
         """search by query params"""
         if not HAVE_SQLITE3:
-            return [], []
+            return [], [], False
 
         q = ""
         v   = ""
         va   = []
         have_up = False  # query has up.* operands
         have_mt = False
         is_key = True
@@ -268,15 +268,15 @@
         self,
         vols    ,
         uq ,
         uv  ,
         have_up ,
         have_mt ,
         lim ,
-    )    :
+    )     :
         done_flag  = []
         self.active_id = "{:.6f}_{}".format(
             time.time(), threading.current_thread().ident
         )
         Daemon(self.terminator, "u2idx-terminator", (self.active_id, done_flag))
 
         if not uq or not uv:
@@ -309,17 +309,14 @@
 
             sret = []
             fk = flags.get("fk")
             dots = flags.get("dotsrch")
             c = cur.execute(uq, tuple(vuv))
             for hit in c:
                 w, ts, sz, rd, fn, ip, at = hit[:7]
-                lim -= 1
-                if lim < 0:
-                    break
 
                 if rd.startswith("//") or fn.startswith("//"):
                     rd, fn = s3dec(rd, fn)
 
                 rp = quotep("/".join([x for x in [vtop, rd, fn] if x]))
                 if not dots and "/." in ("/" + rp):
                     continue
@@ -339,14 +336,18 @@
                     suf = (
                         "?k="
                         + gen_filekey(
                             self.args.fk_salt, ap, sz, 0 if ANYWIN else inf.st_ino
                         )[:fk]
                     )
 
+                lim -= 1
+                if lim < 0:
+                    break
+
                 seen_rps.add(rp)
                 sret.append({"ts": int(ts), "sz": sz, "rp": rp + suf, "w": w[:16]})
 
             for hit in sret:
                 w = hit["w"]
                 del hit["w"]
                 tags = {}
@@ -361,15 +362,15 @@
             # print("[{}] {}".format(ptop, sret))
 
         done_flag.append(True)
         self.active_id = ""
 
         ret.sort(key=itemgetter("rp"))
 
-        return ret, list(taglist.keys())
+        return ret, list(taglist.keys()), lim < 0
 
     def terminator(self, identifier , done_flag )  :
         for _ in range(self.timeout):
             time.sleep(1)
             if done_flag:
                 return
```

### Comparing `copyparty-1.6.8/copyparty/up2k.py` & `copyparty-1.6.9/copyparty/up2k.py`

 * *Files 1% similar despite different names*

```diff
@@ -1244,20 +1244,23 @@
                     q = "delete from up where rd = ? and fn = ?"
                     c2.execute(q, (drd, dfn))
                     n_rm2 += 1
 
         if n_rm2:
             self.log("forgetting {} shadowed deleted files".format(n_rm2))
 
+        c2.connection.commit()
+
         # then covers
         n_rm3 = 0
+        qu = "select 1 from up where rd=? and +fn=? limit 1"
         q = "delete from cv where rd=? and dn=? and +fn=?"
         for crd, cdn, fn in cur.execute("select * from cv"):
-            ap = os.path.join(top, crd, cdn, fn)
-            if not bos.path.exists(ap):
+            urd = vjoin(crd, cdn)
+            if not c2.execute(qu, (urd, fn)).fetchone():
                 c2.execute(q, (crd, cdn, fn))
                 n_rm3 += 1
 
         if n_rm3:
             self.log("forgetting {} deleted covers".format(n_rm3))
 
         c2.connection.commit()
```

### Comparing `copyparty-1.6.8/copyparty/util.py` & `copyparty-1.6.9/copyparty/util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/a/partyfuse.py` & `copyparty-1.6.9/copyparty/web/a/partyfuse.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/a/up2k.py` & `copyparty-1.6.9/copyparty/web/a/up2k.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/a/webdav-cfg.bat` & `copyparty-1.6.9/copyparty/web/a/webdav-cfg.bat`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/baguettebox.js.gz` & `copyparty-1.6.9/copyparty/web/baguettebox.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/browser.html` & `copyparty-1.6.9/copyparty/web/browser.html`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 			have_del = {{ have_del|tojson }},
 			have_unpost = {{ have_unpost }},
 			have_zip = {{ have_zip|tojson }},
 			sb_md = "{{ sb_md }}",
 			sb_lg = "{{ sb_lg }}",
 			lifetime = {{ lifetime }},
 			turbolvl = {{ turbolvl }},
+			idxh = {{ idxh }},
 			frand = {{ frand|tojson }},
 			u2sort = "{{ u2sort }}",
 			have_emp = {{ have_emp|tojson }},
 			txt_ext = "{{ txt_ext }}",
 			logues = {{ logues|tojson if sb_lg else "[]" }},
 			readme = {{ readme|tojson }},
 			ls0 = {{ ls0|tojson }};
```

### Comparing `copyparty-1.6.8/copyparty/web/browser2.html` & `copyparty-1.6.9/copyparty/web/browser2.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/cf.html` & `copyparty-1.6.9/copyparty/web/cf.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/dbg-audio.js.gz` & `copyparty-1.6.9/copyparty/web/dbg-audio.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/easymde.css.gz` & `copyparty-1.6.9/copyparty/web/deps/easymde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/easymde.js.gz` & `copyparty-1.6.9/copyparty/web/deps/easymde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/marked.js.gz` & `copyparty-1.6.9/copyparty/web/deps/marked.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/mini-fa.css.gz` & `copyparty-1.6.9/copyparty/web/deps/mini-fa.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/mini-fa.woff` & `copyparty-1.6.9/copyparty/web/deps/mini-fa.woff`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/prism.css.gz` & `copyparty-1.6.9/copyparty/web/deps/prism.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/prism.js.gz` & `copyparty-1.6.9/copyparty/web/deps/prism.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/prismd.css.gz` & `copyparty-1.6.9/copyparty/web/deps/prismd.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/scp.woff2` & `copyparty-1.6.9/copyparty/web/deps/scp.woff2`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/sha512.ac.js.gz` & `copyparty-1.6.9/copyparty/web/deps/sha512.ac.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/deps/sha512.hw.js.gz` & `copyparty-1.6.9/copyparty/web/deps/sha512.hw.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/md.css.gz` & `copyparty-1.6.9/copyparty/web/md.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/md.html` & `copyparty-1.6.9/copyparty/web/md.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/md.js.gz` & `copyparty-1.6.9/copyparty/web/md.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/md2.css.gz` & `copyparty-1.6.9/copyparty/web/md2.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/md2.js.gz` & `copyparty-1.6.9/copyparty/web/md2.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/mde.css.gz` & `copyparty-1.6.9/copyparty/web/mde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/mde.html` & `copyparty-1.6.9/copyparty/web/mde.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/mde.js.gz` & `copyparty-1.6.9/copyparty/web/mde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/msg.html` & `copyparty-1.6.9/copyparty/web/msg.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/splash.css.gz` & `copyparty-1.6.9/copyparty/web/splash.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/splash.html` & `copyparty-1.6.9/copyparty/web/splash.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/splash.js.gz` & `copyparty-1.6.9/copyparty/web/splash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/svcs.html` & `copyparty-1.6.9/copyparty/web/svcs.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/svcs.js.gz` & `copyparty-1.6.9/copyparty/web/svcs.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/ui.css.gz` & `copyparty-1.6.9/copyparty/web/ui.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/up2k.js.gz` & `copyparty-1.6.9/copyparty/web/up2k.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty/web/w.hash.js.gz` & `copyparty-1.6.9/copyparty/web/w.hash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/copyparty.egg-info/PKG-INFO` & `copyparty-1.6.9/copyparty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.6.8
+Version: 1.6.9
 Summary: Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Home-page: https://github.com/9001/copyparty
 Author: ed
 Author-email: copyparty@ocv.me
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -48,15 +48,15 @@
 
 turn your phone or raspi into a portable file server with resumable uploads/downloads using *any* web browser
 
 * server only needs Python (`2.7` or `3.3+`), all dependencies optional
 * browse/upload with [IE4](#browser-support) / netscape4.0 on win3.11 (heh)
 * protocols: [http](#the-browser) // [ftp](#ftp-server) // [webdav](#webdav-server) // [smb/cifs](#smb-server)
 
-try the **[read-only demo server](https://a.ocv.me/pub/demo/)** 👀 running from a basement in finland
+**[Get started](#quickstart)!** or visit the **[read-only demo server](https://a.ocv.me/pub/demo/)** 👀 running from a basement in finland
 
 📷 **screenshots:** [browser](#the-browser) // [upload](#uploading) // [unpost](#unpost) // [thumbnails](#thumbnails) // [search](#searching) // [fsearch](#file-search) // [zip-DL](#zip-downloads) // [md-viewer](#markdown-viewer)
 
 
 ## get the app
 
 <a href="https://f-droid.org/packages/me.ocv.partyup/"><img src="https://ocv.me/fdroid.png" alt="Get it on F-Droid" height="50" /> '' <img src="https://img.shields.io/f-droid/v/me.ocv.partyup.svg" alt="f-droid version info" /></a> '' <a href="https://github.com/9001/party-up"><img src="https://img.shields.io/github/release/9001/party-up.svg?logo=github" alt="github version info" /></a>
@@ -144,14 +144,15 @@
 
 ## quickstart
 
 just run **[copyparty-sfx.py](https://github.com/9001/copyparty/releases/latest/download/copyparty-sfx.py)** -- that's it! 🎉
 
 * or install through pypi (python3 only): `python3 -m pip install --user -U copyparty`
 * or if you cannot install python, you can use [copyparty.exe](#copypartyexe) instead
+* or if you are on android, [install copyparty in termux](#install-on-android)
 * or if you prefer to [use docker](./scripts/docker/) 🐋 you can do that too
   * docker has all deps built-in, so skip this step:
 
 enable thumbnails (images/audio/video), media indexing, and audio transcoding by installing some recommended deps:
 
 * **Alpine:** `apk add py3-pillow ffmpeg`
 * **Debian:** `apt install python3-pil ffmpeg`
@@ -201,19 +202,23 @@
   * ☑ volumes (mountpoints)
   * ☑ [accounts](#accounts-and-volumes)
   * ☑ [ftp server](#ftp-server)
   * ☑ [webdav server](#webdav-server)
   * ☑ [smb/cifs server](#smb-server)
   * ☑ [qr-code](#qr-code) for quick access
   * ☑ [upnp / zeroconf / mdns / ssdp](#zeroconf)
+  * ☑ [event hooks](#event-hooks) / script runner
+  * ☑ [reverse-proxy support](https://github.com/9001/copyparty#reverse-proxy)
 * upload
   * ☑ basic: plain multipart, ie6 support
   * ☑ [up2k](#uploading): js, resumable, multithreaded
     * unaffected by cloudflare's max-upload-size (100 MiB)
   * ☑ stash: simple PUT filedropper
+  * ☑ filename randomizer
+  * ☑ write-only folders
   * ☑ [unpost](#unpost): undo/delete accidental uploads
   * ☑ [self-destruct](#self-destruct) (specified server-side or client-side)
   * ☑ symlink/discard existing files (content-matching)
 * download
   * ☑ single files in browser
   * ☑ [folders as zip / tar files](#zip-downloads)
   * ☑ [FUSE client](https://github.com/9001/copyparty/tree/hovudstraum/bin#partyfusepy) (read-only)
@@ -229,18 +234,23 @@
     * ☑ ...of audio (spectrograms) using FFmpeg
     * ☑ cache eviction (max-age; maybe max-size eventually)
   * ☑ SPA (browse while uploading)
 * server indexing
   * ☑ [locate files by contents](#file-search)
   * ☑ search by name/path/date/size
   * ☑ [search by ID3-tags etc.](#searching)
+* client support
+  * ☑ [sync folder to server](https://github.com/9001/copyparty/tree/hovudstraum/bin#up2kpy)
+  * ☑ [curl-friendly](https://user-images.githubusercontent.com/241032/215322619-ea5fd606-3654-40ad-94ee-2bc058647bb2.png)
 * markdown
   * ☑ [viewer](#markdown-viewer)
   * ☑ editor (sure why not)
 
+PS: something missing? post any crazy ideas you've got as a [feature request](https://github.com/9001/copyparty/issues/new?assignees=9001&labels=enhancement&template=feature_request.md) or [discussion](https://github.com/9001/copyparty/discussions/new?category=ideas) 🤙
+
 
 ## testimonials
 
 small collection of user feedback
 
 `good enough`, `surprisingly correct`, `certified good software`, `just works`, `why`, `wow this is better than nextcloud`
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_cz2chf20_/tmp321ousi3_TarContainer/0/118", line 1476, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_cz2chf20_/tmp321ousi3_TarContainer/0/118", line 1476, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copyparty Version: 1.6.8 Summary: Portable file
+Metadata-Version: 2.1 Name: copyparty Version: 1.6.9 Summary: Portable file
 server with accelerated resumable uploads, deduplication, WebDAV, FTP,
 zeroconf, media indexer, video thumbnails, audio transcoding, and write-only
 folders Home-page: https://github.com/9001/copyparty Author: ed Author-email:
 copyparty@ocv.me License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
@@ -24,97 +24,98 @@
 Provides-Extra: ftpd Provides-Extra: ftps License-File: LICENSE # ð¾ð
 copyparty * portable file sharing hub (py2/py3) [(on PyPI)](https://pypi.org/
 project/copyparty/) * MIT-Licensed, 2019-05-26, ed @ irc.rizon.net ## summary
 turn your phone or raspi into a portable file server with resumable uploads/
 downloads using *any* web browser * server only needs Python (`2.7` or `3.3+`),
 all dependencies optional * browse/upload with [IE4](#browser-support) /
 netscape4.0 on win3.11 (heh) * protocols: [http](#the-browser) // [ftp](#ftp-
-server) // [webdav](#webdav-server) // [smb/cifs](#smb-server) try the **[read-
-only demo server](https://a.ocv.me/pub/demo/)** ð running from a basement in
-finland ð· **screenshots:** [browser](#the-browser) // [upload](#uploading) /
-/ [unpost](#unpost) // [thumbnails](#thumbnails) // [search](#searching) //
-[fsearch](#file-search) // [zip-DL](#zip-downloads) // [md-viewer](#markdown-
-viewer) ## get the app [Get_it_on_F-Droid]_''_[f-droid_version_info] '' [github
-version_info] (the app is **NOT** the full copyparty server! just a basic
-upload client, nothing fancy yet) ## readme toc * top * [quickstart]
-(#quickstart) - just run **[copyparty-sfx.py](https://github.com/9001/
-copyparty/releases/latest/download/copyparty-sfx.py)** -- that's it! ð * [on
-servers](#on-servers) - you may also want these, especially on servers *
-[features](#features) * [testimonials](#testimonials) - small collection of
-user feedback * [motivations](#motivations) - project goals / philosophy *
-[notes](#notes) - general notes * [bugs](#bugs) * [general bugs](#general-bugs)
-* [not my bugs](#not-my-bugs) * [breaking changes](#breaking-changes) - upgrade
-notes * [FAQ](#FAQ) - "frequently" asked questions * [accounts and volumes]
-(#accounts-and-volumes) - per-folder, per-user permissions * [shadowing]
-(#shadowing) - hiding specific subfolders * [the browser](#the-browser) -
-accessing a copyparty server using a web-browser * [tabs](#tabs) - the main
-tabs in the ui * [hotkeys](#hotkeys) - the browser has the following hotkeys *
-[navpane](#navpane) - switching between breadcrumbs or navpane * [thumbnails]
-(#thumbnails) - press `g` or `ç°` to toggle grid-view instead of the file
-listing * [zip downloads](#zip-downloads) - download folders (or file
-selections) as `zip` or `tar` files * [uploading](#uploading) - drag files/
-folders into the web-browser to upload * [file-search](#file-search) - dropping
-files into the browser also lets you see if they exist on the server * [unpost]
-(#unpost) - undo/delete accidental uploads * [self-destruct](#self-destruct) -
-uploads can be given a lifetime * [file manager](#file-manager) - cut/paste,
-rename, and delete files/folders (if you have permission) * [batch rename]
-(#batch-rename) - select some files and press `F2` to bring up the rename UI *
-[markdown viewer](#markdown-viewer) - and there are *two* editors * [other
-tricks](#other-tricks) * [searching](#searching) - search by size, date, path/
-name, mp3-tags, ... * [server config](#server-config) - using arguments or
-config files, or a mix of both * [zeroconf](#zeroconf) - announce enabled
-services on the LAN ([pic](https://user-images.githubusercontent.com/241032/
-215344737-0eae8d98-9496-4256-9aa8-cd2f6971810d.png)) * [mdns](#mdns) - LAN
-domain-name and feature announcer * [ssdp](#ssdp) - windows-explorer announcer
-* [qr-code](#qr-code) - print a qr-code [(screenshot)](https://user-
-images.githubusercontent.com/241032/194728533-6f00849b-c6ac-43c6-9359-
-83e454d11e00.png) for quick access * [ftp server](#ftp-server) - an FTP server
-can be started using `--ftp 3921` * [webdav server](#webdav-server) - with
-read-write support * [connecting to webdav from windows](#connecting-to-webdav-
-from-windows) - using the GUI * [smb server](#smb-server) - unsafe, slow, not
-recommended for wan * [file indexing](#file-indexing) - enables dedup and music
-search ++ * [exclude-patterns](#exclude-patterns) - to save some time *
-[filesystem guards](#filesystem-guards) - avoid traversing into other
-filesystems * [periodic rescan](#periodic-rescan) - filesystem monitoring *
-[upload rules](#upload-rules) - set upload rules using volflags * [compress
-uploads](#compress-uploads) - files can be autocompressed on upload * [other
-flags](#other-flags) * [database location](#database-location) - in-volume
-(`.hist/up2k.db`, default) or somewhere else * [metadata from audio files]
-(#metadata-from-audio-files) - set `-e2t` to index tags on upload * [file
-parser plugins](#file-parser-plugins) - provide custom parsers to index
-additional tags * [event hooks](#event-hooks) - trigger a program on uploads,
-renames etc ([examples](./bin/hooks/)) * [upload events](#upload-events) - the
-older, more powerful approach ([examples](./bin/mtag/)) * [hiding from google]
-(#hiding-from-google) - tell search engines you dont wanna be indexed *
-[themes](#themes) * [complete examples](#complete-examples) * [reverse-proxy]
-(#reverse-proxy) - running copyparty next to other websites * [browser support]
-(#browser-support) - TLDR: yes * [client examples](#client-examples) - interact
-with copyparty using non-browser clients * [mount as drive](#mount-as-drive) -
-a remote copyparty server as a local filesystem * [performance](#performance) -
-defaults are usually fine - expect `8 GiB/s` download, `1 GiB/s` upload *
-[client-side](#client-side) - when uploading files * [security](#security) -
-some notes on hardening * [gotchas](#gotchas) - behavior that might be
-unexpected * [cors](#cors) - cross-site request config * [recovering from
-crashes](#recovering-from-crashes) * [client crashes](#client-crashes) *
-[frefox wsod](#frefox-wsod) - firefox 87 can crash during uploads * [HTTP API]
-(#HTTP-API) - see [devnotes](#./docs/devnotes.md#http-api) * [dependencies]
-(#dependencies) - mandatory deps * [optional dependencies](#optional-
-dependencies) - install these to enable bonus features * [optional gpl stuff]
-(#optional-gpl-stuff) * [sfx](#sfx) - the self-contained "binary" *
+server) // [webdav](#webdav-server) // [smb/cifs](#smb-server) **[Get started]
+(#quickstart)!** or visit the **[read-only demo server](https://a.ocv.me/pub/
+demo/)** ð running from a basement in finland ð· **screenshots:**
+[browser](#the-browser) // [upload](#uploading) // [unpost](#unpost) //
+[thumbnails](#thumbnails) // [search](#searching) // [fsearch](#file-search) /
+/ [zip-DL](#zip-downloads) // [md-viewer](#markdown-viewer) ## get the app [Get
+it_on_F-Droid]_''_[f-droid_version_info] '' [github_version_info] (the app is
+**NOT** the full copyparty server! just a basic upload client, nothing fancy
+yet) ## readme toc * top * [quickstart](#quickstart) - just run **[copyparty-
+sfx.py](https://github.com/9001/copyparty/releases/latest/download/copyparty-
+sfx.py)** -- that's it! ð * [on servers](#on-servers) - you may also want
+these, especially on servers * [features](#features) * [testimonials]
+(#testimonials) - small collection of user feedback * [motivations]
+(#motivations) - project goals / philosophy * [notes](#notes) - general notes *
+[bugs](#bugs) * [general bugs](#general-bugs) * [not my bugs](#not-my-bugs) *
+[breaking changes](#breaking-changes) - upgrade notes * [FAQ](#FAQ) -
+"frequently" asked questions * [accounts and volumes](#accounts-and-volumes) -
+per-folder, per-user permissions * [shadowing](#shadowing) - hiding specific
+subfolders * [the browser](#the-browser) - accessing a copyparty server using a
+web-browser * [tabs](#tabs) - the main tabs in the ui * [hotkeys](#hotkeys) -
+the browser has the following hotkeys * [navpane](#navpane) - switching between
+breadcrumbs or navpane * [thumbnails](#thumbnails) - press `g` or `ç°` to
+toggle grid-view instead of the file listing * [zip downloads](#zip-downloads)
+- download folders (or file selections) as `zip` or `tar` files * [uploading]
+(#uploading) - drag files/folders into the web-browser to upload * [file-
+search](#file-search) - dropping files into the browser also lets you see if
+they exist on the server * [unpost](#unpost) - undo/delete accidental uploads *
+[self-destruct](#self-destruct) - uploads can be given a lifetime * [file
+manager](#file-manager) - cut/paste, rename, and delete files/folders (if you
+have permission) * [batch rename](#batch-rename) - select some files and press
+`F2` to bring up the rename UI * [markdown viewer](#markdown-viewer) - and
+there are *two* editors * [other tricks](#other-tricks) * [searching]
+(#searching) - search by size, date, path/name, mp3-tags, ... * [server config]
+(#server-config) - using arguments or config files, or a mix of both *
+[zeroconf](#zeroconf) - announce enabled services on the LAN ([pic](https://
+user-images.githubusercontent.com/241032/215344737-0eae8d98-9496-4256-9aa8-
+cd2f6971810d.png)) * [mdns](#mdns) - LAN domain-name and feature announcer *
+[ssdp](#ssdp) - windows-explorer announcer * [qr-code](#qr-code) - print a qr-
+code [(screenshot)](https://user-images.githubusercontent.com/241032/194728533-
+6f00849b-c6ac-43c6-9359-83e454d11e00.png) for quick access * [ftp server](#ftp-
+server) - an FTP server can be started using `--ftp 3921` * [webdav server]
+(#webdav-server) - with read-write support * [connecting to webdav from
+windows](#connecting-to-webdav-from-windows) - using the GUI * [smb server]
+(#smb-server) - unsafe, slow, not recommended for wan * [file indexing](#file-
+indexing) - enables dedup and music search ++ * [exclude-patterns](#exclude-
+patterns) - to save some time * [filesystem guards](#filesystem-guards) - avoid
+traversing into other filesystems * [periodic rescan](#periodic-rescan) -
+filesystem monitoring * [upload rules](#upload-rules) - set upload rules using
+volflags * [compress uploads](#compress-uploads) - files can be autocompressed
+on upload * [other flags](#other-flags) * [database location](#database-
+location) - in-volume (`.hist/up2k.db`, default) or somewhere else * [metadata
+from audio files](#metadata-from-audio-files) - set `-e2t` to index tags on
+upload * [file parser plugins](#file-parser-plugins) - provide custom parsers
+to index additional tags * [event hooks](#event-hooks) - trigger a program on
+uploads, renames etc ([examples](./bin/hooks/)) * [upload events](#upload-
+events) - the older, more powerful approach ([examples](./bin/mtag/)) * [hiding
+from google](#hiding-from-google) - tell search engines you dont wanna be
+indexed * [themes](#themes) * [complete examples](#complete-examples) *
+[reverse-proxy](#reverse-proxy) - running copyparty next to other websites *
+[browser support](#browser-support) - TLDR: yes * [client examples](#client-
+examples) - interact with copyparty using non-browser clients * [mount as
+drive](#mount-as-drive) - a remote copyparty server as a local filesystem *
+[performance](#performance) - defaults are usually fine - expect `8 GiB/s`
+download, `1 GiB/s` upload * [client-side](#client-side) - when uploading files
+* [security](#security) - some notes on hardening * [gotchas](#gotchas) -
+behavior that might be unexpected * [cors](#cors) - cross-site request config *
+[recovering from crashes](#recovering-from-crashes) * [client crashes](#client-
+crashes) * [frefox wsod](#frefox-wsod) - firefox 87 can crash during uploads *
+[HTTP API](#HTTP-API) - see [devnotes](#./docs/devnotes.md#http-api) *
+[dependencies](#dependencies) - mandatory deps * [optional dependencies]
+(#optional-dependencies) - install these to enable bonus features * [optional
+gpl stuff](#optional-gpl-stuff) * [sfx](#sfx) - the self-contained "binary" *
 [copyparty.exe](#copypartyexe) - download [copyparty.exe](https://github.com/
 9001/copyparty/releases/latest/download/copyparty.exe) (win8+) or
 [copyparty32.exe](https://github.com/9001/copyparty/releases/latest/download/
 copyparty32.exe) (win7+) * [install on android](#install-on-android) *
 [reporting bugs](#reporting-bugs) - ideas for context to include in bug reports
 * [devnotes](#devnotes) - for build instructions etc, see [./docs/devnotes.md]
 (./docs/devnotes.md) ## quickstart just run **[copyparty-sfx.py](https://
 github.com/9001/copyparty/releases/latest/download/copyparty-sfx.py)** -
 - that's it! ð * or install through pypi (python3 only): `python3 -m pip
 install --user -U copyparty` * or if you cannot install python, you can use
-[copyparty.exe](#copypartyexe) instead * or if you prefer to [use docker](./
+[copyparty.exe](#copypartyexe) instead * or if you are on android, [install
+copyparty in termux](#install-on-android) * or if you prefer to [use docker](./
 scripts/docker/) ð you can do that too * docker has all deps built-in, so
 skip this step: enable thumbnails (images/audio/video), media indexing, and
 audio transcoding by installing some recommended deps: * **Alpine:** `apk add
 py3-pillow ffmpeg` * **Debian:** `apt install python3-pil ffmpeg` * **Fedora:**
 `dnf install python3-pillow ffmpeg` * **FreeBSD:** `pkg install py39-sqlite3
 py39-pillow ffmpeg` * **MacOS:** `port install py-Pillow ffmpeg` * **MacOS**
 (alternative): `brew install pillow ffmpeg` * **Windows:** `python -m pip
@@ -144,54 +145,64 @@
 --zone=libvirt firewall-cmd --permanent --add-port={1900,5353}/udp # --
 zone=libvirt firewall-cmd --reload ``` (1900:ssdp, 3921:ftp, 3923:http/https,
 3945:smb, 3990:ftps, 5353:mdns, 12000:passive-ftp) ## features * backend stuff
 * â IPv6 * â [multiprocessing](#performance) (actual multithreading) * â
 volumes (mountpoints) * â [accounts](#accounts-and-volumes) * â [ftp
 server](#ftp-server) * â [webdav server](#webdav-server) * â [smb/cifs
 server](#smb-server) * â [qr-code](#qr-code) for quick access * â [upnp /
-zeroconf / mdns / ssdp](#zeroconf) * upload * â basic: plain multipart, ie6
-support * â [up2k](#uploading): js, resumable, multithreaded * unaffected by
-cloudflare's max-upload-size (100 MiB) * â stash: simple PUT filedropper *
-â [unpost](#unpost): undo/delete accidental uploads * â [self-destruct]
-(#self-destruct) (specified server-side or client-side) * â symlink/discard
-existing files (content-matching) * download * â single files in browser *
-â [folders as zip / tar files](#zip-downloads) * â [FUSE client](https://
-github.com/9001/copyparty/tree/hovudstraum/bin#partyfusepy) (read-only) *
-browser * â [navpane](#navpane) (directory tree sidebar) * â file manager
-(cut/paste, delete, [batch-rename](#batch-rename)) * â audio player (with [OS
-media controls](https://user-images.githubusercontent.com/241032/215347492-
-b4250797-6c90-4e09-9a4c-721edf2fb15c.png) and opus transcoding) * â image
-gallery with webm player * â textfile browser with syntax hilighting * â
-[thumbnails](#thumbnails) * â ...of images using Pillow, pyvips, or FFmpeg *
-â ...of videos using FFmpeg * â ...of audio (spectrograms) using FFmpeg *
-â cache eviction (max-age; maybe max-size eventually) * â SPA (browse while
-uploading) * server indexing * â [locate files by contents](#file-search) *
-â search by name/path/date/size * â [search by ID3-tags etc.](#searching) *
-markdown * â [viewer](#markdown-viewer) * â editor (sure why not) ##
-testimonials small collection of user feedback `good enough`, `surprisingly
-correct`, `certified good software`, `just works`, `why`, `wow this is better
-than nextcloud` # motivations project goals / philosophy * inverse linux
-philosophy -- do all the things, and do an *okay* job * quick drop-in service
-to get a lot of features in a pinch * some of [the alternatives](./docs/
-versus.md) might be a better fit for you * run anywhere, support everything *
-as many web-browsers and python versions as possible * every browser should at
-least be able to browse, download, upload files * be a good emergency solution
-for transferring stuff between ancient boxes * minimal dependencies * but
-optional dependencies adding bonus-features are ok * everything being plaintext
-makes it possible to proofread for malicious code * no preparations / setup
-necessary, just run the sfx (which is also plaintext) * adaptable, malleable,
-hackable * no build steps; modify the js/python without needing node.js or
-anything like that ## notes general notes: * paper-printing is affected by
-dark/light-mode! use lightmode for color, darkmode for grayscale * because no
-browsers currently implement the media-query to do this properly orz browser-
-specific: * iPhone/iPad: use Firefox to download files * Android-Chrome:
-increase "parallel uploads" for higher speed (android bug) * Android-Firefox:
-takes a while to select files (their fix for âï¸) * Desktop-Firefox: ~~may
-use gigabytes of RAM if your files are massive~~ *seems to be OK now* *
-Desktop-Firefox: [may stop you from unplugging USB flashdrives](https://
+zeroconf / mdns / ssdp](#zeroconf) * â [event hooks](#event-hooks) / script
+runner * â [reverse-proxy support](https://github.com/9001/copyparty#reverse-
+proxy) * upload * â basic: plain multipart, ie6 support * â [up2k]
+(#uploading): js, resumable, multithreaded * unaffected by cloudflare's max-
+upload-size (100 MiB) * â stash: simple PUT filedropper * â filename
+randomizer * â write-only folders * â [unpost](#unpost): undo/delete
+accidental uploads * â [self-destruct](#self-destruct) (specified server-side
+or client-side) * â symlink/discard existing files (content-matching) *
+download * â single files in browser * â [folders as zip / tar files](#zip-
+downloads) * â [FUSE client](https://github.com/9001/copyparty/tree/
+hovudstraum/bin#partyfusepy) (read-only) * browser * â [navpane](#navpane)
+(directory tree sidebar) * â file manager (cut/paste, delete, [batch-rename]
+(#batch-rename)) * â audio player (with [OS media controls](https://user-
+images.githubusercontent.com/241032/215347492-b4250797-6c90-4e09-9a4c-
+721edf2fb15c.png) and opus transcoding) * â image gallery with webm player *
+â textfile browser with syntax hilighting * â [thumbnails](#thumbnails) *
+â ...of images using Pillow, pyvips, or FFmpeg * â ...of videos using
+FFmpeg * â ...of audio (spectrograms) using FFmpeg * â cache eviction (max-
+age; maybe max-size eventually) * â SPA (browse while uploading) * server
+indexing * â [locate files by contents](#file-search) * â search by name/
+path/date/size * â [search by ID3-tags etc.](#searching) * client support *
+â [sync folder to server](https://github.com/9001/copyparty/tree/hovudstraum/
+bin#up2kpy) * â [curl-friendly](https://user-images.githubusercontent.com/
+241032/215322619-ea5fd606-3654-40ad-94ee-2bc058647bb2.png) * markdown * â
+[viewer](#markdown-viewer) * â editor (sure why not) PS: something missing?
+post any crazy ideas you've got as a [feature request](https://github.com/9001/
+copyparty/issues/
+new?assignees=9001&labels=enhancement&template=feature_request.md) or
+[discussion](https://github.com/9001/copyparty/discussions/new?category=ideas)
+ð¤ ## testimonials small collection of user feedback `good enough`,
+`surprisingly correct`, `certified good software`, `just works`, `why`, `wow
+this is better than nextcloud` # motivations project goals / philosophy *
+inverse linux philosophy -- do all the things, and do an *okay* job * quick
+drop-in service to get a lot of features in a pinch * some of [the
+alternatives](./docs/versus.md) might be a better fit for you * run anywhere,
+support everything * as many web-browsers and python versions as possible *
+every browser should at least be able to browse, download, upload files * be a
+good emergency solution for transferring stuff between ancient boxes * minimal
+dependencies * but optional dependencies adding bonus-features are ok *
+everything being plaintext makes it possible to proofread for malicious code *
+no preparations / setup necessary, just run the sfx (which is also plaintext) *
+adaptable, malleable, hackable * no build steps; modify the js/python without
+needing node.js or anything like that ## notes general notes: * paper-printing
+is affected by dark/light-mode! use lightmode for color, darkmode for grayscale
+* because no browsers currently implement the media-query to do this properly
+orz browser-specific: * iPhone/iPad: use Firefox to download files * Android-
+Chrome: increase "parallel uploads" for higher speed (android bug) * Android-
+Firefox: takes a while to select files (their fix for âï¸) * Desktop-
+Firefox: ~~may use gigabytes of RAM if your files are massive~~ *seems to be OK
+now* * Desktop-Firefox: [may stop you from unplugging USB flashdrives](https://
 bugzilla.mozilla.org/show_bug.cgi?id=1792598) until you visit `about:memory`
 and click `Minimize memory usage` server-os-specific: * RHEL8 / Rocky8: you can
 run copyparty using `/usr/libexec/platform-python` server notes: * pypy is
 supported but regular cpython is faster if you enable the database # bugs *
 Windows: python 2.7 cannot index non-ascii filenames with `-e2d` * Windows:
 python 2.7 cannot handle filenames with mojibake * `--th-ff-jpg` may fix video
 thumbnails on some FFmpeg versions (macos, some linux) * `--th-ff-swr` may fix
```

### Comparing `copyparty-1.6.8/copyparty.egg-info/SOURCES.txt` & `copyparty-1.6.9/copyparty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.6.8/setup.py` & `copyparty-1.6.9/setup.py`

 * *Files identical despite different names*

