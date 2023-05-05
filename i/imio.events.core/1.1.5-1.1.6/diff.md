# Comparing `tmp/imio.events.core-1.1.5.tar.gz` & `tmp/imio.events.core-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.events.core-1.1.5.tar", last modified: Fri Mar 31 12:17:15 2023, max compression
+gzip compressed data, was "imio.events.core-1.1.6.tar", last modified: Fri May  5 07:45:56 2023, max compression
```

## Comparing `imio.events.core-1.1.5.tar` & `imio.events.core-1.1.6.tar`

### file list

```diff
@@ -1,132 +1,133 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2963 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      651 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6037 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1993 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/README.rst
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7958 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       71 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/setup.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2536 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/setup.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.353954 imio.events.core-1.1.5/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio/events/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio/events/core/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      267 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio/events/core/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      718 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/browser/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio/events/core/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/browser/overrides/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio/events/core/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/browser/static/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1472 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/browser/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      850 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio/events/core/contents/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/contents/agenda/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/agenda/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/agenda/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1264 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/agenda/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      198 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/contents/entity/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/entity/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/entity/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1153 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/entity/content.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/contents/event/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/event/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      664 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/event/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6641 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/event/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2785 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/event/serializer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8341 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/event/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4323 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/event/views.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/contents/folder/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/folder/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/folder/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/contents/folder/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/converters.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio/events/core/faceted/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8038 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/faceted/config/events.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5107 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/indexers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1795 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/indexers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      201 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/overrides.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      520 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio/events/core/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2525 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      590 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      685 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      840 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/profiles/default/taxonomies/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/taxonomies/event_public.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4154 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/taxonomies/event_public.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/types/Plone_Site.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1386 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1583 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/types/imio.events.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1659 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/types/imio.events.Event.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1345 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/types/imio.events.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      362 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/default/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      126 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/profiles.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/rest/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/rest/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/rest/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3008 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/rest/endpoint.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      667 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/setuphandlers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5607 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/subscribers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1308 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1873 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/testing.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/tests/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/resources/plone.png
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2852 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1995 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8078 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_agenda.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1573 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3566 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_entity.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14464 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_event.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4202 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_folder.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9739 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_indexes.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2204 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_local_roles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7860 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_multilingual.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5919 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_rest.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      935 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1971 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7479 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5147 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/test_vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/tests/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/upgrades/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3567 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/upgrades/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio/events/core/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/upgrades/profiles/1002_to_1003/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/upgrades/profiles/1002_to_1003/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.361954 imio.events.core-1.1.5/src/imio/events/core/upgrades/profiles/1005_to_1006/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3666 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3772 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4548 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1006 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio/events/core/vocabularies.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 12:17:15.357954 imio.events.core-1.1.5/src/imio.events.core.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6037 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio.events.core.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4269 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio.events.core.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio.events.core.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       17 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio.events.core.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio.events.core.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio.events.core.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-03-31 12:17:15.000000 imio.events.core-1.1.5/src/imio.events.core.egg-info/top_level.txt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.229793 imio.events.core-1.1.6/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3127 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      651 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6181 2023-05-05 07:45:56.229793 imio.events.core-1.1.6/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1993 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/README.rst
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.213793 imio.events.core-1.1.6/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7958 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/docs/conf.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       71 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-05-05 07:45:56.229793 imio.events.core-1.1.6/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2536 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.201793 imio.events.core-1.1.6/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.213793 imio.events.core-1.1.6/src/imio/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.213793 imio.events.core-1.1.6/src/imio/events/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.217793 imio.events.core-1.1.6/src/imio/events/core/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      267 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.217793 imio.events.core-1.1.6/src/imio/events/core/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/browser/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      920 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/browser/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      387 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/browser/json_recurrence.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.217793 imio.events.core-1.1.6/src/imio/events/core/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/browser/overrides/.gitkeep
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.217793 imio.events.core-1.1.6/src/imio/events/core/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/browser/static/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1472 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/browser/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      850 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.217793 imio.events.core-1.1.6/src/imio/events/core/contents/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.217793 imio.events.core-1.1.6/src/imio/events/core/contents/agenda/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/agenda/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/agenda/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1264 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/agenda/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      198 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.221793 imio.events.core-1.1.6/src/imio/events/core/contents/entity/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/entity/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/entity/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1153 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/entity/content.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.221793 imio.events.core-1.1.6/src/imio/events/core/contents/event/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/event/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      664 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/event/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6641 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/event/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2785 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/event/serializer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8341 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/event/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4323 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/event/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.221793 imio.events.core-1.1.6/src/imio/events/core/contents/folder/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/folder/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/folder/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/contents/folder/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/converters.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.201793 imio.events.core-1.1.6/src/imio/events/core/faceted/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.221793 imio.events.core-1.1.6/src/imio/events/core/faceted/config/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8038 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/faceted/config/events.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5107 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/indexers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1795 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/indexers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      201 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/overrides.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      520 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.205793 imio.events.core-1.1.6/src/imio/events/core/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.221793 imio.events.core-1.1.6/src/imio/events/core/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2525 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      590 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      685 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      840 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.221793 imio.events.core-1.1.6/src/imio/events/core/profiles/default/taxonomies/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/taxonomies/event_public.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4154 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/taxonomies/event_public.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.225793 imio.events.core-1.1.6/src/imio/events/core/profiles/default/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/types/Plone_Site.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1386 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1583 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/types/imio.events.Entity.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1659 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/types/imio.events.Event.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1345 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/types/imio.events.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      362 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/default/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.225793 imio.events.core-1.1.6/src/imio/events/core/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      126 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/profiles.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.225793 imio.events.core-1.1.6/src/imio/events/core/rest/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/rest/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/rest/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3059 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/rest/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      667 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/setuphandlers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5607 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/subscribers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1308 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/subscribers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1873 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/testing.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.225793 imio.events.core-1.1.6/src/imio/events/core/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.225793 imio.events.core-1.1.6/src/imio/events/core/tests/resources/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/resources/plone.png
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.225793 imio.events.core-1.1.6/src/imio/events/core/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2852 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1995 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8078 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_agenda.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1573 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_cropping.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3566 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_entity.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14464 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_event.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4202 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_folder.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9739 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_indexes.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2204 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_local_roles.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7860 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_multilingual.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5919 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_rest.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      935 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_robot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1971 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7479 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5147 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/test_vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/tests/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.225793 imio.events.core-1.1.6/src/imio/events/core/upgrades/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/upgrades/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3567 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/upgrades/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.209793 imio.events.core-1.1.6/src/imio/events/core/upgrades/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.225793 imio.events.core-1.1.6/src/imio/events/core/upgrades/profiles/1002_to_1003/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/upgrades/profiles/1002_to_1003/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.225793 imio.events.core-1.1.6/src/imio/events/core/upgrades/profiles/1005_to_1006/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3666 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/upgrades/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3772 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4548 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1006 2023-05-05 07:45:55.000000 imio.events.core-1.1.6/src/imio/events/core/vocabularies.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-05 07:45:56.213793 imio.events.core-1.1.6/src/imio.events.core.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6181 2023-05-05 07:45:56.000000 imio.events.core-1.1.6/src/imio.events.core.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4317 2023-05-05 07:45:56.000000 imio.events.core-1.1.6/src/imio.events.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-05-05 07:45:56.000000 imio.events.core-1.1.6/src/imio.events.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       17 2023-05-05 07:45:56.000000 imio.events.core-1.1.6/src/imio.events.core.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-05-05 07:45:56.000000 imio.events.core-1.1.6/src/imio.events.core.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-05-05 07:45:56.000000 imio.events.core-1.1.6/src/imio.events.core.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-05-05 07:45:56.000000 imio.events.core-1.1.6/src/imio.events.core.egg-info/top_level.txt
```

### Comparing `imio.events.core-1.1.5/CHANGES.rst` & `imio.events.core-1.1.6/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 Changelog
 =========
 
 
+1.1.6 (2023-05-05)
+------------------
+
+- INFRA-4725 : Add logging to find infinite loop in recurrence calculation
+  [laulaz]
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+
 1.1.5 (2023-03-31)
 ------------------
 
 - Need fullobjects in query to avoid "Cannot read properties of undefined (reading 'latitude')" in rest view
   So, we need to serialize first_start and first_end from obj.start and obj.end. If we don't do that, we got brain.start/end
   these are updates with first valid event occurence
   [boulch]
```

### Comparing `imio.events.core-1.1.5/DEVELOP.rst` & `imio.events.core-1.1.6/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/LICENSE.GPL` & `imio.events.core-1.1.6/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/LICENSE.rst` & `imio.events.core-1.1.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/PKG-INFO` & `imio.events.core-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: imio.events.core
-Version: 1.1.5
+Version: 1.1.6
 Summary: Core product for iMio events website
 Home-page: https://github.com/collective/imio.events.core
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.events.core
 Project-URL: Source, https://github.com/collective/imio.events.core
 Project-URL: Tracker, https://github.com/collective/imio.events.core/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -120,14 +119,24 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.1.6 (2023-05-05)
+------------------
+
+- INFRA-4725 : Add logging to find infinite loop in recurrence calculation
+  [laulaz]
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+
 1.1.5 (2023-03-31)
 ------------------
 
 - Need fullobjects in query to avoid "Cannot read properties of undefined (reading 'latitude')" in rest view
   So, we need to serialize first_start and first_end from obj.start and obj.end. If we don't do that, we got brain.start/end
   these are updates with first valid event occurence
   [boulch]
@@ -261,9 +270,7 @@
 
 
 1.0a1 (2022-01-25)
 ------------------
 
 - Initial release.
   [boulch]
-
-
```

### Comparing `imio.events.core-1.1.5/README.rst` & `imio.events.core-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/docs/conf.py` & `imio.events.core-1.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/setup.cfg` & `imio.events.core-1.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/setup.py` & `imio.events.core-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.events.core",
-    version="1.1.5",
+    version="1.1.6",
     description="Core product for iMio events website",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imio.events.core-1.1.5/src/imio/events/core/browser/configure.zcml` & `imio.events.core-1.1.6/src/imio/events/core/browser/configure.zcml`

 * *Files 21% similar despite different names*

```diff
@@ -21,9 +21,16 @@
     name="utils"
     for="*"
     class=".utils.UtilsView"
     permission="zope2.View"
     layer="imio.events.core.interfaces.IImioEventsCoreLayer"
     />
 
+  <browser:page
+    name="json_recurrence"
+    for="*"
+    class=".json_recurrence.LoggingRecurrenceView"
+    permission="zope2.View"
+    layer="imio.events.core.interfaces.IImioEventsCoreLayer"
+    />
 
 </configure>
```

### Comparing `imio.events.core-1.1.5/src/imio/events/core/browser/utils.py` & `imio.events.core-1.1.6/src/imio/events/core/browser/utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/configure.zcml` & `imio.events.core-1.1.6/src/imio/events/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/contents/agenda/content.py` & `imio.events.core-1.1.6/src/imio/events/core/contents/agenda/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/contents/entity/content.py` & `imio.events.core-1.1.6/src/imio/events/core/contents/entity/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/contents/event/configure.zcml` & `imio.events.core-1.1.6/src/imio/events/core/contents/event/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/contents/event/content.py` & `imio.events.core-1.1.6/src/imio/events/core/contents/event/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/contents/event/serializer.py` & `imio.events.core-1.1.6/src/imio/events/core/contents/event/serializer.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/contents/event/view.pt` & `imio.events.core-1.1.6/src/imio/events/core/contents/event/view.pt`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/contents/event/views.py` & `imio.events.core-1.1.6/src/imio/events/core/contents/event/views.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/faceted/config/events.xml` & `imio.events.core-1.1.6/src/imio/events/core/faceted/config/events.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/indexers.py` & `imio.events.core-1.1.6/src/imio/events/core/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/indexers.zcml` & `imio.events.core-1.1.6/src/imio/events/core/indexers.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/permissions.zcml` & `imio.events.core-1.1.6/src/imio/events/core/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/profiles/default/catalog.xml` & `imio.events.core-1.1.6/src/imio/events/core/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/profiles/default/metadata.xml` & `imio.events.core-1.1.6/src/imio/events/core/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/profiles/default/registry.xml` & `imio.events.core-1.1.6/src/imio/events/core/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/profiles/default/rolemap.xml` & `imio.events.core-1.1.6/src/imio/events/core/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/profiles/default/taxonomies/event_public.xml` & `imio.events.core-1.1.6/src/imio/events/core/profiles/default/taxonomies/event_public.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml` & `imio.events.core-1.1.6/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/profiles/default/types/imio.events.Entity.xml` & `imio.events.core-1.1.6/src/imio/events/core/profiles/default/types/imio.events.Entity.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/profiles/default/types/imio.events.Event.xml` & `imio.events.core-1.1.6/src/imio/events/core/profiles/default/types/imio.events.Event.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/profiles/default/types/imio.events.Folder.xml` & `imio.events.core-1.1.6/src/imio/events/core/profiles/default/types/imio.events.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/profiles.zcml` & `imio.events.core-1.1.6/src/imio/events/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/rest/endpoint.py` & `imio.events.core-1.1.6/src/imio/events/core/rest/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,23 +52,26 @@
 
         self._constrain_query_by_path(query)
         query = self._parse_query(query)
         lazy_resultset = self.catalog.searchResults(**query)
         if "metadata_fields" not in self.request.form:
             self.request.form["metadata_fields"] = []
         self.request.form["metadata_fields"] += [
-        "recurrence",
-        "whole_day",
-        "first_start",
-        "first_end",
-        "open_end",]
+            "recurrence",
+            "whole_day",
+            "first_start",
+            "first_end",
+            "open_end",
+        ]
         # ISerializeToJson use a default request batch so we force a "full" b_size and a "zero" b_start
         self.request.form["b_size"] = 10000
         self.request.form["b_start"] = 0
-        results = getMultiAdapter((lazy_resultset, self.request), ISerializeToJson)(fullobjects=fullobjects)
+        results = getMultiAdapter((lazy_resultset, self.request), ISerializeToJson)(
+            fullobjects=fullobjects
+        )
         expanded_occurences = expand_occurences(results.get("items"))
         sorted_expanded_occurences = sorted(expanded_occurences, key=get_start_date)
 
         # It's time to get real b_size/b_start from the smartweb query
         self.request.form["b_size"] = b_size
         self.request.form["b_start"] = b_start
         batch = HypermediaBatch(self.request, sorted_expanded_occurences)
```

### Comparing `imio.events.core-1.1.5/src/imio/events/core/setuphandlers.py` & `imio.events.core-1.1.6/src/imio/events/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/subscribers.py` & `imio.events.core-1.1.6/src/imio/events/core/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/subscribers.zcml` & `imio.events.core-1.1.6/src/imio/events/core/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/testing.py` & `imio.events.core-1.1.6/src/imio/events/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/resources/plone.png` & `imio.events.core-1.1.6/src/imio/events/core/tests/resources/plone.png`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot` & `imio.events.core-1.1.6/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot` & `imio.events.core-1.1.6/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot` & `imio.events.core-1.1.6/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/robot/test_example.robot` & `imio.events.core-1.1.6/src/imio/events/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_agenda.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_agenda.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_cropping.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_entity.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_event.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_folder.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_indexes.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_local_roles.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_multilingual.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_multilingual.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_rest.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_robot.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_setup.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_utils.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/tests/test_vocabularies.py` & `imio.events.core-1.1.6/src/imio/events/core/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/upgrades/configure.zcml` & `imio.events.core-1.1.6/src/imio/events/core/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml` & `imio.events.core-1.1.6/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/upgrades/upgrades.py` & `imio.events.core-1.1.6/src/imio/events/core/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/utils.py` & `imio.events.core-1.1.6/src/imio/events/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/vocabularies.py` & `imio.events.core-1.1.6/src/imio/events/core/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio/events/core/vocabularies.zcml` & `imio.events.core-1.1.6/src/imio/events/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.5/src/imio.events.core.egg-info/PKG-INFO` & `imio.events.core-1.1.6/src/imio.events.core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: imio.events.core
-Version: 1.1.5
+Version: 1.1.6
 Summary: Core product for iMio events website
 Home-page: https://github.com/collective/imio.events.core
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.events.core
 Project-URL: Source, https://github.com/collective/imio.events.core
 Project-URL: Tracker, https://github.com/collective/imio.events.core/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -120,14 +119,24 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.1.6 (2023-05-05)
+------------------
+
+- INFRA-4725 : Add logging to find infinite loop in recurrence calculation
+  [laulaz]
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+
 1.1.5 (2023-03-31)
 ------------------
 
 - Need fullobjects in query to avoid "Cannot read properties of undefined (reading 'latitude')" in rest view
   So, we need to serialize first_start and first_end from obj.start and obj.end. If we don't do that, we got brain.start/end
   these are updates with first valid event occurence
   [boulch]
@@ -261,9 +270,7 @@
 
 
 1.0a1 (2022-01-25)
 ------------------
 
 - Initial release.
   [boulch]
-
-
```

### Comparing `imio.events.core-1.1.5/src/imio.events.core.egg-info/SOURCES.txt` & `imio.events.core-1.1.6/src/imio.events.core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/imio/events/core/subscribers.zcml
 src/imio/events/core/testing.py
 src/imio/events/core/utils.py
 src/imio/events/core/vocabularies.py
 src/imio/events/core/vocabularies.zcml
 src/imio/events/core/browser/__init__.py
 src/imio/events/core/browser/configure.zcml
+src/imio/events/core/browser/json_recurrence.py
 src/imio/events/core/browser/utils.py
 src/imio/events/core/browser/overrides/.gitkeep
 src/imio/events/core/browser/static/.gitkeep
 src/imio/events/core/contents/__init__.py
 src/imio/events/core/contents/configure.zcml
 src/imio/events/core/contents/agenda/__init__.py
 src/imio/events/core/contents/agenda/configure.zcml
```

