# Comparing `tmp/micropython_esp32_stubs-1.19.1.post9.tar.gz` & `tmp/micropython_esp32_stubs-1.20.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_esp32_stubs-1.19.1.post9.tar", max compression
+gzip compressed data, was "micropython_esp32_stubs-1.20.0.post1.tar", max compression
```

## Comparing `micropython_esp32_stubs-1.19.1.post9.tar` & `micropython_esp32_stubs-1.20.0.post1.tar`

### file list

```diff
@@ -1,86 +1,90 @@
--rw-r--r--   0        0        0     1070 2023-01-16 00:27:39.469365 micropython_esp32_stubs-1.19.1.post9/LICENSE.md
--rw-r--r--   0        0        0     2038 2023-01-16 00:27:39.465365 micropython_esp32_stubs-1.19.1.post9/README.md
--rw-r--r--   0        0        0       50 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/_boot.pyi
--rw-r--r--   0        0        0      269 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/_onewire.pyi
--rw-r--r--   0        0        0      825 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/_thread.pyi
--rw-r--r--   0        0        0      353 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/_uasyncio.pyi
--rw-r--r--   0        0        0      110 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/apa106.pyi
--rw-r--r--   0        0        0     1017 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/array.pyi
--rw-r--r--   0        0        0     1365 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/binascii.pyi
--rw-r--r--   0        0        0     3670 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/btree.pyi
--rw-r--r--   0        0        0     1385 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/cmath.pyi
--rw-r--r--   0        0        0      329 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/dht.pyi
--rw-r--r--   0        0        0      389 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/ds18x20.pyi
--rw-r--r--   0        0        0      676 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/errno.pyi
--rw-r--r--   0        0        0     1700 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/esp.pyi
--rw-r--r--   0        0        0    11743 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/esp32.pyi
--rw-r--r--   0        0        0       51 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/flashbdev.pyi
--rw-r--r--   0        0        0     4787 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/framebuf.pyi
--rw-r--r--   0        0        0     1935 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/gc.pyi
--rw-r--r--   0        0        0     1600 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/hashlib.pyi
--rw-r--r--   0        0        0      897 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/heapq.pyi
--rw-r--r--   0        0        0       74 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/inisetup.pyi
--rw-r--r--   0        0        0     3914 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/io.pyi
--rw-r--r--   0        0        0     1339 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/json.pyi
--rw-r--r--   0        0        0    48110 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/machine.pyi
--rw-r--r--   0        0        0     4400 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/math.pyi
--rw-r--r--   0        0        0     7055 2023-01-16 00:27:02.873534 micropython_esp32_stubs-1.19.1.post9/micropython.pyi
--rw-r--r--   0        0        0      433 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/neopixel.pyi
--rw-r--r--   0        0        0     9921 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/network.pyi
--rw-r--r--   0        0        0       69 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/ntptime.pyi
--rw-r--r--   0        0        0      596 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/onewire.pyi
--rw-r--r--   0        0        0     9111 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/os.pyi
--rw-r--r--   0        0        0      157 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/platform.pyi
--rw-r--r--   0        0        0     3907 2023-01-16 00:27:40.001362 micropython_esp32_stubs-1.19.1.post9/pyproject.toml
--rw-r--r--   0        0        0     2553 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/random.pyi
--rw-r--r--   0        0        0     3760 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/select.pyi
--rw-r--r--   0        0        0     9375 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/socket.pyi
--rw-r--r--   0        0        0     1836 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/ssl.pyi
--rw-r--r--   0        0        0     1521 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/struct.pyi
--rw-r--r--   0        0        0      838 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/sys.pyi
--rw-r--r--   0        0        0    12180 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/time.pyi
--rw-r--r--   0        0        0     1017 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/uarray.pyi
--rw-r--r--   0        0        0      125 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/uasyncio/__init__.pyi
--rw-r--r--   0        0        0     1478 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/uasyncio/core.pyi
--rw-r--r--   0        0        0      577 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/uasyncio/event.pyi
--rw-r--r--   0        0        0      377 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/uasyncio/funcs.pyi
--rw-r--r--   0        0        0      407 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/uasyncio/lock.pyi
--rw-r--r--   0        0        0     1394 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/uasyncio/stream.pyi
--rw-r--r--   0        0        0      760 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/uasyncio/task.pyi
--rw-r--r--   0        0        0     1365 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/ubinascii.pyi
--rw-r--r--   0        0        0    29040 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/ubluetooth.pyi
--rw-r--r--   0        0        0     3526 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/ucollections.pyi
--rw-r--r--   0        0        0     1608 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/ucryptolib.pyi
--rw-r--r--   0        0        0     2277 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/uctypes.pyi
--rw-r--r--   0        0        0      676 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/uerrno.pyi
--rw-r--r--   0        0        0     1600 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/uhashlib.pyi
--rw-r--r--   0        0        0      897 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/uheapq.pyi
--rw-r--r--   0        0        0     3914 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/uio.pyi
--rw-r--r--   0        0        0     1339 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/ujson.pyi
--rw-r--r--   0        0        0    48110 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/umachine.pyi
--rw-r--r--   0        0        0        0 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/umqtt/__init__.pyi
--rw-r--r--   0        0        0      648 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/umqtt/robust.pyi
--rw-r--r--   0        0        0      649 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/umqtt/simple.pyi
--rw-r--r--   0        0        0     9111 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/uos.pyi
--rw-r--r--   0        0        0      717 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/upip.pyi
--rw-r--r--   0        0        0      689 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/upip_utarfile.pyi
--rw-r--r--   0        0        0      157 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/uplatform.pyi
--rw-r--r--   0        0        0     2553 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/urandom.pyi
--rw-r--r--   0        0        0      181 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/ure.pyi
--rw-r--r--   0        0        0      492 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/urequests.pyi
--rw-r--r--   0        0        0     3760 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/uselect.pyi
--rw-r--r--   0        0        0     9375 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/usocket.pyi
--rw-r--r--   0        0        0     1836 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/ussl.pyi
--rw-r--r--   0        0        0     1521 2023-01-16 00:27:03.153533 micropython_esp32_stubs-1.19.1.post9/ustruct.pyi
--rw-r--r--   0        0        0      838 2023-01-16 00:27:03.157533 micropython_esp32_stubs-1.19.1.post9/usys.pyi
--rw-r--r--   0        0        0    12180 2023-01-16 00:27:03.157533 micropython_esp32_stubs-1.19.1.post9/utime.pyi
--rw-r--r--   0        0        0      238 2023-01-16 00:27:03.157533 micropython_esp32_stubs-1.19.1.post9/utimeq.pyi
--rw-r--r--   0        0        0      393 2023-01-16 00:27:03.157533 micropython_esp32_stubs-1.19.1.post9/uwebsocket.pyi
--rw-r--r--   0        0        0     1503 2023-01-16 00:27:03.157533 micropython_esp32_stubs-1.19.1.post9/uzlib.pyi
--rw-r--r--   0        0        0      366 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/webrepl.pyi
--rw-r--r--   0        0        0      222 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/webrepl_setup.pyi
--rw-r--r--   0        0        0      393 2023-01-16 00:27:03.157533 micropython_esp32_stubs-1.19.1.post9/websocket.pyi
--rw-r--r--   0        0        0       92 2023-01-16 00:27:03.165533 micropython_esp32_stubs-1.19.1.post9/websocket_helper.pyi
--rw-r--r--   0        0        0     1503 2023-01-16 00:27:03.157533 micropython_esp32_stubs-1.19.1.post9/zlib.pyi
--rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 micropython_esp32_stubs-1.19.1.post9/setup.py
--rw-r--r--   0        0        0     3327 1970-01-01 00:00:00.000000 micropython_esp32_stubs-1.19.1.post9/PKG-INFO
+-rw-r--r--   0        0        0       53 2023-05-05 19:49:06.160838 micropython_esp32_stubs-1.20.0.post1/_boot.pyi
+-rw-r--r--   0        0        0      277 2023-05-05 20:22:59.220054 micropython_esp32_stubs-1.20.0.post1/_onewire.pyi
+-rw-r--r--   0        0        0      848 2023-05-05 20:23:06.206407 micropython_esp32_stubs-1.20.0.post1/_thread.pyi
+-rw-r--r--   0        0        0      364 2023-05-05 20:22:59.228399 micropython_esp32_stubs-1.20.0.post1/_uasyncio.pyi
+-rw-r--r--   0        0        0      115 2023-05-05 19:49:06.163754 micropython_esp32_stubs-1.20.0.post1/apa106.pyi
+-rw-r--r--   0        0        0     1003 2023-05-05 20:23:25.942461 micropython_esp32_stubs-1.20.0.post1/array.pyi
+-rw-r--r--   0        0        0     1408 2023-05-05 20:23:26.029016 micropython_esp32_stubs-1.20.0.post1/binascii.pyi
+-rw-r--r--   0        0        0    31291 2023-05-05 20:23:26.116139 micropython_esp32_stubs-1.20.0.post1/bluetooth.pyi
+-rw-r--r--   0        0        0     3837 2023-05-05 20:23:07.461038 micropython_esp32_stubs-1.20.0.post1/btree.pyi
+-rw-r--r--   0        0        0     1454 2023-05-05 20:23:26.163497 micropython_esp32_stubs-1.20.0.post1/cmath.pyi
+-rw-r--r--   0        0        0     3640 2023-05-05 20:23:26.161452 micropython_esp32_stubs-1.20.0.post1/collections.pyi
+-rw-r--r--   0        0        0     1647 2023-05-05 20:23:08.299942 micropython_esp32_stubs-1.20.0.post1/cryptolib.pyi
+-rw-r--r--   0        0        0      344 2023-05-05 19:49:06.167790 micropython_esp32_stubs-1.20.0.post1/dht.pyi
+-rw-r--r--   0        0        0      404 2023-05-05 19:49:06.170625 micropython_esp32_stubs-1.20.0.post1/ds18x20.pyi
+-rw-r--r--   0        0        0      709 2023-05-05 20:23:08.509119 micropython_esp32_stubs-1.20.0.post1/errno.pyi
+-rw-r--r--   0        0        0     1703 2023-05-05 20:23:26.202466 micropython_esp32_stubs-1.20.0.post1/esp.pyi
+-rw-r--r--   0        0        0    12242 2023-05-05 20:23:26.332028 micropython_esp32_stubs-1.20.0.post1/esp32.pyi
+-rw-r--r--   0        0        0       54 2023-05-05 19:49:06.172981 micropython_esp32_stubs-1.20.0.post1/flashbdev.pyi
+-rw-r--r--   0        0        0     6349 2023-05-05 20:23:26.258860 micropython_esp32_stubs-1.20.0.post1/framebuf.pyi
+-rw-r--r--   0        0        0     1993 2023-05-05 20:23:26.246651 micropython_esp32_stubs-1.20.0.post1/gc.pyi
+-rw-r--r--   0        0        0     1642 2023-05-05 20:23:26.258860 micropython_esp32_stubs-1.20.0.post1/hashlib.pyi
+-rw-r--r--   0        0        0      930 2023-05-05 20:23:26.279660 micropython_esp32_stubs-1.20.0.post1/heapq.pyi
+-rw-r--r--   0        0        0       77 2023-05-05 19:49:06.175994 micropython_esp32_stubs-1.20.0.post1/inisetup.pyi
+-rw-r--r--   0        0        0     2650 2023-05-05 20:23:26.364596 micropython_esp32_stubs-1.20.0.post1/io.pyi
+-rw-r--r--   0        0        0     1384 2023-05-05 20:23:26.291952 micropython_esp32_stubs-1.20.0.post1/json.pyi
+-rw-r--r--   0        0        0     1092 2023-05-05 20:31:11.115559 micropython_esp32_stubs-1.20.0.post1/LICENSE.md
+-rw-r--r--   0        0        0      827 2023-05-05 20:22:59.278622 micropython_esp32_stubs-1.20.0.post1/logging.pyi
+-rw-r--r--   0        0        0    52352 2023-05-05 20:23:29.666884 micropython_esp32_stubs-1.20.0.post1/machine.pyi
+-rw-r--r--   0        0        0     4654 2023-05-05 20:23:26.479425 micropython_esp32_stubs-1.20.0.post1/math.pyi
+-rw-r--r--   0        0        0     7213 2023-04-05 11:07:45.360315 micropython_esp32_stubs-1.20.0.post1/micropython.pyi
+-rw-r--r--   0        0        0      598 2023-05-05 19:51:58.147437 micropython_esp32_stubs-1.20.0.post1/mip/__init__.pyi
+-rw-r--r--   0        0        0       68 2023-05-05 20:22:59.278622 micropython_esp32_stubs-1.20.0.post1/mip.pyi
+-rw-r--r--   0        0        0      448 2023-05-05 19:49:06.179674 micropython_esp32_stubs-1.20.0.post1/neopixel.pyi
+-rw-r--r--   0        0        0    10529 2023-05-05 20:23:26.560051 micropython_esp32_stubs-1.20.0.post1/network.pyi
+-rw-r--r--   0        0        0       72 2023-05-05 19:49:06.185571 micropython_esp32_stubs-1.20.0.post1/ntptime.pyi
+-rw-r--r--   0        0        0      617 2023-05-05 19:49:06.192533 micropython_esp32_stubs-1.20.0.post1/onewire.pyi
+-rw-r--r--   0        0        0     9356 2023-05-05 20:23:26.672646 micropython_esp32_stubs-1.20.0.post1/os.pyi
+-rw-r--r--   0        0        0      162 2023-05-05 20:22:59.295467 micropython_esp32_stubs-1.20.0.post1/platform.pyi
+-rw-r--r--   0        0        0     4034 2023-05-05 20:31:13.441563 micropython_esp32_stubs-1.20.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     2638 2023-05-05 20:23:26.583649 micropython_esp32_stubs-1.20.0.post1/random.pyi
+-rw-r--r--   0        0        0     2011 2023-05-05 20:31:11.114544 micropython_esp32_stubs-1.20.0.post1/README.md
+-rw-r--r--   0        0        0     3853 2023-05-05 20:23:15.774982 micropython_esp32_stubs-1.20.0.post1/select.pyi
+-rw-r--r--   0        0        0     9602 2023-05-05 20:23:26.730375 micropython_esp32_stubs-1.20.0.post1/socket.pyi
+-rw-r--r--   0        0        0     2668 2023-05-05 20:23:26.688689 micropython_esp32_stubs-1.20.0.post1/ssl.pyi
+-rw-r--r--   0        0        0     4241 2023-05-05 20:23:26.761968 micropython_esp32_stubs-1.20.0.post1/struct.pyi
+-rw-r--r--   0        0        0      875 2023-05-05 20:23:26.737644 micropython_esp32_stubs-1.20.0.post1/sys.pyi
+-rw-r--r--   0        0        0    12515 2023-05-05 20:23:26.805066 micropython_esp32_stubs-1.20.0.post1/time.pyi
+-rw-r--r--   0        0        0     1003 2023-05-05 20:23:26.788193 micropython_esp32_stubs-1.20.0.post1/uarray.pyi
+-rw-r--r--   0        0        0      132 2023-05-05 19:49:06.046649 micropython_esp32_stubs-1.20.0.post1/uasyncio/__init__.pyi
+-rw-r--r--   0        0        0     1530 2023-05-05 19:49:06.047659 micropython_esp32_stubs-1.20.0.post1/uasyncio/core.pyi
+-rw-r--r--   0        0        0      625 2023-05-05 19:49:06.055187 micropython_esp32_stubs-1.20.0.post1/uasyncio/event.pyi
+-rw-r--r--   0        0        0      390 2023-05-05 19:49:06.060787 micropython_esp32_stubs-1.20.0.post1/uasyncio/funcs.pyi
+-rw-r--r--   0        0        0      414 2023-05-05 19:49:06.060787 micropython_esp32_stubs-1.20.0.post1/uasyncio/lock.pyi
+-rw-r--r--   0        0        0     1410 2023-05-05 19:51:58.349367 micropython_esp32_stubs-1.20.0.post1/uasyncio/stream.pyi
+-rw-r--r--   0        0        0      789 2023-05-05 19:49:06.084965 micropython_esp32_stubs-1.20.0.post1/uasyncio/task.pyi
+-rw-r--r--   0        0        0     1408 2023-05-05 20:23:26.891363 micropython_esp32_stubs-1.20.0.post1/ubinascii.pyi
+-rw-r--r--   0        0        0    31291 2023-05-05 20:23:27.051854 micropython_esp32_stubs-1.20.0.post1/ubluetooth.pyi
+-rw-r--r--   0        0        0     3640 2023-05-05 20:23:26.981894 micropython_esp32_stubs-1.20.0.post1/ucollections.pyi
+-rw-r--r--   0        0        0     1647 2023-05-05 20:23:18.641139 micropython_esp32_stubs-1.20.0.post1/ucryptolib.pyi
+-rw-r--r--   0        0        0     2363 2023-05-05 20:23:27.063883 micropython_esp32_stubs-1.20.0.post1/uctypes.pyi
+-rw-r--r--   0        0        0      709 2023-05-05 20:23:19.110558 micropython_esp32_stubs-1.20.0.post1/uerrno.pyi
+-rw-r--r--   0        0        0     1642 2023-05-05 20:23:27.055940 micropython_esp32_stubs-1.20.0.post1/uhashlib.pyi
+-rw-r--r--   0        0        0      930 2023-05-05 20:23:27.088447 micropython_esp32_stubs-1.20.0.post1/uheapq.pyi
+-rw-r--r--   0        0        0     2650 2023-05-05 20:23:27.155029 micropython_esp32_stubs-1.20.0.post1/uio.pyi
+-rw-r--r--   0        0        0     1384 2023-05-05 20:23:27.113374 micropython_esp32_stubs-1.20.0.post1/ujson.pyi
+-rw-r--r--   0        0        0    52352 2023-05-05 20:23:31.772392 micropython_esp32_stubs-1.20.0.post1/umachine.pyi
+-rw-r--r--   0        0        0        0 2023-05-05 19:49:06.127996 micropython_esp32_stubs-1.20.0.post1/umqtt/__init__.pyi
+-rw-r--r--   0        0        0      377 2023-05-05 19:49:06.127996 micropython_esp32_stubs-1.20.0.post1/umqtt/robust.pyi
+-rw-r--r--   0        0        0     1292 2023-05-05 19:51:58.397212 micropython_esp32_stubs-1.20.0.post1/umqtt/simple.pyi
+-rw-r--r--   0        0        0     9356 2023-05-05 20:23:27.332182 micropython_esp32_stubs-1.20.0.post1/uos.pyi
+-rw-r--r--   0        0        0      162 2023-05-05 20:22:59.331083 micropython_esp32_stubs-1.20.0.post1/uplatform.pyi
+-rw-r--r--   0        0        0      641 2023-05-05 19:49:06.211075 micropython_esp32_stubs-1.20.0.post1/upysh.pyi
+-rw-r--r--   0        0        0     2638 2023-05-05 20:23:27.212075 micropython_esp32_stubs-1.20.0.post1/urandom.pyi
+-rw-r--r--   0        0        0      187 2023-05-05 20:22:59.338712 micropython_esp32_stubs-1.20.0.post1/ure.pyi
+-rw-r--r--   0        0        0      739 2023-05-05 19:51:58.393263 micropython_esp32_stubs-1.20.0.post1/urequests.pyi
+-rw-r--r--   0        0        0     3853 2023-05-05 20:23:23.154717 micropython_esp32_stubs-1.20.0.post1/uselect.pyi
+-rw-r--r--   0        0        0     9602 2023-05-05 20:23:27.360579 micropython_esp32_stubs-1.20.0.post1/usocket.pyi
+-rw-r--r--   0        0        0     2668 2023-05-05 20:23:27.285085 micropython_esp32_stubs-1.20.0.post1/ussl.pyi
+-rw-r--r--   0        0        0     4241 2023-05-05 20:23:27.315416 micropython_esp32_stubs-1.20.0.post1/ustruct.pyi
+-rw-r--r--   0        0        0      875 2023-05-05 20:23:27.365511 micropython_esp32_stubs-1.20.0.post1/usys.pyi
+-rw-r--r--   0        0        0    12515 2023-05-05 20:23:27.446527 micropython_esp32_stubs-1.20.0.post1/utime.pyi
+-rw-r--r--   0        0        0      245 2023-05-05 20:22:59.351492 micropython_esp32_stubs-1.20.0.post1/utimeq.pyi
+-rw-r--r--   0        0        0      403 2023-05-05 20:22:59.351492 micropython_esp32_stubs-1.20.0.post1/uwebsocket.pyi
+-rw-r--r--   0        0        0     1535 2023-05-05 20:23:27.431524 micropython_esp32_stubs-1.20.0.post1/uzlib.pyi
+-rw-r--r--   0        0        0      513 2023-05-05 19:49:06.216864 micropython_esp32_stubs-1.20.0.post1/webrepl.pyi
+-rw-r--r--   0        0        0      232 2023-05-05 19:49:06.222477 micropython_esp32_stubs-1.20.0.post1/webrepl_setup.pyi
+-rw-r--r--   0        0        0      403 2023-05-05 20:22:59.357196 micropython_esp32_stubs-1.20.0.post1/websocket.pyi
+-rw-r--r--   0        0        0     1535 2023-05-05 20:23:27.462203 micropython_esp32_stubs-1.20.0.post1/zlib.pyi
+-rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 micropython_esp32_stubs-1.20.0.post1/setup.py
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 micropython_esp32_stubs-1.20.0.post1/PKG-INFO
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/README.md` & `micropython_esp32_stubs-1.20.0.post1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# micropython-esp32-stubs
-
-
-This is a stub-only package for MicroPython.
-It is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.
-
-The version of this package is alligned the the version of the MicroPython firmware.
- - Major, Minor and Patch levels are alligned to the same version as the firmware.  
- - The post release level is used to publish new releases of the stubs.
-
-For `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  
-for `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  
-
-To install the latest stubs:  
-`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.
-
-To install the stubs for an older version, such as MicroPython 1.17:  
-`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.
-
-
-As the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.
-To upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`
-
-If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
-
-For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
- * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
-
-Included stubs:
-* Merged stubs from `stubs/micropython-v1_19_1-esp32-merged`
-* Frozen stubs from `stubs/micropython-v1_19_1-frozen/esp32/GENERIC`
-* Core Stubs from `stubs/cpython_core-pycopy`
-
-
-origin | Family | Port | Board | Version
--------|--------|------|-------|--------
-Firmware | micropython | esp32 | ESP32 module (spiram) with ESP32 | v1.19.1 
-Documentation | micropython | - | - | v1.19.1 
-Core | micropython | esp32 | - | v1.19.1 
+# micropython-esp32-stubs
+
+
+This is a stub-only package for MicroPython.
+It is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.
+
+The version of this package is alligned the the version of the MicroPython firmware.
+ - Major, Minor and Patch levels are alligned to the same version as the firmware.  
+ - The post release level is used to publish new releases of the stubs.
+
+For `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  
+for `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  
+
+To install the latest stubs:  
+`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.
+
+To install the stubs for an older version, such as MicroPython 1.17:  
+`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.
+
+
+As the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.
+To upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`
+
+If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
+
+For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
+ * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
+
+Included stubs:
+* StubSource.MERGED from `stubs/micropython-v1_20_0-esp32-merged`
+* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
+* StubSource.CORE from `stubs/micropython-core`
+
+
+origin | Family | Port | Board | Version
+-------|--------|------|-------|--------
+Documentation | micropython | - | - | v1.20.0 
+Core | micropython | esp32 | - | v1.20.0
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/array.pyi` & `micropython_esp32_stubs-1.20.0.post1/array.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-"""
-efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.19.1/library/array.html
-
-|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
-
-Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
-``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
-floating-point support).
-"""
-from typing import Optional, Any
-
-class array:
-    """
-    Create array with elements of given type. Initial contents of the
-    array are given by *iterable*. If it is not provided, an empty
-    array is created.
-    """
-
-    def extend(self, iterable) -> Any:
-        """
-        Append new elements as contained in *iterable* to the end of
-        array, growing it.
-        """
-        ...
-    def decode(self, *args, **kwargs) -> Any: ...
-    def append(self, val) -> Any:
-        """
-        Append new element *val* to the end of array, growing it.
-        """
-        ...
-    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
+"""
+efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.20.0/library/array.html
+
+|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
+
+Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
+``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
+floating-point support).
+"""
+from typing import List, Optional, Any
+
+class array:
+    """
+    Create array with elements of given type. Initial contents of the
+    array are given by *iterable*. If it is not provided, an empty
+    array is created.
+    """
+
+    def extend(self, iterable) -> Any:
+        """
+        Append new elements as contained in *iterable* to the end of
+        array, growing it.
+        """
+        ...
+    def append(self, val) -> Any:
+        """
+        Append new element *val* to the end of array, growing it.
+        """
+        ...
+    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/binascii.pyi` & `micropython_esp32_stubs-1.20.0.post1/binascii.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""
-binary/ASCII conversions. See: https://docs.micropython.org/en/v1.19.1/library/binascii.html
-
-|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
-
-This module implements conversions between binary data and various
-encodings of it in ASCII form (in both directions).
-"""
-from typing import Optional, Any
-
-def crc32(*args, **kwargs) -> Any: ...
-def hexlify(data, sep: Optional[Any] = None) -> bytes:
-    """
-    Convert the bytes in the *data* object to a hexadecimal representation.
-    Returns a bytes object.
-
-    If the additional argument *sep* is supplied it is used as a separator
-    between hexadecimal values.
-    """
-    ...
-
-def unhexlify(data) -> bytes:
-    """
-    Convert hexadecimal data to binary representation. Returns bytes string.
-    (i.e. inverse of hexlify)
-    """
-    ...
-
-def b2a_base64(data, *, newline=True) -> bytes:
-    """
-    Encode binary data in base64 format, as in `RFC 3548
-    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
-    followed by a newline character if newline is true, as a bytes object.
-    """
-    ...
-
-def a2b_base64(data) -> bytes:
-    """
-    Decode base64-encoded data, ignoring invalid characters in the input.
-    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
-    Returns a bytes object.
-    """
-    ...
+"""
+binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20.0/library/binascii.html
+
+|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
+
+This module implements conversions between binary data and various
+encodings of it in ASCII form (in both directions).
+"""
+from typing import Optional, Any
+
+def crc32(*args, **kwargs) -> Any: ...
+def hexlify(data, sep: Optional[Any] = None) -> bytes:
+    """
+    Convert the bytes in the *data* object to a hexadecimal representation.
+    Returns a bytes object.
+
+    If the additional argument *sep* is supplied it is used as a separator
+    between hexadecimal values.
+    """
+    ...
+
+def unhexlify(data) -> bytes:
+    """
+    Convert hexadecimal data to binary representation. Returns bytes string.
+    (i.e. inverse of hexlify)
+    """
+    ...
+
+def b2a_base64(data, *, newline=True) -> bytes:
+    """
+    Encode binary data in base64 format, as in `RFC 3548
+    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
+    followed by a newline character if newline is true, as a bytes object.
+    """
+    ...
+
+def a2b_base64(data) -> bytes:
+    """
+    Decode base64-encoded data, ignoring invalid characters in the input.
+    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
+    Returns a bytes object.
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/btree.pyi` & `micropython_esp32_stubs-1.20.0.post1/btree.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,103 @@
-"""
-simple BTree database. See: https://docs.micropython.org/en/v1.19.1/library/btree.html
-
-The ``btree`` module implements a simple key-value database using external
-storage (disk files, or in general case, a random-access `stream`). Keys are
-stored sorted in the database, and besides efficient retrieval by a key
-value, a database also supports efficient ordered range scans (retrieval
-of values with the keys in a given range). On the application interface
-side, BTree database work as close a possible to a way standard `dict`
-type works, one notable difference is that both keys and values must
-be `bytes` objects (so, if you want to store objects of other types, you
-need to serialize them to `bytes` first).
-
-The module is based on the well-known BerkelyDB library, version 1.xx.
-
-Example::
-
-    import btree
-
-    # First, we need to open a stream which holds a database
-    # This is usually a file, but can be in-memory database
-    # using io.BytesIO, a raw flash partition, etc.
-    # Oftentimes, you want to create a database file if it doesn't
-    # exist and open if it exists. Idiom below takes care of this.
-    # DO NOT open database with "a+b" access mode.
-    try:
-        f = open("mydb", "r+b")
-    except OSError:
-        f = open("mydb", "w+b")
-
-    # Now open a database itself
-    db = btree.open(f)
-
-    # The keys you add will be sorted internally in the database
-    db[b"3"] = b"three"
-    db[b"1"] = b"one"
-    db[b"2"] = b"two"
-
-    # Assume that any changes are cached in memory unless
-    # explicitly flushed (or database closed). Flush database
-    # at the end of each "transaction".
-    db.flush()
-
-    # Prints b'two'
-    print(db[b"2"])
-
-    # Iterate over sorted keys in the database, starting from b"2"
-    # until the end of the database, returning only values.
-    # Mind that arguments passed to values() method are *key* values.
-    # Prints:
-    #   b'two'
-    #   b'three'
-    for word in db.values(b"2"):
-        print(word)
-
-    del db[b"2"]
-
-    # No longer true, prints False
-    print(b"2" in db)
-
-    # Prints:
-    #  b"1"
-    #  b"3"
-    for key in db:
-        print(key)
-
-    db.close()
-
-    # Don't forget to close the underlying stream!
-    f.close()
-
-"""
-from typing import Dict, Optional, Any
-
-DESC: int
-INCL: int
-
-def open(stream, *, flags=0, pagesize=0, cachesize=0, minkeypage=0) -> Dict:
-    """
-    Open a database from a random-access `stream` (like an open file). All
-    other parameters are optional and keyword-only, and allow to tweak advanced
-    parameters of the database operation (most users will not need them):
-
-    * *flags* - Currently unused.
-    * *pagesize* - Page size used for the nodes in BTree. Acceptable range
-      is 512-65536. If 0, a port-specific default will be used, optimized for
-      port's memory usage and/or performance.
-    * *cachesize* - Suggested memory cache size in bytes. For a
-      board with enough memory using larger values may improve performance.
-      Cache policy is as follows: entire cache is not allocated at once;
-      instead, accessing a new page in database will allocate a memory buffer
-      for it, until value specified by *cachesize* is reached. Then, these
-      buffers will be managed using LRU (least recently used) policy. More
-      buffers may still be allocated if needed (e.g., if a database contains
-      big keys and/or values). Allocated cache buffers aren't reclaimed.
-    * *minkeypage* - Minimum number of keys to store per page. Default value
-      of 0 equivalent to 2.
-
-    Returns a BTree object, which implements a dictionary protocol (set
-    of methods), and some additional methods described below.
-    """
-    ...
+"""
+simple BTree database. See: https://docs.micropython.org/en/v1.20.0/library/btree.html
+
+The ``btree`` module implements a simple key-value database using external
+storage (disk files, or in general case, a random-access `stream`). Keys are
+stored sorted in the database, and besides efficient retrieval by a key
+value, a database also supports efficient ordered range scans (retrieval
+of values with the keys in a given range). On the application interface
+side, BTree database work as close a possible to a way standard `dict`
+type works, one notable difference is that both keys and values must
+be `bytes`-like objects (so, if you want to store objects of other types, you
+need to first serialize them to `str` or `bytes` or another type that supports
+the buffer protocol).
+
+The module is based on the well-known BerkelyDB library, version 1.xx.
+
+Example::
+
+    import btree
+
+    # First, we need to open a stream which holds a database
+    # This is usually a file, but can be in-memory database
+    # using io.BytesIO, a raw flash partition, etc.
+    # Oftentimes, you want to create a database file if it doesn't
+    # exist and open if it exists. Idiom below takes care of this.
+    # DO NOT open database with "a+b" access mode.
+    try:
+        f = open("mydb", "r+b")
+    except OSError:
+        f = open("mydb", "w+b")
+
+    # Now open a database itself
+    db = btree.open(f)
+
+    # The keys you add will be sorted internally in the database
+    db[b"3"] = b"three"
+    db[b"1"] = b"one"
+    db[b"2"] = b"two"
+
+    # Assume that any changes are cached in memory unless
+    # explicitly flushed (or database closed). Flush database
+    # at the end of each "transaction".
+    db.flush()
+
+    # Prints b'two'
+    print(db[b"2"])
+
+    # Iterate over sorted keys in the database, starting from b"2"
+    # until the end of the database, returning only values.
+    # Mind that arguments passed to values() method are *key* values.
+    # Prints:
+    #   b'two'
+    #   b'three'
+    for word in db.values(b"2"):
+        print(word)
+
+    del db[b"2"]
+
+    # No longer true, prints False
+    print(b"2" in db)
+
+    # Prints:
+    #  b"1"
+    #  b"3"
+    for key in db:
+        print(key)
+
+    db.close()
+
+    # Don't forget to close the underlying stream!
+    f.close()
+
+"""
+from typing import Dict, Optional, Any
+
+DESC: int
+INCL: int
+
+def open(stream, *, flags=0, pagesize=0, cachesize=0, minkeypage=0) -> Dict:
+    """
+    Open a database from a random-access `stream` (like an open file). All
+    other parameters are optional and keyword-only, and allow to tweak advanced
+    parameters of the database operation (most users will not need them):
+
+    * *flags* - Currently unused.
+    * *pagesize* - Page size used for the nodes in BTree. Acceptable range
+      is 512-65536. If 0, a port-specific default will be used, optimized for
+      port's memory usage and/or performance.
+    * *cachesize* - Suggested memory cache size in bytes. For a
+      board with enough memory using larger values may improve performance.
+      Cache policy is as follows: entire cache is not allocated at once;
+      instead, accessing a new page in database will allocate a memory buffer
+      for it, until value specified by *cachesize* is reached. Then, these
+      buffers will be managed using LRU (least recently used) policy. More
+      buffers may still be allocated if needed (e.g., if a database contains
+      big keys and/or values). Allocated cache buffers aren't reclaimed.
+    * *minkeypage* - Minimum number of keys to store per page. Default value
+      of 0 equivalent to 2.
+
+    Returns a BTree object, which implements a dictionary protocol (set
+    of methods), and some additional methods described below.
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/esp32.pyi` & `micropython_esp32_stubs-1.20.0.post1/esp32.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,304 +1,311 @@
-"""
-functionality specific to the ESP32. See: https://docs.micropython.org/en/v1.19.1/library/esp32.html
-
-The ``esp32`` module contains functions and classes specifically aimed at
-controlling ESP32 modules.
-
-"""
-from __future__ import annotations
-from typing import List, Optional, Tuple, Union, Any
-
-WAKEUP_ALL_LOW: bool
-WAKEUP_ANY_HIGH: bool
-HEAP_EXEC: int
-HEAP_DATA: int
-
-def idf_heap_info(capabilities) -> List[Tuple]:
-    """
-    Returns information about the ESP-IDF heap memory regions. One of them contains
-    the MicroPython heap and the others are used by ESP-IDF, e.g., for network
-    buffers and other data. This data is useful to get a sense of how much memory
-    is available to ESP-IDF and the networking stack in particular. It may shed
-    some light on situations where ESP-IDF operations fail due to allocation failures.
-    The information returned is *not* useful to troubleshoot Python allocation failures,
-    use `micropython.mem_info()` instead.
-
-    The capabilities parameter corresponds to ESP-IDF's ``MALLOC_CAP_XXX`` values but the
-    two most useful ones are predefined as `esp32.HEAP_DATA` for data heap regions and
-    `esp32.HEAP_EXEC` for executable regions as used by the native code emitter.
-
-    The return value is a list of 4-tuples, where each 4-tuple corresponds to one heap
-    and contains: the total bytes, the free bytes, the largest free block, and
-    the minimum free seen over time.
-
-    Example after booting::
-
-        >>> import esp32; esp32.idf_heap_info(esp32.HEAP_DATA)
-        [(240, 0, 0, 0), (7288, 0, 0, 0), (16648, 4, 4, 4), (79912, 35712, 35512, 35108),
-         (15072, 15036, 15036, 15036), (113840, 0, 0, 0)]
-    """
-    ...
-
-def hall_sensor() -> int:
-    """
-    Read the raw value of the internal Hall sensor, returning an integer.
-    """
-    ...
-
-def wake_on_ext1(pins, level) -> None:
-    """
-    Configure how EXT1 wakes the device from sleep.  *pins* can be ``None``
-    or a tuple/list of valid Pin objects.  *level* should be ``esp32.WAKEUP_ALL_LOW``
-    or ``esp32.WAKEUP_ANY_HIGH``.
-    """
-    ...
-
-def raw_temperature() -> int:
-    """
-    Read the raw value of the internal temperature sensor, returning an integer.
-    """
-    ...
-
-def wake_on_ext0(pin, level) -> None:
-    """
-    Configure how EXT0 wakes the device from sleep.  *pin* can be ``None``
-    or a valid Pin object.  *level* should be ``esp32.WAKEUP_ALL_LOW`` or
-    ``esp32.WAKEUP_ANY_HIGH``.
-    """
-    ...
-
-def wake_on_touch(wake) -> None:
-    """
-    Configure whether or not a touch will wake the device from sleep.
-    *wake* should be a boolean value.
-    """
-    ...
-
-def gpio_deep_sleep_hold(enable) -> None:
-    """
-    Configure whether non-RTC GPIO pin configuration is retained during
-    deep-sleep mode for held pads. *enable* should be a boolean value.
-    """
-    ...
-
-class ULP:
-    """
-    This class provides access to the Ultra-Low-Power co-processor.
-    """
-
-    RESERVE_MEM: int
-    def run(self, entry_point) -> Any:
-        """
-        Start the ULP running at the given *entry_point*.
-
-        """
-        ...
-    def set_wakeup_period(self, period_index, period_us) -> None:
-        """
-        Set the wake-up period.
-        """
-        ...
-    def load_binary(self, load_addr, program_binary) -> None:
-        """
-        Load a *program_binary* into the ULP at the given *load_addr*.
-        """
-        ...
-    def __init__(self) -> None: ...
-
-class NVS:
-    """
-    Create an object providing access to a namespace (which is automatically created if not
-    present).
-    """
-
-    def get_i32(self, key) -> int:
-        """
-        Returns the signed integer value for the specified key. Raises an OSError if the key does not
-        exist or has a different type.
-        """
-        ...
-    def set_i32(self, key, value) -> None:
-        """
-        Sets a 32-bit signed integer value for the specified key. Remember to call *commit*!
-        """
-        ...
-    def set_blob(self, key, value) -> None:
-        """
-        Sets a binary blob value for the specified key. The value passed in must support the buffer
-        protocol, e.g. bytes, bytearray, str. (Note that esp-idf distinguishes blobs and strings, this
-        method always writes a blob even if a string is passed in as value.)
-        Remember to call *commit*!
-        """
-        ...
-    def commit(self) -> Any:
-        """
-        Commits changes made by *set_xxx* methods to flash.
-        """
-        ...
-    def get_blob(self, key, buffer) -> int:
-        """
-        Reads the value of the blob for the specified key into the buffer, which must be a bytearray.
-        Returns the actual length read. Raises an OSError if the key does not exist, has a different
-        type, or if the buffer is too small.
-        """
-        ...
-    def erase_key(self, key) -> Any:
-        """
-        Erases a key-value pair.
-        """
-        ...
-    def __init__(self, namespace) -> None: ...
-
-class Partition:
-    """
-    Create an object representing a partition.  *id* can be a string which is the label
-    of the partition to retrieve, or one of the constants: ``BOOT`` or ``RUNNING``.
-    *block_size* specifies the byte size of an individual block.
-    """
-
-    RUNNING: int
-    TYPE_APP: int
-    TYPE_DATA: int
-    BOOT: int
-    def readblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any: ...
-    def ioctl(self, cmd, arg) -> Any:
-        """
-        These methods implement the simple and :ref:`extended
-        <block-device-interface>` block protocol defined by
-        :class:`os.AbstractBlockDev`.
-        """
-        ...
-    def set_boot(self) -> None:
-        """
-        Sets the partition as the boot partition.
-        """
-        ...
-    def writeblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any: ...
-    def info(self) -> Tuple:
-        """
-        Returns a 6-tuple ``(type, subtype, addr, size, label, encrypted)``.
-        """
-        ...
-    @classmethod
-    def find(cls, type=TYPE_APP, subtype=0xFF, label=None, block_size=4096) -> List:
-        """
-        Find a partition specified by *type*, *subtype* and *label*.  Returns a
-        (possibly empty) list of Partition objects. Note: ``subtype=0xff`` matches any subtype
-        and ``label=None`` matches any label.
-
-        *block_size* specifies the byte size of an individual block used by the returned
-        objects.
-        """
-        ...
-    def get_next_update(self) -> Partition:
-        """
-        Gets the next update partition after this one, and returns a new Partition object.
-        Typical usage is ``Partition(Partition.RUNNING).get_next_update()``
-        which returns the next partition to update given the current running one.
-        """
-        ...
-    @classmethod
-    def mark_app_valid_cancel_rollback(cls) -> Any:
-        """
-        Signals that the current boot is considered successful.
-        Calling ``mark_app_valid_cancel_rollback`` is required on the first boot of a new
-        partition to avoid an automatic rollback at the next boot.
-        This uses the ESP-IDF "app rollback" feature with "CONFIG_BOOTLOADER_APP_ROLLBACK_ENABLE"
-        and  an ``OSError(-261)`` is raised if called on firmware that doesn't have the
-        feature enabled.
-        It is OK to call ``mark_app_valid_cancel_rollback`` on every boot and it is not
-        necessary when booting firmare that was loaded using esptool.
-        """
-        ...
-    def __init__(self, id, block_size=4096, /) -> None: ...
-
-class RMT:
-    """
-    This class provides access to one of the eight RMT channels. *channel* is
-    required and identifies which RMT channel (0-7) will be configured. *pin*,
-    also required, configures which Pin is bound to the RMT channel. *clock_div*
-    is an 8-bit clock divider that divides the source clock (80MHz) to the RMT
-    channel allowing the resolution to be specified. *idle_level* specifies
-    what level the output will be when no transmission is in progress and can
-    be any value that converts to a boolean, with ``True`` representing high
-    voltage and ``False`` representing low.
-
-    To enable the transmission carrier feature, *tx_carrier* should be a tuple
-    of three positive integers: carrier frequency, duty percent (``0`` to
-    ``100``) and the output level to apply the carrier to (a boolean as per
-    *idle_level*).
-    """
-
-    def source_freq(self) -> Any:
-        """
-        Returns the source clock frequency. Currently the source clock is not
-        configurable so this will always return 80MHz.
-        """
-        ...
-    def loop(self, enable_loop) -> None:
-        """
-        Configure looping on the channel. *enable_loop* is bool, set to ``True`` to
-        enable looping on the *next* call to `RMT.write_pulses`. If called with
-        ``False`` while a looping sequence is currently being transmitted then the
-        current loop iteration will be completed and then transmission will stop.
-        """
-        ...
-    def wait_done(self, *, timeout=0) -> bool:
-        """
-        Returns ``True`` if the channel is idle or ``False`` if a sequence of
-        pulses started with `RMT.write_pulses` is being transmitted. If the
-        *timeout* keyword argument is given then block for up to this many
-        milliseconds for transmission to complete.
-        """
-        ...
-    def write_pulses(self, duration, data: Union[bool, int] = True) -> Any:
-        """
-        Begin transmitting a sequence. There are three ways to specify this:
-
-        **Mode 1:** *duration* is a list or tuple of durations. The optional *data*
-        argument specifies the initial output level. The output level will toggle
-        after each duration.
-
-        **Mode 2:** *duration* is a positive integer and *data* is a list or tuple
-        of output levels. *duration* specifies a fixed duration for each.
-
-        **Mode 3:** *duration* and *data* are lists or tuples of equal length,
-        specifying individual durations and the output level for each.
-
-        Durations are in integer units of the channel resolution (as described
-        above), between 1 and 32767 units. Output levels are any value that can
-        be converted to a boolean, with ``True`` representing high voltage and
-        ``False`` representing low.
-
-        If transmission of an earlier sequence is in progress then this method will
-        block until that transmission is complete before beginning the new sequence.
-
-        If looping has been enabled with `RMT.loop`, the sequence will be
-        repeated indefinitely. Further calls to this method will block until the
-        end of the current loop iteration before immediately beginning to loop the
-        new sequence of pulses. Looping sequences longer than 126 pulses is not
-        supported by the hardware.
-        """
-        ...
-    @staticmethod
-    def bitstream_channel(value: Optional[Any] = None) -> int:
-        """
-        Select which RMT channel is used by the `machine.bitstream` implementation.
-        *value* can be ``None`` or a valid RMT channel number.  The default RMT
-        channel is the highest numbered one.
-
-        Passing in ``None`` disables the use of RMT and instead selects a bit-banging
-        implementation for `machine.bitstream`.
-
-        Passing in no argument will not change the channel.  This function returns
-        the current channel number.
-        """
-        ...
-    def deinit(self, *args, **kwargs) -> Any: ...
-    def clock_div(self) -> Any:
-        """
-        Return the clock divider. Note that the channel resolution is
-        ``1 / (source_freq / clock_div)``.
-        """
-        ...
-    def __init__(self, channel, *, pin=None, clock_div=8, idle_level=False, tx_carrier=None) -> None: ...
+"""
+functionality specific to the ESP32. See: https://docs.micropython.org/en/v1.20.0/library/esp32.html
+
+The ``esp32`` module contains functions and classes specifically aimed at
+controlling ESP32 modules.
+
+"""
+from __future__ import annotations
+from typing import List, Optional, Tuple, Union, Any
+
+WAKEUP_ANY_HIGH: bool
+WAKEUP_ALL_LOW: bool
+HEAP_EXEC: int
+HEAP_DATA: int
+
+def wake_on_ulp(wake) -> None:
+    """
+    Configure whether or not the Ultra-Low-Power co-processor can wake the
+    device from sleep. *wake* should be a boolean value.
+    """
+    ...
+
+def idf_heap_info(capabilities) -> List[Tuple]:
+    """
+    Returns information about the ESP-IDF heap memory regions. One of them contains
+    the MicroPython heap and the others are used by ESP-IDF, e.g., for network
+    buffers and other data. This data is useful to get a sense of how much memory
+    is available to ESP-IDF and the networking stack in particular. It may shed
+    some light on situations where ESP-IDF operations fail due to allocation failures.
+    The information returned is *not* useful to troubleshoot Python allocation failures,
+    use `micropython.mem_info()` instead.
+
+    The capabilities parameter corresponds to ESP-IDF's ``MALLOC_CAP_XXX`` values but the
+    two most useful ones are predefined as `esp32.HEAP_DATA` for data heap regions and
+    `esp32.HEAP_EXEC` for executable regions as used by the native code emitter.
+
+    The return value is a list of 4-tuples, where each 4-tuple corresponds to one heap
+    and contains: the total bytes, the free bytes, the largest free block, and
+    the minimum free seen over time.
+
+    Example after booting::
+
+        >>> import esp32; esp32.idf_heap_info(esp32.HEAP_DATA)
+        [(240, 0, 0, 0), (7288, 0, 0, 0), (16648, 4, 4, 4), (79912, 35712, 35512, 35108),
+         (15072, 15036, 15036, 15036), (113840, 0, 0, 0)]
+    """
+    ...
+
+def raw_temperature() -> int:
+    """
+    Read the raw value of the internal temperature sensor, returning an integer.
+    """
+    ...
+
+def wake_on_touch(wake) -> None:
+    """
+    Configure whether or not a touch will wake the device from sleep.
+    *wake* should be a boolean value.
+    """
+    ...
+
+def wake_on_ext1(pins, level) -> None:
+    """
+    Configure how EXT1 wakes the device from sleep.  *pins* can be ``None``
+    or a tuple/list of valid Pin objects.  *level* should be ``esp32.WAKEUP_ALL_LOW``
+    or ``esp32.WAKEUP_ANY_HIGH``.
+    """
+    ...
+
+def wake_on_ext0(pin, level) -> None:
+    """
+    Configure how EXT0 wakes the device from sleep.  *pin* can be ``None``
+    or a valid Pin object.  *level* should be ``esp32.WAKEUP_ALL_LOW`` or
+    ``esp32.WAKEUP_ANY_HIGH``.
+    """
+    ...
+
+def hall_sensor() -> int:
+    """
+    Read the raw value of the internal Hall sensor, returning an integer.
+    """
+    ...
+
+def gpio_deep_sleep_hold(enable) -> None:
+    """
+    Configure whether non-RTC GPIO pin configuration is retained during
+    deep-sleep mode for held pads. *enable* should be a boolean value.
+    """
+    ...
+
+class ULP:
+    """
+    This class provides access to the Ultra-Low-Power co-processor.
+    """
+
+    RESERVE_MEM: int
+    def run(self, entry_point) -> Any:
+        """
+        Start the ULP running at the given *entry_point*.
+
+        """
+        ...
+    def set_wakeup_period(self, period_index, period_us) -> None:
+        """
+        Set the wake-up period.
+        """
+        ...
+    def load_binary(self, load_addr, program_binary) -> None:
+        """
+        Load a *program_binary* into the ULP at the given *load_addr*.
+        """
+        ...
+    def __init__(self) -> None: ...
+
+class NVS:
+    """
+    Create an object providing access to a namespace (which is automatically created if not
+    present).
+    """
+
+    def get_i32(self, key) -> int:
+        """
+        Returns the signed integer value for the specified key. Raises an OSError if the key does not
+        exist or has a different type.
+        """
+        ...
+    def set_i32(self, key, value) -> None:
+        """
+        Sets a 32-bit signed integer value for the specified key. Remember to call *commit*!
+        """
+        ...
+    def set_blob(self, key, value) -> None:
+        """
+        Sets a binary blob value for the specified key. The value passed in must support the buffer
+        protocol, e.g. bytes, bytearray, str. (Note that esp-idf distinguishes blobs and strings, this
+        method always writes a blob even if a string is passed in as value.)
+        Remember to call *commit*!
+        """
+        ...
+    def commit(self) -> Any:
+        """
+        Commits changes made by *set_xxx* methods to flash.
+        """
+        ...
+    def get_blob(self, key, buffer) -> int:
+        """
+        Reads the value of the blob for the specified key into the buffer, which must be a bytearray.
+        Returns the actual length read. Raises an OSError if the key does not exist, has a different
+        type, or if the buffer is too small.
+        """
+        ...
+    def erase_key(self, key) -> Any:
+        """
+        Erases a key-value pair.
+        """
+        ...
+    def __init__(self, namespace) -> None: ...
+
+class Partition:
+    """
+    Create an object representing a partition.  *id* can be a string which is the label
+    of the partition to retrieve, or one of the constants: ``BOOT`` or ``RUNNING``.
+    *block_size* specifies the byte size of an individual block.
+    """
+
+    RUNNING: int
+    TYPE_APP: int
+    TYPE_DATA: int
+    BOOT: int
+    def readblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any: ...
+    def ioctl(self, cmd, arg) -> Any:
+        """
+        These methods implement the simple and :ref:`extended
+        <block-device-interface>` block protocol defined by
+        :class:`os.AbstractBlockDev`.
+        """
+        ...
+    def set_boot(self) -> None:
+        """
+        Sets the partition as the boot partition.
+        """
+        ...
+    def writeblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any: ...
+    def info(self) -> Tuple:
+        """
+        Returns a 6-tuple ``(type, subtype, addr, size, label, encrypted)``.
+        """
+        ...
+    @classmethod
+    def find(cls, type=TYPE_APP, subtype=0xFF, label=None, block_size=4096) -> List:
+        """
+        Find a partition specified by *type*, *subtype* and *label*.  Returns a
+        (possibly empty) list of Partition objects. Note: ``subtype=0xff`` matches any subtype
+        and ``label=None`` matches any label.
+
+        *block_size* specifies the byte size of an individual block used by the returned
+        objects.
+        """
+        ...
+    def get_next_update(self) -> Partition:
+        """
+        Gets the next update partition after this one, and returns a new Partition object.
+        Typical usage is ``Partition(Partition.RUNNING).get_next_update()``
+        which returns the next partition to update given the current running one.
+        """
+        ...
+    @classmethod
+    def mark_app_valid_cancel_rollback(cls) -> Any:
+        """
+        Signals that the current boot is considered successful.
+        Calling ``mark_app_valid_cancel_rollback`` is required on the first boot of a new
+        partition to avoid an automatic rollback at the next boot.
+        This uses the ESP-IDF "app rollback" feature with "CONFIG_BOOTLOADER_APP_ROLLBACK_ENABLE"
+        and  an ``OSError(-261)`` is raised if called on firmware that doesn't have the
+        feature enabled.
+        It is OK to call ``mark_app_valid_cancel_rollback`` on every boot and it is not
+        necessary when booting firmare that was loaded using esptool.
+        """
+        ...
+    def __init__(self, id, block_size=4096, /) -> None: ...
+
+class RMT:
+    """
+    This class provides access to one of the eight RMT channels. *channel* is
+    required and identifies which RMT channel (0-7) will be configured. *pin*,
+    also required, configures which Pin is bound to the RMT channel. *clock_div*
+    is an 8-bit clock divider that divides the source clock (80MHz) to the RMT
+    channel allowing the resolution to be specified. *idle_level* specifies
+    what level the output will be when no transmission is in progress and can
+    be any value that converts to a boolean, with ``True`` representing high
+    voltage and ``False`` representing low.
+
+    To enable the transmission carrier feature, *tx_carrier* should be a tuple
+    of three positive integers: carrier frequency, duty percent (``0`` to
+    ``100``) and the output level to apply the carrier to (a boolean as per
+    *idle_level*).
+    """
+
+    def source_freq(self) -> Any:
+        """
+        Returns the source clock frequency. Currently the source clock is not
+        configurable so this will always return 80MHz.
+        """
+        ...
+    def loop(self, enable_loop) -> None:
+        """
+        Configure looping on the channel. *enable_loop* is bool, set to ``True`` to
+        enable looping on the *next* call to `RMT.write_pulses`. If called with
+        ``False`` while a looping sequence is currently being transmitted then the
+        current loop iteration will be completed and then transmission will stop.
+        """
+        ...
+    def wait_done(self, *, timeout=0) -> bool:
+        """
+        Returns ``True`` if the channel is idle or ``False`` if a sequence of
+        pulses started with `RMT.write_pulses` is being transmitted. If the
+        *timeout* keyword argument is given then block for up to this many
+        milliseconds for transmission to complete.
+        """
+        ...
+    def write_pulses(self, duration, data: Union[bool, int] = True) -> Any:
+        """
+        Begin transmitting a sequence. There are three ways to specify this:
+
+        **Mode 1:** *duration* is a list or tuple of durations. The optional *data*
+        argument specifies the initial output level. The output level will toggle
+        after each duration.
+
+        **Mode 2:** *duration* is a positive integer and *data* is a list or tuple
+        of output levels. *duration* specifies a fixed duration for each.
+
+        **Mode 3:** *duration* and *data* are lists or tuples of equal length,
+        specifying individual durations and the output level for each.
+
+        Durations are in integer units of the channel resolution (as described
+        above), between 1 and 32767 units. Output levels are any value that can
+        be converted to a boolean, with ``True`` representing high voltage and
+        ``False`` representing low.
+
+        If transmission of an earlier sequence is in progress then this method will
+        block until that transmission is complete before beginning the new sequence.
+
+        If looping has been enabled with `RMT.loop`, the sequence will be
+        repeated indefinitely. Further calls to this method will block until the
+        end of the current loop iteration before immediately beginning to loop the
+        new sequence of pulses. Looping sequences longer than 126 pulses is not
+        supported by the hardware.
+        """
+        ...
+    @staticmethod
+    def bitstream_channel(value: Optional[Any] = None) -> int:
+        """
+        Select which RMT channel is used by the `machine.bitstream` implementation.
+        *value* can be ``None`` or a valid RMT channel number.  The default RMT
+        channel is the highest numbered one.
+
+        Passing in ``None`` disables the use of RMT and instead selects a bit-banging
+        implementation for `machine.bitstream`.
+
+        Passing in no argument will not change the channel.  This function returns
+        the current channel number.
+        """
+        ...
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def clock_div(self) -> Any:
+        """
+        Return the clock divider. Note that the channel resolution is
+        ``1 / (source_freq / clock_div)``.
+        """
+        ...
+    def __init__(self, channel, *, pin=None, clock_div=8, idle_level=False, tx_carrier=None) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/framebuf.pyi` & `micropython_esp32_stubs-1.20.0.post1/framebuf.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,140 @@
-"""
-Frame buffer manipulation. See: https://docs.micropython.org/en/v1.19.1/library/framebuf.html
-
-This module provides a general frame buffer which can be used to create
-bitmap images, which can then be sent to a display.
-"""
-from typing import Optional, Any
-
-MONO_HMSB: int
-MONO_HLSB: int
-RGB565: int
-MONO_VLSB: int
-MVLSB: int
-GS2_HMSB: int
-GS8: int
-GS4_HMSB: int
-
-def FrameBuffer1(*args, **kwargs) -> Any: ...
-
-class FrameBuffer:
-    """
-    Construct a FrameBuffer object.  The parameters are:
-
-        - *buffer* is an object with a buffer protocol which must be large
-          enough to contain every pixel defined by the width, height and
-          format of the FrameBuffer.
-        - *width* is the width of the FrameBuffer in pixels
-        - *height* is the height of the FrameBuffer in pixels
-        - *format* specifies the type of pixel used in the FrameBuffer;
-          permissible values are listed under Constants below. These set the
-          number of bits used to encode a color value and the layout of these
-          bits in *buffer*.
-          Where a color value c is passed to a method, c is a small integer
-          with an encoding that is dependent on the format of the FrameBuffer.
-        - *stride* is the number of pixels between each horizontal line
-          of pixels in the FrameBuffer. This defaults to *width* but may
-          need adjustments when implementing a FrameBuffer within another
-          larger FrameBuffer or screen. The *buffer* size must accommodate
-          an increased step size.
-
-    One must specify valid *buffer*, *width*, *height*, *format* and
-    optionally *stride*.  Invalid *buffer* size or dimensions may lead to
-    unexpected errors.
-    """
-
-    def rect(self, x, y, w, h, c) -> Any: ...
-    def pixel(self, x, y, c: Optional[Any] = None) -> Any:
-        """
-        If *c* is not given, get the color value of the specified pixel.
-        If *c* is given, set the specified pixel to the given color.
-        """
-        ...
-    def vline(self, x, y, h, c) -> Any: ...
-    def scroll(self, xstep, ystep) -> Any:
-        """
-        Shift the contents of the FrameBuffer by the given vector. This may
-        leave a footprint of the previous colors in the FrameBuffer.
-        """
-        ...
-    def text(self, s, x, y, c: Optional[Any] = None) -> None:
-        """
-        Write text to the FrameBuffer using the the coordinates as the upper-left
-        corner of the text. The color of the text can be defined by the optional
-        argument but is otherwise a default value of 1. All characters have
-        dimensions of 8x8 pixels and there is currently no way to change the font.
-
-        """
-        ...
-    def fill(self, c) -> None:
-        """
-        Fill the entire FrameBuffer with the specified color.
-        """
-        ...
-    def blit(self, fbuf, x, y, key=-1, palette=None) -> None:
-        """
-        Draw another FrameBuffer on top of the current one at the given coordinates.
-        If *key* is specified then it should be a color integer and the
-        corresponding color will be considered transparent: all pixels with that
-        color value will not be drawn.
-
-        The *palette* argument enables blitting between FrameBuffers with differing
-        formats. Typical usage is to render a monochrome or grayscale glyph/icon to
-        a color display. The *palette* is a FrameBuffer instance whose format is
-        that of the current FrameBuffer. The *palette* height is one pixel and its
-        pixel width is the number of colors in the source FrameBuffer. The *palette*
-        for an N-bit source needs 2**N pixels; the *palette* for a monochrome source
-        would have 2 pixels representing background and foreground colors. The
-        application assigns a color to each pixel in the *palette*. The color of the
-        current pixel will be that of that *palette* pixel whose x position is the
-        color of the corresponding source pixel.
-        """
-        ...
-    def line(self, x1, y1, x2, y2, c) -> None:
-        """
-        Draw a line from a set of coordinates using the given color and
-        a thickness of 1 pixel. The `line` method draws the line up to
-        a second set of coordinates whereas the `hline` and `vline`
-        methods draw horizontal and vertical lines respectively up to
-        a given length.
-        """
-        ...
-    def fill_rect(self, x, y, w, h, c) -> None:
-        """
-        Draw a rectangle at the given location, size and color. The `rect`
-        method draws only a 1 pixel outline whereas the `fill_rect` method
-        draws both the outline and interior.
-        """
-        ...
-    def hline(self, x, y, w, c) -> Any: ...
-    def __init__(self, buffer, width, height, format, stride=-1, /) -> None: ...
+"""
+Frame buffer manipulation. See: https://docs.micropython.org/en/v1.20.0/library/framebuf.html
+
+This module provides a general frame buffer which can be used to create
+bitmap images, which can then be sent to a display.
+"""
+from typing import Optional, Any
+
+MONO_HMSB: int
+MONO_HLSB: int
+RGB565: int
+MONO_VLSB: int
+MVLSB: int
+GS2_HMSB: int
+GS8: int
+GS4_HMSB: int
+
+def FrameBuffer1(*args, **kwargs) -> Any: ...
+
+class FrameBuffer:
+    """
+    Construct a FrameBuffer object.  The parameters are:
+
+        - *buffer* is an object with a buffer protocol which must be large
+          enough to contain every pixel defined by the width, height and
+          format of the FrameBuffer.
+        - *width* is the width of the FrameBuffer in pixels
+        - *height* is the height of the FrameBuffer in pixels
+        - *format* specifies the type of pixel used in the FrameBuffer;
+          permissible values are listed under Constants below. These set the
+          number of bits used to encode a color value and the layout of these
+          bits in *buffer*.
+          Where a color value c is passed to a method, c is a small integer
+          with an encoding that is dependent on the format of the FrameBuffer.
+        - *stride* is the number of pixels between each horizontal line
+          of pixels in the FrameBuffer. This defaults to *width* but may
+          need adjustments when implementing a FrameBuffer within another
+          larger FrameBuffer or screen. The *buffer* size must accommodate
+          an increased step size.
+
+    One must specify valid *buffer*, *width*, *height*, *format* and
+    optionally *stride*.  Invalid *buffer* size or dimensions may lead to
+    unexpected errors.
+    """
+
+    def poly(self, x, y, coords, c, f: Optional[Any] = None) -> Any:
+        """
+        Given a list of coordinates, draw an arbitrary (convex or concave) closed
+        polygon at the given x, y location using the given color.
+
+        The *coords* must be specified as a :mod:`array` of integers, e.g.
+        ``array('h', [x0, y0, x1, y1, ... xn, yn])``.
+
+        The optional *f* parameter can be set to ``True`` to fill the polygon.
+        Otherwise just a one pixel outline is drawn.
+        """
+        ...
+    def vline(self, x, y, h, c) -> Any: ...
+    def pixel(self, x, y, c: Optional[Any] = None) -> Any:
+        """
+        If *c* is not given, get the color value of the specified pixel.
+        If *c* is given, set the specified pixel to the given color.
+        """
+        ...
+    def text(self, s, x, y, c: Optional[Any] = None) -> None:
+        """
+        Write text to the FrameBuffer using the the coordinates as the upper-left
+        corner of the text. The color of the text can be defined by the optional
+        argument but is otherwise a default value of 1. All characters have
+        dimensions of 8x8 pixels and there is currently no way to change the font.
+
+        """
+        ...
+    def rect(self, x, y, w, h, c, f: Optional[Any] = None) -> None:
+        """
+        Draw a rectangle at the given location, size and color.
+
+        The optional *f* parameter can be set to ``True`` to fill the rectangle.
+        Otherwise just a one pixel outline is drawn.
+        """
+        ...
+    def scroll(self, xstep, ystep) -> Any:
+        """
+        Shift the contents of the FrameBuffer by the given vector. This may
+        leave a footprint of the previous colors in the FrameBuffer.
+        """
+        ...
+    def ellipse(self, x, y, xr, yr, c, f, m: Optional[Any] = None) -> None:
+        """
+        Draw an ellipse at the given location. Radii *xr* and *yr* define the
+        geometry; equal values cause a circle to be drawn. The *c* parameter
+        defines the color.
+
+        The optional *f* parameter can be set to ``True`` to fill the ellipse.
+        Otherwise just a one pixel outline is drawn.
+
+        The optional *m* parameter enables drawing to be restricted to certain
+        quadrants of the ellipse. The LS four bits determine which quadrants are
+        to be drawn, with bit 0 specifying Q1, b1 Q2, b2 Q3 and b3 Q4. Quadrants
+        are numbered counterclockwise with Q1 being top right.
+        """
+        ...
+    def line(self, x1, y1, x2, y2, c) -> None:
+        """
+        Draw a line from a set of coordinates using the given color and
+        a thickness of 1 pixel. The `line` method draws the line up to
+        a second set of coordinates whereas the `hline` and `vline`
+        methods draw horizontal and vertical lines respectively up to
+        a given length.
+        """
+        ...
+    def blit(self, fbuf, x, y, key=-1, palette=None) -> None:
+        """
+        Draw another FrameBuffer on top of the current one at the given coordinates.
+        If *key* is specified then it should be a color integer and the
+        corresponding color will be considered transparent: all pixels with that
+        color value will not be drawn. (If the *palette* is specified then the *key*
+        is compared to the value from *palette*, not to the value directly from
+        *fbuf*.)
+
+        The *palette* argument enables blitting between FrameBuffers with differing
+        formats. Typical usage is to render a monochrome or grayscale glyph/icon to
+        a color display. The *palette* is a FrameBuffer instance whose format is
+        that of the current FrameBuffer. The *palette* height is one pixel and its
+        pixel width is the number of colors in the source FrameBuffer. The *palette*
+        for an N-bit source needs 2**N pixels; the *palette* for a monochrome source
+        would have 2 pixels representing background and foreground colors. The
+        application assigns a color to each pixel in the *palette*. The color of the
+        current pixel will be that of that *palette* pixel whose x position is the
+        color of the corresponding source pixel.
+        """
+        ...
+    def hline(self, x, y, w, c) -> Any: ...
+    def fill(self, c) -> None:
+        """
+        Fill the entire FrameBuffer with the specified color.
+        """
+        ...
+    def fill_rect(self, *args, **kwargs) -> Any: ...
+    def __init__(self, buffer, width, height, format, stride=-1, /) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/gc.pyi` & `micropython_esp32_stubs-1.20.0.post1/gc.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-"""
-control the garbage collector. See: https://docs.micropython.org/en/v1.19.1/library/gc.html
-
-|see_cpython_module| :mod:`python:gc` https://docs.python.org/3/library/gc.html .
-"""
-from typing import Optional, Any
-
-def mem_alloc() -> int:
-    """
-    Return the number of bytes of heap RAM that are allocated.
-    """
-    ...
-
-def isenabled(*args, **kwargs) -> Any: ...
-def mem_free() -> int:
-    """
-    Return the number of bytes of available heap RAM, or -1 if this amount
-    is not known.
-    """
-    ...
-
-def threshold(amount: Optional[Any] = None) -> Any:
-    """
-    Set or query the additional GC allocation threshold. Normally, a collection
-    is triggered only when a new allocation cannot be satisfied, i.e. on an
-    out-of-memory (OOM) condition. If this function is called, in addition to
-    OOM, a collection will be triggered each time after *amount* bytes have been
-    allocated (in total, since the previous time such an amount of bytes
-    have been allocated). *amount* is usually specified as less than the
-    full heap size, with the intention to trigger a collection earlier than when the
-    heap becomes exhausted, and in the hope that an early collection will prevent
-    excessive memory fragmentation. This is a heuristic measure, the effect
-    of which will vary from application to application, as well as
-    the optimal value of the *amount* parameter.
-
-    Calling the function without argument will return the current value of
-    the threshold. A value of -1 means a disabled allocation threshold.
-    """
-    ...
-
-def collect() -> None:
-    """
-    Run a garbage collection.
-    """
-    ...
-
-def enable() -> None:
-    """
-    Enable automatic garbage collection.
-    """
-    ...
-
-def disable() -> None:
-    """
-    Disable automatic garbage collection.  Heap memory can still be allocated,
-    and garbage collection can still be initiated manually using :meth:`gc.collect`.
-    """
-    ...
+"""
+control the garbage collector. See: https://docs.micropython.org/en/v1.20.0/library/gc.html
+
+|see_cpython_module| :mod:`python:gc` https://docs.python.org/3/library/gc.html .
+"""
+from typing import Optional, Any
+
+def mem_alloc() -> int:
+    """
+    Return the number of bytes of heap RAM that are allocated.
+    """
+    ...
+
+def isenabled(*args, **kwargs) -> Any: ...
+def mem_free() -> int:
+    """
+    Return the number of bytes of available heap RAM, or -1 if this amount
+    is not known.
+    """
+    ...
+
+def threshold(amount: Optional[Any] = None) -> Any:
+    """
+    Set or query the additional GC allocation threshold. Normally, a collection
+    is triggered only when a new allocation cannot be satisfied, i.e. on an
+    out-of-memory (OOM) condition. If this function is called, in addition to
+    OOM, a collection will be triggered each time after *amount* bytes have been
+    allocated (in total, since the previous time such an amount of bytes
+    have been allocated). *amount* is usually specified as less than the
+    full heap size, with the intention to trigger a collection earlier than when the
+    heap becomes exhausted, and in the hope that an early collection will prevent
+    excessive memory fragmentation. This is a heuristic measure, the effect
+    of which will vary from application to application, as well as
+    the optimal value of the *amount* parameter.
+
+    Calling the function without argument will return the current value of
+    the threshold. A value of -1 means a disabled allocation threshold.
+    """
+    ...
+
+def collect() -> None:
+    """
+    Run a garbage collection.
+    """
+    ...
+
+def enable() -> None:
+    """
+    Enable automatic garbage collection.
+    """
+    ...
+
+def disable() -> None:
+    """
+    Disable automatic garbage collection.  Heap memory can still be allocated,
+    and garbage collection can still be initiated manually using :meth:`gc.collect`.
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/hashlib.pyi` & `micropython_esp32_stubs-1.20.0.post1/hashlib.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-hashing algorithms. See: https://docs.micropython.org/en/v1.19.1/library/hashlib.html
-
-|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
-
-This module implements binary data hashing algorithms. The exact inventory
-of available algorithms depends on a board. Among the algorithms which may
-be implemented:
-
-* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
-  It is suitable for cryptographically-secure purposes. Included in the
-  MicroPython core and any board is recommended to provide this, unless
-  it has particular code size constraints.
-
-* SHA1 - A previous generation algorithm. Not recommended for new usages,
-  but SHA1 is a part of number of Internet standards and existing
-  applications, so boards targeting network connectivity and
-  interoperability will try to provide this.
-
-* MD5 - A legacy algorithm, not considered cryptographically secure. Only
-  selected boards, targeting interoperability with legacy applications,
-  will offer this.
-"""
-from typing import Optional, Any
-
-class sha256:
-    """
-    Create an SHA256 hasher object and optionally feed ``data`` into it.
-    """
-
-    def digest(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def __init__(self, data: Optional[Any] = None) -> None: ...
-
-class sha1:
-    """
-    Create an SHA1 hasher object and optionally feed ``data`` into it.
-    """
-
-    def digest(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def __init__(self, data: Optional[Any] = None) -> None: ...
+"""
+hashing algorithms. See: https://docs.micropython.org/en/v1.20.0/library/hashlib.html
+
+|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
+
+This module implements binary data hashing algorithms. The exact inventory
+of available algorithms depends on a board. Among the algorithms which may
+be implemented:
+
+* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
+  It is suitable for cryptographically-secure purposes. Included in the
+  MicroPython core and any board is recommended to provide this, unless
+  it has particular code size constraints.
+
+* SHA1 - A previous generation algorithm. Not recommended for new usages,
+  but SHA1 is a part of number of Internet standards and existing
+  applications, so boards targeting network connectivity and
+  interoperability will try to provide this.
+
+* MD5 - A legacy algorithm, not considered cryptographically secure. Only
+  selected boards, targeting interoperability with legacy applications,
+  will offer this.
+"""
+from typing import Optional, Any
+
+class sha256:
+    """
+    Create an SHA256 hasher object and optionally feed ``data`` into it.
+    """
+
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
+
+class sha1:
+    """
+    Create an SHA1 hasher object and optionally feed ``data`` into it.
+    """
+
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/heapq.pyi` & `micropython_esp32_stubs-1.20.0.post1/heapq.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-heap queue algorithm. See: https://docs.micropython.org/en/v1.19.1/library/heapq.html
-
-|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
-
-This module implements the
-`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
-
-A heap queue is essentially a list that has its elements stored in such a way
-that the first item of the list is always the smallest.
-"""
-from typing import Any
-
-def heappop(heap) -> Any:
-    """
-    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
-    ``heap`` is empty.
-
-    The returned item will be the smallest item in the ``heap``.
-    """
-    ...
-
-def heappush(heap, item) -> Any:
-    """
-    Push the ``item`` onto the ``heap``.
-    """
-    ...
-
-def heapify(x) -> Any:
-    """
-    Convert the list ``x`` into a heap.  This is an in-place operation.
-    """
-    ...
+"""
+heap queue algorithm. See: https://docs.micropython.org/en/v1.20.0/library/heapq.html
+
+|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
+
+This module implements the
+`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
+
+A heap queue is essentially a list that has its elements stored in such a way
+that the first item of the list is always the smallest.
+"""
+from typing import Any
+
+def heappop(heap) -> Any:
+    """
+    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
+    ``heap`` is empty.
+
+    The returned item will be the smallest item in the ``heap``.
+    """
+    ...
+
+def heappush(heap, item) -> Any:
+    """
+    Push the ``item`` onto the ``heap``.
+    """
+    ...
+
+def heapify(x) -> Any:
+    """
+    Convert the list ``x`` into a heap.  This is an in-place operation.
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/machine.pyi` & `micropython_esp32_stubs-1.20.0.post1/machine.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,1174 +1,1243 @@
-"""
-functions related to the hardware. See: https://docs.micropython.org/en/v1.19.1/library/machine.html
-
-The ``machine`` module contains specific functions related to the hardware
-on a particular board. Most functions in this module allow to achieve direct
-and unrestricted access to and control of hardware blocks on a system
-(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
-malfunction, lockups, crashes of your board, and in extreme cases, hardware
-damage.
-"""
-from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
-
-TIMER_WAKE: int
-EXT1_WAKE: int
-HARD_RESET: int
-SOFT_RESET: int
-PIN_WAKE: int
-PWRON_RESET: int
-SLEEP: int
-WDT_RESET: int
-TOUCHPAD_WAKE: int
-ULP_WAKE: int
-EXT0_WAKE: int
-DEEPSLEEP: int
-DEEPSLEEP_RESET: int
-
-def enable_irq(state) -> Any:
-    """
-    Re-enable interrupt requests.
-    The *state* parameter should be the value that was returned from the most
-    recent call to the `disable_irq()` function.
-    """
-    ...
-
-def bitstream(pin, encoding, timing, data, /) -> Any:
-    """
-    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
-    specifies how the bits are encoded, and *timing* is an encoding-specific timing
-    specification.
-
-    The supported encodings are:
-
-      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
-        1 bits as timed pulses, starting with the most significant bit.
-        The *timing* must be a four-tuple of nanoseconds in the format
-        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
-        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
-        at 800kHz.
-
-    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
-    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
-    will be closer to +/-30ns.
-
-    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
-       module for a higher-level API.
-    """
-    ...
-
-def disable_irq() -> Any:
-    """
-    Disable interrupt requests.
-    Returns the previous IRQ state which should be considered an opaque value.
-    This return value should be passed to the `enable_irq()` function to restore
-    interrupts to their original state, before `disable_irq()` was called.
-    """
-    ...
-
-def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def wake_reason() -> Any:
-    """
-    Get the wake reason. See :ref:`constants <machine_constants>` for the possible return values.
-
-    Availability: ESP32, WiPy.
-    """
-    ...
-
-def sleep() -> Any:
-    """
-    ``Note:`` This function is deprecated, use `lightsleep()` instead with no arguments.
-    """
-    ...
-
-def soft_reset() -> NoReturn:
-    """
-    Performs a soft reset of the interpreter, deleting all Python objects and
-    resetting the Python heap.  It tries to retain the method by which the user
-    is connected to the MicroPython REPL (eg serial, USB, Wifi).
-    """
-    ...
-
-def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
-    """
-    Time a pulse on the given *pin*, and return the duration of the pulse in
-    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
-    or 1 to time a high pulse.
-
-    If the current input value of the pin is different to *pulse_level*,
-    the function first (*) waits until the pin input becomes equal to *pulse_level*,
-    then (**) times the duration that the pin is equal to *pulse_level*.
-    If the pin is already equal to *pulse_level* then timing starts straight away.
-
-    The function will return -2 if there was timeout waiting for condition marked
-    (*) above, and -1 if there was timeout during the main measurement, marked (**)
-    above. The timeout is the same for both cases and given by *timeout_us* (which
-    is in microseconds).
-    """
-    ...
-
-def unique_id() -> bytes:
-    """
-    Returns a byte string with a unique identifier of a board/SoC. It will vary
-    from a board/SoC instance to another, if underlying hardware allows. Length
-    varies by hardware (so use substring of a full value if you expect a short
-    ID). In some MicroPython ports, ID corresponds to the network MAC address.
-    """
-    ...
-
-def freq(hz: Optional[Any] = None) -> Any:
-    """
-    Returns the CPU frequency in hertz.
-
-    On some ports this can also be used to set the CPU frequency by passing in *hz*.
-    """
-    ...
-
-def reset_cause() -> int:
-    """
-    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
-    """
-    ...
-
-def idle() -> Any:
-    """
-    Gates the clock to the CPU, useful to reduce power consumption at any time during
-    short or long periods. Peripherals continue working and execution resumes as soon
-    as any interrupt is triggered (on many ports this includes system timer
-    interrupt occurring at regular intervals on the order of millisecond).
-    """
-    ...
-
-def lightsleep(time_ms: Optional[Any] = None) -> Any:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def reset() -> NoReturn:
-    """
-    Resets the device in a manner similar to pushing the external RESET
-    button.
-    """
-    ...
-
-mem8: Any
-
-class PWM:
-    """
-    Construct and return a new PWM object using the following parameters:
-
-       - *dest* is the entity on which the PWM is output, which is usually a
-         :ref:`machine.Pin <machine.Pin>` object, but a port may allow other values,
-         like integers.
-       - *freq* should be an integer which sets the frequency in Hz for the
-         PWM cycle.
-       - *duty_u16* sets the duty cycle as a ratio ``duty_u16 / 65535``.
-       - *duty_ns* sets the pulse width in nanoseconds.
-
-    Setting *freq* may affect other PWM objects if the objects share the same
-    underlying PWM generator (this is hardware specific).
-    Only one of *duty_u16* and *duty_ns* should be specified at a time.
-    """
-
-    def duty_u16(self, value: Optional[Any] = None) -> int:
-        """
-        Get or set the current duty cycle of the PWM output, as an unsigned 16-bit
-        value in the range 0 to 65535 inclusive.
-
-        With no arguments the duty cycle is returned.
-
-        With a single *value* argument the duty cycle is set to that value, measured
-        as the ratio ``value / 65535``.
-        """
-        ...
-    def init(self, *, freq, duty_u16, duty_ns) -> None:
-        """
-        Modify settings for the PWM object.  See the above constructor for details
-        about the parameters.
-        """
-        ...
-    def freq(self, value: Optional[Any] = None) -> Any:
-        """
-        Get or set the current frequency of the PWM output.
-
-        With no arguments the frequency in Hz is returned.
-
-        With a single *value* argument the frequency is set to that value in Hz.  The
-        method may raise a ``ValueError`` if the frequency is outside the valid range.
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Disable the PWM output.
-        """
-        ...
-    def duty_ns(self, value: Optional[Any] = None) -> int:
-        """
-        Get or set the current pulse width of the PWM output, as a value in nanoseconds.
-
-        With no arguments the pulse width in nanoseconds is returned.
-
-        With a single *value* argument the pulse width is set to that value.
-        """
-        ...
-    def duty(self, *args, **kwargs) -> Any: ...
-    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None: ...
-
-class UART:
-    """
-    Construct a UART object of the given id.
-    """
-
-    INV_RTS: int
-    INV_RX: int
-    CTS: int
-    INV_CTS: int
-    INV_TX: int
-    RTS: int
-    def deinit(self) -> None:
-        """
-        Turn off the UART bus.
-        """
-        ...
-    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
-        """
-        Initialise the UART bus with the given parameters:
-
-          - *baudrate* is the clock rate.
-          - *bits* is the number of bits per character, 7, 8 or 9.
-          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
-          - *stop* is the number of stop bits, 1 or 2.
-
-        Additional keyword-only parameters that may be supported by a port are:
-
-          - *tx* specifies the TX pin to use.
-          - *rx* specifies the RX pin to use.
-          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
-          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
-          - *txbuf* specifies the length in characters of the TX buffer.
-          - *rxbuf* specifies the length in characters of the RX buffer.
-          - *timeout* specifies the time to wait for the first character (in ms).
-          - *timeout_char* specifies the time to wait between characters (in ms).
-          - *invert* specifies which lines to invert.
-
-              - ``0`` will not invert lines (idle state of both lines is logic high).
-              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
-              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
-              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
-
-          - *flow* specifies which hardware flow control signals to use. The value
-            is a bitmask.
-
-              - ``0`` will ignore hardware flow control signals.
-              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
-                signal if the receive FIFO has sufficient space to accept more data.
-              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
-                CTS input pin signals that the receiver is running low on buffer space.
-              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
-
-        On the WiPy only the following keyword-only parameter is supported:
-
-          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
-            Any of the pins can be None if one wants the UART to operate with limited functionality.
-            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
-            When no pins are given, then the default set of TX and RX pins is taken, and hardware
-            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
-        """
-        ...
-    def sendbreak(self) -> None:
-        """
-        Send a break condition on the bus. This drives the bus low for a duration
-        longer than required for a normal transmission of a character.
-        """
-        ...
-    def read(self, nbytes: Optional[Any] = None) -> bytes:
-        """
-        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
-        otherwise read as much data as possible. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: a bytes object containing the bytes read in.  Returns ``None``
-        on timeout.
-        """
-        ...
-    def any(self) -> int:
-        """
-        Returns an integer counting the number of characters that can be read without
-        blocking.  It will return 0 if there are no characters available and a positive
-        number if there are characters.  The method may return 1 even if there is more
-        than one character available for reading.
-
-        For more sophisticated querying of available characters use select.poll::
-
-         poll = select.poll()
-         poll.register(uart, select.POLLIN)
-         poll.poll(timeout)
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the bus.
-
-        Return value: number of bytes written or ``None`` on timeout.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
-        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: number of bytes read and stored into ``buf`` or ``None`` on
-        timeout.
-        """
-        ...
-    def readline(self) -> None:
-        """
-        Read a line, ending in a newline character. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: the line read or ``None`` on timeout.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-mem32: Any
-mem16: Any
-
-class ADCBlock:
-    """
-    Access the ADC peripheral identified by *id*, which may be an integer
-    or string.
-
-    The *bits* argument, if given, sets the resolution in bits of the
-    conversion process.  If not specified then the previous or default
-    resolution is used.
-    """
-
-    def init(self, *, bits) -> None:
-        """
-        Configure the ADC peripheral.  *bits* will set the resolution of the
-        conversion process.
-        """
-        ...
-    def connect(self, channel, source) -> Any:
-        """
-        Connect up a channel on the ADC peripheral so it is ready for sampling,
-        and return an :ref:`ADC <machine.ADC>` object that represents that connection.
-
-        The *channel* argument must be an integer, and *source* must be an object
-        (for example a :ref:`Pin <machine.Pin>`) which can be connected up for sampling.
-
-        If only *channel* is given then it is configured for sampling.
-
-        If only *source* is given then that object is connected to a default
-        channel ready for sampling.
-
-        If both *channel* and *source* are given then they are connected together
-        and made ready for sampling.
-        """
-        ...
-    def __init__(self, id, *, bits) -> None: ...
-
-class ADC:
-    """
-    Access the ADC associated with a source identified by *id*.  This
-    *id* may be an integer (usually specifying a channel number), a
-    :ref:`Pin <machine.Pin>` object, or other value supported by the
-    underlying machine.
-
-    If additional keyword-arguments are given then they will configure
-    various aspects of the ADC.  If not given, these settings will take
-    previous or default values.  The settings are:
-
-      - *sample_ns* is the sampling time in nanoseconds.
-
-      - *atten* specifies the input attenuation.
-    """
-
-    ATTN_6DB: int
-    WIDTH_10BIT: int
-    WIDTH_11BIT: int
-    WIDTH_12BIT: int
-    WIDTH_9BIT: int
-    ATTN_0DB: int
-    ATTN_2_5DB: int
-    ATTN_11DB: int
-    def read_u16(self) -> int:
-        """
-        Take an analog reading and return an integer in the range 0-65535.
-        The return value represents the raw reading taken by the ADC, scaled
-        such that the minimum value is 0 and the maximum value is 65535.
-        """
-        ...
-    def init(self, *, sample_ns, atten) -> Any:
-        """
-        Apply the given settings to the ADC.  Only those arguments that are
-        specified will be changed.  See the ADC constructor above for what the
-        arguments are.
-        """
-        ...
-    def read_uv(self) -> int:
-        """
-        Take an analog reading and return an integer value with units of
-        microvolts.  It is up to the particular port whether or not this value
-        is calibrated, and how calibration is done.
-        """
-        ...
-    def width(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def block(self) -> Any:
-        """
-        Return the :ref:`ADCBlock <machine.ADCBlock>` instance associated with
-        this ADC object.
-
-        This method only exists if the port supports the
-        :ref:`ADCBlock <machine.ADCBlock>` class.
-        """
-        ...
-    def atten(self, *args, **kwargs) -> Any: ...
-    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
-
-class I2S:
-    """
-    Construct an I2S object of the given id:
-
-    - ``id`` identifies a particular I2S bus; it is board and port specific
-
-    Keyword-only parameters that are supported on all ports:
-
-      - ``sck`` is a pin object for the serial clock line
-      - ``ws`` is a pin object for the word select line
-      - ``sd`` is a pin object for the serial data line
-      - ``mck`` is a pin object for the master clock line;
-        master clock frequency is sampling rate * 256
-      - ``mode`` specifies receive or transmit
-      - ``bits`` specifies sample size (bits), 16 or 32
-      - ``format`` specifies channel format, STEREO or MONO
-      - ``rate`` specifies audio sampling rate (Hz);
-        this is the frequency of the ``ws`` signal
-      - ``ibuf`` specifies internal buffer length (bytes)
-
-    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
-    sample data is transfered between the internal buffer and the I2S peripheral unit.
-    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
-    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
-    """
-
-    RX: int
-    MONO: int
-    STEREO: int
-    TX: int
-    @staticmethod
-    def shift(*, buf, bits, shift) -> Any:
-        """
-        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
-        Positive for left shift, negative for right shift.
-        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
-        """
-        ...
-    def init(self, sck, *args, **kwargs) -> Any:
-        """
-        see Constructor for argument descriptions
-        """
-        ...
-    def irq(self, handler) -> Any:
-        """
-        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
-        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
-        ``handler`` is called in the context of the MicroPython scheduler.
-        """
-        ...
-    def readinto(self, buf) -> int:
-        """
-        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the left channel sample data is used.
-        Returns number of bytes read
-        """
-        ...
-    def deinit(self) -> Any:
-        """
-        Deinitialize the I2S bus
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the sample data is written to both the right and left channels.
-        Returns number of bytes written
-        """
-        ...
-    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
-
-class DAC:
-    def write(self, *args, **kwargs) -> Any: ...
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class I2C:
-    """
-    Construct and return a new I2C object using the following parameters:
-
-       - *id* identifies a particular I2C peripheral.  Allowed values for
-         depend on the particular port/board
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-
-    Note that some ports/boards will have default values of *scl* and *sda*
-    that can be changed in this constructor.  Others will have fixed values
-    of *scl* and *sda* that cannot be changed.
-    """
-
-    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.  The number of bytes read is the
-        length of *buf*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_into(self, addr, buf, stop=True, /) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr*.
-        The number of bytes read will be the length of *buf*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr* starting from the memory
-        address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Write *buf* to the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def scan(self) -> List:
-        """
-        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
-        those that respond.  A device responds if it pulls the SDA line low after
-        its address (including a write bit) is sent on the bus.
-        """
-        ...
-    def writeto(self, addr, buf, stop=True, /) -> int:
-        """
-        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
-        NACK is received following the write of a byte from *buf* then the
-        remaining bytes are not sent.  If *stop* is true then a STOP condition is
-        generated at the end of the transfer, even if a NACK is received.
-        The function returns the number of ACKs that were received.
-        """
-        ...
-    def writevto(self, addr, vector, stop=True, /) -> int:
-        """
-        Write the bytes contained in *vector* to the peripheral specified by *addr*.
-        *vector* should be a tuple or list of objects with the buffer protocol.
-        The *addr* is sent once and then the bytes from each object in *vector*
-        are written out sequentially.  The objects in *vector* may be zero bytes
-        in length in which case they don't contribute to the output.
-
-        If a NACK is received following the write of a byte from one of the
-        objects in *vector* then the remaining bytes, and any remaining objects,
-        are not sent.  If *stop* is true then a STOP condition is generated at
-        the end of the transfer, even if a NACK is received.  The function
-        returns the number of ACKs that were received.
-        """
-        ...
-    def start(self) -> None:
-        """
-        Generate a START condition on the bus (SDA transitions to low while SCL is high).
-        """
-        ...
-    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def readinto(self, buf, nack=True, /) -> Any:
-        """
-        Reads bytes from the bus and stores them into *buf*.  The number of bytes
-        read is the length of *buf*.  An ACK will be sent on the bus after
-        receiving all but the last byte.  After the last byte is received, if *nack*
-        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
-        case the peripheral assumes more bytes are going to be read in a later call).
-        """
-        ...
-    def init(self, scl, sda, *, freq=400000) -> None:
-        """
-        Initialise the I2C bus with the given arguments:
-
-           - *scl* is a pin object for the SCL line
-           - *sda* is a pin object for the SDA line
-           - *freq* is the SCL clock rate
-        """
-        ...
-    def stop(self) -> None:
-        """
-        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes from *buf* to the bus.  Checks that an ACK is received
-        after each byte and stops transmitting the remaining bytes if a NACK is
-        received.  The function returns the number of ACKs that were received.
-        """
-        ...
-    def __init__(
-        self, id: Union[int, str] = -1, *, scl: Optional[Union[Pin, str]] = None, sda: Optional[Union[Pin, str]] = None, freq=400_000
-    ) -> None: ...
-
-class Timer:
-    """
-    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
-    virtual timer (if supported by a board).
-    ``id`` shall not be passed as a keyword argument.
-
-    See ``init`` for parameters of initialisation.
-    """
-
-    ONE_SHOT: int
-    PERIODIC: int
-    def deinit(self) -> None:
-        """
-        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
-        """
-        ...
-    def init(self, *, mode=PERIODIC, period=-1, callback=None) -> None:
-        """
-        Initialise the timer. Example::
-
-            def mycallback(t):
-                pass
-
-            # periodic with 100ms period
-            tim.init(period=100, callback=mycallback)
-
-            # one shot firing after 1000ms
-            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
-
-        Keyword arguments:
-
-          - ``mode`` can be one of:
-
-            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
-              period of the channel expires.
-            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
-              frequency of the channel.
-
-          - ``period`` - The timer period, in milliseconds.
-
-          - ``callback`` - The callable to call upon expiration of the timer period.
-            The callback must take one argument, which is passed the Timer object.
-            The ``callback`` argument shall be specified. Otherwise an exception
-            will occurr upon timer expiration:
-            ``TypeError: 'NoneType' object isn't callable``
-        """
-        ...
-    def value(self, *args, **kwargs) -> Any: ...
-    def __init__(self, id=-1, *args, **kwargs) -> None: ...
-
-class SoftSPI:
-    """
-    Construct a new software SPI object.  Additional parameters must be
-    given, usually at least *sck*, *mosi* and *miso*, and these are used
-    to initialise the bus.  See `SPI.init` for a description of the parameters.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def write_readinto(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
-
-class Pin:
-    """
-    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
-    additional arguments are given in the constructor then they are used to initialise
-    the pin.  Any settings that are not specified will remain in their previous state.
-
-    The arguments are:
-
-      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
-        types are: int (an internal Pin identifier), str (a Pin name), and tuple
-        (pair of [port, pin]).
-
-      - ``mode`` specifies the pin mode, which can be one of:
-
-        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
-          is in high-impedance state.
-
-        - ``Pin.OUT`` - Pin is configured for (normal) output.
-
-        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
-          output works in the following way: if the output value is set to 0 the pin
-          is active at a low level; if the output value is 1 the pin is in a high-impedance
-          state.  Not all ports implement this mode, or some might only on certain pins.
-
-        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
-          port specific.  For a pin configured in such a way any other Pin methods
-          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
-          or a hardware-specific, result).  Not all ports implement this mode.
-
-        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
-          open-drain.  Not all ports implement this mode.
-
-        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
-
-      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
-        one of:
-
-        - ``None`` - No pull up or down resistor.
-        - ``Pin.PULL_UP`` - Pull up resistor enabled.
-        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
-
-      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
-        output pin value if given, otherwise the state of the pin peripheral remains
-        unchanged.
-
-      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
-        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
-        capabilities are port dependent.  Not all ports implement this argument.
-
-      - ``alt`` specifies an alternate function for the pin and the values it can take are
-        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
-        modes.  It may be used when a pin supports more than one alternate function.  If only
-        one pin alternate function is supported the this argument is not required.  Not all
-        ports implement this argument.
-
-    As specified above, the Pin class allows to set an alternate function for a particular
-    pin, but it does not specify any further operations on such a pin.  Pins configured in
-    alternate-function mode are usually not used as GPIO but are instead driven by other
-    hardware peripherals.  The only operation supported on such a pin is re-initialising,
-    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
-    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
-    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
-    """
-
-    OPEN_DRAIN: int
-    IRQ_FALLING: int
-    IRQ_RISING: int
-    PULL_UP: int
-    OUT: int
-    PULL_DOWN: int
-    WAKE_HIGH: int
-    DRIVE_0: int
-    IN: int
-    WAKE_LOW: int
-    DRIVE_3: int
-    DRIVE_1: int
-    DRIVE_2: int
-    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
-        """
-           Configure an interrupt handler to be called when the trigger source of the
-           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
-           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
-           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
-           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
-           state '0' and the external pin value for state '1'.
-
-           The arguments are:
-
-             - ``handler`` is an optional function to be called when the interrupt
-               triggers. The handler must take exactly one argument which is the
-               ``Pin`` instance.
-
-             - ``trigger`` configures the event which can generate an interrupt.
-               Possible values are:
-
-               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
-               - ``Pin.IRQ_RISING`` interrupt on rising edge.
-               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
-               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
-
-               These values can be OR'ed together to trigger on multiple events.
-
-             - ``priority`` sets the priority level of the interrupt.  The values it
-               can take are port-specific, but higher values always represent higher
-               priorities.
-
-             - ``wake`` selects the power mode in which this interrupt can wake up the
-               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
-               These values can also be OR'ed together to make a pin generate interrupts in
-               more than one power mode.
-
-             - ``hard`` if true a hardware interrupt is used. This reduces the delay
-               between the pin change and the handler being called. Hard interrupt
-               handlers may not allocate memory; see :ref:`isr_rules`.
-               Not all ports support this argument.
-
-           This method returns a callback object.
-
-        The following methods are not part of the core Pin API and only implemented on certain ports.
-        """
-        ...
-    def off(self) -> None:
-        """
-        Set pin to "0" output level.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Set pin to "1" output level.
-        """
-        ...
-    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
-        """
-        Re-initialise the pin using the given parameters.  Only those arguments that
-        are specified will be set.  The rest of the pin peripheral state will remain
-        unchanged.  See the constructor documentation for details of the arguments.
-
-        Returns ``None``.
-        """
-        ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the pin, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the digital logic level of
-        the pin, returning 0 or 1 corresponding to low and high voltage signals
-        respectively.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The method returns the actual input value currently present
-            on the pin.
-          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
-          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
-            return value of the method is undefined.  Otherwise, if the pin is in
-            state '1', the method returns the actual input value currently present
-            on the pin.
-
-        If the argument is supplied then this method sets the digital logic level of
-        the pin.  The argument ``x`` can be anything that converts to a boolean.
-        If it converts to ``True``, the pin is set to state '1', otherwise it is set
-        to state '0'.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
-            pin state does not change, it remains in the high-impedance state.  The
-            stored value will become active on the pin as soon as it is changed to
-            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
-          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
-          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
-            state.  Otherwise the pin is set to high-impedance state.
-
-        When setting the value this method returns ``None``.
-        """
-        ...
-    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
-
-class WDT:
-    """
-    Create a WDT object and start it. The timeout must be given in milliseconds.
-    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
-
-    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
-    cannot be specified, it is determined by the underlying system.
-    """
-
-    def feed(self) -> None:
-        """
-        Feed the WDT to prevent it from resetting the system. The application
-        should place this call in a sensible place ensuring that the WDT is
-        only fed after verifying that everything is functioning correctly.
-        """
-        ...
-    def __init__(self, id=0, timeout=5000) -> None: ...
-
-class TouchPad:
-    def config(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class SDCard:
-    """
-    This class provides access to SD or MMC storage cards using either
-    a dedicated SD/MMC interface hardware or through an SPI channel.
-    The class implements the block protocol defined by :class:`os.AbstractBlockDev`.
-    This allows the mounting of an SD card to be as simple as::
-
-      os.mount(machine.SDCard(), "/sd")
-
-    The constructor takes the following parameters:
-
-     - *slot* selects which of the available interfaces to use. Leaving this
-       unset will select the default interface.
-
-     - *width* selects the bus width for the SD/MMC interface.
-
-     - *cd* can be used to specify a card-detect pin.
-
-     - *wp* can be used to specify a write-protect pin.
-
-     - *sck* can be used to specify an SPI clock pin.
-
-     - *miso* can be used to specify an SPI miso pin.
-
-     - *mosi* can be used to specify an SPI mosi pin.
-
-     - *cs* can be used to specify an SPI chip select pin.
-
-     - *freq* selects the SD/MMC interface frequency in Hz (only supported on the ESP32).
-    """
-
-    def ioctl(self, *args, **kwargs) -> Any: ...
-    def readblocks(self, *args, **kwargs) -> Any: ...
-    def writeblocks(self, *args, **kwargs) -> Any: ...
-    def info(self, *args, **kwargs) -> Any: ...
-    def deinit(self, *args, **kwargs) -> Any: ...
-    def __init__(self, slot=1, width=1, cd=None, wp=None, sck=None, miso=None, mosi=None, cs=None, freq=20000000) -> None: ...
-
-class RTC:
-    """
-    Create an RTC object. See init for parameters of initialization.
-    """
-
-    def init(self, datetime) -> None:
-        """
-        Initialise the RTC. Datetime is a tuple of the form:
-
-           ``(year, month, day[, hour[, minute[, second[, microsecond[, tzinfo]]]]])``
-        """
-        ...
-    def memory(self, *args, **kwargs) -> Any: ...
-    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
-        """
-        Get or set the date and time of the RTC.
-
-        With no arguments, this method returns an 8-tuple with the current
-        date and time.  With 1 argument (being an 8-tuple) it sets the date
-        and time.
-
-        The 8-tuple has the following format:
-
-            (year, month, day, weekday, hours, minutes, seconds, subseconds)
-
-        The meaning of the ``subseconds`` field is hardware dependent.
-        """
-        ...
-    def __init__(self, id=0, *args, **kwargs) -> None: ...
-
-class SoftI2C:
-    """
-    Construct a new software I2C object.  The parameters are:
-
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-       - *timeout* is the maximum time in microseconds to wait for clock
-         stretching (SCL held low by another device on the bus), after
-         which an ``OSError(ETIMEDOUT)`` exception is raised.
-    """
-
-    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_mem(self, *args, **kwargs) -> Any: ...
-    def writeto_mem(self, *args, **kwargs) -> Any: ...
-    def scan(self, *args, **kwargs) -> Any: ...
-    def writeto(self, *args, **kwargs) -> Any: ...
-    def writevto(self, *args, **kwargs) -> Any: ...
-    def start(self, *args, **kwargs) -> Any: ...
-    def readfrom(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def stop(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
-
-class SPI:
-    """
-    Construct an SPI object on the given bus, *id*. Values of *id* depend
-    on a particular port and its hardware. Values 0, 1, etc. are commonly used
-    to select hardware SPI block #0, #1, etc.
-
-    With no additional parameters, the SPI object is created but not
-    initialised (it has the settings from the last initialisation of
-    the bus, if any).  If extra arguments are given, the bus is initialised.
-    See ``init`` for parameters of initialisation.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self) -> None:
-        """
-        Turn off the SPI bus.
-        """
-        ...
-    def init(
-        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
-    ) -> None:
-        """
-        Initialise the SPI bus with the given parameters:
-
-          - ``baudrate`` is the SCK clock rate.
-          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
-          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
-            respectively.
-          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
-          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
-          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
-            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
-            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
-            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
-            (``id`` = -1).
-          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
-            specify them as a tuple of ``pins`` parameter.
-
-        In the case of hardware SPI the actual clock frequency may be lower than the
-        requested baudrate. This is dependant on the platform hardware. The actual
-        rate may be determined by printing the SPI object.
-        """
-        ...
-    def write_readinto(self, write_buf, read_buf) -> int:
-        """
-        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
-        buffers can be the same or different, but both buffers must have the
-        same length.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def read(self, nbytes, write=0x00) -> bytes:
-        """
-        Read a number of bytes specified by ``nbytes`` while continuously writing
-        the single byte given by ``write``.
-        Returns a ``bytes`` object with the data that was read.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes contained in ``buf``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def readinto(self, buf, write=0x00) -> int:
-        """
-        Read into the buffer specified by ``buf`` while continuously writing the
-        single byte given by ``write``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes read.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-class Signal:
-    """
-            Signal(pin_arguments..., *, invert=False)
-
-    Create a Signal object. There're two ways to create it:
-
-    * By wrapping existing Pin object - universal method which works for
-      any board.
-    * By passing required Pin parameters directly to Signal constructor,
-      skipping the need to create intermediate Pin object. Available on
-      many, but not all boards.
-
-    The arguments are:
-
-      - ``pin_obj`` is existing Pin object.
-
-      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
-
-      - ``invert`` - if True, the signal will be inverted (active low).
-    """
-
-    def off(self) -> None:
-        """
-        Deactivate signal.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Activate signal.
-        """
-        ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the signal, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the signal level, 1 meaning
-        signal is asserted (active) and 0 - signal inactive.
-
-        If the argument is supplied then this method sets the signal level. The
-        argument ``x`` can be anything that converts to a boolean. If it converts
-        to ``True``, the signal is active, otherwise it is inactive.
-
-        Correspondence between signal being active and actual logic level on the
-        underlying pin depends on whether signal is inverted (active-low) or not.
-        For non-inverted signal, active status corresponds to logical 1, inactive -
-        to logical 0. For inverted/active-low signal, active status corresponds
-        to logical 0, while inactive - to logical 1.
-        """
-        ...
-    def __init__(self, pin_obj, *args, invert=False) -> None: ...
+"""
+functions related to the hardware. See: https://docs.micropython.org/en/v1.20.0/library/machine.html
+
+The ``machine`` module contains specific functions related to the hardware
+on a particular board. Most functions in this module allow to achieve direct
+and unrestricted access to and control of hardware blocks on a system
+(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
+malfunction, lockups, crashes of your board, and in extreme cases, hardware
+damage.
+"""
+from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
+
+ULP_WAKE: int
+SLEEP: int
+PWRON_RESET: int
+PIN_WAKE: int
+SOFT_RESET: int
+WDT_RESET: int
+TOUCHPAD_WAKE: int
+TIMER_WAKE: int
+HARD_RESET: int
+EXT0_WAKE: int
+DEEPSLEEP_RESET: int
+DEEPSLEEP: int
+EXT1_WAKE: int
+
+def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def soft_reset() -> NoReturn:
+    """
+    Performs a soft reset of the interpreter, deleting all Python objects and
+    resetting the Python heap.  It tries to retain the method by which the user
+    is connected to the MicroPython REPL (eg serial, USB, Wifi).
+    """
+    ...
+
+def dht_readinto(*args, **kwargs) -> Any: ...
+def reset() -> NoReturn:
+    """
+    Resets the device in a manner similar to pushing the external RESET
+    button.
+    """
+    ...
+
+def unique_id() -> bytes:
+    """
+    Returns a byte string with a unique identifier of a board/SoC. It will vary
+    from a board/SoC instance to another, if underlying hardware allows. Length
+    varies by hardware (so use substring of a full value if you expect a short
+    ID). In some MicroPython ports, ID corresponds to the network MAC address.
+    """
+    ...
+
+def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
+    """
+    Time a pulse on the given *pin*, and return the duration of the pulse in
+    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
+    or 1 to time a high pulse.
+
+    If the current input value of the pin is different to *pulse_level*,
+    the function first (*) waits until the pin input becomes equal to *pulse_level*,
+    then (**) times the duration that the pin is equal to *pulse_level*.
+    If the pin is already equal to *pulse_level* then timing starts straight away.
+
+    The function will return -2 if there was timeout waiting for condition marked
+    (*) above, and -1 if there was timeout during the main measurement, marked (**)
+    above. The timeout is the same for both cases and given by *timeout_us* (which
+    is in microseconds).
+    """
+    ...
+
+def bitstream(pin, encoding, timing, data, /) -> Any:
+    """
+    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
+    specifies how the bits are encoded, and *timing* is an encoding-specific timing
+    specification.
+
+    The supported encodings are:
+
+      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
+        1 bits as timed pulses, starting with the most significant bit.
+        The *timing* must be a four-tuple of nanoseconds in the format
+        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
+        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
+        at 800kHz.
+
+    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
+    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
+    will be closer to +/-30ns.
+
+    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
+       module for a higher-level API.
+    """
+    ...
+
+def idle() -> Any:
+    """
+    Gates the clock to the CPU, useful to reduce power consumption at any time during
+    short or long periods. Peripherals continue working and execution resumes as soon
+    as any interrupt is triggered (on many ports this includes system timer
+    interrupt occurring at regular intervals on the order of millisecond).
+    """
+    ...
+
+def freq(hz: Optional[Any] = None) -> Any:
+    """
+    Returns the CPU frequency in hertz.
+
+    On some ports this can also be used to set the CPU frequency by passing in *hz*.
+    """
+    ...
+
+def lightsleep(time_ms: Optional[Any] = None) -> Any:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def disable_irq() -> Any:
+    """
+    Disable interrupt requests.
+    Returns the previous IRQ state which should be considered an opaque value.
+    This return value should be passed to the `enable_irq()` function to restore
+    interrupts to their original state, before `disable_irq()` was called.
+    """
+    ...
+
+def enable_irq(state) -> Any:
+    """
+    Re-enable interrupt requests.
+    The *state* parameter should be the value that was returned from the most
+    recent call to the `disable_irq()` function.
+    """
+    ...
+
+def reset_cause() -> int:
+    """
+    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
+    """
+    ...
+
+def sleep() -> Any:
+    """
+    ``Note:`` This function is deprecated, use `lightsleep()` instead with no arguments.
+    """
+    ...
+
+def wake_reason() -> Any:
+    """
+    Get the wake reason. See :ref:`constants <machine_constants>` for the possible return values.
+
+    Availability: ESP32, WiPy.
+    """
+    ...
+
+mem8: Any
+
+class PWM:
+    """
+    Construct and return a new PWM object using the following parameters:
+
+       - *dest* is the entity on which the PWM is output, which is usually a
+         :ref:`machine.Pin <machine.Pin>` object, but a port may allow other values,
+         like integers.
+       - *freq* should be an integer which sets the frequency in Hz for the
+         PWM cycle.
+       - *duty_u16* sets the duty cycle as a ratio ``duty_u16 / 65535``.
+       - *duty_ns* sets the pulse width in nanoseconds.
+
+    Setting *freq* may affect other PWM objects if the objects share the same
+    underlying PWM generator (this is hardware specific).
+    Only one of *duty_u16* and *duty_ns* should be specified at a time.
+    """
+
+    def duty_u16(self, value: Optional[Any] = None) -> int:
+        """
+        Get or set the current duty cycle of the PWM output, as an unsigned 16-bit
+        value in the range 0 to 65535 inclusive.
+
+        With no arguments the duty cycle is returned.
+
+        With a single *value* argument the duty cycle is set to that value, measured
+        as the ratio ``value / 65535``.
+        """
+        ...
+    def init(self, *, freq, duty_u16, duty_ns) -> None:
+        """
+        Modify settings for the PWM object.  See the above constructor for details
+        about the parameters.
+        """
+        ...
+    def freq(self, value: Optional[Any] = None) -> Any:
+        """
+        Get or set the current frequency of the PWM output.
+
+        With no arguments the frequency in Hz is returned.
+
+        With a single *value* argument the frequency is set to that value in Hz.  The
+        method may raise a ``ValueError`` if the frequency is outside the valid range.
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Disable the PWM output.
+        """
+        ...
+    def duty_ns(self, value: Optional[Any] = None) -> int:
+        """
+        Get or set the current pulse width of the PWM output, as a value in nanoseconds.
+
+        With no arguments the pulse width in nanoseconds is returned.
+
+        With a single *value* argument the pulse width is set to that value.
+        """
+        ...
+    def duty(self, *args, **kwargs) -> Any: ...
+    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None: ...
+
+class UART:
+    """
+    Construct a UART object of the given id.
+    """
+
+    INV_CTS: int
+    CTS: int
+    INV_TX: int
+    INV_RTS: int
+    INV_RX: int
+    RTS: int
+    def deinit(self) -> None:
+        """
+        Turn off the UART bus.
+
+        .. note::
+          You will not be able to call ``init()`` on the object after ``deinit()``.
+          A new instance needs to be created in that case.
+        """
+        ...
+    def sendbreak(self) -> None:
+        """
+        Send a break condition on the bus. This drives the bus low for a duration
+        longer than required for a normal transmission of a character.
+        """
+        ...
+    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
+        """
+        Initialise the UART bus with the given parameters:
+
+          - *baudrate* is the clock rate.
+          - *bits* is the number of bits per character, 7, 8 or 9.
+          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
+          - *stop* is the number of stop bits, 1 or 2.
+
+        Additional keyword-only parameters that may be supported by a port are:
+
+          - *tx* specifies the TX pin to use.
+          - *rx* specifies the RX pin to use.
+          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
+          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
+          - *txbuf* specifies the length in characters of the TX buffer.
+          - *rxbuf* specifies the length in characters of the RX buffer.
+          - *timeout* specifies the time to wait for the first character (in ms).
+          - *timeout_char* specifies the time to wait between characters (in ms).
+          - *invert* specifies which lines to invert.
+
+              - ``0`` will not invert lines (idle state of both lines is logic high).
+              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
+              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
+              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
+
+          - *flow* specifies which hardware flow control signals to use. The value
+            is a bitmask.
+
+              - ``0`` will ignore hardware flow control signals.
+              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
+                signal if the receive FIFO has sufficient space to accept more data.
+              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
+                CTS input pin signals that the receiver is running low on buffer space.
+              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
+
+        On the WiPy only the following keyword-only parameter is supported:
+
+          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
+            Any of the pins can be None if one wants the UART to operate with limited functionality.
+            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
+            When no pins are given, then the default set of TX and RX pins is taken, and hardware
+            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
+
+        .. note::
+          It is possible to call ``init()`` multiple times on the same object in
+          order to reconfigure  UART on the fly. That allows using single UART
+          peripheral to serve different devices attached to different GPIO pins.
+          Only one device can be served at a time in that case.
+          Also do not call ``deinit()`` as it will prevent calling ``init()``
+          again.
+        """
+        ...
+    def flush(self) -> Any:
+        """
+        Waits until all data has been sent. In case of a timeout, an exception is raised. The timeout
+        duration depends on the tx buffer size and the baud rate. Unless flow control is enabled, a timeout
+        should not occur.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call returns while the last byte is sent.
+            If required, a one character wait time has to be added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def txdone(self) -> bool:
+        """
+        Tells whether all data has been sent or no data transfer is happening. In this case,
+        it returns ``True``. If a data transmission is ongoing it returns ``False``.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call may return ``True`` even if the last byte
+            of a transfer is still being sent. If required, a one character wait time has to be
+            added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def read(self, nbytes: Optional[Any] = None) -> bytes:
+        """
+        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
+        otherwise read as much data as possible. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: a bytes object containing the bytes read in.  Returns ``None``
+        on timeout.
+        """
+        ...
+    def any(self) -> int:
+        """
+        Returns an integer counting the number of characters that can be read without
+        blocking.  It will return 0 if there are no characters available and a positive
+        number if there are characters.  The method may return 1 even if there is more
+        than one character available for reading.
+
+        For more sophisticated querying of available characters use select.poll::
+
+         poll = select.poll()
+         poll.register(uart, select.POLLIN)
+         poll.poll(timeout)
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the bus.
+
+        Return value: number of bytes written or ``None`` on timeout.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
+        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: number of bytes read and stored into ``buf`` or ``None`` on
+        timeout.
+        """
+        ...
+    def readline(self) -> None:
+        """
+        Read a line, ending in a newline character. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: the line read or ``None`` on timeout.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+mem32: Any
+mem16: Any
+
+class ADCBlock:
+    """
+    Access the ADC peripheral identified by *id*, which may be an integer
+    or string.
+
+    The *bits* argument, if given, sets the resolution in bits of the
+    conversion process.  If not specified then the previous or default
+    resolution is used.
+    """
+
+    def init(self, *, bits) -> None:
+        """
+        Configure the ADC peripheral.  *bits* will set the resolution of the
+        conversion process.
+        """
+        ...
+    def connect(self, channel, source) -> Any:
+        """
+        Connect up a channel on the ADC peripheral so it is ready for sampling,
+        and return an :ref:`ADC <machine.ADC>` object that represents that connection.
+
+        The *channel* argument must be an integer, and *source* must be an object
+        (for example a :ref:`Pin <machine.Pin>`) which can be connected up for sampling.
+
+        If only *channel* is given then it is configured for sampling.
+
+        If only *source* is given then that object is connected to a default
+        channel ready for sampling.
+
+        If both *channel* and *source* are given then they are connected together
+        and made ready for sampling.
+        """
+        ...
+    def __init__(self, id, *, bits) -> None: ...
+
+class ADC:
+    """
+    Access the ADC associated with a source identified by *id*.  This
+    *id* may be an integer (usually specifying a channel number), a
+    :ref:`Pin <machine.Pin>` object, or other value supported by the
+    underlying machine.
+
+    If additional keyword-arguments are given then they will configure
+    various aspects of the ADC.  If not given, these settings will take
+    previous or default values.  The settings are:
+
+      - *sample_ns* is the sampling time in nanoseconds.
+
+      - *atten* specifies the input attenuation.
+    """
+
+    ATTN_6DB: int
+    WIDTH_10BIT: int
+    WIDTH_11BIT: int
+    WIDTH_12BIT: int
+    WIDTH_9BIT: int
+    ATTN_0DB: int
+    ATTN_2_5DB: int
+    ATTN_11DB: int
+    def read_u16(self) -> int:
+        """
+        Take an analog reading and return an integer in the range 0-65535.
+        The return value represents the raw reading taken by the ADC, scaled
+        such that the minimum value is 0 and the maximum value is 65535.
+        """
+        ...
+    def init(self, *, sample_ns, atten) -> Any:
+        """
+        Apply the given settings to the ADC.  Only those arguments that are
+        specified will be changed.  See the ADC constructor above for what the
+        arguments are.
+        """
+        ...
+    def read_uv(self) -> int:
+        """
+        Take an analog reading and return an integer value with units of
+        microvolts.  It is up to the particular port whether or not this value
+        is calibrated, and how calibration is done.
+        """
+        ...
+    def width(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def block(self) -> Any:
+        """
+        Return the :ref:`ADCBlock <machine.ADCBlock>` instance associated with
+        this ADC object.
+
+        This method only exists if the port supports the
+        :ref:`ADCBlock <machine.ADCBlock>` class.
+        """
+        ...
+    def atten(self, *args, **kwargs) -> Any: ...
+    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
+
+class I2S:
+    """
+    Construct an I2S object of the given id:
+
+    - ``id`` identifies a particular I2S bus; it is board and port specific
+
+    Keyword-only parameters that are supported on all ports:
+
+      - ``sck`` is a pin object for the serial clock line
+      - ``ws`` is a pin object for the word select line
+      - ``sd`` is a pin object for the serial data line
+      - ``mck`` is a pin object for the master clock line;
+        master clock frequency is sampling rate * 256
+      - ``mode`` specifies receive or transmit
+      - ``bits`` specifies sample size (bits), 16 or 32
+      - ``format`` specifies channel format, STEREO or MONO
+      - ``rate`` specifies audio sampling rate (Hz);
+        this is the frequency of the ``ws`` signal
+      - ``ibuf`` specifies internal buffer length (bytes)
+
+    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
+    sample data is transfered between the internal buffer and the I2S peripheral unit.
+    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
+    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
+    """
+
+    RX: int
+    MONO: int
+    STEREO: int
+    TX: int
+    @staticmethod
+    def shift(*, buf, bits, shift) -> Any:
+        """
+        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
+        Positive for left shift, negative for right shift.
+        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
+        """
+        ...
+    def init(self, sck, *args, **kwargs) -> Any:
+        """
+        see Constructor for argument descriptions
+        """
+        ...
+    def irq(self, handler) -> Any:
+        """
+        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
+        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
+        ``handler`` is called in the context of the MicroPython scheduler.
+        """
+        ...
+    def readinto(self, buf) -> int:
+        """
+        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the left channel sample data is used.
+        Returns number of bytes read
+        """
+        ...
+    def deinit(self) -> Any:
+        """
+        Deinitialize the I2S bus
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the sample data is written to both the right and left channels.
+        Returns number of bytes written
+        """
+        ...
+    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
+
+class DAC:
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
+
+class I2C:
+    """
+    Construct and return a new I2C object using the following parameters:
+
+       - *id* identifies a particular I2C peripheral.  Allowed values for
+         depend on the particular port/board
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to allow for I2C
+         transactions.  This parameter is not allowed on some ports.
+
+    Note that some ports/boards will have default values of *scl* and *sda*
+    that can be changed in this constructor.  Others will have fixed values
+    of *scl* and *sda* that cannot be changed.
+    """
+
+    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.  The number of bytes read is the
+        length of *buf*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_into(self, addr, buf, stop=True, /) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr*.
+        The number of bytes read will be the length of *buf*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr* starting from the memory
+        address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Write *buf* to the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def scan(self) -> List:
+        """
+        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
+        those that respond.  A device responds if it pulls the SDA line low after
+        its address (including a write bit) is sent on the bus.
+        """
+        ...
+    def writeto(self, addr, buf, stop=True, /) -> int:
+        """
+        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
+        NACK is received following the write of a byte from *buf* then the
+        remaining bytes are not sent.  If *stop* is true then a STOP condition is
+        generated at the end of the transfer, even if a NACK is received.
+        The function returns the number of ACKs that were received.
+        """
+        ...
+    def writevto(self, addr, vector, stop=True, /) -> int:
+        """
+        Write the bytes contained in *vector* to the peripheral specified by *addr*.
+        *vector* should be a tuple or list of objects with the buffer protocol.
+        The *addr* is sent once and then the bytes from each object in *vector*
+        are written out sequentially.  The objects in *vector* may be zero bytes
+        in length in which case they don't contribute to the output.
+
+        If a NACK is received following the write of a byte from one of the
+        objects in *vector* then the remaining bytes, and any remaining objects,
+        are not sent.  If *stop* is true then a STOP condition is generated at
+        the end of the transfer, even if a NACK is received.  The function
+        returns the number of ACKs that were received.
+        """
+        ...
+    def start(self) -> None:
+        """
+        Generate a START condition on the bus (SDA transitions to low while SCL is high).
+        """
+        ...
+    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def readinto(self, buf, nack=True, /) -> Any:
+        """
+        Reads bytes from the bus and stores them into *buf*.  The number of bytes
+        read is the length of *buf*.  An ACK will be sent on the bus after
+        receiving all but the last byte.  After the last byte is received, if *nack*
+        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
+        case the peripheral assumes more bytes are going to be read in a later call).
+        """
+        ...
+    def init(self, scl, sda, *, freq=400000) -> None:
+        """
+        Initialise the I2C bus with the given arguments:
+
+           - *scl* is a pin object for the SCL line
+           - *sda* is a pin object for the SDA line
+           - *freq* is the SCL clock rate
+
+         In the case of hardware I2C the actual clock frequency may be lower than the
+         requested frequency. This is dependant on the platform hardware. The actual
+         rate may be determined by printing the I2C object.
+        """
+        ...
+    def stop(self) -> None:
+        """
+        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes from *buf* to the bus.  Checks that an ACK is received
+        after each byte and stops transmitting the remaining bytes if a NACK is
+        received.  The function returns the number of ACKs that were received.
+        """
+        ...
+    def __init__(
+        self,
+        id: Union[int, str] = -1,
+        *,
+        scl: Optional[Union[Pin, str]] = None,
+        sda: Optional[Union[Pin, str]] = None,
+        freq=400_000,
+        timeout=50000,
+    ) -> None: ...
+
+class Timer:
+    """
+    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
+    virtual timer (if supported by a board).
+    ``id`` shall not be passed as a keyword argument.
+
+    See ``init`` for parameters of initialisation.
+    """
+
+    ONE_SHOT: int
+    PERIODIC: int
+    def deinit(self) -> None:
+        """
+        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
+        """
+        ...
+    def init(self, *, mode=PERIODIC, freq=-1, period=-1, callback=None) -> None:
+        """
+        Initialise the timer. Example::
+
+            def mycallback(t):
+                pass
+
+            # periodic at 1kHz
+            tim.init(mode=Timer.PERIODIC, freq=1000, callback=mycallback)
+
+            # periodic with 100ms period
+            tim.init(period=100, callback=mycallback)
+
+            # one shot firing after 1000ms
+            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
+
+        Keyword arguments:
+
+          - ``mode`` can be one of:
+
+            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
+              period of the channel expires.
+            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
+              frequency of the channel.
+
+          - ``freq`` - The timer frequency, in units of Hz.  The upper bound of
+            the frequency is dependent on the port.  When both the ``freq`` and
+            ``period`` arguments are given, ``freq`` has a higher priority and
+            ``period`` is ignored.
+
+          - ``period`` - The timer period, in milliseconds.
+
+          - ``callback`` - The callable to call upon expiration of the timer period.
+            The callback must take one argument, which is passed the Timer object.
+            The ``callback`` argument shall be specified. Otherwise an exception
+            will occurr upon timer expiration:
+            ``TypeError: 'NoneType' object isn't callable``
+        """
+        ...
+    def value(self, *args, **kwargs) -> Any: ...
+    def __init__(self, id=-1, *args, **kwargs) -> None: ...
+
+class SoftSPI:
+    """
+    Construct a new software SPI object.  Additional parameters must be
+    given, usually at least *sck*, *mosi* and *miso*, and these are used
+    to initialise the bus.  See `SPI.init` for a description of the parameters.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def write_readinto(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
+
+class Pin:
+    """
+    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
+    additional arguments are given in the constructor then they are used to initialise
+    the pin.  Any settings that are not specified will remain in their previous state.
+
+    The arguments are:
+
+      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
+        types are: int (an internal Pin identifier), str (a Pin name), and tuple
+        (pair of [port, pin]).
+
+      - ``mode`` specifies the pin mode, which can be one of:
+
+        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
+          is in high-impedance state.
+
+        - ``Pin.OUT`` - Pin is configured for (normal) output.
+
+        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
+          output works in the following way: if the output value is set to 0 the pin
+          is active at a low level; if the output value is 1 the pin is in a high-impedance
+          state.  Not all ports implement this mode, or some might only on certain pins.
+
+        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
+          port specific.  For a pin configured in such a way any other Pin methods
+          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
+          or a hardware-specific, result).  Not all ports implement this mode.
+
+        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
+          open-drain.  Not all ports implement this mode.
+
+        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
+
+      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
+        one of:
+
+        - ``None`` - No pull up or down resistor.
+        - ``Pin.PULL_UP`` - Pull up resistor enabled.
+        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
+
+      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
+        output pin value if given, otherwise the state of the pin peripheral remains
+        unchanged.
+
+      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
+        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
+        capabilities are port dependent.  Not all ports implement this argument.
+
+      - ``alt`` specifies an alternate function for the pin and the values it can take are
+        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
+        modes.  It may be used when a pin supports more than one alternate function.  If only
+        one pin alternate function is supported the this argument is not required.  Not all
+        ports implement this argument.
+
+    As specified above, the Pin class allows to set an alternate function for a particular
+    pin, but it does not specify any further operations on such a pin.  Pins configured in
+    alternate-function mode are usually not used as GPIO but are instead driven by other
+    hardware peripherals.  The only operation supported on such a pin is re-initialising,
+    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
+    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
+    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
+    """
+
+    OPEN_DRAIN: int
+    IRQ_FALLING: int
+    IRQ_RISING: int
+    PULL_UP: int
+    OUT: int
+    PULL_DOWN: int
+    WAKE_HIGH: int
+    DRIVE_0: int
+    IN: int
+    WAKE_LOW: int
+    DRIVE_3: int
+    DRIVE_1: int
+    DRIVE_2: int
+    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
+        """
+           Configure an interrupt handler to be called when the trigger source of the
+           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
+           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
+           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
+           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
+           state '0' and the external pin value for state '1'.
+
+           The arguments are:
+
+             - ``handler`` is an optional function to be called when the interrupt
+               triggers. The handler must take exactly one argument which is the
+               ``Pin`` instance.
+
+             - ``trigger`` configures the event which can generate an interrupt.
+               Possible values are:
+
+               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
+               - ``Pin.IRQ_RISING`` interrupt on rising edge.
+               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
+               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
+
+               These values can be OR'ed together to trigger on multiple events.
+
+             - ``priority`` sets the priority level of the interrupt.  The values it
+               can take are port-specific, but higher values always represent higher
+               priorities.
+
+             - ``wake`` selects the power mode in which this interrupt can wake up the
+               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
+               These values can also be OR'ed together to make a pin generate interrupts in
+               more than one power mode.
+
+             - ``hard`` if true a hardware interrupt is used. This reduces the delay
+               between the pin change and the handler being called. Hard interrupt
+               handlers may not allocate memory; see :ref:`isr_rules`.
+               Not all ports support this argument.
+
+           This method returns a callback object.
+
+        The following methods are not part of the core Pin API and only implemented on certain ports.
+        """
+        ...
+    def off(self) -> None:
+        """
+        Set pin to "0" output level.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Set pin to "1" output level.
+        """
+        ...
+    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
+        """
+        Re-initialise the pin using the given parameters.  Only those arguments that
+        are specified will be set.  The rest of the pin peripheral state will remain
+        unchanged.  See the constructor documentation for details of the arguments.
+
+        Returns ``None``.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the pin, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the digital logic level of
+        the pin, returning 0 or 1 corresponding to low and high voltage signals
+        respectively.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The method returns the actual input value currently present
+            on the pin.
+          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
+          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
+            return value of the method is undefined.  Otherwise, if the pin is in
+            state '1', the method returns the actual input value currently present
+            on the pin.
+
+        If the argument is supplied then this method sets the digital logic level of
+        the pin.  The argument ``x`` can be anything that converts to a boolean.
+        If it converts to ``True``, the pin is set to state '1', otherwise it is set
+        to state '0'.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
+            pin state does not change, it remains in the high-impedance state.  The
+            stored value will become active on the pin as soon as it is changed to
+            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
+          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
+          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
+            state.  Otherwise the pin is set to high-impedance state.
+
+        When setting the value this method returns ``None``.
+        """
+        ...
+    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
+    def __call__(self, x: Optional[Any] = None) -> Any:
+        """
+        Pin objects are callable.  The call method provides a (fast) shortcut to set
+        and get the value of the pin.  It is equivalent to Pin.value([x]).
+        See :meth:`Pin.value` for more details.
+        """
+        ...
+
+class TouchPad:
+    def config(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
+
+class WDT:
+    """
+    Create a WDT object and start it. The timeout must be given in milliseconds.
+    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
+
+    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
+    cannot be specified, it is determined by the underlying system. On rp2040 devices,
+    the maximum timeout is 8388 ms.
+    """
+
+    def feed(self) -> None:
+        """
+        Feed the WDT to prevent it from resetting the system. The application
+        should place this call in a sensible place ensuring that the WDT is
+        only fed after verifying that everything is functioning correctly.
+        """
+        ...
+    def __init__(self, id=0, timeout=5000) -> None: ...
+
+class SDCard:
+    """
+    This class provides access to SD or MMC storage cards using either
+    a dedicated SD/MMC interface hardware or through an SPI channel.
+    The class implements the block protocol defined by :class:`os.AbstractBlockDev`.
+    This allows the mounting of an SD card to be as simple as::
+
+      os.mount(machine.SDCard(), "/sd")
+
+    The constructor takes the following parameters:
+
+     - *slot* selects which of the available interfaces to use. Leaving this
+       unset will select the default interface.
+
+     - *width* selects the bus width for the SD/MMC interface.
+
+     - *cd* can be used to specify a card-detect pin.
+
+     - *wp* can be used to specify a write-protect pin.
+
+     - *sck* can be used to specify an SPI clock pin.
+
+     - *miso* can be used to specify an SPI miso pin.
+
+     - *mosi* can be used to specify an SPI mosi pin.
+
+     - *cs* can be used to specify an SPI chip select pin.
+
+     - *freq* selects the SD/MMC interface frequency in Hz (only supported on the ESP32).
+    """
+
+    def ioctl(self, *args, **kwargs) -> Any: ...
+    def readblocks(self, *args, **kwargs) -> Any: ...
+    def writeblocks(self, *args, **kwargs) -> Any: ...
+    def info(self, *args, **kwargs) -> Any: ...
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def __init__(self, slot=1, width=1, cd=None, wp=None, sck=None, miso=None, mosi=None, cs=None, freq=20000000) -> None: ...
+
+class RTC:
+    """
+    Create an RTC object. See init for parameters of initialization.
+    """
+
+    def init(self, datetime) -> None:
+        """
+        Initialise the RTC. Datetime is a tuple of the form:
+
+           ``(year, month, day[, hour[, minute[, second[, microsecond[, tzinfo]]]]])``
+        """
+        ...
+    def memory(self, *args, **kwargs) -> Any: ...
+    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
+        """
+        Get or set the date and time of the RTC.
+
+        With no arguments, this method returns an 8-tuple with the current
+        date and time.  With 1 argument (being an 8-tuple) it sets the date
+        and time.
+
+        The 8-tuple has the following format:
+
+            (year, month, day, weekday, hours, minutes, seconds, subseconds)
+
+        The meaning of the ``subseconds`` field is hardware dependent.
+        """
+        ...
+    def __init__(self, id=0, *args, **kwargs) -> None: ...
+
+class SoftI2C(I2C):
+    """
+    Construct a new software I2C object.  The parameters are:
+
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to wait for clock
+         stretching (SCL held low by another device on the bus), after
+         which an ``OSError(ETIMEDOUT)`` exception is raised.
+    """
+
+    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_mem(self, *args, **kwargs) -> Any: ...
+    def writeto_mem(self, *args, **kwargs) -> Any: ...
+    def scan(self, *args, **kwargs) -> Any: ...
+    def writeto(self, *args, **kwargs) -> Any: ...
+    def writevto(self, *args, **kwargs) -> Any: ...
+    def start(self, *args, **kwargs) -> Any: ...
+    def readfrom(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def stop(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
+
+class SPI:
+    """
+    Construct an SPI object on the given bus, *id*. Values of *id* depend
+    on a particular port and its hardware. Values 0, 1, etc. are commonly used
+    to select hardware SPI block #0, #1, etc.
+
+    With no additional parameters, the SPI object is created but not
+    initialised (it has the settings from the last initialisation of
+    the bus, if any).  If extra arguments are given, the bus is initialised.
+    See ``init`` for parameters of initialisation.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self) -> None:
+        """
+        Turn off the SPI bus.
+        """
+        ...
+    def init(
+        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
+    ) -> None:
+        """
+        Initialise the SPI bus with the given parameters:
+
+          - ``baudrate`` is the SCK clock rate.
+          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
+          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
+            respectively.
+          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
+          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
+          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
+            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
+            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
+            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
+            (``id`` = -1).
+          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
+            specify them as a tuple of ``pins`` parameter.
+
+        In the case of hardware SPI the actual clock frequency may be lower than the
+        requested baudrate. This is dependant on the platform hardware. The actual
+        rate may be determined by printing the SPI object.
+        """
+        ...
+    def write_readinto(self, write_buf, read_buf) -> int:
+        """
+        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
+        buffers can be the same or different, but both buffers must have the
+        same length.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def read(self, nbytes, write=0x00) -> bytes:
+        """
+        Read a number of bytes specified by ``nbytes`` while continuously writing
+        the single byte given by ``write``.
+        Returns a ``bytes`` object with the data that was read.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes contained in ``buf``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def readinto(self, buf, write=0x00) -> int:
+        """
+        Read into the buffer specified by ``buf`` while continuously writing the
+        single byte given by ``write``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes read.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+class Signal(Pin):
+    """
+            Signal(pin_arguments..., *, invert=False)
+
+    Create a Signal object. There're two ways to create it:
+
+    * By wrapping existing Pin object - universal method which works for
+      any board.
+    * By passing required Pin parameters directly to Signal constructor,
+      skipping the need to create intermediate Pin object. Available on
+      many, but not all boards.
+
+    The arguments are:
+
+      - ``pin_obj`` is existing Pin object.
+
+      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
+
+      - ``invert`` - if True, the signal will be inverted (active low).
+    """
+
+    def off(self) -> None:
+        """
+        Deactivate signal.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Activate signal.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the signal, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the signal level, 1 meaning
+        signal is asserted (active) and 0 - signal inactive.
+
+        If the argument is supplied then this method sets the signal level. The
+        argument ``x`` can be anything that converts to a boolean. If it converts
+        to ``True``, the signal is active, otherwise it is inactive.
+
+        Correspondence between signal being active and actual logic level on the
+        underlying pin depends on whether signal is inverted (active-low) or not.
+        For non-inverted signal, active status corresponds to logical 1, inactive -
+        to logical 0. For inverted/active-low signal, active status corresponds
+        to logical 0, while inactive - to logical 1.
+        """
+        ...
+    def __init__(self, pin_obj, *args, invert=False) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/micropython.pyi` & `micropython_esp32_stubs-1.20.0.post1/micropython.pyi`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-"""
-access and control MicroPython internals. See: https://docs.micropython.org/en/v1.19.1/library/micropython.html
-"""
-from typing import Optional, Any, Callable
-
-def opt_level(level: Optional[Any] = None) -> Any:
-    """
-    If *level* is given then this function sets the optimisation level for subsequent
-    compilation of scripts, and returns ``None``.  Otherwise it returns the current
-    optimisation level.
-
-    The optimisation level controls the following compilation features:
-
-    - Assertions: at level 0 assertion statements are enabled and compiled into the
-      bytecode; at levels 1 and higher assertions are not compiled.
-    - Built-in ``__debug__`` variable: at level 0 this variable expands to ``True``;
-      at levels 1 and higher it expands to ``False``.
-    - Source-code line numbers: at levels 0, 1 and 2 source-code line number are
-      stored along with the bytecode so that exceptions can report the line number
-      they occurred at; at levels 3 and higher line numbers are not stored.
-
-    The default optimisation level is usually level 0.
-    """
-    ...
-
-def mem_info(verbose: Optional[Any] = None) -> None:
-    """
-    Print information about currently used memory.  If the *verbose* argument
-    is given then extra information is printed.
-
-    The information that is printed is implementation dependent, but currently
-    includes the amount of stack and heap used.  In verbose mode it prints out
-    the entire heap indicating which blocks are used and which are free.
-    """
-    ...
-
-def stack_use() -> int:
-    """
-    Return an integer representing the current amount of stack that is being
-    used.  The absolute value of this is not particularly useful, rather it
-    should be used to compute differences in stack usage at different points.
-    """
-    ...
-
-def qstr_info(verbose: Optional[Any] = None) -> None:
-    """
-    Print information about currently interned strings.  If the *verbose*
-    argument is given then extra information is printed.
-
-    The information that is printed is implementation dependent, but currently
-    includes the number of interned strings and the amount of RAM they use.  In
-    verbose mode it prints out the names of all RAM-interned strings.
-    """
-    ...
-
-def schedule(func, arg) -> Any:
-    """
-    Schedule the function *func* to be executed "very soon".  The function
-    is passed the value *arg* as its single argument.  "Very soon" means that
-    the MicroPython runtime will do its best to execute the function at the
-    earliest possible time, given that it is also trying to be efficient, and
-    that the following conditions hold:
-
-    - A scheduled function will never preempt another scheduled function.
-    - Scheduled functions are always executed "between opcodes" which means
-      that all fundamental Python operations (such as appending to a list)
-      are guaranteed to be atomic.
-    - A given port may define "critical regions" within which scheduled
-      functions will never be executed.  Functions may be scheduled within
-      a critical region but they will not be executed until that region
-      is exited.  An example of a critical region is a preempting interrupt
-      handler (an IRQ).
-
-    A use for this function is to schedule a callback from a preempting IRQ.
-    Such an IRQ puts restrictions on the code that runs in the IRQ (for example
-    the heap may be locked) and scheduling a function to call later will lift
-    those restrictions.
-
-    Note: If `schedule()` is called from a preempting IRQ, when memory
-    allocation is not allowed and the callback to be passed to `schedule()` is
-    a bound method, passing this directly will fail. This is because creating a
-    reference to a bound method causes memory allocation. A solution is to
-    create a reference to the method in the class constructor and to pass that
-    reference to `schedule()`. This is discussed in detail here
-    :ref:`reference documentation <isr_rules>` under "Creation of Python
-    objects".
-
-    There is a finite queue to hold the scheduled functions and `schedule()`
-    will raise a `RuntimeError` if the queue is full.
-    """
-    ...
-
-def alloc_emergency_exception_buf(size) -> Any:
-    """
-    Allocate *size* bytes of RAM for the emergency exception buffer (a good
-    size is around 100 bytes).  The buffer is used to create exceptions in cases
-    when normal RAM allocation would fail (eg within an interrupt handler) and
-    therefore give useful traceback information in these situations.
-
-    A good way to use this function is to put it at the start of your main script
-    (eg ``boot.py`` or ``main.py``) and then the emergency exception buffer will be active
-    for all the code following it.
-    """
-    ...
-
-def const(expr) -> int:
-    """
-    Used to declare that the expression is a constant so that the compile can
-    optimise it.  The use of this function should be as follows::
-
-     from micropython import const
-
-     CONST_X = const(123)
-     CONST_Y = const(2 * CONST_X + 1)
-
-    Constants declared this way are still accessible as global variables from
-    outside the module they are declared in.  On the other hand, if a constant
-    begins with an underscore then it is hidden, it is not available as a global
-    variable, and does not take up any memory during execution.
-
-    This `const` function is recognised directly by the MicroPython parser and is
-    provided as part of the :mod:`micropython` module mainly so that scripts can be
-    written which run under both CPython and MicroPython, by following the above
-    pattern.
-    """
-    ...
-
-def kbd_intr(chr) -> None:
-    """
-    Set the character that will raise a `KeyboardInterrupt` exception.  By
-    default this is set to 3 during script execution, corresponding to Ctrl-C.
-    Passing -1 to this function will disable capture of Ctrl-C, and passing 3
-    will restore it.
-
-    This function can be used to prevent the capturing of Ctrl-C on the
-    incoming stream of characters that is usually used for the REPL, in case
-    that stream is used for other purposes.
-    """
-    ...
-
-def heap_lock() -> Any: ...
-def heap_unlock() -> Any: ...
-def viper(func: Callable) -> Callable:
-    """
-    The Viper code emitter is not fully compliant. It supports special Viper native data types in pursuit of performance.
-    Integer processing is non-compliant because it uses machine words: arithmetic on 32 bit hardware is performed modulo 2**32.
-    Like the Native emitter Viper produces machine instructions but further optimisations are performed, substantially increasing
-    performance especially for integer arithmetic and bit manipulations.
-    """
-    ...
-
-def native(func: Callable) -> Callable:
-    """
-    This causes the MicroPython compiler to emit native CPU opcodes rather than bytecode.
-    It covers the bulk of the MicroPython functionality, so most functions will require no adaptation.
-    See: https://docs.micropython.org/en/latest/reference/speed_python.html?highlight=viper#the-native-code-emitter
-    """
-    ...
+"""
+access and control MicroPython internals. See: https://docs.micropython.org/en/v1.19.1/library/micropython.html
+"""
+from typing import Optional, Any, Callable
+
+def opt_level(level: Optional[Any] = None) -> Any:
+    """
+    If *level* is given then this function sets the optimisation level for subsequent
+    compilation of scripts, and returns ``None``.  Otherwise it returns the current
+    optimisation level.
+
+    The optimisation level controls the following compilation features:
+
+    - Assertions: at level 0 assertion statements are enabled and compiled into the
+      bytecode; at levels 1 and higher assertions are not compiled.
+    - Built-in ``__debug__`` variable: at level 0 this variable expands to ``True``;
+      at levels 1 and higher it expands to ``False``.
+    - Source-code line numbers: at levels 0, 1 and 2 source-code line number are
+      stored along with the bytecode so that exceptions can report the line number
+      they occurred at; at levels 3 and higher line numbers are not stored.
+
+    The default optimisation level is usually level 0.
+    """
+    ...
+
+def mem_info(verbose: Optional[Any] = None) -> None:
+    """
+    Print information about currently used memory.  If the *verbose* argument
+    is given then extra information is printed.
+
+    The information that is printed is implementation dependent, but currently
+    includes the amount of stack and heap used.  In verbose mode it prints out
+    the entire heap indicating which blocks are used and which are free.
+    """
+    ...
+
+def stack_use() -> int:
+    """
+    Return an integer representing the current amount of stack that is being
+    used.  The absolute value of this is not particularly useful, rather it
+    should be used to compute differences in stack usage at different points.
+    """
+    ...
+
+def qstr_info(verbose: Optional[Any] = None) -> None:
+    """
+    Print information about currently interned strings.  If the *verbose*
+    argument is given then extra information is printed.
+
+    The information that is printed is implementation dependent, but currently
+    includes the number of interned strings and the amount of RAM they use.  In
+    verbose mode it prints out the names of all RAM-interned strings.
+    """
+    ...
+
+def schedule(func, arg) -> Any:
+    """
+    Schedule the function *func* to be executed "very soon".  The function
+    is passed the value *arg* as its single argument.  "Very soon" means that
+    the MicroPython runtime will do its best to execute the function at the
+    earliest possible time, given that it is also trying to be efficient, and
+    that the following conditions hold:
+
+    - A scheduled function will never preempt another scheduled function.
+    - Scheduled functions are always executed "between opcodes" which means
+      that all fundamental Python operations (such as appending to a list)
+      are guaranteed to be atomic.
+    - A given port may define "critical regions" within which scheduled
+      functions will never be executed.  Functions may be scheduled within
+      a critical region but they will not be executed until that region
+      is exited.  An example of a critical region is a preempting interrupt
+      handler (an IRQ).
+
+    A use for this function is to schedule a callback from a preempting IRQ.
+    Such an IRQ puts restrictions on the code that runs in the IRQ (for example
+    the heap may be locked) and scheduling a function to call later will lift
+    those restrictions.
+
+    Note: If `schedule()` is called from a preempting IRQ, when memory
+    allocation is not allowed and the callback to be passed to `schedule()` is
+    a bound method, passing this directly will fail. This is because creating a
+    reference to a bound method causes memory allocation. A solution is to
+    create a reference to the method in the class constructor and to pass that
+    reference to `schedule()`. This is discussed in detail here
+    :ref:`reference documentation <isr_rules>` under "Creation of Python
+    objects".
+
+    There is a finite queue to hold the scheduled functions and `schedule()`
+    will raise a `RuntimeError` if the queue is full.
+    """
+    ...
+
+def alloc_emergency_exception_buf(size) -> Any:
+    """
+    Allocate *size* bytes of RAM for the emergency exception buffer (a good
+    size is around 100 bytes).  The buffer is used to create exceptions in cases
+    when normal RAM allocation would fail (eg within an interrupt handler) and
+    therefore give useful traceback information in these situations.
+
+    A good way to use this function is to put it at the start of your main script
+    (eg ``boot.py`` or ``main.py``) and then the emergency exception buffer will be active
+    for all the code following it.
+    """
+    ...
+
+def const(expr) -> int:
+    """
+    Used to declare that the expression is a constant so that the compile can
+    optimise it.  The use of this function should be as follows::
+
+     from micropython import const
+
+     CONST_X = const(123)
+     CONST_Y = const(2 * CONST_X + 1)
+
+    Constants declared this way are still accessible as global variables from
+    outside the module they are declared in.  On the other hand, if a constant
+    begins with an underscore then it is hidden, it is not available as a global
+    variable, and does not take up any memory during execution.
+
+    This `const` function is recognised directly by the MicroPython parser and is
+    provided as part of the :mod:`micropython` module mainly so that scripts can be
+    written which run under both CPython and MicroPython, by following the above
+    pattern.
+    """
+    ...
+
+def kbd_intr(chr) -> None:
+    """
+    Set the character that will raise a `KeyboardInterrupt` exception.  By
+    default this is set to 3 during script execution, corresponding to Ctrl-C.
+    Passing -1 to this function will disable capture of Ctrl-C, and passing 3
+    will restore it.
+
+    This function can be used to prevent the capturing of Ctrl-C on the
+    incoming stream of characters that is usually used for the REPL, in case
+    that stream is used for other purposes.
+    """
+    ...
+
+def heap_lock() -> Any: ...
+def heap_unlock() -> Any: ...
+def viper(func: Callable) -> Callable:
+    """
+    The Viper code emitter is not fully compliant. It supports special Viper native data types in pursuit of performance.
+    Integer processing is non-compliant because it uses machine words: arithmetic on 32 bit hardware is performed modulo 2**32.
+    Like the Native emitter Viper produces machine instructions but further optimisations are performed, substantially increasing
+    performance especially for integer arithmetic and bit manipulations.
+    """
+    ...
+
+def native(func: Callable) -> Callable:
+    """
+    This causes the MicroPython compiler to emit native CPU opcodes rather than bytecode.
+    It covers the bulk of the MicroPython functionality, so most functions will require no adaptation.
+    See: https://docs.micropython.org/en/latest/reference/speed_python.html?highlight=viper#the-native-code-emitter
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/network.pyi` & `micropython_esp32_stubs-1.20.0.post1/network.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,269 +1,276 @@
-"""
-network configuration. See: https://docs.micropython.org/en/v1.19.1/library/network.html
-
-This module provides network drivers and routing configuration. To use this
-module, a MicroPython variant/build with network capabilities must be installed.
-Network drivers for specific hardware are available within this module and are
-used to configure hardware network interface(s). Network services provided
-by configured interfaces are then available for use via the :mod:`socket`
-module.
-
-For example::
-
-    # connect/ show IP config a specific network interface
-    # see below for examples of specific drivers
-    import network
-    import time
-    nic = network.Driver(...)
-    if not nic.isconnected():
-        nic.connect()
-        print("Waiting for connection...")
-        while not nic.isconnected():
-            time.sleep(1)
-    print(nic.ifconfig())
-
-    # now use socket as usual
-    import socket
-    addr = socket.getaddrinfo('micropython.org', 80)[0][-1]
-    s = socket.socket()
-    s.connect(addr)
-    s.send(b'GET / HTTP/1.1\r\nHost: micropython.org\r\n\r\n')
-    data = s.recv(1000)
-    s.close()
-"""
-from typing import List, Optional, Tuple, Union, Any
-
-STAT_WRONG_PASSWORD: int
-PHY_IP101: int
-PHY_LAN8720: int
-PHY_RTL8201: int
-PHY_DP83848: int
-MODE_11B: int
-MODE_11G: int
-MODE_11N: int
-STA_IF: int
-STAT_HANDSHAKE_TIMEOUT: int
-STAT_IDLE: int
-STAT_NO_AP_FOUND: int
-STAT_GOT_IP: int
-STAT_ASSOC_FAIL: int
-STAT_BEACON_TIMEOUT: int
-STAT_CONNECTING: int
-AUTH_WPA3_PSK: int
-AUTH_WPA2_ENTERPRISE: int
-AUTH_WPA2_PSK: int
-AUTH_WPA2_WPA3_PSK: int
-AUTH_WEP: int
-AP_IF: int
-AUTH_MAX: int
-AUTH_OPEN: int
-ETH_STOPPED: int
-ETH_INITIALIZED: int
-ETH_GOT_IP: int
-ETH_STARTED: int
-AUTH_WPA_PSK: int
-AUTH_WPA_WPA2_PSK: int
-ETH_DISCONNECTED: int
-ETH_CONNECTED: int
-
-class WLAN:
-    """
-    Create a WLAN network interface object. Supported interfaces are
-    ``network.STA_IF`` (station aka client, connects to upstream WiFi access
-    points) and ``network.AP_IF`` (access point, allows other WiFi clients to
-    connect). Availability of the methods below depends on interface type.
-    For example, only STA interface may `WLAN.connect()` to an access point.
-    """
-
-    def __init__(self, interface_id) -> None: ...
-    def active(self, is_active: Optional[Any] = None) -> None:
-        """
-        Activate ("up") or deactivate ("down") network interface, if boolean
-        argument is passed. Otherwise, query current state if no argument is
-        provided. Most other methods require active interface.
-        """
-        ...
-    def connect(self, ssid=None, password=None, *, bssid=None) -> None:
-        """
-        Connect to the specified wireless network, using the specified password.
-        If *bssid* is given then the connection will be restricted to the
-        access-point with that MAC address (the *ssid* must also be specified
-        in this case).
-        """
-        ...
-    def disconnect(self) -> None:
-        """
-        Disconnect from the currently connected wireless network.
-        """
-        ...
-    def scan(self) -> List[Tuple]:
-        """
-        Scan for the available wireless networks.
-        Hidden networks -- where the SSID is not broadcast -- will also be scanned
-        if the WLAN interface allows it.
-
-        Scanning is only possible on STA interface. Returns list of tuples with
-        the information about WiFi access points:
-
-            (ssid, bssid, channel, RSSI, authmode, hidden)
-
-        *bssid* is hardware address of an access point, in binary form, returned as
-        bytes object. You can use `binascii.hexlify()` to convert it to ASCII form.
-
-        There are five values for authmode:
-
-            * 0 -- open
-            * 1 -- WEP
-            * 2 -- WPA-PSK
-            * 3 -- WPA2-PSK
-            * 4 -- WPA/WPA2-PSK
-
-        and two for hidden:
-
-            * 0 -- visible
-            * 1 -- hidden
-        """
-        ...
-    def status(self, param: Optional[Any] = None) -> Any:
-        """
-        Return the current status of the wireless connection.
-
-        When called with no argument the return value describes the network link status.
-        The possible statuses are defined as constants:
-
-            * ``STAT_IDLE`` -- no connection and no activity,
-            * ``STAT_CONNECTING`` -- connecting in progress,
-            * ``STAT_WRONG_PASSWORD`` -- failed due to incorrect password,
-            * ``STAT_NO_AP_FOUND`` -- failed because no access point replied,
-            * ``STAT_CONNECT_FAIL`` -- failed due to other problems,
-            * ``STAT_GOT_IP`` -- connection successful.
-
-        When called with one argument *param* should be a string naming the status
-        parameter to retrieve.  Supported parameters in WiFI STA mode are: ``'rssi'``.
-        """
-        ...
-    def isconnected(self) -> bool:
-        """
-        In case of STA mode, returns ``True`` if connected to a WiFi access
-        point and has a valid IP address.  In AP mode returns ``True`` when a
-        station is connected. Returns ``False`` otherwise.
-        """
-        ...
-    def ifconfig(self, configtuple: Optional[Any] = None) -> Tuple:
-        """
-        Get/set IP-level network interface parameters: IP address, subnet mask,
-        gateway and DNS server. When called with no arguments, this method returns
-        a 4-tuple with the above information. To set the above values, pass a
-        4-tuple with the required information.  For example::
-
-         nic.ifconfig(('192.168.0.4', '255.255.255.0', '192.168.0.1', '8.8.8.8'))
-        """
-        ...
-    def config(self, *args, **kwargs) -> Any:
-        """
-        Get or set general network interface parameters. These methods allow to work
-        with additional parameters beyond standard IP configuration (as dealt with by
-        `WLAN.ifconfig()`). These include network-specific and hardware-specific
-        parameters. For setting parameters, keyword argument syntax should be used,
-        multiple parameters can be set at once. For querying, parameters name should
-        be quoted as a string, and only one parameter can be queries at time::
-
-         # Set WiFi access point name (formally known as ESSID) and WiFi channel
-         ap.config(essid='My AP', channel=11)
-         # Query params one by one
-         print(ap.config('essid'))
-         print(ap.config('channel'))
-
-        Following are commonly supported parameters (availability of a specific parameter
-        depends on network technology type, driver, and :term:`MicroPython port`).
-
-        =============  ===========
-        Parameter      Description
-        =============  ===========
-        mac            MAC address (bytes)
-        essid          WiFi access point name (string)
-        channel        WiFi channel (integer)
-        hidden         Whether ESSID is hidden (boolean)
-        authmode       Authentication mode supported (enumeration, see module constants)
-        password       Access password (string)
-        dhcp_hostname  The DHCP hostname to use
-        reconnects     Number of reconnect attempts to make (integer, 0=none, -1=unlimited)
-        txpower        Maximum transmit power in dBm (integer or float)
-        =============  ===========
-        """
-        ...
-
-def phy_mode(*args, **kwargs) -> Any: ...
-def PPP(*args, **kwargs) -> Any: ...
-
-class LAN:
-    """
-    Create a LAN driver object, initialise the LAN module using the given
-    PHY driver name, and return the LAN object.
-
-    Arguments are:
-
-      - *id* is the number of the Ethernet port, either 0 or 1.
-      - *phy_type* is the name of the PHY driver. For most board the on-board PHY has to be used and
-        is the default. Suitable values are port specific.
-      - *phy_addr* specifies the address of the PHY interface. As with *phy_type*, the hardwired value has
-        to be used for most boards and that value is the default.
-      - *phy_clock* specifies, whether the data clock is provided by the Ethernet controller or the PYH interface.
-        The default value is the one that matches the board. If set to ``True``, the clock is driven by the
-        Ethernet controller, otherwise by the PHY interface.
-
-    For example, with the Seeed Arch Mix board you can  use::
-
-      nic = LAN(0, phy_type=LAN.PHY_LAN8720, phy_addr=2, phy_clock=False)
-    """
-
-    def __init__(self, id, *, phy_type=0, phy_addr=0, phy_clock=0) -> None: ...
-    def active(self, state: Optional[Any] = None) -> Any:
-        """
-        With a parameter, it sets the interface active if *state* is true, otherwise it
-        sets it inactive.
-        Without a parameter, it returns the state.
-        """
-        ...
-    def isconnected(self) -> bool:
-        """
-        Returns ``True`` if the physical Ethernet link is connected and up.
-        Returns ``False`` otherwise.
-        """
-        ...
-    def status(self) -> Any:
-        """
-        Returns the LAN status.
-        """
-        ...
-    def ifconfig(self, configtuple: Optional[Any] = None) -> Tuple:
-        """
-        Get/set IP address, subnet mask, gateway and DNS.
-
-        When called with no arguments, this method returns a 4-tuple with the above information.
-
-        To set the above values, pass a 4-tuple with the required information.  For example::
-
-         nic.ifconfig(('192.168.0.4', '255.255.255.0', '192.168.0.1', '8.8.8.8'))
-        """
-        ...
-    def config(self, config_parameters) -> Any:
-        """
-        Sets or gets parameters of the LAN interface. The only parameter that can be
-        retrieved is the MAC address, using::
-
-           mac = LAN.config("mac")
-
-        The parameters that can be set are:
-
-         - ``trace=n`` sets trace levels; suitable values are:
-
-             - 2: trace TX
-             - 4: trace RX
-             - 8: full trace
-
-         - ``low_power=bool`` sets or clears low power mode, valid values being ``False``
-           or ``True``.
-
-        """
-        ...
+"""
+network configuration. See: https://docs.micropython.org/en/v1.20.0/library/network.html
+
+This module provides network drivers and routing configuration. To use this
+module, a MicroPython variant/build with network capabilities must be installed.
+Network drivers for specific hardware are available within this module and are
+used to configure hardware network interface(s). Network services provided
+by configured interfaces are then available for use via the :mod:`socket`
+module.
+
+For example::
+
+    # connect/ show IP config a specific network interface
+    # see below for examples of specific drivers
+    import network
+    import time
+    nic = network.Driver(...)
+    if not nic.isconnected():
+        nic.connect()
+        print("Waiting for connection...")
+        while not nic.isconnected():
+            time.sleep(1)
+    print(nic.ifconfig())
+
+    # now use socket as usual
+    import socket
+    addr = socket.getaddrinfo('micropython.org', 80)[0][-1]
+    s = socket.socket()
+    s.connect(addr)
+    s.send(b'GET / HTTP/1.1\r\nHost: micropython.org\r\n\r\n')
+    data = s.recv(1000)
+    s.close()
+"""
+from typing import List, Optional, Tuple, Union, Any
+
+PHY_LAN8720: int
+PHY_DP83848: int
+PHY_IP101: int
+PHY_LAN8710: int
+MODE_LR: int
+MODE_11B: int
+MODE_11G: int
+MODE_11N: int
+STAT_NO_AP_FOUND: int
+PHY_RTL8201: int
+STAT_GOT_IP: int
+STAT_HANDSHAKE_TIMEOUT: int
+STAT_IDLE: int
+STAT_CONNECTING: int
+STAT_WRONG_PASSWORD: int
+STAT_ASSOC_FAIL: int
+STAT_BEACON_TIMEOUT: int
+AUTH_WPA3_PSK: int
+AUTH_WPA2_ENTERPRISE: int
+AUTH_WPA2_PSK: int
+AUTH_WPA2_WPA3_PSK: int
+AUTH_WEP: int
+AP_IF: int
+AUTH_MAX: int
+AUTH_OPEN: int
+STA_IF: int
+AUTH_WPA_PSK: int
+ETH_INITIALIZED: int
+ETH_STARTED: int
+ETH_STOPPED: int
+ETH_GOT_IP: int
+AUTH_WPA_WPA2_PSK: int
+ETH_CONNECTED: int
+ETH_DISCONNECTED: int
+
+def phy_mode(*args, **kwargs) -> Any: ...
+def country(*args, **kwargs) -> Any: ...
+def hostname(*args, **kwargs) -> Any: ...
+
+class LAN:
+    """
+    Create a LAN driver object, initialise the LAN module using the given
+    PHY driver name, and return the LAN object.
+
+    Arguments are:
+
+      - *id* is the number of the Ethernet port, either 0 or 1.
+      - *phy_type* is the name of the PHY driver. For most board the on-board PHY has to be used and
+        is the default. Suitable values are port specific.
+      - *phy_addr* specifies the address of the PHY interface. As with *phy_type*, the hardwired value has
+        to be used for most boards and that value is the default.
+      - *ref_clk_mode* specifies, whether the data clock is provided by the Ethernet controller or
+        the PYH interface.
+        The default value is the one that matches the board. If set to ``LAN.OUT`` or ``Pin.OUT``
+        or ``True``, the clock is driven by the Ethernet controller, if set to ``LAN.IN``
+        or ``Pin.IN`` or ``False``, the clock is driven by the PHY interface.
+
+    For example, with the Seeed Arch Mix board you can  use::
+
+      nic = LAN(0, phy_type=LAN.PHY_LAN8720, phy_addr=1, ref_clk_mode=Pin.IN)
+    """
+
+    def __init__(self, id, *, phy_type=0, phy_addr=0, ref_clk_mode=0) -> None: ...
+    def active(self, state: Optional[Any] = None) -> Any:
+        """
+        With a parameter, it sets the interface active if *state* is true, otherwise it
+        sets it inactive.
+        Without a parameter, it returns the state.
+        """
+        ...
+    def isconnected(self) -> bool:
+        """
+        Returns ``True`` if the physical Ethernet link is connected and up.
+        Returns ``False`` otherwise.
+        """
+        ...
+    def status(self) -> Any:
+        """
+        Returns the LAN status.
+        """
+        ...
+    def ifconfig(self, configtuple: Optional[Any] = None) -> Tuple:
+        """
+        Get/set IP address, subnet mask, gateway and DNS.
+
+        When called with no arguments, this method returns a 4-tuple with the above information.
+
+        To set the above values, pass a 4-tuple with the required information.  For example::
+
+         nic.ifconfig(('192.168.0.4', '255.255.255.0', '192.168.0.1', '8.8.8.8'))
+        """
+        ...
+    def config(self, config_parameters) -> Any:
+        """
+        Sets or gets parameters of the LAN interface. The only parameter that can be
+        retrieved is the MAC address, using::
+
+           mac = LAN.config("mac")
+
+        The parameters that can be set are:
+
+         - ``trace=n`` sets trace levels; suitable values are:
+
+             - 2: trace TX
+             - 4: trace RX
+             - 8: full trace
+
+         - ``low_power=bool`` sets or clears low power mode, valid values being ``False``
+           or ``True``.
+
+        """
+        ...
+
+class WLAN:
+    """
+    Create a WLAN network interface object. Supported interfaces are
+    ``network.STA_IF`` (station aka client, connects to upstream WiFi access
+    points) and ``network.AP_IF`` (access point, allows other WiFi clients to
+    connect). Availability of the methods below depends on interface type.
+    For example, only STA interface may `WLAN.connect()` to an access point.
+    """
+
+    def __init__(self, interface_id) -> None: ...
+    def active(self, is_active: Optional[Any] = None) -> None:
+        """
+        Activate ("up") or deactivate ("down") network interface, if boolean
+        argument is passed. Otherwise, query current state if no argument is
+        provided. Most other methods require active interface.
+        """
+        ...
+    def connect(self, ssid=None, key=None, *, bssid=None) -> None:
+        """
+        Connect to the specified wireless network, using the specified key.
+        If *bssid* is given then the connection will be restricted to the
+        access-point with that MAC address (the *ssid* must also be specified
+        in this case).
+        """
+        ...
+    def disconnect(self) -> None:
+        """
+        Disconnect from the currently connected wireless network.
+        """
+        ...
+    def scan(self) -> List[Tuple]:
+        """
+        Scan for the available wireless networks.
+        Hidden networks -- where the SSID is not broadcast -- will also be scanned
+        if the WLAN interface allows it.
+
+        Scanning is only possible on STA interface. Returns list of tuples with
+        the information about WiFi access points:
+
+            (ssid, bssid, channel, RSSI, security, hidden)
+
+        *bssid* is hardware address of an access point, in binary form, returned as
+        bytes object. You can use `binascii.hexlify()` to convert it to ASCII form.
+
+        There are five values for security:
+
+            * 0 -- open
+            * 1 -- WEP
+            * 2 -- WPA-PSK
+            * 3 -- WPA2-PSK
+            * 4 -- WPA/WPA2-PSK
+
+        and two for hidden:
+
+            * 0 -- visible
+            * 1 -- hidden
+        """
+        ...
+    def status(self, param: Optional[Any] = None) -> Any:
+        """
+        Return the current status of the wireless connection.
+
+        When called with no argument the return value describes the network link status.
+        The possible statuses are defined as constants:
+
+            * ``STAT_IDLE`` -- no connection and no activity,
+            * ``STAT_CONNECTING`` -- connecting in progress,
+            * ``STAT_WRONG_PASSWORD`` -- failed due to incorrect password,
+            * ``STAT_NO_AP_FOUND`` -- failed because no access point replied,
+            * ``STAT_CONNECT_FAIL`` -- failed due to other problems,
+            * ``STAT_GOT_IP`` -- connection successful.
+
+        When called with one argument *param* should be a string naming the status
+        parameter to retrieve.  Supported parameters in WiFI STA mode are: ``'rssi'``.
+        """
+        ...
+    def isconnected(self) -> bool:
+        """
+        In case of STA mode, returns ``True`` if connected to a WiFi access
+        point and has a valid IP address.  In AP mode returns ``True`` when a
+        station is connected. Returns ``False`` otherwise.
+        """
+        ...
+    def ifconfig(self, configtuple: Optional[Any] = None) -> Tuple:
+        """
+        Get/set IP-level network interface parameters: IP address, subnet mask,
+        gateway and DNS server. When called with no arguments, this method returns
+        a 4-tuple with the above information. To set the above values, pass a
+        4-tuple with the required information.  For example::
+
+         nic.ifconfig(('192.168.0.4', '255.255.255.0', '192.168.0.1', '8.8.8.8'))
+        """
+        ...
+    def config(self, *args, **kwargs) -> Any:
+        """
+        Get or set general network interface parameters. These methods allow to work
+        with additional parameters beyond standard IP configuration (as dealt with by
+        `WLAN.ifconfig()`). These include network-specific and hardware-specific
+        parameters. For setting parameters, keyword argument syntax should be used,
+        multiple parameters can be set at once. For querying, parameters name should
+        be quoted as a string, and only one parameter can be queries at time::
+
+         # Set WiFi access point name (formally known as SSID) and WiFi channel
+         ap.config(ssid='My AP', channel=11)
+         # Query params one by one
+         print(ap.config('ssid'))
+         print(ap.config('channel'))
+
+        Following are commonly supported parameters (availability of a specific parameter
+        depends on network technology type, driver, and :term:`MicroPython port`).
+
+        =============  ===========
+        Parameter      Description
+        =============  ===========
+        mac            MAC address (bytes)
+        ssid           WiFi access point name (string)
+        channel        WiFi channel (integer)
+        hidden         Whether SSID is hidden (boolean)
+        security       Security protocol supported (enumeration, see module constants)
+        key            Access key (string)
+        hostname       The hostname that will be sent to DHCP (STA interfaces) and mDNS (if supported, both STA and AP). (Deprecated, use :func:`network.hostname` instead)
+        reconnects     Number of reconnect attempts to make (integer, 0=none, -1=unlimited)
+        txpower        Maximum transmit power in dBm (integer or float)
+        =============  ===========
+        """
+        ...
+
+def PPP(*args, **kwargs) -> Any: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/onewire.pyi` & `micropython_esp32_stubs-1.20.0.post1/onewire.pyi`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from _typeshed import Incomplete
-
-class OneWireError(Exception): ...
-
-class OneWire:
-    SEARCH_ROM: int
-    MATCH_ROM: int
-    SKIP_ROM: int
-    pin: Incomplete
-    def __init__(self, pin) -> None: ...
-    def reset(self, required: bool = ...): ...
-    def readbit(self): ...
-    def readbyte(self): ...
-    def readinto(self, buf) -> None: ...
-    def writebit(self, value): ...
-    def writebyte(self, value): ...
-    def write(self, buf) -> None: ...
-    def select_rom(self, rom) -> None: ...
-    def scan(self): ...
-    def _search_rom(self, l_rom, diff): ...
-    def crc8(self, data): ...
+from _typeshed import Incomplete
+
+class OneWireError(Exception): ...
+
+class OneWire:
+    SEARCH_ROM: int
+    MATCH_ROM: int
+    SKIP_ROM: int
+    pin: Incomplete
+    def __init__(self, pin) -> None: ...
+    def reset(self, required: bool = ...): ...
+    def readbit(self): ...
+    def readbyte(self): ...
+    def readinto(self, buf) -> None: ...
+    def writebit(self, value): ...
+    def writebyte(self, value): ...
+    def write(self, buf) -> None: ...
+    def select_rom(self, rom) -> None: ...
+    def scan(self): ...
+    def _search_rom(self, l_rom, diff): ...
+    def crc8(self, data): ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/os.pyi` & `micropython_esp32_stubs-1.20.0.post1/os.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,245 +1,245 @@
-"""
-basic "operating system" services. See: https://docs.micropython.org/en/v1.19.1/library/os.html
-
-|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
-
-The ``os`` module contains functions for filesystem access and mounting,
-terminal redirection and duplication, and the ``uname`` and ``urandom``
-functions.
-"""
-from typing import IO, Iterator, Optional, Tuple, Any
-from stdlib.os import uname_result
-
-def stat(path) -> Any:
-    """
-    Get the status of a file or directory.
-    """
-    ...
-
-def rmdir(path) -> None:
-    """
-    Remove a directory.
-    """
-    ...
-
-def rename(old_path, new_path) -> None:
-    """
-    Rename a file.
-    """
-    ...
-
-def mount(fsobj, mount_point, *, readonly) -> Any:
-    """
-    Mount the filesystem object *fsobj* at the location in the VFS given by the
-    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
-    method, or a block device.  If it's a block device then the filesystem type
-    is automatically detected (an exception is raised if no filesystem was
-    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
-    or ``'/<name>'`` to mount it at a subdirectory under the root.
-
-    If *readonly* is ``True`` then the filesystem is mounted read-only.
-
-    During the mount process the method ``mount()`` is called on the filesystem
-    object.
-
-    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
-    """
-    ...
-
-def mkdir(path) -> Any:
-    """
-    Create a new directory.
-    """
-    ...
-
-def statvfs(path) -> Tuple:
-    """
-    Get the status of a fileystem.
-
-    Returns a tuple with the filesystem information in the following order:
-
-         * ``f_bsize`` -- file system block size
-         * ``f_frsize`` -- fragment size
-         * ``f_blocks`` -- size of fs in f_frsize units
-         * ``f_bfree`` -- number of free blocks
-         * ``f_bavail`` -- number of free blocks for unprivileged users
-         * ``f_files`` -- number of inodes
-         * ``f_ffree`` -- number of free inodes
-         * ``f_favail`` -- number of free inodes for unprivileged users
-         * ``f_flag`` -- mount flags
-         * ``f_namemax`` -- maximum filename length
-
-    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
-    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
-    in a port-specific implementation.
-    """
-    ...
-
-def unlink(*args, **kwargs) -> Any: ...
-def uname() -> uname_result:
-    """
-    Return a tuple (possibly a named tuple) containing information about the
-    underlying machine and/or its operating system.  The tuple has five fields
-    in the following order, each of them being a string:
-
-         * ``sysname`` -- the name of the underlying system
-         * ``nodename`` -- the network name (can be the same as ``sysname``)
-         * ``release`` -- the version of the underlying system
-         * ``version`` -- the MicroPython version and build date
-         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
-    """
-    ...
-
-def umount(mount_point) -> Any:
-    """
-    Unmount a filesystem. *mount_point* can be a string naming the mount location,
-    or a previously-mounted filesystem object.  During the unmount process the
-    method ``umount()`` is called on the filesystem object.
-
-    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
-    """
-    ...
-
-def urandom(n) -> bytes:
-    """
-    Return a bytes object with *n* random bytes. Whenever possible, it is
-    generated by the hardware random number generator.
-    """
-    ...
-
-def chdir(path) -> Any:
-    """
-    Change current directory.
-    """
-    ...
-
-def dupterm(stream_object, index=0, /) -> IO:
-    """
-    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
-    object. The *stream_object* argument must be a native stream object, or derive
-    from ``io.IOBase`` and implement the ``readinto()`` and
-    ``write()`` methods.  The stream should be in non-blocking mode and
-    ``readinto()`` should return ``None`` if there is no data available for reading.
-
-    After calling this function all terminal output is repeated on this stream,
-    and any input that is available on the stream is passed on to the terminal input.
-
-    The *index* parameter should be a non-negative integer and specifies which
-    duplication slot is set.  A given port may implement more than one slot (slot 0
-    will always be available) and in that case terminal input and output is
-    duplicated on all the slots that are set.
-
-    If ``None`` is passed as the *stream_object* then duplication is cancelled on
-    the slot given by *index*.
-
-    The function returns the previous stream-like object in the given slot.
-    """
-    ...
-
-def remove(path) -> None:
-    """
-    Remove a file.
-    """
-    ...
-
-def listdir(dir: Optional[Any] = None) -> Any:
-    """
-    With no argument, list the current directory.  Otherwise list the given directory.
-    """
-    ...
-
-def dupterm_notify(*args, **kwargs) -> Any: ...
-def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
-    """
-    This function returns an iterator which then yields tuples corresponding to
-    the entries in the directory that it is listing.  With no argument it lists the
-    current directory, otherwise it lists the directory given by *dir*.
-
-    The tuples have the form *(name, type, inode[, size])*:
-
-     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
-       the entry;
-     - *type* is an integer that specifies the type of the entry, with 0x4000 for
-       directories and 0x8000 for regular files;
-     - *inode* is an integer corresponding to the inode of the file, and may be 0
-       for filesystems that don't have such a notion.
-     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
-       file entries, *size* is an integer representing the size of the file
-       or -1 if unknown.  Its meaning is currently undefined for directory
-       entries.
-    """
-    ...
-
-def getcwd() -> Any:
-    """
-    Get the current directory.
-    """
-    ...
-
-class VfsLfs2:
-    """
-    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
-    Storage of the littlefs filesystem is provided by *block_dev*, which must
-    support the :ref:`extended interface <block-device-interface>`.
-    Objects created by this constructor can be mounted using :func:`mount`.
-
-    The *mtime* argument enables modification timestamps for files, stored using
-    littlefs attributes.  This option can be disabled or enabled differently each
-    mount time and timestamps will only be added or updated if *mtime* is enabled,
-    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
-    timestamps will work without reformatting and timestamps will be added
-    transparently to existing files once they are opened for writing.  When *mtime*
-    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
-
-    See :ref:`filesystem` for more information.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
-        """
-            Build a Lfs2 filesystem on *block_dev*.
-
-        ``Note:`` There are reports of littlefs v2 failing in certain situations,
-                  for details see `littlefs issue 295`_.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
-
-class VfsFat:
-    """
-    Create a filesystem object that uses the FAT filesystem format.  Storage of
-    the FAT filesystem is provided by *block_dev*.
-    Objects created by this constructor can be mounted using :func:`mount`.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev) -> None:
-        """
-        Build a FAT filesystem on *block_dev*.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev) -> None: ...
+"""
+basic "operating system" services. See: https://docs.micropython.org/en/v1.20.0/library/os.html
+
+|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
+
+The ``os`` module contains functions for filesystem access and mounting,
+terminal redirection and duplication, and the ``uname`` and ``urandom``
+functions.
+"""
+from typing import IO, Iterator, Optional, Tuple, Any
+from stdlib.os import uname_result
+
+def stat(path) -> Any:
+    """
+    Get the status of a file or directory.
+    """
+    ...
+
+def rmdir(path) -> None:
+    """
+    Remove a directory.
+    """
+    ...
+
+def rename(old_path, new_path) -> None:
+    """
+    Rename a file.
+    """
+    ...
+
+def mount(fsobj, mount_point, *, readonly) -> Any:
+    """
+    Mount the filesystem object *fsobj* at the location in the VFS given by the
+    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
+    method, or a block device.  If it's a block device then the filesystem type
+    is automatically detected (an exception is raised if no filesystem was
+    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
+    or ``'/<name>'`` to mount it at a subdirectory under the root.
+
+    If *readonly* is ``True`` then the filesystem is mounted read-only.
+
+    During the mount process the method ``mount()`` is called on the filesystem
+    object.
+
+    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
+    """
+    ...
+
+def mkdir(path) -> Any:
+    """
+    Create a new directory.
+    """
+    ...
+
+def statvfs(path) -> Tuple:
+    """
+    Get the status of a fileystem.
+
+    Returns a tuple with the filesystem information in the following order:
+
+         * ``f_bsize`` -- file system block size
+         * ``f_frsize`` -- fragment size
+         * ``f_blocks`` -- size of fs in f_frsize units
+         * ``f_bfree`` -- number of free blocks
+         * ``f_bavail`` -- number of free blocks for unprivileged users
+         * ``f_files`` -- number of inodes
+         * ``f_ffree`` -- number of free inodes
+         * ``f_favail`` -- number of free inodes for unprivileged users
+         * ``f_flag`` -- mount flags
+         * ``f_namemax`` -- maximum filename length
+
+    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
+    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
+    in a port-specific implementation.
+    """
+    ...
+
+def unlink(*args, **kwargs) -> Any: ...
+def uname() -> uname_result:
+    """
+    Return a tuple (possibly a named tuple) containing information about the
+    underlying machine and/or its operating system.  The tuple has five fields
+    in the following order, each of them being a string:
+
+         * ``sysname`` -- the name of the underlying system
+         * ``nodename`` -- the network name (can be the same as ``sysname``)
+         * ``release`` -- the version of the underlying system
+         * ``version`` -- the MicroPython version and build date
+         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
+    """
+    ...
+
+def umount(mount_point) -> Any:
+    """
+    Unmount a filesystem. *mount_point* can be a string naming the mount location,
+    or a previously-mounted filesystem object.  During the unmount process the
+    method ``umount()`` is called on the filesystem object.
+
+    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
+    """
+    ...
+
+def urandom(n) -> bytes:
+    """
+    Return a bytes object with *n* random bytes. Whenever possible, it is
+    generated by the hardware random number generator.
+    """
+    ...
+
+def chdir(path) -> Any:
+    """
+    Change current directory.
+    """
+    ...
+
+def dupterm(stream_object, index=0, /) -> IO:
+    """
+    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
+    object. The *stream_object* argument must be a native stream object, or derive
+    from ``io.IOBase`` and implement the ``readinto()`` and
+    ``write()`` methods.  The stream should be in non-blocking mode and
+    ``readinto()`` should return ``None`` if there is no data available for reading.
+
+    After calling this function all terminal output is repeated on this stream,
+    and any input that is available on the stream is passed on to the terminal input.
+
+    The *index* parameter should be a non-negative integer and specifies which
+    duplication slot is set.  A given port may implement more than one slot (slot 0
+    will always be available) and in that case terminal input and output is
+    duplicated on all the slots that are set.
+
+    If ``None`` is passed as the *stream_object* then duplication is cancelled on
+    the slot given by *index*.
+
+    The function returns the previous stream-like object in the given slot.
+    """
+    ...
+
+def remove(path) -> None:
+    """
+    Remove a file.
+    """
+    ...
+
+def listdir(dir: Optional[Any] = None) -> Any:
+    """
+    With no argument, list the current directory.  Otherwise list the given directory.
+    """
+    ...
+
+def dupterm_notify(*args, **kwargs) -> Any: ...
+def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
+    """
+    This function returns an iterator which then yields tuples corresponding to
+    the entries in the directory that it is listing.  With no argument it lists the
+    current directory, otherwise it lists the directory given by *dir*.
+
+    The tuples have the form *(name, type, inode[, size])*:
+
+     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
+       the entry;
+     - *type* is an integer that specifies the type of the entry, with 0x4000 for
+       directories and 0x8000 for regular files;
+     - *inode* is an integer corresponding to the inode of the file, and may be 0
+       for filesystems that don't have such a notion.
+     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
+       file entries, *size* is an integer representing the size of the file
+       or -1 if unknown.  Its meaning is currently undefined for directory
+       entries.
+    """
+    ...
+
+def getcwd() -> Any:
+    """
+    Get the current directory.
+    """
+    ...
+
+class VfsLfs2:
+    """
+    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
+    Storage of the littlefs filesystem is provided by *block_dev*, which must
+    support the :ref:`extended interface <block-device-interface>`.
+    Objects created by this constructor can be mounted using :func:`mount`.
+
+    The *mtime* argument enables modification timestamps for files, stored using
+    littlefs attributes.  This option can be disabled or enabled differently each
+    mount time and timestamps will only be added or updated if *mtime* is enabled,
+    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
+    timestamps will work without reformatting and timestamps will be added
+    transparently to existing files once they are opened for writing.  When *mtime*
+    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
+
+    See :ref:`filesystem` for more information.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
+        """
+            Build a Lfs2 filesystem on *block_dev*.
+
+        ``Note:`` There are reports of littlefs v2 failing in certain situations,
+                  for details see `littlefs issue 295`_.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
+
+class VfsFat:
+    """
+    Create a filesystem object that uses the FAT filesystem format.  Storage of
+    the FAT filesystem is provided by *block_dev*.
+    Objects created by this constructor can be mounted using :func:`mount`.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev) -> None:
+        """
+        Build a FAT filesystem on *block_dev*.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/pyproject.toml` & `micropython_esp32_stubs-1.20.0.post1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-esp32-stubs"
-version = "1.19.1.post9"
+version = "1.20.0.post1"
 description = "MicroPython stubs"
 authors = [
     "josverl <josverl@users.noreply.github.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/josverl/micropython-stubs#micropython-stubs"
@@ -35,32 +35,38 @@
     { include = "_boot.pyi" },
     { include = "_onewire.pyi" },
     { include = "_thread.pyi" },
     { include = "_uasyncio.pyi" },
     { include = "apa106.pyi" },
     { include = "array.pyi" },
     { include = "binascii.pyi" },
+    { include = "bluetooth.pyi" },
     { include = "btree.pyi" },
     { include = "cmath.pyi" },
+    { include = "collections.pyi" },
+    { include = "cryptolib.pyi" },
     { include = "dht.pyi" },
     { include = "ds18x20.pyi" },
     { include = "errno.pyi" },
     { include = "esp.pyi" },
     { include = "esp32.pyi" },
     { include = "flashbdev.pyi" },
     { include = "framebuf.pyi" },
     { include = "gc.pyi" },
     { include = "hashlib.pyi" },
     { include = "heapq.pyi" },
     { include = "inisetup.pyi" },
     { include = "io.pyi" },
     { include = "json.pyi" },
+    { include = "logging.pyi" },
     { include = "machine.pyi" },
     { include = "math.pyi" },
     { include = "micropython.pyi" },
+    { include = "mip/__init__.pyi" },
+    { include = "mip.pyi" },
     { include = "neopixel.pyi" },
     { include = "network.pyi" },
     { include = "ntptime.pyi" },
     { include = "onewire.pyi" },
     { include = "os.pyi" },
     { include = "platform.pyi" },
     { include = "random.pyi" },
@@ -89,17 +95,16 @@
     { include = "uio.pyi" },
     { include = "ujson.pyi" },
     { include = "umachine.pyi" },
     { include = "umqtt/__init__.pyi" },
     { include = "umqtt/robust.pyi" },
     { include = "umqtt/simple.pyi" },
     { include = "uos.pyi" },
-    { include = "upip.pyi" },
-    { include = "upip_utarfile.pyi" },
     { include = "uplatform.pyi" },
+    { include = "upysh.pyi" },
     { include = "urandom.pyi" },
     { include = "ure.pyi" },
     { include = "urequests.pyi" },
     { include = "uselect.pyi" },
     { include = "usocket.pyi" },
     { include = "ussl.pyi" },
     { include = "ustruct.pyi" },
@@ -107,15 +112,14 @@
     { include = "utime.pyi" },
     { include = "utimeq.pyi" },
     { include = "uwebsocket.pyi" },
     { include = "uzlib.pyi" },
     { include = "webrepl.pyi" },
     { include = "webrepl_setup.pyi" },
     { include = "websocket.pyi" },
-    { include = "websocket_helper.pyi" },
     { include = "zlib.pyi" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 micropython-stdlib-stubs = ">=0.9.0"
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/select.pyi` & `micropython_esp32_stubs-1.20.0.post1/select.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-"""
-wait for events on a set of streams. See: https://docs.micropython.org/en/v1.19.1/library/select.html
-
-|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
-
-This module provides functions to efficiently wait for events on multiple
-`streams <stream>` (select streams which are ready for operations).
-"""
-from typing import Iterator, List, Optional, Tuple, Any
-
-POLLOUT: int
-POLLIN: int
-POLLHUP: int
-POLLERR: int
-
-class select:
-    """
-    Wait for activity on a set of objects.
-
-    This function is provided by some MicroPython ports for compatibility
-    and is not efficient. Usage of :class:`Poll` is recommended instead.
-    """
-
-    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
-
-class poll:
-    """
-    Create an instance of the Poll class.
-    """
-
-    def __init__(self) -> None: ...
-    def register(self, obj, eventmask: Optional[Any] = None) -> None:
-        """
-        Register `stream` *obj* for polling. *eventmask* is logical OR of:
-
-        * ``select.POLLIN``  - data available for reading
-        * ``select.POLLOUT`` - more data can be written
-
-        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
-        *not* valid as input eventmask (these are unsolicited events which
-        will be returned from `poll()` regardless of whether they are asked
-        for). This semantics is per POSIX.
-
-        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
-
-        It is OK to call this function multiple times for the same *obj*.
-        Successive calls will update *obj*'s eventmask to the value of
-        *eventmask* (i.e. will behave as `modify()`).
-        """
-        ...
-    def unregister(self, obj) -> Any:
-        """
-        Unregister *obj* from polling.
-        """
-        ...
-    def modify(self, obj, eventmask) -> None:
-        """
-        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
-        is raised with error of ENOENT.
-        """
-        ...
-    def poll(self, timeout=-1, /) -> List:
-        """
-        Wait for at least one of the registered objects to become ready or have an
-        exceptional condition, with optional timeout in milliseconds (if *timeout*
-        arg is not specified or -1, there is no timeout).
-
-        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
-        tuple, depending on a platform and version, so don't assume that its size is 2.
-        The ``event`` element specifies which events happened with a stream and
-        is a combination of ``select.POLL*`` constants described above. Note that
-        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
-        (even if were not asked for), and must be acted on accordingly (the
-        corresponding stream unregistered from poll and likely closed), because
-        otherwise all further invocations of `poll()` may return immediately with
-        these flags set for this stream again.
-
-        In case of timeout, an empty list is returned.
-        """
-        ...
-    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
-        """
-        Like :meth:`poll.poll`, but instead returns an iterator which yields a
-        `callee-owned tuple`. This function provides an efficient, allocation-free
-        way to poll on streams.
-
-        If *flags* is 1, one-shot behaviour for events is employed: streams for
-        which events happened will have their event masks automatically reset
-        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
-        won't be processed until new mask is set with `poll.modify()`. This
-        behaviour is useful for asynchronous I/O schedulers.
-        """
-        ...
+"""
+wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20.0/library/select.html
+
+|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
+
+This module provides functions to efficiently wait for events on multiple
+`streams <stream>` (select streams which are ready for operations).
+"""
+from typing import Iterator, List, Optional, Tuple, Any
+
+POLLOUT: int
+POLLIN: int
+POLLHUP: int
+POLLERR: int
+
+class select:
+    """
+    Wait for activity on a set of objects.
+
+    This function is provided by some MicroPython ports for compatibility
+    and is not efficient. Usage of :class:`Poll` is recommended instead.
+    """
+
+    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
+
+class poll:
+    """
+    Create an instance of the Poll class.
+    """
+
+    def __init__(self) -> None: ...
+    def register(self, obj, eventmask: Optional[Any] = None) -> None:
+        """
+        Register `stream` *obj* for polling. *eventmask* is logical OR of:
+
+        * ``select.POLLIN``  - data available for reading
+        * ``select.POLLOUT`` - more data can be written
+
+        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
+        *not* valid as input eventmask (these are unsolicited events which
+        will be returned from `poll()` regardless of whether they are asked
+        for). This semantics is per POSIX.
+
+        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
+
+        It is OK to call this function multiple times for the same *obj*.
+        Successive calls will update *obj*'s eventmask to the value of
+        *eventmask* (i.e. will behave as `modify()`).
+        """
+        ...
+    def unregister(self, obj) -> Any:
+        """
+        Unregister *obj* from polling.
+        """
+        ...
+    def modify(self, obj, eventmask) -> None:
+        """
+        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
+        is raised with error of ENOENT.
+        """
+        ...
+    def poll(self, timeout=-1, /) -> List:
+        """
+        Wait for at least one of the registered objects to become ready or have an
+        exceptional condition, with optional timeout in milliseconds (if *timeout*
+        arg is not specified or -1, there is no timeout).
+
+        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
+        tuple, depending on a platform and version, so don't assume that its size is 2.
+        The ``event`` element specifies which events happened with a stream and
+        is a combination of ``select.POLL*`` constants described above. Note that
+        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
+        (even if were not asked for), and must be acted on accordingly (the
+        corresponding stream unregistered from poll and likely closed), because
+        otherwise all further invocations of `poll()` may return immediately with
+        these flags set for this stream again.
+
+        In case of timeout, an empty list is returned.
+        """
+        ...
+    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
+        """
+        Like :meth:`poll.poll`, but instead returns an iterator which yields a
+        `callee-owned tuple`. This function provides an efficient, allocation-free
+        way to poll on streams.
+
+        If *flags* is 1, one-shot behaviour for events is employed: streams for
+        which events happened will have their event masks automatically reset
+        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
+        won't be processed until new mask is set with `poll.modify()`. This
+        behaviour is useful for asynchronous I/O schedulers.
+        """
+        ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/socket.pyi` & `micropython_esp32_stubs-1.20.0.post1/socket.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-"""
-socket module. See: https://docs.micropython.org/en/v1.19.1/library/socket.html
-
-|see_cpython_module| :mod:`python:socket` https://docs.python.org/3/library/socket.html .
-
-This module provides access to the BSD socket interface.
-"""
-from typing import IO, Optional, Tuple, Any
-
-SOCK_RAW: int
-SOCK_DGRAM: int
-IP_ADD_MEMBERSHIP: int
-SOCK_STREAM: int
-SOL_SOCKET: int
-SO_REUSEADDR: int
-AF_INET6: int
-AF_INET: int
-IPPROTO_UDP: int
-IPPROTO_IP: int
-IPPROTO_TCP: int
-
-def getaddrinfo(host, port, af=0, type=0, proto=0, flags=0, /) -> Any:
-    """
-    Translate the host/port argument into a sequence of 5-tuples that contain all the
-    necessary arguments for creating a socket connected to that service. Arguments
-    *af*, *type*, and *proto* (which have the same meaning as for the `socket()` function)
-    can be used to filter which kind of addresses are returned. If a parameter is not
-    specified or zero, all combinations of addresses can be returned (requiring
-    filtering on the user side).
-
-    The resulting list of 5-tuples has the following structure::
-
-       (family, type, proto, canonname, sockaddr)
-
-    The following example shows how to connect to a given url::
-
-       s = socket.socket()
-       # This assumes that if "type" is not specified, an address for
-       # SOCK_STREAM will be returned, which may be not true
-       s.connect(socket.getaddrinfo('www.micropython.org', 80)[0][-1])
-
-    Recommended use of filtering params::
-
-       s = socket.socket()
-       # Guaranteed to return an address which can be connect'ed to for
-       # stream operation.
-       s.connect(socket.getaddrinfo('www.micropython.org', 80, 0, SOCK_STREAM)[0][-1])
-    """
-    ...
-
-class socket:
-    """
-    Create a new socket using the given address family, socket type and
-    protocol number. Note that specifying *proto* in most cases is not
-    required (and not recommended, as some MicroPython ports may omit
-    ``IPPROTO_*`` constants). Instead, *type* argument will select needed
-    protocol automatically::
-
-         # Create STREAM TCP socket
-         socket(AF_INET, SOCK_STREAM)
-         # Create DGRAM UDP socket
-         socket(AF_INET, SOCK_DGRAM)
-    """
-
-    def recvfrom(self, bufsize) -> Tuple:
-        """
-        Receive data from the socket. The return value is a pair *(bytes, address)* where *bytes* is a
-        bytes object representing the data received and *address* is the address of the socket sending
-        the data.
-        """
-        ...
-    def recv(self, bufsize) -> bytes:
-        """
-        Receive data from the socket. The return value is a bytes object representing the data
-        received. The maximum amount of data to be received at once is specified by bufsize.
-        """
-        ...
-    def makefile(self, mode="rb", buffering=0, /) -> IO:
-        """
-        Return a file object associated with the socket. The exact returned type depends on the arguments
-        given to makefile(). The support is limited to binary modes only ('rb', 'wb', and 'rwb').
-        CPython's arguments: *encoding*, *errors* and *newline* are not supported.
-        """
-        ...
-    def listen(self, backlog: Optional[Any] = None) -> None:
-        """
-        Enable a server to accept connections. If *backlog* is specified, it must be at least 0
-        (if it's lower, it will be set to 0); and specifies the number of unaccepted connections
-        that the system will allow before refusing new connections. If not specified, a default
-        reasonable value is chosen.
-        """
-        ...
-    def fileno(self, *args, **kwargs) -> Any: ...
-    def sendall(self, bytes) -> int:
-        """
-        Send all data to the socket. The socket must be connected to a remote socket.
-        Unlike `send()`, this method will try to send all of data, by sending data
-        chunk by chunk consecutively.
-
-        The behaviour of this method on non-blocking sockets is undefined. Due to this,
-        on MicroPython, it's recommended to use `write()` method instead, which
-        has the same "no short writes" policy for blocking sockets, and will return
-        number of bytes sent on non-blocking sockets.
-        """
-        ...
-    def setsockopt(self, level, optname, value) -> None:
-        """
-        Set the value of the given socket option. The needed symbolic constants are defined in the
-        socket module (SO_* etc.). The *value* can be an integer or a bytes-like object representing
-        a buffer.
-        """
-        ...
-    def setblocking(self, flag) -> Any:
-        """
-        Set blocking or non-blocking mode of the socket: if flag is false, the socket is set to non-blocking,
-        else to blocking mode.
-
-        This method is a shorthand for certain `settimeout()` calls:
-
-        * ``sock.setblocking(True)`` is equivalent to ``sock.settimeout(None)``
-        * ``sock.setblocking(False)`` is equivalent to ``sock.settimeout(0)``
-        """
-        ...
-    def sendto(self, bytes, address) -> None:
-        """
-        Send data to the socket. The socket should not be connected to a remote socket, since the
-        destination socket is specified by *address*.
-        """
-        ...
-    def settimeout(self, value) -> Any:
-        """
-        **Note**: Not every port supports this method, see below.
-
-        Set a timeout on blocking socket operations. The value argument can be a nonnegative floating
-        point number expressing seconds, or None. If a non-zero value is given, subsequent socket operations
-        will raise an `OSError` exception if the timeout period value has elapsed before the operation has
-        completed. If zero is given, the socket is put in non-blocking mode. If None is given, the socket
-        is put in blocking mode.
-
-        Not every :term:`MicroPython port` supports this method. A more portable and
-        generic solution is to use `select.poll` object. This allows to wait on
-        multiple objects at the same time (and not just on sockets, but on generic
-        `stream` objects which support polling). Example::
-
-             # Instead of:
-             s.settimeout(1.0)  # time in seconds
-             s.read(10)  # may timeout
-
-             # Use:
-             poller = select.poll()
-             poller.register(s, select.POLLIN)
-             res = poller.poll(1000)  # time in milliseconds
-             if not res:
-                 # s is still not ready for input, i.e. operation timed out
-        """
-        ...
-    def readline(self) -> Any:
-        """
-        Read a line, ending in a newline character.
-
-        Return value: the line read.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the *buf*.  If *nbytes* is specified then read at most
-        that many bytes.  Otherwise, read at most *len(buf)* bytes. Just as
-        `read()`, this method follows "no short reads" policy.
-
-        Return value: number of bytes read and stored into *buf*.
-        """
-        ...
-    def read(self, size: Optional[Any] = None) -> bytes:
-        """
-        Read up to size bytes from the socket. Return a bytes object. If *size* is not given, it
-        reads all data available from the socket until EOF; as such the method will not return until
-        the socket is closed. This function tries to read as much data as
-        requested (no "short reads"). This may be not possible with
-        non-blocking socket though, and then less data will be returned.
-        """
-        ...
-    def close(self) -> Any:
-        """
-        Mark the socket closed and release all resources. Once that happens, all future operations
-        on the socket object will fail. The remote end will receive EOF indication if
-        supported by protocol.
-
-        Sockets are automatically closed when they are garbage-collected, but it is recommended
-        to `close()` them explicitly as soon you finished working with them.
-        """
-        ...
-    def connect(self, address) -> None:
-        """
-        Connect to a remote socket at *address*.
-        """
-        ...
-    def send(self, bytes) -> int:
-        """
-        Send data to the socket. The socket must be connected to a remote socket.
-        Returns number of bytes sent, which may be smaller than the length of data
-        ("short write").
-        """
-        ...
-    def bind(self, address) -> Any:
-        """
-        Bind the socket to *address*. The socket must not already be bound.
-        """
-        ...
-    def accept(self) -> Tuple:
-        """
-        Accept a connection. The socket must be bound to an address and listening for connections.
-        The return value is a pair (conn, address) where conn is a new socket object usable to send
-        and receive data on the connection, and address is the address bound to the socket on the
-        other end of the connection.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the socket. This function will try to
-        write all data to a socket (no "short writes"). This may be not possible
-        with a non-blocking socket though, and returned value will be less than
-        the length of *buf*.
-
-        Return value: number of bytes written.
-        """
-        ...
-    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None: ...
+"""
+socket module. See: https://docs.micropython.org/en/v1.20.0/library/socket.html
+
+|see_cpython_module| :mod:`python:socket` https://docs.python.org/3/library/socket.html .
+
+This module provides access to the BSD socket interface.
+"""
+from typing import IO, Optional, Tuple, Any
+
+SOCK_RAW: int
+SOCK_DGRAM: int
+IP_ADD_MEMBERSHIP: int
+SOCK_STREAM: int
+SOL_SOCKET: int
+SO_REUSEADDR: int
+AF_INET6: int
+AF_INET: int
+IPPROTO_UDP: int
+IPPROTO_IP: int
+IPPROTO_TCP: int
+
+def getaddrinfo(host, port, af=0, type=0, proto=0, flags=0, /) -> Any:
+    """
+    Translate the host/port argument into a sequence of 5-tuples that contain all the
+    necessary arguments for creating a socket connected to that service. Arguments
+    *af*, *type*, and *proto* (which have the same meaning as for the `socket()` function)
+    can be used to filter which kind of addresses are returned. If a parameter is not
+    specified or zero, all combinations of addresses can be returned (requiring
+    filtering on the user side).
+
+    The resulting list of 5-tuples has the following structure::
+
+       (family, type, proto, canonname, sockaddr)
+
+    The following example shows how to connect to a given url::
+
+       s = socket.socket()
+       # This assumes that if "type" is not specified, an address for
+       # SOCK_STREAM will be returned, which may be not true
+       s.connect(socket.getaddrinfo('www.micropython.org', 80)[0][-1])
+
+    Recommended use of filtering params::
+
+       s = socket.socket()
+       # Guaranteed to return an address which can be connect'ed to for
+       # stream operation.
+       s.connect(socket.getaddrinfo('www.micropython.org', 80, 0, SOCK_STREAM)[0][-1])
+    """
+    ...
+
+class socket:
+    """
+    Create a new socket using the given address family, socket type and
+    protocol number. Note that specifying *proto* in most cases is not
+    required (and not recommended, as some MicroPython ports may omit
+    ``IPPROTO_*`` constants). Instead, *type* argument will select needed
+    protocol automatically::
+
+         # Create STREAM TCP socket
+         socket(AF_INET, SOCK_STREAM)
+         # Create DGRAM UDP socket
+         socket(AF_INET, SOCK_DGRAM)
+    """
+
+    def recvfrom(self, bufsize) -> Tuple:
+        """
+        Receive data from the socket. The return value is a pair *(bytes, address)* where *bytes* is a
+        bytes object representing the data received and *address* is the address of the socket sending
+        the data.
+        """
+        ...
+    def recv(self, bufsize) -> bytes:
+        """
+        Receive data from the socket. The return value is a bytes object representing the data
+        received. The maximum amount of data to be received at once is specified by bufsize.
+        """
+        ...
+    def makefile(self, mode="rb", buffering=0, /) -> IO:
+        """
+        Return a file object associated with the socket. The exact returned type depends on the arguments
+        given to makefile(). The support is limited to binary modes only ('rb', 'wb', and 'rwb').
+        CPython's arguments: *encoding*, *errors* and *newline* are not supported.
+        """
+        ...
+    def listen(self, backlog: Optional[Any] = None) -> None:
+        """
+        Enable a server to accept connections. If *backlog* is specified, it must be at least 0
+        (if it's lower, it will be set to 0); and specifies the number of unaccepted connections
+        that the system will allow before refusing new connections. If not specified, a default
+        reasonable value is chosen.
+        """
+        ...
+    def fileno(self, *args, **kwargs) -> Any: ...
+    def sendall(self, bytes) -> int:
+        """
+        Send all data to the socket. The socket must be connected to a remote socket.
+        Unlike `send()`, this method will try to send all of data, by sending data
+        chunk by chunk consecutively.
+
+        The behaviour of this method on non-blocking sockets is undefined. Due to this,
+        on MicroPython, it's recommended to use `write()` method instead, which
+        has the same "no short writes" policy for blocking sockets, and will return
+        number of bytes sent on non-blocking sockets.
+        """
+        ...
+    def setsockopt(self, level, optname, value) -> None:
+        """
+        Set the value of the given socket option. The needed symbolic constants are defined in the
+        socket module (SO_* etc.). The *value* can be an integer or a bytes-like object representing
+        a buffer.
+        """
+        ...
+    def setblocking(self, flag) -> Any:
+        """
+        Set blocking or non-blocking mode of the socket: if flag is false, the socket is set to non-blocking,
+        else to blocking mode.
+
+        This method is a shorthand for certain `settimeout()` calls:
+
+        * ``sock.setblocking(True)`` is equivalent to ``sock.settimeout(None)``
+        * ``sock.setblocking(False)`` is equivalent to ``sock.settimeout(0)``
+        """
+        ...
+    def sendto(self, bytes, address) -> None:
+        """
+        Send data to the socket. The socket should not be connected to a remote socket, since the
+        destination socket is specified by *address*.
+        """
+        ...
+    def settimeout(self, value) -> Any:
+        """
+        **Note**: Not every port supports this method, see below.
+
+        Set a timeout on blocking socket operations. The value argument can be a nonnegative floating
+        point number expressing seconds, or None. If a non-zero value is given, subsequent socket operations
+        will raise an `OSError` exception if the timeout period value has elapsed before the operation has
+        completed. If zero is given, the socket is put in non-blocking mode. If None is given, the socket
+        is put in blocking mode.
+
+        Not every :term:`MicroPython port` supports this method. A more portable and
+        generic solution is to use `select.poll` object. This allows to wait on
+        multiple objects at the same time (and not just on sockets, but on generic
+        `stream` objects which support polling). Example::
+
+             # Instead of:
+             s.settimeout(1.0)  # time in seconds
+             s.read(10)  # may timeout
+
+             # Use:
+             poller = select.poll()
+             poller.register(s, select.POLLIN)
+             res = poller.poll(1000)  # time in milliseconds
+             if not res:
+                 # s is still not ready for input, i.e. operation timed out
+        """
+        ...
+    def readline(self) -> Any:
+        """
+        Read a line, ending in a newline character.
+
+        Return value: the line read.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the *buf*.  If *nbytes* is specified then read at most
+        that many bytes.  Otherwise, read at most *len(buf)* bytes. Just as
+        `read()`, this method follows "no short reads" policy.
+
+        Return value: number of bytes read and stored into *buf*.
+        """
+        ...
+    def read(self, size: Optional[Any] = None) -> bytes:
+        """
+        Read up to size bytes from the socket. Return a bytes object. If *size* is not given, it
+        reads all data available from the socket until EOF; as such the method will not return until
+        the socket is closed. This function tries to read as much data as
+        requested (no "short reads"). This may be not possible with
+        non-blocking socket though, and then less data will be returned.
+        """
+        ...
+    def close(self) -> Any:
+        """
+        Mark the socket closed and release all resources. Once that happens, all future operations
+        on the socket object will fail. The remote end will receive EOF indication if
+        supported by protocol.
+
+        Sockets are automatically closed when they are garbage-collected, but it is recommended
+        to `close()` them explicitly as soon you finished working with them.
+        """
+        ...
+    def connect(self, address) -> None:
+        """
+        Connect to a remote socket at *address*.
+        """
+        ...
+    def send(self, bytes) -> int:
+        """
+        Send data to the socket. The socket must be connected to a remote socket.
+        Returns number of bytes sent, which may be smaller than the length of data
+        ("short write").
+        """
+        ...
+    def bind(self, address) -> Any:
+        """
+        Bind the socket to *address*. The socket must not already be bound.
+        """
+        ...
+    def accept(self) -> Tuple:
+        """
+        Accept a connection. The socket must be bound to an address and listening for connections.
+        The return value is a pair (conn, address) where conn is a new socket object usable to send
+        and receive data on the connection, and address is the address bound to the socket on the
+        other end of the connection.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the socket. This function will try to
+        write all data to a socket (no "short writes"). This may be not possible
+        with a non-blocking socket though, and returned value will be less than
+        the length of *buf*.
+
+        Return value: number of bytes written.
+        """
+        ...
+    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/ssl.pyi` & `micropython_esp32_stubs-1.20.0.post1/ssl.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,50 @@
-"""
-TLS/SSL wrapper for socket objects. See: https://docs.micropython.org/en/v1.19.1/library/ssl.html
-
-|see_cpython_module| :mod:`python:ssl` https://docs.python.org/3/library/ssl.html .
-
-This module provides access to Transport Layer Security (previously and
-widely known as “Secure Sockets Layer”) encryption and peer authentication
-facilities for network sockets, both client-side and server-side.
-"""
-from typing import Any
-
-def wrap_socket(sock, server_side=False, keyfile=None, certfile=None, cert_reqs=None, ca_certs=None, do_handshake=True) -> Any:
-    """
-    Takes a `stream` *sock* (usually socket.socket instance of ``SOCK_STREAM`` type),
-    and returns an instance of ssl.SSLSocket, which wraps the underlying stream in
-    an SSL context. Returned object has the usual `stream` interface methods like
-    ``read()``, ``write()``, etc.
-    A server-side SSL socket should be created from a normal socket returned from
-    :meth:`~socket.socket.accept()` on a non-SSL listening server socket.
-
-    - *do_handshake* determines whether the handshake is done as part of the ``wrap_socket``
-      or whether it is deferred to be done as part of the initial reads or writes
-      (there is no ``do_handshake`` method as in CPython).
-      For blocking sockets doing the handshake immediately is standard. For non-blocking
-      sockets (i.e. when the *sock* passed into ``wrap_socket`` is in non-blocking mode)
-      the handshake should generally be deferred because otherwise ``wrap_socket`` blocks
-      until it completes. Note that in AXTLS the handshake can be deferred until the first
-      read or write but it then blocks until completion.
-
-    Depending on the underlying module implementation in a particular
-    :term:`MicroPython port`, some or all keyword arguments above may be not supported.
-    """
-    ...
+"""
+TLS/SSL wrapper for socket objects. See: https://docs.micropython.org/en/v1.20.0/library/ssl.html
+
+|see_cpython_module| :mod:`python:ssl` https://docs.python.org/3/library/ssl.html .
+
+This module provides access to Transport Layer Security (previously and
+widely known as “Secure Sockets Layer”) encryption and peer authentication
+facilities for network sockets, both client-side and server-side.
+"""
+from typing import Any
+
+CERT_OPTIONAL: int
+CERT_REQUIRED: int
+CERT_NONE: int
+
+def wrap_socket(
+    sock, server_side=False, keyfile=None, certfile=None, cert_reqs=None, cadata=None, server_hostname=None, do_handshake=True
+) -> Any:
+    """
+    Takes a `stream` *sock* (usually socket.socket instance of ``SOCK_STREAM`` type),
+    and returns an instance of ssl.SSLSocket, which wraps the underlying stream in
+    an SSL context. Returned object has the usual `stream` interface methods like
+    ``read()``, ``write()``, etc.
+    A server-side SSL socket should be created from a normal socket returned from
+    :meth:`~socket.socket.accept()` on a non-SSL listening server socket.
+
+    - *do_handshake* determines whether the handshake is done as part of the ``wrap_socket``
+      or whether it is deferred to be done as part of the initial reads or writes
+      (there is no ``do_handshake`` method as in CPython).
+      For blocking sockets doing the handshake immediately is standard. For non-blocking
+      sockets (i.e. when the *sock* passed into ``wrap_socket`` is in non-blocking mode)
+      the handshake should generally be deferred because otherwise ``wrap_socket`` blocks
+      until it completes. Note that in AXTLS the handshake can be deferred until the first
+      read or write but it then blocks until completion.
+
+    - *cert_reqs* determines whether the peer (server or client) must present a valid certificate.
+      Note that for mbedtls based ports, ``ssl.CERT_NONE`` and ``ssl.CERT_OPTIONAL`` will not
+      validate any certificate, only ``ssl.CERT_REQUIRED`` will.
+
+    - *cadata* is a bytes object containing the CA certificate chain (in DER format) that will
+      validate the peer's certificate.  Currently only a single DER-encoded certificate is supported.
+
+    - *server_hostname* is for use as a client, and sets the hostname to check against the received
+      server certificate.  It also sets the name for Server Name Indication (SNI), allowing the server
+      to present the proper certificate.
+
+    Depending on the underlying module implementation in a particular
+    :term:`MicroPython port`, some or all keyword arguments above may be not supported.
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/sys.pyi` & `micropython_esp32_stubs-1.20.0.post1/sys.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-system specific functions. See: https://docs.micropython.org/en/v1.19.1/library/sys.html
-
-|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
-"""
-from typing import Dict, List, Tuple, Any
-
-platform: str
-version_info: tuple
-path: list
-version: str
-ps1: str
-ps2: str
-byteorder: str
-modules: dict
-argv: list
-implementation: tuple
-maxsize: int
-
-def print_exception(exc, file=stdout, /) -> None:
-    """
-    Print exception with a traceback to a file-like object *file* (or
-    `sys.stdout` by default).
-    """
-    ...
-
-def exit(retval=0, /) -> Any:
-    """
-    Terminate current program with a given exit code. Underlyingly, this
-    function raise as `SystemExit` exception. If an argument is given, its
-    value given as an argument to `SystemExit`.
-    """
-    ...
-
-stderr: Any
-stdout: Any
-stdin: Any
+"""
+system specific functions. See: https://docs.micropython.org/en/v1.20.0/library/sys.html
+
+|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
+"""
+from typing import Dict, List, Tuple, Any
+
+platform: str
+version_info: tuple
+path: list
+version: str
+ps1: str
+ps2: str
+byteorder: str
+modules: dict
+argv: list
+implementation: tuple
+maxsize: int
+
+def print_exception(exc, file=stdout, /) -> None:
+    """
+    Print exception with a traceback to a file-like object *file* (or
+    `sys.stdout` by default).
+    """
+    ...
+
+def exit(retval=0, /) -> Any:
+    """
+    Terminate current program with a given exit code. Underlyingly, this
+    function raise as `SystemExit` exception. If an argument is given, its
+    value given as an argument to `SystemExit`.
+    """
+    ...
+
+stderr: Any
+stdout: Any
+stdin: Any
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/time.pyi` & `micropython_esp32_stubs-1.20.0.post1/time.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-"""
-time related functions. See: https://docs.micropython.org/en/v1.19.1/library/time.html
-
-|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
-
-The ``time`` module provides functions for getting the current time and date,
-measuring time intervals, and for delays.
-
-**Time Epoch**: Unix port uses standard for POSIX systems epoch of
-1970-01-01 00:00:00 UTC. However, embedded ports use epoch of
-2000-01-01 00:00:00 UTC.
-
-**Maintaining actual calendar date/time**: This requires a
-Real Time Clock (RTC). On systems with underlying OS (including some
-RTOS), an RTC may be implicit. Setting and maintaining actual calendar
-time is responsibility of OS/RTOS and is done outside of MicroPython,
-it just uses OS API to query date/time. On baremetal ports however
-system time depends on ``machine.RTC()`` object. The current calendar time
-may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
-by following means:
-
-* By a backup battery (which may be an additional, optional component for
-  a particular board).
-* Using networked time protocol (requires setup by a port/user).
-* Set manually by a user on each power-up (many boards then maintain
-  RTC time across hard resets, though some may require setting it again
-  in such case).
-
-If actual calendar time is not maintained with a system/MicroPython RTC,
-functions below which require reference to current absolute time may
-behave not as expected.
-"""
-from typing import Optional, Tuple, Any
-
-def ticks_diff(ticks1, ticks2) -> int:
-    """
-    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
-    or `ticks_cpu()` functions, as a signed value which may wrap around.
-
-    The argument order is the same as for subtraction
-    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
-    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
-    directly using subtraction on them will produce incorrect result. That is why
-    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
-    arithmetics to produce correct result even for wrap-around values (as long as they not
-    too distant inbetween, see below). The function returns **signed** value in the range
-    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
-    two's-complement signed binary integers). If the result is negative, it means that
-    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
-    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
-    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
-    not hold, incorrect result will be returned. Specifically, if two tick values are
-    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
-    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
-    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
-    to the negative range of possible values.
-
-    Informal rationale of the constraints above: Suppose you are locked in a room with no
-    means to monitor passing of time except a standard 12-notch clock. Then if you look at
-    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
-    long sleep), then once you finally look again, it may seem to you that only 1 hour
-    has passed. To avoid this mistake, just look at the clock regularly. Your application
-    should do the same. "Too long sleep" metaphor also maps directly to application
-    behaviour: don't let your application run any single task for too long. Run tasks
-    in steps, and do time-keeping inbetween.
-
-    `ticks_diff()` is designed to accommodate various usage patterns, among them:
-
-    * Polling with timeout. In this case, the order of events is known, and you will deal
-      only with positive results of `ticks_diff()`::
-
-         # Wait for GPIO pin to be asserted, but at most 500us
-         start = time.ticks_us()
-         while pin.value() == 0:
-             if time.ticks_diff(time.ticks_us(), start) > 500:
-                 raise TimeoutError
-
-    * Scheduling events. In this case, `ticks_diff()` result may be negative
-      if an event is overdue::
-
-         # This code snippet is not optimized
-         now = time.ticks_ms()
-         scheduled_time = task.scheduled_time()
-         if ticks_diff(scheduled_time, now) > 0:
-             print("Too early, let's nap")
-             sleep_ms(ticks_diff(scheduled_time, now))
-             task.run()
-         elif ticks_diff(scheduled_time, now) == 0:
-             print("Right at time!")
-             task.run()
-         elif ticks_diff(scheduled_time, now) < 0:
-             print("Oops, running late, tell task to run faster!")
-             task.run(run_faster=true)
-
-    Note: Do not pass `time()` values to `ticks_diff()`, you should use
-    normal mathematical operations on them. But note that `time()` may (and will)
-    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
-
-    """
-    ...
-
-def ticks_add(ticks, delta) -> Any:
-    """
-    Offset ticks value by a given number, which can be either positive or negative.
-    Given a *ticks* value, this function allows to calculate ticks value *delta*
-    ticks before or after it, following modular-arithmetic definition of tick values
-    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
-    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
-    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
-    or numeric expression. `ticks_add()` is useful for calculating deadlines for
-    events/tasks. (Note: you must use `ticks_diff()` function to work with
-    deadlines.)
-
-    Examples::
-
-         # Find out what ticks value there was 100ms ago
-         print(ticks_add(time.ticks_ms(), -100))
-
-         # Calculate deadline for operation and test for it
-         deadline = ticks_add(time.ticks_ms(), 200)
-         while ticks_diff(deadline, time.ticks_ms()) > 0:
-             do_a_little_of_something()
-
-         # Find out TICKS_MAX used by this port
-         print(ticks_add(0, -1))
-
-    """
-    ...
-
-def ticks_cpu() -> Any:
-    """
-    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
-    in the system. This is usually CPU clocks, and that's why the function is named that
-    way. But it doesn't have to be a CPU clock, some other timing source available in a
-    system (e.g. high-resolution timer) can be used instead. The exact timing unit
-    (resolution) of this function is not specified on ``time`` module level, but
-    documentation for a specific port may provide more specific information. This
-    function is intended for very fine benchmarking or very tight real-time loops.
-    Avoid using it in portable code.
-
-    Availability: Not every port implements this function.
-
-    """
-    ...
-
-class time:
-    """
-    Returns the number of seconds, as an integer, since the Epoch, assuming that
-    underlying RTC is set and maintained as described above. If an RTC is not set, this
-    function returns number of seconds since a port-specific reference point in time (for
-    embedded boards without a battery-backed RTC, usually since power up or reset). If you
-    want to develop portable MicroPython application, you should not rely on this function
-    to provide higher than second precision.  If you need higher precision, absolute
-    timestamps, use `time_ns()`.  If relative times are acceptable then use the
-    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
-    `localtime()` without an argument is a better choice.
-    """
-
-    def __init__(self) -> None: ...
-
-def ticks_ms() -> int:
-    """
-    Returns an increasing millisecond counter with an arbitrary reference point, that
-    wraps around after some value.
-
-    The wrap-around value is not explicitly exposed, but we will
-    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
-    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
-    two, but otherwise may differ from port to port. The same period value is used
-    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
-    simplicity). Thus, these functions will return a value in range [*0* ..
-    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
-    non-negative values are used. For the most part, you should treat values returned
-    by these functions as opaque. The only operations available for them are
-    `ticks_diff()` and `ticks_add()` functions described below.
-
-    Note: Performing standard mathematical operations (+, -) or relational
-    operators (<, <=, >, >=) directly on these value will lead to invalid
-    result. Performing mathematical operations and then passing their results
-    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
-    invalid results from the latter functions.
-    """
-    ...
-
-def ticks_us() -> Any:
-    """
-    Just like `ticks_ms()` above, but in microseconds.
-    """
-    ...
-
-def time_ns() -> int:
-    """
-    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
-    a big integer, so will allocate on the heap).
-    """
-    ...
-
-def localtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_us(us) -> None:
-    """
-    Delay for given number of microseconds, should be positive or 0.
-
-    This function attempts to provide an accurate delay of at least *us*
-    microseconds, but it may take longer if the system has other higher priority
-    processing to perform.
-    """
-    ...
-
-def gmtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_ms(ms) -> None:
-    """
-    Delay for given number of milliseconds, should be positive or 0.
-
-    This function will delay for at least the given number of milliseconds, but
-    may take longer than that if other processing must take place, for example
-    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
-    this other processing to occur.  Use `sleep_us()` for more precise delays.
-    """
-    ...
-
-def mktime() -> int:
-    """
-    This is inverse function of localtime. It's argument is a full 8-tuple
-    which expresses a time as per localtime. It returns an integer which is
-    the number of seconds since Jan 1, 2000.
-    """
-    ...
-
-def sleep(seconds) -> Any:
-    """
-    Sleep for the given number of seconds. Some boards may accept *seconds* as a
-    floating-point number to sleep for a fractional number of seconds. Note that
-    other boards may not accept a floating-point argument, for compatibility with
-    them use `sleep_ms()` and `sleep_us()` functions.
-    """
-    ...
+"""
+time related functions. See: https://docs.micropython.org/en/v1.20.0/library/time.html
+
+|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
+
+The ``time`` module provides functions for getting the current time and date,
+measuring time intervals, and for delays.
+
+**Time Epoch**: Unix port uses standard for POSIX systems epoch of
+1970-01-01 00:00:00 UTC. However, some embedded ports use epoch of
+2000-01-01 00:00:00 UTC. Epoch year may be determined with ``gmtime(0)[0]``.
+
+**Maintaining actual calendar date/time**: This requires a
+Real Time Clock (RTC). On systems with underlying OS (including some
+RTOS), an RTC may be implicit. Setting and maintaining actual calendar
+time is responsibility of OS/RTOS and is done outside of MicroPython,
+it just uses OS API to query date/time. On baremetal ports however
+system time depends on ``machine.RTC()`` object. The current calendar time
+may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
+by following means:
+
+* By a backup battery (which may be an additional, optional component for
+  a particular board).
+* Using networked time protocol (requires setup by a port/user).
+* Set manually by a user on each power-up (many boards then maintain
+  RTC time across hard resets, though some may require setting it again
+  in such case).
+
+If actual calendar time is not maintained with a system/MicroPython RTC,
+functions below which require reference to current absolute time may
+behave not as expected.
+"""
+from typing import Optional, Tuple, Any
+
+def ticks_diff(ticks1, ticks2) -> int:
+    """
+    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
+    or `ticks_cpu()` functions, as a signed value which may wrap around.
+
+    The argument order is the same as for subtraction
+    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
+    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
+    directly using subtraction on them will produce incorrect result. That is why
+    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
+    arithmetics to produce correct result even for wrap-around values (as long as they not
+    too distant inbetween, see below). The function returns **signed** value in the range
+    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
+    two's-complement signed binary integers). If the result is negative, it means that
+    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
+    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
+    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
+    not hold, incorrect result will be returned. Specifically, if two tick values are
+    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
+    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
+    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
+    to the negative range of possible values.
+
+    Informal rationale of the constraints above: Suppose you are locked in a room with no
+    means to monitor passing of time except a standard 12-notch clock. Then if you look at
+    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
+    long sleep), then once you finally look again, it may seem to you that only 1 hour
+    has passed. To avoid this mistake, just look at the clock regularly. Your application
+    should do the same. "Too long sleep" metaphor also maps directly to application
+    behaviour: don't let your application run any single task for too long. Run tasks
+    in steps, and do time-keeping inbetween.
+
+    `ticks_diff()` is designed to accommodate various usage patterns, among them:
+
+    * Polling with timeout. In this case, the order of events is known, and you will deal
+      only with positive results of `ticks_diff()`::
+
+         # Wait for GPIO pin to be asserted, but at most 500us
+         start = time.ticks_us()
+         while pin.value() == 0:
+             if time.ticks_diff(time.ticks_us(), start) > 500:
+                 raise TimeoutError
+
+    * Scheduling events. In this case, `ticks_diff()` result may be negative
+      if an event is overdue::
+
+         # This code snippet is not optimized
+         now = time.ticks_ms()
+         scheduled_time = task.scheduled_time()
+         if ticks_diff(scheduled_time, now) > 0:
+             print("Too early, let's nap")
+             sleep_ms(ticks_diff(scheduled_time, now))
+             task.run()
+         elif ticks_diff(scheduled_time, now) == 0:
+             print("Right at time!")
+             task.run()
+         elif ticks_diff(scheduled_time, now) < 0:
+             print("Oops, running late, tell task to run faster!")
+             task.run(run_faster=true)
+
+    Note: Do not pass `time()` values to `ticks_diff()`, you should use
+    normal mathematical operations on them. But note that `time()` may (and will)
+    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
+
+    """
+    ...
+
+def ticks_add(ticks, delta) -> Any:
+    """
+    Offset ticks value by a given number, which can be either positive or negative.
+    Given a *ticks* value, this function allows to calculate ticks value *delta*
+    ticks before or after it, following modular-arithmetic definition of tick values
+    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
+    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
+    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
+    or numeric expression. `ticks_add()` is useful for calculating deadlines for
+    events/tasks. (Note: you must use `ticks_diff()` function to work with
+    deadlines.)
+
+    Examples::
+
+         # Find out what ticks value there was 100ms ago
+         print(ticks_add(time.ticks_ms(), -100))
+
+         # Calculate deadline for operation and test for it
+         deadline = ticks_add(time.ticks_ms(), 200)
+         while ticks_diff(deadline, time.ticks_ms()) > 0:
+             do_a_little_of_something()
+
+         # Find out TICKS_MAX used by this port
+         print(ticks_add(0, -1))
+
+    """
+    ...
+
+def ticks_cpu() -> Any:
+    """
+    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
+    in the system. This is usually CPU clocks, and that's why the function is named that
+    way. But it doesn't have to be a CPU clock, some other timing source available in a
+    system (e.g. high-resolution timer) can be used instead. The exact timing unit
+    (resolution) of this function is not specified on ``time`` module level, but
+    documentation for a specific port may provide more specific information. This
+    function is intended for very fine benchmarking or very tight real-time loops.
+    Avoid using it in portable code.
+
+    Availability: Not every port implements this function.
+
+    """
+    ...
+
+class time:
+    """
+    Returns the number of seconds, as an integer, since the Epoch, assuming that
+    underlying RTC is set and maintained as described above. If an RTC is not set, this
+    function returns number of seconds since a port-specific reference point in time (for
+    embedded boards without a battery-backed RTC, usually since power up or reset). If you
+    want to develop portable MicroPython application, you should not rely on this function
+    to provide higher than second precision.  If you need higher precision, absolute
+    timestamps, use `time_ns()`.  If relative times are acceptable then use the
+    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
+    `localtime()` without an argument is a better choice.
+    """
+
+    def __init__(self) -> None: ...
+
+def ticks_ms() -> int:
+    """
+    Returns an increasing millisecond counter with an arbitrary reference point, that
+    wraps around after some value.
+
+    The wrap-around value is not explicitly exposed, but we will
+    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
+    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
+    two, but otherwise may differ from port to port. The same period value is used
+    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
+    simplicity). Thus, these functions will return a value in range [*0* ..
+    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
+    non-negative values are used. For the most part, you should treat values returned
+    by these functions as opaque. The only operations available for them are
+    `ticks_diff()` and `ticks_add()` functions described below.
+
+    Note: Performing standard mathematical operations (+, -) or relational
+    operators (<, <=, >, >=) directly on these value will lead to invalid
+    result. Performing mathematical operations and then passing their results
+    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
+    invalid results from the latter functions.
+    """
+    ...
+
+def ticks_us() -> Any:
+    """
+    Just like `ticks_ms()` above, but in microseconds.
+    """
+    ...
+
+def time_ns() -> int:
+    """
+    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
+    a big integer, so will allocate on the heap).
+    """
+    ...
+
+def localtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_us(us) -> None:
+    """
+    Delay for given number of microseconds, should be positive or 0.
+
+    This function attempts to provide an accurate delay of at least *us*
+    microseconds, but it may take longer if the system has other higher priority
+    processing to perform.
+    """
+    ...
+
+def gmtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_ms(ms) -> None:
+    """
+    Delay for given number of milliseconds, should be positive or 0.
+
+    This function will delay for at least the given number of milliseconds, but
+    may take longer than that if other processing must take place, for example
+    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
+    this other processing to occur.  Use `sleep_us()` for more precise delays.
+    """
+    ...
+
+def mktime() -> int:
+    """
+    This is inverse function of localtime. It's argument is a full 8-tuple
+    which expresses a time as per localtime. It returns an integer which is
+    the number of seconds since Jan 1, 2000.
+    """
+    ...
+
+def sleep(seconds) -> Any:
+    """
+    Sleep for the given number of seconds. Some boards may accept *seconds* as a
+    floating-point number to sleep for a fractional number of seconds. Note that
+    other boards may not accept a floating-point argument, for compatibility with
+    them use `sleep_ms()` and `sleep_us()` functions.
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/uarray.pyi` & `micropython_esp32_stubs-1.20.0.post1/uarray.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-"""
-efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.19.1/library/array.html
-
-|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
-
-Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
-``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
-floating-point support).
-"""
-from typing import Optional, Any
-
-class array:
-    """
-    Create array with elements of given type. Initial contents of the
-    array are given by *iterable*. If it is not provided, an empty
-    array is created.
-    """
-
-    def extend(self, iterable) -> Any:
-        """
-        Append new elements as contained in *iterable* to the end of
-        array, growing it.
-        """
-        ...
-    def decode(self, *args, **kwargs) -> Any: ...
-    def append(self, val) -> Any:
-        """
-        Append new element *val* to the end of array, growing it.
-        """
-        ...
-    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
+"""
+efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.20.0/library/array.html
+
+|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
+
+Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
+``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
+floating-point support).
+"""
+from typing import List, Optional, Any
+
+class array:
+    """
+    Create array with elements of given type. Initial contents of the
+    array are given by *iterable*. If it is not provided, an empty
+    array is created.
+    """
+
+    def extend(self, iterable) -> Any:
+        """
+        Append new elements as contained in *iterable* to the end of
+        array, growing it.
+        """
+        ...
+    def append(self, val) -> Any:
+        """
+        Append new element *val* to the end of array, growing it.
+        """
+        ...
+    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/uasyncio/core.pyi` & `micropython_esp32_stubs-1.20.0.post1/uasyncio/core.pyi`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from .task import Task as Task, TaskQueue as TaskQueue
-from _typeshed import Incomplete
-
-class CancelledError(BaseException): ...
-class TimeoutError(Exception): ...
-
-_exc_context: Incomplete
-
-class SingletonGenerator:
-    state: Incomplete
-    exc: Incomplete
-    def __init__(self) -> None: ...
-    def __iter__(self): ...
-    def __next__(self) -> None: ...
-
-def sleep_ms(t, sgen=...): ...
-def sleep(t): ...
-
-class IOQueue:
-    poller: Incomplete
-    map: Incomplete
-    def __init__(self) -> None: ...
-    def _enqueue(self, s, idx) -> None: ...
-    def _dequeue(self, s) -> None: ...
-    def queue_read(self, s) -> None: ...
-    def queue_write(self, s) -> None: ...
-    def remove(self, task) -> None: ...
-    def wait_io_event(self, dt) -> None: ...
-
-def _promote_to_task(aw): ...
-def create_task(coro): ...
-def run_until_complete(main_task: Incomplete | None = ...): ...
-def run(coro): ...
-async def _stopper() -> None: ...
-
-_stop_task: Incomplete
-
-class Loop:
-    _exc_handler: Incomplete
-    def create_task(coro): ...
-    def run_forever() -> None: ...
-    def run_until_complete(aw): ...
-    def stop() -> None: ...
-    def close() -> None: ...
-    def set_exception_handler(handler) -> None: ...
-    def get_exception_handler(): ...
-    def default_exception_handler(loop, context) -> None: ...
-    def call_exception_handler(context) -> None: ...
-
-def get_event_loop(runq_len: int = ..., waitq_len: int = ...): ...
-def current_task(): ...
-def new_event_loop(): ...
+from .task import Task as Task, TaskQueue as TaskQueue
+from _typeshed import Incomplete
+
+class CancelledError(BaseException): ...
+class TimeoutError(Exception): ...
+
+_exc_context: Incomplete
+
+class SingletonGenerator:
+    state: Incomplete
+    exc: Incomplete
+    def __init__(self) -> None: ...
+    def __iter__(self): ...
+    def __next__(self) -> None: ...
+
+def sleep_ms(t, sgen=...): ...
+def sleep(t): ...
+
+class IOQueue:
+    poller: Incomplete
+    map: Incomplete
+    def __init__(self) -> None: ...
+    def _enqueue(self, s, idx) -> None: ...
+    def _dequeue(self, s) -> None: ...
+    def queue_read(self, s) -> None: ...
+    def queue_write(self, s) -> None: ...
+    def remove(self, task) -> None: ...
+    def wait_io_event(self, dt) -> None: ...
+
+def _promote_to_task(aw): ...
+def create_task(coro): ...
+def run_until_complete(main_task: Incomplete | None = ...): ...
+def run(coro): ...
+async def _stopper() -> None: ...
+
+_stop_task: Incomplete
+
+class Loop:
+    _exc_handler: Incomplete
+    def create_task(coro): ...
+    def run_forever() -> None: ...
+    def run_until_complete(aw): ...
+    def stop() -> None: ...
+    def close() -> None: ...
+    def set_exception_handler(handler) -> None: ...
+    def get_exception_handler(): ...
+    def default_exception_handler(loop, context) -> None: ...
+    def call_exception_handler(context) -> None: ...
+
+def get_event_loop(runq_len: int = ..., waitq_len: int = ...): ...
+def current_task(): ...
+def new_event_loop(): ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/uasyncio/event.pyi` & `micropython_esp32_stubs-1.20.0.post1/uasyncio/event.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import uio
-from . import core as core
-from _typeshed import Incomplete
-from collections.abc import Generator
-
-class Event:
-    state: bool
-    waiting: Incomplete
-    def __init__(self) -> None: ...
-    def is_set(self): ...
-    def set(self) -> None: ...
-    def clear(self) -> None: ...
-    async def wait(self) -> Generator[None, None, Incomplete]: ...
-
-class ThreadSafeFlag(uio.IOBase):
-    _flag: int
-    def __init__(self) -> None: ...
-    def ioctl(self, req, flags): ...
-    def set(self) -> None: ...
-    async def wait(self) -> Generator[Incomplete, None, None]: ...
+import uio
+from . import core as core
+from _typeshed import Incomplete
+from collections.abc import Generator
+
+class Event:
+    state: bool
+    waiting: Incomplete
+    def __init__(self) -> None: ...
+    def is_set(self): ...
+    def set(self) -> None: ...
+    def clear(self) -> None: ...
+    def wait(self) -> Generator[None, None, Incomplete]: ...
+
+class ThreadSafeFlag(uio.IOBase):
+    state: int
+    def __init__(self) -> None: ...
+    def ioctl(self, req, flags): ...
+    def set(self) -> None: ...
+    def clear(self) -> None: ...
+    async def wait(self) -> Generator[Incomplete, None, None]: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/uasyncio/stream.pyi` & `micropython_esp32_stubs-1.20.0.post1/uasyncio/stream.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from . import core as core
-from _typeshed import Incomplete
-from collections.abc import Generator
-
-class Stream:
-    s: Incomplete
-    e: Incomplete
-    out_buf: bytes
-    def __init__(self, s, e=...) -> None: ...
-    def get_extra_info(self, v): ...
-    async def __aenter__(self): ...
-    async def __aexit__(self, exc_type, exc, tb) -> None: ...
-    def close(self) -> None: ...
-    async def wait_closed(self) -> None: ...
-    async def read(self, n) -> Generator[Incomplete, None, Incomplete]: ...
-    async def readinto(self, buf) -> Generator[Incomplete, None, Incomplete]: ...
-    async def readexactly(self, n) -> Generator[Incomplete, None, Incomplete]: ...
-    async def readline(self) -> Generator[Incomplete, None, Incomplete]: ...
-    def write(self, buf) -> None: ...
-    async def drain(self) -> Generator[Incomplete, None, None]: ...
-
-StreamReader = Stream
-StreamWriter = Stream
-
-async def open_connection(host, port) -> Generator[Incomplete, None, Incomplete]: ...
-
-class Server:
-    async def __aenter__(self): ...
-    async def __aexit__(self, exc_type, exc, tb) -> None: ...
-    def close(self) -> None: ...
-    async def wait_closed(self) -> None: ...
-    async def _serve(self, s, cb) -> Generator[Incomplete, None, None]: ...
-
-async def start_server(cb, host, port, backlog: int = ...): ...
-async def stream_awrite(self, buf, off: int = ..., sz: int = ...) -> None: ...
+from . import core as core
+from _typeshed import Incomplete
+from collections.abc import Generator
+
+class Stream:
+    s: Incomplete
+    e: Incomplete
+    out_buf: bytes
+    def __init__(self, s, e=...) -> None: ...
+    def get_extra_info(self, v): ...
+    async def __aenter__(self): ...
+    async def __aexit__(self, exc_type, exc, tb) -> None: ...
+    def close(self) -> None: ...
+    async def wait_closed(self) -> None: ...
+    def read(self, n: int = ...) -> Generator[Incomplete, None, Incomplete]: ...
+    def readinto(self, buf) -> Generator[Incomplete, None, Incomplete]: ...
+    def readexactly(self, n) -> Generator[Incomplete, None, Incomplete]: ...
+    def readline(self) -> Generator[Incomplete, None, Incomplete]: ...
+    def write(self, buf) -> None: ...
+    def drain(self) -> Generator[Incomplete, None, Incomplete]: ...
+
+StreamReader = Stream
+StreamWriter = Stream
+
+def open_connection(host, port) -> Generator[Incomplete, None, Incomplete]: ...
+
+class Server:
+    async def __aenter__(self): ...
+    async def __aexit__(self, exc_type, exc, tb) -> None: ...
+    def close(self) -> None: ...
+    async def wait_closed(self) -> None: ...
+    async def _serve(self, s, cb) -> Generator[Incomplete, None, None]: ...
+
+async def start_server(cb, host, port, backlog: int = ...): ...
+async def stream_awrite(self, buf, off: int = ..., sz: int = ...) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/ubinascii.pyi` & `micropython_esp32_stubs-1.20.0.post1/ubinascii.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""
-binary/ASCII conversions. See: https://docs.micropython.org/en/v1.19.1/library/binascii.html
-
-|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
-
-This module implements conversions between binary data and various
-encodings of it in ASCII form (in both directions).
-"""
-from typing import Optional, Any
-
-def crc32(*args, **kwargs) -> Any: ...
-def hexlify(data, sep: Optional[Any] = None) -> bytes:
-    """
-    Convert the bytes in the *data* object to a hexadecimal representation.
-    Returns a bytes object.
-
-    If the additional argument *sep* is supplied it is used as a separator
-    between hexadecimal values.
-    """
-    ...
-
-def unhexlify(data) -> bytes:
-    """
-    Convert hexadecimal data to binary representation. Returns bytes string.
-    (i.e. inverse of hexlify)
-    """
-    ...
-
-def b2a_base64(data, *, newline=True) -> bytes:
-    """
-    Encode binary data in base64 format, as in `RFC 3548
-    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
-    followed by a newline character if newline is true, as a bytes object.
-    """
-    ...
-
-def a2b_base64(data) -> bytes:
-    """
-    Decode base64-encoded data, ignoring invalid characters in the input.
-    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
-    Returns a bytes object.
-    """
-    ...
+"""
+binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20.0/library/binascii.html
+
+|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
+
+This module implements conversions between binary data and various
+encodings of it in ASCII form (in both directions).
+"""
+from typing import Optional, Any
+
+def crc32(*args, **kwargs) -> Any: ...
+def hexlify(data, sep: Optional[Any] = None) -> bytes:
+    """
+    Convert the bytes in the *data* object to a hexadecimal representation.
+    Returns a bytes object.
+
+    If the additional argument *sep* is supplied it is used as a separator
+    between hexadecimal values.
+    """
+    ...
+
+def unhexlify(data) -> bytes:
+    """
+    Convert hexadecimal data to binary representation. Returns bytes string.
+    (i.e. inverse of hexlify)
+    """
+    ...
+
+def b2a_base64(data, *, newline=True) -> bytes:
+    """
+    Encode binary data in base64 format, as in `RFC 3548
+    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
+    followed by a newline character if newline is true, as a bytes object.
+    """
+    ...
+
+def a2b_base64(data) -> bytes:
+    """
+    Decode base64-encoded data, ignoring invalid characters in the input.
+    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
+    Returns a bytes object.
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/ubluetooth.pyi` & `micropython_esp32_stubs-1.20.0.post1/bluetooth.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,589 +1,623 @@
-"""
-Low-level Bluetooth radio functionality. See: https://docs.micropython.org/en/v1.19.1/library/bluetooth.html
-
-This module provides an interface to a Bluetooth controller on a board.
-Currently this supports Bluetooth Low Energy (BLE) in Central, Peripheral,
-Broadcaster, and Observer roles, as well as GATT Server and Client and L2CAP
-connection-oriented-channels. A device may operate in multiple roles
-concurrently. Pairing (and bonding) is supported on some ports.
-
-This API is intended to match the low-level Bluetooth protocol and provide
-building-blocks for higher-level abstractions such as specific device types.
-
-``Note:`` This module is still under development and its classes, functions,
-          methods and constants are subject to change.
-"""
-from typing import Optional, Tuple, Any
-
-FLAG_NOTIFY: int
-FLAG_READ: int
-FLAG_WRITE: int
-FLAG_INDICATE: int
-FLAG_WRITE_NO_RESPONSE: int
-
-class UUID:
-    """
-    Creates a UUID instance with the specified **value**.
-
-    The **value** can be either:
-
-    - A 16-bit integer. e.g. ``0x2908``.
-    - A 128-bit UUID string. e.g. ``'6E400001-B5A3-F393-E0A9-E50E24DCCA9E'``.
-    """
-
-    def __init__(self, value, /) -> None: ...
-
-class BLE:
-    """
-    Returns the singleton BLE object.
-    """
-
-    def gatts_notify(self, conn_handle, value_handle, data=None, /) -> None:
-        """
-        Sends a notification request to a connected client.
-
-        If *data* is not ``None``, then that value is sent to the client as part of
-        the notification. The local value will not be modified.
-
-        Otherwise, if *data* is ``None``, then the current local value (as
-        set with :meth:`gatts_write <BLE.gatts_write>`) will be sent.
-
-        **Note:** The notification will be sent regardless of the subscription
-        status of the client to this characteristic.
-        """
-        ...
-    def gatts_indicate(self, conn_handle, value_handle, /) -> None:
-        """
-        Sends an indication request containing the characteristic's current value to
-        a connected client.
-
-        On acknowledgment (or failure, e.g. timeout), the
-        ``_IRQ_GATTS_INDICATE_DONE`` event will be raised.
-
-        **Note:** The indication will be sent regardless of the subscription
-        status of the client to this characteristic.
-        """
-        ...
-    def gattc_write(self, conn_handle, value_handle, data, mode=0, /) -> None:
-        """
-        Issue a remote write to a connected server for the specified
-        characteristic or descriptor handle.
-
-        The argument *mode* specifies the write behaviour, with the currently
-        supported values being:
-
-            * ``mode=0`` (default) is a write-without-response: the write will
-              be sent to the remote server but no confirmation will be
-              returned, and no event will be raised.
-            * ``mode=1`` is a write-with-response: the remote server is
-              requested to send a response/acknowledgement that it received the
-              data.
-
-        If a response is received from the remote server the
-        ``_IRQ_GATTC_WRITE_DONE`` event will be raised.
-        """
-        ...
-    def gattc_read(self, conn_handle, value_handle, /) -> None:
-        """
-        Issue a remote read to a connected server for the specified
-        characteristic or descriptor handle.
-
-        When a value is available, the ``_IRQ_GATTC_READ_RESULT`` event will be
-        raised. Additionally, the ``_IRQ_GATTC_READ_DONE`` will be raised.
-        """
-        ...
-    def gattc_exchange_mtu(self, conn_handle, /) -> Any:
-        """
-        Initiate MTU exchange with a connected server, using the preferred MTU
-        set using ``BLE.config(mtu=value)``.
-
-        The ``_IRQ_MTU_EXCHANGED`` event will be raised when MTU exchange
-        completes.
-
-        **Note:** MTU exchange is typically initiated by the central. When using
-        the BlueKitchen stack in the central role, it does not support a remote
-        peripheral initiating the MTU exchange. NimBLE works for both roles.
-
-        """
-        ...
-    def gatts_read(self, value_handle, /) -> Any:
-        """
-        Reads the local value for this handle (which has either been written by
-        :meth:`gatts_write <BLE.gatts_write>` or by a remote client).
-        """
-        ...
-    def gatts_write(self, value_handle, data, send_update=False, /) -> None:
-        """
-        Writes the local value for this handle, which can be read by a client.
-
-        If *send_update* is ``True``, then any subscribed clients will be notified
-        (or indicated, depending on what they're subscribed to and which operations
-        the characteristic supports) about this write.
-        """
-        ...
-    def gatts_set_buffer(self, value_handle, len, append=False, /) -> None:
-        """
-        Sets the internal buffer size for a value in bytes. This will limit the
-        largest possible write that can be received. The default is 20.
-
-        Setting *append* to ``True`` will make all remote writes append to, rather
-        than replace, the current value. At most *len* bytes can be buffered in
-        this way. When you use :meth:`gatts_read <BLE.gatts_read>`, the value will
-        be cleared after reading. This feature is useful when implementing something
-        like the Nordic UART Service.
-        """
-        ...
-    def gatts_register_services(self, services_definition, /) -> Any:
-        """
-        Configures the server with the specified services, replacing any
-        existing services.
-
-        *services_definition* is a list of **services**, where each **service** is a
-        two-element tuple containing a UUID and a list of **characteristics**.
-
-        Each **characteristic** is a two-or-three-element tuple containing a UUID, a
-        **flags** value, and optionally a list of *descriptors*.
-
-        Each **descriptor** is a two-element tuple containing a UUID and a **flags**
-        value.
-
-        The **flags** are a bitwise-OR combination of the flags defined below. These
-        set both the behaviour of the characteristic (or descriptor) as well as the
-        security and privacy requirements.
-
-        The return value is a list (one element per service) of tuples (each element
-        is a value handle). Characteristics and descriptor handles are flattened
-        into the same tuple, in the order that they are defined.
-
-        The following example registers two services (Heart Rate, and Nordic UART)::
-
-            HR_UUID = bluetooth.UUID(0x180D)
-            HR_CHAR = (bluetooth.UUID(0x2A37), bluetooth.FLAG_READ | bluetooth.FLAG_NOTIFY,)
-            HR_SERVICE = (HR_UUID, (HR_CHAR,),)
-            UART_UUID = bluetooth.UUID('6E400001-B5A3-F393-E0A9-E50E24DCCA9E')
-            UART_TX = (bluetooth.UUID('6E400003-B5A3-F393-E0A9-E50E24DCCA9E'), bluetooth.FLAG_READ | bluetooth.FLAG_NOTIFY,)
-            UART_RX = (bluetooth.UUID('6E400002-B5A3-F393-E0A9-E50E24DCCA9E'), bluetooth.FLAG_WRITE,)
-            UART_SERVICE = (UART_UUID, (UART_TX, UART_RX,),)
-            SERVICES = (HR_SERVICE, UART_SERVICE,)
-            ( (hr,), (tx, rx,), ) = bt.gatts_register_services(SERVICES)
-
-        The three value handles (``hr``, ``tx``, ``rx``) can be used with
-        :meth:`gatts_read <BLE.gatts_read>`, :meth:`gatts_write <BLE.gatts_write>`, :meth:`gatts_notify <BLE.gatts_notify>`, and
-        :meth:`gatts_indicate <BLE.gatts_indicate>`.
-
-        **Note:** Advertising must be stopped before registering services.
-
-        Available flags for characteristics and descriptors are::
-
-            from micropython import const
-            _FLAG_BROADCAST = const(0x0001)
-            _FLAG_READ = const(0x0002)
-            _FLAG_WRITE_NO_RESPONSE = const(0x0004)
-            _FLAG_WRITE = const(0x0008)
-            _FLAG_NOTIFY = const(0x0010)
-            _FLAG_INDICATE = const(0x0020)
-            _FLAG_AUTHENTICATED_SIGNED_WRITE = const(0x0040)
-
-            _FLAG_AUX_WRITE = const(0x0100)
-            _FLAG_READ_ENCRYPTED = const(0x0200)
-            _FLAG_READ_AUTHENTICATED = const(0x0400)
-            _FLAG_READ_AUTHORIZED = const(0x0800)
-            _FLAG_WRITE_ENCRYPTED = const(0x1000)
-            _FLAG_WRITE_AUTHENTICATED = const(0x2000)
-            _FLAG_WRITE_AUTHORIZED = const(0x4000)
-
-        As for the IRQs above, any required constants should be added to your Python code.
-        """
-        ...
-    def irq(self, handler, /) -> int:
-        """
-            Registers a callback for events from the BLE stack. The *handler* takes two
-            arguments, ``event`` (which will be one of the codes below) and ``data``
-            (which is an event-specific tuple of values).
-
-            **Note:** As an optimisation to prevent unnecessary allocations, the ``addr``,
-            ``adv_data``, ``char_data``, ``notify_data``, and ``uuid`` entries in the
-            tuples are read-only memoryview instances pointing to :mod:`bluetooth`'s internal
-            ringbuffer, and are only valid during the invocation of the IRQ handler
-            function.  If your program needs to save one of these values to access after
-            the IRQ handler has returned (e.g. by saving it in a class instance or global
-            variable), then it needs to take a copy of the data, either by using ``bytes()``
-            or ``bluetooth.UUID()``, like this::
-
-                connected_addr = bytes(addr)  # equivalently: adv_data, char_data, or notify_data
-                matched_uuid = bluetooth.UUID(uuid)
-
-            For example, the IRQ handler for a scan result might inspect the ``adv_data``
-            to decide if it's the correct device, and only then copy the address data to be
-            used elsewhere in the program.  And to print data from within the IRQ handler,
-            ``print(bytes(addr))`` will be needed.
-
-            An event handler showing all possible events::
-
-                def bt_irq(event, data):
-                    if event == _IRQ_CENTRAL_CONNECT:
-                        # A central has connected to this peripheral.
-                        conn_handle, addr_type, addr = data
-                    elif event == _IRQ_CENTRAL_DISCONNECT:
-                        # A central has disconnected from this peripheral.
-                        conn_handle, addr_type, addr = data
-                    elif event == _IRQ_GATTS_WRITE:
-                        # A client has written to this characteristic or descriptor.
-                        conn_handle, attr_handle = data
-                    elif event == _IRQ_GATTS_READ_REQUEST:
-                        # A client has issued a read. Note: this is only supported on STM32.
-                        # Return a non-zero integer to deny the read (see below), or zero (or None)
-                        # to accept the read.
-                        conn_handle, attr_handle = data
-                    elif event == _IRQ_SCAN_RESULT:
-                        # A single scan result.
-                        addr_type, addr, adv_type, rssi, adv_data = data
-                    elif event == _IRQ_SCAN_DONE:
-                        # Scan duration finished or manually stopped.
-                        pass
-                    elif event == _IRQ_PERIPHERAL_CONNECT:
-                        # A successful gap_connect().
-                        conn_handle, addr_type, addr = data
-                    elif event == _IRQ_PERIPHERAL_DISCONNECT:
-                        # Connected peripheral has disconnected.
-                        conn_handle, addr_type, addr = data
-                    elif event == _IRQ_GATTC_SERVICE_RESULT:
-                        # Called for each service found by gattc_discover_services().
-                        conn_handle, start_handle, end_handle, uuid = data
-                    elif event == _IRQ_GATTC_SERVICE_DONE:
-                        # Called once service discovery is complete.
-                        # Note: Status will be zero on success, implementation-specific value otherwise.
-                        conn_handle, status = data
-                    elif event == _IRQ_GATTC_CHARACTERISTIC_RESULT:
-                        # Called for each characteristic found by gattc_discover_services().
-                        conn_handle, def_handle, value_handle, properties, uuid = data
-                    elif event == _IRQ_GATTC_CHARACTERISTIC_DONE:
-                        # Called once service discovery is complete.
-                        # Note: Status will be zero on success, implementation-specific value otherwise.
-                        conn_handle, status = data
-                    elif event == _IRQ_GATTC_DESCRIPTOR_RESULT:
-                        # Called for each descriptor found by gattc_discover_descriptors().
-                        conn_handle, dsc_handle, uuid = data
-                    elif event == _IRQ_GATTC_DESCRIPTOR_DONE:
-                        # Called once service discovery is complete.
-                        # Note: Status will be zero on success, implementation-specific value otherwise.
-                        conn_handle, status = data
-                    elif event == _IRQ_GATTC_READ_RESULT:
-                        # A gattc_read() has completed.
-                        conn_handle, value_handle, char_data = data
-                    elif event == _IRQ_GATTC_READ_DONE:
-                        # A gattc_read() has completed.
-                        # Note: The value_handle will be zero on btstack (but present on NimBLE).
-                        # Note: Status will be zero on success, implementation-specific value otherwise.
-                        conn_handle, value_handle, status = data
-                    elif event == _IRQ_GATTC_WRITE_DONE:
-                        # A gattc_write() has completed.
-                        # Note: The value_handle will be zero on btstack (but present on NimBLE).
-                        # Note: Status will be zero on success, implementation-specific value otherwise.
-                        conn_handle, value_handle, status = data
-                    elif event == _IRQ_GATTC_NOTIFY:
-                        # A server has sent a notify request.
-                        conn_handle, value_handle, notify_data = data
-                    elif event == _IRQ_GATTC_INDICATE:
-                        # A server has sent an indicate request.
-                        conn_handle, value_handle, notify_data = data
-                    elif event == _IRQ_GATTS_INDICATE_DONE:
-                        # A client has acknowledged the indication.
-                        # Note: Status will be zero on successful acknowledgment, implementation-specific value otherwise.
-                        conn_handle, value_handle, status = data
-                    elif event == _IRQ_MTU_EXCHANGED:
-                        # ATT MTU exchange complete (either initiated by us or the remote device).
-                        conn_handle, mtu = data
-                    elif event == _IRQ_L2CAP_ACCEPT:
-                        # A new channel has been accepted.
-                        # Return a non-zero integer to reject the connection, or zero (or None) to accept.
-                        conn_handle, cid, psm, our_mtu, peer_mtu = data
-                    elif event == _IRQ_L2CAP_CONNECT:
-                        # A new channel is now connected (either as a result of connecting or accepting).
-                        conn_handle, cid, psm, our_mtu, peer_mtu = data
-                    elif event == _IRQ_L2CAP_DISCONNECT:
-                        # Existing channel has disconnected (status is zero), or a connection attempt failed (non-zero status).
-                        conn_handle, cid, psm, status = data
-                    elif event == _IRQ_L2CAP_RECV:
-                        # New data is available on the channel. Use l2cap_recvinto to read.
-                        conn_handle, cid = data
-                    elif event == _IRQ_L2CAP_SEND_READY:
-                        # A previous l2cap_send that returned False has now completed and the channel is ready to send again.
-                        # If status is non-zero, then the transmit buffer overflowed and the application should re-send the data.
-                        conn_handle, cid, status = data
-                    elif event == _IRQ_CONNECTION_UPDATE:
-                        # The remote device has updated connection parameters.
-                        conn_handle, conn_interval, conn_latency, supervision_timeout, status = data
-                    elif event == _IRQ_ENCRYPTION_UPDATE:
-                        # The encryption state has changed (likely as a result of pairing or bonding).
-                        conn_handle, encrypted, authenticated, bonded, key_size = data
-                    elif event == _IRQ_GET_SECRET:
-                        # Return a stored secret.
-                        # If key is None, return the index'th value of this sec_type.
-                        # Otherwise return the corresponding value for this sec_type and key.
-                        sec_type, index, key = data
-                        return value
-                    elif event == _IRQ_SET_SECRET:
-                        # Save a secret to the store for this sec_type and key.
-                        sec_type, key, value = data
-                        return True
-                    elif event == _IRQ_PASSKEY_ACTION:
-                        # Respond to a passkey request during pairing.
-                        # See gap_passkey() for details.
-                        # action will be an action that is compatible with the configured "io" config.
-                        # passkey will be non-zero if action is "numeric comparison".
-                        conn_handle, action, passkey = data
-
-
-        The event codes are::
-
-            from micropython import const
-            _IRQ_CENTRAL_CONNECT = const(1)
-            _IRQ_CENTRAL_DISCONNECT = const(2)
-            _IRQ_GATTS_WRITE = const(3)
-            _IRQ_GATTS_READ_REQUEST = const(4)
-            _IRQ_SCAN_RESULT = const(5)
-            _IRQ_SCAN_DONE = const(6)
-            _IRQ_PERIPHERAL_CONNECT = const(7)
-            _IRQ_PERIPHERAL_DISCONNECT = const(8)
-            _IRQ_GATTC_SERVICE_RESULT = const(9)
-            _IRQ_GATTC_SERVICE_DONE = const(10)
-            _IRQ_GATTC_CHARACTERISTIC_RESULT = const(11)
-            _IRQ_GATTC_CHARACTERISTIC_DONE = const(12)
-            _IRQ_GATTC_DESCRIPTOR_RESULT = const(13)
-            _IRQ_GATTC_DESCRIPTOR_DONE = const(14)
-            _IRQ_GATTC_READ_RESULT = const(15)
-            _IRQ_GATTC_READ_DONE = const(16)
-            _IRQ_GATTC_WRITE_DONE = const(17)
-            _IRQ_GATTC_NOTIFY = const(18)
-            _IRQ_GATTC_INDICATE = const(19)
-            _IRQ_GATTS_INDICATE_DONE = const(20)
-            _IRQ_MTU_EXCHANGED = const(21)
-            _IRQ_L2CAP_ACCEPT = const(22)
-            _IRQ_L2CAP_CONNECT = const(23)
-            _IRQ_L2CAP_DISCONNECT = const(24)
-            _IRQ_L2CAP_RECV = const(25)
-            _IRQ_L2CAP_SEND_READY = const(26)
-            _IRQ_CONNECTION_UPDATE = const(27)
-            _IRQ_ENCRYPTION_UPDATE = const(28)
-            _IRQ_GET_SECRET = const(29)
-            _IRQ_SET_SECRET = const(30)
-
-        For the ``_IRQ_GATTS_READ_REQUEST`` event, the available return codes are::
-
-            _GATTS_NO_ERROR = const(0x00)
-            _GATTS_ERROR_READ_NOT_PERMITTED = const(0x02)
-            _GATTS_ERROR_WRITE_NOT_PERMITTED = const(0x03)
-            _GATTS_ERROR_INSUFFICIENT_AUTHENTICATION = const(0x05)
-            _GATTS_ERROR_INSUFFICIENT_AUTHORIZATION = const(0x08)
-            _GATTS_ERROR_INSUFFICIENT_ENCRYPTION = const(0x0f)
-
-        For the ``_IRQ_PASSKEY_ACTION`` event, the available actions are::
-
-            _PASSKEY_ACTION_NONE = const(0)
-            _PASSKEY_ACTION_INPUT = const(2)
-            _PASSKEY_ACTION_DISPLAY = const(3)
-            _PASSKEY_ACTION_NUMERIC_COMPARISON = const(4)
-
-        In order to save space in the firmware, these constants are not included on the
-        :mod:`bluetooth` module. Add the ones that you need from the list above to your
-        program.
-
-        """
-        ...
-    def gap_connect(self, addr_type, addr, scan_duration_ms=2000, min_conn_interval_us=None, max_conn_interval_us=None, /) -> None:
-        """
-        Connect to a peripheral.
-
-        See :meth:`gap_scan <BLE.gap_scan>` for details about address types.
-
-        To cancel an outstanding connection attempt early, call
-        ``gap_connect(None)``.
-
-        On success, the ``_IRQ_PERIPHERAL_CONNECT`` event will be raised. If
-        cancelling a connection attempt, the ``_IRQ_PERIPHERAL_DISCONNECT`` event
-        will be raised.
-
-        The device will wait up to *scan_duration_ms* to receive an advertising
-        payload from the device.
-
-        The connection interval can be configured in **micro** seconds using either
-        or both of *min_conn_interval_us* and *max_conn_interval_us*. Otherwise a
-        default interval will be chosen, typically between 30000 and 50000
-        microseconds. A shorter interval will increase throughput, at the expense
-        of power usage.
-
-        """
-        ...
-    def gap_advertise(self, interval_us, adv_data=None, *, resp_data=None, connectable=True) -> Any:
-        """
-        Starts advertising at the specified interval (in **micro** seconds). This
-        interval will be rounded down to the nearest 625us. To stop advertising, set
-        *interval_us* to ``None``.
-
-        *adv_data* and *resp_data* can be any type that implements the buffer
-        protocol (e.g. ``bytes``, ``bytearray``, ``str``). *adv_data* is included
-        in all broadcasts, and *resp_data* is send in reply to an active scan.
-
-        **Note:** if *adv_data* (or *resp_data*) is ``None``, then the data passed
-        to the previous call to ``gap_advertise`` will be re-used. This allows a
-        broadcaster to resume advertising with just ``gap_advertise(interval_us)``.
-        To clear the advertising payload pass an empty ``bytes``, i.e. ``b''``.
-
-        """
-        ...
-    def config(self, param, /) -> Tuple:
-        """
-        Get or set configuration values of the BLE interface.  To get a value the
-        parameter name should be quoted as a string, and just one parameter is
-        queried at a time.  To set values use the keyword syntax, and one ore more
-        parameter can be set at a time.
-
-        Currently supported values are:
-
-        - ``'mac'``: The current address in use, depending on the current address mode.
-          This returns a tuple of ``(addr_type, addr)``.
-
-          See :meth:`gatts_write <BLE.gatts_write>` for details about address type.
-
-          This may only be queried while the interface is currently active.
-
-        - ``'addr_mode'``: Sets the address mode. Values can be:
-
-            * 0x00 - PUBLIC - Use the controller's public address.
-            * 0x01 - RANDOM - Use a generated static address.
-            * 0x02 - RPA - Use resolvable private addresses.
-            * 0x03 - NRPA - Use non-resolvable private addresses.
-
-          By default the interface mode will use a PUBLIC address if available, otherwise
-          it will use a RANDOM address.
-
-        - ``'gap_name'``: Get/set the GAP device name used by service 0x1800,
-          characteristic 0x2a00.  This can be set at any time and changed multiple
-          times.
-
-        - ``'rxbuf'``: Get/set the size in bytes of the internal buffer used to store
-          incoming events.  This buffer is global to the entire BLE driver and so
-          handles incoming data for all events, including all characteristics.
-          Increasing this allows better handling of bursty incoming data (for
-          example scan results) and the ability to receive larger characteristic values.
-
-        - ``'mtu'``: Get/set the MTU that will be used during a ATT MTU exchange. The
-          resulting MTU will be the minimum of this and the remote device's MTU.
-          ATT MTU exchange will not happen automatically (unless the remote device initiates
-          it), and must be manually initiated with
-          :meth:`gattc_exchange_mtu<BLE.gattc_exchange_mtu>`.
-          Use the ``_IRQ_MTU_EXCHANGED`` event to discover the MTU for a given connection.
-
-        - ``'bond'``: Sets whether bonding will be enabled during pairing. When
-          enabled, pairing requests will set the "bond" flag and the keys will be stored
-          by both devices.
-
-        - ``'mitm'``: Sets whether MITM-protection is required for pairing.
-
-        - ``'io'``: Sets the I/O capabilities of this device.
-
-          Available options are::
-
-            _IO_CAPABILITY_DISPLAY_ONLY = const(0)
-            _IO_CAPABILITY_DISPLAY_YESNO = const(1)
-            _IO_CAPABILITY_KEYBOARD_ONLY = const(2)
-            _IO_CAPABILITY_NO_INPUT_OUTPUT = const(3)
-            _IO_CAPABILITY_KEYBOARD_DISPLAY = const(4)
-
-        - ``'le_secure'``: Sets whether "LE Secure" pairing is required. Default is
-          false (i.e. allow "Legacy Pairing").
-        """
-        ...
-    def active(self, active: Optional[Any] = None, /) -> Any:
-        """
-        Optionally changes the active state of the BLE radio, and returns the
-        current state.
-
-        The radio must be made active before using any other methods on this class.
-        """
-        ...
-    def gattc_discover_services(self, conn_handle, uuid=None, /) -> Any:
-        """
-        Query a connected server for its services.
-
-        Optionally specify a service *uuid* to query for that service only.
-
-        For each service discovered, the ``_IRQ_GATTC_SERVICE_RESULT`` event will
-        be raised, followed by ``_IRQ_GATTC_SERVICE_DONE`` on completion.
-        """
-        ...
-    def gap_disconnect(self, conn_handle, /) -> bool:
-        """
-        Disconnect the specified connection handle. This can either be a
-        central that has connected to this device (if acting as a peripheral)
-        or a peripheral that was previously connected to by this device (if acting
-        as a central).
-
-        On success, the ``_IRQ_PERIPHERAL_DISCONNECT`` or ``_IRQ_CENTRAL_DISCONNECT``
-        event will be raised.
-
-        Returns ``False`` if the connection handle wasn't connected, and ``True``
-        otherwise.
-
-        """
-        ...
-    def gattc_discover_descriptors(self, conn_handle, start_handle, end_handle, /) -> Any:
-        """
-        Query a connected server for descriptors in the specified range.
-
-        For each descriptor discovered, the ``_IRQ_GATTC_DESCRIPTOR_RESULT`` event
-        will be raised, followed by ``_IRQ_GATTC_DESCRIPTOR_DONE`` on completion.
-        """
-        ...
-    def gattc_discover_characteristics(self, conn_handle, start_handle, end_handle, uuid=None, /) -> Any:
-        """
-        Query a connected server for characteristics in the specified range.
-
-        Optionally specify a characteristic *uuid* to query for that
-        characteristic only.
-
-        You can use ``start_handle=1``, ``end_handle=0xffff`` to search for a
-        characteristic in any service.
-
-        For each characteristic discovered, the ``_IRQ_GATTC_CHARACTERISTIC_RESULT``
-        event will be raised, followed by ``_IRQ_GATTC_CHARACTERISTIC_DONE`` on completion.
-        """
-        ...
-    def gap_scan(self, duration_ms, interval_us=1280000, window_us=11250, active=False, /) -> Any:
-        """
-        Run a scan operation lasting for the specified duration (in **milli** seconds).
-
-        To scan indefinitely, set *duration_ms* to ``0``.
-
-        To stop scanning, set *duration_ms* to ``None``.
-
-        Use *interval_us* and *window_us* to optionally configure the duty cycle.
-        The scanner will run for *window_us* **micro** seconds every *interval_us*
-        **micro** seconds for a total of *duration_ms* **milli** seconds. The default
-        interval and window are 1.28 seconds and 11.25 milliseconds respectively
-        (background scanning).
-
-        For each scan result the ``_IRQ_SCAN_RESULT`` event will be raised, with event
-        data ``(addr_type, addr, adv_type, rssi, adv_data)``.
-
-        ``addr_type`` values indicate public or random addresses:
-            * 0x00 - PUBLIC
-            * 0x01 - RANDOM (either static, RPA, or NRPA, the type is encoded in the address itself)
-
-        ``adv_type`` values correspond to the Bluetooth Specification:
-
-            * 0x00 - ADV_IND - connectable and scannable undirected advertising
-            * 0x01 - ADV_DIRECT_IND - connectable directed advertising
-            * 0x02 - ADV_SCAN_IND - scannable undirected advertising
-            * 0x03 - ADV_NONCONN_IND - non-connectable undirected advertising
-            * 0x04 - SCAN_RSP - scan response
-
-        ``active`` can be set ``True`` if you want to receive scan responses in the results.
-
-        When scanning is stopped (either due to the duration finishing or when
-        explicitly stopped), the ``_IRQ_SCAN_DONE`` event will be raised.
-
-        """
-        ...
-    def __init__(self) -> None: ...
+"""
+Low-level Bluetooth radio functionality. See: https://docs.micropython.org/en/v1.20.0/library/bluetooth.html
+
+This module provides an interface to a Bluetooth controller on a board.
+Currently this supports Bluetooth Low Energy (BLE) in Central, Peripheral,
+Broadcaster, and Observer roles, as well as GATT Server and Client and L2CAP
+connection-oriented-channels. A device may operate in multiple roles
+concurrently. Pairing (and bonding) is supported on some ports.
+
+This API is intended to match the low-level Bluetooth protocol and provide
+building-blocks for higher-level abstractions such as specific device types.
+
+``Note:`` For most applications, we recommend using the higher-level
+          `aioble library <https://github.com/micropython/micropython-lib/tree/master/micropython/bluetooth/aioble>`_.
+
+``Note:`` This module is still under development and its classes, functions,
+          methods and constants are subject to change.
+"""
+from typing import Optional, Tuple, Any
+
+FLAG_NOTIFY: int
+FLAG_READ: int
+FLAG_WRITE: int
+FLAG_INDICATE: int
+FLAG_WRITE_NO_RESPONSE: int
+
+class UUID:
+    """
+    Creates a UUID instance with the specified **value**.
+
+    The **value** can be either:
+
+    - A 16-bit integer. e.g. ``0x2908``.
+    - A 128-bit UUID string. e.g. ``'6E400001-B5A3-F393-E0A9-E50E24DCCA9E'``.
+    """
+
+    def __init__(self, value, /) -> None: ...
+
+class BLE:
+    """
+    Returns the singleton BLE object.
+    """
+
+    def gattc_write(self, conn_handle, value_handle, data, mode=0, /) -> None:
+        """
+        Issue a remote write to a connected server for the specified
+        characteristic or descriptor handle.
+
+        The argument *mode* specifies the write behaviour, with the currently
+        supported values being:
+
+            * ``mode=0`` (default) is a write-without-response: the write will
+              be sent to the remote server but no confirmation will be
+              returned, and no event will be raised.
+            * ``mode=1`` is a write-with-response: the remote server is
+              requested to send a response/acknowledgement that it received the
+              data.
+
+        If a response is received from the remote server the
+        ``_IRQ_GATTC_WRITE_DONE`` event will be raised.
+        """
+        ...
+    def gatts_indicate(self, conn_handle, value_handle, data=None, /) -> None:
+        """
+        Sends a indication request to a connected client.
+
+        If *data* is ``None`` (the default), then the current local value (as set
+        with :meth:`gatts_write <BLE.gatts_write>`) will be sent.
+
+        Otherwise, if *data* is not ``None``, then that value is sent to the client
+        as part of the indication. The local value will not be modified.
+
+        On acknowledgment (or failure, e.g. timeout), the
+        ``_IRQ_GATTS_INDICATE_DONE`` event will be raised.
+
+        **Note:** The indication will be sent regardless of the subscription
+        status of the client to this characteristic.
+        """
+        ...
+    def gattc_discover_services(self, conn_handle, uuid=None, /) -> Any:
+        """
+        Query a connected server for its services.
+
+        Optionally specify a service *uuid* to query for that service only.
+
+        For each service discovered, the ``_IRQ_GATTC_SERVICE_RESULT`` event will
+        be raised, followed by ``_IRQ_GATTC_SERVICE_DONE`` on completion.
+        """
+        ...
+    def gattc_read(self, conn_handle, value_handle, /) -> None:
+        """
+        Issue a remote read to a connected server for the specified
+        characteristic or descriptor handle.
+
+        When a value is available, the ``_IRQ_GATTC_READ_RESULT`` event will be
+        raised. Additionally, the ``_IRQ_GATTC_READ_DONE`` will be raised.
+        """
+        ...
+    def gattc_exchange_mtu(self, conn_handle, /) -> Any:
+        """
+        Initiate MTU exchange with a connected server, using the preferred MTU
+        set using ``BLE.config(mtu=value)``.
+
+        The ``_IRQ_MTU_EXCHANGED`` event will be raised when MTU exchange
+        completes.
+
+        **Note:** MTU exchange is typically initiated by the central. When using
+        the BlueKitchen stack in the central role, it does not support a remote
+        peripheral initiating the MTU exchange. NimBLE works for both roles.
+
+        """
+        ...
+    def gatts_set_buffer(self, value_handle, len, append=False, /) -> None:
+        """
+        Sets the internal buffer size for a value in bytes. This will limit the
+        largest possible write that can be received. The default is 20.
+
+        Setting *append* to ``True`` will make all remote writes append to, rather
+        than replace, the current value. At most *len* bytes can be buffered in
+        this way. When you use :meth:`gatts_read <BLE.gatts_read>`, the value will
+        be cleared after reading. This feature is useful when implementing something
+        like the Nordic UART Service.
+        """
+        ...
+    def gatts_write(self, value_handle, data, send_update=False, /) -> None:
+        """
+        Writes the local value for this handle, which can be read by a client.
+
+        If *send_update* is ``True``, then any subscribed clients will be notified
+        (or indicated, depending on what they're subscribed to and which operations
+        the characteristic supports) about this write.
+        """
+        ...
+    def gatts_notify(self, conn_handle, value_handle, data=None, /) -> None:
+        """
+        Sends a notification request to a connected client.
+
+        If *data* is ``None`` (the default), then the current local value (as set
+        with :meth:`gatts_write <BLE.gatts_write>`) will be sent.
+
+        Otherwise, if *data* is not ``None``, then that value is sent to the client
+        as part of the notification. The local value will not be modified.
+
+        **Note:** The notification will be sent regardless of the subscription
+        status of the client to this characteristic.
+        """
+        ...
+    def gatts_register_services(self, services_definition, /) -> Any:
+        """
+        Configures the server with the specified services, replacing any
+        existing services.
+
+        *services_definition* is a list of **services**, where each **service** is a
+        two-element tuple containing a UUID and a list of **characteristics**.
+
+        Each **characteristic** is a two-or-three-element tuple containing a UUID, a
+        **flags** value, and optionally a list of *descriptors*.
+
+        Each **descriptor** is a two-element tuple containing a UUID and a **flags**
+        value.
+
+        The **flags** are a bitwise-OR combination of the flags defined below. These
+        set both the behaviour of the characteristic (or descriptor) as well as the
+        security and privacy requirements.
+
+        The return value is a list (one element per service) of tuples (each element
+        is a value handle). Characteristics and descriptor handles are flattened
+        into the same tuple, in the order that they are defined.
+
+        The following example registers two services (Heart Rate, and Nordic UART)::
+
+            HR_UUID = bluetooth.UUID(0x180D)
+            HR_CHAR = (bluetooth.UUID(0x2A37), bluetooth.FLAG_READ | bluetooth.FLAG_NOTIFY,)
+            HR_SERVICE = (HR_UUID, (HR_CHAR,),)
+            UART_UUID = bluetooth.UUID('6E400001-B5A3-F393-E0A9-E50E24DCCA9E')
+            UART_TX = (bluetooth.UUID('6E400003-B5A3-F393-E0A9-E50E24DCCA9E'), bluetooth.FLAG_READ | bluetooth.FLAG_NOTIFY,)
+            UART_RX = (bluetooth.UUID('6E400002-B5A3-F393-E0A9-E50E24DCCA9E'), bluetooth.FLAG_WRITE,)
+            UART_SERVICE = (UART_UUID, (UART_TX, UART_RX,),)
+            SERVICES = (HR_SERVICE, UART_SERVICE,)
+            ( (hr,), (tx, rx,), ) = bt.gatts_register_services(SERVICES)
+
+        The three value handles (``hr``, ``tx``, ``rx``) can be used with
+        :meth:`gatts_read <BLE.gatts_read>`, :meth:`gatts_write <BLE.gatts_write>`, :meth:`gatts_notify <BLE.gatts_notify>`, and
+        :meth:`gatts_indicate <BLE.gatts_indicate>`.
+
+        **Note:** Advertising must be stopped before registering services.
+
+        Available flags for characteristics and descriptors are::
+
+            from micropython import const
+            _FLAG_BROADCAST = const(0x0001)
+            _FLAG_READ = const(0x0002)
+            _FLAG_WRITE_NO_RESPONSE = const(0x0004)
+            _FLAG_WRITE = const(0x0008)
+            _FLAG_NOTIFY = const(0x0010)
+            _FLAG_INDICATE = const(0x0020)
+            _FLAG_AUTHENTICATED_SIGNED_WRITE = const(0x0040)
+
+            _FLAG_AUX_WRITE = const(0x0100)
+            _FLAG_READ_ENCRYPTED = const(0x0200)
+            _FLAG_READ_AUTHENTICATED = const(0x0400)
+            _FLAG_READ_AUTHORIZED = const(0x0800)
+            _FLAG_WRITE_ENCRYPTED = const(0x1000)
+            _FLAG_WRITE_AUTHENTICATED = const(0x2000)
+            _FLAG_WRITE_AUTHORIZED = const(0x4000)
+
+        As for the IRQs above, any required constants should be added to your Python code.
+        """
+        ...
+    def gatts_read(self, value_handle, /) -> Any:
+        """
+        Reads the local value for this handle (which has either been written by
+        :meth:`gatts_write <BLE.gatts_write>` or by a remote client).
+        """
+        ...
+    def irq(self, handler, /) -> int:
+        """
+            Registers a callback for events from the BLE stack. The *handler* takes two
+            arguments, ``event`` (which will be one of the codes below) and ``data``
+            (which is an event-specific tuple of values).
+
+            **Note:** As an optimisation to prevent unnecessary allocations, the ``addr``,
+            ``adv_data``, ``char_data``, ``notify_data``, and ``uuid`` entries in the
+            tuples are read-only memoryview instances pointing to :mod:`bluetooth`'s internal
+            ringbuffer, and are only valid during the invocation of the IRQ handler
+            function.  If your program needs to save one of these values to access after
+            the IRQ handler has returned (e.g. by saving it in a class instance or global
+            variable), then it needs to take a copy of the data, either by using ``bytes()``
+            or ``bluetooth.UUID()``, like this::
+
+                connected_addr = bytes(addr)  # equivalently: adv_data, char_data, or notify_data
+                matched_uuid = bluetooth.UUID(uuid)
+
+            For example, the IRQ handler for a scan result might inspect the ``adv_data``
+            to decide if it's the correct device, and only then copy the address data to be
+            used elsewhere in the program.  And to print data from within the IRQ handler,
+            ``print(bytes(addr))`` will be needed.
+
+            An event handler showing all possible events::
+
+                def bt_irq(event, data):
+                    if event == _IRQ_CENTRAL_CONNECT:
+                        # A central has connected to this peripheral.
+                        conn_handle, addr_type, addr = data
+                    elif event == _IRQ_CENTRAL_DISCONNECT:
+                        # A central has disconnected from this peripheral.
+                        conn_handle, addr_type, addr = data
+                    elif event == _IRQ_GATTS_WRITE:
+                        # A client has written to this characteristic or descriptor.
+                        conn_handle, attr_handle = data
+                    elif event == _IRQ_GATTS_READ_REQUEST:
+                        # A client has issued a read. Note: this is only supported on STM32.
+                        # Return a non-zero integer to deny the read (see below), or zero (or None)
+                        # to accept the read.
+                        conn_handle, attr_handle = data
+                    elif event == _IRQ_SCAN_RESULT:
+                        # A single scan result.
+                        addr_type, addr, adv_type, rssi, adv_data = data
+                    elif event == _IRQ_SCAN_DONE:
+                        # Scan duration finished or manually stopped.
+                        pass
+                    elif event == _IRQ_PERIPHERAL_CONNECT:
+                        # A successful gap_connect().
+                        conn_handle, addr_type, addr = data
+                    elif event == _IRQ_PERIPHERAL_DISCONNECT:
+                        # Connected peripheral has disconnected.
+                        conn_handle, addr_type, addr = data
+                    elif event == _IRQ_GATTC_SERVICE_RESULT:
+                        # Called for each service found by gattc_discover_services().
+                        conn_handle, start_handle, end_handle, uuid = data
+                    elif event == _IRQ_GATTC_SERVICE_DONE:
+                        # Called once service discovery is complete.
+                        # Note: Status will be zero on success, implementation-specific value otherwise.
+                        conn_handle, status = data
+                    elif event == _IRQ_GATTC_CHARACTERISTIC_RESULT:
+                        # Called for each characteristic found by gattc_discover_services().
+                        conn_handle, end_handle, value_handle, properties, uuid = data
+                    elif event == _IRQ_GATTC_CHARACTERISTIC_DONE:
+                        # Called once service discovery is complete.
+                        # Note: Status will be zero on success, implementation-specific value otherwise.
+                        conn_handle, status = data
+                    elif event == _IRQ_GATTC_DESCRIPTOR_RESULT:
+                        # Called for each descriptor found by gattc_discover_descriptors().
+                        conn_handle, dsc_handle, uuid = data
+                    elif event == _IRQ_GATTC_DESCRIPTOR_DONE:
+                        # Called once service discovery is complete.
+                        # Note: Status will be zero on success, implementation-specific value otherwise.
+                        conn_handle, status = data
+                    elif event == _IRQ_GATTC_READ_RESULT:
+                        # A gattc_read() has completed.
+                        conn_handle, value_handle, char_data = data
+                    elif event == _IRQ_GATTC_READ_DONE:
+                        # A gattc_read() has completed.
+                        # Note: Status will be zero on success, implementation-specific value otherwise.
+                        conn_handle, value_handle, status = data
+                    elif event == _IRQ_GATTC_WRITE_DONE:
+                        # A gattc_write() has completed.
+                        # Note: Status will be zero on success, implementation-specific value otherwise.
+                        conn_handle, value_handle, status = data
+                    elif event == _IRQ_GATTC_NOTIFY:
+                        # A server has sent a notify request.
+                        conn_handle, value_handle, notify_data = data
+                    elif event == _IRQ_GATTC_INDICATE:
+                        # A server has sent an indicate request.
+                        conn_handle, value_handle, notify_data = data
+                    elif event == _IRQ_GATTS_INDICATE_DONE:
+                        # A client has acknowledged the indication.
+                        # Note: Status will be zero on successful acknowledgment, implementation-specific value otherwise.
+                        conn_handle, value_handle, status = data
+                    elif event == _IRQ_MTU_EXCHANGED:
+                        # ATT MTU exchange complete (either initiated by us or the remote device).
+                        conn_handle, mtu = data
+                    elif event == _IRQ_L2CAP_ACCEPT:
+                        # A new channel has been accepted.
+                        # Return a non-zero integer to reject the connection, or zero (or None) to accept.
+                        conn_handle, cid, psm, our_mtu, peer_mtu = data
+                    elif event == _IRQ_L2CAP_CONNECT:
+                        # A new channel is now connected (either as a result of connecting or accepting).
+                        conn_handle, cid, psm, our_mtu, peer_mtu = data
+                    elif event == _IRQ_L2CAP_DISCONNECT:
+                        # Existing channel has disconnected (status is zero), or a connection attempt failed (non-zero status).
+                        conn_handle, cid, psm, status = data
+                    elif event == _IRQ_L2CAP_RECV:
+                        # New data is available on the channel. Use l2cap_recvinto to read.
+                        conn_handle, cid = data
+                    elif event == _IRQ_L2CAP_SEND_READY:
+                        # A previous l2cap_send that returned False has now completed and the channel is ready to send again.
+                        # If status is non-zero, then the transmit buffer overflowed and the application should re-send the data.
+                        conn_handle, cid, status = data
+                    elif event == _IRQ_CONNECTION_UPDATE:
+                        # The remote device has updated connection parameters.
+                        conn_handle, conn_interval, conn_latency, supervision_timeout, status = data
+                    elif event == _IRQ_ENCRYPTION_UPDATE:
+                        # The encryption state has changed (likely as a result of pairing or bonding).
+                        conn_handle, encrypted, authenticated, bonded, key_size = data
+                    elif event == _IRQ_GET_SECRET:
+                        # Return a stored secret.
+                        # If key is None, return the index'th value of this sec_type.
+                        # Otherwise return the corresponding value for this sec_type and key.
+                        sec_type, index, key = data
+                        return value
+                    elif event == _IRQ_SET_SECRET:
+                        # Save a secret to the store for this sec_type and key.
+                        sec_type, key, value = data
+                        return True
+                    elif event == _IRQ_PASSKEY_ACTION:
+                        # Respond to a passkey request during pairing.
+                        # See gap_passkey() for details.
+                        # action will be an action that is compatible with the configured "io" config.
+                        # passkey will be non-zero if action is "numeric comparison".
+                        conn_handle, action, passkey = data
+
+
+        The event codes are::
+
+            from micropython import const
+            _IRQ_CENTRAL_CONNECT = const(1)
+            _IRQ_CENTRAL_DISCONNECT = const(2)
+            _IRQ_GATTS_WRITE = const(3)
+            _IRQ_GATTS_READ_REQUEST = const(4)
+            _IRQ_SCAN_RESULT = const(5)
+            _IRQ_SCAN_DONE = const(6)
+            _IRQ_PERIPHERAL_CONNECT = const(7)
+            _IRQ_PERIPHERAL_DISCONNECT = const(8)
+            _IRQ_GATTC_SERVICE_RESULT = const(9)
+            _IRQ_GATTC_SERVICE_DONE = const(10)
+            _IRQ_GATTC_CHARACTERISTIC_RESULT = const(11)
+            _IRQ_GATTC_CHARACTERISTIC_DONE = const(12)
+            _IRQ_GATTC_DESCRIPTOR_RESULT = const(13)
+            _IRQ_GATTC_DESCRIPTOR_DONE = const(14)
+            _IRQ_GATTC_READ_RESULT = const(15)
+            _IRQ_GATTC_READ_DONE = const(16)
+            _IRQ_GATTC_WRITE_DONE = const(17)
+            _IRQ_GATTC_NOTIFY = const(18)
+            _IRQ_GATTC_INDICATE = const(19)
+            _IRQ_GATTS_INDICATE_DONE = const(20)
+            _IRQ_MTU_EXCHANGED = const(21)
+            _IRQ_L2CAP_ACCEPT = const(22)
+            _IRQ_L2CAP_CONNECT = const(23)
+            _IRQ_L2CAP_DISCONNECT = const(24)
+            _IRQ_L2CAP_RECV = const(25)
+            _IRQ_L2CAP_SEND_READY = const(26)
+            _IRQ_CONNECTION_UPDATE = const(27)
+            _IRQ_ENCRYPTION_UPDATE = const(28)
+            _IRQ_GET_SECRET = const(29)
+            _IRQ_SET_SECRET = const(30)
+
+        For the ``_IRQ_GATTS_READ_REQUEST`` event, the available return codes are::
+
+            _GATTS_NO_ERROR = const(0x00)
+            _GATTS_ERROR_READ_NOT_PERMITTED = const(0x02)
+            _GATTS_ERROR_WRITE_NOT_PERMITTED = const(0x03)
+            _GATTS_ERROR_INSUFFICIENT_AUTHENTICATION = const(0x05)
+            _GATTS_ERROR_INSUFFICIENT_AUTHORIZATION = const(0x08)
+            _GATTS_ERROR_INSUFFICIENT_ENCRYPTION = const(0x0f)
+
+        For the ``_IRQ_PASSKEY_ACTION`` event, the available actions are::
+
+            _PASSKEY_ACTION_NONE = const(0)
+            _PASSKEY_ACTION_INPUT = const(2)
+            _PASSKEY_ACTION_DISPLAY = const(3)
+            _PASSKEY_ACTION_NUMERIC_COMPARISON = const(4)
+
+        In order to save space in the firmware, these constants are not included on the
+        :mod:`bluetooth` module. Add the ones that you need from the list above to your
+        program.
+
+        """
+        ...
+    def gap_advertise(self, interval_us, adv_data=None, *, resp_data=None, connectable=True) -> Any:
+        """
+        Starts advertising at the specified interval (in **micro** seconds). This
+        interval will be rounded down to the nearest 625us. To stop advertising, set
+        *interval_us* to ``None``.
+
+        *adv_data* and *resp_data* can be any type that implements the buffer
+        protocol (e.g. ``bytes``, ``bytearray``, ``str``). *adv_data* is included
+        in all broadcasts, and *resp_data* is send in reply to an active scan.
+
+        **Note:** if *adv_data* (or *resp_data*) is ``None``, then the data passed
+        to the previous call to ``gap_advertise`` will be re-used. This allows a
+        broadcaster to resume advertising with just ``gap_advertise(interval_us)``.
+        To clear the advertising payload pass an empty ``bytes``, i.e. ``b''``.
+
+        """
+        ...
+    def gap_connect(self, addr_type, addr, scan_duration_ms=2000, min_conn_interval_us=None, max_conn_interval_us=None, /) -> None:
+        """
+        Connect to a peripheral.
+
+        See :meth:`gap_scan <BLE.gap_scan>` for details about address types.
+
+        To cancel an outstanding connection attempt early, call
+        ``gap_connect(None)``.
+
+        On success, the ``_IRQ_PERIPHERAL_CONNECT`` event will be raised. If
+        cancelling a connection attempt, the ``_IRQ_PERIPHERAL_DISCONNECT`` event
+        will be raised.
+
+        The device will wait up to *scan_duration_ms* to receive an advertising
+        payload from the device.
+
+        The connection interval can be configured in **micro** seconds using either
+        or both of *min_conn_interval_us* and *max_conn_interval_us*. Otherwise a
+        default interval will be chosen, typically between 30000 and 50000
+        microseconds. A shorter interval will increase throughput, at the expense
+        of power usage.
+
+        """
+        ...
+    def gattc_discover_descriptors(self, conn_handle, start_handle, end_handle, /) -> Any:
+        """
+        Query a connected server for descriptors in the specified range.
+
+        For each descriptor discovered, the ``_IRQ_GATTC_DESCRIPTOR_RESULT`` event
+        will be raised, followed by ``_IRQ_GATTC_DESCRIPTOR_DONE`` on completion.
+        """
+        ...
+    def config(self, param, /) -> Tuple:
+        """
+        Get or set configuration values of the BLE interface.  To get a value the
+        parameter name should be quoted as a string, and just one parameter is
+        queried at a time.  To set values use the keyword syntax, and one ore more
+        parameter can be set at a time.
+
+        Currently supported values are:
+
+        - ``'mac'``: The current address in use, depending on the current address mode.
+          This returns a tuple of ``(addr_type, addr)``.
+
+          See :meth:`gatts_write <BLE.gatts_write>` for details about address type.
+
+          This may only be queried while the interface is currently active.
+
+        - ``'addr_mode'``: Sets the address mode. Values can be:
+
+            * 0x00 - PUBLIC - Use the controller's public address.
+            * 0x01 - RANDOM - Use a generated static address.
+            * 0x02 - RPA - Use resolvable private addresses.
+            * 0x03 - NRPA - Use non-resolvable private addresses.
+
+          By default the interface mode will use a PUBLIC address if available, otherwise
+          it will use a RANDOM address.
+
+        - ``'gap_name'``: Get/set the GAP device name used by service 0x1800,
+          characteristic 0x2a00.  This can be set at any time and changed multiple
+          times.
+
+        - ``'rxbuf'``: Get/set the size in bytes of the internal buffer used to store
+          incoming events.  This buffer is global to the entire BLE driver and so
+          handles incoming data for all events, including all characteristics.
+          Increasing this allows better handling of bursty incoming data (for
+          example scan results) and the ability to receive larger characteristic values.
+
+        - ``'mtu'``: Get/set the MTU that will be used during a ATT MTU exchange. The
+          resulting MTU will be the minimum of this and the remote device's MTU.
+          ATT MTU exchange will not happen automatically (unless the remote device initiates
+          it), and must be manually initiated with
+          :meth:`gattc_exchange_mtu<BLE.gattc_exchange_mtu>`.
+          Use the ``_IRQ_MTU_EXCHANGED`` event to discover the MTU for a given connection.
+
+        - ``'bond'``: Sets whether bonding will be enabled during pairing. When
+          enabled, pairing requests will set the "bond" flag and the keys will be stored
+          by both devices.
+
+        - ``'mitm'``: Sets whether MITM-protection is required for pairing.
+
+        - ``'io'``: Sets the I/O capabilities of this device.
+
+          Available options are::
+
+            _IO_CAPABILITY_DISPLAY_ONLY = const(0)
+            _IO_CAPABILITY_DISPLAY_YESNO = const(1)
+            _IO_CAPABILITY_KEYBOARD_ONLY = const(2)
+            _IO_CAPABILITY_NO_INPUT_OUTPUT = const(3)
+            _IO_CAPABILITY_KEYBOARD_DISPLAY = const(4)
+
+        - ``'le_secure'``: Sets whether "LE Secure" pairing is required. Default is
+          false (i.e. allow "Legacy Pairing").
+        """
+        ...
+    def active(self, active: Optional[Any] = None, /) -> Any:
+        """
+        Optionally changes the active state of the BLE radio, and returns the
+        current state.
+
+        The radio must be made active before using any other methods on this class.
+        """
+        ...
+    def gap_scan(self, duration_ms, interval_us=1280000, window_us=11250, active=False, /) -> Any:
+        """
+        Run a scan operation lasting for the specified duration (in **milli** seconds).
+
+        To scan indefinitely, set *duration_ms* to ``0``.
+
+        To stop scanning, set *duration_ms* to ``None``.
+
+        Use *interval_us* and *window_us* to optionally configure the duty cycle.
+        The scanner will run for *window_us* **micro** seconds every *interval_us*
+        **micro** seconds for a total of *duration_ms* **milli** seconds. The default
+        interval and window are 1.28 seconds and 11.25 milliseconds respectively
+        (background scanning).
+
+        For each scan result the ``_IRQ_SCAN_RESULT`` event will be raised, with event
+        data ``(addr_type, addr, adv_type, rssi, adv_data)``.
+
+        ``addr_type`` values indicate public or random addresses:
+            * 0x00 - PUBLIC
+            * 0x01 - RANDOM (either static, RPA, or NRPA, the type is encoded in the address itself)
+
+        ``adv_type`` values correspond to the Bluetooth Specification:
+
+            * 0x00 - ADV_IND - connectable and scannable undirected advertising
+            * 0x01 - ADV_DIRECT_IND - connectable directed advertising
+            * 0x02 - ADV_SCAN_IND - scannable undirected advertising
+            * 0x03 - ADV_NONCONN_IND - non-connectable undirected advertising
+            * 0x04 - SCAN_RSP - scan response
+
+        ``active`` can be set ``True`` if you want to receive scan responses in the results.
+
+        When scanning is stopped (either due to the duration finishing or when
+        explicitly stopped), the ``_IRQ_SCAN_DONE`` event will be raised.
+
+        """
+        ...
+    def gattc_discover_characteristics(self, conn_handle, start_handle, end_handle, uuid=None, /) -> Any:
+        """
+        Query a connected server for characteristics in the specified range.
+
+        Optionally specify a characteristic *uuid* to query for that
+        characteristic only.
+
+        You can use ``start_handle=1``, ``end_handle=0xffff`` to search for a
+        characteristic in any service.
+
+        For each characteristic discovered, the ``_IRQ_GATTC_CHARACTERISTIC_RESULT``
+        event will be raised, followed by ``_IRQ_GATTC_CHARACTERISTIC_DONE`` on completion.
+        """
+        ...
+    def gap_disconnect(self, conn_handle, /) -> bool:
+        """
+        Disconnect the specified connection handle. This can either be a
+        central that has connected to this device (if acting as a peripheral)
+        or a peripheral that was previously connected to by this device (if acting
+        as a central).
+
+        On success, the ``_IRQ_PERIPHERAL_DISCONNECT`` or ``_IRQ_CENTRAL_DISCONNECT``
+        event will be raised.
+
+        Returns ``False`` if the connection handle wasn't connected, and ``True``
+        otherwise.
+
+        """
+        ...
+    def gap_passkey(self, conn_handle, action, passkey, /) -> Any:
+        """
+        Respond to a ``_IRQ_PASSKEY_ACTION`` event for the specified *conn_handle*
+        and *action*.
+
+        The *passkey* is a numeric value and will depend on on the
+        *action* (which will depend on what I/O capability has been set):
+
+            * When the *action* is ``_PASSKEY_ACTION_INPUT``, then the application should
+              prompt the user to enter the passkey that is shown on the remote device.
+            * When the *action* is ``_PASSKEY_ACTION_DISPLAY``, then the application should
+              generate a random 6-digit passkey and show it to the user.
+            * When the *action* is ``_PASSKEY_ACTION_NUMERIC_COMPARISON``, then the application
+              should show the passkey that was provided in the ``_IRQ_PASSKEY_ACTION`` event
+              and then respond with either ``0`` (cancel pairing), or ``1`` (accept pairing).
+
+        """
+        ...
+    def gap_pair(self, conn_handle, /) -> Any:
+        """
+        Initiate pairing with the remote device.
+
+        Before calling this, ensure that the ``io``, ``mitm``, ``le_secure``, and
+        ``bond`` configuration options are set (via :meth:`config<BLE.config>`).
+
+        On successful pairing, the ``_IRQ_ENCRYPTION_UPDATE`` event will be raised.
+        """
+        ...
+    def __init__(self) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/ucollections.pyi` & `micropython_esp32_stubs-1.20.0.post1/collections.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-"""
-collection and container types. See: https://docs.micropython.org/en/v1.19.1/library/collections.html
-
-|see_cpython_module| :mod:`python:collections` https://docs.python.org/3/library/collections.html .
-
-This module implements advanced collection and container types to
-hold/accumulate various objects.
-"""
-from typing import Optional, Any
-from queue import Queue
-
-def namedtuple(name, fields) -> Any:
-    """
-    This is factory function to create a new namedtuple type with a specific
-    name and set of fields. A namedtuple is a subclass of tuple which allows
-    to access its fields not just by numeric index, but also with an attribute
-    access syntax using symbolic field names. Fields is a sequence of strings
-    specifying field names. For compatibility with CPython it can also be a
-    a string with space-separated field named (but this is less efficient).
-    Example of use::
-
-        from collections import namedtuple
-
-        MyTuple = namedtuple("MyTuple", ("id", "name"))
-        t1 = MyTuple(1, "foo")
-        t2 = MyTuple(2, "bar")
-        print(t1.name)
-        assert t2.name == t2[1]
-    """
-    ...
-
-class OrderedDict:
-    """
-    ``dict`` type subclass which remembers and preserves the order of keys
-    added. When ordered dict is iterated over, keys/items are returned in
-    the order they were added::
-
-        from collections import OrderedDict
-
-        # To make benefit of ordered keys, OrderedDict should be initialized
-        # from sequence of (key, value) pairs.
-        d = OrderedDict([("z", 1), ("a", 2)])
-        # More items can be added as usual
-        d["w"] = 5
-        d["b"] = 3
-        for k, v in d.items():
-            print(k, v)
-
-    Output::
-
-        z 1
-        a 2
-        w 5
-        b 3
-    """
-
-    def popitem(self, *args, **kwargs) -> Any: ...
-    def pop(self, *args, **kwargs) -> Any: ...
-    def values(self, *args, **kwargs) -> Any: ...
-    def setdefault(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def copy(self, *args, **kwargs) -> Any: ...
-    def clear(self, *args, **kwargs) -> Any: ...
-    def keys(self, *args, **kwargs) -> Any: ...
-    def get(self, *args, **kwargs) -> Any: ...
-    def items(self, *args, **kwargs) -> Any: ...
-    @classmethod
-    def fromkeys(cls, *args, **kwargs) -> Any: ...
-    def __init__(self, *args, **kwargs) -> None: ...
-
-class deque:
-    """
-    Deques (double-ended queues) are a list-like container that support O(1)
-    appends and pops from either side of the deque.  New deques are created
-    using the following arguments:
-
-        - *iterable* must be the empty tuple, and the new deque is created empty.
-
-        - *maxlen* must be specified and the deque will be bounded to this
-          maximum length.  Once the deque is full, any new items added will
-          discard items from the opposite end.
-
-        - The optional *flags* can be 1 to check for overflow when adding items.
-
-    As well as supporting `bool` and `len`, deque objects have the following
-    methods:
-    """
-
-    def popleft(self) -> Any:
-        """
-        Remove and return an item from the left side of the deque.
-        Raises IndexError if no items are present.
-        """
-        ...
-    def append(self, x) -> Any:
-        """
-        Add *x* to the right side of the deque.
-        Raises IndexError if overflow checking is enabled and there is no more room left.
-        """
-        ...
-    def __init__(self, iterable, maxlen, flags: Optional[Any] = None) -> None: ...
+"""
+collection and container types. See: https://docs.micropython.org/en/v1.20.0/library/collections.html
+
+|see_cpython_module| :mod:`python:collections` https://docs.python.org/3/library/collections.html .
+
+This module implements advanced collection and container types to
+hold/accumulate various objects.
+"""
+from typing import Optional, Any
+from queue import Queue
+
+def namedtuple(name, fields) -> Any:
+    """
+    This is factory function to create a new namedtuple type with a specific
+    name and set of fields. A namedtuple is a subclass of tuple which allows
+    to access its fields not just by numeric index, but also with an attribute
+    access syntax using symbolic field names. Fields is a sequence of strings
+    specifying field names. For compatibility with CPython it can also be a
+    a string with space-separated field named (but this is less efficient).
+    Example of use::
+
+        from collections import namedtuple
+
+        MyTuple = namedtuple("MyTuple", ("id", "name"))
+        t1 = MyTuple(1, "foo")
+        t2 = MyTuple(2, "bar")
+        print(t1.name)
+        assert t2.name == t2[1]
+    """
+    ...
+
+class OrderedDict(dict):
+    """
+    ``dict`` type subclass which remembers and preserves the order of keys
+    added. When ordered dict is iterated over, keys/items are returned in
+    the order they were added::
+
+        from collections import OrderedDict
+
+        # To make benefit of ordered keys, OrderedDict should be initialized
+        # from sequence of (key, value) pairs.
+        d = OrderedDict([("z", 1), ("a", 2)])
+        # More items can be added as usual
+        d["w"] = 5
+        d["b"] = 3
+        for k, v in d.items():
+            print(k, v)
+
+    Output::
+
+        z 1
+        a 2
+        w 5
+        b 3
+    """
+
+    def popitem(self, *args, **kwargs) -> Any: ...
+    def pop(self, *args, **kwargs) -> Any: ...
+    def values(self, *args, **kwargs) -> Any: ...
+    def setdefault(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def copy(self, *args, **kwargs) -> Any: ...
+    def clear(self, *args, **kwargs) -> Any: ...
+    def keys(self, *args, **kwargs) -> Any: ...
+    def get(self, *args, **kwargs) -> Any: ...
+    def items(self, *args, **kwargs) -> Any: ...
+    @classmethod
+    def fromkeys(cls, *args, **kwargs) -> Any: ...
+    def __init__(self, *args, **kwargs) -> None: ...
+
+class deque(Queue):
+    """
+    Deques (double-ended queues) are a list-like container that support O(1)
+    appends and pops from either side of the deque.  New deques are created
+    using the following arguments:
+
+        - *iterable* must be the empty tuple, and the new deque is created empty.
+
+        - *maxlen* must be specified and the deque will be bounded to this
+          maximum length.  Once the deque is full, any new items added will
+          discard items from the opposite end.
+
+        - The optional *flags* can be 1 to check for overflow when adding items.
+
+    As well as supporting `bool` and `len`, deque objects have the following
+    methods:
+    """
+
+    def popleft(self) -> Any:
+        """
+        Remove and return an item from the left side of the deque.
+        Raises IndexError if no items are present.
+        """
+        ...
+    def append(self, x) -> Any:
+        """
+        Add *x* to the right side of the deque.
+        Raises IndexError if overflow checking is enabled and there is no more room left.
+        """
+        ...
+    def __init__(self, iterable, maxlen, flags: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/ucryptolib.pyi` & `micropython_esp32_stubs-1.20.0.post1/cryptolib.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""
-cryptographic ciphers. See: https://docs.micropython.org/en/v1.19.1/library/cryptolib.html
-"""
-from typing import Optional, Any
-
-class aes:
-    def encrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
-        """
-        Encrypt *in_buf*. If no *out_buf* is given result is returned as a
-        newly allocated `bytes` object. Otherwise, result is written into
-        mutable buffer *out_buf*. *in_buf* and *out_buf* can also refer
-        to the same mutable buffer, in which case data is encrypted in-place.
-        """
-        ...
-    def decrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
-        """
-        Like `encrypt()`, but for decryption.
-        """
-        ...
-    def __init__(self, key, mode, IV: Optional[Any] = None) -> None:
-        """
-        Initialize cipher object, suitable for encryption/decryption. Note:
-        after initialization, cipher object can be use only either for
-        encryption or decryption. Running decrypt() operation after encrypt()
-        or vice versa is not supported.
-
-        Parameters are:
-
-            * *key* is an encryption/decryption key (bytes-like).
-            * *mode* is:
-
-                * ``1`` (or ``cryptolib.MODE_ECB`` if it exists) for Electronic Code Book (ECB).
-                * ``2`` (or ``cryptolib.MODE_CBC`` if it exists) for Cipher Block Chaining (CBC).
-                * ``6`` (or ``cryptolib.MODE_CTR`` if it exists) for Counter mode (CTR).
-
-            * *IV* is an initialization vector for CBC mode.
-            * For Counter mode, *IV* is the initial value for the counter.
-        """
-        ...
+"""
+cryptographic ciphers. See: https://docs.micropython.org/en/v1.20.0/library/cryptolib.html
+"""
+from typing import Optional, Any
+
+class aes:
+    def encrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
+        """
+        Encrypt *in_buf*. If no *out_buf* is given result is returned as a
+        newly allocated `bytes` object. Otherwise, result is written into
+        mutable buffer *out_buf*. *in_buf* and *out_buf* can also refer
+        to the same mutable buffer, in which case data is encrypted in-place.
+        """
+        ...
+    def decrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
+        """
+        Like `encrypt()`, but for decryption.
+        """
+        ...
+    def __init__(self, key, mode, IV: Optional[Any] = None) -> None:
+        """
+        Initialize cipher object, suitable for encryption/decryption. Note:
+        after initialization, cipher object can be use only either for
+        encryption or decryption. Running decrypt() operation after encrypt()
+        or vice versa is not supported.
+
+        Parameters are:
+
+            * *key* is an encryption/decryption key (bytes-like).
+            * *mode* is:
+
+                * ``1`` (or ``cryptolib.MODE_ECB`` if it exists) for Electronic Code Book (ECB).
+                * ``2`` (or ``cryptolib.MODE_CBC`` if it exists) for Cipher Block Chaining (CBC).
+                * ``6`` (or ``cryptolib.MODE_CTR`` if it exists) for Counter mode (CTR).
+
+            * *IV* is an initialization vector for CBC mode.
+            * For Counter mode, *IV* is the initial value for the counter.
+        """
+        ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/uctypes.pyi` & `micropython_esp32_stubs-1.20.0.post1/uctypes.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""
-access binary data in a structured way. See: https://docs.micropython.org/en/v1.19.1/library/uctypes.html
-
-This module implements "foreign data interface" for MicroPython. The idea
-behind it is similar to CPython's ``ctypes`` modules, but the actual API is
-different, streamlined and optimized for small size. The basic idea of the
-module is to define data structure layout with about the same power as the
-C language allows, and then access it using familiar dot-syntax to reference
-sub-fields.
-"""
-from typing import Any
-
-VOID: int
-NATIVE: int
-PTR: int
-SHORT: int
-LONGLONG: int
-INT8: int
-LITTLE_ENDIAN: int
-LONG: int
-UINT: int
-ULONG: int
-ULONGLONG: int
-USHORT: int
-UINT8: int
-UINT16: int
-UINT32: int
-UINT64: int
-INT64: int
-BFUINT16: int
-BFUINT32: int
-BFUINT8: int
-BFINT8: int
-ARRAY: int
-BFINT16: int
-BFINT32: int
-BF_LEN: int
-INT: int
-INT16: int
-INT32: int
-FLOAT64: int
-BF_POS: int
-BIG_ENDIAN: int
-FLOAT32: int
-
-def sizeof(struct, layout_type=NATIVE, /) -> int:
-    """
-    Return size of data structure in bytes. The *struct* argument can be
-    either a structure class or a specific instantiated structure object
-    (or its aggregate field).
-    """
-    ...
-
-def bytes_at(addr, size) -> bytes:
-    """
-    Capture memory at the given address and size as bytes object. As bytes
-    object is immutable, memory is actually duplicated and copied into
-    bytes object, so if memory contents change later, created object
-    retains original value.
-    """
-    ...
-
-def bytearray_at(addr, size) -> bytearray:
-    """
-    Capture memory at the given address and size as bytearray object.
-    Unlike bytes_at() function above, memory is captured by reference,
-    so it can be both written too, and you will access current value
-    at the given memory address.
-    """
-    ...
-
-def addressof(obj) -> int:
-    """
-    Return address of an object. Argument should be bytes, bytearray or
-    other object supporting buffer protocol (and address of this buffer
-    is what actually returned).
-    """
-    ...
-
-class struct:
-    """
-    Instantiate a "foreign data structure" object based on structure address in
-    memory, descriptor (encoded as a dictionary), and layout type (see below).
-    """
-
-    def __init__(self, addr, descriptor, layout_type=NATIVE, /) -> None: ...
+"""
+access binary data in a structured way. See: https://docs.micropython.org/en/v1.20.0/library/uctypes.html
+
+This module implements "foreign data interface" for MicroPython. The idea
+behind it is similar to CPython's ``ctypes`` modules, but the actual API is
+different, streamlined and optimized for small size. The basic idea of the
+module is to define data structure layout with about the same power as the
+C language allows, and then access it using familiar dot-syntax to reference
+sub-fields.
+"""
+from typing import Any
+
+VOID: int
+NATIVE: int
+PTR: int
+SHORT: int
+LONGLONG: int
+INT8: int
+LITTLE_ENDIAN: int
+LONG: int
+UINT: int
+ULONG: int
+ULONGLONG: int
+USHORT: int
+UINT8: int
+UINT16: int
+UINT32: int
+UINT64: int
+INT64: int
+BFUINT16: int
+BFUINT32: int
+BFUINT8: int
+BFINT8: int
+ARRAY: int
+BFINT16: int
+BFINT32: int
+BF_LEN: int
+INT: int
+INT16: int
+INT32: int
+FLOAT64: int
+BF_POS: int
+BIG_ENDIAN: int
+FLOAT32: int
+
+def sizeof(struct, layout_type=NATIVE, /) -> int:
+    """
+    Return size of data structure in bytes. The *struct* argument can be
+    either a structure class or a specific instantiated structure object
+    (or its aggregate field).
+    """
+    ...
+
+def bytes_at(addr, size) -> bytes:
+    """
+    Capture memory at the given address and size as bytes object. As bytes
+    object is immutable, memory is actually duplicated and copied into
+    bytes object, so if memory contents change later, created object
+    retains original value.
+    """
+    ...
+
+def bytearray_at(addr, size) -> bytearray:
+    """
+    Capture memory at the given address and size as bytearray object.
+    Unlike bytes_at() function above, memory is captured by reference,
+    so it can be both written too, and you will access current value
+    at the given memory address.
+    """
+    ...
+
+def addressof(obj) -> int:
+    """
+    Return address of an object. Argument should be bytes, bytearray or
+    other object supporting buffer protocol (and address of this buffer
+    is what actually returned).
+    """
+    ...
+
+class struct:
+    """
+    Instantiate a "foreign data structure" object based on structure address in
+    memory, descriptor (encoded as a dictionary), and layout type (see below).
+    """
+
+    def __init__(self, addr, descriptor, layout_type=NATIVE, /) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/uhashlib.pyi` & `micropython_esp32_stubs-1.20.0.post1/uhashlib.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-hashing algorithms. See: https://docs.micropython.org/en/v1.19.1/library/hashlib.html
-
-|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
-
-This module implements binary data hashing algorithms. The exact inventory
-of available algorithms depends on a board. Among the algorithms which may
-be implemented:
-
-* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
-  It is suitable for cryptographically-secure purposes. Included in the
-  MicroPython core and any board is recommended to provide this, unless
-  it has particular code size constraints.
-
-* SHA1 - A previous generation algorithm. Not recommended for new usages,
-  but SHA1 is a part of number of Internet standards and existing
-  applications, so boards targeting network connectivity and
-  interoperability will try to provide this.
-
-* MD5 - A legacy algorithm, not considered cryptographically secure. Only
-  selected boards, targeting interoperability with legacy applications,
-  will offer this.
-"""
-from typing import Optional, Any
-
-class sha256:
-    """
-    Create an SHA256 hasher object and optionally feed ``data`` into it.
-    """
-
-    def digest(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def __init__(self, data: Optional[Any] = None) -> None: ...
-
-class sha1:
-    """
-    Create an SHA1 hasher object and optionally feed ``data`` into it.
-    """
-
-    def digest(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def __init__(self, data: Optional[Any] = None) -> None: ...
+"""
+hashing algorithms. See: https://docs.micropython.org/en/v1.20.0/library/hashlib.html
+
+|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
+
+This module implements binary data hashing algorithms. The exact inventory
+of available algorithms depends on a board. Among the algorithms which may
+be implemented:
+
+* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
+  It is suitable for cryptographically-secure purposes. Included in the
+  MicroPython core and any board is recommended to provide this, unless
+  it has particular code size constraints.
+
+* SHA1 - A previous generation algorithm. Not recommended for new usages,
+  but SHA1 is a part of number of Internet standards and existing
+  applications, so boards targeting network connectivity and
+  interoperability will try to provide this.
+
+* MD5 - A legacy algorithm, not considered cryptographically secure. Only
+  selected boards, targeting interoperability with legacy applications,
+  will offer this.
+"""
+from typing import Optional, Any
+
+class sha256:
+    """
+    Create an SHA256 hasher object and optionally feed ``data`` into it.
+    """
+
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
+
+class sha1:
+    """
+    Create an SHA1 hasher object and optionally feed ``data`` into it.
+    """
+
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/uheapq.pyi` & `micropython_esp32_stubs-1.20.0.post1/uheapq.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-heap queue algorithm. See: https://docs.micropython.org/en/v1.19.1/library/heapq.html
-
-|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
-
-This module implements the
-`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
-
-A heap queue is essentially a list that has its elements stored in such a way
-that the first item of the list is always the smallest.
-"""
-from typing import Any
-
-def heappop(heap) -> Any:
-    """
-    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
-    ``heap`` is empty.
-
-    The returned item will be the smallest item in the ``heap``.
-    """
-    ...
-
-def heappush(heap, item) -> Any:
-    """
-    Push the ``item`` onto the ``heap``.
-    """
-    ...
-
-def heapify(x) -> Any:
-    """
-    Convert the list ``x`` into a heap.  This is an in-place operation.
-    """
-    ...
+"""
+heap queue algorithm. See: https://docs.micropython.org/en/v1.20.0/library/heapq.html
+
+|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
+
+This module implements the
+`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
+
+A heap queue is essentially a list that has its elements stored in such a way
+that the first item of the list is always the smallest.
+"""
+from typing import Any
+
+def heappop(heap) -> Any:
+    """
+    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
+    ``heap`` is empty.
+
+    The returned item will be the smallest item in the ``heap``.
+    """
+    ...
+
+def heappush(heap, item) -> Any:
+    """
+    Push the ``item`` onto the ``heap``.
+    """
+    ...
+
+def heapify(x) -> Any:
+    """
+    Convert the list ``x`` into a heap.  This is an in-place operation.
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/umachine.pyi` & `micropython_esp32_stubs-1.20.0.post1/umachine.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,1174 +1,1243 @@
-"""
-functions related to the hardware. See: https://docs.micropython.org/en/v1.19.1/library/machine.html
-
-The ``machine`` module contains specific functions related to the hardware
-on a particular board. Most functions in this module allow to achieve direct
-and unrestricted access to and control of hardware blocks on a system
-(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
-malfunction, lockups, crashes of your board, and in extreme cases, hardware
-damage.
-"""
-from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
-
-TIMER_WAKE: int
-EXT1_WAKE: int
-HARD_RESET: int
-SOFT_RESET: int
-PIN_WAKE: int
-PWRON_RESET: int
-SLEEP: int
-WDT_RESET: int
-TOUCHPAD_WAKE: int
-ULP_WAKE: int
-EXT0_WAKE: int
-DEEPSLEEP: int
-DEEPSLEEP_RESET: int
-
-def enable_irq(state) -> Any:
-    """
-    Re-enable interrupt requests.
-    The *state* parameter should be the value that was returned from the most
-    recent call to the `disable_irq()` function.
-    """
-    ...
-
-def bitstream(pin, encoding, timing, data, /) -> Any:
-    """
-    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
-    specifies how the bits are encoded, and *timing* is an encoding-specific timing
-    specification.
-
-    The supported encodings are:
-
-      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
-        1 bits as timed pulses, starting with the most significant bit.
-        The *timing* must be a four-tuple of nanoseconds in the format
-        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
-        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
-        at 800kHz.
-
-    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
-    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
-    will be closer to +/-30ns.
-
-    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
-       module for a higher-level API.
-    """
-    ...
-
-def disable_irq() -> Any:
-    """
-    Disable interrupt requests.
-    Returns the previous IRQ state which should be considered an opaque value.
-    This return value should be passed to the `enable_irq()` function to restore
-    interrupts to their original state, before `disable_irq()` was called.
-    """
-    ...
-
-def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def wake_reason() -> Any:
-    """
-    Get the wake reason. See :ref:`constants <machine_constants>` for the possible return values.
-
-    Availability: ESP32, WiPy.
-    """
-    ...
-
-def sleep() -> Any:
-    """
-    ``Note:`` This function is deprecated, use `lightsleep()` instead with no arguments.
-    """
-    ...
-
-def soft_reset() -> NoReturn:
-    """
-    Performs a soft reset of the interpreter, deleting all Python objects and
-    resetting the Python heap.  It tries to retain the method by which the user
-    is connected to the MicroPython REPL (eg serial, USB, Wifi).
-    """
-    ...
-
-def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
-    """
-    Time a pulse on the given *pin*, and return the duration of the pulse in
-    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
-    or 1 to time a high pulse.
-
-    If the current input value of the pin is different to *pulse_level*,
-    the function first (*) waits until the pin input becomes equal to *pulse_level*,
-    then (**) times the duration that the pin is equal to *pulse_level*.
-    If the pin is already equal to *pulse_level* then timing starts straight away.
-
-    The function will return -2 if there was timeout waiting for condition marked
-    (*) above, and -1 if there was timeout during the main measurement, marked (**)
-    above. The timeout is the same for both cases and given by *timeout_us* (which
-    is in microseconds).
-    """
-    ...
-
-def unique_id() -> bytes:
-    """
-    Returns a byte string with a unique identifier of a board/SoC. It will vary
-    from a board/SoC instance to another, if underlying hardware allows. Length
-    varies by hardware (so use substring of a full value if you expect a short
-    ID). In some MicroPython ports, ID corresponds to the network MAC address.
-    """
-    ...
-
-def freq(hz: Optional[Any] = None) -> Any:
-    """
-    Returns the CPU frequency in hertz.
-
-    On some ports this can also be used to set the CPU frequency by passing in *hz*.
-    """
-    ...
-
-def reset_cause() -> int:
-    """
-    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
-    """
-    ...
-
-def idle() -> Any:
-    """
-    Gates the clock to the CPU, useful to reduce power consumption at any time during
-    short or long periods. Peripherals continue working and execution resumes as soon
-    as any interrupt is triggered (on many ports this includes system timer
-    interrupt occurring at regular intervals on the order of millisecond).
-    """
-    ...
-
-def lightsleep(time_ms: Optional[Any] = None) -> Any:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def reset() -> NoReturn:
-    """
-    Resets the device in a manner similar to pushing the external RESET
-    button.
-    """
-    ...
-
-mem8: Any
-
-class PWM:
-    """
-    Construct and return a new PWM object using the following parameters:
-
-       - *dest* is the entity on which the PWM is output, which is usually a
-         :ref:`machine.Pin <machine.Pin>` object, but a port may allow other values,
-         like integers.
-       - *freq* should be an integer which sets the frequency in Hz for the
-         PWM cycle.
-       - *duty_u16* sets the duty cycle as a ratio ``duty_u16 / 65535``.
-       - *duty_ns* sets the pulse width in nanoseconds.
-
-    Setting *freq* may affect other PWM objects if the objects share the same
-    underlying PWM generator (this is hardware specific).
-    Only one of *duty_u16* and *duty_ns* should be specified at a time.
-    """
-
-    def duty_u16(self, value: Optional[Any] = None) -> int:
-        """
-        Get or set the current duty cycle of the PWM output, as an unsigned 16-bit
-        value in the range 0 to 65535 inclusive.
-
-        With no arguments the duty cycle is returned.
-
-        With a single *value* argument the duty cycle is set to that value, measured
-        as the ratio ``value / 65535``.
-        """
-        ...
-    def init(self, *, freq, duty_u16, duty_ns) -> None:
-        """
-        Modify settings for the PWM object.  See the above constructor for details
-        about the parameters.
-        """
-        ...
-    def freq(self, value: Optional[Any] = None) -> Any:
-        """
-        Get or set the current frequency of the PWM output.
-
-        With no arguments the frequency in Hz is returned.
-
-        With a single *value* argument the frequency is set to that value in Hz.  The
-        method may raise a ``ValueError`` if the frequency is outside the valid range.
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Disable the PWM output.
-        """
-        ...
-    def duty_ns(self, value: Optional[Any] = None) -> int:
-        """
-        Get or set the current pulse width of the PWM output, as a value in nanoseconds.
-
-        With no arguments the pulse width in nanoseconds is returned.
-
-        With a single *value* argument the pulse width is set to that value.
-        """
-        ...
-    def duty(self, *args, **kwargs) -> Any: ...
-    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None: ...
-
-class UART:
-    """
-    Construct a UART object of the given id.
-    """
-
-    INV_RTS: int
-    INV_RX: int
-    CTS: int
-    INV_CTS: int
-    INV_TX: int
-    RTS: int
-    def deinit(self) -> None:
-        """
-        Turn off the UART bus.
-        """
-        ...
-    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
-        """
-        Initialise the UART bus with the given parameters:
-
-          - *baudrate* is the clock rate.
-          - *bits* is the number of bits per character, 7, 8 or 9.
-          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
-          - *stop* is the number of stop bits, 1 or 2.
-
-        Additional keyword-only parameters that may be supported by a port are:
-
-          - *tx* specifies the TX pin to use.
-          - *rx* specifies the RX pin to use.
-          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
-          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
-          - *txbuf* specifies the length in characters of the TX buffer.
-          - *rxbuf* specifies the length in characters of the RX buffer.
-          - *timeout* specifies the time to wait for the first character (in ms).
-          - *timeout_char* specifies the time to wait between characters (in ms).
-          - *invert* specifies which lines to invert.
-
-              - ``0`` will not invert lines (idle state of both lines is logic high).
-              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
-              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
-              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
-
-          - *flow* specifies which hardware flow control signals to use. The value
-            is a bitmask.
-
-              - ``0`` will ignore hardware flow control signals.
-              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
-                signal if the receive FIFO has sufficient space to accept more data.
-              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
-                CTS input pin signals that the receiver is running low on buffer space.
-              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
-
-        On the WiPy only the following keyword-only parameter is supported:
-
-          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
-            Any of the pins can be None if one wants the UART to operate with limited functionality.
-            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
-            When no pins are given, then the default set of TX and RX pins is taken, and hardware
-            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
-        """
-        ...
-    def sendbreak(self) -> None:
-        """
-        Send a break condition on the bus. This drives the bus low for a duration
-        longer than required for a normal transmission of a character.
-        """
-        ...
-    def read(self, nbytes: Optional[Any] = None) -> bytes:
-        """
-        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
-        otherwise read as much data as possible. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: a bytes object containing the bytes read in.  Returns ``None``
-        on timeout.
-        """
-        ...
-    def any(self) -> int:
-        """
-        Returns an integer counting the number of characters that can be read without
-        blocking.  It will return 0 if there are no characters available and a positive
-        number if there are characters.  The method may return 1 even if there is more
-        than one character available for reading.
-
-        For more sophisticated querying of available characters use select.poll::
-
-         poll = select.poll()
-         poll.register(uart, select.POLLIN)
-         poll.poll(timeout)
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the bus.
-
-        Return value: number of bytes written or ``None`` on timeout.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
-        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: number of bytes read and stored into ``buf`` or ``None`` on
-        timeout.
-        """
-        ...
-    def readline(self) -> None:
-        """
-        Read a line, ending in a newline character. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: the line read or ``None`` on timeout.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-mem32: Any
-mem16: Any
-
-class ADCBlock:
-    """
-    Access the ADC peripheral identified by *id*, which may be an integer
-    or string.
-
-    The *bits* argument, if given, sets the resolution in bits of the
-    conversion process.  If not specified then the previous or default
-    resolution is used.
-    """
-
-    def init(self, *, bits) -> None:
-        """
-        Configure the ADC peripheral.  *bits* will set the resolution of the
-        conversion process.
-        """
-        ...
-    def connect(self, channel, source) -> Any:
-        """
-        Connect up a channel on the ADC peripheral so it is ready for sampling,
-        and return an :ref:`ADC <machine.ADC>` object that represents that connection.
-
-        The *channel* argument must be an integer, and *source* must be an object
-        (for example a :ref:`Pin <machine.Pin>`) which can be connected up for sampling.
-
-        If only *channel* is given then it is configured for sampling.
-
-        If only *source* is given then that object is connected to a default
-        channel ready for sampling.
-
-        If both *channel* and *source* are given then they are connected together
-        and made ready for sampling.
-        """
-        ...
-    def __init__(self, id, *, bits) -> None: ...
-
-class ADC:
-    """
-    Access the ADC associated with a source identified by *id*.  This
-    *id* may be an integer (usually specifying a channel number), a
-    :ref:`Pin <machine.Pin>` object, or other value supported by the
-    underlying machine.
-
-    If additional keyword-arguments are given then they will configure
-    various aspects of the ADC.  If not given, these settings will take
-    previous or default values.  The settings are:
-
-      - *sample_ns* is the sampling time in nanoseconds.
-
-      - *atten* specifies the input attenuation.
-    """
-
-    ATTN_6DB: int
-    WIDTH_10BIT: int
-    WIDTH_11BIT: int
-    WIDTH_12BIT: int
-    WIDTH_9BIT: int
-    ATTN_0DB: int
-    ATTN_2_5DB: int
-    ATTN_11DB: int
-    def read_u16(self) -> int:
-        """
-        Take an analog reading and return an integer in the range 0-65535.
-        The return value represents the raw reading taken by the ADC, scaled
-        such that the minimum value is 0 and the maximum value is 65535.
-        """
-        ...
-    def init(self, *, sample_ns, atten) -> Any:
-        """
-        Apply the given settings to the ADC.  Only those arguments that are
-        specified will be changed.  See the ADC constructor above for what the
-        arguments are.
-        """
-        ...
-    def read_uv(self) -> int:
-        """
-        Take an analog reading and return an integer value with units of
-        microvolts.  It is up to the particular port whether or not this value
-        is calibrated, and how calibration is done.
-        """
-        ...
-    def width(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def block(self) -> Any:
-        """
-        Return the :ref:`ADCBlock <machine.ADCBlock>` instance associated with
-        this ADC object.
-
-        This method only exists if the port supports the
-        :ref:`ADCBlock <machine.ADCBlock>` class.
-        """
-        ...
-    def atten(self, *args, **kwargs) -> Any: ...
-    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
-
-class I2S:
-    """
-    Construct an I2S object of the given id:
-
-    - ``id`` identifies a particular I2S bus; it is board and port specific
-
-    Keyword-only parameters that are supported on all ports:
-
-      - ``sck`` is a pin object for the serial clock line
-      - ``ws`` is a pin object for the word select line
-      - ``sd`` is a pin object for the serial data line
-      - ``mck`` is a pin object for the master clock line;
-        master clock frequency is sampling rate * 256
-      - ``mode`` specifies receive or transmit
-      - ``bits`` specifies sample size (bits), 16 or 32
-      - ``format`` specifies channel format, STEREO or MONO
-      - ``rate`` specifies audio sampling rate (Hz);
-        this is the frequency of the ``ws`` signal
-      - ``ibuf`` specifies internal buffer length (bytes)
-
-    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
-    sample data is transfered between the internal buffer and the I2S peripheral unit.
-    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
-    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
-    """
-
-    RX: int
-    MONO: int
-    STEREO: int
-    TX: int
-    @staticmethod
-    def shift(*, buf, bits, shift) -> Any:
-        """
-        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
-        Positive for left shift, negative for right shift.
-        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
-        """
-        ...
-    def init(self, sck, *args, **kwargs) -> Any:
-        """
-        see Constructor for argument descriptions
-        """
-        ...
-    def irq(self, handler) -> Any:
-        """
-        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
-        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
-        ``handler`` is called in the context of the MicroPython scheduler.
-        """
-        ...
-    def readinto(self, buf) -> int:
-        """
-        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the left channel sample data is used.
-        Returns number of bytes read
-        """
-        ...
-    def deinit(self) -> Any:
-        """
-        Deinitialize the I2S bus
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the sample data is written to both the right and left channels.
-        Returns number of bytes written
-        """
-        ...
-    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
-
-class DAC:
-    def write(self, *args, **kwargs) -> Any: ...
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class I2C:
-    """
-    Construct and return a new I2C object using the following parameters:
-
-       - *id* identifies a particular I2C peripheral.  Allowed values for
-         depend on the particular port/board
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-
-    Note that some ports/boards will have default values of *scl* and *sda*
-    that can be changed in this constructor.  Others will have fixed values
-    of *scl* and *sda* that cannot be changed.
-    """
-
-    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.  The number of bytes read is the
-        length of *buf*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_into(self, addr, buf, stop=True, /) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr*.
-        The number of bytes read will be the length of *buf*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr* starting from the memory
-        address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Write *buf* to the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def scan(self) -> List:
-        """
-        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
-        those that respond.  A device responds if it pulls the SDA line low after
-        its address (including a write bit) is sent on the bus.
-        """
-        ...
-    def writeto(self, addr, buf, stop=True, /) -> int:
-        """
-        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
-        NACK is received following the write of a byte from *buf* then the
-        remaining bytes are not sent.  If *stop* is true then a STOP condition is
-        generated at the end of the transfer, even if a NACK is received.
-        The function returns the number of ACKs that were received.
-        """
-        ...
-    def writevto(self, addr, vector, stop=True, /) -> int:
-        """
-        Write the bytes contained in *vector* to the peripheral specified by *addr*.
-        *vector* should be a tuple or list of objects with the buffer protocol.
-        The *addr* is sent once and then the bytes from each object in *vector*
-        are written out sequentially.  The objects in *vector* may be zero bytes
-        in length in which case they don't contribute to the output.
-
-        If a NACK is received following the write of a byte from one of the
-        objects in *vector* then the remaining bytes, and any remaining objects,
-        are not sent.  If *stop* is true then a STOP condition is generated at
-        the end of the transfer, even if a NACK is received.  The function
-        returns the number of ACKs that were received.
-        """
-        ...
-    def start(self) -> None:
-        """
-        Generate a START condition on the bus (SDA transitions to low while SCL is high).
-        """
-        ...
-    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def readinto(self, buf, nack=True, /) -> Any:
-        """
-        Reads bytes from the bus and stores them into *buf*.  The number of bytes
-        read is the length of *buf*.  An ACK will be sent on the bus after
-        receiving all but the last byte.  After the last byte is received, if *nack*
-        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
-        case the peripheral assumes more bytes are going to be read in a later call).
-        """
-        ...
-    def init(self, scl, sda, *, freq=400000) -> None:
-        """
-        Initialise the I2C bus with the given arguments:
-
-           - *scl* is a pin object for the SCL line
-           - *sda* is a pin object for the SDA line
-           - *freq* is the SCL clock rate
-        """
-        ...
-    def stop(self) -> None:
-        """
-        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes from *buf* to the bus.  Checks that an ACK is received
-        after each byte and stops transmitting the remaining bytes if a NACK is
-        received.  The function returns the number of ACKs that were received.
-        """
-        ...
-    def __init__(
-        self, id: Union[int, str] = -1, *, scl: Optional[Union[Pin, str]] = None, sda: Optional[Union[Pin, str]] = None, freq=400_000
-    ) -> None: ...
-
-class Timer:
-    """
-    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
-    virtual timer (if supported by a board).
-    ``id`` shall not be passed as a keyword argument.
-
-    See ``init`` for parameters of initialisation.
-    """
-
-    ONE_SHOT: int
-    PERIODIC: int
-    def deinit(self) -> None:
-        """
-        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
-        """
-        ...
-    def init(self, *, mode=PERIODIC, period=-1, callback=None) -> None:
-        """
-        Initialise the timer. Example::
-
-            def mycallback(t):
-                pass
-
-            # periodic with 100ms period
-            tim.init(period=100, callback=mycallback)
-
-            # one shot firing after 1000ms
-            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
-
-        Keyword arguments:
-
-          - ``mode`` can be one of:
-
-            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
-              period of the channel expires.
-            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
-              frequency of the channel.
-
-          - ``period`` - The timer period, in milliseconds.
-
-          - ``callback`` - The callable to call upon expiration of the timer period.
-            The callback must take one argument, which is passed the Timer object.
-            The ``callback`` argument shall be specified. Otherwise an exception
-            will occurr upon timer expiration:
-            ``TypeError: 'NoneType' object isn't callable``
-        """
-        ...
-    def value(self, *args, **kwargs) -> Any: ...
-    def __init__(self, id=-1, *args, **kwargs) -> None: ...
-
-class SoftSPI:
-    """
-    Construct a new software SPI object.  Additional parameters must be
-    given, usually at least *sck*, *mosi* and *miso*, and these are used
-    to initialise the bus.  See `SPI.init` for a description of the parameters.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def write_readinto(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
-
-class Pin:
-    """
-    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
-    additional arguments are given in the constructor then they are used to initialise
-    the pin.  Any settings that are not specified will remain in their previous state.
-
-    The arguments are:
-
-      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
-        types are: int (an internal Pin identifier), str (a Pin name), and tuple
-        (pair of [port, pin]).
-
-      - ``mode`` specifies the pin mode, which can be one of:
-
-        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
-          is in high-impedance state.
-
-        - ``Pin.OUT`` - Pin is configured for (normal) output.
-
-        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
-          output works in the following way: if the output value is set to 0 the pin
-          is active at a low level; if the output value is 1 the pin is in a high-impedance
-          state.  Not all ports implement this mode, or some might only on certain pins.
-
-        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
-          port specific.  For a pin configured in such a way any other Pin methods
-          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
-          or a hardware-specific, result).  Not all ports implement this mode.
-
-        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
-          open-drain.  Not all ports implement this mode.
-
-        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
-
-      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
-        one of:
-
-        - ``None`` - No pull up or down resistor.
-        - ``Pin.PULL_UP`` - Pull up resistor enabled.
-        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
-
-      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
-        output pin value if given, otherwise the state of the pin peripheral remains
-        unchanged.
-
-      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
-        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
-        capabilities are port dependent.  Not all ports implement this argument.
-
-      - ``alt`` specifies an alternate function for the pin and the values it can take are
-        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
-        modes.  It may be used when a pin supports more than one alternate function.  If only
-        one pin alternate function is supported the this argument is not required.  Not all
-        ports implement this argument.
-
-    As specified above, the Pin class allows to set an alternate function for a particular
-    pin, but it does not specify any further operations on such a pin.  Pins configured in
-    alternate-function mode are usually not used as GPIO but are instead driven by other
-    hardware peripherals.  The only operation supported on such a pin is re-initialising,
-    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
-    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
-    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
-    """
-
-    OPEN_DRAIN: int
-    IRQ_FALLING: int
-    IRQ_RISING: int
-    PULL_UP: int
-    OUT: int
-    PULL_DOWN: int
-    WAKE_HIGH: int
-    DRIVE_0: int
-    IN: int
-    WAKE_LOW: int
-    DRIVE_3: int
-    DRIVE_1: int
-    DRIVE_2: int
-    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
-        """
-           Configure an interrupt handler to be called when the trigger source of the
-           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
-           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
-           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
-           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
-           state '0' and the external pin value for state '1'.
-
-           The arguments are:
-
-             - ``handler`` is an optional function to be called when the interrupt
-               triggers. The handler must take exactly one argument which is the
-               ``Pin`` instance.
-
-             - ``trigger`` configures the event which can generate an interrupt.
-               Possible values are:
-
-               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
-               - ``Pin.IRQ_RISING`` interrupt on rising edge.
-               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
-               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
-
-               These values can be OR'ed together to trigger on multiple events.
-
-             - ``priority`` sets the priority level of the interrupt.  The values it
-               can take are port-specific, but higher values always represent higher
-               priorities.
-
-             - ``wake`` selects the power mode in which this interrupt can wake up the
-               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
-               These values can also be OR'ed together to make a pin generate interrupts in
-               more than one power mode.
-
-             - ``hard`` if true a hardware interrupt is used. This reduces the delay
-               between the pin change and the handler being called. Hard interrupt
-               handlers may not allocate memory; see :ref:`isr_rules`.
-               Not all ports support this argument.
-
-           This method returns a callback object.
-
-        The following methods are not part of the core Pin API and only implemented on certain ports.
-        """
-        ...
-    def off(self) -> None:
-        """
-        Set pin to "0" output level.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Set pin to "1" output level.
-        """
-        ...
-    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
-        """
-        Re-initialise the pin using the given parameters.  Only those arguments that
-        are specified will be set.  The rest of the pin peripheral state will remain
-        unchanged.  See the constructor documentation for details of the arguments.
-
-        Returns ``None``.
-        """
-        ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the pin, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the digital logic level of
-        the pin, returning 0 or 1 corresponding to low and high voltage signals
-        respectively.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The method returns the actual input value currently present
-            on the pin.
-          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
-          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
-            return value of the method is undefined.  Otherwise, if the pin is in
-            state '1', the method returns the actual input value currently present
-            on the pin.
-
-        If the argument is supplied then this method sets the digital logic level of
-        the pin.  The argument ``x`` can be anything that converts to a boolean.
-        If it converts to ``True``, the pin is set to state '1', otherwise it is set
-        to state '0'.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
-            pin state does not change, it remains in the high-impedance state.  The
-            stored value will become active on the pin as soon as it is changed to
-            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
-          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
-          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
-            state.  Otherwise the pin is set to high-impedance state.
-
-        When setting the value this method returns ``None``.
-        """
-        ...
-    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
-
-class WDT:
-    """
-    Create a WDT object and start it. The timeout must be given in milliseconds.
-    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
-
-    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
-    cannot be specified, it is determined by the underlying system.
-    """
-
-    def feed(self) -> None:
-        """
-        Feed the WDT to prevent it from resetting the system. The application
-        should place this call in a sensible place ensuring that the WDT is
-        only fed after verifying that everything is functioning correctly.
-        """
-        ...
-    def __init__(self, id=0, timeout=5000) -> None: ...
-
-class TouchPad:
-    def config(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class SDCard:
-    """
-    This class provides access to SD or MMC storage cards using either
-    a dedicated SD/MMC interface hardware or through an SPI channel.
-    The class implements the block protocol defined by :class:`os.AbstractBlockDev`.
-    This allows the mounting of an SD card to be as simple as::
-
-      os.mount(machine.SDCard(), "/sd")
-
-    The constructor takes the following parameters:
-
-     - *slot* selects which of the available interfaces to use. Leaving this
-       unset will select the default interface.
-
-     - *width* selects the bus width for the SD/MMC interface.
-
-     - *cd* can be used to specify a card-detect pin.
-
-     - *wp* can be used to specify a write-protect pin.
-
-     - *sck* can be used to specify an SPI clock pin.
-
-     - *miso* can be used to specify an SPI miso pin.
-
-     - *mosi* can be used to specify an SPI mosi pin.
-
-     - *cs* can be used to specify an SPI chip select pin.
-
-     - *freq* selects the SD/MMC interface frequency in Hz (only supported on the ESP32).
-    """
-
-    def ioctl(self, *args, **kwargs) -> Any: ...
-    def readblocks(self, *args, **kwargs) -> Any: ...
-    def writeblocks(self, *args, **kwargs) -> Any: ...
-    def info(self, *args, **kwargs) -> Any: ...
-    def deinit(self, *args, **kwargs) -> Any: ...
-    def __init__(self, slot=1, width=1, cd=None, wp=None, sck=None, miso=None, mosi=None, cs=None, freq=20000000) -> None: ...
-
-class RTC:
-    """
-    Create an RTC object. See init for parameters of initialization.
-    """
-
-    def init(self, datetime) -> None:
-        """
-        Initialise the RTC. Datetime is a tuple of the form:
-
-           ``(year, month, day[, hour[, minute[, second[, microsecond[, tzinfo]]]]])``
-        """
-        ...
-    def memory(self, *args, **kwargs) -> Any: ...
-    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
-        """
-        Get or set the date and time of the RTC.
-
-        With no arguments, this method returns an 8-tuple with the current
-        date and time.  With 1 argument (being an 8-tuple) it sets the date
-        and time.
-
-        The 8-tuple has the following format:
-
-            (year, month, day, weekday, hours, minutes, seconds, subseconds)
-
-        The meaning of the ``subseconds`` field is hardware dependent.
-        """
-        ...
-    def __init__(self, id=0, *args, **kwargs) -> None: ...
-
-class SoftI2C:
-    """
-    Construct a new software I2C object.  The parameters are:
-
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-       - *timeout* is the maximum time in microseconds to wait for clock
-         stretching (SCL held low by another device on the bus), after
-         which an ``OSError(ETIMEDOUT)`` exception is raised.
-    """
-
-    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_mem(self, *args, **kwargs) -> Any: ...
-    def writeto_mem(self, *args, **kwargs) -> Any: ...
-    def scan(self, *args, **kwargs) -> Any: ...
-    def writeto(self, *args, **kwargs) -> Any: ...
-    def writevto(self, *args, **kwargs) -> Any: ...
-    def start(self, *args, **kwargs) -> Any: ...
-    def readfrom(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def stop(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
-
-class SPI:
-    """
-    Construct an SPI object on the given bus, *id*. Values of *id* depend
-    on a particular port and its hardware. Values 0, 1, etc. are commonly used
-    to select hardware SPI block #0, #1, etc.
-
-    With no additional parameters, the SPI object is created but not
-    initialised (it has the settings from the last initialisation of
-    the bus, if any).  If extra arguments are given, the bus is initialised.
-    See ``init`` for parameters of initialisation.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self) -> None:
-        """
-        Turn off the SPI bus.
-        """
-        ...
-    def init(
-        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
-    ) -> None:
-        """
-        Initialise the SPI bus with the given parameters:
-
-          - ``baudrate`` is the SCK clock rate.
-          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
-          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
-            respectively.
-          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
-          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
-          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
-            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
-            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
-            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
-            (``id`` = -1).
-          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
-            specify them as a tuple of ``pins`` parameter.
-
-        In the case of hardware SPI the actual clock frequency may be lower than the
-        requested baudrate. This is dependant on the platform hardware. The actual
-        rate may be determined by printing the SPI object.
-        """
-        ...
-    def write_readinto(self, write_buf, read_buf) -> int:
-        """
-        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
-        buffers can be the same or different, but both buffers must have the
-        same length.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def read(self, nbytes, write=0x00) -> bytes:
-        """
-        Read a number of bytes specified by ``nbytes`` while continuously writing
-        the single byte given by ``write``.
-        Returns a ``bytes`` object with the data that was read.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes contained in ``buf``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def readinto(self, buf, write=0x00) -> int:
-        """
-        Read into the buffer specified by ``buf`` while continuously writing the
-        single byte given by ``write``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes read.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-class Signal:
-    """
-            Signal(pin_arguments..., *, invert=False)
-
-    Create a Signal object. There're two ways to create it:
-
-    * By wrapping existing Pin object - universal method which works for
-      any board.
-    * By passing required Pin parameters directly to Signal constructor,
-      skipping the need to create intermediate Pin object. Available on
-      many, but not all boards.
-
-    The arguments are:
-
-      - ``pin_obj`` is existing Pin object.
-
-      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
-
-      - ``invert`` - if True, the signal will be inverted (active low).
-    """
-
-    def off(self) -> None:
-        """
-        Deactivate signal.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Activate signal.
-        """
-        ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the signal, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the signal level, 1 meaning
-        signal is asserted (active) and 0 - signal inactive.
-
-        If the argument is supplied then this method sets the signal level. The
-        argument ``x`` can be anything that converts to a boolean. If it converts
-        to ``True``, the signal is active, otherwise it is inactive.
-
-        Correspondence between signal being active and actual logic level on the
-        underlying pin depends on whether signal is inverted (active-low) or not.
-        For non-inverted signal, active status corresponds to logical 1, inactive -
-        to logical 0. For inverted/active-low signal, active status corresponds
-        to logical 0, while inactive - to logical 1.
-        """
-        ...
-    def __init__(self, pin_obj, *args, invert=False) -> None: ...
+"""
+functions related to the hardware. See: https://docs.micropython.org/en/v1.20.0/library/machine.html
+
+The ``machine`` module contains specific functions related to the hardware
+on a particular board. Most functions in this module allow to achieve direct
+and unrestricted access to and control of hardware blocks on a system
+(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
+malfunction, lockups, crashes of your board, and in extreme cases, hardware
+damage.
+"""
+from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
+
+ULP_WAKE: int
+SLEEP: int
+PWRON_RESET: int
+PIN_WAKE: int
+SOFT_RESET: int
+WDT_RESET: int
+TOUCHPAD_WAKE: int
+TIMER_WAKE: int
+HARD_RESET: int
+EXT0_WAKE: int
+DEEPSLEEP_RESET: int
+DEEPSLEEP: int
+EXT1_WAKE: int
+
+def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def soft_reset() -> NoReturn:
+    """
+    Performs a soft reset of the interpreter, deleting all Python objects and
+    resetting the Python heap.  It tries to retain the method by which the user
+    is connected to the MicroPython REPL (eg serial, USB, Wifi).
+    """
+    ...
+
+def dht_readinto(*args, **kwargs) -> Any: ...
+def reset() -> NoReturn:
+    """
+    Resets the device in a manner similar to pushing the external RESET
+    button.
+    """
+    ...
+
+def unique_id() -> bytes:
+    """
+    Returns a byte string with a unique identifier of a board/SoC. It will vary
+    from a board/SoC instance to another, if underlying hardware allows. Length
+    varies by hardware (so use substring of a full value if you expect a short
+    ID). In some MicroPython ports, ID corresponds to the network MAC address.
+    """
+    ...
+
+def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
+    """
+    Time a pulse on the given *pin*, and return the duration of the pulse in
+    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
+    or 1 to time a high pulse.
+
+    If the current input value of the pin is different to *pulse_level*,
+    the function first (*) waits until the pin input becomes equal to *pulse_level*,
+    then (**) times the duration that the pin is equal to *pulse_level*.
+    If the pin is already equal to *pulse_level* then timing starts straight away.
+
+    The function will return -2 if there was timeout waiting for condition marked
+    (*) above, and -1 if there was timeout during the main measurement, marked (**)
+    above. The timeout is the same for both cases and given by *timeout_us* (which
+    is in microseconds).
+    """
+    ...
+
+def bitstream(pin, encoding, timing, data, /) -> Any:
+    """
+    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
+    specifies how the bits are encoded, and *timing* is an encoding-specific timing
+    specification.
+
+    The supported encodings are:
+
+      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
+        1 bits as timed pulses, starting with the most significant bit.
+        The *timing* must be a four-tuple of nanoseconds in the format
+        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
+        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
+        at 800kHz.
+
+    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
+    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
+    will be closer to +/-30ns.
+
+    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
+       module for a higher-level API.
+    """
+    ...
+
+def idle() -> Any:
+    """
+    Gates the clock to the CPU, useful to reduce power consumption at any time during
+    short or long periods. Peripherals continue working and execution resumes as soon
+    as any interrupt is triggered (on many ports this includes system timer
+    interrupt occurring at regular intervals on the order of millisecond).
+    """
+    ...
+
+def freq(hz: Optional[Any] = None) -> Any:
+    """
+    Returns the CPU frequency in hertz.
+
+    On some ports this can also be used to set the CPU frequency by passing in *hz*.
+    """
+    ...
+
+def lightsleep(time_ms: Optional[Any] = None) -> Any:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def disable_irq() -> Any:
+    """
+    Disable interrupt requests.
+    Returns the previous IRQ state which should be considered an opaque value.
+    This return value should be passed to the `enable_irq()` function to restore
+    interrupts to their original state, before `disable_irq()` was called.
+    """
+    ...
+
+def enable_irq(state) -> Any:
+    """
+    Re-enable interrupt requests.
+    The *state* parameter should be the value that was returned from the most
+    recent call to the `disable_irq()` function.
+    """
+    ...
+
+def reset_cause() -> int:
+    """
+    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
+    """
+    ...
+
+def sleep() -> Any:
+    """
+    ``Note:`` This function is deprecated, use `lightsleep()` instead with no arguments.
+    """
+    ...
+
+def wake_reason() -> Any:
+    """
+    Get the wake reason. See :ref:`constants <machine_constants>` for the possible return values.
+
+    Availability: ESP32, WiPy.
+    """
+    ...
+
+mem8: Any
+
+class PWM:
+    """
+    Construct and return a new PWM object using the following parameters:
+
+       - *dest* is the entity on which the PWM is output, which is usually a
+         :ref:`machine.Pin <machine.Pin>` object, but a port may allow other values,
+         like integers.
+       - *freq* should be an integer which sets the frequency in Hz for the
+         PWM cycle.
+       - *duty_u16* sets the duty cycle as a ratio ``duty_u16 / 65535``.
+       - *duty_ns* sets the pulse width in nanoseconds.
+
+    Setting *freq* may affect other PWM objects if the objects share the same
+    underlying PWM generator (this is hardware specific).
+    Only one of *duty_u16* and *duty_ns* should be specified at a time.
+    """
+
+    def duty_u16(self, value: Optional[Any] = None) -> int:
+        """
+        Get or set the current duty cycle of the PWM output, as an unsigned 16-bit
+        value in the range 0 to 65535 inclusive.
+
+        With no arguments the duty cycle is returned.
+
+        With a single *value* argument the duty cycle is set to that value, measured
+        as the ratio ``value / 65535``.
+        """
+        ...
+    def init(self, *, freq, duty_u16, duty_ns) -> None:
+        """
+        Modify settings for the PWM object.  See the above constructor for details
+        about the parameters.
+        """
+        ...
+    def freq(self, value: Optional[Any] = None) -> Any:
+        """
+        Get or set the current frequency of the PWM output.
+
+        With no arguments the frequency in Hz is returned.
+
+        With a single *value* argument the frequency is set to that value in Hz.  The
+        method may raise a ``ValueError`` if the frequency is outside the valid range.
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Disable the PWM output.
+        """
+        ...
+    def duty_ns(self, value: Optional[Any] = None) -> int:
+        """
+        Get or set the current pulse width of the PWM output, as a value in nanoseconds.
+
+        With no arguments the pulse width in nanoseconds is returned.
+
+        With a single *value* argument the pulse width is set to that value.
+        """
+        ...
+    def duty(self, *args, **kwargs) -> Any: ...
+    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None: ...
+
+class UART:
+    """
+    Construct a UART object of the given id.
+    """
+
+    INV_CTS: int
+    CTS: int
+    INV_TX: int
+    INV_RTS: int
+    INV_RX: int
+    RTS: int
+    def deinit(self) -> None:
+        """
+        Turn off the UART bus.
+
+        .. note::
+          You will not be able to call ``init()`` on the object after ``deinit()``.
+          A new instance needs to be created in that case.
+        """
+        ...
+    def sendbreak(self) -> None:
+        """
+        Send a break condition on the bus. This drives the bus low for a duration
+        longer than required for a normal transmission of a character.
+        """
+        ...
+    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
+        """
+        Initialise the UART bus with the given parameters:
+
+          - *baudrate* is the clock rate.
+          - *bits* is the number of bits per character, 7, 8 or 9.
+          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
+          - *stop* is the number of stop bits, 1 or 2.
+
+        Additional keyword-only parameters that may be supported by a port are:
+
+          - *tx* specifies the TX pin to use.
+          - *rx* specifies the RX pin to use.
+          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
+          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
+          - *txbuf* specifies the length in characters of the TX buffer.
+          - *rxbuf* specifies the length in characters of the RX buffer.
+          - *timeout* specifies the time to wait for the first character (in ms).
+          - *timeout_char* specifies the time to wait between characters (in ms).
+          - *invert* specifies which lines to invert.
+
+              - ``0`` will not invert lines (idle state of both lines is logic high).
+              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
+              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
+              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
+
+          - *flow* specifies which hardware flow control signals to use. The value
+            is a bitmask.
+
+              - ``0`` will ignore hardware flow control signals.
+              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
+                signal if the receive FIFO has sufficient space to accept more data.
+              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
+                CTS input pin signals that the receiver is running low on buffer space.
+              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
+
+        On the WiPy only the following keyword-only parameter is supported:
+
+          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
+            Any of the pins can be None if one wants the UART to operate with limited functionality.
+            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
+            When no pins are given, then the default set of TX and RX pins is taken, and hardware
+            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
+
+        .. note::
+          It is possible to call ``init()`` multiple times on the same object in
+          order to reconfigure  UART on the fly. That allows using single UART
+          peripheral to serve different devices attached to different GPIO pins.
+          Only one device can be served at a time in that case.
+          Also do not call ``deinit()`` as it will prevent calling ``init()``
+          again.
+        """
+        ...
+    def flush(self) -> Any:
+        """
+        Waits until all data has been sent. In case of a timeout, an exception is raised. The timeout
+        duration depends on the tx buffer size and the baud rate. Unless flow control is enabled, a timeout
+        should not occur.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call returns while the last byte is sent.
+            If required, a one character wait time has to be added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def txdone(self) -> bool:
+        """
+        Tells whether all data has been sent or no data transfer is happening. In this case,
+        it returns ``True``. If a data transmission is ongoing it returns ``False``.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call may return ``True`` even if the last byte
+            of a transfer is still being sent. If required, a one character wait time has to be
+            added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def read(self, nbytes: Optional[Any] = None) -> bytes:
+        """
+        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
+        otherwise read as much data as possible. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: a bytes object containing the bytes read in.  Returns ``None``
+        on timeout.
+        """
+        ...
+    def any(self) -> int:
+        """
+        Returns an integer counting the number of characters that can be read without
+        blocking.  It will return 0 if there are no characters available and a positive
+        number if there are characters.  The method may return 1 even if there is more
+        than one character available for reading.
+
+        For more sophisticated querying of available characters use select.poll::
+
+         poll = select.poll()
+         poll.register(uart, select.POLLIN)
+         poll.poll(timeout)
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the bus.
+
+        Return value: number of bytes written or ``None`` on timeout.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
+        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: number of bytes read and stored into ``buf`` or ``None`` on
+        timeout.
+        """
+        ...
+    def readline(self) -> None:
+        """
+        Read a line, ending in a newline character. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: the line read or ``None`` on timeout.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+mem32: Any
+mem16: Any
+
+class ADCBlock:
+    """
+    Access the ADC peripheral identified by *id*, which may be an integer
+    or string.
+
+    The *bits* argument, if given, sets the resolution in bits of the
+    conversion process.  If not specified then the previous or default
+    resolution is used.
+    """
+
+    def init(self, *, bits) -> None:
+        """
+        Configure the ADC peripheral.  *bits* will set the resolution of the
+        conversion process.
+        """
+        ...
+    def connect(self, channel, source) -> Any:
+        """
+        Connect up a channel on the ADC peripheral so it is ready for sampling,
+        and return an :ref:`ADC <machine.ADC>` object that represents that connection.
+
+        The *channel* argument must be an integer, and *source* must be an object
+        (for example a :ref:`Pin <machine.Pin>`) which can be connected up for sampling.
+
+        If only *channel* is given then it is configured for sampling.
+
+        If only *source* is given then that object is connected to a default
+        channel ready for sampling.
+
+        If both *channel* and *source* are given then they are connected together
+        and made ready for sampling.
+        """
+        ...
+    def __init__(self, id, *, bits) -> None: ...
+
+class ADC:
+    """
+    Access the ADC associated with a source identified by *id*.  This
+    *id* may be an integer (usually specifying a channel number), a
+    :ref:`Pin <machine.Pin>` object, or other value supported by the
+    underlying machine.
+
+    If additional keyword-arguments are given then they will configure
+    various aspects of the ADC.  If not given, these settings will take
+    previous or default values.  The settings are:
+
+      - *sample_ns* is the sampling time in nanoseconds.
+
+      - *atten* specifies the input attenuation.
+    """
+
+    ATTN_6DB: int
+    WIDTH_10BIT: int
+    WIDTH_11BIT: int
+    WIDTH_12BIT: int
+    WIDTH_9BIT: int
+    ATTN_0DB: int
+    ATTN_2_5DB: int
+    ATTN_11DB: int
+    def read_u16(self) -> int:
+        """
+        Take an analog reading and return an integer in the range 0-65535.
+        The return value represents the raw reading taken by the ADC, scaled
+        such that the minimum value is 0 and the maximum value is 65535.
+        """
+        ...
+    def init(self, *, sample_ns, atten) -> Any:
+        """
+        Apply the given settings to the ADC.  Only those arguments that are
+        specified will be changed.  See the ADC constructor above for what the
+        arguments are.
+        """
+        ...
+    def read_uv(self) -> int:
+        """
+        Take an analog reading and return an integer value with units of
+        microvolts.  It is up to the particular port whether or not this value
+        is calibrated, and how calibration is done.
+        """
+        ...
+    def width(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def block(self) -> Any:
+        """
+        Return the :ref:`ADCBlock <machine.ADCBlock>` instance associated with
+        this ADC object.
+
+        This method only exists if the port supports the
+        :ref:`ADCBlock <machine.ADCBlock>` class.
+        """
+        ...
+    def atten(self, *args, **kwargs) -> Any: ...
+    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
+
+class I2S:
+    """
+    Construct an I2S object of the given id:
+
+    - ``id`` identifies a particular I2S bus; it is board and port specific
+
+    Keyword-only parameters that are supported on all ports:
+
+      - ``sck`` is a pin object for the serial clock line
+      - ``ws`` is a pin object for the word select line
+      - ``sd`` is a pin object for the serial data line
+      - ``mck`` is a pin object for the master clock line;
+        master clock frequency is sampling rate * 256
+      - ``mode`` specifies receive or transmit
+      - ``bits`` specifies sample size (bits), 16 or 32
+      - ``format`` specifies channel format, STEREO or MONO
+      - ``rate`` specifies audio sampling rate (Hz);
+        this is the frequency of the ``ws`` signal
+      - ``ibuf`` specifies internal buffer length (bytes)
+
+    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
+    sample data is transfered between the internal buffer and the I2S peripheral unit.
+    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
+    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
+    """
+
+    RX: int
+    MONO: int
+    STEREO: int
+    TX: int
+    @staticmethod
+    def shift(*, buf, bits, shift) -> Any:
+        """
+        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
+        Positive for left shift, negative for right shift.
+        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
+        """
+        ...
+    def init(self, sck, *args, **kwargs) -> Any:
+        """
+        see Constructor for argument descriptions
+        """
+        ...
+    def irq(self, handler) -> Any:
+        """
+        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
+        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
+        ``handler`` is called in the context of the MicroPython scheduler.
+        """
+        ...
+    def readinto(self, buf) -> int:
+        """
+        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the left channel sample data is used.
+        Returns number of bytes read
+        """
+        ...
+    def deinit(self) -> Any:
+        """
+        Deinitialize the I2S bus
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the sample data is written to both the right and left channels.
+        Returns number of bytes written
+        """
+        ...
+    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
+
+class DAC:
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
+
+class I2C:
+    """
+    Construct and return a new I2C object using the following parameters:
+
+       - *id* identifies a particular I2C peripheral.  Allowed values for
+         depend on the particular port/board
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to allow for I2C
+         transactions.  This parameter is not allowed on some ports.
+
+    Note that some ports/boards will have default values of *scl* and *sda*
+    that can be changed in this constructor.  Others will have fixed values
+    of *scl* and *sda* that cannot be changed.
+    """
+
+    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.  The number of bytes read is the
+        length of *buf*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_into(self, addr, buf, stop=True, /) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr*.
+        The number of bytes read will be the length of *buf*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr* starting from the memory
+        address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Write *buf* to the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def scan(self) -> List:
+        """
+        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
+        those that respond.  A device responds if it pulls the SDA line low after
+        its address (including a write bit) is sent on the bus.
+        """
+        ...
+    def writeto(self, addr, buf, stop=True, /) -> int:
+        """
+        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
+        NACK is received following the write of a byte from *buf* then the
+        remaining bytes are not sent.  If *stop* is true then a STOP condition is
+        generated at the end of the transfer, even if a NACK is received.
+        The function returns the number of ACKs that were received.
+        """
+        ...
+    def writevto(self, addr, vector, stop=True, /) -> int:
+        """
+        Write the bytes contained in *vector* to the peripheral specified by *addr*.
+        *vector* should be a tuple or list of objects with the buffer protocol.
+        The *addr* is sent once and then the bytes from each object in *vector*
+        are written out sequentially.  The objects in *vector* may be zero bytes
+        in length in which case they don't contribute to the output.
+
+        If a NACK is received following the write of a byte from one of the
+        objects in *vector* then the remaining bytes, and any remaining objects,
+        are not sent.  If *stop* is true then a STOP condition is generated at
+        the end of the transfer, even if a NACK is received.  The function
+        returns the number of ACKs that were received.
+        """
+        ...
+    def start(self) -> None:
+        """
+        Generate a START condition on the bus (SDA transitions to low while SCL is high).
+        """
+        ...
+    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def readinto(self, buf, nack=True, /) -> Any:
+        """
+        Reads bytes from the bus and stores them into *buf*.  The number of bytes
+        read is the length of *buf*.  An ACK will be sent on the bus after
+        receiving all but the last byte.  After the last byte is received, if *nack*
+        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
+        case the peripheral assumes more bytes are going to be read in a later call).
+        """
+        ...
+    def init(self, scl, sda, *, freq=400000) -> None:
+        """
+        Initialise the I2C bus with the given arguments:
+
+           - *scl* is a pin object for the SCL line
+           - *sda* is a pin object for the SDA line
+           - *freq* is the SCL clock rate
+
+         In the case of hardware I2C the actual clock frequency may be lower than the
+         requested frequency. This is dependant on the platform hardware. The actual
+         rate may be determined by printing the I2C object.
+        """
+        ...
+    def stop(self) -> None:
+        """
+        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes from *buf* to the bus.  Checks that an ACK is received
+        after each byte and stops transmitting the remaining bytes if a NACK is
+        received.  The function returns the number of ACKs that were received.
+        """
+        ...
+    def __init__(
+        self,
+        id: Union[int, str] = -1,
+        *,
+        scl: Optional[Union[Pin, str]] = None,
+        sda: Optional[Union[Pin, str]] = None,
+        freq=400_000,
+        timeout=50000,
+    ) -> None: ...
+
+class Timer:
+    """
+    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
+    virtual timer (if supported by a board).
+    ``id`` shall not be passed as a keyword argument.
+
+    See ``init`` for parameters of initialisation.
+    """
+
+    ONE_SHOT: int
+    PERIODIC: int
+    def deinit(self) -> None:
+        """
+        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
+        """
+        ...
+    def init(self, *, mode=PERIODIC, freq=-1, period=-1, callback=None) -> None:
+        """
+        Initialise the timer. Example::
+
+            def mycallback(t):
+                pass
+
+            # periodic at 1kHz
+            tim.init(mode=Timer.PERIODIC, freq=1000, callback=mycallback)
+
+            # periodic with 100ms period
+            tim.init(period=100, callback=mycallback)
+
+            # one shot firing after 1000ms
+            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
+
+        Keyword arguments:
+
+          - ``mode`` can be one of:
+
+            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
+              period of the channel expires.
+            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
+              frequency of the channel.
+
+          - ``freq`` - The timer frequency, in units of Hz.  The upper bound of
+            the frequency is dependent on the port.  When both the ``freq`` and
+            ``period`` arguments are given, ``freq`` has a higher priority and
+            ``period`` is ignored.
+
+          - ``period`` - The timer period, in milliseconds.
+
+          - ``callback`` - The callable to call upon expiration of the timer period.
+            The callback must take one argument, which is passed the Timer object.
+            The ``callback`` argument shall be specified. Otherwise an exception
+            will occurr upon timer expiration:
+            ``TypeError: 'NoneType' object isn't callable``
+        """
+        ...
+    def value(self, *args, **kwargs) -> Any: ...
+    def __init__(self, id=-1, *args, **kwargs) -> None: ...
+
+class SoftSPI:
+    """
+    Construct a new software SPI object.  Additional parameters must be
+    given, usually at least *sck*, *mosi* and *miso*, and these are used
+    to initialise the bus.  See `SPI.init` for a description of the parameters.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def write_readinto(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
+
+class Pin:
+    """
+    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
+    additional arguments are given in the constructor then they are used to initialise
+    the pin.  Any settings that are not specified will remain in their previous state.
+
+    The arguments are:
+
+      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
+        types are: int (an internal Pin identifier), str (a Pin name), and tuple
+        (pair of [port, pin]).
+
+      - ``mode`` specifies the pin mode, which can be one of:
+
+        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
+          is in high-impedance state.
+
+        - ``Pin.OUT`` - Pin is configured for (normal) output.
+
+        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
+          output works in the following way: if the output value is set to 0 the pin
+          is active at a low level; if the output value is 1 the pin is in a high-impedance
+          state.  Not all ports implement this mode, or some might only on certain pins.
+
+        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
+          port specific.  For a pin configured in such a way any other Pin methods
+          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
+          or a hardware-specific, result).  Not all ports implement this mode.
+
+        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
+          open-drain.  Not all ports implement this mode.
+
+        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
+
+      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
+        one of:
+
+        - ``None`` - No pull up or down resistor.
+        - ``Pin.PULL_UP`` - Pull up resistor enabled.
+        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
+
+      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
+        output pin value if given, otherwise the state of the pin peripheral remains
+        unchanged.
+
+      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
+        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
+        capabilities are port dependent.  Not all ports implement this argument.
+
+      - ``alt`` specifies an alternate function for the pin and the values it can take are
+        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
+        modes.  It may be used when a pin supports more than one alternate function.  If only
+        one pin alternate function is supported the this argument is not required.  Not all
+        ports implement this argument.
+
+    As specified above, the Pin class allows to set an alternate function for a particular
+    pin, but it does not specify any further operations on such a pin.  Pins configured in
+    alternate-function mode are usually not used as GPIO but are instead driven by other
+    hardware peripherals.  The only operation supported on such a pin is re-initialising,
+    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
+    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
+    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
+    """
+
+    OPEN_DRAIN: int
+    IRQ_FALLING: int
+    IRQ_RISING: int
+    PULL_UP: int
+    OUT: int
+    PULL_DOWN: int
+    WAKE_HIGH: int
+    DRIVE_0: int
+    IN: int
+    WAKE_LOW: int
+    DRIVE_3: int
+    DRIVE_1: int
+    DRIVE_2: int
+    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
+        """
+           Configure an interrupt handler to be called when the trigger source of the
+           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
+           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
+           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
+           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
+           state '0' and the external pin value for state '1'.
+
+           The arguments are:
+
+             - ``handler`` is an optional function to be called when the interrupt
+               triggers. The handler must take exactly one argument which is the
+               ``Pin`` instance.
+
+             - ``trigger`` configures the event which can generate an interrupt.
+               Possible values are:
+
+               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
+               - ``Pin.IRQ_RISING`` interrupt on rising edge.
+               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
+               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
+
+               These values can be OR'ed together to trigger on multiple events.
+
+             - ``priority`` sets the priority level of the interrupt.  The values it
+               can take are port-specific, but higher values always represent higher
+               priorities.
+
+             - ``wake`` selects the power mode in which this interrupt can wake up the
+               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
+               These values can also be OR'ed together to make a pin generate interrupts in
+               more than one power mode.
+
+             - ``hard`` if true a hardware interrupt is used. This reduces the delay
+               between the pin change and the handler being called. Hard interrupt
+               handlers may not allocate memory; see :ref:`isr_rules`.
+               Not all ports support this argument.
+
+           This method returns a callback object.
+
+        The following methods are not part of the core Pin API and only implemented on certain ports.
+        """
+        ...
+    def off(self) -> None:
+        """
+        Set pin to "0" output level.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Set pin to "1" output level.
+        """
+        ...
+    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
+        """
+        Re-initialise the pin using the given parameters.  Only those arguments that
+        are specified will be set.  The rest of the pin peripheral state will remain
+        unchanged.  See the constructor documentation for details of the arguments.
+
+        Returns ``None``.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the pin, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the digital logic level of
+        the pin, returning 0 or 1 corresponding to low and high voltage signals
+        respectively.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The method returns the actual input value currently present
+            on the pin.
+          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
+          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
+            return value of the method is undefined.  Otherwise, if the pin is in
+            state '1', the method returns the actual input value currently present
+            on the pin.
+
+        If the argument is supplied then this method sets the digital logic level of
+        the pin.  The argument ``x`` can be anything that converts to a boolean.
+        If it converts to ``True``, the pin is set to state '1', otherwise it is set
+        to state '0'.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
+            pin state does not change, it remains in the high-impedance state.  The
+            stored value will become active on the pin as soon as it is changed to
+            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
+          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
+          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
+            state.  Otherwise the pin is set to high-impedance state.
+
+        When setting the value this method returns ``None``.
+        """
+        ...
+    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
+    def __call__(self, x: Optional[Any] = None) -> Any:
+        """
+        Pin objects are callable.  The call method provides a (fast) shortcut to set
+        and get the value of the pin.  It is equivalent to Pin.value([x]).
+        See :meth:`Pin.value` for more details.
+        """
+        ...
+
+class TouchPad:
+    def config(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
+
+class WDT:
+    """
+    Create a WDT object and start it. The timeout must be given in milliseconds.
+    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
+
+    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
+    cannot be specified, it is determined by the underlying system. On rp2040 devices,
+    the maximum timeout is 8388 ms.
+    """
+
+    def feed(self) -> None:
+        """
+        Feed the WDT to prevent it from resetting the system. The application
+        should place this call in a sensible place ensuring that the WDT is
+        only fed after verifying that everything is functioning correctly.
+        """
+        ...
+    def __init__(self, id=0, timeout=5000) -> None: ...
+
+class SDCard:
+    """
+    This class provides access to SD or MMC storage cards using either
+    a dedicated SD/MMC interface hardware or through an SPI channel.
+    The class implements the block protocol defined by :class:`os.AbstractBlockDev`.
+    This allows the mounting of an SD card to be as simple as::
+
+      os.mount(machine.SDCard(), "/sd")
+
+    The constructor takes the following parameters:
+
+     - *slot* selects which of the available interfaces to use. Leaving this
+       unset will select the default interface.
+
+     - *width* selects the bus width for the SD/MMC interface.
+
+     - *cd* can be used to specify a card-detect pin.
+
+     - *wp* can be used to specify a write-protect pin.
+
+     - *sck* can be used to specify an SPI clock pin.
+
+     - *miso* can be used to specify an SPI miso pin.
+
+     - *mosi* can be used to specify an SPI mosi pin.
+
+     - *cs* can be used to specify an SPI chip select pin.
+
+     - *freq* selects the SD/MMC interface frequency in Hz (only supported on the ESP32).
+    """
+
+    def ioctl(self, *args, **kwargs) -> Any: ...
+    def readblocks(self, *args, **kwargs) -> Any: ...
+    def writeblocks(self, *args, **kwargs) -> Any: ...
+    def info(self, *args, **kwargs) -> Any: ...
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def __init__(self, slot=1, width=1, cd=None, wp=None, sck=None, miso=None, mosi=None, cs=None, freq=20000000) -> None: ...
+
+class RTC:
+    """
+    Create an RTC object. See init for parameters of initialization.
+    """
+
+    def init(self, datetime) -> None:
+        """
+        Initialise the RTC. Datetime is a tuple of the form:
+
+           ``(year, month, day[, hour[, minute[, second[, microsecond[, tzinfo]]]]])``
+        """
+        ...
+    def memory(self, *args, **kwargs) -> Any: ...
+    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
+        """
+        Get or set the date and time of the RTC.
+
+        With no arguments, this method returns an 8-tuple with the current
+        date and time.  With 1 argument (being an 8-tuple) it sets the date
+        and time.
+
+        The 8-tuple has the following format:
+
+            (year, month, day, weekday, hours, minutes, seconds, subseconds)
+
+        The meaning of the ``subseconds`` field is hardware dependent.
+        """
+        ...
+    def __init__(self, id=0, *args, **kwargs) -> None: ...
+
+class SoftI2C(I2C):
+    """
+    Construct a new software I2C object.  The parameters are:
+
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to wait for clock
+         stretching (SCL held low by another device on the bus), after
+         which an ``OSError(ETIMEDOUT)`` exception is raised.
+    """
+
+    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_mem(self, *args, **kwargs) -> Any: ...
+    def writeto_mem(self, *args, **kwargs) -> Any: ...
+    def scan(self, *args, **kwargs) -> Any: ...
+    def writeto(self, *args, **kwargs) -> Any: ...
+    def writevto(self, *args, **kwargs) -> Any: ...
+    def start(self, *args, **kwargs) -> Any: ...
+    def readfrom(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def stop(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
+
+class SPI:
+    """
+    Construct an SPI object on the given bus, *id*. Values of *id* depend
+    on a particular port and its hardware. Values 0, 1, etc. are commonly used
+    to select hardware SPI block #0, #1, etc.
+
+    With no additional parameters, the SPI object is created but not
+    initialised (it has the settings from the last initialisation of
+    the bus, if any).  If extra arguments are given, the bus is initialised.
+    See ``init`` for parameters of initialisation.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self) -> None:
+        """
+        Turn off the SPI bus.
+        """
+        ...
+    def init(
+        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
+    ) -> None:
+        """
+        Initialise the SPI bus with the given parameters:
+
+          - ``baudrate`` is the SCK clock rate.
+          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
+          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
+            respectively.
+          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
+          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
+          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
+            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
+            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
+            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
+            (``id`` = -1).
+          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
+            specify them as a tuple of ``pins`` parameter.
+
+        In the case of hardware SPI the actual clock frequency may be lower than the
+        requested baudrate. This is dependant on the platform hardware. The actual
+        rate may be determined by printing the SPI object.
+        """
+        ...
+    def write_readinto(self, write_buf, read_buf) -> int:
+        """
+        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
+        buffers can be the same or different, but both buffers must have the
+        same length.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def read(self, nbytes, write=0x00) -> bytes:
+        """
+        Read a number of bytes specified by ``nbytes`` while continuously writing
+        the single byte given by ``write``.
+        Returns a ``bytes`` object with the data that was read.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes contained in ``buf``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def readinto(self, buf, write=0x00) -> int:
+        """
+        Read into the buffer specified by ``buf`` while continuously writing the
+        single byte given by ``write``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes read.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+class Signal(Pin):
+    """
+            Signal(pin_arguments..., *, invert=False)
+
+    Create a Signal object. There're two ways to create it:
+
+    * By wrapping existing Pin object - universal method which works for
+      any board.
+    * By passing required Pin parameters directly to Signal constructor,
+      skipping the need to create intermediate Pin object. Available on
+      many, but not all boards.
+
+    The arguments are:
+
+      - ``pin_obj`` is existing Pin object.
+
+      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
+
+      - ``invert`` - if True, the signal will be inverted (active low).
+    """
+
+    def off(self) -> None:
+        """
+        Deactivate signal.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Activate signal.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the signal, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the signal level, 1 meaning
+        signal is asserted (active) and 0 - signal inactive.
+
+        If the argument is supplied then this method sets the signal level. The
+        argument ``x`` can be anything that converts to a boolean. If it converts
+        to ``True``, the signal is active, otherwise it is inactive.
+
+        Correspondence between signal being active and actual logic level on the
+        underlying pin depends on whether signal is inverted (active-low) or not.
+        For non-inverted signal, active status corresponds to logical 1, inactive -
+        to logical 0. For inverted/active-low signal, active status corresponds
+        to logical 0, while inactive - to logical 1.
+        """
+        ...
+    def __init__(self, pin_obj, *args, invert=False) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/umqtt/simple.pyi` & `micropython_esp32_stubs-1.20.0.post1/_thread.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from typing import Any
-
-def hexlify(*args, **kwargs) -> Any: ...
-
-class MQTTClient:
-    def ping(self, *args, **kwargs) -> Any: ...
-    def publish(self, *args, **kwargs) -> Any: ...
-    def wait_msg(self, *args, **kwargs) -> Any: ...
-    def subscribe(self, *args, **kwargs) -> Any: ...
-    def check_msg(self, *args, **kwargs) -> Any: ...
-    def set_last_will(self, *args, **kwargs) -> Any: ...
-    def connect(self, *args, **kwargs) -> Any: ...
-    def disconnect(self, *args, **kwargs) -> Any: ...
-    def set_callback(self, *args, **kwargs) -> Any: ...
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class MQTTException(Exception): ...
+"""
+multithreading support. See: https://docs.micropython.org/en/v1.20.0/library/_thread.html
+
+|see_cpython_module| :mod:`python:_thread` https://docs.python.org/3/library/_thread.html .
+
+This module implements multithreading support.
+
+This module is highly experimental and its API is not yet fully settled
+and not yet described in this documentation.
+"""
+from typing import Any
+
+def get_ident(*args, **kwargs) -> Any: ...
+def start_new_thread(*args, **kwargs) -> Any: ...
+def stack_size(*args, **kwargs) -> Any: ...
+def exit(*args, **kwargs) -> Any: ...
+def allocate_lock(*args, **kwargs) -> Any: ...
+
+class LockType:
+    def locked(self, *args, **kwargs) -> Any: ...
+    def release(self, *args, **kwargs) -> Any: ...
+    def acquire(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/uos.pyi` & `micropython_esp32_stubs-1.20.0.post1/uos.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,245 +1,245 @@
-"""
-basic "operating system" services. See: https://docs.micropython.org/en/v1.19.1/library/os.html
-
-|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
-
-The ``os`` module contains functions for filesystem access and mounting,
-terminal redirection and duplication, and the ``uname`` and ``urandom``
-functions.
-"""
-from typing import IO, Iterator, Optional, Tuple, Any
-from stdlib.os import uname_result
-
-def stat(path) -> Any:
-    """
-    Get the status of a file or directory.
-    """
-    ...
-
-def rmdir(path) -> None:
-    """
-    Remove a directory.
-    """
-    ...
-
-def rename(old_path, new_path) -> None:
-    """
-    Rename a file.
-    """
-    ...
-
-def mount(fsobj, mount_point, *, readonly) -> Any:
-    """
-    Mount the filesystem object *fsobj* at the location in the VFS given by the
-    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
-    method, or a block device.  If it's a block device then the filesystem type
-    is automatically detected (an exception is raised if no filesystem was
-    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
-    or ``'/<name>'`` to mount it at a subdirectory under the root.
-
-    If *readonly* is ``True`` then the filesystem is mounted read-only.
-
-    During the mount process the method ``mount()`` is called on the filesystem
-    object.
-
-    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
-    """
-    ...
-
-def mkdir(path) -> Any:
-    """
-    Create a new directory.
-    """
-    ...
-
-def statvfs(path) -> Tuple:
-    """
-    Get the status of a fileystem.
-
-    Returns a tuple with the filesystem information in the following order:
-
-         * ``f_bsize`` -- file system block size
-         * ``f_frsize`` -- fragment size
-         * ``f_blocks`` -- size of fs in f_frsize units
-         * ``f_bfree`` -- number of free blocks
-         * ``f_bavail`` -- number of free blocks for unprivileged users
-         * ``f_files`` -- number of inodes
-         * ``f_ffree`` -- number of free inodes
-         * ``f_favail`` -- number of free inodes for unprivileged users
-         * ``f_flag`` -- mount flags
-         * ``f_namemax`` -- maximum filename length
-
-    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
-    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
-    in a port-specific implementation.
-    """
-    ...
-
-def unlink(*args, **kwargs) -> Any: ...
-def uname() -> uname_result:
-    """
-    Return a tuple (possibly a named tuple) containing information about the
-    underlying machine and/or its operating system.  The tuple has five fields
-    in the following order, each of them being a string:
-
-         * ``sysname`` -- the name of the underlying system
-         * ``nodename`` -- the network name (can be the same as ``sysname``)
-         * ``release`` -- the version of the underlying system
-         * ``version`` -- the MicroPython version and build date
-         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
-    """
-    ...
-
-def umount(mount_point) -> Any:
-    """
-    Unmount a filesystem. *mount_point* can be a string naming the mount location,
-    or a previously-mounted filesystem object.  During the unmount process the
-    method ``umount()`` is called on the filesystem object.
-
-    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
-    """
-    ...
-
-def urandom(n) -> bytes:
-    """
-    Return a bytes object with *n* random bytes. Whenever possible, it is
-    generated by the hardware random number generator.
-    """
-    ...
-
-def chdir(path) -> Any:
-    """
-    Change current directory.
-    """
-    ...
-
-def dupterm(stream_object, index=0, /) -> IO:
-    """
-    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
-    object. The *stream_object* argument must be a native stream object, or derive
-    from ``io.IOBase`` and implement the ``readinto()`` and
-    ``write()`` methods.  The stream should be in non-blocking mode and
-    ``readinto()`` should return ``None`` if there is no data available for reading.
-
-    After calling this function all terminal output is repeated on this stream,
-    and any input that is available on the stream is passed on to the terminal input.
-
-    The *index* parameter should be a non-negative integer and specifies which
-    duplication slot is set.  A given port may implement more than one slot (slot 0
-    will always be available) and in that case terminal input and output is
-    duplicated on all the slots that are set.
-
-    If ``None`` is passed as the *stream_object* then duplication is cancelled on
-    the slot given by *index*.
-
-    The function returns the previous stream-like object in the given slot.
-    """
-    ...
-
-def remove(path) -> None:
-    """
-    Remove a file.
-    """
-    ...
-
-def listdir(dir: Optional[Any] = None) -> Any:
-    """
-    With no argument, list the current directory.  Otherwise list the given directory.
-    """
-    ...
-
-def dupterm_notify(*args, **kwargs) -> Any: ...
-def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
-    """
-    This function returns an iterator which then yields tuples corresponding to
-    the entries in the directory that it is listing.  With no argument it lists the
-    current directory, otherwise it lists the directory given by *dir*.
-
-    The tuples have the form *(name, type, inode[, size])*:
-
-     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
-       the entry;
-     - *type* is an integer that specifies the type of the entry, with 0x4000 for
-       directories and 0x8000 for regular files;
-     - *inode* is an integer corresponding to the inode of the file, and may be 0
-       for filesystems that don't have such a notion.
-     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
-       file entries, *size* is an integer representing the size of the file
-       or -1 if unknown.  Its meaning is currently undefined for directory
-       entries.
-    """
-    ...
-
-def getcwd() -> Any:
-    """
-    Get the current directory.
-    """
-    ...
-
-class VfsLfs2:
-    """
-    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
-    Storage of the littlefs filesystem is provided by *block_dev*, which must
-    support the :ref:`extended interface <block-device-interface>`.
-    Objects created by this constructor can be mounted using :func:`mount`.
-
-    The *mtime* argument enables modification timestamps for files, stored using
-    littlefs attributes.  This option can be disabled or enabled differently each
-    mount time and timestamps will only be added or updated if *mtime* is enabled,
-    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
-    timestamps will work without reformatting and timestamps will be added
-    transparently to existing files once they are opened for writing.  When *mtime*
-    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
-
-    See :ref:`filesystem` for more information.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
-        """
-            Build a Lfs2 filesystem on *block_dev*.
-
-        ``Note:`` There are reports of littlefs v2 failing in certain situations,
-                  for details see `littlefs issue 295`_.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
-
-class VfsFat:
-    """
-    Create a filesystem object that uses the FAT filesystem format.  Storage of
-    the FAT filesystem is provided by *block_dev*.
-    Objects created by this constructor can be mounted using :func:`mount`.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev) -> None:
-        """
-        Build a FAT filesystem on *block_dev*.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev) -> None: ...
+"""
+basic "operating system" services. See: https://docs.micropython.org/en/v1.20.0/library/os.html
+
+|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
+
+The ``os`` module contains functions for filesystem access and mounting,
+terminal redirection and duplication, and the ``uname`` and ``urandom``
+functions.
+"""
+from typing import IO, Iterator, Optional, Tuple, Any
+from stdlib.os import uname_result
+
+def stat(path) -> Any:
+    """
+    Get the status of a file or directory.
+    """
+    ...
+
+def rmdir(path) -> None:
+    """
+    Remove a directory.
+    """
+    ...
+
+def rename(old_path, new_path) -> None:
+    """
+    Rename a file.
+    """
+    ...
+
+def mount(fsobj, mount_point, *, readonly) -> Any:
+    """
+    Mount the filesystem object *fsobj* at the location in the VFS given by the
+    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
+    method, or a block device.  If it's a block device then the filesystem type
+    is automatically detected (an exception is raised if no filesystem was
+    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
+    or ``'/<name>'`` to mount it at a subdirectory under the root.
+
+    If *readonly* is ``True`` then the filesystem is mounted read-only.
+
+    During the mount process the method ``mount()`` is called on the filesystem
+    object.
+
+    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
+    """
+    ...
+
+def mkdir(path) -> Any:
+    """
+    Create a new directory.
+    """
+    ...
+
+def statvfs(path) -> Tuple:
+    """
+    Get the status of a fileystem.
+
+    Returns a tuple with the filesystem information in the following order:
+
+         * ``f_bsize`` -- file system block size
+         * ``f_frsize`` -- fragment size
+         * ``f_blocks`` -- size of fs in f_frsize units
+         * ``f_bfree`` -- number of free blocks
+         * ``f_bavail`` -- number of free blocks for unprivileged users
+         * ``f_files`` -- number of inodes
+         * ``f_ffree`` -- number of free inodes
+         * ``f_favail`` -- number of free inodes for unprivileged users
+         * ``f_flag`` -- mount flags
+         * ``f_namemax`` -- maximum filename length
+
+    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
+    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
+    in a port-specific implementation.
+    """
+    ...
+
+def unlink(*args, **kwargs) -> Any: ...
+def uname() -> uname_result:
+    """
+    Return a tuple (possibly a named tuple) containing information about the
+    underlying machine and/or its operating system.  The tuple has five fields
+    in the following order, each of them being a string:
+
+         * ``sysname`` -- the name of the underlying system
+         * ``nodename`` -- the network name (can be the same as ``sysname``)
+         * ``release`` -- the version of the underlying system
+         * ``version`` -- the MicroPython version and build date
+         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
+    """
+    ...
+
+def umount(mount_point) -> Any:
+    """
+    Unmount a filesystem. *mount_point* can be a string naming the mount location,
+    or a previously-mounted filesystem object.  During the unmount process the
+    method ``umount()`` is called on the filesystem object.
+
+    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
+    """
+    ...
+
+def urandom(n) -> bytes:
+    """
+    Return a bytes object with *n* random bytes. Whenever possible, it is
+    generated by the hardware random number generator.
+    """
+    ...
+
+def chdir(path) -> Any:
+    """
+    Change current directory.
+    """
+    ...
+
+def dupterm(stream_object, index=0, /) -> IO:
+    """
+    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
+    object. The *stream_object* argument must be a native stream object, or derive
+    from ``io.IOBase`` and implement the ``readinto()`` and
+    ``write()`` methods.  The stream should be in non-blocking mode and
+    ``readinto()`` should return ``None`` if there is no data available for reading.
+
+    After calling this function all terminal output is repeated on this stream,
+    and any input that is available on the stream is passed on to the terminal input.
+
+    The *index* parameter should be a non-negative integer and specifies which
+    duplication slot is set.  A given port may implement more than one slot (slot 0
+    will always be available) and in that case terminal input and output is
+    duplicated on all the slots that are set.
+
+    If ``None`` is passed as the *stream_object* then duplication is cancelled on
+    the slot given by *index*.
+
+    The function returns the previous stream-like object in the given slot.
+    """
+    ...
+
+def remove(path) -> None:
+    """
+    Remove a file.
+    """
+    ...
+
+def listdir(dir: Optional[Any] = None) -> Any:
+    """
+    With no argument, list the current directory.  Otherwise list the given directory.
+    """
+    ...
+
+def dupterm_notify(*args, **kwargs) -> Any: ...
+def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
+    """
+    This function returns an iterator which then yields tuples corresponding to
+    the entries in the directory that it is listing.  With no argument it lists the
+    current directory, otherwise it lists the directory given by *dir*.
+
+    The tuples have the form *(name, type, inode[, size])*:
+
+     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
+       the entry;
+     - *type* is an integer that specifies the type of the entry, with 0x4000 for
+       directories and 0x8000 for regular files;
+     - *inode* is an integer corresponding to the inode of the file, and may be 0
+       for filesystems that don't have such a notion.
+     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
+       file entries, *size* is an integer representing the size of the file
+       or -1 if unknown.  Its meaning is currently undefined for directory
+       entries.
+    """
+    ...
+
+def getcwd() -> Any:
+    """
+    Get the current directory.
+    """
+    ...
+
+class VfsLfs2:
+    """
+    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
+    Storage of the littlefs filesystem is provided by *block_dev*, which must
+    support the :ref:`extended interface <block-device-interface>`.
+    Objects created by this constructor can be mounted using :func:`mount`.
+
+    The *mtime* argument enables modification timestamps for files, stored using
+    littlefs attributes.  This option can be disabled or enabled differently each
+    mount time and timestamps will only be added or updated if *mtime* is enabled,
+    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
+    timestamps will work without reformatting and timestamps will be added
+    transparently to existing files once they are opened for writing.  When *mtime*
+    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
+
+    See :ref:`filesystem` for more information.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
+        """
+            Build a Lfs2 filesystem on *block_dev*.
+
+        ``Note:`` There are reports of littlefs v2 failing in certain situations,
+                  for details see `littlefs issue 295`_.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
+
+class VfsFat:
+    """
+    Create a filesystem object that uses the FAT filesystem format.  Storage of
+    the FAT filesystem is provided by *block_dev*.
+    Objects created by this constructor can be mounted using :func:`mount`.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev) -> None:
+        """
+        Build a FAT filesystem on *block_dev*.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/upip_utarfile.pyi` & `micropython_esp32_stubs-1.20.0.post1/uasyncio/task.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from _typeshed import Incomplete
-
-TAR_HEADER: Incomplete
-DIRTYPE: str
-REGTYPE: str
-
-def roundup(val, align): ...
-
-class FileSection:
-    f: Incomplete
-    content_len: Incomplete
-    align: Incomplete
-    def __init__(self, f, content_len, aligned_len) -> None: ...
-    def read(self, sz: int = ...): ...
-    def readinto(self, buf): ...
-    def skip(self) -> None: ...
-
-class TarInfo:
-    def __str__(self): ...
-
-class TarFile:
-    f: Incomplete
-    subf: Incomplete
-    def __init__(self, name: Incomplete | None = ..., fileobj: Incomplete | None = ...) -> None: ...
-    def next(self): ...
-    def __iter__(self): ...
-    def __next__(self): ...
-    def extractfile(self, tarinfo): ...
+from . import core as core
+from _typeshed import Incomplete
+
+def ph_meld(h1, h2): ...
+def ph_pairing(child): ...
+def ph_delete(heap, node): ...
+
+class TaskQueue:
+    heap: Incomplete
+    def __init__(self) -> None: ...
+    def peek(self): ...
+    def push(self, v, key: Incomplete | None = ...) -> None: ...
+    def pop(self): ...
+    def remove(self, v) -> None: ...
+
+class Task:
+    coro: Incomplete
+    data: Incomplete
+    state: bool
+    ph_key: int
+    ph_child: Incomplete
+    ph_child_last: Incomplete
+    ph_next: Incomplete
+    ph_rightmost_parent: Incomplete
+    def __init__(self, coro, globals: Incomplete | None = ...) -> None: ...
+    def __iter__(self): ...
+    def __next__(self) -> None: ...
+    def done(self): ...
+    def cancel(self): ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/uselect.pyi` & `micropython_esp32_stubs-1.20.0.post1/uselect.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-"""
-wait for events on a set of streams. See: https://docs.micropython.org/en/v1.19.1/library/select.html
-
-|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
-
-This module provides functions to efficiently wait for events on multiple
-`streams <stream>` (select streams which are ready for operations).
-"""
-from typing import Iterator, List, Optional, Tuple, Any
-
-POLLOUT: int
-POLLIN: int
-POLLHUP: int
-POLLERR: int
-
-class select:
-    """
-    Wait for activity on a set of objects.
-
-    This function is provided by some MicroPython ports for compatibility
-    and is not efficient. Usage of :class:`Poll` is recommended instead.
-    """
-
-    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
-
-class poll:
-    """
-    Create an instance of the Poll class.
-    """
-
-    def __init__(self) -> None: ...
-    def register(self, obj, eventmask: Optional[Any] = None) -> None:
-        """
-        Register `stream` *obj* for polling. *eventmask* is logical OR of:
-
-        * ``select.POLLIN``  - data available for reading
-        * ``select.POLLOUT`` - more data can be written
-
-        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
-        *not* valid as input eventmask (these are unsolicited events which
-        will be returned from `poll()` regardless of whether they are asked
-        for). This semantics is per POSIX.
-
-        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
-
-        It is OK to call this function multiple times for the same *obj*.
-        Successive calls will update *obj*'s eventmask to the value of
-        *eventmask* (i.e. will behave as `modify()`).
-        """
-        ...
-    def unregister(self, obj) -> Any:
-        """
-        Unregister *obj* from polling.
-        """
-        ...
-    def modify(self, obj, eventmask) -> None:
-        """
-        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
-        is raised with error of ENOENT.
-        """
-        ...
-    def poll(self, timeout=-1, /) -> List:
-        """
-        Wait for at least one of the registered objects to become ready or have an
-        exceptional condition, with optional timeout in milliseconds (if *timeout*
-        arg is not specified or -1, there is no timeout).
-
-        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
-        tuple, depending on a platform and version, so don't assume that its size is 2.
-        The ``event`` element specifies which events happened with a stream and
-        is a combination of ``select.POLL*`` constants described above. Note that
-        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
-        (even if were not asked for), and must be acted on accordingly (the
-        corresponding stream unregistered from poll and likely closed), because
-        otherwise all further invocations of `poll()` may return immediately with
-        these flags set for this stream again.
-
-        In case of timeout, an empty list is returned.
-        """
-        ...
-    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
-        """
-        Like :meth:`poll.poll`, but instead returns an iterator which yields a
-        `callee-owned tuple`. This function provides an efficient, allocation-free
-        way to poll on streams.
-
-        If *flags* is 1, one-shot behaviour for events is employed: streams for
-        which events happened will have their event masks automatically reset
-        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
-        won't be processed until new mask is set with `poll.modify()`. This
-        behaviour is useful for asynchronous I/O schedulers.
-        """
-        ...
+"""
+wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20.0/library/select.html
+
+|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
+
+This module provides functions to efficiently wait for events on multiple
+`streams <stream>` (select streams which are ready for operations).
+"""
+from typing import Iterator, List, Optional, Tuple, Any
+
+POLLOUT: int
+POLLIN: int
+POLLHUP: int
+POLLERR: int
+
+class select:
+    """
+    Wait for activity on a set of objects.
+
+    This function is provided by some MicroPython ports for compatibility
+    and is not efficient. Usage of :class:`Poll` is recommended instead.
+    """
+
+    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
+
+class poll:
+    """
+    Create an instance of the Poll class.
+    """
+
+    def __init__(self) -> None: ...
+    def register(self, obj, eventmask: Optional[Any] = None) -> None:
+        """
+        Register `stream` *obj* for polling. *eventmask* is logical OR of:
+
+        * ``select.POLLIN``  - data available for reading
+        * ``select.POLLOUT`` - more data can be written
+
+        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
+        *not* valid as input eventmask (these are unsolicited events which
+        will be returned from `poll()` regardless of whether they are asked
+        for). This semantics is per POSIX.
+
+        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
+
+        It is OK to call this function multiple times for the same *obj*.
+        Successive calls will update *obj*'s eventmask to the value of
+        *eventmask* (i.e. will behave as `modify()`).
+        """
+        ...
+    def unregister(self, obj) -> Any:
+        """
+        Unregister *obj* from polling.
+        """
+        ...
+    def modify(self, obj, eventmask) -> None:
+        """
+        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
+        is raised with error of ENOENT.
+        """
+        ...
+    def poll(self, timeout=-1, /) -> List:
+        """
+        Wait for at least one of the registered objects to become ready or have an
+        exceptional condition, with optional timeout in milliseconds (if *timeout*
+        arg is not specified or -1, there is no timeout).
+
+        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
+        tuple, depending on a platform and version, so don't assume that its size is 2.
+        The ``event`` element specifies which events happened with a stream and
+        is a combination of ``select.POLL*`` constants described above. Note that
+        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
+        (even if were not asked for), and must be acted on accordingly (the
+        corresponding stream unregistered from poll and likely closed), because
+        otherwise all further invocations of `poll()` may return immediately with
+        these flags set for this stream again.
+
+        In case of timeout, an empty list is returned.
+        """
+        ...
+    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
+        """
+        Like :meth:`poll.poll`, but instead returns an iterator which yields a
+        `callee-owned tuple`. This function provides an efficient, allocation-free
+        way to poll on streams.
+
+        If *flags* is 1, one-shot behaviour for events is employed: streams for
+        which events happened will have their event masks automatically reset
+        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
+        won't be processed until new mask is set with `poll.modify()`. This
+        behaviour is useful for asynchronous I/O schedulers.
+        """
+        ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/usocket.pyi` & `micropython_esp32_stubs-1.20.0.post1/usocket.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-"""
-socket module. See: https://docs.micropython.org/en/v1.19.1/library/socket.html
-
-|see_cpython_module| :mod:`python:socket` https://docs.python.org/3/library/socket.html .
-
-This module provides access to the BSD socket interface.
-"""
-from typing import IO, Optional, Tuple, Any
-
-SOCK_RAW: int
-SOCK_DGRAM: int
-IP_ADD_MEMBERSHIP: int
-SOCK_STREAM: int
-SOL_SOCKET: int
-SO_REUSEADDR: int
-AF_INET6: int
-AF_INET: int
-IPPROTO_UDP: int
-IPPROTO_IP: int
-IPPROTO_TCP: int
-
-def getaddrinfo(host, port, af=0, type=0, proto=0, flags=0, /) -> Any:
-    """
-    Translate the host/port argument into a sequence of 5-tuples that contain all the
-    necessary arguments for creating a socket connected to that service. Arguments
-    *af*, *type*, and *proto* (which have the same meaning as for the `socket()` function)
-    can be used to filter which kind of addresses are returned. If a parameter is not
-    specified or zero, all combinations of addresses can be returned (requiring
-    filtering on the user side).
-
-    The resulting list of 5-tuples has the following structure::
-
-       (family, type, proto, canonname, sockaddr)
-
-    The following example shows how to connect to a given url::
-
-       s = socket.socket()
-       # This assumes that if "type" is not specified, an address for
-       # SOCK_STREAM will be returned, which may be not true
-       s.connect(socket.getaddrinfo('www.micropython.org', 80)[0][-1])
-
-    Recommended use of filtering params::
-
-       s = socket.socket()
-       # Guaranteed to return an address which can be connect'ed to for
-       # stream operation.
-       s.connect(socket.getaddrinfo('www.micropython.org', 80, 0, SOCK_STREAM)[0][-1])
-    """
-    ...
-
-class socket:
-    """
-    Create a new socket using the given address family, socket type and
-    protocol number. Note that specifying *proto* in most cases is not
-    required (and not recommended, as some MicroPython ports may omit
-    ``IPPROTO_*`` constants). Instead, *type* argument will select needed
-    protocol automatically::
-
-         # Create STREAM TCP socket
-         socket(AF_INET, SOCK_STREAM)
-         # Create DGRAM UDP socket
-         socket(AF_INET, SOCK_DGRAM)
-    """
-
-    def recvfrom(self, bufsize) -> Tuple:
-        """
-        Receive data from the socket. The return value is a pair *(bytes, address)* where *bytes* is a
-        bytes object representing the data received and *address* is the address of the socket sending
-        the data.
-        """
-        ...
-    def recv(self, bufsize) -> bytes:
-        """
-        Receive data from the socket. The return value is a bytes object representing the data
-        received. The maximum amount of data to be received at once is specified by bufsize.
-        """
-        ...
-    def makefile(self, mode="rb", buffering=0, /) -> IO:
-        """
-        Return a file object associated with the socket. The exact returned type depends on the arguments
-        given to makefile(). The support is limited to binary modes only ('rb', 'wb', and 'rwb').
-        CPython's arguments: *encoding*, *errors* and *newline* are not supported.
-        """
-        ...
-    def listen(self, backlog: Optional[Any] = None) -> None:
-        """
-        Enable a server to accept connections. If *backlog* is specified, it must be at least 0
-        (if it's lower, it will be set to 0); and specifies the number of unaccepted connections
-        that the system will allow before refusing new connections. If not specified, a default
-        reasonable value is chosen.
-        """
-        ...
-    def fileno(self, *args, **kwargs) -> Any: ...
-    def sendall(self, bytes) -> int:
-        """
-        Send all data to the socket. The socket must be connected to a remote socket.
-        Unlike `send()`, this method will try to send all of data, by sending data
-        chunk by chunk consecutively.
-
-        The behaviour of this method on non-blocking sockets is undefined. Due to this,
-        on MicroPython, it's recommended to use `write()` method instead, which
-        has the same "no short writes" policy for blocking sockets, and will return
-        number of bytes sent on non-blocking sockets.
-        """
-        ...
-    def setsockopt(self, level, optname, value) -> None:
-        """
-        Set the value of the given socket option. The needed symbolic constants are defined in the
-        socket module (SO_* etc.). The *value* can be an integer or a bytes-like object representing
-        a buffer.
-        """
-        ...
-    def setblocking(self, flag) -> Any:
-        """
-        Set blocking or non-blocking mode of the socket: if flag is false, the socket is set to non-blocking,
-        else to blocking mode.
-
-        This method is a shorthand for certain `settimeout()` calls:
-
-        * ``sock.setblocking(True)`` is equivalent to ``sock.settimeout(None)``
-        * ``sock.setblocking(False)`` is equivalent to ``sock.settimeout(0)``
-        """
-        ...
-    def sendto(self, bytes, address) -> None:
-        """
-        Send data to the socket. The socket should not be connected to a remote socket, since the
-        destination socket is specified by *address*.
-        """
-        ...
-    def settimeout(self, value) -> Any:
-        """
-        **Note**: Not every port supports this method, see below.
-
-        Set a timeout on blocking socket operations. The value argument can be a nonnegative floating
-        point number expressing seconds, or None. If a non-zero value is given, subsequent socket operations
-        will raise an `OSError` exception if the timeout period value has elapsed before the operation has
-        completed. If zero is given, the socket is put in non-blocking mode. If None is given, the socket
-        is put in blocking mode.
-
-        Not every :term:`MicroPython port` supports this method. A more portable and
-        generic solution is to use `select.poll` object. This allows to wait on
-        multiple objects at the same time (and not just on sockets, but on generic
-        `stream` objects which support polling). Example::
-
-             # Instead of:
-             s.settimeout(1.0)  # time in seconds
-             s.read(10)  # may timeout
-
-             # Use:
-             poller = select.poll()
-             poller.register(s, select.POLLIN)
-             res = poller.poll(1000)  # time in milliseconds
-             if not res:
-                 # s is still not ready for input, i.e. operation timed out
-        """
-        ...
-    def readline(self) -> Any:
-        """
-        Read a line, ending in a newline character.
-
-        Return value: the line read.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the *buf*.  If *nbytes* is specified then read at most
-        that many bytes.  Otherwise, read at most *len(buf)* bytes. Just as
-        `read()`, this method follows "no short reads" policy.
-
-        Return value: number of bytes read and stored into *buf*.
-        """
-        ...
-    def read(self, size: Optional[Any] = None) -> bytes:
-        """
-        Read up to size bytes from the socket. Return a bytes object. If *size* is not given, it
-        reads all data available from the socket until EOF; as such the method will not return until
-        the socket is closed. This function tries to read as much data as
-        requested (no "short reads"). This may be not possible with
-        non-blocking socket though, and then less data will be returned.
-        """
-        ...
-    def close(self) -> Any:
-        """
-        Mark the socket closed and release all resources. Once that happens, all future operations
-        on the socket object will fail. The remote end will receive EOF indication if
-        supported by protocol.
-
-        Sockets are automatically closed when they are garbage-collected, but it is recommended
-        to `close()` them explicitly as soon you finished working with them.
-        """
-        ...
-    def connect(self, address) -> None:
-        """
-        Connect to a remote socket at *address*.
-        """
-        ...
-    def send(self, bytes) -> int:
-        """
-        Send data to the socket. The socket must be connected to a remote socket.
-        Returns number of bytes sent, which may be smaller than the length of data
-        ("short write").
-        """
-        ...
-    def bind(self, address) -> Any:
-        """
-        Bind the socket to *address*. The socket must not already be bound.
-        """
-        ...
-    def accept(self) -> Tuple:
-        """
-        Accept a connection. The socket must be bound to an address and listening for connections.
-        The return value is a pair (conn, address) where conn is a new socket object usable to send
-        and receive data on the connection, and address is the address bound to the socket on the
-        other end of the connection.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the socket. This function will try to
-        write all data to a socket (no "short writes"). This may be not possible
-        with a non-blocking socket though, and returned value will be less than
-        the length of *buf*.
-
-        Return value: number of bytes written.
-        """
-        ...
-    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None: ...
+"""
+socket module. See: https://docs.micropython.org/en/v1.20.0/library/socket.html
+
+|see_cpython_module| :mod:`python:socket` https://docs.python.org/3/library/socket.html .
+
+This module provides access to the BSD socket interface.
+"""
+from typing import IO, Optional, Tuple, Any
+
+SOCK_RAW: int
+SOCK_DGRAM: int
+IP_ADD_MEMBERSHIP: int
+SOCK_STREAM: int
+SOL_SOCKET: int
+SO_REUSEADDR: int
+AF_INET6: int
+AF_INET: int
+IPPROTO_UDP: int
+IPPROTO_IP: int
+IPPROTO_TCP: int
+
+def getaddrinfo(host, port, af=0, type=0, proto=0, flags=0, /) -> Any:
+    """
+    Translate the host/port argument into a sequence of 5-tuples that contain all the
+    necessary arguments for creating a socket connected to that service. Arguments
+    *af*, *type*, and *proto* (which have the same meaning as for the `socket()` function)
+    can be used to filter which kind of addresses are returned. If a parameter is not
+    specified or zero, all combinations of addresses can be returned (requiring
+    filtering on the user side).
+
+    The resulting list of 5-tuples has the following structure::
+
+       (family, type, proto, canonname, sockaddr)
+
+    The following example shows how to connect to a given url::
+
+       s = socket.socket()
+       # This assumes that if "type" is not specified, an address for
+       # SOCK_STREAM will be returned, which may be not true
+       s.connect(socket.getaddrinfo('www.micropython.org', 80)[0][-1])
+
+    Recommended use of filtering params::
+
+       s = socket.socket()
+       # Guaranteed to return an address which can be connect'ed to for
+       # stream operation.
+       s.connect(socket.getaddrinfo('www.micropython.org', 80, 0, SOCK_STREAM)[0][-1])
+    """
+    ...
+
+class socket:
+    """
+    Create a new socket using the given address family, socket type and
+    protocol number. Note that specifying *proto* in most cases is not
+    required (and not recommended, as some MicroPython ports may omit
+    ``IPPROTO_*`` constants). Instead, *type* argument will select needed
+    protocol automatically::
+
+         # Create STREAM TCP socket
+         socket(AF_INET, SOCK_STREAM)
+         # Create DGRAM UDP socket
+         socket(AF_INET, SOCK_DGRAM)
+    """
+
+    def recvfrom(self, bufsize) -> Tuple:
+        """
+        Receive data from the socket. The return value is a pair *(bytes, address)* where *bytes* is a
+        bytes object representing the data received and *address* is the address of the socket sending
+        the data.
+        """
+        ...
+    def recv(self, bufsize) -> bytes:
+        """
+        Receive data from the socket. The return value is a bytes object representing the data
+        received. The maximum amount of data to be received at once is specified by bufsize.
+        """
+        ...
+    def makefile(self, mode="rb", buffering=0, /) -> IO:
+        """
+        Return a file object associated with the socket. The exact returned type depends on the arguments
+        given to makefile(). The support is limited to binary modes only ('rb', 'wb', and 'rwb').
+        CPython's arguments: *encoding*, *errors* and *newline* are not supported.
+        """
+        ...
+    def listen(self, backlog: Optional[Any] = None) -> None:
+        """
+        Enable a server to accept connections. If *backlog* is specified, it must be at least 0
+        (if it's lower, it will be set to 0); and specifies the number of unaccepted connections
+        that the system will allow before refusing new connections. If not specified, a default
+        reasonable value is chosen.
+        """
+        ...
+    def fileno(self, *args, **kwargs) -> Any: ...
+    def sendall(self, bytes) -> int:
+        """
+        Send all data to the socket. The socket must be connected to a remote socket.
+        Unlike `send()`, this method will try to send all of data, by sending data
+        chunk by chunk consecutively.
+
+        The behaviour of this method on non-blocking sockets is undefined. Due to this,
+        on MicroPython, it's recommended to use `write()` method instead, which
+        has the same "no short writes" policy for blocking sockets, and will return
+        number of bytes sent on non-blocking sockets.
+        """
+        ...
+    def setsockopt(self, level, optname, value) -> None:
+        """
+        Set the value of the given socket option. The needed symbolic constants are defined in the
+        socket module (SO_* etc.). The *value* can be an integer or a bytes-like object representing
+        a buffer.
+        """
+        ...
+    def setblocking(self, flag) -> Any:
+        """
+        Set blocking or non-blocking mode of the socket: if flag is false, the socket is set to non-blocking,
+        else to blocking mode.
+
+        This method is a shorthand for certain `settimeout()` calls:
+
+        * ``sock.setblocking(True)`` is equivalent to ``sock.settimeout(None)``
+        * ``sock.setblocking(False)`` is equivalent to ``sock.settimeout(0)``
+        """
+        ...
+    def sendto(self, bytes, address) -> None:
+        """
+        Send data to the socket. The socket should not be connected to a remote socket, since the
+        destination socket is specified by *address*.
+        """
+        ...
+    def settimeout(self, value) -> Any:
+        """
+        **Note**: Not every port supports this method, see below.
+
+        Set a timeout on blocking socket operations. The value argument can be a nonnegative floating
+        point number expressing seconds, or None. If a non-zero value is given, subsequent socket operations
+        will raise an `OSError` exception if the timeout period value has elapsed before the operation has
+        completed. If zero is given, the socket is put in non-blocking mode. If None is given, the socket
+        is put in blocking mode.
+
+        Not every :term:`MicroPython port` supports this method. A more portable and
+        generic solution is to use `select.poll` object. This allows to wait on
+        multiple objects at the same time (and not just on sockets, but on generic
+        `stream` objects which support polling). Example::
+
+             # Instead of:
+             s.settimeout(1.0)  # time in seconds
+             s.read(10)  # may timeout
+
+             # Use:
+             poller = select.poll()
+             poller.register(s, select.POLLIN)
+             res = poller.poll(1000)  # time in milliseconds
+             if not res:
+                 # s is still not ready for input, i.e. operation timed out
+        """
+        ...
+    def readline(self) -> Any:
+        """
+        Read a line, ending in a newline character.
+
+        Return value: the line read.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the *buf*.  If *nbytes* is specified then read at most
+        that many bytes.  Otherwise, read at most *len(buf)* bytes. Just as
+        `read()`, this method follows "no short reads" policy.
+
+        Return value: number of bytes read and stored into *buf*.
+        """
+        ...
+    def read(self, size: Optional[Any] = None) -> bytes:
+        """
+        Read up to size bytes from the socket. Return a bytes object. If *size* is not given, it
+        reads all data available from the socket until EOF; as such the method will not return until
+        the socket is closed. This function tries to read as much data as
+        requested (no "short reads"). This may be not possible with
+        non-blocking socket though, and then less data will be returned.
+        """
+        ...
+    def close(self) -> Any:
+        """
+        Mark the socket closed and release all resources. Once that happens, all future operations
+        on the socket object will fail. The remote end will receive EOF indication if
+        supported by protocol.
+
+        Sockets are automatically closed when they are garbage-collected, but it is recommended
+        to `close()` them explicitly as soon you finished working with them.
+        """
+        ...
+    def connect(self, address) -> None:
+        """
+        Connect to a remote socket at *address*.
+        """
+        ...
+    def send(self, bytes) -> int:
+        """
+        Send data to the socket. The socket must be connected to a remote socket.
+        Returns number of bytes sent, which may be smaller than the length of data
+        ("short write").
+        """
+        ...
+    def bind(self, address) -> Any:
+        """
+        Bind the socket to *address*. The socket must not already be bound.
+        """
+        ...
+    def accept(self) -> Tuple:
+        """
+        Accept a connection. The socket must be bound to an address and listening for connections.
+        The return value is a pair (conn, address) where conn is a new socket object usable to send
+        and receive data on the connection, and address is the address bound to the socket on the
+        other end of the connection.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the socket. This function will try to
+        write all data to a socket (no "short writes"). This may be not possible
+        with a non-blocking socket though, and returned value will be less than
+        the length of *buf*.
+
+        Return value: number of bytes written.
+        """
+        ...
+    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/ussl.pyi` & `micropython_esp32_stubs-1.20.0.post1/ussl.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,50 @@
-"""
-TLS/SSL wrapper for socket objects. See: https://docs.micropython.org/en/v1.19.1/library/ssl.html
-
-|see_cpython_module| :mod:`python:ssl` https://docs.python.org/3/library/ssl.html .
-
-This module provides access to Transport Layer Security (previously and
-widely known as “Secure Sockets Layer”) encryption and peer authentication
-facilities for network sockets, both client-side and server-side.
-"""
-from typing import Any
-
-def wrap_socket(sock, server_side=False, keyfile=None, certfile=None, cert_reqs=None, ca_certs=None, do_handshake=True) -> Any:
-    """
-    Takes a `stream` *sock* (usually socket.socket instance of ``SOCK_STREAM`` type),
-    and returns an instance of ssl.SSLSocket, which wraps the underlying stream in
-    an SSL context. Returned object has the usual `stream` interface methods like
-    ``read()``, ``write()``, etc.
-    A server-side SSL socket should be created from a normal socket returned from
-    :meth:`~socket.socket.accept()` on a non-SSL listening server socket.
-
-    - *do_handshake* determines whether the handshake is done as part of the ``wrap_socket``
-      or whether it is deferred to be done as part of the initial reads or writes
-      (there is no ``do_handshake`` method as in CPython).
-      For blocking sockets doing the handshake immediately is standard. For non-blocking
-      sockets (i.e. when the *sock* passed into ``wrap_socket`` is in non-blocking mode)
-      the handshake should generally be deferred because otherwise ``wrap_socket`` blocks
-      until it completes. Note that in AXTLS the handshake can be deferred until the first
-      read or write but it then blocks until completion.
-
-    Depending on the underlying module implementation in a particular
-    :term:`MicroPython port`, some or all keyword arguments above may be not supported.
-    """
-    ...
+"""
+TLS/SSL wrapper for socket objects. See: https://docs.micropython.org/en/v1.20.0/library/ssl.html
+
+|see_cpython_module| :mod:`python:ssl` https://docs.python.org/3/library/ssl.html .
+
+This module provides access to Transport Layer Security (previously and
+widely known as “Secure Sockets Layer”) encryption and peer authentication
+facilities for network sockets, both client-side and server-side.
+"""
+from typing import Any
+
+CERT_OPTIONAL: int
+CERT_REQUIRED: int
+CERT_NONE: int
+
+def wrap_socket(
+    sock, server_side=False, keyfile=None, certfile=None, cert_reqs=None, cadata=None, server_hostname=None, do_handshake=True
+) -> Any:
+    """
+    Takes a `stream` *sock* (usually socket.socket instance of ``SOCK_STREAM`` type),
+    and returns an instance of ssl.SSLSocket, which wraps the underlying stream in
+    an SSL context. Returned object has the usual `stream` interface methods like
+    ``read()``, ``write()``, etc.
+    A server-side SSL socket should be created from a normal socket returned from
+    :meth:`~socket.socket.accept()` on a non-SSL listening server socket.
+
+    - *do_handshake* determines whether the handshake is done as part of the ``wrap_socket``
+      or whether it is deferred to be done as part of the initial reads or writes
+      (there is no ``do_handshake`` method as in CPython).
+      For blocking sockets doing the handshake immediately is standard. For non-blocking
+      sockets (i.e. when the *sock* passed into ``wrap_socket`` is in non-blocking mode)
+      the handshake should generally be deferred because otherwise ``wrap_socket`` blocks
+      until it completes. Note that in AXTLS the handshake can be deferred until the first
+      read or write but it then blocks until completion.
+
+    - *cert_reqs* determines whether the peer (server or client) must present a valid certificate.
+      Note that for mbedtls based ports, ``ssl.CERT_NONE`` and ``ssl.CERT_OPTIONAL`` will not
+      validate any certificate, only ``ssl.CERT_REQUIRED`` will.
+
+    - *cadata* is a bytes object containing the CA certificate chain (in DER format) that will
+      validate the peer's certificate.  Currently only a single DER-encoded certificate is supported.
+
+    - *server_hostname* is for use as a client, and sets the hostname to check against the received
+      server certificate.  It also sets the name for Server Name Indication (SNI), allowing the server
+      to present the proper certificate.
+
+    Depending on the underlying module implementation in a particular
+    :term:`MicroPython port`, some or all keyword arguments above may be not supported.
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/usys.pyi` & `micropython_esp32_stubs-1.20.0.post1/usys.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-system specific functions. See: https://docs.micropython.org/en/v1.19.1/library/sys.html
-
-|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
-"""
-from typing import Dict, List, Tuple, Any
-
-platform: str
-version_info: tuple
-path: list
-version: str
-ps1: str
-ps2: str
-byteorder: str
-modules: dict
-argv: list
-implementation: tuple
-maxsize: int
-
-def print_exception(exc, file=stdout, /) -> None:
-    """
-    Print exception with a traceback to a file-like object *file* (or
-    `sys.stdout` by default).
-    """
-    ...
-
-def exit(retval=0, /) -> Any:
-    """
-    Terminate current program with a given exit code. Underlyingly, this
-    function raise as `SystemExit` exception. If an argument is given, its
-    value given as an argument to `SystemExit`.
-    """
-    ...
-
-stderr: Any
-stdout: Any
-stdin: Any
+"""
+system specific functions. See: https://docs.micropython.org/en/v1.20.0/library/sys.html
+
+|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
+"""
+from typing import Dict, List, Tuple, Any
+
+platform: str
+version_info: tuple
+path: list
+version: str
+ps1: str
+ps2: str
+byteorder: str
+modules: dict
+argv: list
+implementation: tuple
+maxsize: int
+
+def print_exception(exc, file=stdout, /) -> None:
+    """
+    Print exception with a traceback to a file-like object *file* (or
+    `sys.stdout` by default).
+    """
+    ...
+
+def exit(retval=0, /) -> Any:
+    """
+    Terminate current program with a given exit code. Underlyingly, this
+    function raise as `SystemExit` exception. If an argument is given, its
+    value given as an argument to `SystemExit`.
+    """
+    ...
+
+stderr: Any
+stdout: Any
+stdin: Any
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/utime.pyi` & `micropython_esp32_stubs-1.20.0.post1/utime.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-"""
-time related functions. See: https://docs.micropython.org/en/v1.19.1/library/time.html
-
-|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
-
-The ``time`` module provides functions for getting the current time and date,
-measuring time intervals, and for delays.
-
-**Time Epoch**: Unix port uses standard for POSIX systems epoch of
-1970-01-01 00:00:00 UTC. However, embedded ports use epoch of
-2000-01-01 00:00:00 UTC.
-
-**Maintaining actual calendar date/time**: This requires a
-Real Time Clock (RTC). On systems with underlying OS (including some
-RTOS), an RTC may be implicit. Setting and maintaining actual calendar
-time is responsibility of OS/RTOS and is done outside of MicroPython,
-it just uses OS API to query date/time. On baremetal ports however
-system time depends on ``machine.RTC()`` object. The current calendar time
-may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
-by following means:
-
-* By a backup battery (which may be an additional, optional component for
-  a particular board).
-* Using networked time protocol (requires setup by a port/user).
-* Set manually by a user on each power-up (many boards then maintain
-  RTC time across hard resets, though some may require setting it again
-  in such case).
-
-If actual calendar time is not maintained with a system/MicroPython RTC,
-functions below which require reference to current absolute time may
-behave not as expected.
-"""
-from typing import Optional, Tuple, Any
-
-def ticks_diff(ticks1, ticks2) -> int:
-    """
-    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
-    or `ticks_cpu()` functions, as a signed value which may wrap around.
-
-    The argument order is the same as for subtraction
-    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
-    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
-    directly using subtraction on them will produce incorrect result. That is why
-    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
-    arithmetics to produce correct result even for wrap-around values (as long as they not
-    too distant inbetween, see below). The function returns **signed** value in the range
-    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
-    two's-complement signed binary integers). If the result is negative, it means that
-    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
-    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
-    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
-    not hold, incorrect result will be returned. Specifically, if two tick values are
-    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
-    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
-    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
-    to the negative range of possible values.
-
-    Informal rationale of the constraints above: Suppose you are locked in a room with no
-    means to monitor passing of time except a standard 12-notch clock. Then if you look at
-    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
-    long sleep), then once you finally look again, it may seem to you that only 1 hour
-    has passed. To avoid this mistake, just look at the clock regularly. Your application
-    should do the same. "Too long sleep" metaphor also maps directly to application
-    behaviour: don't let your application run any single task for too long. Run tasks
-    in steps, and do time-keeping inbetween.
-
-    `ticks_diff()` is designed to accommodate various usage patterns, among them:
-
-    * Polling with timeout. In this case, the order of events is known, and you will deal
-      only with positive results of `ticks_diff()`::
-
-         # Wait for GPIO pin to be asserted, but at most 500us
-         start = time.ticks_us()
-         while pin.value() == 0:
-             if time.ticks_diff(time.ticks_us(), start) > 500:
-                 raise TimeoutError
-
-    * Scheduling events. In this case, `ticks_diff()` result may be negative
-      if an event is overdue::
-
-         # This code snippet is not optimized
-         now = time.ticks_ms()
-         scheduled_time = task.scheduled_time()
-         if ticks_diff(scheduled_time, now) > 0:
-             print("Too early, let's nap")
-             sleep_ms(ticks_diff(scheduled_time, now))
-             task.run()
-         elif ticks_diff(scheduled_time, now) == 0:
-             print("Right at time!")
-             task.run()
-         elif ticks_diff(scheduled_time, now) < 0:
-             print("Oops, running late, tell task to run faster!")
-             task.run(run_faster=true)
-
-    Note: Do not pass `time()` values to `ticks_diff()`, you should use
-    normal mathematical operations on them. But note that `time()` may (and will)
-    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
-
-    """
-    ...
-
-def ticks_add(ticks, delta) -> Any:
-    """
-    Offset ticks value by a given number, which can be either positive or negative.
-    Given a *ticks* value, this function allows to calculate ticks value *delta*
-    ticks before or after it, following modular-arithmetic definition of tick values
-    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
-    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
-    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
-    or numeric expression. `ticks_add()` is useful for calculating deadlines for
-    events/tasks. (Note: you must use `ticks_diff()` function to work with
-    deadlines.)
-
-    Examples::
-
-         # Find out what ticks value there was 100ms ago
-         print(ticks_add(time.ticks_ms(), -100))
-
-         # Calculate deadline for operation and test for it
-         deadline = ticks_add(time.ticks_ms(), 200)
-         while ticks_diff(deadline, time.ticks_ms()) > 0:
-             do_a_little_of_something()
-
-         # Find out TICKS_MAX used by this port
-         print(ticks_add(0, -1))
-
-    """
-    ...
-
-def ticks_cpu() -> Any:
-    """
-    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
-    in the system. This is usually CPU clocks, and that's why the function is named that
-    way. But it doesn't have to be a CPU clock, some other timing source available in a
-    system (e.g. high-resolution timer) can be used instead. The exact timing unit
-    (resolution) of this function is not specified on ``time`` module level, but
-    documentation for a specific port may provide more specific information. This
-    function is intended for very fine benchmarking or very tight real-time loops.
-    Avoid using it in portable code.
-
-    Availability: Not every port implements this function.
-
-    """
-    ...
-
-class time:
-    """
-    Returns the number of seconds, as an integer, since the Epoch, assuming that
-    underlying RTC is set and maintained as described above. If an RTC is not set, this
-    function returns number of seconds since a port-specific reference point in time (for
-    embedded boards without a battery-backed RTC, usually since power up or reset). If you
-    want to develop portable MicroPython application, you should not rely on this function
-    to provide higher than second precision.  If you need higher precision, absolute
-    timestamps, use `time_ns()`.  If relative times are acceptable then use the
-    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
-    `localtime()` without an argument is a better choice.
-    """
-
-    def __init__(self) -> None: ...
-
-def ticks_ms() -> int:
-    """
-    Returns an increasing millisecond counter with an arbitrary reference point, that
-    wraps around after some value.
-
-    The wrap-around value is not explicitly exposed, but we will
-    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
-    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
-    two, but otherwise may differ from port to port. The same period value is used
-    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
-    simplicity). Thus, these functions will return a value in range [*0* ..
-    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
-    non-negative values are used. For the most part, you should treat values returned
-    by these functions as opaque. The only operations available for them are
-    `ticks_diff()` and `ticks_add()` functions described below.
-
-    Note: Performing standard mathematical operations (+, -) or relational
-    operators (<, <=, >, >=) directly on these value will lead to invalid
-    result. Performing mathematical operations and then passing their results
-    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
-    invalid results from the latter functions.
-    """
-    ...
-
-def ticks_us() -> Any:
-    """
-    Just like `ticks_ms()` above, but in microseconds.
-    """
-    ...
-
-def time_ns() -> int:
-    """
-    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
-    a big integer, so will allocate on the heap).
-    """
-    ...
-
-def localtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_us(us) -> None:
-    """
-    Delay for given number of microseconds, should be positive or 0.
-
-    This function attempts to provide an accurate delay of at least *us*
-    microseconds, but it may take longer if the system has other higher priority
-    processing to perform.
-    """
-    ...
-
-def gmtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_ms(ms) -> None:
-    """
-    Delay for given number of milliseconds, should be positive or 0.
-
-    This function will delay for at least the given number of milliseconds, but
-    may take longer than that if other processing must take place, for example
-    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
-    this other processing to occur.  Use `sleep_us()` for more precise delays.
-    """
-    ...
-
-def mktime() -> int:
-    """
-    This is inverse function of localtime. It's argument is a full 8-tuple
-    which expresses a time as per localtime. It returns an integer which is
-    the number of seconds since Jan 1, 2000.
-    """
-    ...
-
-def sleep(seconds) -> Any:
-    """
-    Sleep for the given number of seconds. Some boards may accept *seconds* as a
-    floating-point number to sleep for a fractional number of seconds. Note that
-    other boards may not accept a floating-point argument, for compatibility with
-    them use `sleep_ms()` and `sleep_us()` functions.
-    """
-    ...
+"""
+time related functions. See: https://docs.micropython.org/en/v1.20.0/library/time.html
+
+|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
+
+The ``time`` module provides functions for getting the current time and date,
+measuring time intervals, and for delays.
+
+**Time Epoch**: Unix port uses standard for POSIX systems epoch of
+1970-01-01 00:00:00 UTC. However, some embedded ports use epoch of
+2000-01-01 00:00:00 UTC. Epoch year may be determined with ``gmtime(0)[0]``.
+
+**Maintaining actual calendar date/time**: This requires a
+Real Time Clock (RTC). On systems with underlying OS (including some
+RTOS), an RTC may be implicit. Setting and maintaining actual calendar
+time is responsibility of OS/RTOS and is done outside of MicroPython,
+it just uses OS API to query date/time. On baremetal ports however
+system time depends on ``machine.RTC()`` object. The current calendar time
+may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
+by following means:
+
+* By a backup battery (which may be an additional, optional component for
+  a particular board).
+* Using networked time protocol (requires setup by a port/user).
+* Set manually by a user on each power-up (many boards then maintain
+  RTC time across hard resets, though some may require setting it again
+  in such case).
+
+If actual calendar time is not maintained with a system/MicroPython RTC,
+functions below which require reference to current absolute time may
+behave not as expected.
+"""
+from typing import Optional, Tuple, Any
+
+def ticks_diff(ticks1, ticks2) -> int:
+    """
+    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
+    or `ticks_cpu()` functions, as a signed value which may wrap around.
+
+    The argument order is the same as for subtraction
+    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
+    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
+    directly using subtraction on them will produce incorrect result. That is why
+    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
+    arithmetics to produce correct result even for wrap-around values (as long as they not
+    too distant inbetween, see below). The function returns **signed** value in the range
+    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
+    two's-complement signed binary integers). If the result is negative, it means that
+    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
+    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
+    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
+    not hold, incorrect result will be returned. Specifically, if two tick values are
+    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
+    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
+    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
+    to the negative range of possible values.
+
+    Informal rationale of the constraints above: Suppose you are locked in a room with no
+    means to monitor passing of time except a standard 12-notch clock. Then if you look at
+    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
+    long sleep), then once you finally look again, it may seem to you that only 1 hour
+    has passed. To avoid this mistake, just look at the clock regularly. Your application
+    should do the same. "Too long sleep" metaphor also maps directly to application
+    behaviour: don't let your application run any single task for too long. Run tasks
+    in steps, and do time-keeping inbetween.
+
+    `ticks_diff()` is designed to accommodate various usage patterns, among them:
+
+    * Polling with timeout. In this case, the order of events is known, and you will deal
+      only with positive results of `ticks_diff()`::
+
+         # Wait for GPIO pin to be asserted, but at most 500us
+         start = time.ticks_us()
+         while pin.value() == 0:
+             if time.ticks_diff(time.ticks_us(), start) > 500:
+                 raise TimeoutError
+
+    * Scheduling events. In this case, `ticks_diff()` result may be negative
+      if an event is overdue::
+
+         # This code snippet is not optimized
+         now = time.ticks_ms()
+         scheduled_time = task.scheduled_time()
+         if ticks_diff(scheduled_time, now) > 0:
+             print("Too early, let's nap")
+             sleep_ms(ticks_diff(scheduled_time, now))
+             task.run()
+         elif ticks_diff(scheduled_time, now) == 0:
+             print("Right at time!")
+             task.run()
+         elif ticks_diff(scheduled_time, now) < 0:
+             print("Oops, running late, tell task to run faster!")
+             task.run(run_faster=true)
+
+    Note: Do not pass `time()` values to `ticks_diff()`, you should use
+    normal mathematical operations on them. But note that `time()` may (and will)
+    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
+
+    """
+    ...
+
+def ticks_add(ticks, delta) -> Any:
+    """
+    Offset ticks value by a given number, which can be either positive or negative.
+    Given a *ticks* value, this function allows to calculate ticks value *delta*
+    ticks before or after it, following modular-arithmetic definition of tick values
+    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
+    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
+    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
+    or numeric expression. `ticks_add()` is useful for calculating deadlines for
+    events/tasks. (Note: you must use `ticks_diff()` function to work with
+    deadlines.)
+
+    Examples::
+
+         # Find out what ticks value there was 100ms ago
+         print(ticks_add(time.ticks_ms(), -100))
+
+         # Calculate deadline for operation and test for it
+         deadline = ticks_add(time.ticks_ms(), 200)
+         while ticks_diff(deadline, time.ticks_ms()) > 0:
+             do_a_little_of_something()
+
+         # Find out TICKS_MAX used by this port
+         print(ticks_add(0, -1))
+
+    """
+    ...
+
+def ticks_cpu() -> Any:
+    """
+    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
+    in the system. This is usually CPU clocks, and that's why the function is named that
+    way. But it doesn't have to be a CPU clock, some other timing source available in a
+    system (e.g. high-resolution timer) can be used instead. The exact timing unit
+    (resolution) of this function is not specified on ``time`` module level, but
+    documentation for a specific port may provide more specific information. This
+    function is intended for very fine benchmarking or very tight real-time loops.
+    Avoid using it in portable code.
+
+    Availability: Not every port implements this function.
+
+    """
+    ...
+
+class time:
+    """
+    Returns the number of seconds, as an integer, since the Epoch, assuming that
+    underlying RTC is set and maintained as described above. If an RTC is not set, this
+    function returns number of seconds since a port-specific reference point in time (for
+    embedded boards without a battery-backed RTC, usually since power up or reset). If you
+    want to develop portable MicroPython application, you should not rely on this function
+    to provide higher than second precision.  If you need higher precision, absolute
+    timestamps, use `time_ns()`.  If relative times are acceptable then use the
+    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
+    `localtime()` without an argument is a better choice.
+    """
+
+    def __init__(self) -> None: ...
+
+def ticks_ms() -> int:
+    """
+    Returns an increasing millisecond counter with an arbitrary reference point, that
+    wraps around after some value.
+
+    The wrap-around value is not explicitly exposed, but we will
+    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
+    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
+    two, but otherwise may differ from port to port. The same period value is used
+    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
+    simplicity). Thus, these functions will return a value in range [*0* ..
+    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
+    non-negative values are used. For the most part, you should treat values returned
+    by these functions as opaque. The only operations available for them are
+    `ticks_diff()` and `ticks_add()` functions described below.
+
+    Note: Performing standard mathematical operations (+, -) or relational
+    operators (<, <=, >, >=) directly on these value will lead to invalid
+    result. Performing mathematical operations and then passing their results
+    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
+    invalid results from the latter functions.
+    """
+    ...
+
+def ticks_us() -> Any:
+    """
+    Just like `ticks_ms()` above, but in microseconds.
+    """
+    ...
+
+def time_ns() -> int:
+    """
+    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
+    a big integer, so will allocate on the heap).
+    """
+    ...
+
+def localtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_us(us) -> None:
+    """
+    Delay for given number of microseconds, should be positive or 0.
+
+    This function attempts to provide an accurate delay of at least *us*
+    microseconds, but it may take longer if the system has other higher priority
+    processing to perform.
+    """
+    ...
+
+def gmtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_ms(ms) -> None:
+    """
+    Delay for given number of milliseconds, should be positive or 0.
+
+    This function will delay for at least the given number of milliseconds, but
+    may take longer than that if other processing must take place, for example
+    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
+    this other processing to occur.  Use `sleep_us()` for more precise delays.
+    """
+    ...
+
+def mktime() -> int:
+    """
+    This is inverse function of localtime. It's argument is a full 8-tuple
+    which expresses a time as per localtime. It returns an integer which is
+    the number of seconds since Jan 1, 2000.
+    """
+    ...
+
+def sleep(seconds) -> Any:
+    """
+    Sleep for the given number of seconds. Some boards may accept *seconds* as a
+    floating-point number to sleep for a fractional number of seconds. Note that
+    other boards may not accept a floating-point argument, for compatibility with
+    them use `sleep_ms()` and `sleep_us()` functions.
+    """
+    ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/uzlib.pyi` & `micropython_esp32_stubs-1.20.0.post1/uzlib.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-zlib decompression. See: https://docs.micropython.org/en/v1.19.1/library/zlib.html
-
-|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
-
-This module allows to decompress binary data compressed with
-`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
-(commonly used in zlib library and gzip archiver). Compression
-is not yet implemented.
-"""
-from typing import IO, Any
-
-def decompress(data, wbits=0, bufsize=0, /) -> bytes:
-    """
-    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
-    size used during compression (8-15, the dictionary size is power of 2 of
-    that value). Additionally, if value is positive, *data* is assumed to be
-    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
-    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
-    CPython and is ignored.
-    """
-    ...
-
-class DecompIO:
-    """
-    Create a `stream` wrapper which allows transparent decompression of
-    compressed data in another *stream*. This allows to process compressed
-    streams with data larger than available heap size. In addition to
-    values described in :func:`decompress`, *wbits* may take values
-    24..31 (16 + 8..15), meaning that input stream has gzip header.
-    """
-
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def readline(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def __init__(self, stream, wbits=0, /) -> None: ...
+"""
+zlib decompression. See: https://docs.micropython.org/en/v1.20.0/library/zlib.html
+
+|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
+
+This module allows to decompress binary data compressed with
+`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
+(commonly used in zlib library and gzip archiver). Compression
+is not yet implemented.
+"""
+from typing import Any
+
+def decompress(data, wbits=0, bufsize=0, /) -> bytes:
+    """
+    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
+    size used during compression (8-15, the dictionary size is power of 2 of
+    that value). Additionally, if value is positive, *data* is assumed to be
+    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
+    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
+    CPython and is ignored.
+    """
+    ...
+
+class DecompIO:
+    """
+    Create a `stream` wrapper which allows transparent decompression of
+    compressed data in another *stream*. This allows to process compressed
+    streams with data larger than available heap size. In addition to
+    values described in :func:`decompress`, *wbits* may take values
+    24..31 (16 + 8..15), meaning that input stream has gzip header.
+    """
+
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def readline(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def __init__(self, stream, wbits=0, /) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/zlib.pyi` & `micropython_esp32_stubs-1.20.0.post1/zlib.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-zlib decompression. See: https://docs.micropython.org/en/v1.19.1/library/zlib.html
-
-|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
-
-This module allows to decompress binary data compressed with
-`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
-(commonly used in zlib library and gzip archiver). Compression
-is not yet implemented.
-"""
-from typing import IO, Any
-
-def decompress(data, wbits=0, bufsize=0, /) -> bytes:
-    """
-    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
-    size used during compression (8-15, the dictionary size is power of 2 of
-    that value). Additionally, if value is positive, *data* is assumed to be
-    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
-    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
-    CPython and is ignored.
-    """
-    ...
-
-class DecompIO:
-    """
-    Create a `stream` wrapper which allows transparent decompression of
-    compressed data in another *stream*. This allows to process compressed
-    streams with data larger than available heap size. In addition to
-    values described in :func:`decompress`, *wbits* may take values
-    24..31 (16 + 8..15), meaning that input stream has gzip header.
-    """
-
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def readline(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def __init__(self, stream, wbits=0, /) -> None: ...
+"""
+zlib decompression. See: https://docs.micropython.org/en/v1.20.0/library/zlib.html
+
+|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
+
+This module allows to decompress binary data compressed with
+`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
+(commonly used in zlib library and gzip archiver). Compression
+is not yet implemented.
+"""
+from typing import Any
+
+def decompress(data, wbits=0, bufsize=0, /) -> bytes:
+    """
+    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
+    size used during compression (8-15, the dictionary size is power of 2 of
+    that value). Additionally, if value is positive, *data* is assumed to be
+    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
+    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
+    CPython and is ignored.
+    """
+    ...
+
+class DecompIO:
+    """
+    Create a `stream` wrapper which allows transparent decompression of
+    compressed data in another *stream*. This allows to process compressed
+    streams with data larger than available heap size. In addition to
+    values described in :func:`decompress`, *wbits* may take values
+    24..31 (16 + 8..15), meaning that input stream has gzip header.
+    """
+
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def readline(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def __init__(self, stream, wbits=0, /) -> None: ...
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/setup.py` & `micropython_esp32_stubs-1.20.0.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,47 +5,52 @@
 ['_boot',
  '_onewire',
  '_thread',
  '_uasyncio',
  'apa106',
  'array',
  'binascii',
+ 'bluetooth',
  'btree',
  'cmath',
+ 'collections',
+ 'cryptolib',
  'dht',
  'ds18x20',
  'errno',
  'esp',
  'esp32',
  'flashbdev',
  'framebuf',
  'gc',
  'hashlib',
  'heapq',
  'inisetup',
  'io',
  'json',
+ 'logging',
  'machine',
  'math',
  'micropython',
+ '__init__',
+ 'mip',
  'neopixel',
  'network',
  'ntptime',
  'onewire',
  'os',
  'platform',
  'random',
  'select',
  'socket',
  'ssl',
  'struct',
  'sys',
  'time',
  'uarray',
- '__init__',
  'core',
  'event',
  'funcs',
  'lock',
  'stream',
  'task',
  'ubinascii',
@@ -58,17 +63,16 @@
  'uheapq',
  'uio',
  'ujson',
  'umachine',
  'robust',
  'simple',
  'uos',
- 'upip',
- 'upip_utarfile',
  'uplatform',
+ 'upysh',
  'urandom',
  'ure',
  'urequests',
  'uselect',
  'usocket',
  'ussl',
  'ustruct',
@@ -76,24 +80,23 @@
  'utime',
  'utimeq',
  'uwebsocket',
  'uzlib',
  'webrepl',
  'webrepl_setup',
  'websocket',
- 'websocket_helper',
  'zlib']
 install_requires = \
 ['micropython-stdlib-stubs>=0.9.0']
 
 setup_kwargs = {
     'name': 'micropython-esp32-stubs',
-    'version': '1.19.1.post9',
+    'version': '1.20.0.post1',
     'description': 'MicroPython stubs',
-    'long_description': '# micropython-esp32-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_19_1-esp32-merged`\n* Frozen stubs from `stubs/micropython-v1_19_1-frozen/esp32/GENERIC`\n* Core Stubs from `stubs/cpython_core-pycopy`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nFirmware | micropython | esp32 | ESP32 module (spiram) with ESP32 | v1.19.1 \nDocumentation | micropython | - | - | v1.19.1 \nCore | micropython | esp32 | - | v1.19.1 \n',
+    'long_description': '# micropython-esp32-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* StubSource.MERGED from `stubs/micropython-v1_20_0-esp32-merged`\n* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`\n* StubSource.CORE from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | esp32 | - | v1.20.0 \n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `micropython_esp32_stubs-1.19.1.post9/PKG-INFO` & `micropython_esp32_stubs-1.20.0.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-esp32-stubs
-Version: 1.19.1.post9
+Version: 1.20.0.post1
 Summary: MicroPython stubs
 Home-page: https://github.com/josverl/micropython-stubs#micropython-stubs
 License: MIT
 Author: josverl
 Author-email: josverl@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -52,18 +52,17 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* Merged stubs from `stubs/micropython-v1_19_1-esp32-merged`
-* Frozen stubs from `stubs/micropython-v1_19_1-frozen/esp32/GENERIC`
-* Core Stubs from `stubs/cpython_core-pycopy`
+* StubSource.MERGED from `stubs/micropython-v1_20_0-esp32-merged`
+* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
+* StubSource.CORE from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
-Firmware | micropython | esp32 | ESP32 module (spiram) with ESP32 | v1.19.1 
-Documentation | micropython | - | - | v1.19.1 
-Core | micropython | esp32 | - | v1.19.1 
+Documentation | micropython | - | - | v1.20.0 
+Core | micropython | esp32 | - | v1.20.0
```

