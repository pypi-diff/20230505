# Comparing `tmp/databento_dbn-0.5.0-cp39-none-win_amd64.whl.zip` & `tmp/databento_dbn-0.5.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 548221 bytes, number of entries: 8
--rw-r--r--  4.6 unx     2966 b- defN 23-Apr-25 21:19 databento_dbn-0.5.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-25 21:19 databento_dbn-0.5.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     9868 b- defN 23-Apr-25 21:19 databento_dbn-0.5.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      135 b- defN 23-Apr-25 21:19 databento_dbn/__init__.py
--rw-r--r--  4.6 unx    34694 b- defN 23-Apr-25 21:19 databento_dbn/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Apr-25 21:19 databento_dbn/py.typed
--rwxr-xr-x  4.6 unx  1567232 b- defN 23-Apr-25 21:19 databento_dbn/databento_dbn.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      679 b- defN 23-Apr-25 21:19 databento_dbn-0.5.0.dist-info/RECORD
-8 files, 1615670 bytes uncompressed, 547033 bytes compressed:  66.1%
+Zip file size: 547876 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     2966 b- defN 23-May-05 09:39 databento_dbn-0.5.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-May-05 09:39 databento_dbn-0.5.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     9868 b- defN 23-May-05 09:39 databento_dbn-0.5.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      135 b- defN 23-May-05 09:39 databento_dbn/__init__.py
+-rw-r--r--  4.6 unx    37073 b- defN 23-May-05 09:39 databento_dbn/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-May-05 09:39 databento_dbn/py.typed
+-rwxr-xr-x  4.6 unx  1566720 b- defN 23-May-05 09:39 databento_dbn/databento_dbn.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      679 b- defN 23-May-05 09:39 databento_dbn-0.5.1.dist-info/RECORD
+8 files, 1617537 bytes uncompressed, 546688 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: databento_dbn-0.5.0.dist-info/METADATA
+Filename: databento_dbn-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: databento_dbn-0.5.0.dist-info/WHEEL
+Filename: databento_dbn-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: databento_dbn-0.5.0.dist-info/license_files/LICENSE
+Filename: databento_dbn-0.5.1.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: databento_dbn/__init__.py
 Comment: 
 
 Filename: databento_dbn/__init__.pyi
 Comment: 
 
 Filename: databento_dbn/py.typed
 Comment: 
 
 Filename: databento_dbn/databento_dbn.cp39-win_amd64.pyd
 Comment: 
 
-Filename: databento_dbn-0.5.0.dist-info/RECORD
+Filename: databento_dbn-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databento_dbn/__init__.pyi

```diff
@@ -19,14 +19,15 @@
     OHLCVMsg,
     TradeMsg,
     InstrumentDefMsg,
     ImbalanceMsg,
     ErrorMsg,
     SymbolMappingMsg,
     SystemMsg,
+    StatMsg,
 ]
 
 class Metadata(SupportsBytes):
     """
     Information about the data contained in a DBN file or stream. DBN requires
     the Metadata to be included at the start of the encoded data.
 
@@ -386,16 +387,16 @@
         -------
         int
 
         """
     @property
     def action(self) -> str:
         """
-        The event action. Can be `A`dd, `C`ancel, `M`odify, clea`R`, or
-        `T`rade.
+        The event action. Can be `A`dd, `C`ancel, `M`odify, clea`R`, `T`rade,
+        or `F`ill.
 
         Returns
         -------
         str
 
         """
     @property
@@ -1543,14 +1544,129 @@
 
         Returns
         -------
         str
 
         """
 
+class StatMsg(Record):
+    """
+    A statistics message.
+
+    A catchall for various data disseminated by publishers. The
+    `stat_type` field indicates the statistic contained in the message.
+
+    """
+
+    @property
+    def ts_recv(self) -> int:
+        """
+        The capture-server-received timestamp expressed as the number of
+        nanoseconds since the UNIX epoch.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def ts_ref(self) -> int:
+        """
+        Reference timestamp expressed as the number of nanoseconds since the
+        UNIX epoch.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def price(self) -> int:
+        """
+        The value for price statistics expressed as a signed integer where
+        every 1 unit corresponds to 1e-9, i.e. 1/1,000,000,000 or 0.000000001.
+        Will be undefined when unused.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def quantity(self) -> int:
+        """
+        The value for non-price statistics. Will be undefined when unused.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def sequence(self) -> int:
+        """
+        The message sequence number assigned at the venue.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def ts_in_delta(self) -> int:
+        """
+        The delta of `ts_recv - ts_exchange_send`, max 2 seconds.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def stat_type(self) -> int:
+        """
+        The type of statistic value contained in the message.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def channel_id(self) -> int:
+        """
+        A channel ID within the venue.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def update_action(self) -> int:
+        """
+        Indicates if the statistic is new added or deleted. Deleted is only
+        used for a couple stat types.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def stat_flags(self) -> int:
+        """
+        Additional flags associate with certain stat types.
+
+        Returns
+        -------
+        int
+
+        """
+
 class ErrorMsg(Record):
     """An error message from the Databento Live Subscription Gateway (LSG)."""
 
     @property
     def err(self) -> str:
         """
         The error message.
@@ -1625,16 +1741,16 @@
         -------
         str
 
         """
     @property
     def is_heartbeat(self) -> bool:
         """
-        `true` if this message is a heartbeat, used to indicate the connection with the gateway
-        is still open.
+        `true` if this message is a heartbeat, used to indicate the connection
+        with the gateway is still open.
 
         Returns
         -------
         bool
 
         """
```

## Comparing `databento_dbn-0.5.0.dist-info/METADATA` & `databento_dbn-0.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databento-dbn
-Version: 0.5.0
+Version: 0.5.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Native Databento bindings based on dbn Rust crate
 Author: Databento <support@databento.com>
 Author-email: Databento <support@databento.com>
```

## Comparing `databento_dbn-0.5.0.dist-info/license_files/LICENSE` & `databento_dbn-0.5.1.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

