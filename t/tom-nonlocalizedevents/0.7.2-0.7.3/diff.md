# Comparing `tmp/tom_nonlocalizedevents-0.7.2.tar.gz` & `tmp/tom_nonlocalizedevents-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_nonlocalizedevents-0.7.2.tar", max compression
+gzip compressed data, was "tom_nonlocalizedevents-0.7.3.tar", max compression
```

## Comparing `tom_nonlocalizedevents-0.7.2.tar` & `tom_nonlocalizedevents-0.7.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    35149 2023-04-28 21:04:24.549482 tom_nonlocalizedevents-0.7.2/LICENSE
--rw-r--r--   0        0        0     5324 2023-04-28 21:04:24.549482 tom_nonlocalizedevents-0.7.2/README.md
--rw-r--r--   0        0        0     2632 2023-04-28 21:04:49.621361 tom_nonlocalizedevents-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      144 2023-04-28 21:04:49.621361 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/__init__.py
--rw-r--r--   0        0        0      459 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/admin.py
--rw-r--r--   0        0        0        0 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/alertstream_handlers/__init__.py
--rw-r--r--   0        0        0     5307 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py
--rw-r--r--   0        0        0     4359 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py
--rw-r--r--   0        0        0      228 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/apps.py
--rw-r--r--   0        0        0    12419 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/healpix_utils.py
--rw-r--r--   0        0        0     3766 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/ingestion.py
--rw-r--r--   0        0        0      437 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0001_initial.py
--rw-r--r--   0        0        0      585 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0002_superevent.py
--rw-r--r--   0        0        0     1075 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py
--rw-r--r--   0        0        0      460 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0004_superevent_superevent_type.py
--rw-r--r--   0        0        0      543 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py
--rw-r--r--   0        0        0     1015 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py
--rw-r--r--   0        0        0      409 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0007_eventcandidate_viable.py
--rw-r--r--   0        0        0      411 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0008_eventcandidate_priority.py
--rw-r--r--   0        0        0      365 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0009_rename_superevent_nonlocalizedevent.py
--rw-r--r--   0        0        0     1434 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py
--rw-r--r--   0        0        0     2028 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py
--rw-r--r--   0        0        0      574 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py
--rw-r--r--   0        0        0     2510 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py
--rw-r--r--   0        0        0     2082 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py
--rw-r--r--   0        0        0     4567 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py
--rw-r--r--   0        0        0     3814 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py
--rw-r--r--   0        0        0      872 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0017_alter_eventsequence_external_coincidence_and_more.py
--rw-r--r--   0        0        0        0 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/__init__.py
--rw-r--r--   0        0        0     9757 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/models.py
--rw-r--r--   0        0        0     6850 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/serializers.py
--rw-r--r--   0        0        0        0 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/signals/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/signals/handlers.py
--rw-r--r--   0        0        0       99 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/css/main.css
--rw-r--r--   0        0        0   218067 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css
--rw-r--r--   0        0        0  1780610 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js
--rw-r--r--   0        0        0      416 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/webpack-stats.json
--rw-r--r--   0        0        0      168 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/detail.html
--rw-r--r--   0        0        0     1606 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html
--rw-r--r--   0        0        0      490 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/superevent_vue_app.html
--rw-r--r--   0        0        0        0 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/tests/__init__.py
--rw-r--r--   0        0        0      693 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/tests/factories.py
--rw-r--r--   0        0        0     2879 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/tests/tests.py
--rw-r--r--   0        0        0     1120 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/urls.py
--rw-r--r--   0        0        0     6577 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/views.py
--rw-r--r--   0        0        0     7523 1970-01-01 00:00:00.000000 tom_nonlocalizedevents-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-05 05:44:53.785058 tom_nonlocalizedevents-0.7.3/LICENSE
+-rw-r--r--   0        0        0     5324 2023-05-05 05:44:53.785058 tom_nonlocalizedevents-0.7.3/README.md
+-rw-r--r--   0        0        0     2632 2023-05-05 05:45:13.341473 tom_nonlocalizedevents-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-05-05 05:45:13.341473 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/__init__.py
+-rw-r--r--   0        0        0      459 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/admin.py
+-rw-r--r--   0        0        0        0 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/alertstream_handlers/__init__.py
+-rw-r--r--   0        0        0     5307 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py
+-rw-r--r--   0        0        0     4427 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py
+-rw-r--r--   0        0        0      228 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/apps.py
+-rw-r--r--   0        0        0    12369 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/healpix_utils.py
+-rw-r--r--   0        0        0     3766 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/ingestion.py
+-rw-r--r--   0        0        0      437 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0001_initial.py
+-rw-r--r--   0        0        0      585 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0002_superevent.py
+-rw-r--r--   0        0        0     1075 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py
+-rw-r--r--   0        0        0      460 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0004_superevent_superevent_type.py
+-rw-r--r--   0        0        0      543 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py
+-rw-r--r--   0        0        0     1015 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py
+-rw-r--r--   0        0        0      409 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0007_eventcandidate_viable.py
+-rw-r--r--   0        0        0      411 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0008_eventcandidate_priority.py
+-rw-r--r--   0        0        0      365 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0009_rename_superevent_nonlocalizedevent.py
+-rw-r--r--   0        0        0     1434 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py
+-rw-r--r--   0        0        0     2028 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py
+-rw-r--r--   0        0        0      574 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py
+-rw-r--r--   0        0        0     2510 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py
+-rw-r--r--   0        0        0     2082 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py
+-rw-r--r--   0        0        0     4567 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py
+-rw-r--r--   0        0        0     3814 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py
+-rw-r--r--   0        0        0      872 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0017_alter_eventsequence_external_coincidence_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/__init__.py
+-rw-r--r--   0        0        0     9779 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/models.py
+-rw-r--r--   0        0        0     6850 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/signals/__init__.py
+-rw-r--r--   0        0        0     1459 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/signals/handlers.py
+-rw-r--r--   0        0        0       99 2023-05-05 05:44:53.789058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/css/main.css
+-rw-r--r--   0        0        0   218067 2023-05-05 05:44:53.793058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css
+-rw-r--r--   0        0        0  1780610 2023-05-05 05:44:53.801058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js
+-rw-r--r--   0        0        0      416 2023-05-05 05:44:53.801058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/webpack-stats.json
+-rw-r--r--   0        0        0      168 2023-05-05 05:44:53.801058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/detail.html
+-rw-r--r--   0        0        0     1606 2023-05-05 05:44:53.801058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html
+-rw-r--r--   0        0        0      490 2023-05-05 05:44:53.801058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/superevent_vue_app.html
+-rw-r--r--   0        0        0        0 2023-05-05 05:44:53.801058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/tests/__init__.py
+-rw-r--r--   0        0        0      693 2023-05-05 05:44:53.801058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/tests/factories.py
+-rw-r--r--   0        0        0     2879 2023-05-05 05:44:53.801058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/tests/tests.py
+-rw-r--r--   0        0        0     1120 2023-05-05 05:44:53.801058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/urls.py
+-rw-r--r--   0        0        0     6577 2023-05-05 05:44:53.801058 tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/views.py
+-rw-r--r--   0        0        0     7523 1970-01-01 00:00:00.000000 tom_nonlocalizedevents-0.7.3/PKG-INFO
```

### Comparing `tom_nonlocalizedevents-0.7.2/LICENSE` & `tom_nonlocalizedevents-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/README.md` & `tom_nonlocalizedevents-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/pyproject.toml` & `tom_nonlocalizedevents-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tom-nonlocalizedevents"
 # this version is a placeholder: version supplied by poetry-dynamic-versioning
-version = "0.7.2"
+version = "0.7.3"
 description = "Reusable TOMToolkit app to support gravitational wave superevent and other nonlocalized event EM follow-up observations."
 authors = ["TOM Toolkit Project <tomtoolkit@lco.global>", "David Collom <dcollom@lco.global>", "Lindy Lindstrom <llindstrom@lco.global>", "Jonathan Nation <jnation@lco.global>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/TOMToolkit/tom_nonlocalizedevents"
 keywords = ["tomtoolkit", "astronomy", "astrophysics", "cosmology", "science"]
 classifiers = [
```

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 
 
 def handle_igwn_message(message: JSONBlob, metadata: Metadata):
     alert = message.content[0]
     logger.warning(f"Handling igwn alert: {alert}")
     # Only store test alerts if we are configured to do so
     if alert.get('superevent_id', '').startswith('M') and not settings.SAVE_TEST_ALERTS:
-        return
+        return None, None
 
     if alert.get('alert_type', '') == 'RETRACTION':
-        NonLocalizedEvent.objects.update_or_create(
+        nonlocalizedevent, nle_created = NonLocalizedEvent.objects.update_or_create(
             event_id=alert['superevent_id'],
             event_type=NonLocalizedEvent.NonLocalizedEventType.GRAVITATIONAL_WAVE,
             defaults={'state': NonLocalizedEvent.NonLocalizedEventState.RETRACTED}
         )
-        return
+        return nonlocalizedevent, None
 
     nonlocalizedevent, nle_created = NonLocalizedEvent.objects.get_or_create(
         event_id=alert['superevent_id'],
         event_type=NonLocalizedEvent.NonLocalizedEventType.GRAVITATIONAL_WAVE,
     )
     if nle_created:
         logger.info(f"Ingested a new GW event with id {alert['superevent_id']} from IGWN alertstream")
```

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/healpix_utils.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/healpix_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from django.db import transaction
 from django.conf import settings
 from django.utils import timezone
 from healpix_alchemy.constants import HPX, LEVEL
 from healpix_alchemy.types import Tile, Point
 import sqlalchemy as sa
 from sqlalchemy.orm import relationship, declarative_base, Session
-from astropy_healpix import uniq_to_level_ipix
+from astropy import units as u
+import astropy_healpix as ah
 from mocpy import MOC
 from ligo.skymap import distance
 from dateutil.parser import parse
 import healpy as hp
 import numpy as np
 import os
 import hashlib
@@ -41,15 +42,15 @@
     'CREDIBLE_REGION_PROBABILITIES', '[0.25, 0.5, 0.75, 0.9, 0.95]')), reverse=True)
 
 Base = declarative_base()
 sa_engine = sa.create_engine(SA_DB_CONNECTION_URL, pool_recycle=POOL_RECYCLE)
 
 
 def uniq_to_bigintrange(value):
-    level, ipix = uniq_to_level_ipix(value)
+    level, ipix = ah.uniq_to_level_ipix(value)
     shift = 2 * (LEVEL - level)
     return (ipix << shift, (ipix + 1) << shift)
 
 
 def sequence_to_bigintrange(sequence):
     return f'[{sequence[0]},{sequence[1]})'
 
@@ -61,35 +62,32 @@
 def tiles_from_polygon_skycoord(polygon):
     return tiles_from_moc(MOC.from_polygon_skycoord(polygon.transform_to(HPX.frame)))
 
 
 def get_confidence_regions(skymap: Table):
     """ This helper method takes in the astropy Table skymap and attempts to parse out
         the 50 and 90 area confidence values. It returns a tuple of (area_50, area_90).
+        See https://emfollow.docs.ligo.org/userguide/tutorial/multiorder_skymaps.html.
     """
     try:
-        # Get the total number of healpixels in the map
-        n_pixels = len(skymap['PROBDENSITY'])
-        # Covert that to the nside parameter
-        nside = hp.npix2nside(n_pixels)
-        # Sort the probabilities so we can do the cumulative sum on them
-        probabilities = skymap['PROBDENSITY']
-        probabilities.sort()
-        # Reverse the list so that the largest pixels are first
-        probabilities = probabilities[::-1]
-        cumulative_probabilities = np.cumsum(probabilities)
-        # The number of pixels in the 90 (or 50) percent range is just given by the first set of pixels that add up
-        # to 0.9 (0.5)
-        index_90 = np.min(np.flatnonzero(cumulative_probabilities >= 0.9))
-        index_50 = np.min(np.flatnonzero(cumulative_probabilities >= 0.5))
-        # Because the healpixel projection has equal area pixels, the total area is just the heal pixel area * the
-        # number of heal pixels
-        healpixel_area = hp.nside2pixarea(nside, degrees=True)
-        area_50 = (index_50 + 1) * healpixel_area
-        area_90 = (index_90 + 1) * healpixel_area
+        # Sort the pixels of the sky map by descending probability density
+        skymap.sort('PROBDENSITY', reverse=True)
+        # Find the area of each pixel
+        level, ipix = ah.uniq_to_level_ipix(skymap['UNIQ'])
+        pixel_area = ah.nside_to_pixel_area(ah.level_to_nside(level))
+        # Calculate the probability within each pixel: the pixel area times the probability density
+        prob = pixel_area * skymap['PROBDENSITY']
+        # Calculate the cumulative sum of the probability
+        cumprob = np.cumsum(prob)
+        # Find the pixel for which the probability sums to 0.5 (0.9)
+        index_50 = cumprob.searchsorted(0.5)
+        index_90 = cumprob.searchsorted(0.9)
+        # The area of the 50% (90%) credible region is simply the sum of the areas of the pixels up to that probability
+        area_50 = pixel_area[:index_50].sum().to_value(u.deg ** 2.)
+        area_90 = pixel_area[:index_90].sum().to_value(u.deg ** 2.)
 
         return area_50, area_90
     except Exception as e:
         logger.error(f'Unable to parse raw skymap for OBJECT {skymap.meta["OBJECT"]} for confidence regions: {e}')
 
     return None, None
```

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/ingestion.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/ingestion.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0002_superevent.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0002_superevent.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0017_alter_eventsequence_external_coincidence_and_more.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/migrations/0017_alter_eventsequence_external_coincidence_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/models.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,18 @@
     )
     event_subtype = models.CharField(
         max_length=256,
         default='',
         help_text='The subtype of the event. Options are type specific, i.e. GW events have initial, '
                   'preliminary, update types.'
     )
-    ingestor_source = models.CharField(default='', max_length=64, help_text='The source of this alert - i.e. which stream is it from?')
+    ingestor_source = models.CharField(
+        default='', max_length=64,
+        help_text='The source of this alert - i.e. which stream is it from?'
+    )
     created = models.DateTimeField(auto_now_add=True)
     modified = models.DateTimeField(auto_now=True)
 
     class Meta:
         ordering = ["sequence_id"]
         constraints = [
             models.UniqueConstraint(
```

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/serializers.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/serializers.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/signals/handlers.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/tests/factories.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/tests/factories.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/tests/tests.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/tests/tests.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/urls.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/urls.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/views.py` & `tom_nonlocalizedevents-0.7.3/tom_nonlocalizedevents/views.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.2/PKG-INFO` & `tom_nonlocalizedevents-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tom-nonlocalizedevents
-Version: 0.7.2
+Version: 0.7.3
 Summary: Reusable TOMToolkit app to support gravitational wave superevent and other nonlocalized event EM follow-up observations.
 Home-page: https://github.com/TOMToolkit/tom_nonlocalizedevents
 License: GPL-3.0-only
 Keywords: tomtoolkit,astronomy,astrophysics,cosmology,science
 Author: TOM Toolkit Project
 Author-email: tomtoolkit@lco.global
 Requires-Python: >=3.8,<3.12
```

