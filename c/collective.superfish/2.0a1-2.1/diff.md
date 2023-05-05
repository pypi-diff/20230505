# Comparing `tmp/collective.superfish-2.0a1.tar.gz` & `tmp/collective.superfish-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.superfish-2.0a1.tar", last modified: Fri Nov 24 09:23:19 2017, max compression
+gzip compressed data, was "collective.superfish-2.1.tar", last modified: Fri May  5 09:00:46 2023, max compression
```

## Comparing `collective.superfish-2.0a1.tar` & `collective.superfish-2.1.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/
--rw-r--r--   0 peterm     (501) staff       (20)     8678 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/PKG-INFO
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/
--rw-r--r--   0 peterm     (501) staff       (20)      244 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/superfish/
--rw-r--r--   0 peterm     (501) staff       (20)      428 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/interfaces.py
--rw-r--r--   0 peterm     (501) staff       (20)      914 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/superfish/browser/
--rw-r--r--   0 peterm     (501) staff       (20)      256 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/interfaces.py
--rw-r--r--   0 peterm     (501) staff       (20)      640 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     8596 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/sections.py
--rw-r--r--   0 peterm     (501) staff       (20)       24 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/superfish/browser/static/
--rw-r--r--   0 peterm     (501) staff       (20)     1283 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/pattern.less
--rw-r--r--   0 peterm     (501) staff       (20)     6882 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/superfish-hoverIntent-compiled.js
--rw-r--r--   0 peterm     (501) staff       (20)     3165 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/superfish-pattern-compiled.js
--rw-r--r--   0 peterm     (501) staff       (20)     3040 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/pattern.js
--rw-r--r--   0 peterm     (501) staff       (20)     1755 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/superfish.less
--rw-r--r--   0 peterm     (501) staff       (20)      185 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/bundle.js
--rw-r--r--   0 peterm     (501) staff       (20)     7618 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/superfish.js
--rw-r--r--   0 peterm     (501) staff       (20)     9989 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/superfish.min.css.map
--rw-r--r--   0 peterm     (501) staff       (20)     7745 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/superfish-compiled.js
--rw-r--r--   0 peterm     (501) staff       (20)    72552 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/superfish.min.js.map
--rw-r--r--   0 peterm     (501) staff       (20)   141244 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/bundle-superfish-compiled.js
--rw-r--r--   0 peterm     (501) staff       (20)     6753 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/hoverIntent.js
--rw-r--r--   0 peterm     (501) staff       (20)     2078 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/superfish.min.css
--rw-r--r--   0 peterm     (501) staff       (20)    51950 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/static/superfish.min.js
--rw-r--r--   0 peterm     (501) staff       (20)      739 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/browser/sections.pt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/superfish/upgrades/
--rw-r--r--   0 peterm     (501) staff       (20)      911 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/upgrades/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)      692 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/upgrades/profiles.zcml
--rw-r--r--   0 peterm     (501) staff       (20)      411 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/upgrades/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/superfish/upgrades/profiles/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/superfish/upgrades/profiles/2_to_5/
--rw-r--r--   0 peterm     (501) staff       (20)      349 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/upgrades/profiles/2_to_5/jsregistry.xml
--rw-r--r--   0 peterm     (501) staff       (20)     1904 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/upgrades/profiles/2_to_5/registry.xml
--rw-r--r--   0 peterm     (501) staff       (20)      284 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/upgrades/profiles/2_to_5/cssregistry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/superfish/upgrades/profiles/1_to_2/
--rw-r--r--   0 peterm     (501) staff       (20)      535 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/upgrades/profiles/1_to_2/cssregistry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/superfish/profiles/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/superfish/profiles/default/
--rw-r--r--   0 peterm     (501) staff       (20)     2328 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/profiles/default/registry.xml
--rw-r--r--   0 peterm     (501) staff       (20)      163 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/profiles/default/browserlayer.xml
--rw-r--r--   0 peterm     (501) staff       (20)       70 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/profiles/default/metadata.xml
--rw-r--r--   0 peterm     (501) staff       (20)      148 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/profiles/default/viewlets.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective/superfish/profiles/uninstall/
--rw-r--r--   0 peterm     (501) staff       (20)      517 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/profiles/uninstall/registry.xml
--rw-r--r--   0 peterm     (501) staff       (20)      188 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 peterm     (501) staff       (20)      272 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/profiles/uninstall/viewlets.xml
--rw-r--r--   0 peterm     (501) staff       (20)     1349 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/collective/superfish/tests.py
--rw-r--r--   0 peterm     (501) staff       (20)      119 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/MANIFEST.in
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/docs/
--rw-r--r--   0 peterm     (501) staff       (20)      365 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/docs/TODO.txt
--rw-r--r--   0 peterm     (501) staff       (20)    12282 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/docs/LICENSE.GPL
--rw-r--r--   0 peterm     (501) staff       (20)     1660 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/docs/INSTALL.txt
--rw-r--r--   0 peterm     (501) staff       (20)      361 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/docs/THANKS.txt
--rw-r--r--   0 peterm     (501) staff       (20)     4181 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/docs/HISTORY.txt
--rw-r--r--   0 peterm     (501) staff       (20)      751 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/docs/LICENSE.txt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective.superfish.egg-info/
--rw-r--r--   0 peterm     (501) staff       (20)     8678 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective.superfish.egg-info/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)        1 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective.superfish.egg-info/not-zip-safe
--rw-r--r--   0 peterm     (501) staff       (20)       11 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective.superfish.egg-info/namespace_packages.txt
--rw-r--r--   0 peterm     (501) staff       (20)     2389 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective.superfish.egg-info/SOURCES.txt
--rw-r--r--   0 peterm     (501) staff       (20)       53 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective.superfish.egg-info/entry_points.txt
--rw-r--r--   0 peterm     (501) staff       (20)       11 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective.superfish.egg-info/requires.txt
--rw-r--r--   0 peterm     (501) staff       (20)       11 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective.superfish.egg-info/top_level.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/collective.superfish.egg-info/dependency_links.txt
--rw-r--r--   0 peterm     (501) staff       (20)     1375 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/setup.py
--rw-r--r--   0 peterm     (501) staff       (20)       98 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/.gitignore
--rw-r--r--   0 peterm     (501) staff       (20)       38 2017-11-24 09:23:19.000000 collective.superfish-2.0a1/setup.cfg
--rw-r--r--   0 peterm     (501) staff       (20)     1351 2017-11-24 09:23:18.000000 collective.superfish-2.0a1/README.rst
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.287103 collective.superfish-2.1/
+-rw-r--r--   0 peterm     (501) staff       (20)     4297 2023-05-05 09:00:45.000000 collective.superfish-2.1/CHANGES.rst
+-rw-r--r--   0 peterm     (501) staff       (20)       92 2023-05-05 09:00:45.000000 collective.superfish-2.1/MANIFEST.in
+-rw-r--r--   0 peterm     (501) staff       (20)     7292 2023-05-05 09:00:46.287161 collective.superfish-2.1/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     1351 2023-05-05 09:00:45.000000 collective.superfish-2.1/README.rst
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.280628 collective.superfish-2.1/collective/
+-rw-r--r--   0 peterm     (501) staff       (20)      244 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.282098 collective.superfish-2.1/collective/superfish/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.282734 collective.superfish-2.1/collective/superfish/browser/
+-rw-r--r--   0 peterm     (501) staff       (20)       24 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)      640 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)      256 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/interfaces.py
+-rw-r--r--   0 peterm     (501) staff       (20)      739 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/sections.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     8489 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/sections.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.284631 collective.superfish-2.1/collective/superfish/browser/static/
+-rw-r--r--   0 peterm     (501) staff       (20)   141244 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/bundle-superfish-compiled.js
+-rw-r--r--   0 peterm     (501) staff       (20)      185 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/bundle.js
+-rw-r--r--   0 peterm     (501) staff       (20)     6753 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/hoverIntent.js
+-rw-r--r--   0 peterm     (501) staff       (20)     3040 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/pattern.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1283 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/pattern.less
+-rw-r--r--   0 peterm     (501) staff       (20)     7745 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/superfish-compiled.js
+-rw-r--r--   0 peterm     (501) staff       (20)     6882 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/superfish-hoverIntent-compiled.js
+-rw-r--r--   0 peterm     (501) staff       (20)     3165 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/superfish-pattern-compiled.js
+-rw-r--r--   0 peterm     (501) staff       (20)     7618 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/superfish.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1755 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/superfish.less
+-rw-r--r--   0 peterm     (501) staff       (20)     2078 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/superfish.min.css
+-rw-r--r--   0 peterm     (501) staff       (20)     9989 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/superfish.min.css.map
+-rw-r--r--   0 peterm     (501) staff       (20)    51950 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/superfish.min.js
+-rw-r--r--   0 peterm     (501) staff       (20)    72552 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/browser/static/superfish.min.js.map
+-rw-r--r--   0 peterm     (501) staff       (20)      914 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)      428 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/interfaces.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.279522 collective.superfish-2.1/collective/superfish/profiles/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.285177 collective.superfish-2.1/collective/superfish/profiles/default/
+-rw-r--r--   0 peterm     (501) staff       (20)      163 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/profiles/default/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)       70 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/profiles/default/metadata.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     2328 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/profiles/default/registry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      148 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/profiles/default/viewlets.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.285538 collective.superfish-2.1/collective/superfish/profiles/uninstall/
+-rw-r--r--   0 peterm     (501) staff       (20)      188 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      517 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/profiles/uninstall/registry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      272 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/profiles/uninstall/viewlets.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     1349 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/tests.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.285910 collective.superfish-2.1/collective/superfish/upgrades/
+-rw-r--r--   0 peterm     (501) staff       (20)      411 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/upgrades/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)      911 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/upgrades/configure.zcml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.279817 collective.superfish-2.1/collective/superfish/upgrades/profiles/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.286031 collective.superfish-2.1/collective/superfish/upgrades/profiles/1_to_2/
+-rw-r--r--   0 peterm     (501) staff       (20)      535 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/upgrades/profiles/1_to_2/cssregistry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.286402 collective.superfish-2.1/collective/superfish/upgrades/profiles/2_to_5/
+-rw-r--r--   0 peterm     (501) staff       (20)      284 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/upgrades/profiles/2_to_5/cssregistry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      349 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/upgrades/profiles/2_to_5/jsregistry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     1904 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/upgrades/profiles/2_to_5/registry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      692 2023-05-05 09:00:45.000000 collective.superfish-2.1/collective/superfish/upgrades/profiles.zcml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.281615 collective.superfish-2.1/collective.superfish.egg-info/
+-rw-r--r--   0 peterm     (501) staff       (20)     7292 2023-05-05 09:00:46.000000 collective.superfish-2.1/collective.superfish.egg-info/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     2383 2023-05-05 09:00:46.000000 collective.superfish-2.1/collective.superfish.egg-info/SOURCES.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-05-05 09:00:46.000000 collective.superfish-2.1/collective.superfish.egg-info/dependency_links.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       40 2023-05-05 09:00:46.000000 collective.superfish-2.1/collective.superfish.egg-info/entry_points.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       11 2023-05-05 09:00:46.000000 collective.superfish-2.1/collective.superfish.egg-info/namespace_packages.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-05-05 09:00:46.000000 collective.superfish-2.1/collective.superfish.egg-info/not-zip-safe
+-rw-r--r--   0 peterm     (501) staff       (20)       11 2023-05-05 09:00:46.000000 collective.superfish-2.1/collective.superfish.egg-info/requires.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       11 2023-05-05 09:00:46.000000 collective.superfish-2.1/collective.superfish.egg-info/top_level.txt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-05 09:00:46.286991 collective.superfish-2.1/docs/
+-rw-r--r--   0 peterm     (501) staff       (20)     1660 2023-05-05 09:00:45.000000 collective.superfish-2.1/docs/INSTALL.txt
+-rw-r--r--   0 peterm     (501) staff       (20)    12282 2023-05-05 09:00:45.000000 collective.superfish-2.1/docs/LICENSE.GPL
+-rw-r--r--   0 peterm     (501) staff       (20)      751 2023-05-05 09:00:45.000000 collective.superfish-2.1/docs/LICENSE.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      361 2023-05-05 09:00:45.000000 collective.superfish-2.1/docs/THANKS.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      365 2023-05-05 09:00:45.000000 collective.superfish-2.1/docs/TODO.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      102 2023-05-05 09:00:46.287382 collective.superfish-2.1/setup.cfg
+-rw-r--r--   0 peterm     (501) staff       (20)     1713 2023-05-05 09:00:45.000000 collective.superfish-2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.superfish-2.0a1/collective/superfish/configure.zcml` & `collective.superfish-2.1/collective/superfish/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/configure.zcml` & `collective.superfish-2.1/collective/superfish/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/sections.py` & `collective.superfish-2.1/collective/superfish/browser/sections.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 # -*- coding: utf-8 -*-
 from AccessControl import getSecurityManager
 from Acquisition import aq_inner
-from Products.CMFCore.utils import getToolByName
-from Products.CMFPlone.browser.navtree import SitemapQueryBuilder
-from Products.CMFPlone.utils import safe_unicode
-from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
-from cStringIO import StringIO
 from collective.superfish.interfaces import ISuperfishSettings
 from plone.app.layout.navigation.navtree import buildFolderTree
 from plone.app.layout.viewlets import common
 from plone.registry.interfaces import IRegistry
+from Products.CMFCore.utils import getToolByName
+from Products.CMFPlone.browser.navtree import SitemapQueryBuilder
+from Products.CMFPlone.utils import safe_unicode
+from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zope.component import getMultiAdapter
 from zope.component import queryUtility
 from zope.i18n import translate
 
 
 def _render_sections_cachekey(fun, self):
-    key = StringIO()
-    print >> key, self.__class__
-    print >> key, getToolByName(aq_inner(self.context), 'portal_url')()
-    print >> key, self.request.get('LANGUAGE', 'de')
-
     catalog = getToolByName(self.context, 'portal_catalog')
     counter = catalog.getCounter()
-    print >> key, counter
-    print >> key, aq_inner(self.context).getPhysicalPath()
-
     user = getSecurityManager().getUser()
     roles = user.getRolesInContext(aq_inner(self.context))
-    print >> key, roles
-
-    return key.getvalue()
+    return "".join([
+        self.__class__,
+        getToolByName(aq_inner(self.context), 'portal_url')(),
+        self.request.get('LANGUAGE', 'de'),
+        counter,
+        aq_inner(self.context).getPhysicalPath(),
+        roles,
+    ])
 
 
 class VirtualCatalogBrain(object):
     """wraps an portal_action actioninfo into a fake catalog brain that can
     be used as item in the dictiontary returned by
     plone.app.layout.navigation.navtree.buildFolderTree
     """
```

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/pattern.less` & `collective.superfish-2.1/collective/superfish/browser/static/pattern.less`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/superfish-hoverIntent-compiled.js` & `collective.superfish-2.1/collective/superfish/browser/static/superfish-hoverIntent-compiled.js`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/superfish-pattern-compiled.js` & `collective.superfish-2.1/collective/superfish/browser/static/superfish-pattern-compiled.js`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/pattern.js` & `collective.superfish-2.1/collective/superfish/browser/static/pattern.js`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/superfish.less` & `collective.superfish-2.1/collective/superfish/browser/static/superfish.less`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/superfish.js` & `collective.superfish-2.1/collective/superfish/browser/static/superfish.js`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/superfish.min.css.map` & `collective.superfish-2.1/collective/superfish/browser/static/superfish.min.css.map`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/superfish-compiled.js` & `collective.superfish-2.1/collective/superfish/browser/static/superfish-compiled.js`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/superfish.min.js.map` & `collective.superfish-2.1/collective/superfish/browser/static/superfish.min.js.map`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/bundle-superfish-compiled.js` & `collective.superfish-2.1/collective/superfish/browser/static/bundle-superfish-compiled.js`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/hoverIntent.js` & `collective.superfish-2.1/collective/superfish/browser/static/hoverIntent.js`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/superfish.min.css` & `collective.superfish-2.1/collective/superfish/browser/static/superfish.min.css`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/static/superfish.min.js` & `collective.superfish-2.1/collective/superfish/browser/static/superfish.min.js`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/browser/sections.pt` & `collective.superfish-2.1/collective/superfish/browser/sections.pt`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/upgrades/configure.zcml` & `collective.superfish-2.1/collective/superfish/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/upgrades/profiles.zcml` & `collective.superfish-2.1/collective/superfish/upgrades/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/upgrades/profiles/2_to_5/registry.xml` & `collective.superfish-2.1/collective/superfish/upgrades/profiles/2_to_5/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/upgrades/profiles/1_to_2/cssregistry.xml` & `collective.superfish-2.1/collective/superfish/upgrades/profiles/1_to_2/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/profiles/default/registry.xml` & `collective.superfish-2.1/collective/superfish/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/profiles/uninstall/registry.xml` & `collective.superfish-2.1/collective/superfish/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective/superfish/tests.py` & `collective.superfish-2.1/collective/superfish/tests.py`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/docs/LICENSE.GPL` & `collective.superfish-2.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/docs/INSTALL.txt` & `collective.superfish-2.1/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/docs/HISTORY.txt` & `collective.superfish-2.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 History
 =======
 
+2.1 (2023-05-05)
+----------------
+
+- Python 3 support.
+
+
+2.0 (2018-08-02)
+----------------
+
+- make final release.
+
+
 2.0a1 (2017-11-24)
 ------------------
 
 - migrate superfish resources to Plone 5 resource registry (see upgrade step)
   [petschki]
 - behave as "drop-in" replacement for global_sections
   [petschki]
```

### Comparing `collective.superfish-2.0a1/docs/LICENSE.txt` & `collective.superfish-2.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.superfish-2.0a1/collective.superfish.egg-info/SOURCES.txt` & `collective.superfish-2.1/collective.superfish.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-.gitignore
+CHANGES.rst
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 collective/__init__.py
 collective.superfish.egg-info/PKG-INFO
 collective.superfish.egg-info/SOURCES.txt
 collective.superfish.egg-info/dependency_links.txt
 collective.superfish.egg-info/entry_points.txt
 collective.superfish.egg-info/namespace_packages.txt
@@ -44,13 +45,12 @@
 collective/superfish/upgrades/__init__.py
 collective/superfish/upgrades/configure.zcml
 collective/superfish/upgrades/profiles.zcml
 collective/superfish/upgrades/profiles/1_to_2/cssregistry.xml
 collective/superfish/upgrades/profiles/2_to_5/cssregistry.xml
 collective/superfish/upgrades/profiles/2_to_5/jsregistry.xml
 collective/superfish/upgrades/profiles/2_to_5/registry.xml
-docs/HISTORY.txt
 docs/INSTALL.txt
 docs/LICENSE.GPL
 docs/LICENSE.txt
 docs/THANKS.txt
 docs/TODO.txt
```

### Comparing `collective.superfish-2.0a1/setup.py` & `collective.superfish-2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,35 +7,42 @@
 
 def read(*pathnames):
     return open(os.path.join(os.path.dirname(__file__), *pathnames)).read()
 
 
 setup(
     name='collective.superfish',
-    version='2.0a1',
+    version='2.1',
     description="A suckerfish/superfish integration into plone",
     long_description='\n'.join([
         read('README.rst'),
         read('docs', 'TODO.txt'),
-        read('docs', 'HISTORY.txt'),
         read('docs', 'THANKS.txt'),
+        read('CHANGES.rst'),
     ]),
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
+        "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 5.0",
         "Framework :: Plone :: 5.1",
+        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: Addon",
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
     ],
     keywords='navigation suckerfish superfish jquery dropdown',
     author='Peter Mathis',
     author_email='peter.mathis@kombinat.at',
-    url='http://svn.plone.org/svn/collective/collective.superfish',
+    url='https://github.com/collective/collective.superfish',
     license='GPL',
     packages=find_packages(exclude=['ez_setup']),
     namespace_packages=['collective'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'setuptools',
```

### Comparing `collective.superfish-2.0a1/README.rst` & `collective.superfish-2.1/README.rst`

 * *Files identical despite different names*

