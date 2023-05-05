# Comparing `tmp/xia_scw_instance-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_instance-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 141541 bytes, number of entries: 11
--rw-r--r--  2.0 unx      133 b- defN 23-May-04 16:55 xia_scw_instance/__init__.py
--rw-r--r--  2.0 unx   335360 b- defN 23-May-04 17:05 xia_scw_instance/instance.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx     3518 b- defN 23-May-03 09:32 xia_scw_instance/templates/ScwInstance/main.tf
--rw-rw-rw-  2.0 unx      931 b- defN 23-May-04 16:55 xia_scw_instance/templates/ScwInstance/output.tf
+Zip file size: 142884 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      133 b- defN 23-May-05 14:46 xia_scw_instance/__init__.py
+-rw-r--r--  2.0 unx   338944 b- defN 23-May-05 15:01 xia_scw_instance/instance.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx     3597 b- defN 23-May-05 08:06 xia_scw_instance/templates/ScwInstance/main.tf
+-rw-rw-rw-  2.0 unx     1025 b- defN 23-May-05 08:10 xia_scw_instance/templates/ScwInstance/output.tf
 -rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/provider.tf
--rw-rw-rw-  2.0 unx     4919 b- defN 23-May-03 09:32 xia_scw_instance/templates/ScwInstance/variables.tf
--rw-rw-rw-  2.0 unx      150 b- defN 23-May-04 17:05 xia_scw_instance-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      693 b- defN 23-May-04 17:05 xia_scw_instance-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-04 17:05 xia_scw_instance-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-04 17:05 xia_scw_instance-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1041 b- defN 23-May-04 17:05 xia_scw_instance-0.1.1.dist-info/RECORD
-11 files, 347204 bytes uncompressed, 139733 bytes compressed:  59.8%
+-rw-rw-rw-  2.0 unx     5100 b- defN 23-May-05 08:06 xia_scw_instance/templates/ScwInstance/variables.tf
+-rw-rw-rw-  2.0 unx      150 b- defN 23-May-05 15:01 xia_scw_instance-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      693 b- defN 23-May-05 15:01 xia_scw_instance-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-05 15:01 xia_scw_instance-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-05 15:01 xia_scw_instance-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1042 b- defN 23-May-05 15:01 xia_scw_instance-0.1.3.dist-info/RECORD
+11 files, 351143 bytes uncompressed, 141076 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: xia_scw_instance/templates/ScwInstance/provider.tf
 Comment: 
 
 Filename: xia_scw_instance/templates/ScwInstance/variables.tf
 Comment: 
 
-Filename: xia_scw_instance-0.1.1.dist-info/LICENSE.txt
+Filename: xia_scw_instance-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_instance-0.1.1.dist-info/METADATA
+Filename: xia_scw_instance-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_instance-0.1.1.dist-info/WHEEL
+Filename: xia_scw_instance-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_instance-0.1.1.dist-info/top_level.txt
+Filename: xia_scw_instance-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_instance-0.1.1.dist-info/RECORD
+Filename: xia_scw_instance-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_instance/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_instance.instance import ScwInstance, ScwForward
 
 
 __all__ = [
     "ScwInstance", "ScwForward"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.3"
```

## xia_scw_instance/templates/ScwInstance/main.tf

```diff
@@ -12,14 +12,20 @@
 }
 
 resource "scaleway_instance_server" "instance" {
   name  = var.name
   zone  = var.zone
   type  = var.type
   image = data.scaleway_instance_image.my_image.id
+
+  root_volume {
+    volume_type = "b_ssd"
+    size_in_gb = var.root_size
+  }
+
   tags  = var.tags
   state = var.state == "maintenance" ? "started" : var.state
 }
 
 
 data "scaleway_vpc_public_gateway" "main" {
   zone = var.zone
```

## xia_scw_instance/templates/ScwInstance/output.tf

```diff
@@ -10,14 +10,18 @@
   value = scaleway_instance_server.instance.zone
 }
 
 output "type" {
   value = scaleway_instance_server.instance.type
 }
 
+output "root_size" {
+  value = scaleway_instance_server.instance.root_volume[0].size_in_gb
+}
+
 output "image" {
   value = data.scaleway_instance_image.my_image.name
 }
 
 output "state" {
   value = scaleway_instance_server.instance.state
 }
```

## xia_scw_instance/templates/ScwInstance/variables.tf

```diff
@@ -29,14 +29,21 @@
 variable "type" {
   type = string
   default = null  #xia#
   #xia# default = {% if type is defined and type is not none %}"{{ type }}"{% else %}null{% endif %}
 
 }
 
+variable "root_size" {
+  type = string
+  default = null  #xia#
+  #xia# default = {% if root_size is defined and root_size is not none %}{{ root_size }}{% else %}null{% endif %}
+
+}
+
 variable "image" {
   type = string
   default = null  #xia#
   #xia# default = {% if image is defined and image is not none %}"{{ image }}"{% else %}null{% endif %}
 
 }
```

## Comparing `xia_scw_instance-0.1.1.dist-info/METADATA` & `xia_scw_instance-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-scw-instance
-Version: 0.1.1
+Version: 0.1.3
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.1.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.1.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_scw_instance-0.1.1.dist-info/RECORD` & `xia_scw_instance-0.1.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-xia_scw_instance/__init__.py,sha256=0X5RFl6_I3kRBuADQmXdg1dAdJAPQQVySGJ4DC6WeYk,133
-xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=eGnCVzbe2A7g71YTJHp_HWuwg3hkTby6Vtr_stLPhEE,335360
-xia_scw_instance/templates/ScwInstance/main.tf,sha256=QVktoXI4so6JjCEsAoWx3YYSrNB1ZMZte82A4-ciiD0,3518
-xia_scw_instance/templates/ScwInstance/output.tf,sha256=AF537TgCRawA_5eATAwdly8PbpLdk3uXn59Dbt2TpiY,931
+xia_scw_instance/__init__.py,sha256=E9OffodOkdJYAqv5s1Z46it322jbgRUPp5wr8aW-oNU,133
+xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=Kv6UahPZzJJ90purPbBc7pw0VGYHXNXGoSruY0rwF1w,338944
+xia_scw_instance/templates/ScwInstance/main.tf,sha256=w4WG7u11Q07ffNsKdeC9Zp2L6kE3QkZd3_0AKgDfbog,3597
+xia_scw_instance/templates/ScwInstance/output.tf,sha256=y6KYVxZ8ypYlimYkuYPb1QXB0mdSu5SJYKpF0ZsSpxU,1025
 xia_scw_instance/templates/ScwInstance/provider.tf,sha256=h_zFGas7QtYJPGvufLGuPHtgDhoZa28Qa5t--1dpheI,343
-xia_scw_instance/templates/ScwInstance/variables.tf,sha256=e4dj7oe4zKHcOjIXFmJqQJB8iodQvsQ9HwvnIBKoFDA,4919
-xia_scw_instance-0.1.1.dist-info/LICENSE.txt,sha256=2HzK8y__YhkYAEzI5V38DGwiVGnADL74BLH_dyBEs7I,150
-xia_scw_instance-0.1.1.dist-info/METADATA,sha256=DefZ10GQi2DIJV03ekKrLHU8WBjOtxvbuULOyIz7QgU,693
-xia_scw_instance-0.1.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_instance-0.1.1.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
-xia_scw_instance-0.1.1.dist-info/RECORD,,
+xia_scw_instance/templates/ScwInstance/variables.tf,sha256=UiHAbJOzMF-2zOga1lagT7GkhFQ469-PDoEEDzgL8Wg,5100
+xia_scw_instance-0.1.3.dist-info/LICENSE.txt,sha256=2HzK8y__YhkYAEzI5V38DGwiVGnADL74BLH_dyBEs7I,150
+xia_scw_instance-0.1.3.dist-info/METADATA,sha256=A8wTgPD2f-VptxyLKQInpRvRPQLhsCMo8WY75i80Afs,693
+xia_scw_instance-0.1.3.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_scw_instance-0.1.3.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
+xia_scw_instance-0.1.3.dist-info/RECORD,,
```

