# Comparing `tmp/pypcapkit-0.9.9rc3.tar.gz` & `tmp/pypcapkit-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypcapkit-0.9.9rc3.tar", last modified: Tue Aug  7 05:36:48 2018, max compression
+gzip compressed data, was "pypcapkit-1.0.0b1.tar", last modified: Fri Apr 21 04:07:17 2023, max compression
```

## Comparing `pypcapkit-0.9.9rc3.tar` & `pypcapkit-1.0.0b1.tar`

### file list

```diff
@@ -1,173 +1,511 @@
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/
--rw-r--r--   0 jarryshaw   (502) staff       (20)      145 2018-06-23 07:26:52.000000 pypcapkit-0.9.9rc3/MANIFEST.in
--rw-r--r--   0 jarryshaw   (502) staff       (20)    23473 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/PKG-INFO
--rw-r--r--   0 jarryshaw   (502) staff       (20)    19248 2018-07-29 10:27:11.000000 pypcapkit-0.9.9rc3/README.md
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/doc/
--rw-r--r--   0 jarryshaw   (502) staff       (20)   907777 2018-06-02 15:27:11.000000 pypcapkit-0.9.9rc3/doc/jspcap.png
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/
--rw-r--r--   0 jarryshaw   (502) staff       (20)    16833 2018-07-25 03:13:22.000000 pypcapkit-0.9.9rc3/pcapkit/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)     3558 2018-08-04 03:17:22.000000 pypcapkit-0.9.9rc3/pcapkit/__all__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     3848 2018-08-04 03:17:32.000000 pypcapkit-0.9.9rc3/pcapkit/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     5198 2018-07-07 06:39:46.000000 pypcapkit-0.9.9rc3/pcapkit/__main__.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/corekit/
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2035 2018-07-25 13:07:39.000000 pypcapkit-0.9.9rc3/pcapkit/corekit/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      433 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/corekit/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2731 2018-08-03 04:27:10.000000 pypcapkit-0.9.9rc3/pcapkit/corekit/infoclass.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     4209 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/corekit/protochain.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)      358 2018-07-29 06:18:21.000000 pypcapkit-0.9.9rc3/pcapkit/corekit/version.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/dumpkit/
--rw-r--r--   0 jarryshaw   (502) staff       (20)     1225 2018-07-25 13:22:27.000000 pypcapkit-0.9.9rc3/pcapkit/dumpkit/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)     1039 2018-07-13 06:27:23.000000 pypcapkit-0.9.9rc3/pcapkit/dumpkit/__init__.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/foundation/
--rw-r--r--   0 jarryshaw   (502) staff       (20)    10838 2018-07-26 04:57:09.000000 pypcapkit-0.9.9rc3/pcapkit/foundation/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      415 2018-08-03 14:03:55.000000 pypcapkit-0.9.9rc3/pcapkit/foundation/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     1876 2018-08-04 03:18:18.000000 pypcapkit-0.9.9rc3/pcapkit/foundation/analysis.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)    43026 2018-08-03 13:41:32.000000 pypcapkit-0.9.9rc3/pcapkit/foundation/extraction.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     7819 2018-07-25 14:25:04.000000 pypcapkit-0.9.9rc3/pcapkit/foundation/traceflow.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/interface/
--rw-r--r--   0 jarryshaw   (502) staff       (20)     8097 2018-07-29 06:17:40.000000 pypcapkit-0.9.9rc3/pcapkit/interface/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)     7220 2018-08-03 14:03:43.000000 pypcapkit-0.9.9rc3/pcapkit/interface/__init__.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/
--rw-r--r--   0 jarryshaw   (502) staff       (20)       42 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      559 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/__init__.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/application/
--rw-r--r--   0 jarryshaw   (502) staff       (20)       55 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/application/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      160 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/application/__init__.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/internet/
--rw-r--r--   0 jarryshaw   (502) staff       (20)       52 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/internet/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      151 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/internet/__init__.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/link/
--rw-r--r--   0 jarryshaw   (502) staff       (20)       48 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/link/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      139 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/link/__init__.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/pcap/
--rw-r--r--   0 jarryshaw   (502) staff       (20)       45 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/pcap/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      316 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/pcap/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2484 2018-07-13 06:28:39.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/pcap/frame.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2047 2018-07-13 06:29:09.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/pcap/header.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     4653 2018-07-13 06:30:17.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/protocol.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/transport/
--rw-r--r--   0 jarryshaw   (502) staff       (20)       53 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/transport/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      154 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/ipsuite/transport/__init__.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/
--rw-r--r--   0 jarryshaw   (502) staff       (20)    14595 2018-07-29 10:37:20.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)     1621 2018-08-04 03:19:07.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/__init__.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/application.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/bgp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/dhcp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/dns.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/ftp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/http.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2945 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/httpv2.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/imap.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/ldap.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/mqtt.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/nntp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/ntp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/onc:rpc.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/pop.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/rip.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/rtp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/sip.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/smtp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/snmp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/ssh.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/ssl.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/telnet.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/tls.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/NotImplemented/xmpp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)       62 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      685 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2857 2018-08-04 06:32:30.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/application.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2509 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/http.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     6683 2018-08-07 05:34:59.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/httpv1.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)    33340 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/application/httpv2.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/NotImplemented/
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/NotImplemented/ecn.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     5683 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/NotImplemented/esp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/NotImplemented/icmp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/NotImplemented/icmpv6.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/NotImplemented/igmp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/NotImplemented/shim6.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)       59 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)     1389 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     6719 2018-08-03 14:11:06.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ah.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     9239 2018-08-03 14:11:20.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/hip.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     5200 2018-08-03 14:11:10.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/hopopt.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     6781 2018-08-04 03:16:13.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/internet.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2439 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ip.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2327 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ipsec.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)    34733 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ipv4.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)    12642 2018-08-03 14:07:47.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ipv6.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     5076 2018-08-03 14:10:36.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ipv6_frag.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     5414 2018-08-03 14:10:44.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ipv6_opts.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     6127 2018-08-03 14:10:49.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ipv6_route.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     7113 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ipx.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     7343 2018-08-03 14:10:55.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/internet/mh.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/NotImplemented/
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/NotImplemented/dsl.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)       24 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/NotImplemented/eapol.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/NotImplemented/fddi.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/NotImplemented/isdn.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/NotImplemented/ndp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/NotImplemented/ppp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)    14319 2018-07-29 10:38:28.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)     1010 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)    10902 2018-07-29 10:42:16.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/arp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     4527 2018-07-29 10:42:19.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/ethernet.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     7132 2018-07-29 10:42:23.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/l2tp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     4404 2018-08-04 03:16:04.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/link.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     8575 2018-07-29 10:42:39.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/ospf.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2968 2018-07-29 10:42:51.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/rarp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     4740 2018-07-29 10:42:59.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/link/vlan.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/pcap/
--rw-r--r--   0 jarryshaw   (502) staff       (20)     4428 2018-07-29 10:37:47.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/pcap/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      291 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/pcap/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)    10088 2018-08-04 03:15:44.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/pcap/frame.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     5865 2018-08-03 04:12:17.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/pcap/header.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)    15447 2018-08-05 14:24:25.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/protocol.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     3555 2018-08-04 03:13:26.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/raw.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/transport/
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/transport/NotImplemented/
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/transport/NotImplemented/dccp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/transport/NotImplemented/rsvp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)        0 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/transport/NotImplemented/sctp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)       60 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/transport/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      640 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/transport/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)    57210 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/transport/tcp.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     4153 2018-08-03 14:02:42.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/transport/transport.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     4542 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/protocols/transport/udp.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/reassembly/
--rw-r--r--   0 jarryshaw   (502) staff       (20)    17525 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/reassembly/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      686 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/reassembly/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     6897 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/reassembly/ip.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     6305 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/reassembly/ipv4.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     6465 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/reassembly/ipv6.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     5073 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/reassembly/reassembly.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)    16194 2018-08-03 14:01:30.000000 pypcapkit-0.9.9rc3/pcapkit/reassembly/tcp.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/toolkit/
--rw-r--r--   0 jarryshaw   (502) staff       (20)    14679 2018-07-29 06:13:09.000000 pypcapkit-0.9.9rc3/pcapkit/toolkit/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)     1889 2018-07-25 22:09:05.000000 pypcapkit-0.9.9rc3/pcapkit/toolkit/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     5289 2018-07-26 04:39:55.000000 pypcapkit-0.9.9rc3/pcapkit/toolkit/default.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     7140 2018-07-29 02:27:38.000000 pypcapkit-0.9.9rc3/pcapkit/toolkit/dpkt.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     1853 2018-07-25 22:13:06.000000 pypcapkit-0.9.9rc3/pcapkit/toolkit/pyshark.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     7055 2018-07-25 22:13:20.000000 pypcapkit-0.9.9rc3/pcapkit/toolkit/scapy.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pcapkit/utilities/
--rw-r--r--   0 jarryshaw   (502) staff       (20)    11351 2018-07-29 09:21:54.000000 pypcapkit-0.9.9rc3/pcapkit/utilities/README.md
--rw-r--r--   0 jarryshaw   (502) staff       (20)      485 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/utilities/__init__.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2365 2018-08-04 03:16:32.000000 pypcapkit-0.9.9rc3/pcapkit/utilities/decorators.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     7771 2018-08-04 03:07:09.000000 pypcapkit-0.9.9rc3/pcapkit/utilities/exceptions.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     7777 2018-07-04 08:45:21.000000 pypcapkit-0.9.9rc3/pcapkit/utilities/validations.py
--rw-r--r--   0 jarryshaw   (502) staff       (20)     2474 2018-07-25 21:56:26.000000 pypcapkit-0.9.9rc3/pcapkit/utilities/warnings.py
-drwxr-xr-x   0 jarryshaw   (502) staff       (20)        0 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pypcapkit.egg-info/
--rw-r--r--   0 jarryshaw   (502) staff       (20)    23473 2018-08-07 05:36:46.000000 pypcapkit-0.9.9rc3/pypcapkit.egg-info/PKG-INFO
--rw-r--r--   0 jarryshaw   (502) staff       (20)     5292 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/pypcapkit.egg-info/SOURCES.txt
--rw-r--r--   0 jarryshaw   (502) staff       (20)        1 2018-08-07 05:36:46.000000 pypcapkit-0.9.9rc3/pypcapkit.egg-info/dependency_links.txt
--rw-r--r--   0 jarryshaw   (502) staff       (20)       51 2018-08-07 05:36:46.000000 pypcapkit-0.9.9rc3/pypcapkit.egg-info/entry_points.txt
--rw-r--r--   0 jarryshaw   (502) staff       (20)      103 2018-08-07 05:36:46.000000 pypcapkit-0.9.9rc3/pypcapkit.egg-info/requires.txt
--rw-r--r--   0 jarryshaw   (502) staff       (20)        8 2018-08-07 05:36:46.000000 pypcapkit-0.9.9rc3/pypcapkit.egg-info/top_level.txt
--rw-r--r--   0 jarryshaw   (502) staff       (20)      131 2018-08-07 05:36:48.000000 pypcapkit-0.9.9rc3/setup.cfg
--rw-r--r--   0 jarryshaw   (502) staff       (20)     3718 2018-08-07 05:35:37.000000 pypcapkit-0.9.9rc3/setup.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.520397 pypcapkit-1.0.0b1/
+-rwxr-xr-x   0 jarryshaw   (501) staff       (20)     3302 2019-07-10 00:43:13.000000 pypcapkit-1.0.0b1/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 jarryshaw   (501) staff       (20)     2262 2022-06-08 19:16:15.000000 pypcapkit-1.0.0b1/CONTRIBUTING.md
+-rwxr-xr-x   0 jarryshaw   (501) staff       (20)     1516 2022-06-01 05:01:21.000000 pypcapkit-1.0.0b1/LICENSE
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      232 2023-04-21 03:13:28.000000 pypcapkit-1.0.0b1/MANIFEST.in
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6856 2023-04-21 04:07:17.520236 pypcapkit-1.0.0b1/PKG-INFO
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4803 2023-04-20 12:02:38.000000 pypcapkit-1.0.0b1/README.rst
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.307837 pypcapkit-1.0.0b1/pcapkit/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3733 2023-04-20 12:05:52.000000 pypcapkit-1.0.0b1/pcapkit/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5581 2023-04-20 12:05:43.000000 pypcapkit-1.0.0b1/pcapkit/__main__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6171 2023-04-18 01:30:40.000000 pypcapkit-1.0.0b1/pcapkit/all.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.308205 pypcapkit-1.0.0b1/pcapkit/const/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3001 2023-04-17 08:00:48.000000 pypcapkit-1.0.0b1/pcapkit/const/__init__.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.309435 pypcapkit-1.0.0b1/pcapkit/const/arp/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      963 2023-04-18 01:32:09.000000 pypcapkit-1.0.0b1/pcapkit/const/arp/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4382 2023-04-21 04:00:42.000000 pypcapkit-1.0.0b1/pcapkit/const/arp/hardware.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3140 2023-04-21 04:00:42.000000 pypcapkit-1.0.0b1/pcapkit/const/arp/operation.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.310453 pypcapkit-1.0.0b1/pcapkit/const/ftp/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      936 2023-04-18 01:32:09.000000 pypcapkit-1.0.0b1/pcapkit/const/ftp/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    10799 2023-04-21 04:00:44.000000 pypcapkit-1.0.0b1/pcapkit/const/ftp/command.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    10618 2023-04-21 04:02:00.000000 pypcapkit-1.0.0b1/pcapkit/const/ftp/return_code.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.314758 pypcapkit-1.0.0b1/pcapkit/const/hip/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5583 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2097 2023-04-21 04:02:00.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/certificate.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1711 2023-04-21 04:02:01.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/cipher.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1571 2023-04-21 04:02:01.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/di.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1679 2023-04-21 04:02:02.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/ecdsa_curve.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1679 2023-04-21 04:02:02.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/ecdsa_low_curve.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1783 2023-04-21 04:02:10.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/eddsa_curve.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2743 2023-04-21 04:02:03.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/esp_transform_suite.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2263 2023-04-21 04:02:03.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/group.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2142 2023-04-21 04:02:04.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/hi_algorithm.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1809 2023-04-21 04:02:05.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/hit_suite.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1799 2023-04-21 04:02:05.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/nat_traversal.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6079 2023-04-21 04:02:06.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/notify_message.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2502 2023-04-21 04:02:06.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/packet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    12342 2023-04-21 04:02:07.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/parameter.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2016 2023-04-21 04:02:07.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/registration.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2712 2023-04-21 04:02:08.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/registration_failure.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1979 2023-04-21 04:02:09.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/suite.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1546 2023-04-21 04:02:09.000000 pypcapkit-1.0.0b1/pcapkit/const/hip/transport.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.315886 pypcapkit-1.0.0b1/pcapkit/const/http/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1763 2023-04-18 01:48:44.000000 pypcapkit-1.0.0b1/pcapkit/const/http/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3139 2023-04-21 04:02:10.000000 pypcapkit-1.0.0b1/pcapkit/const/http/error_code.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2594 2023-04-21 04:02:11.000000 pypcapkit-1.0.0b1/pcapkit/const/http/frame.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4952 2023-04-21 04:02:11.000000 pypcapkit-1.0.0b1/pcapkit/const/http/method.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3210 2023-04-21 04:02:12.000000 pypcapkit-1.0.0b1/pcapkit/const/http/setting.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     9074 2023-04-21 04:02:12.000000 pypcapkit-1.0.0b1/pcapkit/const/http/status_code.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.318791 pypcapkit-1.0.0b1/pcapkit/const/ipv4/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3089 2023-04-18 01:54:32.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1894 2023-04-21 04:02:12.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/classification_level.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1539 2023-04-21 04:02:12.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/option_class.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3614 2023-04-21 04:02:13.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/option_number.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1750 2023-04-21 04:02:13.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/protection_authority.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1459 2023-04-21 04:02:13.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/qs_function.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     8357 2023-04-21 04:02:14.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/router_alert.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1430 2023-04-21 04:02:14.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/tos_del.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1456 2023-04-21 04:02:14.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/tos_ecn.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1647 2023-04-21 04:02:14.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/tos_pre.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1515 2023-04-21 04:02:14.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/tos_rel.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1501 2023-04-21 04:02:14.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/tos_thr.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1430 2023-04-21 04:02:14.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv4/ts_flag.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.324161 pypcapkit-1.0.0b1/pcapkit/const/ipv6/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2819 2023-04-18 02:07:05.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv6/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1790 2023-04-21 04:02:14.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv6/extension_header.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3903 2023-04-21 04:02:15.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv6/option.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1516 2023-04-21 04:02:17.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv6/option_action.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1459 2023-04-21 04:02:15.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv6/qs_function.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     8843 2023-04-21 04:02:15.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv6/router_alert.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2395 2023-04-21 04:02:16.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv6/routing.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1541 2023-04-21 04:02:16.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv6/seed_id.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1701 2023-04-21 04:02:16.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv6/smf_dpd_mode.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1649 2023-04-21 04:02:17.000000 pypcapkit-1.0.0b1/pcapkit/const/ipv6/tagger_id.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.324990 pypcapkit-1.0.0b1/pcapkit/const/ipx/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      903 2023-04-18 02:14:05.000000 pypcapkit-1.0.0b1/pcapkit/const/ipx/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1779 2023-04-21 04:03:33.000000 pypcapkit-1.0.0b1/pcapkit/const/ipx/packet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3289 2023-04-21 04:04:49.000000 pypcapkit-1.0.0b1/pcapkit/const/ipx/socket.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.325893 pypcapkit-1.0.0b1/pcapkit/const/l2tp/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      548 2023-04-18 02:15:27.000000 pypcapkit-1.0.0b1/pcapkit/const/l2tp/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1342 2023-04-21 04:04:49.000000 pypcapkit-1.0.0b1/pcapkit/const/l2tp/type.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.335936 pypcapkit-1.0.0b1/pcapkit/const/mh/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    13257 2023-04-18 02:16:35.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2599 2023-04-21 04:04:58.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/access_type.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2369 2023-04-21 04:04:55.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/ack_status_code.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2255 2023-04-21 04:05:10.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/ani_suboption.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1845 2023-04-21 04:04:57.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/auth_subtype.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1565 2023-04-21 04:04:59.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/binding_ack_flag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1867 2023-04-21 04:05:00.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/binding_revocation.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1774 2023-04-21 04:04:59.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/binding_update_flag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1611 2023-04-21 04:05:03.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/dhcp_support_mode.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2100 2023-04-21 04:04:54.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/dns_status_code.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1994 2023-04-21 04:05:09.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/dsmip6_tls_packet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2565 2023-04-21 04:05:00.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/dsmipv6_home_address.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1776 2023-04-21 04:04:56.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/enumerating_algorithm.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2066 2023-04-21 04:05:13.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/fb_ack_status.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2120 2023-04-21 04:05:13.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/fb_action.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2260 2023-04-21 04:05:12.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/fb_indication_trigger.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1741 2023-04-21 04:05:12.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/fb_type.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2764 2023-04-21 04:05:05.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/flow_id_status.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2184 2023-04-21 04:05:06.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/flow_id_suboption.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2357 2023-04-21 04:04:57.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/handoff_type.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1452 2023-04-21 04:05:04.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/handover_ack_flag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3057 2023-04-21 04:05:05.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/handover_ack_status.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1561 2023-04-21 04:05:03.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/handover_initiate_flag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2116 2023-04-18 02:42:10.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/handover_initiate_status.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2335 2023-04-21 04:05:02.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/home_address_reply.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2053 2023-04-21 04:05:15.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/lma_mag_suboption.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1795 2023-04-21 04:05:09.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/mn_group_id.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2152 2023-04-21 04:04:55.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/mn_id_subtype.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1938 2023-04-21 04:05:10.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/operator_id.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     7043 2023-04-21 04:04:51.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/option.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3404 2023-04-21 04:04:50.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/packet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2654 2023-04-21 04:05:14.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/qos_attribute.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2208 2023-04-21 04:05:02.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/revocation_status_code.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2893 2023-04-21 04:05:01.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/revocation_trigger.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2033 2023-04-21 04:04:56.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/status_code.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2030 2023-04-21 04:05:07.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/traffic_selector.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2448 2023-04-21 04:05:11.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/upa_status.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2515 2023-04-21 04:05:11.000000 pypcapkit-1.0.0b1/pcapkit/const/mh/upn_reason.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.336977 pypcapkit-1.0.0b1/pcapkit/const/ospf/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1023 2023-04-18 02:27:17.000000 pypcapkit-1.0.0b1/pcapkit/const/ospf/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2157 2023-04-21 02:50:09.000000 pypcapkit-1.0.0b1/pcapkit/const/ospf/authentication.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1964 2023-04-21 04:05:46.000000 pypcapkit-1.0.0b1/pcapkit/const/ospf/packet.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.337690 pypcapkit-1.0.0b1/pcapkit/const/pcapng/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      688 2023-04-18 02:54:10.000000 pypcapkit-1.0.0b1/pcapkit/const/pcapng/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5525 2023-04-21 04:07:04.000000 pypcapkit-1.0.0b1/pcapkit/const/pcapng/block_type.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.338954 pypcapkit-1.0.0b1/pcapkit/const/reg/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1134 2023-04-18 02:51:06.000000 pypcapkit-1.0.0b1/pcapkit/const/reg/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    27235 2023-04-21 04:00:36.000000 pypcapkit-1.0.0b1/pcapkit/const/reg/ethertype.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    37259 2023-04-21 04:00:41.000000 pypcapkit-1.0.0b1/pcapkit/const/reg/linktype.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    12815 2023-04-21 04:00:41.000000 pypcapkit-1.0.0b1/pcapkit/const/reg/transtype.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.339630 pypcapkit-1.0.0b1/pcapkit/const/tcp/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1049 2023-04-18 02:53:54.000000 pypcapkit-1.0.0b1/pcapkit/const/tcp/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1536 2023-04-21 04:05:46.000000 pypcapkit-1.0.0b1/pcapkit/const/tcp/checksum.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1606 2023-04-21 04:05:47.000000 pypcapkit-1.0.0b1/pcapkit/const/tcp/mp_tcp_option.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5824 2023-04-21 04:05:47.000000 pypcapkit-1.0.0b1/pcapkit/const/tcp/option.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.340573 pypcapkit-1.0.0b1/pcapkit/const/vlan/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      690 2023-04-18 02:55:34.000000 pypcapkit-1.0.0b1/pcapkit/const/vlan/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1948 2023-04-21 04:07:03.000000 pypcapkit-1.0.0b1/pcapkit/const/vlan/priority_level.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.343235 pypcapkit-1.0.0b1/pcapkit/corekit/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1420 2023-04-18 03:07:32.000000 pypcapkit-1.0.0b1/pcapkit/corekit/__init__.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.346065 pypcapkit-1.0.0b1/pcapkit/corekit/fields/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1388 2023-04-18 03:07:49.000000 pypcapkit-1.0.0b1/pcapkit/corekit/fields/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     8758 2023-04-18 05:44:09.000000 pypcapkit-1.0.0b1/pcapkit/corekit/fields/collections.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6061 2023-04-19 07:56:40.000000 pypcapkit-1.0.0b1/pcapkit/corekit/fields/field.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3614 2023-04-18 05:41:59.000000 pypcapkit-1.0.0b1/pcapkit/corekit/fields/ipaddress.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    17824 2023-04-18 05:48:36.000000 pypcapkit-1.0.0b1/pcapkit/corekit/fields/misc.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    11410 2023-04-18 05:39:55.000000 pypcapkit-1.0.0b1/pcapkit/corekit/fields/numbers.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     8449 2023-04-21 03:49:48.000000 pypcapkit-1.0.0b1/pcapkit/corekit/fields/strings.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    10595 2023-04-18 05:49:51.000000 pypcapkit-1.0.0b1/pcapkit/corekit/infoclass.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    21969 2023-04-18 05:56:59.000000 pypcapkit-1.0.0b1/pcapkit/corekit/multidict.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     7477 2023-04-18 05:59:31.000000 pypcapkit-1.0.0b1/pcapkit/corekit/protochain.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      470 2023-04-18 06:00:49.000000 pypcapkit-1.0.0b1/pcapkit/corekit/version.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.347682 pypcapkit-1.0.0b1/pcapkit/dumpkit/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      370 2023-04-18 06:03:18.000000 pypcapkit-1.0.0b1/pcapkit/dumpkit/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3055 2023-04-18 06:08:44.000000 pypcapkit-1.0.0b1/pcapkit/dumpkit/common.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2243 2023-04-18 06:09:05.000000 pypcapkit-1.0.0b1/pcapkit/dumpkit/null.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4165 2023-04-18 06:09:35.000000 pypcapkit-1.0.0b1/pcapkit/dumpkit/pcap.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.348943 pypcapkit-1.0.0b1/pcapkit/foundation/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1214 2023-04-18 07:18:15.000000 pypcapkit-1.0.0b1/pcapkit/foundation/__init__.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.350749 pypcapkit-1.0.0b1/pcapkit/foundation/engines/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      858 2023-04-20 03:46:19.000000 pypcapkit-1.0.0b1/pcapkit/foundation/engines/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6256 2023-04-19 07:18:07.000000 pypcapkit-1.0.0b1/pcapkit/foundation/engines/dpkt.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2496 2023-04-19 07:18:10.000000 pypcapkit-1.0.0b1/pcapkit/foundation/engines/engine.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5248 2023-04-19 07:18:13.000000 pypcapkit-1.0.0b1/pcapkit/foundation/engines/pcap.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5419 2023-04-19 07:18:17.000000 pypcapkit-1.0.0b1/pcapkit/foundation/engines/pyshark.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5234 2023-04-19 07:18:19.000000 pypcapkit-1.0.0b1/pcapkit/foundation/engines/scapy.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    27816 2023-04-19 09:16:23.000000 pypcapkit-1.0.0b1/pcapkit/foundation/extraction.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.352391 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1454 2023-04-18 08:19:07.000000 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/__init__.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.353236 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/data/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1900 2023-04-14 09:51:51.000000 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/data/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4112 2023-04-19 09:16:36.000000 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/data/ip.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5061 2023-04-19 09:16:13.000000 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/data/tcp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6281 2023-04-18 08:40:51.000000 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/ip.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1684 2023-04-18 08:40:57.000000 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/ipv4.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1684 2023-04-18 08:40:59.000000 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/ipv6.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6430 2023-04-18 08:22:25.000000 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/reassembly.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     9922 2023-04-19 10:55:26.000000 pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/tcp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    24943 2023-04-19 07:17:03.000000 pypcapkit-1.0.0b1/pcapkit/foundation/registry.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.354376 pypcapkit-1.0.0b1/pcapkit/foundation/traceflow/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      975 2023-04-18 09:02:47.000000 pypcapkit-1.0.0b1/pcapkit/foundation/traceflow/__init__.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.355228 pypcapkit-1.0.0b1/pcapkit/foundation/traceflow/data/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      895 2023-04-14 09:51:51.000000 pypcapkit-1.0.0b1/pcapkit/foundation/traceflow/data/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2954 2023-04-18 08:49:23.000000 pypcapkit-1.0.0b1/pcapkit/foundation/traceflow/data/tcp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5520 2023-04-18 09:05:48.000000 pypcapkit-1.0.0b1/pcapkit/foundation/traceflow/tcp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     8711 2023-04-18 09:05:42.000000 pypcapkit-1.0.0b1/pcapkit/foundation/traceflow/traceflow.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.355961 pypcapkit-1.0.0b1/pcapkit/interface/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      809 2023-04-18 11:55:54.000000 pypcapkit-1.0.0b1/pcapkit/interface/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     7499 2023-04-18 12:03:05.000000 pypcapkit-1.0.0b1/pcapkit/interface/core.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4804 2023-04-18 12:05:26.000000 pypcapkit-1.0.0b1/pcapkit/interface/misc.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.356492 pypcapkit-1.0.0b1/pcapkit/protocols/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1734 2023-04-19 07:26:06.000000 pypcapkit-1.0.0b1/pcapkit/protocols/__init__.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.360468 pypcapkit-1.0.0b1/pcapkit/protocols/application/
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.366110 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/bgp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/dhcp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/dhcpv6.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/dns.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/imap.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/ldap.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/mqtt.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/nntp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/ntp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/onc_rpc.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/pop.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/rip.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/rtp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/sip.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/smtp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/snmp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/ssh.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/telnet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/tls.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/NotImplemented/xmpp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      936 2023-04-19 16:34:36.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4302 2023-04-19 16:34:58.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/application.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6532 2023-04-21 03:47:15.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/ftp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6268 2023-04-19 16:51:00.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/http.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    11617 2023-04-21 03:47:31.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/httpv1.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    49224 2023-04-21 03:49:26.000000 pypcapkit-1.0.0b1/pcapkit/protocols/application/httpv2.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.366897 pypcapkit-1.0.0b1/pcapkit/protocols/data/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6366 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/__init__.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.368858 pypcapkit-1.0.0b1/pcapkit/protocols/data/application/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3270 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/application/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1432 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/application/ftp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2294 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/application/httpv1.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     9209 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/application/httpv2.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      234 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/data.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.372537 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    15499 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      741 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/ah.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    28229 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/hip.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    11866 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/hopopt.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    11909 2023-04-19 09:27:44.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/ipv4.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1751 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/ipv6.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      689 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/ipv6_frag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    12311 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/ipv6_opts.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2450 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/ipv6_route.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1420 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/ipx.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      794 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/internet/mh.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.374704 pypcapkit-1.0.0b1/pcapkit/protocols/data/link/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      956 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/link/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2248 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/link/arp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      656 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/link/ethernet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1521 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/link/l2tp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1561 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/link/ospf.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1090 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/link/vlan.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.375675 pypcapkit-1.0.0b1/pcapkit/protocols/data/misc/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      431 2023-04-10 14:22:26.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/misc/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      524 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/misc/null.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.376741 pypcapkit-1.0.0b1/pcapkit/protocols/data/misc/pcap/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      535 2023-04-10 14:22:34.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/misc/pcap/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1460 2023-03-10 01:26:15.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/misc/pcap/frame.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1518 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/misc/pcap/header.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      691 2023-02-08 01:02:20.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/misc/raw.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      489 2023-02-08 01:03:00.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/protocol.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.377632 pypcapkit-1.0.0b1/pcapkit/protocols/data/transport/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4490 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/transport/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    17409 2023-04-19 10:39:07.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/transport/tcp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      609 2023-03-15 06:50:18.000000 pypcapkit-1.0.0b1/pcapkit/protocols/data/transport/udp.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.384263 pypcapkit-1.0.0b1/pcapkit/protocols/internet/
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.385751 pypcapkit-1.0.0b1/pcapkit/protocols/internet/NotImplemented/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:10.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/NotImplemented/ecn.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4448 2023-04-19 08:19:10.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/NotImplemented/esp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:10.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/NotImplemented/icmp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:10.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/NotImplemented/icmpv6.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:10.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/NotImplemented/igmp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:10.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/NotImplemented/shim6.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1507 2023-04-19 08:04:39.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    10193 2023-04-19 08:09:28.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/ah.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)   209855 2023-04-19 08:18:33.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/hip.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    76152 2023-04-19 08:57:55.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/hopopt.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    10111 2023-04-19 08:04:26.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/internet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1648 2023-04-19 09:25:53.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/ip.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1539 2023-04-19 09:26:14.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/ipsec.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    70654 2023-04-21 00:41:49.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/ipv4.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    13618 2023-04-19 10:21:09.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/ipv6.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     9356 2023-04-19 10:05:24.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/ipv6_frag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    76974 2023-04-19 10:11:42.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/ipv6_opts.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    29634 2023-04-19 10:16:36.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/ipv6_route.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     7802 2023-04-19 10:26:15.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/ipx.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     9877 2023-04-19 10:27:02.000000 pypcapkit-1.0.0b1/pcapkit/protocols/internet/mh.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.388275 pypcapkit-1.0.0b1/pcapkit/protocols/link/
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.389951 pypcapkit-1.0.0b1/pcapkit/protocols/link/NotImplemented/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:07.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/NotImplemented/dsl.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)       24 2023-04-19 08:19:07.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/NotImplemented/eapol.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:07.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/NotImplemented/fddi.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:07.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/NotImplemented/isdn.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:07.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/NotImplemented/ndp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:07.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/NotImplemented/ppp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      998 2023-04-19 16:42:38.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    17024 2023-04-19 16:41:32.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/arp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     8283 2023-04-19 03:51:29.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/ethernet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    10683 2023-04-19 04:00:25.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/l2tp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5056 2023-04-19 03:23:33.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/link.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    13436 2023-04-19 07:15:32.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/ospf.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3250 2023-04-19 16:43:48.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/rarp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     8604 2023-04-19 07:44:39.000000 pypcapkit-1.0.0b1/pcapkit/protocols/link/vlan.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.390840 pypcapkit-1.0.0b1/pcapkit/protocols/misc/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      756 2023-04-19 03:20:32.000000 pypcapkit-1.0.0b1/pcapkit/protocols/misc/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4224 2023-04-19 03:11:39.000000 pypcapkit-1.0.0b1/pcapkit/protocols/misc/null.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.392288 pypcapkit-1.0.0b1/pcapkit/protocols/misc/pcap/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      542 2023-04-19 03:20:37.000000 pypcapkit-1.0.0b1/pcapkit/protocols/misc/pcap/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    14468 2023-04-19 03:01:45.000000 pypcapkit-1.0.0b1/pcapkit/protocols/misc/pcap/frame.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    12696 2023-04-19 02:59:25.000000 pypcapkit-1.0.0b1/pcapkit/protocols/misc/pcap/header.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5933 2023-04-19 03:07:58.000000 pypcapkit-1.0.0b1/pcapkit/protocols/misc/raw.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    42030 2023-04-19 02:59:04.000000 pypcapkit-1.0.0b1/pcapkit/protocols/protocol.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.393659 pypcapkit-1.0.0b1/pcapkit/protocols/schema/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4761 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/__init__.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.396202 pypcapkit-1.0.0b1/pcapkit/protocols/schema/application/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1997 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/application/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      492 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/application/ftp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      495 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/application/httpv1.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    11577 2023-04-20 01:27:14.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/application/httpv2.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.402542 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    14881 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1306 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/ah.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    42307 2023-04-21 03:52:49.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/hip.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    21355 2023-04-19 09:05:50.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/hopopt.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    19514 2023-04-19 09:34:05.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/ipv4.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1980 2023-04-19 10:22:32.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/ipv6.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1390 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/ipv6_frag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    21454 2023-04-19 10:12:35.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/ipv6_opts.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6827 2023-04-19 10:19:11.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/ipv6_route.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1333 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/ipx.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1373 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/internet/mh.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.404762 pypcapkit-1.0.0b1/pcapkit/protocols/schema/link/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      644 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/link/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1583 2023-04-19 08:37:29.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/link/arp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1664 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/link/ethernet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2716 2023-04-19 09:19:06.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/link/l2tp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3155 2023-04-19 08:18:33.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/link/ospf.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2121 2023-04-20 03:44:28.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/link/vlan.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.406065 pypcapkit-1.0.0b1/pcapkit/protocols/schema/misc/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      376 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/misc/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      550 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/misc/null.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.406674 pypcapkit-1.0.0b1/pcapkit/protocols/schema/misc/pcap/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      228 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/misc/pcap/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1127 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/misc/pcap/frame.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2287 2023-04-14 09:38:13.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/misc/pcap/header.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1188 2023-04-17 07:59:07.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/misc/pcapng.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      723 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/misc/raw.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    18250 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/schema.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.407786 pypcapkit-1.0.0b1/pcapkit/protocols/schema/transport/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4377 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/transport/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    26970 2023-04-19 10:39:39.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/transport/tcp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1001 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/protocols/schema/transport/udp.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.409204 pypcapkit-1.0.0b1/pcapkit/protocols/transport/
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.409716 pypcapkit-1.0.0b1/pcapkit/protocols/transport/NotImplemented/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:12.000000 pypcapkit-1.0.0b1/pcapkit/protocols/transport/NotImplemented/dccp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:12.000000 pypcapkit-1.0.0b1/pcapkit/protocols/transport/NotImplemented/rsvp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        0 2023-04-19 08:19:12.000000 pypcapkit-1.0.0b1/pcapkit/protocols/transport/NotImplemented/sctp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      780 2023-04-19 10:30:08.000000 pypcapkit-1.0.0b1/pcapkit/protocols/transport/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)   113820 2023-04-19 16:18:50.000000 pypcapkit-1.0.0b1/pcapkit/protocols/transport/tcp.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6054 2023-04-20 03:44:28.000000 pypcapkit-1.0.0b1/pcapkit/protocols/transport/transport.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6850 2023-04-19 10:36:12.000000 pypcapkit-1.0.0b1/pcapkit/protocols/transport/udp.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.410886 pypcapkit-1.0.0b1/pcapkit/toolkit/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2124 2023-04-18 12:10:13.000000 pypcapkit-1.0.0b1/pcapkit/toolkit/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     9128 2023-04-19 09:12:56.000000 pypcapkit-1.0.0b1/pcapkit/toolkit/default.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    12433 2023-04-19 09:13:09.000000 pypcapkit-1.0.0b1/pcapkit/toolkit/dpkt.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3388 2023-04-18 12:16:01.000000 pypcapkit-1.0.0b1/pcapkit/toolkit/pyshark.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    11400 2023-04-19 09:13:32.000000 pypcapkit-1.0.0b1/pcapkit/toolkit/scapy.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.413070 pypcapkit-1.0.0b1/pcapkit/utilities/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      694 2023-04-18 12:32:34.000000 pypcapkit-1.0.0b1/pcapkit/utilities/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4620 2023-04-21 03:46:54.000000 pypcapkit-1.0.0b1/pcapkit/utilities/compat.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6516 2023-04-18 12:25:58.000000 pypcapkit-1.0.0b1/pcapkit/utilities/decorators.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    10471 2023-04-18 12:29:35.000000 pypcapkit-1.0.0b1/pcapkit/utilities/exceptions.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1918 2023-04-19 07:40:45.000000 pypcapkit-1.0.0b1/pcapkit/utilities/logging.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4102 2023-04-18 12:44:15.000000 pypcapkit-1.0.0b1/pcapkit/utilities/warnings.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.414565 pypcapkit-1.0.0b1/pcapkit/vendor/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3694 2023-04-18 12:50:39.000000 pypcapkit-1.0.0b1/pcapkit/vendor/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2617 2023-04-20 02:19:39.000000 pypcapkit-1.0.0b1/pcapkit/vendor/__main__.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.415845 pypcapkit-1.0.0b1/pcapkit/vendor/arp/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      983 2023-04-18 13:02:06.000000 pypcapkit-1.0.0b1/pcapkit/vendor/arp/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      686 2023-04-18 13:03:04.000000 pypcapkit-1.0.0b1/pcapkit/vendor/arp/hardware.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      696 2023-04-18 13:03:10.000000 pypcapkit-1.0.0b1/pcapkit/vendor/arp/operation.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    13702 2023-04-21 00:42:16.000000 pypcapkit-1.0.0b1/pcapkit/vendor/default.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.416952 pypcapkit-1.0.0b1/pcapkit/vendor/ftp/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      948 2023-04-18 13:30:03.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ftp/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5344 2023-04-18 13:30:23.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ftp/command.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6262 2023-04-18 13:30:41.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ftp/return_code.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.443542 pypcapkit-1.0.0b1/pcapkit/vendor/hip/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5603 2023-04-13 09:24:51.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      704 2023-04-18 13:37:31.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/certificate.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      628 2023-04-18 13:37:37.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/cipher.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      616 2023-04-18 13:37:41.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/di.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      686 2023-04-18 13:37:47.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/ecdsa_curve.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      726 2023-04-18 13:37:53.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/ecdsa_low_curve.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2722 2023-04-18 13:37:58.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/eddsa_curve.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      760 2023-04-18 13:38:03.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/esp_transform_suite.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2586 2023-04-18 13:38:09.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/group.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      667 2023-04-18 13:38:14.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/hi_algorithm.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      646 2023-04-18 13:38:18.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/hit_suite.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      718 2023-04-18 13:38:23.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/nat_traversal.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      715 2023-04-18 13:38:29.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/notify_message.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2629 2023-04-18 13:38:34.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/packet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2715 2023-04-18 13:38:39.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/parameter.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      698 2023-04-18 13:38:48.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/registration.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      774 2023-04-18 13:38:43.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/registration_failure.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      621 2023-04-18 13:39:00.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/suite.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      680 2023-04-18 13:39:06.000000 pypcapkit-1.0.0b1/pcapkit/vendor/hip/transport.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.461870 pypcapkit-1.0.0b1/pcapkit/vendor/http/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1760 2023-04-18 13:43:44.000000 pypcapkit-1.0.0b1/pcapkit/vendor/http/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3107 2023-04-18 13:43:50.000000 pypcapkit-1.0.0b1/pcapkit/vendor/http/error_code.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2915 2023-04-18 13:43:53.000000 pypcapkit-1.0.0b1/pcapkit/vendor/http/frame.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4553 2023-04-18 13:43:59.000000 pypcapkit-1.0.0b1/pcapkit/vendor/http/method.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3024 2023-04-18 13:44:02.000000 pypcapkit-1.0.0b1/pcapkit/vendor/http/setting.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     5152 2023-04-18 13:44:06.000000 pypcapkit-1.0.0b1/pcapkit/vendor/http/status_code.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.480224 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3044 2022-08-04 23:59:18.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2520 2023-04-18 13:51:47.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/classification_level.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2049 2023-04-18 13:51:57.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/option_class.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3041 2023-04-18 13:52:02.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/option_number.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2231 2023-04-18 13:52:08.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/protection_authority.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1974 2023-04-18 13:52:12.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/qs_function.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3082 2023-04-18 13:52:16.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/router_alert.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1953 2023-04-18 13:52:21.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/tos_del.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2475 2023-04-18 13:52:26.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/tos_ecn.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2170 2023-04-18 13:52:32.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/tos_pre.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2002 2023-04-18 13:52:36.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/tos_rel.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1966 2023-04-18 13:52:42.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/tos_thr.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1987 2023-04-18 13:52:47.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv4/ts_flag.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.499419 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2815 2023-04-18 13:55:03.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4957 2023-04-18 13:55:08.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/extension_header.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3081 2023-04-18 13:55:20.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/option.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2649 2023-04-18 13:55:15.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/option_action.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1974 2023-04-18 13:55:24.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/qs_function.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3086 2023-04-18 13:55:29.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/router_alert.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2642 2023-04-18 13:55:33.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/routing.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2214 2023-04-18 13:55:38.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/seed_id.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2224 2023-04-18 13:55:42.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/smf_dpd_mode.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2441 2023-04-18 13:55:46.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipv6/tagger_id.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.504676 pypcapkit-1.0.0b1/pcapkit/vendor/ipx/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1291 2023-04-18 13:59:01.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipx/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3460 2023-04-18 13:59:06.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipx/packet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3655 2023-04-18 13:59:10.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ipx/socket.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.505142 pypcapkit-1.0.0b1/pcapkit/vendor/l2tp/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      533 2023-04-18 14:00:52.000000 pypcapkit-1.0.0b1/pcapkit/vendor/l2tp/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1914 2023-04-18 14:00:59.000000 pypcapkit-1.0.0b1/pcapkit/vendor/l2tp/type.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.514413 pypcapkit-1.0.0b1/pcapkit/vendor/mh/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    13313 2023-04-18 14:10:12.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2712 2023-04-18 14:10:21.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/access_type.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2762 2023-04-18 14:10:28.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/ack_status_code.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2831 2023-04-18 14:10:54.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/ani_suboption.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2526 2023-04-18 14:11:04.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/auth_subtype.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4112 2023-04-18 14:11:14.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/binding_ack_flag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2684 2023-04-18 14:11:24.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/binding_revocation.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     4099 2023-04-18 14:11:31.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/binding_update_flag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2273 2023-04-18 14:11:39.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/dhcp_support_mode.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2731 2023-04-18 14:11:45.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/dns_status_code.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2709 2023-04-18 14:11:55.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/dsmip6_tls_packet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2860 2023-04-18 14:12:03.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/dsmipv6_home_address.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2393 2023-04-18 14:12:10.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/enumerating_algorithm.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2758 2023-04-18 14:12:17.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/fb_ack_status.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2747 2023-04-18 14:12:24.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/fb_action.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2779 2023-04-18 14:12:30.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/fb_indication_trigger.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2695 2023-04-18 14:12:35.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/fb_type.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2740 2023-04-18 14:12:42.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/flow_id_status.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2701 2023-04-18 14:12:48.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/flow_id_suboption.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2703 2023-04-18 14:12:53.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/handoff_type.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3921 2023-04-18 14:13:01.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/handover_ack_flag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2730 2023-04-18 14:13:08.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/handover_ack_status.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3936 2023-04-18 14:13:15.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/handover_initiate_flag.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2745 2023-04-18 14:13:22.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/handover_initiate_status.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2727 2023-04-18 14:13:29.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/home_address_reply.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2921 2023-04-18 14:13:38.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/lma_mag_suboption.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2716 2023-04-18 14:13:44.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/mn_group_id.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2710 2023-04-18 14:13:52.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/mn_id_subtype.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2664 2023-04-18 14:13:57.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/operator_id.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2283 2023-04-18 14:14:02.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/option.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2490 2023-04-18 14:14:07.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/packet.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2700 2023-04-18 14:14:13.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/qos_attribute.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2798 2023-04-18 14:14:20.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/revocation_status_code.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2694 2023-04-18 14:14:26.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/revocation_trigger.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2835 2023-04-18 14:14:31.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/status_code.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2665 2023-04-18 14:14:38.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/traffic_selector.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2807 2023-04-18 14:14:46.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/upa_status.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2736 2023-04-18 14:14:51.000000 pypcapkit-1.0.0b1/pcapkit/vendor/mh/upn_reason.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.514962 pypcapkit-1.0.0b1/pcapkit/vendor/ospf/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1010 2023-04-18 14:15:22.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ospf/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      737 2023-04-18 14:15:29.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ospf/authentication.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      668 2023-04-18 14:15:35.000000 pypcapkit-1.0.0b1/pcapkit/vendor/ospf/packet.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.516000 pypcapkit-1.0.0b1/pcapkit/vendor/pcapng/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      666 2023-04-18 14:16:30.000000 pypcapkit-1.0.0b1/pcapkit/vendor/pcapng/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2760 2023-04-18 14:16:42.000000 pypcapkit-1.0.0b1/pcapkit/vendor/pcapng/block_type.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.517237 pypcapkit-1.0.0b1/pcapkit/vendor/reg/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1085 2023-04-18 14:16:50.000000 pypcapkit-1.0.0b1/pcapkit/vendor/reg/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3798 2023-04-18 14:16:59.000000 pypcapkit-1.0.0b1/pcapkit/vendor/reg/ethertype.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3309 2023-04-18 14:17:05.000000 pypcapkit-1.0.0b1/pcapkit/vendor/reg/linktype.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3411 2023-04-18 14:17:11.000000 pypcapkit-1.0.0b1/pcapkit/vendor/reg/transtype.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.518078 pypcapkit-1.0.0b1/pcapkit/vendor/tcp/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1132 2023-04-18 14:16:23.000000 pypcapkit-1.0.0b1/pcapkit/vendor/tcp/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2053 2023-04-18 14:16:18.000000 pypcapkit-1.0.0b1/pcapkit/vendor/tcp/checksum.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2145 2023-04-18 14:16:11.000000 pypcapkit-1.0.0b1/pcapkit/vendor/tcp/mp_tcp_option.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3004 2023-04-18 14:16:01.000000 pypcapkit-1.0.0b1/pcapkit/vendor/tcp/option.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.518496 pypcapkit-1.0.0b1/pcapkit/vendor/vlan/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      674 2023-04-18 14:15:53.000000 pypcapkit-1.0.0b1/pcapkit/vendor/vlan/__init__.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2986 2023-04-18 14:15:47.000000 pypcapkit-1.0.0b1/pcapkit/vendor/vlan/priority_level.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-04-21 04:07:17.520022 pypcapkit-1.0.0b1/pypcapkit.egg-info/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     6856 2023-04-21 04:07:14.000000 pypcapkit-1.0.0b1/pypcapkit.egg-info/PKG-INFO
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    15754 2023-04-21 04:07:17.000000 pypcapkit-1.0.0b1/pypcapkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        1 2023-04-21 04:07:14.000000 pypcapkit-1.0.0b1/pypcapkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      100 2023-04-21 04:07:14.000000 pypcapkit-1.0.0b1/pypcapkit.egg-info/entry_points.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        1 2023-04-20 12:48:49.000000 pypcapkit-1.0.0b1/pypcapkit.egg-info/not-zip-safe
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      335 2023-04-21 04:07:14.000000 pypcapkit-1.0.0b1/pypcapkit.egg-info/requires.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        8 2023-04-21 04:07:14.000000 pypcapkit-1.0.0b1/pypcapkit.egg-info/top_level.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3203 2023-04-21 03:52:08.000000 pypcapkit-1.0.0b1/pyproject.toml
+-rw-r--r--   0 jarryshaw   (501) staff       (20)       38 2023-04-21 04:07:17.520439 pypcapkit-1.0.0b1/setup.cfg
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3649 2023-04-21 03:50:54.000000 pypcapkit-1.0.0b1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/corekit/infoclass.py` & `pypcapkit-1.0.0b1/pcapkit/const/hip/packet.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,92 @@
 # -*- coding: utf-8 -*-
-"""info class
+# pylint: disable=line-too-long,consider-using-f-string
+"""HIP Packet Types
+======================
 
-`pcapkit.corekit.infoclass` contains dict-like class
-`Info` only, which is originally designed to work alike
-`dataclasses.dataclass` in Python 3.7 and later versions.
+.. module:: pcapkit.const.hip.packet
+
+This module contains the constant enumeration for **HIP Packet Types**,
+which is automatically generated from :class:`pcapkit.vendor.hip.packet.Packet`.
 
 """
-import copy
 
-from pcapkit.utilities.exceptions import UnsupportedCall
-from pcapkit.utilities.validations import dict_check
+from aenum import IntEnum, extend_enum
 
+__all__ = ['Packet']
 
-__all__ = ['Info']
 
+class Packet(IntEnum):
+    """[Packet] HIP Packet Types"""
 
-class Info(dict):
-    """Turn dictionaries into object-like instances.
-
-    Methods:
-        * infotodict -- reverse Info object into dict type
-
-    Notes:
-        * Info objects inherit from `dict` type
-        * Info objects are iterable, and support all functions as `dict`
-        * Info objects are one-time-modeling, thus cannot set or delete
-            attributes after initialisation
-
-    """
-    def __new__(cls, dict_=None, **kwargs):
-        def __read__(dict_):
-            __dict__ = dict()
-            for (key, value) in dict_.items():
-                if isinstance(value, dict):
-                    __dict__[key] = Info(value)
-                else:
-                    # if isinstance(key, str):
-                    #     key = re.sub('\W', '_', key)
-                    __dict__[key] = value
-            return __dict__
-
-        self = super().__new__(cls)
-        if dict_ is not None:
-            if isinstance(dict_, Info):
-                self = copy.deepcopy(dict_)
-            else:
-                dict_check(dict_)
-                self.__dict__.update(__read__(dict_))
-
-        self.__dict__.update(__read__(kwargs))
-        return self
-
-    def __repr__(self):
-        temp = list()
-        for (key, value) in self.__dict__.items():
-            temp.append(f'{key}={value}')
-        args = ', '.join(temp)
-        return f'Info({args})'
-
-    __str__ = __repr__
-
-    def __iter__(self):
-        return iter(self.__dict__)
-
-    def __getitem__(self, key):
-        return self.__dict__[key]
-
-    def __contains__(self, name):
-        return (name in self.__dict__)
-
-    def __setattr__(self, name, value):
-        raise UnsupportedCall("can't set attribute")
-
-    def __delattr__(self, name):
-        raise UnsupportedCall("can't delete attribute")
-
-    def infotodict(self):
-        dict_ = dict()
-        for (key, value) in self.__dict__.items():
-            if isinstance(value, Info):
-                dict_[key] = value.infotodict()
-            elif isinstance(value, (tuple, list)):
-                temp = list()
-                for item in value:
-                    if isinstance(item, Info):
-                        temp.append(item.infotodict())
-                    else:
-                        temp.append(item)
-                dict_[key] = value.__class__(temp)
-            else:
-                dict_[key] = value
-        return dict_
+    #: Reserved [:rfc:`7401`]
+    Reserved_0 = 0
+
+    #: I1 the HIP Initiator Packet [:rfc:`7401`]
+    I1 = 1
+
+    #: R1 the HIP Responder Packet [:rfc:`7401`]
+    R1 = 2
+
+    #: I2 the Second HIP Initiator Packet [:rfc:`7401`]
+    I2 = 3
+
+    #: R2 the Second HIP Responder Packet [:rfc:`7401`]
+    R2 = 4
+
+    #: UPDATE the HIP Update Packet [:rfc:`7401`]
+    UPDATE = 16
+
+    #: NOTIFY the HIP Notify Packet [:rfc:`7401`]
+    NOTIFY = 17
+
+    #: CLOSE the HIP Association Closing Packet [:rfc:`7401`]
+    CLOSE = 18
+
+    #: CLOSE_ACK the HIP Closing Acknowledgment Packet [:rfc:`7401`]
+    CLOSE_ACK = 19
+
+    #: HDRR (HIP Distributed Hash Table Resource Record) [:rfc:`6537`]
+    HDRR = 20
+
+    #: HIP_DATA [:rfc:`6078`]
+    HIP_DATA = 32
+
+    @staticmethod
+    def get(key: 'int | str', default: 'int' = -1) -> 'Packet':
+        """Backport support for original codes.
+
+        Args:
+            key: Key to get enum item.
+            default: Default value if not found.
+
+        :meta private:
+        """
+        if isinstance(key, int):
+            return Packet(key)
+        if key not in Packet._member_map_:  # pylint: disable=no-member
+            extend_enum(Packet, key, default)
+        return Packet[key]  # type: ignore[misc]
+
+    @classmethod
+    def _missing_(cls, value: 'int') -> 'Packet':
+        """Lookup function used when value is not found.
+
+        Args:
+            value: Value to get enum item.
+
+        """
+        if not (isinstance(value, int) and 0 <= value <= 127):
+            raise ValueError('%r is not a valid %s' % (value, cls.__name__))
+        if 5 <= value <= 15:
+            # Unassigned
+            extend_enum(cls, 'Unassigned_%d' % value, value)
+            return cls(value)
+        if 21 <= value <= 31:
+            # Unassigned
+            extend_enum(cls, 'Unassigned_%d' % value, value)
+            return cls(value)
+        if 33 <= value <= 127:
+            # Unassigned
+            extend_enum(cls, 'Unassigned_%d' % value, value)
+            return cls(value)
+        return super()._missing_(value)
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/foundation/traceflow.py` & `pypcapkit-1.0.0b1/pcapkit/foundation/traceflow/traceflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,219 +1,260 @@
 # -*- coding: utf-8 -*-
-"""trace TCP flows
+"""Base Class
+================
 
-`pcapkit.foundation.traceflow` is the interface to trace
-TCP flows from a series of packets and connections. This
-was implemented as the demand of my mate @gousaiyang.
+.. module:: pcapkit.foundation.traceflow.traceflow
+
+:mod:`pcapkit.foundation.traceflow.traceflow` contains
+:class:`~pcapkit.foundation.traceflow.traceflow.TraceFlow` only,
+which is an abstract base class for all flow tracing classes.
 
 """
-import copy
-import pathlib
-import warnings
-
-###############################################################################
-# from dictdumper import PLIST, JSON, Tree, JavaScript, XML
-###############################################################################
+import abc
+import collections
+import importlib
+import os
+import sys
+from typing import TYPE_CHECKING, Generic, TypeVar, overload
 
 from pcapkit.corekit.infoclass import Info
-from pcapkit.utilities.exceptions import stacklevel, FileExists
-from pcapkit.utilities.warnings import FormatWarning, FileWarning
-from pcapkit.utilities.validations import pkt_check
-
-###############################################################################
-# from pcapkit.dumpkit import PCAP, NotImplementedIO
-###############################################################################
+from pcapkit.dumpkit.common import _append_fallback as dumpkit_append_fallback
+from pcapkit.dumpkit.common import default as dumpkit_default
+from pcapkit.dumpkit.common import object_hook as dumpkit_object_hook
+from pcapkit.utilities.exceptions import FileExists, stacklevel
+from pcapkit.utilities.warnings import FileWarning, FormatWarning, warn
+
+__all__ = ['TraceFlow']
+
+if TYPE_CHECKING:
+    from typing import Any, DefaultDict, Optional, Type
+
+    from dictdumper.dumper import Dumper
+    from typing_extensions import Literal
+
+    from pcapkit.protocols.protocol import Protocol
+
+BufferID = TypeVar('BufferID')
+Buffer = TypeVar('Buffer', bound='Info')
+Index = TypeVar('Index', bound='Info')
+Packet = TypeVar('Packet', bound='Info')
+
+
+class TraceFlow(Generic[BufferID, Buffer, Index, Packet], metaclass=abc.ABCMeta):
+    """Base flow tracing class.
+
+    Arguments:
+        fout: output path
+        format: output format
+        byteorder: output file byte order
+        nanosecond: output nanosecond-resolution file flag
+        *args: Arbitrary positional arguments.
+        **kwargs: Arbitrary keyword arguments.
 
+    """
 
-class TraceFlow:
-    """Trace TCP flows.
+    # Internal data storage for cached properties.
+    __cached__: 'dict[str, Any]'
 
-    Properties:
-        * index -- tuple<Info>, index table for traced flows
+    ##########################################################################
+    # Defaults.
+    ##########################################################################
 
-    Methods:
-        * make_fout -- make root path for output
-        * dump -- dump frame to output files
-        * trace -- trace packets
+    #: DefaultDict[str, tuple[str, str, str | None]]: Format dumper mapping for
+    #: writing output files. The values should be a tuple representing the
+    #: module name, class name and file extension.
+    __output__ = collections.defaultdict(
+        lambda: ('pcapkit.dumpkit', 'NotImplementedIO', None),
+        {
+            'pcap': ('pcapkit.dumpkit', 'PCAPIO', '.pcap'),
+            'cap': ('pcapkit.dumpkit', 'PCAPIO', '.pcap'),
+            'plist': ('dictdumper', 'PLIST', '.plist'),
+            'xml': ('dictdumper', 'PLIST', '.plist'),
+            'json': ('dictdumper', 'JSON', '.json'),
+            'tree': ('dictdumper', 'Tree', '.txt'),
+            'text': ('dictdumper', 'Text', '.txt'),
+            'txt': ('dictdumper', 'Tree', '.txt'),
+        }
+    )  # type: DefaultDict[str, tuple[str, str, str | None]]
 
-    """
     ##########################################################################
     # Properties.
     ##########################################################################
 
     @property
-    def index(self):
-        if self._newflg:
+    @abc.abstractmethod
+    def name(self) -> 'str':
+        """Protocol name of current reassembly object."""
+
+    @property
+    @abc.abstractmethod
+    def protocol(self) -> 'Type[Protocol]':
+        """Protocol of current reassembly object."""
+
+    @property
+    def index(self) -> 'tuple[Index, ...]':
+        """Index table for traced flow."""
+        if self._buffer:
             return self.submit()
         return tuple(self._stream)
 
     ##########################################################################
     # Methods.
     ##########################################################################
 
-    @staticmethod
-    def make_fout(fout='./tmp', fmt='pcap'):
+    @classmethod
+    def register(cls, format: 'str', module: 'str', class_: 'str', ext: 'str') -> 'None':  # pylint: disable=redefined-builtin
+        r"""Register a new dumper class.
+
+        Notes:
+            The full qualified class name of the new dumper class
+            should be as ``{module}.{class_}``.
+
+        Arguments:
+            format: format name
+            module: module name
+            class\_: class name
+            ext: file extension
+
+        """
+        cls.__output__[format] = (module, class_, ext)
+
+    @classmethod
+    def make_fout(cls, fout: 'str' = './tmp', fmt: 'str' = 'pcap') -> 'tuple[Type[Dumper], str | None]':
         """Make root path for output.
 
-        Positional arguments:
-            * fout -- str, root path for output
-            * fmt -- str, output format
+        Args:
+            fout: root path for output
+            fmt: output format
 
         Returns:
-            * output -- dumper of specified format
+            Dumper of specified format and file extension of output file.
+
+        Warns:
+            FormatWarning: If ``fmt`` is not supported.
+            FileWarning: If ``fout`` exists and ``fmt`` is :data:`None`.
+
+        Raises:
+            FileExists: If ``fout`` exists and ``fmt`` is **NOT** :data:`None`.
 
         """
-        if fmt == 'pcap':
-            from pcapkit.dumpkit import PCAP as output      # output PCAP file 
-        elif fmt == 'plist':
-            from dictdumper import PLIST as output          # output PLIST file
-        elif fmt == 'json':
-            from dictdumper import JSON as output           # output JSON file
-        elif fmt == 'tree':
-            from dictdumper import Tree as output           # output treeview text file
-            fmt = 'txt'
-        elif fmt == 'html':
-            from dictdumper import JavaScript as output     # output JavaScript file
-            fmt = 'js'
-        elif fmt == 'xml':
-            from dictdumper import XML as output            # output XML file
-        else:
-            from pcapkit.dumpkit import NotImplementedIO as output
-                                                            # no output file
-            if fmt is not None:
-                warnings.warn(f'Unsupported output format: {fmt}; '
-                                'disabled file output feature',
-                                FormatWarning, stacklevel=stacklevel())
-            return output, ''
+        module, class_, ext = cls.__output__[fmt]
+        if ext is None:
+            warn(f'Unsupported output format: {fmt}; disabled file output feature',
+                 FormatWarning, stacklevel=stacklevel())
+        output = getattr(importlib.import_module(module), class_)  # type: Type[Dumper]
 
         try:
-            pathlib.Path(fout).mkdir(parents=True, exist_ok=True)
+            os.makedirs(fout, exist_ok=True)
         except FileExistsError as error:
-            if fmt is None:
-                warnings.warn(str(error), FileWarning, stacklevel=stacklevel())
+            if ext is None:
+                warn(error.strerror, FileWarning, stacklevel=stacklevel())
             else:
-                raise FileExists(str(error)) from None
+                raise FileExists(*error.args).with_traceback(error.__traceback__)
+
+        class DictDumper(output):  # type: ignore[valid-type,misc]
+            """Customised :class:`~dictdumper.dumper.Dumper` object."""
 
-        return output, fmt
+            object_hook = dumpkit_object_hook
+            default = dumpkit_default
+            _append_fallback = dumpkit_append_fallback
 
-    def dump(self, packet):
+        return DictDumper, ext
+
+    @abc.abstractmethod
+    def dump(self, packet: 'Packet') -> 'None':
         """Dump frame to output files.
 
-        Positional arguments:
-            * packet -- dict, a flow packet
-                |-- (str) protocol -- data link type from global header
-                |-- (int) index -- frame number
-                |-- (Info) frame -- extracted frame info
-                |-- (bool) syn -- TCP synchronise (SYN) flag
-                |-- (bool) fin -- TCP finish (FIN) flag
-                |-- (str) src -- source IP
-                |-- (int) srcport -- TCP source port
-                |-- (str) dst -- destination IP
-                |-- (int) dstport -- TCP destination port
-                |-- (numbers.Real) timestamp -- frame timestamp
+        Arguments:
+            packet: a flow packet (:term:`trace.tcp.packet`)
 
         """
-        # fetch flow label
-        output = self.trace(packet, _check=False, _output=True)
 
-        # dump files
-        output(packet['frame'], name=f"Frame {packet['index']}")
+    @overload
+    def trace(self, packet: 'Packet', *, output: 'Literal[True]' = ...) -> 'Dumper': ...
+    @overload
+    def trace(self, packet: 'Packet', *, output: 'Literal[False]' = ...) -> 'str': ...
 
-    def trace(self, packet, *, _check=True, _output=False):
+    @abc.abstractmethod
+    def trace(self, packet: 'Packet', *, output: 'bool' = False) -> 'Dumper | str':
         """Trace packets.
 
-        Positional arguments:
-            * packet -- dict, a flow packet
+        Arguments:
+            packet: a flow packet (:term:`trace.tcp.packet`)
+            output: flag if has formatted dumper
 
-        Keyword arguments:
-            * _check -- bool, flag if run validations
-            * _output -- bool, flag if has formatted dumper
-
-        """
-        self._newflg = True
-        if _check:
-            pkt_check(packet)
-        info = Info(packet)
-
-        BUFID = tuple(sorted([str(info.src), str(info.srcport), str(info.dst), str(info.dstport)]))
-                            # Buffer Identifier
-        SYN = info.syn      # Synchronise Flag (Establishment)
-        FIN = info.fin      # Finish Flag (Termination)
-
-        # # when SYN is set, reset buffer of this seesion
-        # if SYN and BUFID in self._buffer:
-        #     temp = self._buffer.pop(BUFID)
-        #     temp['fpout'] = (self._fproot, self._fdpext)
-        #     temp['index'] = tuple(temp['index'])
-        #     self._stream.append(Info(temp))
-
-        # initialise buffer with BUFID
-        if BUFID not in self._buffer:
-            label = f'{info.src}_{info.srcport}-{info.dst}_{info.dstport}-{info.timestamp}'
-            self._buffer[BUFID] = dict(
-                fpout = self._foutio(f'{self._fproot}/{label}.{self._fdpext}', protocol=info.protocol),
-                index = list(),
-                label = label,
-            )
+        Returns:
+            If ``output`` is :data:`True`, returns the initiated
+            :class:`~dictdumper.dumper.Dumper` object, which will dump data to
+            the output file named after the flow label; otherwise, returns the
+            flow label itself.
 
-        # trace frame record
-        self._buffer[BUFID]['index'].append(info.index)
-        fpout = self._buffer[BUFID]['fpout']
-        label = self._buffer[BUFID]['label']
-
-        # when FIN is set, submit buffer of this session
-        if FIN:
-            buf = self._buffer.pop(BUFID)
-            # fpout, label = buf['fpout'], buf['label']
-            if self._fdpext:    buf['fpout'] = f'{self._fproot}/{label}.{self._fdpext}'
-            else:               del buf['fpout']
-            buf['index'] = tuple(buf['index'])
-            self._stream.append(Info(buf))
-
-        # return label or output object
-        return fpout if _output else label
-
-    def submit(self):
-        """Submit traced TCP flows."""
-        self._newflg = False
-        ret = list()
-        for buf in self._buffer.values():
-            buf = copy.deepcopy(buf)
-            if self._fdpext:    buf['fpout'] = f"{self._fproot}/{buf['label']}.{self._fdpext}"
-            else:               del buf['fpout']
-            buf['index'] = tuple(buf['index'])
-            ret.append(Info(buf))
-        ret += self._stream
-        return tuple(ret)
+        """
+
+    @abc.abstractmethod
+    def submit(self) -> 'tuple[Index, ...]':
+        """Submit traced TCP flows.
+
+        Returns:
+            Traced TCP flow (:term:`trace.tcp.index`).
+
+        """
 
     ##########################################################################
     # Data models.
     ##########################################################################
 
-    # Not hashable
-    __hash__ = None
+    def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'TraceFlow':  # pylint: disable=unused-argument
+        self = super().__new__(cls)
 
-    def __init__(self, *, fout=None, format=None):
+        # NOTE: Assign this attribute after ``__new__`` to avoid shared memory
+        # reference between instances.
+        self.__cached__ = {}
+
+        return self
+
+    def __init__(self, fout: 'Optional[str]', format: 'Optional[str]',  # pylint: disable=redefined-builtin
+                 byteorder: 'Literal["little", "big"]' = sys.byteorder,
+                 nanosecond: bool = False) -> 'None':
         """Initialise instance.
 
-        Keyword arguments:
-            * fout -- str, output path
-            * format -- str, output format
+        Arguments:
+            fout: output path
+            format: output format
+            byteorder: output file byte order
+            nanosecond: output nanosecond-resolution file flag
 
         """
-        self._newflg = False    # new packet flag
-        self._fproot = fout     # output root path
-        self._buffer = dict()   # buffer field
-        self._stream = list()   # stream index
-        self._foutio, self._fdpext \
-                    = self.make_fout(fout, format)
-                                # dump I/O object
+        if fout is None:
+            fout = './tmp'
+        if format is None:
+            format = 'pcap'
+
+        #: str: Output root path.
+        self._fproot = fout
+
+        #: dict[BufferID, Buffer]: Buffer field (:term:`trace.tcp.buffer`).
+        self._buffer = {}  # type: dict[BufferID, Buffer]
+        #: list[Index]: Stream index (:term:`trace.tcp.index`).
+        self._stream = []  # type: list[Index]
+
+        #: Literal['little', 'big']: Output file byte order.
+        self._endian = byteorder
+        #: bool: Output nanosecond-resolution file flag.
+        self._nnsecd = nanosecond
+
+        # dump I/O object
+        fio, ext = self.make_fout(fout, format)
+        #: Type[Dumper]: Dumper class.
+        self._foutio = fio
+        #: Optional[str]: Output file extension.
+        self._fdpext = ext
 
-    def __call__(self, packet):
+    def __call__(self, packet: 'Packet') -> 'None':
         """Dump frame to output files.
-        
-        Positional arguments:
-            * packet -- dict, a flow packet
+
+        Arguments:
+            packet: a flow packet (:term:`trace.tcp.packet`)
 
         """
-        self._newflg = True
+        # trace frame record
         self.dump(packet)
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/interface/__init__.py` & `pypcapkit-1.0.0b1/pcapkit/interface/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,190 +1,177 @@
 # -*- coding: utf-8 -*-
-"""user interface
+"""Core Interface
+====================
 
-`pcapkit.interface` defines several user-oriented
-interfaces, variables, and etc. These interfaces are
-designed to help and simplify the usage of `pcapkit`.
+.. module:: pcapkit.interface.core
+
+:mod:`pcapkit.interface.core` defines core user-oriented
+interfaces, variables, and etc., which wraps around the
+foundation classes from :mod:`pcapkit.foundation`.
 
 """
-import io
 import sys
+from typing import TYPE_CHECKING
 
-from pcapkit.foundation.analysis import analyse as analyse2
 from pcapkit.foundation.extraction import Extractor
-from pcapkit.foundation.traceflow import TraceFlow
+from pcapkit.foundation.reassembly.ipv4 import IPv4 as IPv4_Reassembly
+from pcapkit.foundation.reassembly.ipv6 import IPv6 as IPv6_Reassembly
+from pcapkit.foundation.reassembly.tcp import TCP as TCP_Reassembly
+from pcapkit.foundation.traceflow.tcp import TCP as TCP_TraceFlow
 from pcapkit.protocols.protocol import Protocol
-from pcapkit.reassembly.ipv4 import IPv4_Reassembly
-from pcapkit.reassembly.ipv6 import IPv6_Reassembly
-from pcapkit.reassembly.tcp import TCP_Reassembly
 from pcapkit.utilities.exceptions import FormatError
-from pcapkit.utilities.validations import bool_check, int_check, io_check, str_check
 
+if TYPE_CHECKING:
+    from typing import Any, Callable, Optional, Type, Union
+
+    from typing_extensions import Literal
+
+    from pcapkit.foundation.reassembly.reassembly import Reassembly
+    from pcapkit.foundation.traceflow.traceflow import TraceFlow
+    from pcapkit.protocols.misc.pcap.frame import Frame
+
+    Formats = Literal['pcap', 'json', 'tree', 'plist']
+    Engines = Literal['default', 'pcapkit', 'dpkt', 'scapy', 'pyshark']
+    Layers = Literal['link', 'internet', 'transport', 'application', 'none']
+
+    Protocols = Union[str, Protocol, Type[Protocol]]
+    VerboseHandler = Callable[['Extractor', Frame], Any]
 
 __all__ = [
-    'extract', 'analyse', 'reassemble', 'trace',            # interface functions
+    'extract', 'reassemble', 'trace',                       # interface functions
     'TREE', 'JSON', 'PLIST', 'PCAP',                        # format macros
     'LINK', 'INET', 'TRANS', 'APP', 'RAW',                  # layer macros
-    'DPKT', 'Scapy', 'PyShark', 'MPSearver', 'MPPipeline', 'PCAPKit',
-                                                            # engine macros
+    'DPKT', 'Scapy', 'PyShark', 'PCAPKit',                  # engine macros
 ]
 
-
 # output file formats
-TREE  = 'tree'
-JSON  = 'json'
+TREE = 'tree'
+JSON = 'json'
 PLIST = 'plist'
-PCAP  = 'pcap'
-
+PCAP = 'pcap'
 
 # layer thresholds
-RAW = 'None'
-LINK = 'Link'
-INET = 'Internet'
-TRANS = 'Transport'
-APP = 'Application'
-
+RAW = 'none'
+LINK = 'link'
+INET = 'internet'
+TRANS = 'transport'
+APP = 'application'
 
 # extraction engines
 DPKT = 'dpkt'
 Scapy = 'scapy'
 PCAPKit = 'default'
 PyShark = 'pyshark'
-MPSearver = 'server'
-MPPipeline = 'pipeline'
 
 
-def extract(*, fin=None, fout=None, format=None,                            # basic settings
-                auto=True, extension=True, store=True,                      # internal settings
-                files=False, nofile=False, verbose=False,                   # output settings
-                engine=None, layer=None, protocol=None,                     # extraction settings
-                ip=False, ipv4=False, ipv6=False, tcp=False, strict=True,   # reassembly settings
-                trace=False, trace_fout=None, trace_format=None):           # trace settings
+def extract(fin: 'Optional[str]' = None, fout: 'Optional[str]' = None, format: 'Optional[Formats]' = None,                 # basic settings # pylint: disable=redefined-builtin
+            auto: 'bool' = True, extension: 'bool' = True, store: 'bool' = True,                                           # internal settings # pylint: disable=line-too-long
+            files: 'bool' = False, nofile: 'bool' = False, verbose: 'bool | VerboseHandler' = False,                       # output settings # pylint: disable=line-too-long
+            engine: 'Optional[Engines]' = None, layer: 'Optional[Layers] | Type[Protocol]' = None,                         # extraction settings # pylint: disable=line-too-long
+            protocol: 'Optional[Protocols]' = None,                                                                        # extraction settings # pylint: disable=line-too-long
+            reassembly: 'bool' = False, strict: 'bool' = True,                                                             # reassembly settings # pylint: disable=line-too-long
+            trace: 'bool' = False, trace_fout: 'Optional[str]' = None, trace_format: 'Optional[Formats]' = None,           # trace settings # pylint: disable=line-too-long
+            trace_byteorder: 'Literal["big", "little"]' = sys.byteorder, trace_nanosecond: 'bool' = False,                 # trace settings # pylint: disable=line-too-long
+            ip: 'bool' = False, ipv4: 'bool' = False, ipv6: 'bool' = False, tcp: 'bool' = False) -> 'Extractor':
     """Extract a PCAP file.
 
-    Keyword arguments:
-        * fin  -- str, file name to be read; if file not exist, raise an error
-        * fout -- str, file name to be written
-        * format  -- str, file format of output
-                        <keyword> 'plist' / 'json' / 'tree' / 'html'
-
-        * auto -- bool, if automatically run till EOF (default is True)
-                        <keyword> True / False
-        * extension -- bool, if check and append axtensions to output file (default is True)
-                        <keyword> True / False
-        * store -- bool, if store extracted packet info (default is True)
-                        <keyword> True / False
-
-        * files -- bool, if split each frame into different files (default is False)
-                        <keyword> True / False
-        * nofile -- bool, if no output file is to be dumped (default is False)
-                        <keyword> True / False
-        * verbose -- bool, if print verbose output information (default is False)
-                        <keyword> True / False
-
-        * engine -- str, extraction engine to be used
-                        <keyword> 'default | pcapkit'
-        * layer -- str, extract til which layer
-                        <keyword> 'Link' / 'Internet' / 'Transport' / 'Application'
-        * protocol -- str, extract til which protocol
-                        <keyword> available protocol name
-
-        * ip -- bool, if record data for IPv4 & IPv6 reassembly (default is False)
-                        <keyword> True / False
-        * ipv4 -- bool, if perform IPv4 reassembly (default is False)
-                        <keyword> True / False
-        * ipv6 -- bool, if perform IPv6 reassembly (default is False)
-                        <keyword> True / False
-        * tcp -- bool, if perform TCP reassembly (default is False)
-                        <keyword> True / False
-        * strict -- bool, if set strict flag for reassembly (default is True)
-                        <keyword> True / False
-
-        * trace -- bool, if trace TCP traffic flows (default is False)
-                        <keyword> True / False
-        * trace_fout -- str, path name for flow tracer if necessary
-        * trace_format -- str, output file format of flow tracer
-                        <keyword> 'plist' / 'json' / 'tree' / 'html' / 'pcap'
+    Arguments:
+        fin: file name to be read; if file not exist, raise :exc:`FileNotFound`
+        fout: file name to be written
+        format: file format of output
+
+        auto: if automatically run till EOF
+        extension: if check and append extensions to output file
+        store: if store extracted packet info
+
+        files: if split each frame into different files
+        nofile: if no output file is to be dumped
+        verbose: a :obj:`bool` value or a function takes the :class:`Extract`
+            instance and current parsed frame (depends on engine selected) as
+            parameters to print verbose output information
+
+        engine: extraction engine to be used
+        layer: extract til which layer
+        protocol: extract til which protocol
+
+        reassembly: if perform reassembly
+        strict: if set strict flag for reassembly
+
+        trace: if trace TCP traffic flows
+        trace_fout: path name for flow tracer if necessary
+        trace_format: output file format of flow tracer
+        trace_byteorder: output file byte order
+        trace_nanosecond: output nanosecond-resolution file flag
+
+        ip: if record data for IPv4 & IPv6 reassembly
+        ipv4: if perform IPv4 reassembly
+        ipv6: if perform IPv6 reassembly
+        tcp: if perform TCP reassembly and/or flow tracing
 
     Returns:
-        * Extractor -- an Extractor object form `pcapkit.extractor`
+        An :class:`~pcapkit.foundation.extraction.Extractor` object.
 
     """
     if isinstance(layer, type) and issubclass(layer, Protocol):
-        layer = layer.__layer__
-    if isinstance(protocol, type) and issubclass(protocol, Protocol):
-        protocol = protocol.__index__()
-
-    str_check(fin or '', fout or '', format or '',
-                trace_fout or '', trace_format or '',
-                engine or '', layer or '', *(protocol or ''))
-    bool_check(files, nofile, verbose, auto, extension, store, 
-                ip, ipv4, ipv6, tcp, strict, trace)
+        layer = (layer.__layer__ or 'none').lower()  # type: ignore[assignment]
 
     return Extractor(fin=fin, fout=fout, format=format,
-                        store=store, files=files, nofile=nofile,
-                        auto=auto, verbose=verbose, extension=extension,
-                        engine=engine, layer=layer, protocol=protocol,
-                        ip=ip, ipv4=ipv4, ipv6=ipv6, tcp=tcp, strict=strict,
-                        trace=trace, trace_fout=trace_fout, trace_format=trace_format)
-
-
-def analyse(*, file, length=None):
-    """Analyse application layer packets.
-
-    Keyword arguments:
-        * file -- bytes or file-like object, packet to be analysed
-        * length -- int, length of the analysing packet
-
-    Returns:
-        * Analysis -- an Analysis object from `pcapkit.analyser`
-
-    """
-    if isinstance(file, bytes):
-        file = io.BytesIO(file)
-
-    io_check(file)
-    int_check(length or sys.maxsize)
-
-    return analyse2(file, length)
+                     store=store, files=files, nofile=nofile,
+                     auto=auto, verbose=verbose, extension=extension,
+                     engine=engine, layer=layer, protocol=protocol,  # type: ignore[arg-type]
+                     ip=ip, ipv4=ipv4, ipv6=ipv6, tcp=tcp, strict=strict, reassembly=reassembly,
+                     trace=trace, trace_fout=trace_fout, trace_format=trace_format,
+                     trace_byteorder=trace_byteorder, trace_nanosecond=trace_nanosecond)
 
 
-def reassemble(*, protocol, strict=False):
+def reassemble(protocol: 'str | Type[Protocol]', strict: 'bool' = False) -> 'Reassembly':
     """Reassemble fragmented datagrams.
 
-    Keyword arguments:
-        * protocol -- str, protocol to be reassembled
-        * strict -- bool, if return all datagrams (including those not implemented) when submit (default is False)
-                        <keyword> True / False
+    Arguments:
+        protocol: protocol to be reassembled
+        strict: if return all datagrams (including those not implemented) when submit
 
     Returns:
-        * [if protocol is IPv4] IPv4_Reassembly -- a Reassembly object from `pcapkit.reassembly`
-        * [if protocol is IPv6] IPv6_Reassembly -- a Reassembly object from `pcapkit.reassembly`
-        * [if protocol is TCP] TCP_Reassembly -- a Reassembly object from `pcapkit.reassembly`
+        A :class:`~pcapkit.foundation.reassembly.reassembly.Reassembly` object of corresponding protocol.
+
+    Raises:
+        FormatError: If ``protocol`` is **NOT** any of IPv4, IPv6 or TCP.
 
     """
     if isinstance(protocol, type) and issubclass(protocol, Protocol):
-        protocol = protocol.__index__()
-
-    str_check(protocol)
-    bool_check(strict)
+        protocol = protocol.id()[0]
 
     if protocol == 'IPv4':
         return IPv4_Reassembly(strict=strict)
-    elif protocol == 'IPv6':
+    if protocol == 'IPv6':
         return IPv6_Reassembly(strict=strict)
-    elif protocol == 'TCP':
+    if protocol == 'TCP':
         return TCP_Reassembly(strict=strict)
-    else:
-        raise FormatError(f'Unsupported reassembly protocol: {protocol}')
+    raise FormatError(f'Unsupported reassembly protocol: {protocol}')
+
 
+def trace(protocol: 'str | Type[Protocol]', fout: 'Optional[str]',
+          format: 'Optional[str]',  # pylint: disable=redefined-builtin
+          byteorder: 'Literal["little", "big"]' = sys.byteorder,
+          nanosecond: bool = False) -> 'TraceFlow':
+    """Trace flows.
+
+    Arguments:
+        protocol: protocol to be reassembled
+        fout: output path
+        format: output format
+        byteorder: output file byte order
+        nanosecond: output nanosecond-resolution file flag
 
-def trace(*, fout=None, format=None):
-    """Trace TCP flows.
+    Returns:
+        A :class:`~pcapkit.foundation.traceflow.traceflow.TraceFlow` object.
 
-    Keyword arguments:
-        * fout -- str, output path
-        * format -- str, output format
+    Raises:
+        FormatError: If ``protocol`` is **NOT** TCP.
 
     """
-    str_check(fout or '', format or '')
-    return TraceFlow(fout=fout, format=format)
+    if isinstance(protocol, type) and issubclass(protocol, Protocol):
+        protocol = protocol.id()[0]
+
+    if protocol == 'TCP':
+        return TCP_TraceFlow(fout=fout, format=format, byteorder=byteorder, nanosecond=nanosecond)
+    raise FormatError(f'Unsupported flow tracing protocol: {protocol}')
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/protocols/application/__init__.py` & `pypcapkit-1.0.0b1/pcapkit/protocols/application/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # -*- coding: utf-8 -*-
-"""application layer protocols
+# pylint: disable=unused-import,fixme
+"""Application Layer Protocols
+=================================
 
-`pcapkit.protocols.application` is collection of all
-protocols in application layer, with detailed
-implementation and methods.
+.. module:: pcapkit.protocols.application
+
+:mod:`pcapkit.protocols.application` is collection of all protocols in
+application layer, with detailed implementation and methods.
 
 """
-# TODO: Implements BGP, DHCP, DNS, FTP, IMAP, IDAP, MQTT, NNTP, NTP, ONC:RPC, POP, RIP, RTP, SIP, SMTP, SNMP, SSH, SSL, TELNET, TLS, XMPP.
+# TODO: Implements BGP, DHCP, DHCPv6, DNS, IMAP, LDAP, MQTT,
+#       NNTP, NTP, ONC:RPC, POP, RIP, RTP, SIP, SMTP, SNMP,
+#       SSH, TELNET, TLS/SSL, XMPP.
 
 # Base Class for Internet Layer
 from pcapkit.protocols.application.application import Application
 
 # Utility Classes for Protocols
-from pcapkit.protocols.application.httpv1 import HTTPv1
-from pcapkit.protocols.application.httpv2 import HTTPv2
+from pcapkit.protocols.application.ftp import FTP, FTP_DATA
+from pcapkit.protocols.application.httpv1 import HTTP as HTTPv1
+from pcapkit.protocols.application.httpv2 import HTTP as HTTPv2
 
 # Deprecated / Base Classes
 from pcapkit.protocols.application.http import HTTP
 
-
-__all__ = ['HTTPv1', 'HTTPv2']
+__all__ = [
+    'FTP', 'FTP_DATA',
+    'HTTP', 'HTTPv1', 'HTTPv2',
+]
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/protocols/application/httpv1.py` & `pypcapkit-1.0.0b1/pcapkit/protocols/application/ftp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,190 +1,206 @@
-"""hypertext transfer protocol (HTTP/1.*)
+# -*- coding: utf-8 -*-
+"""file transfer protocol
 
-`pcapkit.protocols.application.httpv1` contains `HTTPv1`
-only, which implements extractor for Hypertext Transfer
-Protocol (HTTP/1.*), whose structure is described as
-below.
-
-METHOD URL HTTP/VERSION\r\n :==: REQUEST LINE
-<key> : <value>\r\n         :==: REQUEST HEADER
-............  (Elipsis)     :==: REQUEST HEADER
-\r\n                        :==: REQUEST SEPERATOR
-<body>                      :==: REQUEST BODY (optional)
-
-HTTP/VERSION CODE DESP \r\n :==: RESPONSE LINE
-<key> : <value>\r\n         :==: RESPONSE HEADER
-............  (Elipsis)     :==: RESPONSE HEADER
-\r\n                        :==: RESPONSE SEPERATOR
-<body>                      :==: RESPONSE BODY (optional)
+.. module:: pcapkit.protocols.application.ftp
+
+:mod:`pcapkit.protocols.application.ftp` contains
+:class:`~pcapkit.protocols.application.ftp.FTP` only,
+which implements extractor for File Transfer Protocol
+(FTP) [*]_.
+
+.. [*] https://en.wikipedia.org/wiki/File_Transfer_Protocol
 
 """
 import re
+from typing import TYPE_CHECKING
 
-from pcapkit.corekit.infoclass import Info
-from pcapkit.protocols.application.http import HTTP
-from pcapkit.utilities.exceptions import ProtocolError
-
+from pcapkit.const.ftp.command import Command as Enum_Command
+from pcapkit.const.ftp.return_code import ReturnCode as Enum_ReturnCode
+from pcapkit.protocols.application.application import Application
+from pcapkit.protocols.data.application.ftp import FTP as Data_FTP
+from pcapkit.protocols.data.application.ftp import Request as Data_Request
+from pcapkit.protocols.data.application.ftp import Response as Data_Response
+from pcapkit.protocols.misc.raw import Raw
+from pcapkit.protocols.schema.application.ftp import FTP as Schema_FTP
+from pcapkit.utilities.compat import StrEnum
+from pcapkit.utilities.exceptions import ProtocolError, UnsupportedCall
 
-__all__ = ['HTTPv1']
+if TYPE_CHECKING:
+    from typing import Any, NoReturn, Optional
 
+    from typing_extensions import Literal
 
-# utility regular expressions
-_RE_METHOD = re.compile(rb'GET|HEAD|POST|PUT|DELETE|CONNECT|OPTIONS|TRACE')
-_RE_VERSION = re.compile(rb'HTTP/(?P<version>\d\.\d)')
-_RE_STATUS = re.compile(rb'\d{3}')
+__all__ = ['FTP', 'FTP_DATA']
 
+# regex for FTP
+FTP_REQUEST = re.compile(rb'^(?P<cmmd>[A-Z]{3,4})( +(?P<args>.*))?\r\n$', re.I)
+FTP_RESPONSE = re.compile(rb'^(?P<code>[0-9]{3})(?P<more>\-)?( +(?P<args>.*))?\r\n$', re.I)
 
-class HTTPv1(HTTP):
-    """This class implements Hypertext Transfer Protocol (HTTP/1.*).
 
-    Properties:
-        * name -- str, name of corresponding procotol
-        * info -- Info, info dict of current instance
-        * alias -- str, acronym of corresponding procotol
-        * layer -- str, `Application`
-        * protocol -- str, name of next layer protocol
-        * protochain -- ProtoChain, protocol chain of current instance
+class Type(StrEnum):
+    """FTP packet type."""
 
-    Methods:
-        * read_http -- read Hypertext Transfer Protocol (HTTP/1.*)
+    #: Request packet.
+    REQUEST = 'request'
+    #: Response packet.
+    RESPONSE = 'response'
 
-    Attributes:
-        * _file -- BytesIO, bytes to be extracted
-        * _info -- Info, info dict of current instance
-        * _protos -- ProtoChain, protocol chain of current instance
 
-    Utilities:
-        * _read_protos -- read next layer protocol type
-        * _read_fileng -- read file buffer
-        * _read_unpack -- read bytes and unpack to integers
-        * _read_binary -- read bytes and convert into binaries
-        * _make_protochain -- make ProtoChain instance for corresponding protocol
-        * _read_http_header -- read HTTP/1.* header
-        * _read_http_body -- read HTTP/1.* body
+class FTP(Application[Data_FTP, Schema_FTP],
+          data=Data_FTP, schema=Schema_FTP):
+    """This class implements File Transfer Protocol."""
 
-    """
     ##########################################################################
     # Properties.
     ##########################################################################
 
     @property
-    def alias(self):
-        """Acronym of current protocol."""
-        return f'HTTP/{self._info.header[self._info.receipt].version}'
+    def name(self) -> 'Literal["File Transfer Protocol"]':
+        """Name of current protocol."""
+        return 'File Transfer Protocol'
+
+    @property
+    def length(self) -> 'NoReturn':
+        """Header length of current protocol.
+
+        Raises:
+            UnsupportedCall: This protocol doesn't support :attr:`length`.
+
+        """
+        raise UnsupportedCall(f"'{self.__class__.__name__}' object has no attribute 'length'")
 
     ##########################################################################
     # Methods.
     ##########################################################################
 
-    def read_http(self, length):
-        """Read Hypertext Transfer Protocol (HTTP/1.*).
+    def read(self, length: 'Optional[int]' = None, **kwargs: 'Any') -> 'Data_FTP':  # pylint: disable=unused-argument
+        """Read File Transfer Protocol (FTP).
+
+        Args:
+            length: Length of packet data.
+            **kwargs: Arbitrary keyword arguments.
 
-        Structure of HTTP/1.* packet [RFC 7230]:
-            HTTP-message    :==:    start-line
-                                    *( header-field CRLF )
-                                    CRLF
-                                    [ message-body ]
+        Returns:
+            Parsed packet data.
+
+        Raises:
+            ProtocolError: If the packet is malformed.
 
         """
         if length is None:
-            length =  len(self)
+            length = len(self)
+        schema = self.__header__
 
-        packet = self._file.read(length)
-        try:
-            header, body = packet.split(b'\r\n\r\n', 1)
-        except ValueError:
-            raise ProtocolError('HTTP: invalid format', quiet=True)
-
-        header_unpacked, http_receipt = self._read_http_header(header)
-        body_unpacked = self._read_http_body(body) or None
-
-        http = dict(
-            receipt = http_receipt,
-            header = header_unpacked,
-            body = body_unpacked,
-            raw = dict(
-                header = header,
-                body = body,
-                packet = self._read_packet(length),
-            ),
-        )
+        data = schema.data
+        if (match := FTP_REQUEST.match(data)) is not None:
+            cmmd = match.group('cmmd').decode()
+            args = match.group('args')
+
+            cmmd_val = Enum_Command.get(cmmd)
+            args_val = self.decode(args)
+
+            ftp = Data_Request(
+                type=Type.REQUEST,
+                cmmd=cmmd_val,
+                args=args_val,
+            )  # type: Data_FTP
+        elif (match := FTP_RESPONSE.match(data)) is not None:
+            code = int(match.group('code'))
+            more = bool(match.group('more'))
+            args = match.group('args')
+
+            code_val = Enum_ReturnCode.get(code)
+            args_val = self.decode(args)
+
+            ftp = Data_Response(
+                type=Type.RESPONSE,
+                code=code_val,
+                more=more,
+                args=args_val,
+            )
+        else:
+            raise ProtocolError('FTP: invalid packet format')
+        return ftp
 
-        return http
+    def make(self,
+             cmmd: 'Optional[Enum_Command | str | bytes]' = None,
+             code: 'Optional[Enum_ReturnCode | int | str | bytes]' = None,
+             args: 'Optional[str | bytes]' = None,
+             more: 'bool' = False,
+             **kwargs: 'Any') -> 'Schema_FTP':
+        """Make (construct) packet data.
+
+        Args:
+            cmmd: FTP command.
+            code: FTP status code.
+            args: Optional FTP command arguments and/or status messages.
+            more: More status messages to follow for response packets.
+            **kwargs: Arbitrary keyword arguments.
 
-    ##########################################################################
-    # Data models.
-    ##########################################################################
+        Returns:
+            Constructed packet data.
 
-    def __length_hint__(self):
-        pass
+        """
+        if cmmd is not None and code is None:
+            if isinstance(cmmd, bytes):
+                prefix = cmmd
+            elif isinstance(cmmd, str):
+                prefix = cmmd.encode()
+            else:
+                prefix = cmmd.value
+
+            mf = b''
+        elif cmmd is None and code is not None:
+            code_val = int(code)
+            prefix = str(code_val).encode()
 
-    @classmethod
-    def __index__(cls):
-        return cls.__name__
+            mf = b'-' if more else b''
+        else:
+            raise ProtocolError('FTP: invalid packet type')
+
+        if args is None:
+            suffix = b''
+        elif isinstance(args, bytes):
+            suffix = args
+        else:
+            suffix = args.encode()
+
+        return Schema_FTP(
+            data=b'%s%s %s' % (prefix, mf, suffix),
+        )
 
     ##########################################################################
     # Utilities.
     ##########################################################################
 
-    def _read_http_header(self, header):
-        """Read HTTP/1.* header.
+    @classmethod
+    def _make_data(cls, data: 'Data_FTP') -> 'dict[str, Any]':  # type: ignore[override]
+        """Create key-value pairs from ``data`` for protocol construction.
+
+        Args:
+            data: protocol data
 
-        Structure of HTTP/1.* header [RFC 7230]:
-            start-line      :==:    request-line / status-line
-            request-line    :==:    method SP request-target SP HTTP-version CRLF
-            status-line     :==:    HTTP-version SP status-code SP reason-phrase CRLF
-            header-field    :==:    field-name ":" OWS field-value OWS
+        Returns:
+            Key-value pairs for protocol construction.
 
         """
-        try:
-            startline, headerfield = header.split(b'\r\n', 1)
-            para1, para2, para3 = re.split(rb'\s+', startline, 2)
-            fields = headerfield.split(b'\r\n')
-            lists = ( re.split(rb'\s*:\s*', field, 1) for field in fields )
-        except ValueError:
-            raise ProtocolError('HTTP: invalid format', quiet=True)
-
-        match1 = re.match(_RE_METHOD, para1)
-        match2 = re.match(_RE_VERSION, para3)
-        match3 = re.match(_RE_VERSION, para1)
-        match4 = re.match(_RE_STATUS, para2)
-        if match1 and match2:
-            receipt = 'request'
-            header = dict(
-                request = dict(
-                    method = self.decode(para1),
-                    target = self.decode(para2),
-                    version = self.decode(match2.group('version')),
-                ),
-            )
-        elif match3 and match4:
-            receipt = 'response'
-            header = dict(
-                response = dict(
-                    version = self.decode(match3.group('version')),
-                    status = int(para2),
-                    phrase = self.decode(para3),
-                ),
-            )
-        else:
-            raise ProtocolError('HTTP: invalid format', quiet=True)
+        return {
+            'cmmd': getattr(data, 'cmmd', None),
+            'code': getattr(data, 'code', None),
+            'args': getattr(data, 'args', None),
+            'more': getattr(data, 'more', False),
+        }
+
+
+class FTP_DATA(Raw):
+    """This class implements FTP data channel transmission."""
+
+    ##########################################################################
+    # Properties.
+    ##########################################################################
 
-        try:
-            for item in lists:
-                key = self.decode(item[0].strip()).replace(receipt, f'{receipt}_field')
-                value = self.decode(item[1].strip())
-                if key in header:
-                    if isinstance(header[key], tuple):
-                        header[key] += (value,)
-                    else:
-                        header[key] = (header[key], value)
-                else:
-                    header[key] = value
-        except IndexError:
-            raise ProtocolError('HTTP: invalid format', quiet=True)
-
-        return header, receipt
-
-    def _read_http_body(self, body):
-        """Read HTTP/1.* body."""
-        return self.decode(body)
+    # name of current protocol
+    @property
+    def name(self) -> 'Literal["FTP_DATA"]':  # type: ignore[override]
+        """Name of current protocol."""
+        return 'FTP_DATA'
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/protocols/internet/__init__.py` & `pypcapkit-1.0.0b1/pcapkit/protocols/internet/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # -*- coding: utf-8 -*-
-"""internet layer protocols
+# pylint: disable=unused-import,fixme
+"""Internet Layer Protocols
+==============================
 
-`pcapkit.protocols.internet` is collection of all protocols
-in internet layer, with detailed implementation and
-methods.
+.. module:: pcapkit.protocols.internet
+
+:mod:`pcapkit.protocols.internet` is collection of all protocols
+in internet layer, with detailed implementation and methods.
 
 """
 # TODO: Implements ECN, ESP, ICMP, ICMPv6, IGMP, Shim6.
 
 # Base Class for Internet Layer
 from pcapkit.protocols.internet.internet import Internet
 
@@ -22,20 +25,19 @@
 from pcapkit.protocols.internet.hopopt import HOPOPT
 from pcapkit.protocols.internet.ipv6_frag import IPv6_Frag
 from pcapkit.protocols.internet.ipv6_opts import IPv6_Opts
 from pcapkit.protocols.internet.ipv6_route import IPv6_Route
 from pcapkit.protocols.internet.mh import MH
 
 # Ethertype IEEE 802 Numbers
-from pcapkit.protocols.internet.internet import ETHERTYPE
+from pcapkit.const.reg.ethertype import EtherType as ETHERTYPE
 
 # Deprecated / Base Classes
 from pcapkit.protocols.internet.ip import IP
 from pcapkit.protocols.internet.ipsec import IPsec
 
-
 __all__ = [
     'ETHERTYPE',                                        # Protocol Numbers
     'AH', 'IP', 'IPsec', 'IPv4', 'IPv6', 'IPX',         # Internet Layer
     'HIP', 'HOPOPT', 'IPv6_Frag',
     'IPv6_Opts', 'IPv6_Route', 'MH',                    # IPv6 Extension Header
 ]
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/protocols/internet/hip.py` & `pypcapkit-1.0.0b1/pcapkit/protocols/link/l2tp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,212 +1,267 @@
 # -*- coding: utf-8 -*-
-"""host identity protocol
+"""L2TP - Layer Two Tunnelling Protocol
+==========================================
 
-`pcapkit.protocols.internet.hip` contains `HIP`
-only, which implements extractor for Host Identity
-Protocol (HIP), whose structure is described as below.
-
- 0                   1                   2                   3
- 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-| Next Header   | Header Length |0| Packet Type |Version| RES.|1|
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|          Checksum             |           Controls            |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|                Sender's Host Identity Tag (HIT)               |
-|                                                               |
-|                                                               |
-|                                                               |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|               Receiver's Host Identity Tag (HIT)              |
-|                                                               |
-|                                                               |
-|                                                               |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|                                                               |
-/                        HIP Parameters                         /
-/                                                               /
-|                                                               |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+.. module:: pcapkit.protocols.link.l2tp
+
+:mod:`pcapkit.protocols.link.l2tp` contains
+:class:`~pcapkit.protocols.link.l2tp.L2TP` only,
+which implements extractor for Layer Two Tunnelling
+Protocol (L2TP) [*]_, whose structure is described
+as below:
+
+.. table::
+
+   ======= ===== ===================== ==========================================
+    Octets Bits  Name                  Description
+   ======= ===== ===================== ==========================================
+    0          0 ``l2tp.flags``        Flags and Version Info
+   ------- ----- --------------------- ------------------------------------------
+    0          0 ``l2tp.flags.type``   Type (control / data)
+   ------- ----- --------------------- ------------------------------------------
+    0          1 ``l2tp.flags.len``    Length
+   ------- ----- --------------------- ------------------------------------------
+    0          2                       Reserved (must be zero ``x00``)
+   ------- ----- --------------------- ------------------------------------------
+    0          4 ``l2tp.flags.seq``    Sequence
+   ------- ----- --------------------- ------------------------------------------
+    0          5                       Reserved (must be zero ``x00``)
+   ------- ----- --------------------- ------------------------------------------
+    0          6 ``l2tp.flags.offset`` Offset
+   ------- ----- --------------------- ------------------------------------------
+    0          7 ``l2tp.flags.prio``   Priority
+   ------- ----- --------------------- ------------------------------------------
+    1          8                       Reserved (must be zero ``x00``)
+   ------- ----- --------------------- ------------------------------------------
+    1         12 ``l2tp.ver``          Version (``2``)
+   ------- ----- --------------------- ------------------------------------------
+    2         16 ``l2tp.length``       Length (optional by ``len``)
+   ------- ----- --------------------- ------------------------------------------
+    4         32 ``l2tp.tunnelid``     Tunnel ID
+   ------- ----- --------------------- ------------------------------------------
+    6         48 ``l2tp.sessionid``    Session ID
+   ------- ----- --------------------- ------------------------------------------
+    8         64 ``l2tp.ns``           Sequence Number (optional by ``seq``)
+   ------- ----- --------------------- ------------------------------------------
+    10        80 ``l2tp.nr``           Next Sequence Number (optional by ``seq``)
+   ------- ----- --------------------- ------------------------------------------
+    12        96 ``l2tp.offset``       Offset Size (optional by ``offset``)
+   ======= ===== ===================== ==========================================
+
+.. [*] https://en.wikipedia.org/wiki/Layer_2_Tunneling_Protocol
 
 """
-# TODO: Implements extractor of all HIP parameters.
-from pcapkit.corekit.infoclass import Info
-from pcapkit.protocols.protocol import Protocol
-from pcapkit.utilities.exceptions import ProtocolError
-
-
-__all__ = ['HIP']
-
-
-# HIP Packet Types
-_HIP_TYPES = {
-    0 : 'Reserved',     # [RFC 7401]
-    1 : 'I1',           # [RFC 7401] the HIP Initiator Packet
-    2 : 'R1',           # [RFC 7401] the HIP Responder Packet
-    3 : 'I2',           # [RFC 7401] the Second HIP Initiator Packet
-    4 : 'R2',           # [RFC 7401] the Second HIP Responder Packet
-   16 : 'UPDATE',       # [RFC 7401] the HIP Update Packet
-   17 : 'NOTIFY',       # [RFC 7401] the HIP Notify Packet
-   18 : 'CLOSE',        # [RFC 7401] the HIP Association Closing Packet
-   19 : 'CLOSE_ACK',    # [RFC 7401] the HIP Closing Acknowledgment Packet
-   20 : 'HDRR',         # [RFC 6537] HIP Distributed Hash Table Resource Record
-   32 : 'HIP_DATA',     # [RFC 6078]
-}
-
-
-class HIP(Protocol):
-    """This class implements Host Identity Protocol.
-
-    Properties:
-        * name -- str, name of corresponding procotol
-        * info -- Info, info dict of current instance
-        * alias -- str, acronym of corresponding procotol
-        * layer -- str, `Internet`
-        * length -- int, header length of corresponding protocol
-        * protocol -- str, name of next layer protocol
-        * protochain -- ProtoChain, protocol chain of current instance
-
-    Methods:
-        * read_hip -- read Host Identity Protocol (HIP)
-
-    Attributes:
-        * _file -- BytesIO, bytes to be extracted
-        * _info -- Info, info dict of current instance
-        * _protos -- ProtoChain, protocol chain of current instance
-
-    Utilities:
-        * _read_protos -- read next layer protocol type
-        * _read_fileng -- read file buffer
-        * _read_unpack -- read bytes and unpack to integers
-        * _read_binary -- read bytes and convert into binaries
-        * _read_packet -- read raw packet data
-        * _decode_next_layer -- decode next layer protocol type
-        * _import_next_layer -- import next layer protocol extractor
+from typing import TYPE_CHECKING
+
+from pcapkit.const.l2tp.type import Type as Enum_Type
+from pcapkit.protocols.data.link.l2tp import L2TP as Data_L2TP
+from pcapkit.protocols.data.link.l2tp import Flags as Data_Flags
+from pcapkit.protocols.link.link import Link
+from pcapkit.protocols.schema.link.l2tp import L2TP as Schema_L2TP
+from pcapkit.utilities.exceptions import UnsupportedCall
+
+if TYPE_CHECKING:
+    from enum import IntEnum as StdlibEnum
+    from typing import Any, NoReturn, Optional, Type
+
+    from aenum import IntEnum as AenumEnum
+    from typing_extensions import Literal
+
+    from pcapkit.protocols.protocol import Protocol
+    from pcapkit.protocols.schema.schema import Schema
+
+__all__ = ['L2TP']
+
+
+class L2TP(Link[Data_L2TP, Schema_L2TP],
+           schema=Schema_L2TP, data=Data_L2TP):
+    """This class implements Layer Two Tunnelling Protocol."""
 
-    """
     ##########################################################################
     # Properties.
     ##########################################################################
 
     @property
-    def name(self):
+    def name(self) -> 'Literal["Layer 2 Tunnelling Protocol"]':
         """Name of current protocol."""
-        return 'Host Identity Protocol'
+        return 'Layer 2 Tunnelling Protocol'
 
     @property
-    def alias(self):
-        """Acronym of corresponding procotol."""
-        return f'HIPv{self._info.version}'
-
-    @property
-    def length(self):
+    def length(self) -> 'int':
         """Header length of current protocol."""
-        return self._info.length
-
-    @property
-    def payload(self):
-        """Payload of current instance."""
-        if self.extension:
-            raise UnsupportedCall(f"'{self.__class__.__name__}' object has no attribute 'payload'")
-        return self._next
+        return self._info.hdr_len
 
     @property
-    def protocol(self):
-        """Name of next layer protocol."""
-        return self._info.next
+    def type(self) -> 'Literal["control", "data"]':
+        """L2TP type."""
+        return self._info.flags.type
 
     ##########################################################################
     # Methods.
     ##########################################################################
 
-    def read_hip(self, length, extension):
-        """Read Host Identity Protocol.
+    def read(self, length: 'Optional[int]' = None, **kwargs: 'Any') -> 'Data_L2TP':  # pylint: disable=unused-argument
+        """Read Layer Two Tunnelling Protocol.
 
-        Structure of HIP header [RFC 7401]:
-             0                   1                   2                   3
-             0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            | Next Header   | Header Length |0| Packet Type |Version| RES.|1|
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            |          Checksum             |           Controls            |
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            |                Sender's Host Identity Tag (HIT)               |
-            |                                                               |
-            |                                                               |
-            |                                                               |
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            |               Receiver's Host Identity Tag (HIT)              |
-            |                                                               |
-            |                                                               |
-            |                                                               |
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            |                                                               |
-            /                        HIP Parameters                         /
-            /                                                               /
-            |                                                               |
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-
-            Octets      Bits        Name                    Discription
-              0           0     hip.next                Next Header
-              1           8     hip.length              Header Length
-              2          16     -                       Reserved (0)
-              2          17     hip.type                Packet Type
-              3          24     hip.version             Version
-              3          28     -                       Reserved
-              3          31     -                       Reserved (1)
-              4          32     hip.chksum              Checksum
-              6          48     hip.control             Controls
-              8          64     hip.shit                Sender's Host Identity Tag
-              24        192     hip.rhit                Receiver's Host Identity Tag
-              40        320     hip.parameters          HIP Parameters
+        Structure of L2TP header [:rfc:`2661`]:
+
+        .. code-block:: text
+
+            0                   1                   2                   3
+            0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+           |T|L|x|x|S|x|O|P|x|x|x|x|  Ver  |          Length (opt)         |
+           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+           |           Tunnel ID           |           Session ID          |
+           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+           |             Ns (opt)          |             Nr (opt)          |
+           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+           |      Offset Size (opt)        |    Offset pad... (opt)
+           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+
+        Args:
+            length: Length of packet data.
+            **kwargs: Arbitrary keyword arguments.
+
+        Returns:
+            Parsed packet data.
 
         """
-        if length is None:
-            length = len(self)
+        schema = self.__header__
+        _flag = schema.flags
 
-        _next = self._read_protos(1)
-        _hlen = self._read_unpack(1)
-        _type = self._read_binary(1)
-        if _type[0] != '0':
-            raise ProtocolError('HIP: invalid format')
-        _vers = self._read_binary(1)
-        if _vers[7] != '1':
-            raise ProtocolError('HIP: invalid format')
-        _csum = self._read_fileng(2)
-        _ctrl = self._read_binary(2)
-        _shit = self._read_unpack(16)
-        _rhit = self._read_unpack(16)
-        _para = self._read_fileng(_hlen - 38)
-
-        hip = dict(
-            next = _next,
-            length = _hlen + 1,
-            type = _HIP_TYPES.get(int(_type[1:], base=2), 'Unassigned'),
-            version = int(_vers[:4], base=2),
-            chksum = _csum,
-            control = dict(
-                anonymous = True if int(_ctrl[15], base=2) else False,
-            ),
-            shit = _shit,
-            rhit = _rhit,
-            parameters = _para,
+        flags = Data_Flags(
+            type=Enum_Type(_flag['type']),
+            len=bool(_flag['len']),
+            seq=bool(_flag['seq']),
+            offset=bool(_flag['offset']),
+            prio=bool(_flag['prio']),
         )
 
-        length -= hip['length']
-        hip['packet'] = self._read_packet(header=hip['length'], payload=length)
+        _size = schema.offset if flags.offset else 0
+        hdr_len = 6 + 2 * (flags.len + 2 * flags.seq + flags.offset) + _size
 
-        if extension:
-            self._protos = None
-            return hip
-        return self._decode_next_layer(hip, _next, length)
+        l2tp = Data_L2TP(
+            flags=flags,
+            version=_flag['version'],
+            length=schema.length if flags.len else None,
+            tunnelid=schema.tunnel_id,
+            sessionid=schema.session_id,
+            ns=schema.ns if flags.seq else None,
+            nr=schema.nr if flags.seq else None,
+            offset=_size if flags.offset else None,
+        )
+
+        l2tp.__update__([
+            ('hdr_len', hdr_len),
+        ])
+        if _size:
+            self._read_fileng(_size)
+            # l2tp['padding'] = self._read_fileng(_size)
+
+        length = schema.length if flags.len else (length or len(self))
+        return self._decode_next_layer(l2tp, length - hdr_len)
+
+    def make(self,
+             version: 'Literal[2]' = 2,
+             type: 'Enum_Type | StdlibEnum | AenumEnum | str | int' = Enum_Type.Data,
+             type_default: 'Optional[int]' = None,
+             type_namespace: 'Optional[dict[str, int] | dict[int, str] | Type[StdlibEnum] | Type[AenumEnum]]' = None,  # pylint: disable=line-too-long
+             type_reversed: 'bool' = False,
+             priority: 'bool' = False,
+             length: 'Optional[int]' = None,
+             tunnel_id: 'int' = 0,
+             session_id: 'int' = 0,
+             ns: 'Optional[int]' = None,
+             nr: 'Optional[int]' = None,
+             offset: 'Optional[int]' = None,
+             payload: 'bytes | Protocol | Schema' = b'',
+             **kwargs: 'Any') -> 'Schema_L2TP':  # pylint: disable=unused-argument
+        """Make (construct) packet data.
+
+        Args:
+            version: L2TP version.
+            type: L2TP type.
+            type_default: Default value of type.
+            type_namespace: Namespace of type.
+            type_reversed: Reversed namespace of type.
+            priority: Priority flag.
+            length: Length of packet data.
+            tunnel_id: Tunnel ID.
+            session_id: Session ID.
+            ns: Sequence number.
+            nr: Acknowledgement number.
+            offset: Offset size.
+            payload: Payload data.
+            **kwargs: Arbitrary keyword arguments.
+
+        Returns:
+            Constructed packet data.
+
+        """
+        type_ = self._make_index(type, type_default, namespace=type_namespace,  # type: ignore[call-overload]
+                                 reversed=type_reversed, pack=False)
+
+        return Schema_L2TP(
+            flags={
+                'type': type_,
+                'len': length is not None,
+                'seq': ns is not None and nr is not None,
+                'offset': offset is not None,
+                'prio': priority,
+                'version': version,
+            },
+            length=length,
+            tunnel_id=tunnel_id,
+            session_id=session_id,
+            ns=ns,
+            nr=nr,
+            offset=offset,
+            payload=payload,
+        )
 
     ##########################################################################
     # Data models.
     ##########################################################################
 
-    def __init__(self, _file, length=None, *, extension=False, **kwargs):
-        self._file = _file
-        self._info = Info(self.read_hip(length, extension))
+    def __length_hint__(self) -> 'Literal[16]':
+        """Return an estimated length for the object."""
+        return 16
+
+    @classmethod
+    def __index__(cls) -> 'NoReturn':  # pylint: disable=invalid-index-returned
+        """Numeral registry index of the protocol.
+
+        Raises:
+            UnsupportedCall: This protocol has no registry entry.
+
+        """
+        raise UnsupportedCall(f'{cls.__name__!r} object cannot be interpreted as an integer')
+
+    ##########################################################################
+    # Utilities.
+    ##########################################################################
+
+    @classmethod
+    def _make_data(cls, data: 'Data_L2TP') -> 'dict[str, Any]':  # type: ignore[override]
+        """Create key-value pairs from ``data`` for protocol construction.
+
+        Args:
+            data: protocol data
 
-    def __length_hint__(self):
-        return 40
+        Returns:
+            Key-value pairs for protocol construction.
+
+        """
+        return {
+            'type': data.flags.type,
+            'prio': data.flags.prio,
+            'version': data.version,
+            'length': data.length,
+            'tunnel_id': data.tunnelid,
+            'session_id': data.sessionid,
+            'ns': data.ns,
+            'nr': data.nr,
+            'offset': data.offset,
+            'payload': cls._make_payload(data),
+        }
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ipv6.py` & `pypcapkit-1.0.0b1/pcapkit/protocols/internet/ipv6.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,301 +1,361 @@
 # -*- coding: utf-8 -*-
-"""internet protocol version 6
+"""IPv6 - Internet Protocol version 6
+========================================
 
-`pcapkit.protocols.internet.ipv6` contains `IPv6` only,
-which implements extractor for Internet Protocol version 6
-(IPv6), whose structure is described as below.
-
- 0                   1                   2                   3
- 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|Version| Traffic Class |           Flow Label                  |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|         Payload Length        |  Next Header  |   Hop Limit   |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|                                                               |
-+                                                               +
-|                                                               |
-+                         Source Address                        +
-|                                                               |
-+                                                               +
-|                                                               |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|                                                               |
-+                                                               +
-|                                                               |
-+                      Destination Address                      +
-|                                                               |
-+                                                               +
-|                                                               |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+.. module:: pcapkit.protocols.internet.ipv6
+
+:mod:`pcapkit.protocols.internet.ipv6` contains
+:class:`~pcapkit.protocols.internet.ipv6.IPv6` only,
+which implements extractor for Internet Protocol
+version 6 (IPv6) [*]_, whose structure is described
+as below:
+
+======= ========= ===================== =======================================
+Octets      Bits        Name                    Description
+======= ========= ===================== =======================================
+  0           0   ``ip.version``              Version (``6``)
+  0           4   ``ip.class``                Traffic Class
+  1          12   ``ip.label``                Flow Label
+  4          32   ``ip.payload``              Payload Length (header excludes)
+  6          48   ``ip.next``                 Next Header
+  7          56   ``ip.limit``                Hop Limit
+  8          64   ``ip.src``                  Source Address
+  24        192   ``ip.dst``                  Destination Address
+======= ========= ===================== =======================================
+
+.. [*] https://en.wikipedia.org/wiki/IPv6_packet
 
 """
-# TODO: Implements IPv6 extension headers.
-import collections
 import ipaddress
+from typing import TYPE_CHECKING
 
-from pcapkit.corekit.infoclass import Info
+from pcapkit.const.ipv6.extension_header import ExtensionHeader as Enum_ExtensionHeader
+from pcapkit.const.reg.transtype import TransType as Enum_TransType
+from pcapkit.corekit.multidict import OrderedMultiDict
 from pcapkit.corekit.protochain import ProtoChain
+from pcapkit.protocols.data.internet.ipv6 import IPv6 as Data_IPv6
 from pcapkit.protocols.internet.ip import IP
+from pcapkit.protocols.schema.internet.ipv6 import IPv6 as Schema_IPv6
+
+if TYPE_CHECKING:
+    from enum import IntEnum as StdlibEnum
+    from ipaddress import IPv6Address
+    from typing import Any, Optional, Type
+
+    from aenum import IntEnum as AenumEnum
+    from typing_extensions import Literal
 
+    from pcapkit.protocols.protocol import Protocol
+    from pcapkit.protocols.schema.schema import Schema
 
 __all__ = ['IPv6']
 
 
-# IPv6 Extension Header Types
-EXT_HDR = (
-    'HOPOPT',       # IPv6 Hop-by-Hop Option
-    'IPv6-Route',   # Routing Header for IPv6
-    'IPv6-Frag',    # Fragment Header for IPv6
-    'ESP',          # Encapsulating Security Payload
-    'AH',           # Authentication Header
-    'IPv6-NoNxt',   # No Next Header for IPv6
-    'IPv6-Opts',    # Destination Options for IPv6 (before routing / upper-layer header)
-    'MH',           # Mobility Extension Header for IPv6 (currently without upper-layer header)
-    'HIP',          # Host Identity Protocol
-    'Shim6',        # Site Multihoming by IPv6 Intermediation
-)
-
-
-class IPv6(IP):
-    """This class implements Internet Protocol version 6.
-
-    Properties:
-        * name -- str, name of corresponding procotol
-        * info -- Info, info dict of current instance
-        * alias -- str, acronym of corresponding procotol
-        * layer -- str, `Internet`
-        * length -- int, header length of corresponding protocol
-        * protocol -- str, name of next layer protocol
-        * protochain -- ProtoChain, protocol chain of current instance
-        * src -- str, source IP address
-        * dst -- str, destination IP address
-
-    Methods:
-        * read_ipv6 -- read Internet Protocol version 6 (IPv6)
-
-    Attributes:
-        * _file -- BytesIO, bytes to be extracted
-        * _info -- Info, info dict of current instance
-        * _protos -- ProtoChain, protocol chain of current instance
-
-    Utilities:
-        * _read_protos -- read next layer protocol type
-        * _read_fileng -- read file buffer
-        * _read_unpack -- read bytes and unpack to integers
-        * _read_binary -- read bytes and convert into binaries
-        * _read_packet -- read raw packet data
-        * _decode_next_layer -- decode next layer protocol type
-        * _import_next_layer -- import next layer protocol extractor
-        * _read_ip_hextet -- read first four hextets of IPv6
-        * _read_ip_addr -- read IP address
+class IPv6(IP[Data_IPv6, Schema_IPv6],
+           schema=Schema_IPv6, data=Data_IPv6):
+    """This class implements Internet Protocol version 6."""
 
-    """
     ##########################################################################
     # Properties.
     ##########################################################################
 
     @property
-    def name(self):
-        """Name of corresponding procotol."""
+    def name(self) -> 'Literal["Internet Protocol version 6"]':
+        """Name of corresponding protocol."""
         return 'Internet Protocol version 6'
 
     @property
-    def length(self):
+    def length(self) -> 'Literal[40]':
         """Header length of corresponding protocol."""
-        return self._info.hdr_len
+        return 40
 
     @property
-    def protocol(self):
+    def protocol(self) -> 'Enum_TransType':
         """Name of next layer protocol."""
-        return self._info.next
+        return self._info.protocol
+
+    # source IP address
+    @property
+    def src(self) -> 'IPv6Address':
+        """Source IP address."""
+        return self._info.src
+
+    # destination IP address
+    @property
+    def dst(self) -> 'IPv6Address':
+        """Destination IP address."""
+        return self._info.dst
+
+    @property
+    def extension_headers(self) -> 'OrderedMultiDict[Enum_ExtensionHeader, Protocol]':
+        """IPv6 extension header records."""
+        return self._exthdr
 
     ##########################################################################
     # Methods.
     ##########################################################################
 
-    def read_ipv6(self, length):
+    def read(self, length: 'Optional[int]' = None, *,
+             packet: 'Optional[dict[str, Any]]' = None, **kwargs: 'Any') -> 'Data_IPv6':  # pylint: disable=unused-argument
         """Read Internet Protocol version 6 (IPv6).
 
-        Structure of IPv6 header [RFC 2460]:
+        Structure of IPv6 header [:rfc:`2460`]:
+
+        .. code-block:: text
+
+            0                   1                   2                   3
+            0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+           |Version| Traffic Class |           Flow Label                  |
+           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+           |         Payload Length        |  Next Header  |   Hop Limit   |
+           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+           |                                                               |
+           +                                                               +
+           |                                                               |
+           +                         Source Address                        +
+           |                                                               |
+           +                                                               +
+           |                                                               |
+           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+           |                                                               |
+           +                                                               +
+           |                                                               |
+           +                      Destination Address                      +
+           |                                                               |
+           +                                                               +
+           |                                                               |
+           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+
+        Args:
+            length: Length of packet data.
+            packet: Optional packet data.
+            **kwargs: Arbitrary keyword arguments.
 
-             0                   1                   2                   3
-             0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            |Version| Traffic Class |           Flow Label                  |
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            |         Payload Length        |  Next Header  |   Hop Limit   |
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            |                                                               |
-            +                                                               +
-            |                                                               |
-            +                         Source Address                        +
-            |                                                               |
-            +                                                               +
-            |                                                               |
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            |                                                               |
-            +                                                               +
-            |                                                               |
-            +                      Destination Address                      +
-            |                                                               |
-            +                                                               +
-            |                                                               |
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-
-            Octets      Bits        Name                    Discription
-              0           0     ip.version              Version (6)
-              0           4     ip.class                Traffic Class
-              1          12     ip.label                Flow Label
-              4          32     ip.payload              Payload Length (header excludes)
-              6          48     ip.next                 Next Header
-              7          56     ip.limit                Hop Limit
-              8          64     ip.src                  Source Address
-              24        192     ip.dst                  Destination Address
+        Returns:
+            Parsed packet data.
 
         """
         if length is None:
             length = len(self)
+        schema = self.__header__
+
+        ipv6 = Data_IPv6.from_dict({
+            'version': schema.hextet['version'],
+            'class': schema.hextet['class'],
+            'label': schema.hextet['label'],
+            'payload': schema.length,
+            'next': schema.next,
+            'limit': schema.limit,
+            'src': schema.src,
+            'dst': schema.dst,
+        })  # type: Data_IPv6
+
+        # update packet info
+        if packet is None:
+            packet = {}
+        packet.update({
+            'src': ipv6.src,
+            'dst': ipv6.dst,
+        })
+
+        return self._decode_next_layer(ipv6, schema.next, ipv6.payload, packet=packet)  # pylint: disable=no-member
+
+    def make(self,
+             traffic_class: 'int' = 0,
+             flow_label: 'int' = 0,
+             next: 'Enum_TransType | StdlibEnum | AenumEnum | str | int' = Enum_TransType.UDP,
+             next_default: 'Optional[int]' = None,
+             next_namespace: 'Optional[dict[str, int] | dict[int, str] | Type[StdlibEnum] | Type[AenumEnum]]' = None,  # pylint: disable=line-too-long
+             next_reversed: 'bool' = False,
+             hop_limit: 'int' = 64,  # reasonable default
+             src: 'IPv6Address | str | bytes | int' = '::1',
+             dst: 'IPv6Address | str | bytes | int' = '::',
+             payload: 'bytes | Protocol | Schema' = b'',
+             **kwargs: 'Any') -> 'Schema_IPv6':
+        """Make (construct) packet data.
+
+        Args:
+            traffic_class: Traffic class.
+            flow_label: Flow label.
+            next: Next header.
+            next_default: Default value of next header.
+            next_namespace: Namespace of next header.
+            next_reversed: Whether to reverse the namespace of next header.
+            hop_limit: Hop limit.
+            src: Source IP address.
+            dst: Destination IP address.
+            payload: Payload data.
+            **kwargs: Arbitrary keyword arguments.
+
+        Returns:
+            Constructed packet data.
 
-        _htet = self._read_ip_hextet()
-        _plen = self._read_unpack(2)
-        _next = self._read_protos(1)
-        _hlmt = self._read_unpack(1)
-        _srca = self._read_ip_addr()
-        _dsta = self._read_ip_addr()
-
-        ipv6 = dict(
-            version = _htet[0],
-            tclass = _htet[1],
-            label = _htet[2],
-            payload = _plen,
-            next = _next,
-            limit = _hlmt,
-            src = _srca,
-            dst = _dsta,
+        """
+        next_val = self._make_index(next, next_default, namespace=next_namespace,  # type: ignore[call-overload]
+                                    reversed=next_reversed, pack=False)
+
+        return Schema_IPv6(
+            hextet={
+                'version': 6,
+                'class': traffic_class,
+                'label': flow_label,
+            },
+            length=len(payload),
+            next=next_val,
+            limit=hop_limit,
+            src=src,
+            dst=dst,
+            payload=payload,
         )
 
-        hdr_len = 40
-        raw_len = ipv6['payload']
-        ipv6['packet'] = self._read_packet(header=hdr_len, payload=raw_len)
+    @classmethod
+    def id(cls) -> 'tuple[Literal["IPv6"]]':  # type: ignore[override]
+        """Index ID of the protocol.
 
-        return self._decode_next_layer(ipv6, _next, raw_len)
+        Returns:
+            Index ID of the protocol.
+
+        """
+        return ('IPv6',)
 
     ##########################################################################
     # Data models.
     ##########################################################################
 
-    def __init__(self, _file, length=None, **kwargs):
-        self._file = _file
-        self._info = Info(self.read_ipv6(length))
-
-    def __length_hint__(self):
+    def __length_hint__(self) -> 'Literal[40]':
+        """Return an estimated length for the object."""
         return 40
 
     @classmethod
-    def __index__(cls):
-        return cls.__name__
+    def __index__(cls) -> 'Enum_TransType':  # pylint: disable=invalid-index-returned
+        """Numeral registry index of the protocol.
+
+        Returns:
+            Numeral registry index of the protocol in `IANA`_.
+
+        .. _IANA: https://www.iana.org/assignments/protocol-numbers/protocol-numbers.xhtml
+
+        """
+        return Enum_TransType.IPv6  # type: ignore[return-value]
 
     ##########################################################################
     # Utilities.
     ##########################################################################
 
-    def _read_ip_hextet(self):
-        """Read first four hextets of IPv6."""
+    @classmethod
+    def _make_data(cls, data: 'Data_IPv6') -> 'dict[str, Any]':  # type: ignore[override]
+        """Create key-value pairs from ``data`` for protocol construction.
+
+        Args:
+            data: protocol data
+
+        Returns:
+            Key-value pairs for protocol construction.
+
+        """
+        return {
+            'traffic_class': data['class'],
+            'flow_label': data.label,
+            'next': data.next,
+            'hop_limit': data.limit,
+            'src': data.src,
+            'dst': data.dst,
+            'payload': cls._make_payload(data)
+        }
+
+    def _read_ip_hextet(self) -> 'tuple[int, int, int]':
+        """Read first four hextets of IPv6.
+
+        Returns:
+            Parsed hextets data, including version number, traffic class and
+            flow label.
+
+        """
         _htet = self._read_fileng(4).hex()
-        _vers = _htet[0]                    # version number (6)
+        _vers = int(_htet[0], base=16)      # version number (6)
         _tcls = int(_htet[0:2], base=16)    # traffic class
         _flow = int(_htet[2:], base=16)     # flow label
 
         return (_vers, _tcls, _flow)
 
-    def _read_ip_addr(self):
-        """Read IP address."""
-        # adlt = []       # list of IPv6 hexadecimal address
-        # ctr_ = collections.defaultdict(int)
-        #                 # counter for consecutive groups of zero value
-        # ptr_ = 0        # start pointer of consecutive groups of zero value
-        # last = False    # if last hextet/group is zero value
-        # ommt = False    # ommitted flag, since IPv6 address can ommit to `::` only once
-
-        # for _ in range(8):
-        #     hex_ = self._read_fileng(2).hex().lstrip('0')
-
-        #     if hex_:    # if hextet is not '', directly append
-        #         adlt.append(hex_)
-        #         last = False
-        #     else:       # if hextet is '', append '0'
-        #         adlt.append('0')
-        #         if last:    # if last hextet is '', ascend counter
-        #             ctr_[ptr_] += 1
-        #         else:       # if last hextet is not '', record pointer
-        #             ptr_ = _
-        #             last = True
-        #             ctr_[ptr_] = 1
-
-        # ptr_ = max(ctr_, key=ctr_.get) if ctr_ else 0   # fetch start pointer with longest zero values
-        # end_ = ptr_ + ctr_[ptr_]                        # calculate end pointer
-
-        # if ctr_[ptr_] > 1:      # only ommit if zero values are in a consecutive group
-        #     del adlt[ptr_:end_] # remove zero values
-
-        #     if ptr_ == 0 and end_ == 8:     # insert `::` if IPv6 unspecified address (::)
-        #         adlt.insert(ptr_, '::')
-        #     elif ptr_ == 0 or end_ == 8:    # insert `:` if zero values are from start or at end
-        #         adlt.insert(ptr_, ':')
-        #     else:                           # insert '' otherwise
-        #         adlt.insert(ptr_, '')
-
-        # addr = ':'.join(adlt)
-        # return addr
-        return ipaddress.ip_address(self._read_fileng(16))
+    def _read_ip_addr(self) -> 'IPv6Address':
+        """Read IP address.
+
+        Returns:
+            Parsed IP address.
+
+        """
+        return ipaddress.ip_address(self._read_fileng(16))  # type: ignore[return-value]
 
-    def _decode_next_layer(self, ipv6, proto=None, length=None):
+    def _decode_next_layer(self, ipv6: 'Data_IPv6', proto: 'Optional[int]' = None,  # type: ignore[override] # pylint: disable=arguments-differ,arguments-renamed
+                           length: 'Optional[int]' = None, *, packet: 'Optional[dict[str, Any]]' = None) -> 'Data_IPv6':  # pylint: disable=arguments-differ
         """Decode next layer extractor.
 
-        Positional arguments:
-            * ipv6 -- dict, info buffer
-            * proto -- str, next layer protocol name
-            * length -- int, valid (not padding) length
+        Arguments:
+            ipv6: info buffer
+            proto: next layer protocol name
+            length: valid (*not padding*) length
+            packet: packet info (passed from :meth:`self.unpack <pcapkit.protocols.protocol.Protocol.unpack>`)
 
         Returns:
-            * dict -- current protocol with next layer extracted
+            Current protocol with next layer extracted.
 
         """
-        # recurse if next header is an extensive header
-        hdr_len = 40                # header length
-        raw_len = ipv6['payload']   # payload length
-        while proto in EXT_HDR:
-            # keep original data after fragment header
-            if proto == 'IPv6-Frag':
-                ipv6['fragment'] = self._read_packet(header=hdr_len, payload=raw_len)
+        #: Extension headers.
+        self._exthdr = OrderedMultiDict()  # type: OrderedMultiDict[Enum_ExtensionHeader, Protocol] # pylint: disable=attribute-defined-outside-init
 
-            # directly break when No Next Header ocuurs
-            if proto == 'IPv6-NoNxt':
-                proto = None
+        hdr_len = self.length       # header length
+        raw_len = ipv6.payload      # payload length
+        _protos = []                # ProtoChain buffer
+
+        # traverse if next header is an extensive header
+        while True:
+            try:
+                ex_proto = Enum_ExtensionHeader(proto)
+            except ValueError:
                 break
 
+            # # directly break when No Next Header occurs
+            # if proto.name == 'IPv6-NoNxt':
+            #     proto = None
+            #     break
+
             # make protocol name
-            flag, next_ = self._import_next_layer(proto, version=6, extension=True)
-            info, chain, alias = next_.info, next_.protochain, next_.alias
-            name = proto.replace('IPv6-', '').lower() if flag else 'raw'
-            ipv6[name] = info
+            next_ = self._import_next_layer(proto, packet=packet, version=6, extension=True)  # type: ignore[misc,call-arg,arg-type]
+            info = next_.info
+            name = next_.alias.lstrip('IPv6-').lower()
+            ipv6.__update__({
+                name: info,
+            })
 
             # record protocol name
-            self._protos = ProtoChain(name, chain, alias)
-            if not flag:
-                proto = None
-                break
+            # self._protos = ProtoChain(name, chain, alias)
+            _protos.append(next_)
             proto = info.next
 
             # update header & payload length
-            hdr_len += info.length
-            raw_len -= info.length
+            hdr_len += next_.length  # type: ignore[assignment]
+            raw_len -= next_.length
+
+            # keep record of extension headers
+            self._exthdr.add(ex_proto, next_)
+
+            # keep original data after fragment header
+            if ex_proto == Enum_ExtensionHeader.IPv6_Frag:
+                ipv6.__update__({
+                    'fragment': self._read_packet(header=hdr_len, payload=raw_len),
+                })
+                break
 
         # record real header & payload length (headers exclude)
-        ipv6['hdr_len'] = hdr_len
-        ipv6['raw_len'] = raw_len
+        ipv6.__update__({
+            'hdr_len': hdr_len,
+            'raw_len': raw_len,
+
+            # update next header
+            'protocol': proto,
+        })
 
-        # update next header
-        ipv6['proto'] = None if proto in EXT_HDR else proto
-        return super()._decode_next_layer(ipv6, proto, raw_len)
+        ipv6_exthdr = ProtoChain.from_list(_protos)  # type: ignore[arg-type]
+        return super()._decode_next_layer(ipv6, proto, raw_len, packet=packet, ipv6_exthdr=ipv6_exthdr)
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/protocols/internet/ipx.py` & `pypcapkit-1.0.0b1/pcapkit/corekit/protochain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,206 +1,249 @@
 # -*- coding: utf-8 -*-
-"""internetwork packet exchange
+"""Protocol Chain
+====================
 
-`pcapkit.protocols.internet.ipx` contains `IPX` only,
-which implements extractor for Internetwork Packet
-Exchange (IPX), whose structure is described as below.
-
-Octets      Bits        Name                    Discription
-  0           0     ipx.cksum               Checksum
-  2          16     ipx.len                 Packet Length (header includes)
-  4          32     ipx.count               Transport Control (hop count)
-  5          40     ipx.type                Packet Type
-  6          48     ipx.dst                 Destination Address
-  18        144     ipx.src                 Source Address
+.. module:: pcapkit.corekit.protochain
+
+:mod:`pcapkit.corekit.protochain` contains special protocol
+collection class :class:`~pcapkit.corekit.protochain.ProtoChain`.
 
 """
-from pcapkit.corekit.infoclass import Info
-from pcapkit.protocols.internet.internet import Internet
+import collections.abc
+import copy
+from typing import TYPE_CHECKING, overload
 
+from pcapkit.utilities.compat import cached_property
+from pcapkit.utilities.exceptions import IndexNotFound
 
-__all__ = ['IPX']
+if TYPE_CHECKING:
+    from typing import Iterator, Optional, Type
 
+    from pcapkit.protocols.protocol import Protocol
 
-# IPX Packet Types
-TYPE = {
-    0 : 'Unknown',
-    1 : 'RIP',          # Routing Information Protocol [RFC 1582][RFC 2091]
-    2 : 'Echo Packet',
-    3 : 'Error Packet',
-    4 : 'PEP',          # Packet Exchange Protocol, used for SAP (Service Advertising Protocol)
-    5 : 'SPX',          # Sequenced Packet Exchange
-    6 : 'NCP',          # NetWare Core Protocol
-}
-
-# Socket Types
-SOCK = {
-    '0001' : 'Routing Information Packet',
-    '0002' : 'Echo Protocol Packet',
-    '0003' : 'Error Handling Packet',
-    '0451' : 'NCP',                         # Netware Core Protocol - used by Novell Netware servers
-    '0452' : 'SAP',                         # Service Advertising Protocol
-    '0453' : 'RIP',                         # Routing Information Protocol
-    '0455' : 'NetBIOS',
-    '0456' : 'Diagnostic Packet',
-    '0457' : 'Serialization Packet',        # used for NCP as well
-    '4003' : 'Novell Netware Client',       # Used by Novell Netware Client
-    '8060' : 'IPX',
-    '9091' : 'TCP',                         # TCP over IPXF
-    '9092' : 'UDP',                         # UDP over IPXF
-    '9093' : 'IPXF',                        # IPX Fragmentation Protocol
-}
-
-
-class IPX(Internet):
-    """This class implements Internetwork Packet Exchange.
-
-    Properties:
-        * name -- str, name of corresponding procotol
-        * info -- Info, info dict of current instance
-        * alias -- str, acronym of corresponding procotol
-        * layer -- str, `Internet`
-        * length -- int, header length of corresponding protocol
-        * protocol -- str, name of next layer protocol
-        * protochain -- ProtoChain, protocol chain of current instance
-        * src -- Info, source IPX address
-        * dst -- Info, destination IPX address
-
-    Methods:
-        * read_ipx -- read Internetwork Packet Exchange
-
-    Attributes:
-        * _file -- BytesIO, bytes to be extracted
-        * _info -- Info, info dict of current instance
-        * _protos -- ProtoChain, protocol chain of current instance
-
-    Utilities:
-        * _read_protos -- read next layer protocol type
-        * _read_fileng -- read file buffer
-        * _read_unpack -- read bytes and unpack to integers
-        * _read_binary -- read bytes and convert into binaries
-        * _read_packet -- read raw packet data
-        * _decode_next_layer -- decode next layer protocol type
-        * _import_next_layer -- import next layer protocol extractor
-        * _read_ipx_address -- read IPX address field
+__all__ = ['ProtoChain']
 
-    """
-    ##########################################################################
-    # Properties.
-    ##########################################################################
 
-    @property
-    def name(self):
-        """Name of corresponding procotol."""
-        return 'Internetwork Packet Exchange'
+class ProtoChain(collections.abc.Sequence):
+    """Protocols chain."""
 
-    @property
-    def length(self):
-        """Header length of corresponding protocol."""
-        return 30
+    #: Internal data storage for protocol chain.
+    __data__: 'tuple[tuple[str, Type[Protocol]], ...]'
 
-    @property
-    def protocol(self):
-        """Name of next layer protocol."""
-        return self._info.type
+    ##########################################################################
+    # Properties.
+    ##########################################################################
 
-    @property
-    def src(self):
-        """Source IPX address."""
-        return self._info.src.addr
+    @cached_property
+    def protocols(self) -> 'tuple[Type[Protocol], ...]':
+        """List of protocols in the chain."""
+        return tuple(data[1] for data in self.__data__)
+
+    @cached_property
+    def aliases(self) -> 'tuple[str, ...]':
+        """Protocol names."""
+        return tuple(data[0] for data in self.__data__)
 
     @property
-    def dst(self):
-        """Destination IPX address."""
-        return self._info.dst.addr
+    def chain(self) -> 'str':
+        """Protocol chain string."""
+        return self.__str__()
 
     ##########################################################################
     # Methods.
     ##########################################################################
 
-    def read_ipx(self, length):
-        """Read Internetwork Packet Exchange.
+    @classmethod
+    def from_list(cls, data: 'list[Protocol | Type[Protocol]]') -> 'ProtoChain':
+        """Create a protocol chain from a list.
 
-        Structure of IPX header [RFC 1132]:
-            Octets      Bits        Name                    Discription
-              0           0     ipx.cksum               Checksum
-              2          16     ipx.len                 Packet Length (header includes)
-              4          32     ipx.count               Transport Control (hop count)
-              5          40     ipx.type                Packet Type
-              6          48     ipx.dst                 Destination Address
-              18        144     ipx.src                 Source Address
-
-        """
-        if length is None:
-            length = len(self)
-
-        _csum = self._read_fileng(2)
-        _tlen = self._read_unpack(2)
-        _ctrl = self._read_unpack(1)
-        _type = self._read_unpack(1)
-        _dsta = self._read_ipx_address()
-        _srca = self._read_ipx_address()
-
-        ipx = dict(
-            chksum = _csum,
-            len = _tlen,
-            count = _ctrl,
-            type = TYPE.get(_type),
-            dst = _dsta,
-            src = _srca,
-        )
-
-        proto = ipx['type']
-        length = ipx['len'] - 30
-        ipx['packet'] = self._read_packet(header=30, payload=length)
+        Args:
+            data: Protocol chain list.
 
-        return self._read_next_layer(ipx, proto, length)
+        """
+        from pcapkit.protocols.protocol import Protocol  # pylint: disable=import-outside-toplevel
+
+        temp_data = []
+        for proto in data:
+            if isinstance(proto, Protocol):
+                alias = proto.alias
+                proto = type(proto)
+
+            temp_data.append((alias, proto))
+
+        obj = cls.__new__(cls)
+        obj.__data__ = tuple(temp_data)
+        return obj
+
+    def index(self, value: 'str | Protocol | Type[Protocol]',
+              start: 'Optional[int]' = None, stop: 'Optional[int]' = None) -> 'int':
+        """First index of ``value``.
+
+        Args:
+            value: Value to search.
+            start: start offset.
+            stop: stop offset.
+
+        Raises:
+            IndexNotFound: If the value is not present.
+
+        """
+        if start is None:
+            start = 0
+        elif start < 0:
+            start = max(len(self) + start, 0)
+
+        if stop is not None and stop < 0:
+            stop += len(self)
+
+        # prepare comparison values
+        from pcapkit.protocols.protocol import Protocol  # pylint: disable=import-outside-toplevel
+        comp = Protocol.expand_comp(value)
+
+        pool = self.__data__[start:stop]
+        for idx, (alias, proto) in enumerate(pool):
+            test_comp = (proto, alias.upper(), *(name.upper() for name in proto.id()))
+            for test in comp:
+                if test in test_comp:
+                    return start + idx
+        raise IndexNotFound(f'{value!r} is not in {self.__class__.__name__!r}')
+
+    def count(self, value: 'str | Protocol | Type[Protocol]') -> int:
+        """Number of occurrences of ``value``.
+
+        Args:
+            value: Value to search.
+
+        """
+        # prepare comparison values
+        from pcapkit.protocols.protocol import Protocol  # pylint: disable=import-outside-toplevel
+        comp = Protocol.expand_comp(value)
+
+        cnt = 0
+        for alias, proto in self.__data__:
+            test_comp = (proto, alias.upper(), *(name.upper() for name in proto.id()))
+            for test in comp:
+                if test in test_comp:
+                    cnt += 1
+                    break
+        return cnt
 
     ##########################################################################
     # Data models.
     ##########################################################################
 
-    def __init__(self, _file, length=None, **kwargs):
-        self._file = _file
-        self._info = Info(self.read_ipx(length))
+    def __init__(self, proto: 'Protocol | Type[Protocol]', alias: 'Optional[str]' = None, *,
+                 basis: 'Optional[ProtoChain]' = None):
+        """Initialisation.
+
+        Args:
+            proto: New protocol class on the top stack.
+            alias: New protocol alias on the top stack.
+            basis: Original protocol chain as base stacks.
 
-    def __length_hint__(self):
-        return 30
+        """
+        from pcapkit.protocols.protocol import Protocol  # pylint: disable=import-outside-toplevel
+        if isinstance(proto, Protocol):
+            if alias is None:
+                alias = proto.alias
+            proto = type(proto)
+
+        if alias is None:
+            alias = proto.__name__
+
+        temp_data = [(alias, proto)]
+        if basis is not None:
+            temp_data.extend(basis)
+        self.__data__ = tuple(temp_data)
+
+    def __repr__(self) -> 'str':
+        """Returns representation of protocol chain data.
+
+        Example:
+            >>> protochain
+            ProtoChain(Ethernet, IPv6, Raw)
 
-    ##########################################################################
-    # Utilities.
-    ##########################################################################
+        """
+        return f"ProtoChain({', '.join(map(lambda p: p[1].__name__, self.__data__))})"
 
-    def _read_ipx_address(self):
-        """Read IPX address field.
+    def __str__(self) -> 'str':
+        """Returns formatted hex representation of source data stream.
 
-        Structure of IPX address:
-            Octets      Bits        Name                    Discription
-              0           0     ipx.addr.network        Network Number
-              4          32     ipx.addr.node           Node Number
-              10         80     ipx.addr.socket         Socket Number
+        Example:
+            >>> protochain
+            ProtoChain(Ethernet, IPv6, Raw)
+            >>> print(protochain)
+            Ethernet:IPv6:Raw
 
         """
-        # Adress Number
-        _byte = self._read_fileng(4)
-        _ntwk = ':'.join(textwrap.wrap(_byte.hex(), 2))
+        return ':'.join(map(lambda p: p[0], self.__data__))
+
+    def __contains__(self, name: 'str | Protocol | Type[Protocol]') -> 'bool':  # type: ignore[override]
+        """Returns if ``name`` is in the chain.
 
-        # Node Number (MAC)
-        _byte = self._read_fileng(6)
-        _node = ':'.join(textwrap.wrap(_byte.hex(), 2))
-        _maca = '-'.join(textwrap.wrap(_byte.hex(), 2))
+        Args:
+            name: Name to search.
+
+        Returns:
+            Whether ``name`` is in the chain.
+
+        """
+        from pcapkit.protocols.protocol import Protocol  # pylint: disable=import-outside-toplevel
+        comp = Protocol.expand_comp(name)
 
-        # Socket Number
-        _sock = self._read_fileng(2)
+        for alias, proto in self.__data__:
+            test_comp = (proto, alias.upper(), *(name.upper() for name in proto.id()))
+            for test in comp:
+                if test in test_comp:
+                    return True
+        return False
+
+    @overload
+    def __getitem__(self, index: 'int') -> 'str': ...
+    @overload
+    def __getitem__(self, index: 'slice') -> 'tuple[str, ...]': ...
+
+    def __getitem__(self, index: 'int | slice') -> 'str | tuple[str, ...]':
+        """Subscription (``getitem``) support.
+
+        Args:
+            index: Indexing key.
+
+        Returns:
+            Protocol alias at such index.
+
+        """
+        if isinstance(index, slice):
+            return tuple(data[0] for data in self.__data__[index])
+        return self.__data__[index][0]
 
-        # Whole Address
-        _list = [_ntwk, _node, _sock.hex()]
-        _addr = ':'.join(_list)
+    def __iter__(self) -> 'Iterator[tuple[str, Type[Protocol]]]':
+        """Iterator support.
 
-        addr = dict(
-            network = _ntwk,
-            node = _maca,
-            socket = SOCK.get(_sock.hex()) or _sock,
-            addr = _addr,
-        )
+        Returns:
+            Iterator of protocol alias and class.
 
-        return addr
+        """
+        return iter(self.__data__)
+
+    def __len__(self) -> 'int':
+        """Length support.
+
+        Returns:
+            Length of protocol chain.
+
+        """
+        return len(self.__data__)
+
+    def __add__(self, other: 'ProtoChain') -> 'ProtoChain':
+        """Merge protocol chain by appending protocols from ``other``.
+
+        Args:
+            other: Protocol chain to be merged.
+
+        Returns:
+            Merged protocol chain.
+
+        """
+        new = copy.copy(self)
+        new.__data__ += other.__data__
+        return new
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/protocols/link/__init__.py` & `pypcapkit-1.0.0b1/pcapkit/protocols/link/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # -*- coding: utf-8 -*-
-"""link layer protocols
+# pylint: disable=unused-import,unused-wildcard-import,fixme
+"""Link Layer Protocols
+==========================
 
-`pcapkit.protocols.link` is collection of all protocols in
+.. module:: pcapkit.protocols.link
+
+:mod:`pcapkit.protocols.link` is collection of all protocols in
 link layer, with detailed implementation and methods.
 
 """
 # TODO: Implements DSL, EAPOL, FDDI, ISDN, NDP, PPP.
 
 # Base Class for Link Layer
 from pcapkit.protocols.link.link import Link
 
 # Utility Classes for Protocols
-from pcapkit.protocols.link.arp import ARP
-from pcapkit.protocols.link.arp import ARP as InARP
+from pcapkit.protocols.link.arp import ARP, InARP
 from pcapkit.protocols.link.ethernet import Ethernet
 from pcapkit.protocols.link.l2tp import L2TP
 from pcapkit.protocols.link.ospf import OSPF
-from pcapkit.protocols.link.rarp import RARP
-from pcapkit.protocols.link.rarp import RARP as DRARP
+from pcapkit.protocols.link.rarp import RARP, DRARP
 from pcapkit.protocols.link.vlan import VLAN
 
 # Link-Layer Header Type Values
-from pcapkit.protocols.link.link import LINKTYPE
-
+from pcapkit.const.reg.linktype import LinkType as LINKTYPE
 
 __all__ = [
-    'LINKTYPE',                             # Protocol Numbers
-    'ARP', 'DRARP', 'Ethernet', 'InARP', 'L2TP', 'OSPF', 'RARP', 'VLAN',
-                                            # Link Layer Protocols
+    # Protocol Numbers
+    'LINKTYPE',
+
+    # Link Layer Protocols
+    'ARP', 'DRARP', 'Ethernet', 'InARP', 'L2TP',
+    'OSPF', 'RARP', 'VLAN',
 ]
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/protocols/link/ospf.py` & `pypcapkit-1.0.0b1/pcapkit/protocols/internet/ipv6_frag.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,221 +1,258 @@
 # -*- coding: utf-8 -*-
-"""open shortest path first
+"""IPv6-Frag - Fragment Header for IPv6
+==========================================
 
-`pcapkit.protocols.link.ospf` contains `OSPF` only,
-which implements extractor for Open Shortest Path First
-(OSPF), whose structure is described as below.
-
- 0                   1                   2                   3
- 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|   Version #   |     Type      |         Packet length         |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|                          Router ID                            |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|                           Area ID                             |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|           Checksum            |             AuType            |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|                       Authentication                          |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-|                       Authentication                          |
-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
+.. module:: pcapkit.protocols.internet.ipv6_frag
+
+:mod:`pcapkit.protocols.internet.ipv6_frag` contains
+:class:`~pcapkit.protocols.internet.ipv6_frag.IPv6_Frag`
+only, which implements extractor for Fragment Header for
+IPv6 (IPv6-Frag) [*]_, whose structure is described as
+below:
+
+======= ========= ==================== =======================
+Octets      Bits        Name                    Description
+======= ========= ==================== =======================
+  0           0   ``frag.next``               Next Header
+  1           8                               Reserved
+  2          16   ``frag.offset``             Fragment Offset
+  3          29                               Reserved
+  3          31   ``frag.mf``                 More Flag
+  4          32   ``frag.id``                 Identification
+======= ========= ==================== =======================
+
+.. [*] https://en.wikipedia.org/wiki/IPv6_packet#Fragment
 
 """
-from pcapkit.corekit.infoclass import Info
-from pcapkit.protocols.link.link import Link
+from typing import TYPE_CHECKING, overload
+
+from pcapkit.const.reg.transtype import TransType as Enum_TransType
+from pcapkit.protocols.data.internet.ipv6_frag import IPv6_Frag as Data_IPv6_Frag
+from pcapkit.protocols.internet.internet import Internet
+from pcapkit.protocols.schema.internet.ipv6_frag import IPv6_Frag as Schema_IPv6_Frag
+from pcapkit.utilities.exceptions import UnsupportedCall
 
+if TYPE_CHECKING:
+    from enum import IntEnum as StdlibEnum
+    from typing import IO, Any, NoReturn, Optional, Type
 
-__all__ = ['OSPF']
+    from aenum import IntEnum as AenumEnum
+    from typing_extensions import Literal
 
+    from pcapkit.corekit.protochain import ProtoChain
+    from pcapkit.protocols.protocol import Protocol
+    from pcapkit.protocols.schema.schema import Schema
 
-# OSPF Packet Types
-TYPE = {
-    1 : 'Hello',
-    2 : 'Database Description',
-    3 : 'Link State Request',
-    4 : 'Link State Update',
-    5 : 'Link State Acknowledgment',
-}
-
-
-# Authentication Types
-AUTH = {
-    0 : 'Null Authentication',
-    1 : 'Simple Password',
-    2 : 'Cryptographic Authentication',
-}
-
-
-class OSPF(Link):
-    """This class implements Open Shortest Path First.
-
-    Properties:
-        * name -- str, name of corresponding protocol
-        * info -- Info, info dict of current instance
-        * alias -- str, acronym of corresponding protocol
-        * layer -- str, `Link`
-        * length -- int, header length of corresponding protocol
-        * protochain -- ProtoChain, protocol chain of current instance
-        * type -- str, OSPF packet type
-
-    Methods:
-        * decode_bytes -- try to decode bytes into str
-        * decode_url -- decode URLs into Unicode
-        * read_ospf -- read Open Shortest Path First
-
-    Attributes:
-        * _file -- BytesIO, bytes to be extracted
-        * _info -- Info, info dict of current instance
-        * _protos -- ProtoChain, protocol chain of current instance
-
-    Utilities:
-        * _read_protos -- read next layer protocol type
-        * _read_fileng -- read file buffer
-        * _read_unpack -- read bytes and unpack to integers
-        * _read_binary -- read bytes and convert into binaries
-        * _read_packet -- read raw packet data
-        * _decode_next_layer -- decode next layer protocol type
-        * _import_next_layer -- import next layer protocol extractor
-        * _read_id_numbers -- read router and area IDs
-        * _read_encrypt_auth -- read Authentication field when CA employed
+__all__ = ['IPv6_Frag']
+
+
+class IPv6_Frag(Internet[Data_IPv6_Frag, Schema_IPv6_Frag],
+                schema=Schema_IPv6_Frag, data=Data_IPv6_Frag):
+    """This class implements Fragment Header for IPv6."""
 
-    """
     ##########################################################################
     # Properties.
     ##########################################################################
 
     @property
-    def name(self):
+    def name(self) -> 'Literal["Fragment Header for IPv6"]':
         """Name of current protocol."""
-        return 'Open Shortest Path First'
+        return 'Fragment Header for IPv6'
 
     @property
-    def length(self):
+    def alias(self) -> 'Literal["IPv6-Frag"]':
+        """Acronym of corresponding protocol."""
+        return 'IPv6-Frag'
+
+    @property
+    def length(self) -> 'Literal[8]':
         """Header length of current protocol."""
-        return 24
+        return 8
+
+    @property
+    def payload(self) -> 'Protocol | NoReturn':
+        """Payload of current instance.
+
+        Raises:
+            UnsupportedCall: if the protocol is used as an IPv6 extension header
+
+        """
+        if self._extf:
+            raise UnsupportedCall(f"'{self.__class__.__name__}' object has no attribute 'payload'")
+        return self._next
+
+    @property
+    def protocol(self) -> 'Optional[str] | NoReturn':
+        """Name of next layer protocol (if any).
+
+        Raises:
+            UnsupportedCall: if the protocol is used as an IPv6 extension header
+
+        """
+        if self._extf:
+            raise UnsupportedCall(f"'{self.__class__.__name__}' object has no attribute 'protocol'")
+        return super().protocol
 
     @property
-    def type(self):
-        """OSPF packet type."""
-        return self._info.type
+    def protochain(self) -> 'ProtoChain | NoReturn':
+        """Protocol chain of current instance.
+
+        Raises:
+            UnsupportedCall: if the protocol is used as an IPv6 extension header
+
+        """
+        if self._extf:
+            raise UnsupportedCall(f"'{self.__class__.__name__}' object has no attribute 'protochain'")
+        return super().protochain
 
     ##########################################################################
     # Methods.
     ##########################################################################
 
-    def read_ospf(self, length):
-        """Read Open Shortest Path First.
+    def read(self, length: 'Optional[int]' = None, *, extension: 'bool' = False,  # pylint: disable=arguments-differ
+             **kwargs: 'Any') -> 'Data_IPv6_Frag':  # pylint: disable=unused-argument
+        """Read Fragment Header for IPv6.
+
+        Structure of IPv6-Frag header [:rfc:`8200`]:
+
+        .. code-block:: text
 
-        Structure of OSPF header [RFC 2328]:
-            0                   1                   2                   3
-            0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
-           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-           |   Version #   |     Type      |         Packet length         |
-           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-           |                          Router ID                            |
-           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-           |                           Area ID                             |
-           +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-           |           Checksum            |             AuType            |
            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-           |                       Authentication                          |
+           |  Next Header  |   Reserved    |      Fragment Offset    |Res|M|
            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-           |                       Authentication                          |
+           |                         Identification                        |
            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 
-            Octets      Bits        Name                    Discription
-              0           0     ospf.version            Version #
-              1           8     ospf.type               Type (0/1)
-              2          16     ospf.len                Packet Length (header includes)
-              4          32     ospf.router_id          Router ID
-              8          64     ospf.area_id            Area ID
-              12         96     ospf.chksum             Checksum
-              14        112     ospf.autype             AuType
-              16        128     ospf.auth               Authentication
+        Args:
+            length: Length of packet data.
+            extension: If the packet is used as an IPv6 extension header.
+            **kwargs: Arbitrary keyword arguments.
+
+        Returns:
+            Parsed packet data.
 
         """
         if length is None:
             length = len(self)
+        schema = self.__header__
 
-        _vers = self._read_unpack(1)
-        _type = self._read_unpack(1)
-        _tlen = self._read_unpack(2)
-        _rtid = self._read_id_numbers()
-        _area = self._read_id_numbers()
-        _csum = self._read_fileng(2)
-        _autp = self._read_unpack(2)
-
-        ospf = dict(
-            version = _vers,
-            type = TYPE.get(_type),
-            len = _tlen,
-            router_id = _rtid,
-            area_id = _area,
-            chksum = _csum,
-            autype = AUTH.get(_autp) or 'Reserved',
+        ipv6_frag = Data_IPv6_Frag(
+            next=schema.next,
+            offset=schema.flags['offset'],
+            mf=bool(schema.flags['mf']),
+            id=schema.id,
         )
 
-        if _autp == 2:
-            ospf['auth'] = self._read_encrypt_auth()
-        else:
-            ospf['auth'] = self._read_fileng(8)
+        if extension:
+            return ipv6_frag
+        return self._decode_next_layer(ipv6_frag, schema.next, length - self.length)
+
+    def make(self,
+             next: 'Enum_TransType | StdlibEnum | AenumEnum | str | int' = Enum_TransType.UDP,
+             next_default: 'Optional[int]' = None,
+             next_namespace: 'Optional[dict[str, int] | dict[int, str] | Type[StdlibEnum] | Type[AenumEnum]]' = None,  # pylint: disable=line-too-long
+             next_reversed: 'bool' = False,
+             offset: 'int' = 0,
+             mf: 'bool' = False,
+             id: 'int' = 0,
+             payload: 'bytes | Protocol | Schema' = b'',
+             **kwargs: 'Any') -> 'Schema_IPv6_Frag':
+        """Make (construct) packet data.
+
+        Args:
+            next: Next header.
+            next_default: Default value of next header.
+            next_namespace: Namespace of next header.
+            next_reversed: If the namespace of next header is reversed.
+            offset: Fragment offset.
+            mf: More fragments flag.
+            id: Identification.
+            payload: Payload of current instance.
+            **kwargs: Arbitrary keyword arguments.
 
-        length = ospf['len'] - 24
-        ospf['packet'] = self._read_packet(header=24, payload=length)
+        Returns:
+            Constructed packet data.
 
-        return self._decode_next_layer(ospf, length)
+        """
+        next_val = self._make_index(next, next_default, namespace=next_namespace,  # type: ignore[call-overload]
+                                    reversed=next_reversed, pack=False)
+
+        return Schema_IPv6_Frag(
+            next=next_val,
+            flags={
+                'offset': offset,
+                'mf': mf,
+            },
+            id=id,
+            payload=payload,
+        )
 
     ##########################################################################
     # Data models.
     ##########################################################################
 
-    def __init__(self, _file, length=None, **kwargs):
-        self._file = _file
-        self._info = Info(self.read_ospf(length))
+    @overload
+    def __post_init__(self, file: 'IO[bytes] | bytes', length: 'Optional[int]' = ..., *,  # pylint: disable=arguments-differ
+                      extension: 'bool' = ..., **kwargs: 'Any') -> 'None': ...
+
+    @overload
+    def __post_init__(self, **kwargs: 'Any') -> 'None': ...  # pylint: disable=arguments-differ
+
+    def __post_init__(self, file: 'Optional[IO[bytes] | bytes]' = None, length: 'Optional[int]' = None, *,  # pylint: disable=arguments-differ
+                      extension: 'bool' = False, **kwargs: 'Any') -> 'None':
+        """Post initialisation hook.
+
+        Args:
+            file: Source packet stream.
+            length: Length of packet data.
+            extension: If the protocol is used as an IPv6 extension header.
+            **kwargs: Arbitrary keyword arguments.
+
+        See Also:
+            For construction argument, please refer to :meth:`make`.
+
+        """
+        #: bool: If the protocol is used as an IPv6 extension header.
+        self._extf = extension
 
-    def __length_hint__(self):
-        return 24
+        # call super __post_init__
+        super().__post_init__(file, length, extension=extension, **kwargs)  # type: ignore[arg-type]
+
+    def __length_hint__(self) -> 'Literal[8]':
+        """Return an estimated length for the object."""
+        return 8
+
+    @classmethod
+    def __index__(cls) -> 'Enum_TransType':  # pylint: disable=invalid-index-returned
+        """Numeral registry index of the protocol.
+
+        Returns:
+            Numeral registry index of the protocol in `IANA`_.
+
+        .. _IANA: https://www.iana.org/assignments/protocol-numbers/protocol-numbers.xhtml
+
+        """
+        return Enum_TransType.IPv6_Frag  # type: ignore[return-value]
 
     ##########################################################################
     # Utilities.
     ##########################################################################
 
-    def _read_id_numbers(self):
-        """Read router and area IDs."""
-        _byte = self._read_fileng(4)
-        _addr = '.'.join([str(_) for _ in _byte])
-        return _addr
-
-    def _read_encrypt_auth(self):
-        """Read Authentication field when Cryptographic Authentication is employed.
-
-        Structure of Cryptographic Authentication [RFC 2328]:
-
-             0                   1                   2                   3
-             0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            |              0                |    Key ID     | Auth Data Len |
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-            |                 Cryptographic sequence number                 |
-            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-
-            Octets      Bits        Name                    Discription
-              0           0     -                       Reserved (must be zero)
-              2          16     ospf.auth.key_id        Key ID
-              3          24     ospf.auth.len           Auth Data Length
-              4          32     ospf.auth.seq           Cryptographic Sequence Number
-
-        """
-        _resv = self._read_fileng(2)
-        _keys = self._read_unpack(1)
-        _alen = self._read_unpack(1)
-        _seqn = self._read_unpack(4)
-
-        auth = dict(
-            key_id = _keys,
-            len = _alen,
-            seq = _seqn,
-        )
+    @classmethod
+    def _make_data(cls, data: 'Data_IPv6_Frag') -> 'dict[str, Any]':  # type: ignore[override]
+        """Create key-value pairs from ``data`` for protocol construction.
+
+        Args:
+            data: protocol data
 
-        return auth
+        Returns:
+            Key-value pairs for protocol construction.
+
+        """
+        return {
+            'next': data.next,
+            'offset': data.offset,
+            'mf': data.mf,
+            'id': data.id,
+            'payload': cls._make_payload(data),
+        }
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/reassembly/ip.py` & `pypcapkit-1.0.0b1/pcapkit/foundation/reassembly/reassembly.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,219 +1,221 @@
 # -*- coding: utf-8 -*-
-"""reassembly IP fragments
+"""Base Class
+================
 
-`pcapkit.reassembly.ip` contains `IP_Reassembly` only,
-which is the base class for IPv4 and IPv6 reassembly.
-The following algorithm implementment is based on IP
-reassembly procedure introduced in RFC 791, using
-`RCVBT` (fragment receivedbit table). Though another
-algorithm is explained in RFC 815, replacing `RCVBT`,
-however, this implementment still used the elder one.
-And here is the pseudo-code:
-
-Notations:
-
-    FO    - Fragment Offset
-    IHL   - Internet Header Length
-    MF    - More Fragments flag
-    TTL   - Time To Live
-    NFB   - Number of Fragment Blocks
-    TL    - Total Length
-    TDL   - Total Data Length
-    BUFID - Buffer Identifier
-    RCVBT - Fragment Received Bit Table
-    TLB   - Timer Lower Bound
-
-Algorithm:
-
-    DO {
-        BUFID <- source|destination|protocol|identification;
-
-        IF (FO = 0 AND MF = 0) {
-            IF (buffer with BUFID is allocated) {
-                flush all reassembly for this BUFID;
-                Submit datagram to next step;
-                DONE.
-            }
-        }
-
-        IF (no buffer with BUFID is allocated) {
-            allocate reassembly resources with BUFID;
-            TIMER <- TLB;
-            TDL <- 0;
-            put data from fragment into data buffer with BUFID
-                [from octet FO*8 to octet (TL-(IHL*4))+FO*8];
-            set RCVBT bits [from FO to FO+((TL-(IHL*4)+7)/8)];
-        }
-
-        IF (MF = 0) {
-            TDL <- TL-(IHL*4)+(FO*8)
-        }
-
-        IF (FO = 0) {
-            put header in header buffer
-        }
-
-        IF (TDL # 0 AND all RCVBT bits [from 0 to (TDL+7)/8] are set) {
-            TL <- TDL+(IHL*4)
-            Submit datagram to next step;
-            free all reassembly resources for this BUFID;
-            DONE.
-        }
-
-        TIMER <- MAX(TIMER,TTL);
-
-    } give up until (next fragment or timer expires);
-
-    timer expires: {
-        flush all reassembly with this BUFID;
-        DONE.
-    }
+.. module:: pcapkit.foundation.reassembly.reassembly
 
-"""
-import copy
+:mod:`pcapkit.foundation.reassembly.reassembly` contains
+:class:`~pcapkit.foundation.reassembly.reassembly.Reassembly` only,
+which is an abstract base class for all reassembly classes,
+bases on algorithms described in :rfc:`791` and :rfc:`815`,
+implements datagram reassembly of IP and TCP packets.
 
-from pcapkit.corekit.infoclass import Info
-from pcapkit.reassembly.reassembly import Reassembly
+"""
+import abc
+from typing import TYPE_CHECKING, Generic, TypeVar
 
+if TYPE_CHECKING:
+    from typing import Any, Optional, Type
 
-__all__ = ['IP_Reassembly']
+    from pcapkit.corekit.infoclass import Info
+    from pcapkit.protocols.protocol import Protocol
 
+__all__ = ['Reassembly']
 
-class IP_Reassembly(Reassembly):
-    """Reassembly for IP payload.
+# packet
+PT = TypeVar('PT', bound='Info')
+# datagram
+DT = TypeVar('DT', bound='Info')
+# buffer ID
+IT = TypeVar('IT', bound='tuple')
+# buffer
+BT = TypeVar('BT', bound='Info')
 
-    Properties:
-        * name -- str, protocol of current packet
-        * count -- int, total number of reassembled packets
-        * datagram -- tuple, reassembled datagram, which structure may vary
-                        according to its protocol
-        * protocol -- str, protocol of current reassembly object
 
-    Methods:
-        * reassembly -- perform the reassembly procedure
-        * submit -- submit reassembled payload
-        * fetch -- fetch datagram
-        * index -- return datagram index
-        * run -- run automatically
+class Reassembly(Generic[PT, DT, IT, BT], metaclass=abc.ABCMeta):
+    """Base class for reassembly procedure.
 
-    Attributes:
-        * _strflg -- bool, stirct mode flag
-        * _buffer -- dict, buffer field
-        * _dtgram -- tuple, reassembled datagram
+    Args:
+        strict: if return all datagrams (including those not
+            implemented) when submit
 
     """
+
+    _strflg: 'bool'
+    _newflg: 'bool'
+
+    # Internal data storage for cached properties.
+    __cached__: 'dict[str, Any]'
+
+    ##########################################################################
+    # Properties.
+    ##########################################################################
+
+    # protocol name of current reassembly object
+    @property
+    @abc.abstractmethod
+    def name(self) -> 'str':
+        """Protocol name of current reassembly object."""
+
+    # total number of reassembled packets
+    @property
+    def count(self) -> 'int':
+        """Total number of reassembled packets."""
+        if self._newflg:
+            self.__cached__.clear()
+            self._newflg = False
+
+        if (cached := self.__cached__.get('count')) is not None:
+            return cached
+
+        ret = len(self.datagram)
+        self.__cached__['count'] = ret
+        return ret
+
+    # reassembled datagram
+    @property
+    def datagram(self) -> 'tuple[DT, ...]':
+        """Reassembled datagram."""
+        if self._buffer:
+            return self.fetch()
+        return tuple(self._dtgram)
+
+    @property
+    @abc.abstractmethod
+    def protocol(self) -> 'Type[Protocol]':
+        """Protocol of current reassembly object."""
+
     ##########################################################################
     # Methods.
     ##########################################################################
 
-    def reassembly(self, info):
+    # reassembly procedure
+    @abc.abstractmethod
+    def reassembly(self, info: 'PT') -> 'None':
         """Reassembly procedure.
 
-        Positional arguments:
-            * info -- Info, info dict of packets to be reassembled
+        Arguments:
+            info: info dict of packets to be reassembled
 
         """
-        BUFID = info.bufid  # Buffer Identifier
-        FO = info.fo        # Fragment Offset
-        IHL = info.ihl      # Internet Header Length
-        MF = info.mf        # More Fragments flag
-        TL = info.tl        # Total Length
-
-        # when unfragmented (possibly discarded) packet received
-        if not FO and not MF:
-            if BUFID in self._buffer:
-                self._dtgram += self.submit(self._buffer[BUFID])
-                del self._buffer[BUFID]
-                return
-
-        # initialise buffer with BUFID
-        if BUFID not in self._buffer:
-            self._buffer[BUFID] = dict(
-                TDL = 0,                        # Total Data Length
-                RCVBT = bytearray(8191),        # Fragment Received Bit Table
-                index = list(),                 # index record
-                header = bytearray(),           # header buffer
-                datagram = bytearray(65535),    # data buffer
-            )
+        # clear cache
+        self._newflg = False
+        self.__cached__['count'] = None
+        self.__cached__['fetch'] = None
+
+    # submit reassembled payload
+    @abc.abstractmethod
+    def submit(self, buf: 'BT', **kwargs: 'Any') -> 'list[DT]':
+        """Submit reassembled payload.
 
-        # append packet index
-        self._buffer[BUFID]['index'].append(info.num)
+        Arguments:
+            buf: buffer dict of reassembled packets
+            **kwargs: arbitrary keyword arguments
 
-        # put data into data buffer
-        start = FO
-        stop = TL - IHL + FO
-        self._buffer[BUFID]['datagram'][start:stop] = info.payload
-
-        # set RCVBT bits (in 8 octets)
-        start = FO // 8
-        stop = FO // 8 + (TL - IHL + 7) // 8
-        self._buffer[BUFID]['RCVBT'][start:stop] = b'\x01' * (stop - start + 1)
-
-        # get total data length (header excludes)
-        if not MF:
-            TDL = TL - IHL + FO
-
-        # put header into header buffer
-        if not FO:
-            self._buffer[BUFID]['header'] = info.header
-
-        # when datagram is reassembled in whole
-        start = 0
-        stop = (TDL + 7) // 8
-        if TDL and all(self._buffer[BUFID]['RCVBT'][start:stop]):
-            self._dtgram += self.submit(self._buffer[BUFID], checked=True)
-            del self._buffer[BUFID]
+        """
 
-    def submit(self, buf, *, checked=False):
-        """Submit reassembled payload.
+    # fetch datagram
+    def fetch(self) -> 'tuple[DT, ...]':
+        """Fetch datagram.
+
+        Returns:
+            Tuple of reassembled datagrams.
+
+        Fetch reassembled datagrams from
+        :attr:`~pcapkit.foundation.reassembly.reassembly.Reassembly._dtgram`
+        and returns a *tuple* of such datagrams.
+
+        If no cache found, the method will call
+        :meth:`~pcapkit.foundation.reassembly.reassembly.Reassembly.submit` to
+        *forcedly* obtain newly reassembled payload. Otherwise, the
+        already calculated :attr:`~pcapkit.foundation.reassembly.reassembly.Reassembly._dtgram`
+        will be returned.
+
+        """
+        if self._newflg:
+            self.__cached__.clear()
+            self._newflg = False
+
+        if (cached := self.__cached__.get('fetch')) is not None:
+            return cached
+
+        temp_dtgram = []  # type: list[DT]
+        for (bufid, buffer) in self._buffer.items():
+            temp_dtgram.extend(
+                self.submit(buffer, bufid=bufid)
+            )
+        temp_dtgram.extend(self._dtgram)
+        ret = tuple(temp_dtgram)
+
+        self.__cached__['fetch'] = ret
+        return ret
 
-        Positional arguments:
-            * buf -- dict, buffer dict of reassembled packets
+    # return datagram index
+    def index(self, pkt_num: 'int') -> 'Optional[int]':
+        """Return datagram index.
 
-        Keyword arguments:
-            * bufid -- tuple, buffer identifier
+        Arguments:
+            pkt_num: index of packet
 
         Returns:
-            * list -- reassembled packets
+            Reassembled datagram index which was from No. ``pkt_num`` packet;
+            if not found, returns :obj:`None`.
 
         """
-        TDL = buf['TDL']
-        RCVBT = buf['RCVBT']
-        index = buf['index']
-        header = buf['header']
-        datagram = buf['datagram']
-
-        start = 0
-        stop = (TDL + 7) // 8
-        flag = checked or (TDL and all(RCVBT[start:stop]))
-        # if datagram is not implemented
-        if not flag and self._strflg:
-            data = list()
-            byte = bytearray()
-            # extract received payload
-            for (bctr, bit) in enumerate(RCVBT):
-                if bit: # received bit
-                    this = bctr * 8
-                    that = this + 8
-                    byte += datagram[this:that]
-                else:   # missing bit
-                    if byte:    # strip empty payload
-                        data.append(bytes(byte))
-                    byte = bytearray()
-            # strip empty packets
-            if data or header:
-                packet = Info(
-                    NotImplemented = True,
-                    index = tuple(index),
-                    header = header or None,
-                    payload = tuple(data) or None,
-                )
-        # if datagram is reassembled in whole
-        else:
-            payload = datagram[:TDL]
-            packet = Info(
-                NotImplemented = False,
-                index = tuple(index),
-                packet = (bytes(header) + bytes(payload)) or None,
-            )
-        return [packet]
+        for counter, datagram in enumerate(self.datagram):
+            if pkt_num in datagram.index:  # type: ignore[attr-defined]
+                return counter
+        return None
+
+    # run automatically
+    def run(self, packets: 'list[PT]') -> 'None':
+        """Run automatically.
+
+        Arguments:
+            packets: list of packet dicts to be reassembled
+
+        """
+        for packet in packets:
+            self.reassembly(packet)
+
+    ##########################################################################
+    # Data models.
+    ##########################################################################
+
+    def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'Reassembly[PT, DT, IT, BT]':  # pylint: disable=unused-argument
+        self = super().__new__(cls)
+
+        # NOTE: Assign this attribute after ``__new__`` to avoid shared memory
+        # reference between instances.
+        self.__cached__ = {}
+
+        return self
+
+    def __init__(self, *, strict: 'bool' = True) -> 'None':
+        """Initialise packet reassembly.
+
+        Args:
+            strict: if return all datagrams (including those not
+                implemented) when submit
+
+        """
+        #: bool: Strict mode flag.
+        self._strflg = strict
+        #: bool: New datagram flag.
+        self._newflg = False
+
+        #: dict[IT, BT]: Dict buffer field.
+        self._buffer = {}  # type: dict[IT, BT]
+        #: list[DT]: List reassembled datagram.
+        self._dtgram = []  # type: list[DT]
+
+    def __call__(self, packet: 'PT') -> 'None':
+        """Call packet reassembly.
+
+        Arguments:
+            packet: packet dict to be reassembled
+                (detailed format described in corresponding protocol)
+
+        """
+        self._newflg = True
+        self.reassembly(packet)
```

### Comparing `pypcapkit-0.9.9rc3/pcapkit/toolkit/__init__.py` & `pypcapkit-1.0.0b1/pcapkit/toolkit/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 # -*- coding: utf-8 -*-
-"""capability tools
+# pylint: disable=unused-import, unused-wildcard-import
+"""Compatibility Tools
+=========================
 
-`pcapkit.toolkit` provides several utility functions for
-capability of multiple engine support.
+.. module:: pcapkit.toolkit
+
+:mod:`pcapkit.toolkit` provides several utility functions for
+compatibility of multiple engine support.
 
 """
 # tools for default engine
-from pcapkit.toolkit.default import *
-
-# tools for DPKT engine
-from pcapkit.toolkit.dpkt import ipv6_hdr_len as dpkt_ipv6_hdr_len
-from pcapkit.toolkit.dpkt import packet2chain as dpkt_packet2chain
-from pcapkit.toolkit.dpkt import packet2dict as dpkt_packet2dict
-from pcapkit.toolkit.dpkt import ipv4_reassembly as dpkt_ipv4_reassembly
-from pcapkit.toolkit.dpkt import ipv6_reassembly as dpkt_ipv6_reassembly
-from pcapkit.toolkit.dpkt import tcp_reassembly as dpkt_tcp_reassembly
-from pcapkit.toolkit.dpkt import tcp_traceflow as dpkt_tcp_traceflow
-
-# tools for PyShark engine
-from pcapkit.toolkit.pyshark import packet2dict as pyshark_packet2dict
-from pcapkit.toolkit.pyshark import tcp_traceflow as pyshark_tcp_traceflow
-
-# tools for Scapy engine
-from pcapkit.toolkit.scapy import packet2chain as scapy_packet2chain
-from pcapkit.toolkit.scapy import packet2dict as scapy_packet2dict
-from pcapkit.toolkit.scapy import ipv4_reassembly as scapy_ipv4_reassembly
-from pcapkit.toolkit.scapy import ipv6_reassembly as scapy_ipv6_reassembly
-from pcapkit.toolkit.scapy import tcp_reassembly as scapy_tcp_reassembly
-from pcapkit.toolkit.scapy import tcp_traceflow as scapy_tcp_traceflow
+from pcapkit.toolkit.default import ipv4_reassembly, ipv6_reassembly, tcp_reassembly, tcp_traceflow
 
+# # tools for DPKT engine
+# from pcapkit.toolkit.dpkt import ipv6_hdr_len as dpkt_ipv6_hdr_len
+# from pcapkit.toolkit.dpkt import packet2chain as dpkt_packet2chain
+# from pcapkit.toolkit.dpkt import packet2dict as dpkt_packet2dict
+# from pcapkit.toolkit.dpkt import ipv4_reassembly as dpkt_ipv4_reassembly
+# from pcapkit.toolkit.dpkt import ipv6_reassembly as dpkt_ipv6_reassembly
+# from pcapkit.toolkit.dpkt import tcp_reassembly as dpkt_tcp_reassembly
+# from pcapkit.toolkit.dpkt import tcp_traceflow as dpkt_tcp_traceflow
+
+# # tools for PyShark engine
+# from pcapkit.toolkit.pyshark import packet2dict as pyshark_packet2dict
+# from pcapkit.toolkit.pyshark import tcp_traceflow as pyshark_tcp_traceflow
+
+# # tools for Scapy engine
+# from pcapkit.toolkit.scapy import packet2chain as scapy_packet2chain
+# from pcapkit.toolkit.scapy import packet2dict as scapy_packet2dict
+# from pcapkit.toolkit.scapy import ipv4_reassembly as scapy_ipv4_reassembly
+# from pcapkit.toolkit.scapy import ipv6_reassembly as scapy_ipv6_reassembly
+# from pcapkit.toolkit.scapy import tcp_reassembly as scapy_tcp_reassembly
+# from pcapkit.toolkit.scapy import tcp_traceflow as scapy_tcp_traceflow
 
 __all__ = [
     # default engine
     'ipv4_reassembly', 'ipv6_reassembly', 'tcp_reassembly', 'tcp_traceflow',
 
-    # DPKT engine
-    'dpkt_ipv6_hdr_len', 'dpkt_packet2chain', 'dpkt_packet2dict',
-    'dpkt_ipv4_reassembly', 'dpkt_ipv6_reassembly', 'dpkt_tcp_reassembly', 'dpkt_tcp_traceflow',
-
-    # PyShark engine
-    'pyshark_packet2dict', 'pyshark_tcp_traceflow',
-
-    # Scapy engine
-    'scapy_packet2chain', 'scapy_packet2dict',
-    'scapy_ipv4_reassembly', 'scapy_ipv6_reassembly', 'scapy_tcp_reassembly', 'scapy_tcp_traceflow',
+    # # DPKT engine
+    # 'dpkt_ipv6_hdr_len', 'dpkt_packet2chain', 'dpkt_packet2dict',
+    # 'dpkt_ipv4_reassembly', 'dpkt_ipv6_reassembly', 'dpkt_tcp_reassembly', 'dpkt_tcp_traceflow',
+
+    # # PyShark engine
+    # 'pyshark_packet2dict', 'pyshark_tcp_traceflow',
+
+    # # Scapy engine
+    # 'scapy_packet2chain', 'scapy_packet2dict',
+    # 'scapy_ipv4_reassembly', 'scapy_ipv6_reassembly', 'scapy_tcp_reassembly', 'scapy_tcp_traceflow',
 ]
```

