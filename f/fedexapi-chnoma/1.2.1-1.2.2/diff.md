# Comparing `tmp/fedexapi_chnoma-1.2.1.tar.gz` & `tmp/fedexapi_chnoma-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedexapi_chnoma-1.2.1.tar", last modified: Wed Apr 19 18:36:07 2023, max compression
+gzip compressed data, was "fedexapi_chnoma-1.2.2.tar", last modified: Fri May  5 14:36:14 2023, max compression
```

## Comparing `fedexapi_chnoma-1.2.1.tar` & `fedexapi_chnoma-1.2.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 18:36:07.020719 fedexapi_chnoma-1.2.1/
--rw-rw-rw-   0        0        0     1079 2023-03-09 14:41:47.000000 fedexapi_chnoma-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      590 2023-04-19 18:36:07.018719 fedexapi_chnoma-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    10964 2023-04-19 18:32:02.000000 fedexapi_chnoma-1.2.1/fedex_api.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:36:07.004484 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/
--rw-rw-rw-   0        0        0      590 2023-04-19 18:36:06.000000 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-04-19 18:36:06.000000 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 18:36:06.000000 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 18:36:06.000000 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 18:36:06.000000 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      703 2023-04-19 18:33:49.000000 fedexapi_chnoma-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 18:36:07.020719 fedexapi_chnoma-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 14:36:14.295043 fedexapi_chnoma-1.2.2/
+-rw-rw-rw-   0        0        0     1079 2023-04-27 15:17:09.000000 fedexapi_chnoma-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-05 14:35:35.000000 fedexapi_chnoma-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      590 2023-05-05 14:36:14.292002 fedexapi_chnoma-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11279 2023-05-05 14:29:24.000000 fedexapi_chnoma-1.2.2/fedex_api.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:36:14.282079 fedexapi_chnoma-1.2.2/fedexapi_chnoma.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-05-05 14:36:14.000000 fedexapi_chnoma-1.2.2/fedexapi_chnoma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-05 14:36:14.000000 fedexapi_chnoma-1.2.2/fedexapi_chnoma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:36:14.000000 fedexapi_chnoma-1.2.2/fedexapi_chnoma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 14:36:14.000000 fedexapi_chnoma-1.2.2/fedexapi_chnoma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 14:36:14.000000 fedexapi_chnoma-1.2.2/fedexapi_chnoma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      703 2023-05-05 14:30:01.000000 fedexapi_chnoma-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 14:36:14.298060 fedexapi_chnoma-1.2.2/setup.cfg
```

### Comparing `fedexapi_chnoma-1.2.1/LICENSE` & `fedexapi_chnoma-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fedexapi_chnoma-1.2.1/PKG-INFO` & `fedexapi_chnoma-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedexapi_chnoma
-Version: 1.2.1
+Version: 1.2.2
 Summary: A module I devloped to abstract the Fedex API for use in my programs.
 Author-email: "Adrian J. Arnett" <adrianarnett0@gmail.com>
 Project-URL: Homepage, https://github.com/chnoma/fedex-api
 Project-URL: Bug Tracker, https://github.com/chnoma/fedex-api/issues
 Keywords: FedEx,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fedexapi_chnoma-1.2.1/fedex_api.py` & `fedexapi_chnoma-1.2.2/fedex_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,15 @@
     unique_id: str = None
     carrier_code: str = None
     is_delivered: bool = None
     is_shipped: bool = None
     date_ship: date = None
     date_delivery: date = None  # EST Delivery date if not delivered.
     latest_status: DateAndTimeEvent = None
+    recipient_name: str = None
     events: list = None
     package: Package = None
     json: dict = None
     has_associated_shipments: bool = False
     master_tracking_number: str = None
 
 
@@ -171,16 +172,23 @@
                 elif event_type == Event.ESTIMATED_DELIVERY:
                     delivery_date = event_date
                 if latest_type is None or event_date > latest_date:
                     latest_date = event_date
                     latest_type = event_type
                 new_event = DateAndTimeEvent(event_date, event_type)
                 events.append(new_event)
+
+            try:
+                recipient_name = tracking_result["deliveryDetails"]["receivedByName"]
+            except KeyError:
+                recipient_name = None
+
             latest_event = DateAndTimeEvent(latest_date, latest_type)
-            if "packageDetails" in tracking_result and "physicalPackagingType" in tracking_result["packageDetails"] and "count" in tracking_result["packageDetails"]:
+            if "packageDetails" in tracking_result and "physicalPackagingType"\
+                    in tracking_result["packageDetails"] and "count" in tracking_result["packageDetails"]:
                 package = Package(PackageType[tracking_result["packageDetails"]["physicalPackagingType"]],
                                 int(tracking_result["packageDetails"]["count"]))
             has_associated_shipments = tracking_result["additionalTrackingInfo"]["hasAssociatedShipments"]
             master_tracking_number = ""
             if has_associated_shipments:
                 master_tracking_number = tracking_result["additionalTrackingInfo"]["packageIdentifiers"][0]["values"][0]
             new_tracking_result = TrackingResult(
@@ -189,14 +197,15 @@
                 unique_id=unique_id,
                 carrier_code=carrier_code,
                 is_delivered=delivered,
                 is_shipped=shipped,
                 date_ship=ship_date,
                 date_delivery=delivery_date,
                 latest_status=latest_event,
+                recipient_name=recipient_name,
                 events=events,
                 package=package,
                 json=json,
                 has_associated_shipments=has_associated_shipments,
                 master_tracking_number=master_tracking_number)
             tracking_results.append(new_tracking_result)
 
@@ -272,23 +281,23 @@
         response_data = response.json()
         tracking_results = process_track_results(response_data)
         mps = MultipieceShipment(tracking_results)
         # if "errors" in response_data:
         #     return TrackingResult(False)
         return mps
 
-    def download_pod(self, unique_id, new_filename, retry=5):
+    def download_pod(self, unique_id, new_filename, account_number="", retry=5):
         if len(unique_id.split('~')) == 1:
             result = self.track_by_number(unique_id)
             if not result.is_valid:
                 raise InvalidRequestError(f"\nInvalid request for tracking number: {unique_id}")
             unique_id = result.unique_id
         qualifier = unique_id.split('~')[0]
         tracking_number = unique_id.split('~')[1]
         while retry>0:
             _download_file(
-                f"https://www.fedex.com/trackingCal/retrievePDF.jsp?accountNbr=&anon=true&appType=&destCountry=&locale=en_US&shipDate=&trackingCarrier=FDXA&trackingNumber={tracking_number}&trackingQualifier={qualifier}&type=SPOD",
+                f"https://www.fedex.com/trackingCal/retrievePDF.jsp?accountNbr={account_number}&anon=true&appType=&destCountry=&locale=en_US&shipDate=&trackingCarrier=FDXA&trackingNumber={tracking_number}&trackingQualifier={qualifier}&type=SPOD",
                 new_filename)
             if os.path.getsize(new_filename) > 10240:
                 break
             retry = retry-1
```

### Comparing `fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/PKG-INFO` & `fedexapi_chnoma-1.2.2/fedexapi_chnoma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedexapi-chnoma
-Version: 1.2.1
+Version: 1.2.2
 Summary: A module I devloped to abstract the Fedex API for use in my programs.
 Author-email: "Adrian J. Arnett" <adrianarnett0@gmail.com>
 Project-URL: Homepage, https://github.com/chnoma/fedex-api
 Project-URL: Bug Tracker, https://github.com/chnoma/fedex-api/issues
 Keywords: FedEx,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fedexapi_chnoma-1.2.1/pyproject.toml` & `fedexapi_chnoma-1.2.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fedexapi_chnoma"
-version = "1.2.1"
+version = "1.2.2"
 description = "A module I devloped to abstract the Fedex API for use in my programs."
 authors = [
   { name="Adrian J. Arnett", email="adrianarnett0@gmail.com" },
 ]
 readme = "readme.md"
 keywords = ["FedEx", "API"]
 requires-python = ">=3.7"
```

