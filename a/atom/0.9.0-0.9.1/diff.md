# Comparing `tmp/atom-0.9.0.tar.gz` & `tmp/atom-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atom-0.9.0.tar", last modified: Tue Feb 21 12:18:53 2023, max compression
+gzip compressed data, was "atom-0.9.1.tar", last modified: Mon Mar 13 12:30:33 2023, max compression
```

## Comparing `atom-0.9.0.tar` & `atom-0.9.1.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.328174 atom-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-21 12:18:35.000000 atom-0.9.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-21 12:18:35.000000 atom-0.9.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.284175 atom-0.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-21 12:18:35.000000 atom-0.9.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-21 12:18:35.000000 atom-0.9.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.284175 atom-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-02-21 12:18:35.000000 atom-0.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-02-21 12:18:35.000000 atom-0.9.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-02-21 12:18:35.000000 atom-0.9.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-02-21 12:18:35.000000 atom-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-21 12:18:35.000000 atom-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-21 12:18:35.000000 atom-0.9.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-02-21 12:18:35.000000 atom-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-21 12:18:35.000000 atom-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-02-21 12:18:53.328174 atom-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-02-21 12:18:35.000000 atom-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.292174 atom-0.9.0/atom/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-21 12:18:35.000000 atom-0.9.0/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-02-21 12:18:35.000000 atom-0.9.0/atom/annotation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-02-21 12:18:35.000000 atom-0.9.0/atom/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23252 2023-02-21 12:18:35.000000 atom-0.9.0/atom/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-02-21 12:18:35.000000 atom-0.9.0/atom/catom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-02-21 12:18:35.000000 atom-0.9.0/atom/coerced.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-02-21 12:18:35.000000 atom-0.9.0/atom/coerced.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-21 12:18:35.000000 atom-0.9.0/atom/containerlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-02-21 12:18:35.000000 atom-0.9.0/atom/containerlist.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.296175 atom-0.9.0/atom/datastructures/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-21 12:18:35.000000 atom-0.9.0/atom/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-21 12:18:35.000000 atom-0.9.0/atom/datastructures/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-21 12:18:35.000000 atom-0.9.0/atom/datastructures/sortedmap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-02-21 12:18:35.000000 atom-0.9.0/atom/delegator.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-21 12:18:35.000000 atom-0.9.0/atom/delegator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-02-21 12:18:35.000000 atom-0.9.0/atom/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-02-21 12:18:35.000000 atom-0.9.0/atom/dict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-02-21 12:18:35.000000 atom-0.9.0/atom/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-02-21 12:18:35.000000 atom-0.9.0/atom/enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-02-21 12:18:35.000000 atom-0.9.0/atom/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-21 12:18:35.000000 atom-0.9.0/atom/event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-02-21 12:18:35.000000 atom-0.9.0/atom/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    15804 2023-02-21 12:18:35.000000 atom-0.9.0/atom/instance.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-21 12:18:35.000000 atom-0.9.0/atom/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-02-21 12:18:35.000000 atom-0.9.0/atom/list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-02-21 12:18:35.000000 atom-0.9.0/atom/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-02-21 12:18:35.000000 atom-0.9.0/atom/property.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:35.000000 atom-0.9.0/atom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-02-21 12:18:35.000000 atom-0.9.0/atom/scalars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-02-21 12:18:35.000000 atom-0.9.0/atom/scalars.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-02-21 12:18:35.000000 atom-0.9.0/atom/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-02-21 12:18:35.000000 atom-0.9.0/atom/set.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-21 12:18:35.000000 atom-0.9.0/atom/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-21 12:18:35.000000 atom-0.9.0/atom/signal.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.304175 atom-0.9.0/atom/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/atomdict.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/atomdict.h
--rw-r--r--   0 runner    (1001) docker     (123)    32189 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/atomlist.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/atomlist.h
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/atomref.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/atomref.h
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/atomset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/atomset.h
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/behaviors.h
--rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/catom.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/catom.h
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/catommodule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/catompointer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/defaultvaluebehavior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/delattrbehavior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/enumtypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/enumtypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/eventbinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/eventbinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/getattrbehavior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/getstatebehavior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/globalstatic.h
--rw-r--r--   0 runner    (1001) docker     (123)    37507 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/member.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/member.h
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/memberchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/memberchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/methodwrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/methodwrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/modifyguard.h
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/msstdint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/observer.h
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/observerpool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/observerpool.h
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/packagenaming.h
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/platstdint.h
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/postgetattrbehavior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/postsetattrbehavior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/postvalidatebehavior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/propertyhelper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/propertyhelper.h
--rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/setattrbehavior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/signalconnector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/signalconnector.h
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/sortedmap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    25000 2023-02-21 12:18:35.000000 atom-0.9.0/atom/src/validatebehavior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-02-21 12:18:35.000000 atom-0.9.0/atom/subclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-02-21 12:18:35.000000 atom-0.9.0/atom/subclass.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-02-21 12:18:35.000000 atom-0.9.0/atom/tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-02-21 12:18:35.000000 atom-0.9.0/atom/tuple.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-02-21 12:18:35.000000 atom-0.9.0/atom/typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-02-21 12:18:35.000000 atom-0.9.0/atom/typed.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-02-21 12:18:35.000000 atom-0.9.0/atom/typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-21 12:18:53.000000 atom-0.9.0/atom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.292174 atom-0.9.0/atom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-02-21 12:18:53.000000 atom-0.9.0/atom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-02-21 12:18:53.000000 atom-0.9.0/atom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 12:18:53.000000 atom-0.9.0/atom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-21 12:18:53.000000 atom-0.9.0/atom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-21 12:18:53.000000 atom-0.9.0/atom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-21 12:18:35.000000 atom-0.9.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.304175 atom-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-02-21 12:18:35.000000 atom-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-02-21 12:18:35.000000 atom-0.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-21 12:18:35.000000 atom-0.9.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.304175 atom-0.9.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.308174 atom-0.9.0/docs/source/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/advanced/containers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/advanced/customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/advanced/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/advanced/manual_notifications.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/advanced/property.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/advanced/typing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/advanced/weakref.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.312174 atom-0.9.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.atom.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.catom.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.coerced.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.containerlist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.datastructures.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.delegator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.enum.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.event.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.instance.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.list.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.property.rst
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.scalars.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.signal.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.subclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.tuple.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/api/atom.typed.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.312174 atom-0.9.0/docs/source/basis/
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/basis/basis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/basis/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/basis/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/basis/mangled_methods.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/basis/members.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/basis/observation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/basis/typing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.312174 atom-0.9.0/docs/source/developer_notes/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/developer_notes/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.316174 atom-0.9.0/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_coersion.rst
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_composition.rst
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_containers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_default_value.rst
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_employee.rst
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_hello_world.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_inventory.rst
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_numeric.rst
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_observe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_observe_hints.rst
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_person.rst
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_property.rst
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_range.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/ex_static_type_checking.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/example_doc_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-02-21 12:18:35.000000 atom-0.9.0/docs/source/substitutions.sub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.280175 atom-0.9.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.316174 atom-0.9.0/examples/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-21 12:18:35.000000 atom-0.9.0/examples/api/coersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-02-21 12:18:35.000000 atom-0.9.0/examples/api/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-02-21 12:18:35.000000 atom-0.9.0/examples/api/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-02-21 12:18:35.000000 atom-0.9.0/examples/api/default_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-21 12:18:35.000000 atom-0.9.0/examples/api/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-21 12:18:35.000000 atom-0.9.0/examples/api/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-21 12:18:35.000000 atom-0.9.0/examples/api/observe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-21 12:18:35.000000 atom-0.9.0/examples/api/observe_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-21 12:18:35.000000 atom-0.9.0/examples/api/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-21 12:18:35.000000 atom-0.9.0/examples/api/range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.316174 atom-0.9.0/examples/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-02-21 12:18:35.000000 atom-0.9.0/examples/tutorial/employee.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-21 12:18:35.000000 atom-0.9.0/examples/tutorial/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-02-21 12:18:35.000000 atom-0.9.0/examples/tutorial/person.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.320174 atom-0.9.0/examples/typehints/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-21 12:18:35.000000 atom-0.9.0/examples/typehints/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-21 12:18:35.000000 atom-0.9.0/examples/typehints/static_type_checking.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-21 12:18:35.000000 atom-0.9.0/lint_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-02-21 12:18:35.000000 atom-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-02-21 12:18:35.000000 atom-0.9.0/releasenotes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 12:18:53.328174 atom-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-02-21 12:18:35.000000 atom-0.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-21 12:18:35.000000 atom-0.9.0/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.324174 atom-0.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.324174 atom-0.9.0/tests/datastructure/
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-02-21 12:18:35.000000 atom-0.9.0/tests/datastructure/test_sortedmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_atom_from_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_atomdict.py
--rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_atomlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_atomref.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_atomset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_default_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_del_behaviors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_delegator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_eventbinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_get_behaviors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_get_set_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_getstate_behaviors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    24110 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_observe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_post_behaviors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_set_behaviors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_signalconnector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-02-21 12:18:35.000000 atom-0.9.0/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:18:53.328174 atom-0.9.0/tests/type_checking/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_annotations.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_coerced.yml
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_delegator.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19382 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_dict.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_enum.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_event.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_generic_aliases.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_list.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_property.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_scalars.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_set.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_signal.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_subclass.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_tuple.yml
--rw-r--r--   0 runner    (1001) docker     (123)    30567 2023-02-21 12:18:35.000000 atom-0.9.0/tests/type_checking/test_typed_instance.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.529261 atom-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-13 12:30:16.000000 atom-0.9.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-13 12:30:16.000000 atom-0.9.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.489260 atom-0.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-13 12:30:16.000000 atom-0.9.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-13 12:30:16.000000 atom-0.9.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.489260 atom-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-03-13 12:30:16.000000 atom-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-13 12:30:16.000000 atom-0.9.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-03-13 12:30:16.000000 atom-0.9.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-03-13 12:30:16.000000 atom-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-13 12:30:16.000000 atom-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-13 12:30:16.000000 atom-0.9.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-03-13 12:30:16.000000 atom-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-13 12:30:16.000000 atom-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-03-13 12:30:33.529261 atom-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-13 12:30:16.000000 atom-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.497260 atom-0.9.1/atom/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-13 12:30:16.000000 atom-0.9.1/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-03-13 12:30:16.000000 atom-0.9.1/atom/annotation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-03-13 12:30:16.000000 atom-0.9.1/atom/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23252 2023-03-13 12:30:16.000000 atom-0.9.1/atom/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-03-13 12:30:16.000000 atom-0.9.1/atom/catom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-03-13 12:30:16.000000 atom-0.9.1/atom/coerced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-03-13 12:30:16.000000 atom-0.9.1/atom/coerced.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-13 12:30:16.000000 atom-0.9.1/atom/containerlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-13 12:30:16.000000 atom-0.9.1/atom/containerlist.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.497260 atom-0.9.1/atom/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-13 12:30:16.000000 atom-0.9.1/atom/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-13 12:30:16.000000 atom-0.9.1/atom/datastructures/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-13 12:30:16.000000 atom-0.9.1/atom/datastructures/sortedmap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-03-13 12:30:16.000000 atom-0.9.1/atom/delegator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-13 12:30:16.000000 atom-0.9.1/atom/delegator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-03-13 12:30:16.000000 atom-0.9.1/atom/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-03-13 12:30:16.000000 atom-0.9.1/atom/dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-13 12:30:16.000000 atom-0.9.1/atom/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-13 12:30:16.000000 atom-0.9.1/atom/enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-13 12:30:16.000000 atom-0.9.1/atom/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-13 12:30:16.000000 atom-0.9.1/atom/event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-03-13 12:30:16.000000 atom-0.9.1/atom/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15804 2023-03-13 12:30:16.000000 atom-0.9.1/atom/instance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-03-13 12:30:16.000000 atom-0.9.1/atom/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-13 12:30:16.000000 atom-0.9.1/atom/list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-03-13 12:30:16.000000 atom-0.9.1/atom/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-13 12:30:16.000000 atom-0.9.1/atom/property.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:16.000000 atom-0.9.1/atom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-03-13 12:30:16.000000 atom-0.9.1/atom/scalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-03-13 12:30:16.000000 atom-0.9.1/atom/scalars.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-13 12:30:16.000000 atom-0.9.1/atom/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-03-13 12:30:16.000000 atom-0.9.1/atom/set.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-13 12:30:16.000000 atom-0.9.1/atom/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-13 12:30:16.000000 atom-0.9.1/atom/signal.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.505261 atom-0.9.1/atom/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/atomdict.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/atomdict.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32189 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/atomlist.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/atomlist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/atomref.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/atomref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/atomset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/atomset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/behaviors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/catom.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/catom.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/catommodule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/catompointer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/defaultvaluebehavior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/delattrbehavior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/enumtypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/enumtypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/eventbinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/eventbinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/getattrbehavior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/getstatebehavior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/globalstatic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37507 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/member.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/member.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/memberchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/memberchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/methodwrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/methodwrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/modifyguard.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/msstdint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/observer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/observerpool.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/observerpool.h
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/packagenaming.h
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/platstdint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/postgetattrbehavior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/postsetattrbehavior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/postvalidatebehavior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/propertyhelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/propertyhelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/setattrbehavior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/signalconnector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/signalconnector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/sortedmap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25000 2023-03-13 12:30:16.000000 atom-0.9.1/atom/src/validatebehavior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-13 12:30:16.000000 atom-0.9.1/atom/subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-13 12:30:16.000000 atom-0.9.1/atom/subclass.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-13 12:30:16.000000 atom-0.9.1/atom/tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-13 12:30:16.000000 atom-0.9.1/atom/tuple.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-03-13 12:30:16.000000 atom-0.9.1/atom/typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-03-13 12:30:16.000000 atom-0.9.1/atom/typed.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-03-13 12:30:16.000000 atom-0.9.1/atom/typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-13 12:30:33.000000 atom-0.9.1/atom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.497260 atom-0.9.1/atom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-03-13 12:30:33.000000 atom-0.9.1/atom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-03-13 12:30:33.000000 atom-0.9.1/atom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 12:30:33.000000 atom-0.9.1/atom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-13 12:30:33.000000 atom-0.9.1/atom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-13 12:30:33.000000 atom-0.9.1/atom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-13 12:30:16.000000 atom-0.9.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.505261 atom-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-03-13 12:30:16.000000 atom-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-13 12:30:16.000000 atom-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-13 12:30:16.000000 atom-0.9.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.505261 atom-0.9.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.509261 atom-0.9.1/docs/source/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/advanced/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/advanced/customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/advanced/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/advanced/manual_notifications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/advanced/property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/advanced/typing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/advanced/weakref.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.513261 atom-0.9.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.catom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.coerced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.containerlist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.datastructures.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.delegator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.enum.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.event.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.instance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.scalars.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.signal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.subclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.tuple.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/api/atom.typed.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.513261 atom-0.9.1/docs/source/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/basis/basis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/basis/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/basis/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/basis/mangled_methods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/basis/members.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/basis/observation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/basis/typing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.513261 atom-0.9.1/docs/source/developer_notes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/developer_notes/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.517261 atom-0.9.1/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_coersion.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_composition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_containers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_default_value.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_employee.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_hello_world.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_inventory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_numeric.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_observe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_observe_hints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_person.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_range.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/ex_static_type_checking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/example_doc_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-03-13 12:30:16.000000 atom-0.9.1/docs/source/substitutions.sub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.485260 atom-0.9.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.521261 atom-0.9.1/examples/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-13 12:30:16.000000 atom-0.9.1/examples/api/coersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-13 12:30:16.000000 atom-0.9.1/examples/api/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-13 12:30:16.000000 atom-0.9.1/examples/api/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-13 12:30:16.000000 atom-0.9.1/examples/api/default_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-13 12:30:16.000000 atom-0.9.1/examples/api/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-13 12:30:16.000000 atom-0.9.1/examples/api/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-13 12:30:16.000000 atom-0.9.1/examples/api/observe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-13 12:30:16.000000 atom-0.9.1/examples/api/observe_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-13 12:30:16.000000 atom-0.9.1/examples/api/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-13 12:30:16.000000 atom-0.9.1/examples/api/range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.521261 atom-0.9.1/examples/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-13 12:30:16.000000 atom-0.9.1/examples/tutorial/employee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-13 12:30:16.000000 atom-0.9.1/examples/tutorial/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-13 12:30:16.000000 atom-0.9.1/examples/tutorial/person.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.521261 atom-0.9.1/examples/typehints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-13 12:30:16.000000 atom-0.9.1/examples/typehints/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-13 12:30:16.000000 atom-0.9.1/examples/typehints/static_type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-13 12:30:16.000000 atom-0.9.1/lint_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-03-13 12:30:16.000000 atom-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-03-13 12:30:16.000000 atom-0.9.1/releasenotes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 12:30:33.529261 atom-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-13 12:30:16.000000 atom-0.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-13 12:30:16.000000 atom-0.9.1/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.525261 atom-0.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.525261 atom-0.9.1/tests/datastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-03-13 12:30:16.000000 atom-0.9.1/tests/datastructure/test_sortedmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_atom_from_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_atomdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_atomlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_atomref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_atomset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_del_behaviors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_delegator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_eventbinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_get_behaviors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_get_set_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_getstate_behaviors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24110 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_observe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_post_behaviors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_set_behaviors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_signalconnector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-13 12:30:16.000000 atom-0.9.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:30:33.529261 atom-0.9.1/tests/type_checking/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_annotations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_coerced.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_delegator.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19382 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_dict.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_enum.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_event.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_generic_aliases.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_list.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_property.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_scalars.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_set.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_signal.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_subclass.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_tuple.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    30567 2023-03-13 12:30:16.000000 atom-0.9.1/tests/type_checking/test_typed_instance.yml
```

### Comparing `atom-0.9.0/.github/FUNDING.yml` & `atom-0.9.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/.github/workflows/ci.yml` & `atom-0.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/.github/workflows/docs.yml` & `atom-0.9.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/.github/workflows/release.yml` & `atom-0.9.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/.gitignore` & `atom-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/.readthedocs.yaml` & `atom-0.9.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/LICENSE` & `atom-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/MANIFEST.in` & `atom-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/PKG-INFO` & `atom-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atom
-Version: 0.9.0
+Version: 0.9.1
 Summary: Memory efficient Python objects
 Author-email: The Nucleic Development Team <sccolbert@gmail.com>
 Maintainer-email: "Matthieu C. Dartiailh" <m.dartiailh@gmail.com>
 License: =========================
          The Atom licensing terms
         =========================
         Atom is licensed under the terms of the Modified BSD License (also known as
```

### Comparing `atom-0.9.0/README.rst` & `atom-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/annotation_utils.py` & `atom-0.9.1/atom/annotation_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     ) and not isinstance(default, Member):
         raise ValueError(
             "Member subclasses cannot be used as annotations without "
             "specifying a default value for the attribute."
         )
     elif object in types or Any in types:
         m_cls = Value
+        parameters = ()
     # Int, Float, Str, Bytes, List, Dict, Set, Tuple, Bool, Callable
     elif len(types) == 1 and types[0] in _TYPE_TO_MEMBER:
         t = types[0]
         m_cls = _TYPE_TO_MEMBER[t]
         if annotate_type_containers and t in (list, dict, set, tuple):
             # We can only validate homogeneous tuple so far so we ignore other cases
             if t is tuple:
```

### Comparing `atom-0.9.0/atom/api.py` & `atom-0.9.1/atom/api.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/atom.py` & `atom-0.9.1/atom/atom.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/catom.pyi` & `atom-0.9.1/atom/catom.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/coerced.py` & `atom-0.9.1/atom/coerced.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/coerced.pyi` & `atom-0.9.1/atom/coerced.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/containerlist.py` & `atom-0.9.1/atom/containerlist.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/containerlist.pyi` & `atom-0.9.1/atom/containerlist.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/datastructures/sortedmap.pyi` & `atom-0.9.1/atom/datastructures/sortedmap.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/delegator.py` & `atom-0.9.1/atom/delegator.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/delegator.pyi` & `atom-0.9.1/atom/delegator.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/dict.py` & `atom-0.9.1/atom/dict.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/dict.pyi` & `atom-0.9.1/atom/dict.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/enum.py` & `atom-0.9.1/atom/enum.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/enum.pyi` & `atom-0.9.1/atom/enum.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/event.py` & `atom-0.9.1/atom/event.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/event.pyi` & `atom-0.9.1/atom/event.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/instance.py` & `atom-0.9.1/atom/instance.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/instance.pyi` & `atom-0.9.1/atom/instance.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/list.py` & `atom-0.9.1/atom/list.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/list.pyi` & `atom-0.9.1/atom/list.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/property.py` & `atom-0.9.1/atom/property.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/property.pyi` & `atom-0.9.1/atom/property.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/scalars.py` & `atom-0.9.1/atom/scalars.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/scalars.pyi` & `atom-0.9.1/atom/scalars.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/set.py` & `atom-0.9.1/atom/set.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/set.pyi` & `atom-0.9.1/atom/set.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/signal.py` & `atom-0.9.1/atom/signal.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/atomdict.cpp` & `atom-0.9.1/atom/src/atomdict.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,16 @@
 	{
 		return cppy::incref( value );
 	}
 	if( AtomDict_ass_subscript( self, key, dfv ) < 0 )
 	{
 		return 0;
 	}
-	return cppy::incref( dfv );
+	// Get the dictionary from the dict itself in case it was corced.
+	return cppy::incref( PyDict_GetItem( pyobject_cast( self ), key ) );
 }
 
 
 PyObject* AtomDict_update( AtomDict* dict, PyObject* args, PyObject* kwargs )
 {
     PyObject* item = 0;
 	if( !PyArg_UnpackTuple( args, "update", 0, 1, &item ) )
```

### Comparing `atom-0.9.0/atom/src/atomdict.h` & `atom-0.9.1/atom/src/atomdict.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/atomlist.cpp` & `atom-0.9.1/atom/src/atomlist.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/atomlist.h` & `atom-0.9.1/atom/src/atomlist.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/atomref.cpp` & `atom-0.9.1/atom/src/atomref.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/atomref.h` & `atom-0.9.1/atom/src/atomref.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/atomset.cpp` & `atom-0.9.1/atom/src/atomset.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/atomset.h` & `atom-0.9.1/atom/src/atomset.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/behaviors.h` & `atom-0.9.1/atom/src/behaviors.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/catom.cpp` & `atom-0.9.1/atom/src/catom.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/catom.h` & `atom-0.9.1/atom/src/catom.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/catommodule.cpp` & `atom-0.9.1/atom/src/catommodule.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/catompointer.h` & `atom-0.9.1/atom/src/catompointer.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/defaultvaluebehavior.cpp` & `atom-0.9.1/atom/src/defaultvaluebehavior.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/delattrbehavior.cpp` & `atom-0.9.1/atom/src/delattrbehavior.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/enumtypes.cpp` & `atom-0.9.1/atom/src/enumtypes.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/enumtypes.h` & `atom-0.9.1/atom/src/enumtypes.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/eventbinder.cpp` & `atom-0.9.1/atom/src/eventbinder.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/eventbinder.h` & `atom-0.9.1/atom/src/eventbinder.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/getattrbehavior.cpp` & `atom-0.9.1/atom/src/getattrbehavior.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/getstatebehavior.cpp` & `atom-0.9.1/atom/src/getstatebehavior.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/globalstatic.h` & `atom-0.9.1/atom/src/globalstatic.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/member.cpp` & `atom-0.9.1/atom/src/member.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/member.h` & `atom-0.9.1/atom/src/member.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/memberchange.cpp` & `atom-0.9.1/atom/src/memberchange.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/memberchange.h` & `atom-0.9.1/atom/src/memberchange.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/methodwrapper.cpp` & `atom-0.9.1/atom/src/methodwrapper.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/methodwrapper.h` & `atom-0.9.1/atom/src/methodwrapper.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/modifyguard.h` & `atom-0.9.1/atom/src/modifyguard.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/msstdint.h` & `atom-0.9.1/atom/src/msstdint.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/observer.h` & `atom-0.9.1/atom/src/observer.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/observerpool.cpp` & `atom-0.9.1/atom/src/observerpool.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/observerpool.h` & `atom-0.9.1/atom/src/observerpool.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/postgetattrbehavior.cpp` & `atom-0.9.1/atom/src/postgetattrbehavior.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/postsetattrbehavior.cpp` & `atom-0.9.1/atom/src/postsetattrbehavior.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/postvalidatebehavior.cpp` & `atom-0.9.1/atom/src/postvalidatebehavior.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/propertyhelper.cpp` & `atom-0.9.1/atom/src/propertyhelper.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/setattrbehavior.cpp` & `atom-0.9.1/atom/src/setattrbehavior.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/signalconnector.cpp` & `atom-0.9.1/atom/src/signalconnector.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/signalconnector.h` & `atom-0.9.1/atom/src/signalconnector.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/sortedmap.cpp` & `atom-0.9.1/atom/src/sortedmap.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/utils.h` & `atom-0.9.1/atom/src/utils.h`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/src/validatebehavior.cpp` & `atom-0.9.1/atom/src/validatebehavior.cpp`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/subclass.py` & `atom-0.9.1/atom/subclass.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/subclass.pyi` & `atom-0.9.1/atom/subclass.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/tuple.py` & `atom-0.9.1/atom/tuple.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/tuple.pyi` & `atom-0.9.1/atom/tuple.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/typed.py` & `atom-0.9.1/atom/typed.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/typed.pyi` & `atom-0.9.1/atom/typed.pyi`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/typing_utils.py` & `atom-0.9.1/atom/typing_utils.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/atom/version.py` & `atom-0.9.1/atom/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 # This file is auto-generated by setuptools-scm do NOT edit it.
 
 from collections import namedtuple
 
 #: A namedtuple of the version info for the current release.
 _version_info = namedtuple("_version_info", "major minor micro status")
 
-parts = "0.9.0".split(".", 3)
+parts = "0.9.1".split(".", 3)
 version_info = _version_info(
     int(parts[0]),
     int(parts[1]),
     int(parts[2]),
     parts[3] if len(parts) == 4 else "",
 )
 
 # Remove everything but the 'version_info' from this module.
 del namedtuple, _version_info, parts
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
```

### Comparing `atom-0.9.0/atom.egg-info/PKG-INFO` & `atom-0.9.1/atom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atom
-Version: 0.9.0
+Version: 0.9.1
 Summary: Memory efficient Python objects
 Author-email: The Nucleic Development Team <sccolbert@gmail.com>
 Maintainer-email: "Matthieu C. Dartiailh" <m.dartiailh@gmail.com>
 License: =========================
          The Atom licensing terms
         =========================
         Atom is licensed under the terms of the Modified BSD License (also known as
```

### Comparing `atom-0.9.0/atom.egg-info/SOURCES.txt` & `atom-0.9.1/atom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/Makefile` & `atom-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/make.bat` & `atom-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/advanced/containers.rst` & `atom-0.9.1/docs/source/advanced/containers.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/advanced/customization.rst` & `atom-0.9.1/docs/source/advanced/customization.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/advanced/index.rst` & `atom-0.9.1/docs/source/advanced/index.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/advanced/manual_notifications.rst` & `atom-0.9.1/docs/source/advanced/manual_notifications.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/advanced/property.rst` & `atom-0.9.1/docs/source/advanced/property.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/advanced/typing.rst` & `atom-0.9.1/docs/source/advanced/typing.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/advanced/weakref.rst` & `atom-0.9.1/docs/source/advanced/weakref.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/api/atom.rst` & `atom-0.9.1/docs/source/api/atom.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/basis/basis.rst` & `atom-0.9.1/docs/source/basis/basis.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/basis/index.rst` & `atom-0.9.1/docs/source/basis/index.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/basis/installation.rst` & `atom-0.9.1/docs/source/basis/installation.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/basis/mangled_methods.rst` & `atom-0.9.1/docs/source/basis/mangled_methods.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/basis/members.rst` & `atom-0.9.1/docs/source/basis/members.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/basis/observation.rst` & `atom-0.9.1/docs/source/basis/observation.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/basis/typing.rst` & `atom-0.9.1/docs/source/basis/typing.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/conf.py` & `atom-0.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/developer_notes/index.rst` & `atom-0.9.1/docs/source/developer_notes/index.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_coersion.rst` & `atom-0.9.1/docs/source/examples/ex_coersion.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_composition.rst` & `atom-0.9.1/docs/source/examples/ex_composition.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_containers.rst` & `atom-0.9.1/docs/source/examples/ex_containers.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_default_value.rst` & `atom-0.9.1/docs/source/examples/ex_default_value.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_employee.rst` & `atom-0.9.1/docs/source/examples/ex_employee.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_hello_world.rst` & `atom-0.9.1/docs/source/examples/ex_hello_world.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_inventory.rst` & `atom-0.9.1/docs/source/examples/ex_inventory.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_metadata.rst` & `atom-0.9.1/docs/source/examples/ex_metadata.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_numeric.rst` & `atom-0.9.1/docs/source/examples/ex_numeric.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_observe.rst` & `atom-0.9.1/docs/source/examples/ex_observe.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_observe_hints.rst` & `atom-0.9.1/docs/source/examples/ex_observe_hints.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_person.rst` & `atom-0.9.1/docs/source/examples/ex_person.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_property.rst` & `atom-0.9.1/docs/source/examples/ex_property.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_range.rst` & `atom-0.9.1/docs/source/examples/ex_range.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/ex_static_type_checking.rst` & `atom-0.9.1/docs/source/examples/ex_static_type_checking.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/example_doc_generator.py` & `atom-0.9.1/docs/source/examples/example_doc_generator.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/examples/index.rst` & `atom-0.9.1/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/index.rst` & `atom-0.9.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/docs/source/substitutions.sub` & `atom-0.9.1/docs/source/substitutions.sub`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/api/coersion.py` & `atom-0.9.1/examples/api/coersion.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/api/composition.py` & `atom-0.9.1/examples/api/composition.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/api/containers.py` & `atom-0.9.1/examples/api/containers.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/api/default_value.py` & `atom-0.9.1/examples/api/default_value.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/api/metadata.py` & `atom-0.9.1/examples/api/metadata.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/api/numeric.py` & `atom-0.9.1/examples/api/numeric.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/api/observe.py` & `atom-0.9.1/examples/api/observe.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/api/observe_hints.py` & `atom-0.9.1/examples/api/observe_hints.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/api/property.py` & `atom-0.9.1/examples/api/property.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/api/range.py` & `atom-0.9.1/examples/api/range.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/tutorial/employee.py` & `atom-0.9.1/examples/tutorial/employee.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/tutorial/hello_world.py` & `atom-0.9.1/examples/tutorial/hello_world.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/tutorial/person.py` & `atom-0.9.1/examples/tutorial/person.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/typehints/inventory.py` & `atom-0.9.1/examples/typehints/inventory.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/examples/typehints/static_type_checking.py` & `atom-0.9.1/examples/typehints/static_type_checking.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/pyproject.toml` & `atom-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/releasenotes.rst` & `atom-0.9.1/releasenotes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Atom Release Notes
 ==================
 
+0.9.1 - 13/03/2023
+------------------
+
+- fix generation of Value member from union containing object/Any PR #198
+- fix setdefault method of atomdict to return the actually stored item PR #197
+
 0.9.0 - 21/02/2023
 ------------------
 
 - fix the generation of Subclass from type annotations PR #193
 - move getstate and setstate implementation to C and allow to customize the condition
   under which a member value is pickled. PR #182
   Customization is used to only pickle member value whose state can be restored
```

### Comparing `atom-0.9.0/setup.py` & `atom-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/datastructure/test_sortedmap.py` & `atom-0.9.1/tests/datastructure/test_sortedmap.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_atom.py` & `atom-0.9.1/tests/test_atom.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_atom_from_annotations.py` & `atom-0.9.1/tests/test_atom_from_annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,15 @@
     [
         (bool, Bool, True),
         (int, Int, 1),
         (float, Float, 1.0),
         (str, Str, "a"),
         (bytes, Bytes, b"a"),
         (Any, Value, 1),
+        (Union[Any, None], Value, None),
         (object, Value, 2),
         (TCallable, Callable, lambda x: x),
         (TList, List, [1]),
         (TSet, Set, {1}),
         (TDict, Dict, {1: 2}),
         (Optional[Iterable], Instance, None),
         (Type[int], Subclass, int),
```

### Comparing `atom-0.9.0/tests/test_atomdict.py` & `atom-0.9.1/tests/test_atomdict.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # --------------------------------------------------------------------------------------
 """Test the typed dictionary.
 
 
 """
 import pytest
 
-from atom.api import Atom, Dict, Int, atomdict
+from atom.api import Atom, Dict, Int, List, atomdict, atomlist
 
 
 @pytest.fixture
 def atom_dict():
     """Atom with different Dict members."""
 
     class DictAtom(Atom):
@@ -145,14 +145,24 @@
     assert atom_dict.fullytyped[1] == 1
     with pytest.raises(TypeError):
         atom_dict.fullytyped.setdefault("", 1)
     with pytest.raises(TypeError):
         atom_dict.fullytyped.setdefault(2, "")
 
 
+def test_setdefault_coercion():
+    class A(Atom):
+        d = Dict(int, List(int))
+
+    a = A()
+    content = a.d.setdefault(1, [])
+    assert isinstance(content, atomlist)
+    assert content is a.d[1]
+
+
 def test_update(atom_dict):
     """Test update a dict."""
     atom_dict.untyped.update({"": 1})
     assert atom_dict.untyped[""] == 1
     atom_dict.untyped.update([("1", 1)])
     assert atom_dict.untyped["1"] == 1
```

### Comparing `atom-0.9.0/tests/test_atomlist.py` & `atom-0.9.1/tests/test_atomlist.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_atomref.py` & `atom-0.9.1/tests/test_atomref.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_atomset.py` & `atom-0.9.1/tests/test_atomset.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_default_values.py` & `atom-0.9.1/tests/test_default_values.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_del_behaviors.py` & `atom-0.9.1/tests/test_del_behaviors.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_delegator.py` & `atom-0.9.1/tests/test_delegator.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_enum.py` & `atom-0.9.1/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_eventbinder.py` & `atom-0.9.1/tests/test_eventbinder.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_examples.py` & `atom-0.9.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_get_behaviors.py` & `atom-0.9.1/tests/test_get_behaviors.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_get_set_state.py` & `atom-0.9.1/tests/test_get_set_state.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_getstate_behaviors.py` & `atom-0.9.1/tests/test_getstate_behaviors.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_member.py` & `atom-0.9.1/tests/test_member.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_observe.py` & `atom-0.9.1/tests/test_observe.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_post_behaviors.py` & `atom-0.9.1/tests/test_post_behaviors.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_property.py` & `atom-0.9.1/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_set_behaviors.py` & `atom-0.9.1/tests/test_set_behaviors.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_signalconnector.py` & `atom-0.9.1/tests/test_signalconnector.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_typing_utils.py` & `atom-0.9.1/tests/test_typing_utils.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_validators.py` & `atom-0.9.1/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/test_version.py` & `atom-0.9.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_annotations.yml` & `atom-0.9.1/tests/type_checking/test_annotations.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_coerced.yml` & `atom-0.9.1/tests/type_checking/test_coerced.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_delegator.yml` & `atom-0.9.1/tests/type_checking/test_delegator.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_dict.yml` & `atom-0.9.1/tests/type_checking/test_dict.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_enum.yml` & `atom-0.9.1/tests/type_checking/test_enum.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_event.yml` & `atom-0.9.1/tests/type_checking/test_event.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_generic_aliases.yml` & `atom-0.9.1/tests/type_checking/test_generic_aliases.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_list.yml` & `atom-0.9.1/tests/type_checking/test_list.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_property.yml` & `atom-0.9.1/tests/type_checking/test_property.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_scalars.yml` & `atom-0.9.1/tests/type_checking/test_scalars.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_set.yml` & `atom-0.9.1/tests/type_checking/test_set.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_signal.yml` & `atom-0.9.1/tests/type_checking/test_signal.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_subclass.yml` & `atom-0.9.1/tests/type_checking/test_subclass.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_tuple.yml` & `atom-0.9.1/tests/type_checking/test_tuple.yml`

 * *Files identical despite different names*

### Comparing `atom-0.9.0/tests/type_checking/test_typed_instance.yml` & `atom-0.9.1/tests/type_checking/test_typed_instance.yml`

 * *Files identical despite different names*

