# Comparing `tmp/xia_scw_forward-0.0.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_forward-0.0.2-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 111560 bytes, number of entries: 12
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-21 19:27 xia_scw_forward/__init__.py
--rw-r--r--  2.0 unx   259072 b- defN 23-Apr-21 19:30 xia_scw_forward/forward.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 19:27 xia_scw_forward/templates/ScwForward/backend.tf
--rw-rw-rw-  2.0 unx     2567 b- defN 23-Apr-21 19:27 xia_scw_forward/templates/ScwForward/main.tf
--rw-rw-rw-  2.0 unx      708 b- defN 23-Apr-21 19:27 xia_scw_forward/templates/ScwForward/output.tf
--rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 19:27 xia_scw_forward/templates/ScwForward/provider.tf
--rw-rw-rw-  2.0 unx     2386 b- defN 23-Apr-21 19:27 xia_scw_forward/templates/ScwForward/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-21 19:30 xia_scw_forward-0.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      727 b- defN 23-Apr-21 19:30 xia_scw_forward-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-21 19:30 xia_scw_forward-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-21 19:30 xia_scw_forward-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1127 b- defN 23-Apr-21 19:30 xia_scw_forward-0.0.1.dist-info/RECORD
-12 files, 267369 bytes uncompressed, 109614 bytes compressed:  59.0%
+Zip file size: 89106 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-21 21:46 xia_scw_forward/__init__.py
+-rw-r--r--  2.0 unx   235496 b- defN 23-Apr-21 21:47 xia_scw_forward/forward.cpython-310-darwin.so
+-rw-r--r--  2.0 unx       69 b- defN 23-Apr-21 19:28 xia_scw_forward/templates/ScwForward/backend.tf
+-rw-r--r--  2.0 unx     2631 b- defN 23-Apr-21 21:46 xia_scw_forward/templates/ScwForward/main.tf
+-rw-r--r--  2.0 unx      708 b- defN 23-Apr-21 19:28 xia_scw_forward/templates/ScwForward/output.tf
+-rw-r--r--  2.0 unx      343 b- defN 23-Apr-21 19:28 xia_scw_forward/templates/ScwForward/provider.tf
+-rw-r--r--  2.0 unx     2451 b- defN 23-Apr-21 21:46 xia_scw_forward/templates/ScwForward/variables.tf
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-21 21:47 xia_scw_forward-0.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      690 b- defN 23-Apr-21 21:47 xia_scw_forward-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-21 21:47 xia_scw_forward-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-21 21:47 xia_scw_forward-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1131 b- defN 23-Apr-21 21:47 xia_scw_forward-0.0.2.dist-info/RECORD
+12 files, 243898 bytes uncompressed, 87154 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: xia_scw_forward/__init__.py
 Comment: 
 
-Filename: xia_scw_forward/forward.cp39-win_amd64.pyd
+Filename: xia_scw_forward/forward.cpython-310-darwin.so
 Comment: 
 
 Filename: xia_scw_forward/templates/ScwForward/backend.tf
 Comment: 
 
 Filename: xia_scw_forward/templates/ScwForward/main.tf
 Comment: 
@@ -15,23 +15,23 @@
 
 Filename: xia_scw_forward/templates/ScwForward/provider.tf
 Comment: 
 
 Filename: xia_scw_forward/templates/ScwForward/variables.tf
 Comment: 
 
-Filename: xia_scw_forward-0.0.1.dist-info/LICENSE.txt
+Filename: xia_scw_forward-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_forward-0.0.1.dist-info/METADATA
+Filename: xia_scw_forward-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_forward-0.0.1.dist-info/WHEEL
+Filename: xia_scw_forward-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_forward-0.0.1.dist-info/top_level.txt
+Filename: xia_scw_forward-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_forward-0.0.1.dist-info/RECORD
+Filename: xia_scw_forward-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_forward/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_forward.forward import ScwForward
 
 
 __all__ = [
     "ScwForward"
 ]
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## xia_scw_forward/templates/ScwForward/main.tf

```diff
@@ -36,16 +36,20 @@
     gateway_id = data.scaleway_vpc_public_gateway.main.id
     private_ip = var.lan_ip
     private_port = var.lan_port
     public_port = var.wan_port
     protocol = "tcp"
     depends_on = [scaleway_vpc_public_gateway_dhcp_reservation.main]
 }
-/*
+
 locals {
+  default_ssh = [
+    "ufw allow ssh",
+    "ufw --force enable"
+  ]
   add_new_rules = [
     for ip in var.allowed_ips : "ufw allow from ${ip} to any port ${var.lan_port}"
   ]
   network_ips = [
     for ip in var.allowed_ips : (
       can(cidrnetmask(ip)) ? cidrsubnet(ip, 0, 0) : ip
     )
@@ -71,20 +75,20 @@
       local.add_new_rules,
       ["for ip in $(ufw status | grep '${var.lan_port}' | awk '{print $3}'); do if ! echo \"${join(" ", local.network_ips)}\" | grep -q -w \"$ip\"; then ufw delete allow from $ip to any port 27017; fi; done"]
     )
 
     connection {
       type        = "ssh"
       user        = "root"
-      private_key = file("tpi-cloud-dev-01.ssh")
+      private_key = file(var.ssh_private_key)
       host        = var.lan_ip
 
-      bastion_host        = var.wan_ip
+      bastion_host        = "212.47.239.148"
       bastion_port        = 59999
       bastion_user        = "bastion"
-      bastion_private_key = file("tpi-cloud-dev-01.ssh")
+      bastion_private_key = file(var.ssh_private_key)
 
       timeout              = "5m"   # Maximum time to wait for the connection to become available
     }
   }
 }
-*/
+
```

## xia_scw_forward/templates/ScwForward/variables.tf

```diff
@@ -74,7 +74,12 @@
           can(regex("^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)/(?:3[0-2]|[12]?[0-9])$", ip))
         )
       ])
     )
     error_message = "Each element of the allowed_ip variable must be a valid IPv4 address or an IPv4 address with a subnet mask."
   }
 }
+
+variable "ssh_private_key" {
+  type = string
+  default = null
+}
```

## Comparing `xia_scw_forward-0.0.1.dist-info/RECORD` & `xia_scw_forward-0.0.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_scw_forward/__init__.py,sha256=9bstekf-kH92bcm2NQt0eGYyh7PypT3YrGqIQ-wVB0U,103
-xia_scw_forward/forward.cp39-win_amd64.pyd,sha256=J5WeX8cHf6FZswLiZNeLY4Q28xWtaxzW6oTiZZ2-OdE,259072
+xia_scw_forward/__init__.py,sha256=C7vLuSciY7sCajiTNG-3pOPPJYBcnigfy6BElk68p7I,103
+xia_scw_forward/forward.cpython-310-darwin.so,sha256=XOfstwE7F9EWdZbt-DU_1d4k7fdqpZJ3pMSoRPFM6fY,235496
 xia_scw_forward/templates/ScwForward/backend.tf,sha256=E6fgAX-nMcTt9oErRKvK67uJPdB-O77YJpzAvf06zgs,69
-xia_scw_forward/templates/ScwForward/main.tf,sha256=1V3TSmRtKaegIDbRXGf3f13x36tEGrDO2dMN6uJ_Luc,2567
+xia_scw_forward/templates/ScwForward/main.tf,sha256=R8SaL521GrPhdJGcCpODjfwrPfWT6YbL0DcHsJ8Bh20,2631
 xia_scw_forward/templates/ScwForward/output.tf,sha256=nREGFAc1hXpAdRGd04io4QsRo28FX-EwgjFNg1PI4aU,708
 xia_scw_forward/templates/ScwForward/provider.tf,sha256=h_zFGas7QtYJPGvufLGuPHtgDhoZa28Qa5t--1dpheI,343
-xia_scw_forward/templates/ScwForward/variables.tf,sha256=kqVfO6iti5HPmGKvHKx4C59zosNLHXmV5Tkxom5c7mM,2386
-xia_scw_forward-0.0.1.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
-xia_scw_forward-0.0.1.dist-info/METADATA,sha256=MBpjRa8cl32YwyrrJkWU8toHg1ghM3LRrgRjW8pSQsk,727
-xia_scw_forward-0.0.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_forward-0.0.1.dist-info/top_level.txt,sha256=zSdl1uiLifiOddj8F4TdDzODhdXe_Ny7s_A4Dfprpw0,16
-xia_scw_forward-0.0.1.dist-info/RECORD,,
+xia_scw_forward/templates/ScwForward/variables.tf,sha256=gXB-8PH9d91xwJNg6dRt_KEPPQizfoZOLxO6E1exba4,2451
+xia_scw_forward-0.0.2.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
+xia_scw_forward-0.0.2.dist-info/METADATA,sha256=SicquyvDpnIvP-UGBFsbHlrSnHlR5nPfCnR8lT4uqb0,690
+xia_scw_forward-0.0.2.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_scw_forward-0.0.2.dist-info/top_level.txt,sha256=zSdl1uiLifiOddj8F4TdDzODhdXe_Ny7s_A4Dfprpw0,16
+xia_scw_forward-0.0.2.dist-info/RECORD,,
```

