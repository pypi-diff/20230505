# Comparing `tmp/ZConfig-3.6.1.tar.gz` & `tmp/ZConfig-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ZConfig-3.6.1.tar", last modified: Tue Dec  6 13:22:04 2022, max compression
+gzip compressed data, was "ZConfig-4.0.tar", last modified: Fri May  5 05:59:37 2023, max compression
```

## Comparing `ZConfig-3.6.1.tar` & `ZConfig-4.0.tar`

### file list

```diff
@@ -1,174 +1,152 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/
--rw-r--r--   0 jens       (501) staff       (20)       80 2021-11-02 08:52:24.000000 ZConfig-3.6.1/.readthedocs.yml
--rw-r--r--   0 jens       (501) staff       (20)    12210 2022-12-06 13:20:09.000000 ZConfig-3.6.1/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      804 2022-12-06 09:38:00.000000 ZConfig-3.6.1/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:52:24.000000 ZConfig-3.6.1/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:52:24.000000 ZConfig-3.6.1/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      530 2022-12-06 09:38:00.000000 ZConfig-3.6.1/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)    21730 2022-12-06 13:22:04.000000 ZConfig-3.6.1/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     3943 2022-12-05 15:30:13.000000 ZConfig-3.6.1/README.rst
--rw-r--r--   0 jens       (501) staff       (20)      341 2021-11-02 08:52:24.000000 ZConfig-3.6.1/buildout.cfg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/docs/
--rw-r--r--   0 jens       (501) staff       (20)      604 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/Makefile
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/docs/_build/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/docs/_build/html/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/docs/_build/html/_sources/
--rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/changelog.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      264 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/developing-with-zconfig.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     2642 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/documenting-components.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1467 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     5339 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/logging-components.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      444 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/py-mod-cmdline.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      443 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/py-mod-datatypes.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1200 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/py-mod-loader.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     2086 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/py-mod-subst.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1922 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/py-mod-zconfig.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     3079 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/standard-components.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     5829 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/standard-datatypes.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      761 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/tools.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     4373 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/using-logging.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     8198 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/using-zconfig.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     5156 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/writing-components.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    22822 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/writing-schema.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      159 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/_build/html/_sources/zconfig.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/changelog.rst
--rw-r--r--   0 jens       (501) staff       (20)     4970 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/conf.py
--rw-r--r--   0 jens       (501) staff       (20)      264 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/developing-with-zconfig.rst
--rw-r--r--   0 jens       (501) staff       (20)     2642 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/documenting-components.rst
--rw-r--r--   0 jens       (501) staff       (20)     1467 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     5339 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/logging-components.rst
--rw-r--r--   0 jens       (501) staff       (20)      811 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/make.bat
--rw-r--r--   0 jens       (501) staff       (20)      444 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/py-mod-cmdline.rst
--rw-r--r--   0 jens       (501) staff       (20)      443 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/py-mod-datatypes.rst
--rw-r--r--   0 jens       (501) staff       (20)     1200 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/py-mod-loader.rst
--rw-r--r--   0 jens       (501) staff       (20)     2086 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/py-mod-subst.rst
--rw-r--r--   0 jens       (501) staff       (20)     1922 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/py-mod-zconfig.rst
--rw-r--r--   0 jens       (501) staff       (20)      186 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/root-and-child-config.conf
--rw-r--r--   0 jens       (501) staff       (20)     3464 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/schema.dtd
--rw-r--r--   0 jens       (501) staff       (20)      131 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/simple-root-config.conf
--rw-r--r--   0 jens       (501) staff       (20)     3079 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/standard-components.rst
--rw-r--r--   0 jens       (501) staff       (20)     5829 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/standard-datatypes.rst
--rw-r--r--   0 jens       (501) staff       (20)      761 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/tools.rst
--rw-r--r--   0 jens       (501) staff       (20)     4373 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/using-logging.rst
--rw-r--r--   0 jens       (501) staff       (20)     8198 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/using-zconfig.rst
--rw-r--r--   0 jens       (501) staff       (20)     5156 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/writing-components.rst
--rw-r--r--   0 jens       (501) staff       (20)    22822 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/writing-schema.rst
--rw-r--r--   0 jens       (501) staff       (20)      159 2022-12-05 15:30:13.000000 ZConfig-3.6.1/docs/zconfig.rst
--rw-r--r--   0 jens       (501) staff       (20)      446 2022-12-06 13:22:04.000000 ZConfig-3.6.1/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     2769 2022-12-06 13:20:23.000000 ZConfig-3.6.1/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/
--rw-r--r--   0 jens       (501) staff       (20)     8190 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     2734 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/_compat.py
--rwxr-xr-x   0 jens       (501) staff       (20)    10909 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/_schema_utils.py
--rw-r--r--   0 jens       (501) staff       (20)     6929 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/cfgparser.py
--rw-r--r--   0 jens       (501) staff       (20)     7631 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/cmdline.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/components/
--rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/components/basic/
--rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/basic/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      206 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/basic/component.xml
--rw-r--r--   0 jens       (501) staff       (20)      765 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/basic/mapping.py
--rw-r--r--   0 jens       (501) staff       (20)      945 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/basic/mapping.xml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/components/basic/tests/
--rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/basic/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     2688 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/basic/tests/test_mapping.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/components/logger/
--rw-r--r--   0 jens       (501) staff       (20)      702 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      151 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/abstract.xml
--rw-r--r--   0 jens       (501) staff       (20)     1801 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/base-logger.xml
--rw-r--r--   0 jens       (501) staff       (20)      375 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/component.xml
--rw-r--r--   0 jens       (501) staff       (20)     1134 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/datatypes.py
--rw-r--r--   0 jens       (501) staff       (20)      478 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/eventlog.xml
--rw-r--r--   0 jens       (501) staff       (20)     1410 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/factory.py
--rw-r--r--   0 jens       (501) staff       (20)    13016 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/formatter.py
--rw-r--r--   0 jens       (501) staff       (20)     7702 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/handlers.py
--rw-r--r--   0 jens       (501) staff       (20)     9833 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/handlers.xml
--rw-r--r--   0 jens       (501) staff       (20)     3513 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/logger.py
--rw-r--r--   0 jens       (501) staff       (20)     1463 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/logger.xml
--rw-r--r--   0 jens       (501) staff       (20)     5285 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/loghandler.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/components/logger/tests/
--rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     2881 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/tests/support.py
--rw-r--r--   0 jens       (501) staff       (20)    24293 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/components/logger/tests/test_formatter.py
--rw-r--r--   0 jens       (501) staff       (20)    35808 2022-12-06 09:45:40.000000 ZConfig-3.6.1/src/ZConfig/components/logger/tests/test_logger.py
--rw-r--r--   0 jens       (501) staff       (20)    17956 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/datatypes.py
--rw-r--r--   0 jens       (501) staff       (20)    17778 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/info.py
--rw-r--r--   0 jens       (501) staff       (20)    18721 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/loader.py
--rw-r--r--   0 jens       (501) staff       (20)    11194 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/matcher.py
--rw-r--r--   0 jens       (501) staff       (20)     2973 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/pygments.py
--rw-r--r--   0 jens       (501) staff       (20)    22743 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/schema.py
--rwxr-xr-x   0 jens       (501) staff       (20)     4691 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/schema2html.py
--rw-r--r--   0 jens       (501) staff       (20)     3168 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/schemaless.py
--rw-r--r--   0 jens       (501) staff       (20)     6913 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/schemaless.txt
--rwxr-xr-x   0 jens       (501) staff       (20)     6140 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/sphinx.py
--rw-r--r--   0 jens       (501) staff       (20)     3782 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/substitution.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/tests/
--rw-r--r--   0 jens       (501) staff       (20)      762 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)       41 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/bad-component.xml
--rw-r--r--   0 jens       (501) staff       (20)      122 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/bad-component2.xml
--rw-r--r--   0 jens       (501) staff       (20)     1581 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/foosample.zip
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/tests/input/
--rw-r--r--   0 jens       (501) staff       (20)       98 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/base-datatype1.xml
--rw-r--r--   0 jens       (501) staff       (20)       98 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/base-datatype2.xml
--rw-r--r--   0 jens       (501) staff       (20)       70 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/base-keytype1.xml
--rw-r--r--   0 jens       (501) staff       (20)       96 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/base-keytype2.xml
--rw-r--r--   0 jens       (501) staff       (20)      161 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/base.xml
--rw-r--r--   0 jens       (501) staff       (20)       56 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/include.conf
--rw-r--r--   0 jens       (501) staff       (20)       42 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/inner.conf
--rw-r--r--   0 jens       (501) staff       (20)      157 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/library.xml
--rw-r--r--   0 jens       (501) staff       (20)      404 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/logger.xml
--rw-r--r--   0 jens       (501) staff       (20)       76 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/non-ascii.txt
--rw-r--r--   0 jens       (501) staff       (20)       62 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/outer.conf
--rw-r--r--   0 jens       (501) staff       (20)      440 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/simple.conf
--rw-r--r--   0 jens       (501) staff       (20)      951 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/simple.xml
--rw-r--r--   0 jens       (501) staff       (20)      409 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/simplesections.conf
--rw-r--r--   0 jens       (501) staff       (20)     1884 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/input/simplesections.xml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/tests/library/
--rw-r--r--   0 jens       (501) staff       (20)       88 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/library/README.txt
--rw-r--r--   0 jens       (501) staff       (20)       23 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/library/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/tests/library/thing/
--rw-r--r--   0 jens       (501) staff       (20)      840 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/library/thing/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      344 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/library/thing/component.xml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/tests/library/thing/extras/
--rw-r--r--   0 jens       (501) staff       (20)      104 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/library/thing/extras/extras.xml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/tests/library/widget/
--rw-r--r--   0 jens       (501) staff       (20)       23 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/library/widget/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      256 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/library/widget/component.xml
--rw-r--r--   0 jens       (501) staff       (20)      103 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/library/widget/extra.xml
--rw-r--r--   0 jens       (501) staff       (20)      623 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/sphinx_test_schema.xml
--rw-r--r--   0 jens       (501) staff       (20)     3588 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/support.py
--rw-r--r--   0 jens       (501) staff       (20)     3031 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_cfgimports.py
--rw-r--r--   0 jens       (501) staff       (20)     8598 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_cmdline.py
--rw-r--r--   0 jens       (501) staff       (20)    10047 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_config.py
--rw-r--r--   0 jens       (501) staff       (20)     2431 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_cookbook.py
--rw-r--r--   0 jens       (501) staff       (20)    16199 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_datatypes.py
--rw-r--r--   0 jens       (501) staff       (20)     7136 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_info.py
--rw-r--r--   0 jens       (501) staff       (20)    16711 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_loader.py
--rw-r--r--   0 jens       (501) staff       (20)     4227 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_matcher.py
--rw-r--r--   0 jens       (501) staff       (20)     8293 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_pygments.py
--rw-r--r--   0 jens       (501) staff       (20)     2706 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_readme.py
--rw-r--r--   0 jens       (501) staff       (20)    50686 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_schema.py
--rw-r--r--   0 jens       (501) staff       (20)     8018 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_schema2html.py
--rw-r--r--   0 jens       (501) staff       (20)     1277 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_schemaless.py
--rw-r--r--   0 jens       (501) staff       (20)     3849 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_subst.py
--rw-r--r--   0 jens       (501) staff       (20)     2514 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/test_validator.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/tests/zipsource/
--rw-r--r--   0 jens       (501) staff       (20)      108 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/zipsource/README.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/tests/zipsource/foo/
--rw-r--r--   0 jens       (501) staff       (20)       38 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/zipsource/foo/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig/tests/zipsource/foo/sample/
--rw-r--r--   0 jens       (501) staff       (20)       38 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/zipsource/foo/sample/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      234 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/zipsource/foo/sample/component.xml
--rw-r--r--   0 jens       (501) staff       (20)      124 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/tests/zipsource/foo/sample/datatypes.py
--rw-r--r--   0 jens       (501) staff       (20)     1915 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/url.py
--rwxr-xr-x   0 jens       (501) staff       (20)     2205 2022-12-05 15:30:13.000000 ZConfig-3.6.1/src/ZConfig/validator.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)    21730 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     5188 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)      158 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig.egg-info/entry_points.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-12-05 15:30:57.000000 ZConfig-3.6.1/src/ZConfig.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)       92 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        8 2022-12-06 13:22:04.000000 ZConfig-3.6.1/src/ZConfig.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     1646 2022-12-06 09:45:40.000000 ZConfig-3.6.1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.244049 ZConfig-4.0/
+-rw-r--r--   0 mac        (513) staff       (20)       80 2023-05-05 05:59:36.000000 ZConfig-4.0/.readthedocs.yml
+-rw-r--r--   0 mac        (513) staff       (20)    12288 2023-05-05 05:59:36.000000 ZConfig-4.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-05-05 05:59:36.000000 ZConfig-4.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-05-05 05:59:36.000000 ZConfig-4.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-05-05 05:59:36.000000 ZConfig-4.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      530 2023-05-05 05:59:36.000000 ZConfig-4.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    17397 2023-05-05 05:59:37.244221 ZConfig-4.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     3842 2023-05-05 05:59:36.000000 ZConfig-4.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      341 2023-05-05 05:59:36.000000 ZConfig-4.0/buildout.cfg
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.209766 ZConfig-4.0/docs/
+-rw-r--r--   0 mac        (513) staff       (20)      604 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/Makefile
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/changelog.rst
+-rw-r--r--   0 mac        (513) staff       (20)     4970 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)      264 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/developing-with-zconfig.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2642 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/documenting-components.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1467 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5339 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/logging-components.rst
+-rw-r--r--   0 mac        (513) staff       (20)      811 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/make.bat
+-rw-r--r--   0 mac        (513) staff       (20)      444 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/py-mod-cmdline.rst
+-rw-r--r--   0 mac        (513) staff       (20)      443 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/py-mod-datatypes.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1200 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/py-mod-loader.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2086 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/py-mod-subst.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1922 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/py-mod-zconfig.rst
+-rw-r--r--   0 mac        (513) staff       (20)      186 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/root-and-child-config.conf
+-rw-r--r--   0 mac        (513) staff       (20)     3464 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/schema.dtd
+-rw-r--r--   0 mac        (513) staff       (20)      131 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/simple-root-config.conf
+-rw-r--r--   0 mac        (513) staff       (20)     3079 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/standard-components.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5829 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/standard-datatypes.rst
+-rw-r--r--   0 mac        (513) staff       (20)      761 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/tools.rst
+-rw-r--r--   0 mac        (513) staff       (20)     4373 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/using-logging.rst
+-rw-r--r--   0 mac        (513) staff       (20)     8198 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/using-zconfig.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5156 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/writing-components.rst
+-rw-r--r--   0 mac        (513) staff       (20)    22822 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/writing-schema.rst
+-rw-r--r--   0 mac        (513) staff       (20)      159 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/zconfig.rst
+-rw-r--r--   0 mac        (513) staff       (20)      447 2023-05-05 05:59:37.244855 ZConfig-4.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2541 2023-05-05 05:59:36.000000 ZConfig-4.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.193939 ZConfig-4.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.215927 ZConfig-4.0/src/ZConfig/
+-rw-r--r--   0 mac        (513) staff       (20)     8188 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/__init__.py
+-rwxr-xr-x   0 mac        (513) staff       (20)    10563 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/_schema_utils.py
+-rw-r--r--   0 mac        (513) staff       (20)     6830 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/cfgparser.py
+-rw-r--r--   0 mac        (513) staff       (20)     7535 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/cmdline.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.218646 ZConfig-4.0/src/ZConfig/components/
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.219984 ZConfig-4.0/src/ZConfig/components/basic/
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      206 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/component.xml
+-rw-r--r--   0 mac        (513) staff       (20)      765 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/mapping.py
+-rw-r--r--   0 mac        (513) staff       (20)      945 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/mapping.xml
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.220641 ZConfig-4.0/src/ZConfig/components/basic/tests/
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     2688 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/tests/test_mapping.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.225108 ZConfig-4.0/src/ZConfig/components/logger/
+-rw-r--r--   0 mac        (513) staff       (20)      702 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      151 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/abstract.xml
+-rw-r--r--   0 mac        (513) staff       (20)     1801 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/base-logger.xml
+-rw-r--r--   0 mac        (513) staff       (20)      375 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/component.xml
+-rw-r--r--   0 mac        (513) staff       (20)     1134 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/datatypes.py
+-rw-r--r--   0 mac        (513) staff       (20)      478 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/eventlog.xml
+-rw-r--r--   0 mac        (513) staff       (20)     1369 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/factory.py
+-rw-r--r--   0 mac        (513) staff       (20)     7708 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/formatter.py
+-rw-r--r--   0 mac        (513) staff       (20)     7689 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/handlers.py
+-rw-r--r--   0 mac        (513) staff       (20)     9706 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/handlers.xml
+-rw-r--r--   0 mac        (513) staff       (20)     3513 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/logger.py
+-rw-r--r--   0 mac        (513) staff       (20)     1463 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/logger.xml
+-rw-r--r--   0 mac        (513) staff       (20)     5272 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/loghandler.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.226639 ZConfig-4.0/src/ZConfig/components/logger/tests/
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     2814 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/tests/support.py
+-rw-r--r--   0 mac        (513) staff       (20)    19118 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/tests/test_formatter.py
+-rw-r--r--   0 mac        (513) staff       (20)    35710 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/tests/test_logger.py
+-rw-r--r--   0 mac        (513) staff       (20)    17571 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/datatypes.py
+-rw-r--r--   0 mac        (513) staff       (20)    17706 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/info.py
+-rw-r--r--   0 mac        (513) staff       (20)    18005 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/loader.py
+-rw-r--r--   0 mac        (513) staff       (20)    11109 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/matcher.py
+-rw-r--r--   0 mac        (513) staff       (20)     2896 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/pygments.py
+-rw-r--r--   0 mac        (513) staff       (20)    22431 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/schema.py
+-rwxr-xr-x   0 mac        (513) staff       (20)     4626 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/schema2html.py
+-rw-r--r--   0 mac        (513) staff       (20)     3168 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/schemaless.py
+-rw-r--r--   0 mac        (513) staff       (20)     6887 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/schemaless.txt
+-rwxr-xr-x   0 mac        (513) staff       (20)     5963 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/sphinx.py
+-rw-r--r--   0 mac        (513) staff       (20)     3782 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/substitution.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.234240 ZConfig-4.0/src/ZConfig/tests/
+-rw-r--r--   0 mac        (513) staff       (20)      762 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)       41 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/bad-component.xml
+-rw-r--r--   0 mac        (513) staff       (20)      122 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/bad-component2.xml
+-rw-r--r--   0 mac        (513) staff       (20)     1581 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/foosample.zip
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.239411 ZConfig-4.0/src/ZConfig/tests/input/
+-rw-r--r--   0 mac        (513) staff       (20)       98 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/base-datatype1.xml
+-rw-r--r--   0 mac        (513) staff       (20)       98 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/base-datatype2.xml
+-rw-r--r--   0 mac        (513) staff       (20)       70 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/base-keytype1.xml
+-rw-r--r--   0 mac        (513) staff       (20)       96 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/base-keytype2.xml
+-rw-r--r--   0 mac        (513) staff       (20)      161 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/base.xml
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/include.conf
+-rw-r--r--   0 mac        (513) staff       (20)       42 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/inner.conf
+-rw-r--r--   0 mac        (513) staff       (20)      157 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/library.xml
+-rw-r--r--   0 mac        (513) staff       (20)      404 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/logger.xml
+-rw-r--r--   0 mac        (513) staff       (20)       76 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/non-ascii.txt
+-rw-r--r--   0 mac        (513) staff       (20)       62 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/outer.conf
+-rw-r--r--   0 mac        (513) staff       (20)      440 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/simple.conf
+-rw-r--r--   0 mac        (513) staff       (20)      951 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/simple.xml
+-rw-r--r--   0 mac        (513) staff       (20)      409 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/simplesections.conf
+-rw-r--r--   0 mac        (513) staff       (20)     1884 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/simplesections.xml
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.240067 ZConfig-4.0/src/ZConfig/tests/library/
+-rw-r--r--   0 mac        (513) staff       (20)       88 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/README.txt
+-rw-r--r--   0 mac        (513) staff       (20)       23 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.240773 ZConfig-4.0/src/ZConfig/tests/library/thing/
+-rw-r--r--   0 mac        (513) staff       (20)      840 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/thing/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      344 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/thing/component.xml
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.241111 ZConfig-4.0/src/ZConfig/tests/library/thing/extras/
+-rw-r--r--   0 mac        (513) staff       (20)      104 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/thing/extras/extras.xml
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.242072 ZConfig-4.0/src/ZConfig/tests/library/widget/
+-rw-r--r--   0 mac        (513) staff       (20)       23 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/widget/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      256 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/widget/component.xml
+-rw-r--r--   0 mac        (513) staff       (20)      103 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/widget/extra.xml
+-rw-r--r--   0 mac        (513) staff       (20)      623 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/sphinx_test_schema.xml
+-rw-r--r--   0 mac        (513) staff       (20)     3553 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/support.py
+-rw-r--r--   0 mac        (513) staff       (20)     3005 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_cfgimports.py
+-rw-r--r--   0 mac        (513) staff       (20)     8598 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_cmdline.py
+-rw-r--r--   0 mac        (513) staff       (20)    10021 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_config.py
+-rw-r--r--   0 mac        (513) staff       (20)     2431 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_cookbook.py
+-rw-r--r--   0 mac        (513) staff       (20)    15856 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_datatypes.py
+-rw-r--r--   0 mac        (513) staff       (20)     7112 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_info.py
+-rw-r--r--   0 mac        (513) staff       (20)    15547 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_loader.py
+-rw-r--r--   0 mac        (513) staff       (20)     4195 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_matcher.py
+-rw-r--r--   0 mac        (513) staff       (20)     8216 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_pygments.py
+-rw-r--r--   0 mac        (513) staff       (20)     2704 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_readme.py
+-rw-r--r--   0 mac        (513) staff       (20)    50528 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_schema.py
+-rw-r--r--   0 mac        (513) staff       (20)     7660 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_schema2html.py
+-rw-r--r--   0 mac        (513) staff       (20)     1277 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_schemaless.py
+-rw-r--r--   0 mac        (513) staff       (20)     3771 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_subst.py
+-rw-r--r--   0 mac        (513) staff       (20)     2449 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_validator.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.242403 ZConfig-4.0/src/ZConfig/tests/zipsource/
+-rw-r--r--   0 mac        (513) staff       (20)      108 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/zipsource/README.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.242734 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/
+-rw-r--r--   0 mac        (513) staff       (20)       38 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.243760 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/sample/
+-rw-r--r--   0 mac        (513) staff       (20)       38 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/sample/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      234 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/sample/component.xml
+-rw-r--r--   0 mac        (513) staff       (20)      124 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/sample/datatypes.py
+-rw-r--r--   0 mac        (513) staff       (20)     1888 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/url.py
+-rwxr-xr-x   0 mac        (513) staff       (20)     2167 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/validator.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.218326 ZConfig-4.0/src/ZConfig.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    17397 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     4282 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)      157 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       92 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        8 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1568 2023-05-05 05:59:36.000000 ZConfig-4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ZConfig-3.6.1/CHANGES.rst` & `ZConfig-4.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ============================
  Change History for ZConfig
 ============================
 
+4.0 (2023-05-05)
+================
+
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
 3.6.1 (2022-12-06)
 ==================
 
 - Add support for Python 3.11.
 
 - Drop support for Python 3.4.
```

### Comparing `ZConfig-3.6.1/CONTRIBUTING.md` & `ZConfig-4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/LICENSE.txt` & `ZConfig-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/MANIFEST.in` & `ZConfig-4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/README.rst` & `ZConfig-4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,9 @@
 
 
 To install to another prefix (for example, /usr/local)::
 
   python setup.py install --prefix=/usr/local
 
 
-If you need to force the python interpreter to (for example) python2::
-
-  python2 setup.py install
-
-
 For more information on installing packages, please refer to the
 `Python Packaging User Guide <https://packaging.python.org/>`__.
```

### Comparing `ZConfig-3.6.1/docs/Makefile` & `ZConfig-4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/documenting-components.rst.txt` & `ZConfig-4.0/docs/documenting-components.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/index.rst.txt` & `ZConfig-4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/logging-components.rst.txt` & `ZConfig-4.0/docs/logging-components.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/py-mod-loader.rst.txt` & `ZConfig-4.0/docs/py-mod-loader.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/py-mod-subst.rst.txt` & `ZConfig-4.0/docs/py-mod-subst.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/py-mod-zconfig.rst.txt` & `ZConfig-4.0/docs/py-mod-zconfig.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/standard-components.rst.txt` & `ZConfig-4.0/docs/standard-components.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/standard-datatypes.rst.txt` & `ZConfig-4.0/docs/standard-datatypes.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/tools.rst.txt` & `ZConfig-4.0/docs/tools.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/using-logging.rst.txt` & `ZConfig-4.0/docs/using-logging.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/using-zconfig.rst.txt` & `ZConfig-4.0/docs/using-zconfig.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/writing-components.rst.txt` & `ZConfig-4.0/docs/writing-components.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/_build/html/_sources/writing-schema.rst.txt` & `ZConfig-4.0/docs/writing-schema.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/conf.py` & `ZConfig-4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/make.bat` & `ZConfig-4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/docs/schema.dtd` & `ZConfig-4.0/docs/schema.dtd`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/setup.py` & `ZConfig-4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 tests_require = [
     'docutils',
     'manuel',
     'zope.exceptions',
     'zope.testrunner',
 ]
 
-options = dict(
+setup(
     name="ZConfig",
-    version='3.6.1',
+    version='4.0',
     author="Fred L. Drake, Jr.",
     author_email="fred@fdrake.net",
     maintainer="Zope Foundation and Contributors",
     description="Structured Configuration Library",
     keywords=('configuration structured simple flexible typed hierarchy'
               ' logging'),
     long_description=README + "\n\n" + CHANGES,
@@ -57,33 +57,26 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: Zope Public License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: OS Independent',
         'Topic :: Software Development',
     ],
-    tests_require=tests_require,
+    python_requires='>=3.7',
     extras_require={
         'test': tests_require,
         'docs': [
             'sphinxcontrib-programoutput',
         ],
     },
 )
-
-
-setup(**options)
```

### Comparing `ZConfig-3.6.1/src/ZConfig/__init__.py` & `ZConfig-4.0/src/ZConfig/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 separate configuration support from configuration loading even with
 configuration data being defined and consumed by a wide range of
 separate packages.
 
 """
 __docformat__ = "reStructuredText"
 
+from io import StringIO
+
 import ZConfig.loader
-from ZConfig._compat import TextIO
 
 
 loadConfigFile = ZConfig.loader.loadConfigFile
 loadSchemaFile = ZConfig.loader.loadSchemaFile
 loadConfig = ZConfig.loader.loadConfig
 loadSchema = ZConfig.loader.loadSchema
 
@@ -190,15 +191,15 @@
     def __init__(self, exception, value, position):
         ConfigurationError.__init__(self, str(exception))
         self.exception = exception
         self.value = value
         self.lineno, self.colno, self.url = position
 
     def __str__(self):
-        s = "%s (line %s" % (self.message, self.lineno)
+        s = "{} (line {}".format(self.message, self.lineno)
         if self.colno is not None:
             s += ", %s" % self.colno
         if self.url:
             s += ", in %s)" % self.url
         else:
             s += ")"
         return s
@@ -223,17 +224,17 @@
         ConfigurationSyntaxError.__init__(
             self, "no replacement for " + repr(name), url, lineno)
 
 
 def configureLoggers(text):
     """Configure one or more loggers from configuration text."""
 
-    schema = ZConfig.loader.loadSchemaFile(TextIO("""
+    schema = ZConfig.loader.loadSchemaFile(StringIO("""
     <schema>
     <import package='ZConfig.components.logger'/>
     <multisection type='logger' name='*' attribute='loggers'/>
     </schema>
     """))
 
-    config, _ = ZConfig.loader.loadConfigFile(schema, TextIO(text))
+    config, _ = ZConfig.loader.loadConfigFile(schema, StringIO(text))
     for factory in config.loggers:
         factory()
```

### Comparing `ZConfig-3.6.1/src/ZConfig/_schema_utils.py` & `ZConfig-4.0/src/ZConfig/_schema_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,57 +7,48 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from __future__ import print_function
 
 import argparse
 import itertools
 import sys
 import textwrap
+from abc import ABC
 from abc import abstractmethod
-
-
-try:
-    from itertools import ifilter
-    from itertools import ifilterfalse
-except ImportError:
-    # Py3
-    from itertools import filterfalse as ifilterfalse
-    ifilter = filter
+from itertools import filterfalse
 
 import ZConfig.loader
-from ZConfig._compat import AbstractBaseClass
 from ZConfig.datatypes import null_conversion
 from ZConfig.info import AbstractType
 from ZConfig.info import MultiKeyInfo
 from ZConfig.info import SectionInfo
 from ZConfig.info import SectionType
 from ZConfig.info import ValueInfo
 
 
 MARKER = object()
 
 
-class _VisitorBuilder(object):
+class _VisitorBuilder:
 
     def __init__(self):
         self.visitors = []
 
     def __call__(self, Type):
         def dec(func):
             self.visitors.append((Type, func))
             return func
         return dec
 
 
-class AbstractSchemaFormatter(AbstractBaseClass):
+class AbstractSchemaFormatter(ABC):
 
     def __init__(self, schema, stream=None):
         self.stream = stream or sys.stdout
         self._dt = schema.registry.find_name
 
     def write(self, *args):
         print(*args, file=self.stream)
@@ -97,15 +88,15 @@
                         **kwargs):
         with self.describing(description):
             self.concrete_name(concrete_name)
             self.datatype(datatype)
 
             for k, v in sorted(kwargs.items()):
                 if v:
-                    self.write(self.esc("(%s: %s)" % (k, v)))
+                    self.write(self.esc("({}: {})".format(k, v)))
 
     def description(self, description):
         if description:
             self.write(self.esc(description))
 
     example = description
 
@@ -129,15 +120,15 @@
         self.write("(%s)" % self._dt(datatype))
 
     @abstractmethod
     def body(self):
         "Context manager for the whole document"
 
 
-class AbstractSchemaPrinter(AbstractBaseClass):
+class AbstractSchemaPrinter(ABC):
 
     def __init__(self, schema, stream=None,
                  allowed_names=(), excluded_names=()):
         self.schema = schema
         stream = stream or sys.stdout
         self._explained = set()
         self._seen_typenames = set()
@@ -158,20 +149,19 @@
 
             def it():
                 return filt(pred, iter_all())
 
             return it
 
         if allowed_names:
-            self._iter_schema_items = _make_filter(allowed_names, ifilter)
+            self._iter_schema_items = _make_filter(allowed_names, filter)
 
         if excluded_names:
             excluded_names = {x.lower() for x in excluded_names}
-            self._iter_schema_items = _make_filter(excluded_names,
-                                                   ifilterfalse)
+            self._iter_schema_items = _make_filter(excluded_names, filterfalse)
             self._included = lambda st: st.name not in excluded_names
 
     @abstractmethod
     def _schema_formatter(self, schema, stream):
         "Return a formatter"
 
     def _included(self, st):
@@ -211,16 +201,15 @@
                 if isinstance(info, SectionInfo):
                     if info.sectiontype.isabstract():
                         yield name, info
 
                     # XXX: This isn't catching everything. Witness the
                     # relstorage component.
                 elif isinstance(info, SectionType):
-                    for x in abstract_sections(info):
-                        yield x
+                    yield from abstract_sections(info)
         return itertools.chain(abstract_sections(everything()), everything())
 
     def printSchema(self):
         # side-effect of building may be printing
         self.buildSchema()
 
     def buildSchema(self):
@@ -326,12 +315,12 @@
         return ZConfig.loader.loadSchemaFile(schema_reader)
 
     try:
         # A component in a package
         schema_template = (
             "<schema><import package='%s' file='%s' /></schema>"
             % (package, schema))
-        from ZConfig._compat import TextIO
-        return ZConfig.loader.loadSchemaFile(TextIO(schema_template))
+        from io import StringIO
+        return ZConfig.loader.loadSchemaFile(StringIO(schema_template))
     except ZConfig.UnknownDocumentTypeError:
         # Ok, not parseable as a component. Try a simple schema.
-        return ZConfig.loader.loadSchema('package:%s:%s' % (package, schema))
+        return ZConfig.loader.loadSchema(f'package:{package}:{schema}')
```

### Comparing `ZConfig-3.6.1/src/ZConfig/cfgparser.py` & `ZConfig-4.0/src/ZConfig/cfgparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 ##############################################################################
 """Configuration parser."""
 
 import re
 
 import ZConfig
 import ZConfig.url
-from ZConfig._compat import raise_with_same_tb
 from ZConfig.substitution import isname
 from ZConfig.substitution import substitute
 
 
 # _name_re does not allow "(" or ")" for historical reasons.  Though
 # the restriction could be lifted, there seems no need to do so.
 _name_re = r"[^\s()]+"
@@ -29,15 +28,15 @@
                           % _name_re)
 _section_start_rx = re.compile(r"(?P<type>%s)"
                                r"(?:\s+(?P<name>%s))?"
                                r"$"
                                % (_name_re, _name_re))
 
 
-class ZConfigParser(object):
+class ZConfigParser:
 
     __slots__ = ('resource', 'context', 'lineno',
                  'stack', 'defines', 'file', 'url')
 
     def __init__(self, resource, context, defines=None):
         self.resource = resource
         self.context = context
@@ -188,15 +187,13 @@
             return substitute(text, self.defines)
         except ZConfig.SubstitutionReplacementError as e:
             e.lineno = self.lineno
             e.url = self.url
             raise
 
     def error(self, message):
-        raise_with_same_tb(
-            ZConfig.ConfigurationSyntaxError(
-                message, self.url, self.lineno))
+        raise ZConfig.ConfigurationSyntaxError(message, self.url, self.lineno)
 
     def _normalize_case(self, string):
         # This method is factored out solely to allow subclasses to modify
         # the behavior of the parser.
         return string.lower()
```

### Comparing `ZConfig-3.6.1/src/ZConfig/cmdline.py` & `ZConfig-4.0/src/ZConfig/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 :meth:`ExtendedConfigLoader.addOption`.
 
 """
 
 import ZConfig
 import ZConfig.loader
 import ZConfig.matcher
-from ZConfig._compat import raise_with_same_tb
 
 
 class ExtendedConfigLoader(ZConfig.loader.ConfigLoader):
     """A :class:`~.ConfigLoader` subclass that adds support for
     command-line overrides.
     """
 
@@ -93,15 +92,15 @@
             sm = ZConfig.loader.ConfigLoader.createSchemaMatcher(self)
         return sm
 
     def cook(self):
         return OptionBag(self.schema, self.schema, self.clopts)
 
 
-class OptionBag(object):
+class OptionBag:
     def __init__(self, schema, sectiontype, options):
         self.sectiontype = sectiontype
         self.schema = schema
         self.keypairs = {}
         self.sectitems = []
         self._basic_key = schema.registry.get("basic-key")
         for item in options:
@@ -112,16 +111,16 @@
             else:
                 self.sectitems.append(item)
 
     def basic_key(self, s, pos):
         try:
             return self._basic_key(s)
         except ValueError as e:
-            raise_with_same_tb(ZConfig.ConfigurationSyntaxError(
-                "could not convert basic-key value: " + str(e), *pos))
+            raise ZConfig.ConfigurationSyntaxError(
+                f"could not convert basic-key value: {e}", *pos)
 
     def add_value(self, name, val, pos):
         if name in self.keypairs:
             L = self.keypairs[name]
         else:
             L = []
             self.keypairs[name] = L
@@ -166,24 +165,24 @@
             raise ZConfig.ConfigurationError(
                 "not all command line options were consumed")
 
     def _normalize_case(self, string):
         return string.lower()
 
 
-class MatcherMixin(object):
+class MatcherMixin:
 
     def set_optionbag(self, bag):
         self.optionbag = bag
 
     def addValue(self, key, value, position):
         try:
             realkey = self.type.keytype(key)
         except ValueError as e:
-            raise_with_same_tb(ZConfig.DataConversionError(e, key, position))
+            raise ZConfig.DataConversionError(e, key, position)
 
         if realkey in self.optionbag:
             return
         ZConfig.matcher.BaseMatcher.addValue(self, key, value, position)
 
     def createChildMatcher(self, type_, name):
         sm = ZConfig.matcher.BaseMatcher.createChildMatcher(self, type_, name)
```

### Comparing `ZConfig-3.6.1/src/ZConfig/components/basic/mapping.py` & `ZConfig-4.0/src/ZConfig/components/basic/mapping.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/components/basic/mapping.xml` & `ZConfig-4.0/src/ZConfig/components/basic/mapping.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/components/basic/tests/test_mapping.py` & `ZConfig-4.0/src/ZConfig/components/basic/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/__init__.py` & `ZConfig-4.0/src/ZConfig/components/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/base-logger.xml` & `ZConfig-4.0/src/ZConfig/components/logger/base-logger.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/datatypes.py` & `ZConfig-4.0/src/ZConfig/components/logger/datatypes.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/factory.py` & `ZConfig-4.0/src/ZConfig/components/logger/factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
+from abc import ABC
 from abc import abstractmethod
 
-from ZConfig._compat import AbstractBaseClass
-
 
 _marker = object()
 
 
-class Factory(AbstractBaseClass):
+class Factory(ABC):
     """Generic wrapper for instance construction.
 
     Calling the factory causes the instance to be created if it hasn't
     already been created, and returns the object.  Calling the factory
     multiple times returns the same object.
 
     The instance is created using the factory's create() method, which
```

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/formatter.py` & `ZConfig-4.0/src/ZConfig/components/logger/formatter.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,34 +17,16 @@
 """
 
 import inspect
 import logging
 import string
 import sys
 
-import ZConfig._compat
 
-
-if sys.version_info[0] == 2:
-
-    class StringFormatter(string.Formatter):
-
-        def get_field(self, field_name, args, kwargs):
-            if field_name == '':
-                # Not correctly supported in Python 2 string.Formatter;
-                # KeyError is raised instead of IndexError for the
-                # computed index.
-                raise IndexError('tuple index out of range')
-            return string.Formatter.get_field(self, field_name, args, kwargs)
-
-else:
-    StringFormatter = string.Formatter
-
-
-class PercentStyle(object):
+class PercentStyle:
 
     logging_style = '%'
     default_format = '%(message)s'
     asctime_format = '%(asctime)s'
     asctime_search = '%(asctime)'
 
     def __init__(self, fmt):
@@ -60,15 +42,15 @@
 class StrFormatStyle(PercentStyle):
 
     logging_style = '{'
     default_format = '{message}'
     asctime_format = '{asctime}'
     asctime_search = '{asctime'
 
-    __formatter = StringFormatter()
+    __formatter = string.Formatter()
 
     def format(self, record):
         return self.__formatter.vformat(self._fmt, (), record.__dict__)
 
 
 class StringTemplateStyle(PercentStyle):
 
@@ -175,41 +157,32 @@
             #
             # - str/repr are safe
             # - numeric formatting is safe, allowing for casting to float
             #
             return 42
 
 
-class FormatterFactory(object):
+class FormatterFactory:
 
     def __init__(self, section):
         self.format = section.format
         self.dateformat = section.dateformat
         self.style = section.style
         self.stylist = _log_format_styles[self.style](self.format)
         self.formatter = section.formatter or 'logging.Formatter'
         if section.formatter:
             self.factory = resolve(section.formatter)
-        elif sys.version_info[0] == 2:
-            self.factory = Py2Formatter
-            self.formatter = __name__ + '.Py2Formatter'
         else:
             self.factory = logging.Formatter
 
         if inspect.isclass(self.factory):
             func = self.factory.__init__
         else:
             func = self.factory
-        # getargspec is deprecated, but signature is not available in Python 2.
-        try:
-            inspect.signature
-        except AttributeError:
-            params = inspect.getargspec(func).args
-        else:
-            params = inspect.signature(func).parameters
+        params = inspect.signature(func).parameters
         self._has_style_param = 'style' in params
 
         # Check that the format specified complies with the style; we
         # just want the format call to not fall over.  If it does, the
         # exception will propagate and generate a (hopefully)
         # informative error.
         #
@@ -224,26 +197,22 @@
             self.stylist.format(record)
         except IndexError:
             #
             # We're checking this exception to catch & report
             # format-style templates that used {} or {#} placeholders,
             # since those aren't allowed when formatting with a mapping.
             #
-            e = ValueError('%s formats cannot use positional placeholders')
-            ZConfig._compat.raise_with_same_tb(e)
+            raise ValueError('%s formats cannot use positional placeholders')
 
     def __call__(self):
         #
         # Need to determine if we should pass
         # style=self.message_formatter.logging_style, or if we need to
         # clobber usesTime and formatMessage directly.
         #
-        # Python 2.7 does not use formatMessage; we'll need to deal with
-        # format instead.
-        #
         stylist = self.stylist
         if self._has_style_param:
             if stylist.logging_style:
                 formatter = self.factory(self.format, self.dateformat,
                                          style=stylist.logging_style)
             else:
                 # A formatter class that supports style, but our style is
@@ -268,104 +237,8 @@
                 # Should verify that these are defined by
                 # logging.Formatter; if not, we risk losing
                 # functionality, and should scream so as to avoid
                 # surprises.
                 #
                 formatter.usesTime = stylist.usesTime
                 formatter.formatMessage = stylist.format
-                #
-                # If Python 2 and format is not overridden, we need to
-                # replace it with a version that uses formatMessage.  If
-                # it is overridden, we need to scream, because we don't
-                # know what to do.
-                #
-                if sys.version_info[0] == 2:
-                    ff = formatter.format
-                    custom = (ff.im_class.format.im_func
-                              is not logging.Formatter.format.im_func)
-                    if custom:
-                        raise ValueError(
-                            'cannot inject non-classic formatting into'
-                            ' formatter %s' % self.formatter)
-
-                    # Style was not explicitly supported in the
-                    # arguments, as expected, but the format method is
-                    # inherited from logging.Formatter, so we can deal
-                    # with this.
-                    #
-                    # Create a bound method on formatter using
-                    # Py2Formatter.format, and apply that.  That'll
-                    # still access the formatException provided by the
-                    # configured formatter factory, and do what else
-                    # that needs to be done for Python 2.
-                    #
-                    function = Py2Formatter.__dict__['format']
-                    bound = function.__get__(formatter, formatter.__class__)
-                    formatter.format = bound
-
         return formatter
-
-
-class Py2Formatter(logging.Formatter):
-
-    def __init__(self, fmt=None, datefmt=None, style='%'):
-        for stylist in _log_format_styles.values():  # pragma: no branch
-            if stylist.logging_style == style:
-                self._style = stylist(fmt)
-                break
-        logging.Formatter.__init__(self, self._style._fmt, datefmt)
-
-    def usesTime(self):
-        """
-        Check if the format uses the creation time of the record.
-        """
-        return self._style.usesTime()
-
-    def formatMessage(self, record):
-        try:
-            s = self._style.format(record)
-        except UnicodeDecodeError as e:
-            # Issue 25664. The logger name may be Unicode. Try again ...
-            try:
-                record.name = record.name.decode('utf-8')
-                s = self._style.format(record)
-            except UnicodeDecodeError:
-                raise e
-        return s
-
-    def format(self, record):
-        """
-        Format the specified record as text.
-
-        The record's attribute dictionary is used as the operand to a
-        string formatting operation which yields the returned string.
-        Before formatting the dictionary, a couple of preparatory steps
-        are carried out. The message attribute of the record is computed
-        using LogRecord.getMessage(). If the formatting string uses the
-        time (as determined by a call to usesTime(), formatTime() is
-        called to format the event time. If there is exception information,
-        it is formatted using formatException() and appended to the message.
-        """
-        record.message = record.getMessage()
-        if self.usesTime():
-            record.asctime = self.formatTime(record, self.datefmt)
-        s = self.formatMessage(record)
-        if record.exc_info:
-            # Cache the traceback text to avoid converting it multiple times
-            # (it's constant anyway)
-            if not record.exc_text:
-                record.exc_text = self.formatException(record.exc_info)
-        if record.exc_text:
-            if s[-1:] != "\n":
-                s = s + "\n"
-            try:
-                s = s + record.exc_text
-            except UnicodeError:
-                # Sometimes filenames have non-ASCII chars, which can lead
-                # to errors when s is Unicode and record.exc_text is str
-                # See issue 8924.
-                # We also use replace for when there are multiple
-                # encodings, e.g. UTF-8 for the filesystem and latin-1
-                # for a script. See issue 13232.
-                s = s + record.exc_text.decode(sys.getfilesystemencoding(),
-                                               'replace')
-        return s
```

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/handlers.py` & `ZConfig-4.0/src/ZConfig/components/logger/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ZConfig factory datatypes for log handlers."""
 
 import functools
 import sys
+import urllib.parse
 from abc import abstractmethod
 
 import ZConfig.components.logger.formatter
-from ZConfig._compat import urlparse
 from ZConfig.components.logger.factory import Factory
 
 
 _log_format_variables = (
     ZConfig.components.logger.formatter._log_format_variables)
 
 
@@ -174,15 +174,15 @@
 
     def create_loghandler(self):
         from ZConfig.components.logger import loghandler
         return loghandler.Win32EventLogHandler(self.section.appname)
 
 
 def http_handler_url(value):
-    scheme, netloc, path, param, query, fragment = urlparse.urlparse(value)
+    scheme, netloc, path, param, query, fragment = urllib.parse.urlparse(value)
     if scheme != 'http':
         raise ValueError('url must be an http url')
     if not netloc:
         raise ValueError('url must specify a location')
     if not path:
         raise ValueError('url must specify a path')
     q = []
```

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/handlers.xml` & `ZConfig-4.0/src/ZConfig/components/logger/handlers.xml`

 * *Files 2% similar despite different names*

#### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/handlers.xml` & `ZConfig-4.0/src/ZConfig/components/logger/handlers.xml`

```diff
@@ -5,17 +5,15 @@
   <sectiontype name="ZConfig.logger.base-log-handler">
     <description>Base type for most log handlers.  This is cannot be used as a
       loghandler directly since it doesn't implement the loghandler
       abstract section type.</description>
     <key name="formatter" datatype="dotted-name" required="no">
       <description>Logging formatter class.
 
-        The default is :class:`logging.Formatter` except for Python 2,
-        where a compatible formatter is used that supports the ``style``
-        option added in Python 3.
+        The default is :class:`logging.Formatter`.
 
         One alternative is 'zope.exceptions.log.Formatter',
         which enhances exception tracebacks with information from
         ``__traceback_info__`` and ``__traceback_supplement__``
         variables from each stack frame.</description>
     </key>
     <key name="dateformat" default="%Y-%m-%dT%H:%M:%S">
```

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/logger.py` & `ZConfig-4.0/src/ZConfig/components/logger/logger.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/logger.xml` & `ZConfig-4.0/src/ZConfig/components/logger/logger.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/loghandler.py` & `ZConfig-4.0/src/ZConfig/components/logger/loghandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
 """Handlers which can plug into a PEP 282 logger."""
 
 import logging
 import logging.handlers
 import os
 import weakref
-
-from ZConfig._compat import maxsize
+from sys import maxsize
 
 
 # Export these, they're used in handlers.py
 StreamHandler = logging.StreamHandler
 SysLogHandler = logging.handlers.SysLogHandler
 HTTPHandler = logging.handlers.HTTPHandler
 SMTPHandler = logging.handlers.SMTPHandler
```

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/tests/support.py` & `ZConfig-4.0/src/ZConfig/components/logger/tests/support.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 Test support for ZConfig.components.logger.
 
 """
 
 import logging
 import os
 import tempfile
+from io import StringIO
 
 import ZConfig
-import ZConfig._compat
 import ZConfig.tests.support
 from ZConfig.components.logger import loghandler
 
 
 class LoggingTestHelper(ZConfig.tests.support.TestHelper):
 
     # Not derived from unittest.TestCase; some test runners seem to
@@ -73,16 +73,16 @@
         os.rename(fn, nfn)
         return nfn
 
     _schema = None
 
     def get_schema(self):
         if self._schema is None:
-            sio = ZConfig._compat.NStringIO(self._schematext)
+            sio = StringIO(self._schematext)
             self.__class__._schema = ZConfig.loadSchemaFile(sio)
         return self._schema
 
     def get_config(self, text):
-        conf, handler = ZConfig.loadConfigFile(self.get_schema(),
-                                               ZConfig._compat.NStringIO(text))
+        conf, handler = ZConfig.loadConfigFile(
+            self.get_schema(), StringIO(text))
         self.assertTrue(not handler)
         return conf
```

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/tests/test_formatter.py` & `ZConfig-4.0/src/ZConfig/components/logger/tests/test_formatter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 ##############################################################################
 #
 # Copyright (c) 2018 Zope Foundation and Contributors.
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
@@ -252,16 +251,15 @@
                       " %(stuff) {extra} $} ${levelno  ${bad-mojo}"))
 
 
 class ZopeExceptionsFormatterTestCase(LoggerStyledFormatterTestCase):
 
     # We test against the zope.exceptions formatter since it's a common
     # example of a formatter that inherits almost everything, but
-    # defines it's own formatException.  For Python 2, we want to be
-    # sure the extended formatException is used.
+    # defines it's own formatException.
 
     _config_template = """\
       <eventlog>
         <logfile>
           path STDOUT
           level debug
           formatter zope.exceptions.log.Formatter
@@ -331,140 +329,14 @@
         logging.Formatter.__init__(self, fmt=fmt, datefmt=datefmt, **kwargs)
 
 
 def styleless_formatter(fmt=None, datefmt=None):
     return StylelessFormatter(fmt=fmt, datefmt=datefmt)
 
 
-class UnstylableFormatter(StylelessFormatter):
-
-    # Really only declared unstylable on Python 2; Python 3 formatters
-    # are assumed to be cooperative w/r/t format invoking formatMessage.
-
-    def format(self, record):
-        return 'No playing nice!'
-
-
-class UnstylableFormatterTestCase(StyledFormatterTestHelper,
-                                  unittest.TestCase):
-
-    _config_template = """\
-      <eventlog>
-        <logfile>
-          path STDOUT
-          level debug
-          formatter %s.UnstylableFormatter
-          %%s
-        </logfile>
-      </eventlog>
-    """ % __name__
-
-    @unittest.skipIf(sys.version_info[0] > 2,
-                     'Only applies for Python 2.')
-    def test_py2_unstylable(self):
-        factory = self.get_formatter_factory(
-            style='template',
-            format='$${levelname} $${levelno} $${message}')
-        with self.assertRaises(ValueError) as cm:
-            factory()
-        self.assertIn('cannot inject non-classic formatting into formatter',
-                      str(cm.exception))
-
-
-class Py2EncodingTestCase(StyledFormatterTestHelper,
-                          unittest.TestCase):
-
-    text = u'\u6d4b\u8bd5'  # u'测试'
-    encoded_text = text.encode('utf-8')
-
-    @unittest.skipIf(sys.version_info[0] > 2,
-                     'Only applies for Python 2.')
-    def test_format_message_with_unhandlable_unicode_decoding_error(self):
-        # Triggering outer exception handler in Py2Formatter.formatMessage.
-        formatter = ZConfig.components.logger.formatter.Py2Formatter(
-            '%(name)s %(message)s ' + self.encoded_text)
-        self.record.message = u'simple text'
-
-        # Because the decoding error is caused by the unicode message,
-        # decoding the nsame of the logger doesn't help:
-        with self.assertRaises(UnicodeDecodeError) as cm:
-            formatter.formatMessage(self.record)
-
-        emsg = str(cm.exception)
-        self.assertIn("'ascii' codec can't decode byte", emsg)
-        self.assertIn('ordinal not in range(128)', emsg)
-
-    @unittest.skipIf(sys.version_info[0] > 2,
-                     'Only applies for Python 2.')
-    def _test_format_message_with_unicode_logger_name(self):
-        # https://bugs.python.org/issue25664
-        logname = __name__ + '.' + self.encoded_text
-        assert isinstance(logname, bytes)
-        self.record.name = logname
-        formatter = ZConfig.components.logger.formatter.Py2Formatter(
-            '%(name)s %(message)s')
-        self.record.message = self.record.getMessage()
-
-        msg = formatter.formatMessage(self.record)
-
-        self.assertIsInstance(msg, bytes)
-        self.assertEqual(msg, logname + b" my message, 'with' 'some args'")
-
-    @unittest.skipIf(sys.version_info[0] > 2,
-                     'Only applies for Python 2.')
-    def test_format_with_unicode_traceback_content(self):
-        try:
-            raise RuntimeError('we made this up')
-        except RuntimeError:
-            self.record.exc_info = sys.exc_info()
-        formatter = ZConfig.components.logger.formatter.Py2Formatter(
-            '%(name)s %(message)s')
-        # For formatMessage to return unicode:
-        self.record.msg += u''
-        formatter.format(self.record)
-        assert isinstance(self.record.exc_text, bytes)
-        assert isinstance(formatter.formatMessage(self.record), unicode)  # NOQA
-        # We're now certain self.record.exc_text has been properly formatted.
-        # Convert to unicode and add some interesting bits.
-        encoded_text = self.text.encode(sys.getfilesystemencoding())
-        self.record.exc_text = (self.record.exc_text + encoded_text)
-        self.record.message = self.record.message.decode('utf-8')
-
-        msg = formatter.format(self.record)
-
-        self.assertIsInstance(msg, unicode)  # NOQA
-
-    @unittest.skipIf(sys.version_info[0] > 2,
-                     'Only applies for Python 2.')
-    def test_format_with_unicode_traceback_content_trailing_msg_newline(self):
-        # The point of this is to cover the case of *not* adding a
-        # newline to the message before appending the formatted
-        # traceback.
-        try:
-            raise RuntimeError('we made this up')
-        except RuntimeError:
-            self.record.exc_info = sys.exc_info()
-        formatter = ZConfig.components.logger.formatter.Py2Formatter(
-            '%(name)s %(message)s')
-        # For formatMessage to return unicode:
-        self.record.msg += u'\n'
-        formatter.format(self.record)
-        assert isinstance(self.record.exc_text, bytes)
-        assert isinstance(formatter.formatMessage(self.record), unicode)  # NOQA
-        # We're now certain self.record.exc_text has been properly formatted.
-        # Convert to unicode and add some interesting bits.
-        encoded_text = self.text.encode(sys.getfilesystemencoding())
-        self.record.exc_text = (self.record.exc_text + encoded_text)
-        self.record.message = self.record.message.decode('utf-8')
-
-        msg = formatter.format(self.record)
-
-        self.assertIsInstance(msg, unicode)  # NOQA
-
-
 class FieldTypesTestCase(StyledFormatterTestHelper, unittest.TestCase):
 
     def test_func_name_classic(self):
         formatter = self.get_formatter(
             style='classic',
             format='%(levelname)s %(levelno)2d %(funcName)s')
         output = formatter.format(self.record)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ZConfig-3.6.1/src/ZConfig/components/logger/tests/test_logger.py` & `ZConfig-4.0/src/ZConfig/components/logger/tests/test_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 """Tests for logging configuration via ZConfig."""
 
 import doctest
 import logging
 import os
 import sys
 import unittest
+from io import StringIO
+from sys import maxsize
 
 import ZConfig
 import ZConfig.components.logger.tests.support
 import ZConfig.tests.support
-from ZConfig._compat import NStringIO as StringIO
-from ZConfig._compat import maxsize
 from ZConfig.components.logger import datatypes
 from ZConfig.components.logger import handlers
 from ZConfig.components.logger import loghandler
 
 
 class CustomFormatter(logging.Formatter):
     def formatException(self, ei):
@@ -405,15 +405,14 @@
                                           "    level fatal\n"
                                           "    smtp-server foo:487\n"
                                           "    smtp-username john\n"
                                           "    smtp-password johnpw\n"
                                           "  </email-notifier>\n"
                                           "</eventlog>")
 
-        self.assertTrue(sys.version_info >= (2, 6))
         handler = logger.handlers[0]
         self.assertEqual(handler.toaddrs, ["sysadmin@example.com"])
         self.assertEqual(handler.fromaddr, "zlog-user@example.com")
         self.assertEqual(handler.fromaddr, "zlog-user@example.com")
         self.assertEqual(handler.level, logging.FATAL)
         self.assertEqual(handler.username, 'john')
         self.assertEqual(handler.password, 'johnpw')
@@ -812,15 +811,15 @@
                                'must specify a path',
                                handlers.http_handler_url, 'http://server')
 
         v = handlers.http_handler_url("http://server/path;param?q=v#fragment")
         self.assertEqual(v, ('server', '/path;param?q=v#fragment'))
 
     def test_close_files(self):
-        class F(object):
+        class F:
             closed = 0
 
             def close(self):
                 self.closed += 1
 
         f = F()
```

### Comparing `ZConfig-3.6.1/src/ZConfig/datatypes.py` & `ZConfig-4.0/src/ZConfig/datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,18 @@
 
 """
 
 import datetime
 import os
 import re
 import sys
+from functools import reduce
 
-from ZConfig._compat import PY3
-from ZConfig._compat import have_unicode
-from ZConfig._compat import text_type
 
-
-if PY3:
-    from functools import reduce
-
-
-class MemoizedConversion(object):
+class MemoizedConversion:
     """Simple memoization for potentially expensive conversions.
 
     This conversion helper caches each successful conversion for re-use
     at a later time; failed conversions are not cached in any way, since
     it is difficult to raise a meaningful exception providing
     information about the specific failure.
 
@@ -63,15 +56,15 @@
             return self._memo[value]
         except KeyError:
             v = self._conversion(value)
             self._memo[value] = v
             return v
 
 
-class RangeCheckedConversion(object):
+class RangeCheckedConversion:
     """Conversion helper that performs range checks on the result of
     another conversion.
 
     Values passed to instances of this conversion are converted using
     *conversion* and then range checked. *min* and *max*, if given and
     not ``None``, are the inclusive endpoints of the allowed range.
     Values returned by *conversion* which lay outside the range
@@ -91,15 +84,15 @@
                              % (repr(v), repr(self._min)))
         if self._max is not None and v > self._max:
             raise ValueError("%s is above upper bound (%s)"
                              % (repr(v), repr(self._max)))
         return v
 
 
-class RegularExpressionConversion(object):
+class RegularExpressionConversion:
     """Conversion that checks that the input matches the regular
     expression *regex*.
 
     If it matches, returns the input, otherwise raises
     :exc:`ValueError`.
     """
 
@@ -109,15 +102,15 @@
         self._rx = re.compile(regex)
 
     def __call__(self, value):
         m = self._rx.match(value)
         if m and m.group() == value:
             return value
         else:
-            raise ValueError("%s: %s" % (self.reason, repr(value)))
+            raise ValueError("{}: {}".format(self.reason, repr(value)))
 
 
 def check_locale(value):
     import locale
     prev = locale.setlocale(locale.LC_ALL)
     try:
         try:
@@ -140,20 +133,15 @@
 
     def __call__(self, value):
         value = str(value)
         return RegularExpressionConversion.__call__(self, value).lower()
 
 
 class ASCIIConversion(RegularExpressionConversion):
-
-    def __call__(self, value):
-        value = RegularExpressionConversion.__call__(self, value)
-        if have_unicode and isinstance(value, text_type):
-            value = value.encode("ascii")
-        return value
+    pass
 
 
 _ident_re = "[_a-zA-Z][_a-zA-Z0-9]*"
 
 
 class IdentifierConversion(ASCIIConversion):
     reason = "not a valid Python identifier"
@@ -163,15 +151,15 @@
 
 
 class DottedNameConversion(ASCIIConversion):
     reason = "not a valid dotted name"
 
     def __init__(self):
         ASCIIConversion.__init__(self,
-                                 r"%s(?:\.%s)*" % (_ident_re, _ident_re))
+                                 r"{}(?:\.{})*".format(_ident_re, _ident_re))
 
 
 class DottedNameSuffixConversion(ASCIIConversion):
     reason = "not a valid dotted name or suffix"
 
     def __init__(self):
         ASCIIConversion.__init__(self,
@@ -202,15 +190,15 @@
     """Convert a string to a list of strings using .split()."""
     return s.split()
 
 
 port_number = RangeCheckedConversion(integer, min=0, max=0xffff).__call__
 
 
-class InetAddress(object):
+class InetAddress:
 
     def __init__(self, default_host):
         self.DEFAULT_HOST = default_host
 
     def __call__(self, s):
         # returns (host, port) tuple
         host = ''
@@ -246,15 +234,15 @@
     DEFAULT_HOST = ""
 
 inet_address = InetAddress(DEFAULT_HOST)
 inet_connection_address = InetAddress("127.0.0.1")
 inet_binding_address = InetAddress("")
 
 
-class SocketAddress(object):
+class SocketAddress:
     # Parsing results in family and address
     # Family can be AF_UNIX (for addresses that are path names)
     # or AF_INET6 (for inet addresses with colons in them)
     # or AF_INET (for all other inet addresses);
     # An inet address is a (host, port) pair
     # Notice that no DNS lookup is performed, so if the host
     # is a DNS name, DNS lookup may end up with either IPv4 or
@@ -311,15 +299,15 @@
         result = RegularExpressionConversion.__call__(self, value).lower()
         # Use C library to validate IPv6 addresses, in particular wrt.
         # number of colons and number of digits per group
         if ':' in result:
             import socket
             try:
                 socket.inet_pton(socket.AF_INET6, result)
-            except socket.error:
+            except OSError:
                 raise ValueError('%r is not a valid IPv6 address' % value)
         return result
 
 
 def existing_directory(v):
     nv = os.path.expanduser(v)
     if os.path.isdir(nv):
@@ -349,15 +337,15 @@
         return nv
     if os.path.isdir(dirname):
         return nv
     raise ValueError('The directory named as part of the path %s '
                      'does not exist.' % v)
 
 
-class SuffixMultiplier(object):
+class SuffixMultiplier:
     # d is a dictionary of suffixes to integer multipliers.  If no suffixes
     # match, default is the multiplier.  Matches are case insensitive.  Return
     # values are in the fundamental unit.
     def __init__(self, d, default=1):
         self._d = d
         self._default = default
         # all keys must be the same size
@@ -405,15 +393,15 @@
         elif suffix == 'h':
             hours = val
         elif suffix == 'm':
             minutes = val
         elif suffix == 's':
             seconds = val
         else:
-            raise TypeError('bad part %s in %s' % (part, s))
+            raise TypeError('bad part {} in {}'.format(part, s))
     return datetime.timedelta(weeks=weeks, days=days, hours=hours,
                               minutes=minutes, seconds=seconds)
 
 
 stock_datatypes = {
     "boolean":           asBoolean,
     "dotted-name":       DottedNameConversion(),
@@ -447,15 +435,15 @@
                                            'h': 60*60,
                                            'd': 60*60*24,
                                            }),
     "timedelta":         timedelta,
     }
 
 
-class Registry(object):
+class Registry:
     """Implementation of a simple type registry.
 
     If given, *stock* should be a mapping which defines the "built-in"
     data types for the registry; if omitted or ``None``, the standard
     set of data types is used (see :ref:`standard-datatypes`).
 
     """
```

### Comparing `ZConfig-3.6.1/src/ZConfig/info.py` & `ZConfig-4.0/src/ZConfig/info.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Objects that can describe a ZConfig schema."""
 
 import copy
+from abc import ABC
 from abc import abstractmethod
 from collections import OrderedDict
 from functools import total_ordering
 
 import ZConfig
-from ZConfig._compat import AbstractBaseClass
 
 
 @total_ordering
-class UnboundedThing(object):
+class UnboundedThing:
     __slots__ = ()
 
     def __gt__(self, other):
         if isinstance(other, self.__class__):
             return False
         return True
 
@@ -37,30 +37,30 @@
     def __repr__(self):
         return "<Unbounded>"
 
 
 Unbounded = UnboundedThing()
 
 
-class ValueInfo(object):
+class ValueInfo:
     __slots__ = 'value', 'position'
 
     def __init__(self, value, position):
         self.value = value
         # position is (lineno, colno, url)
         self.position = position
 
     def convert(self, datatype):
         try:
             return datatype(self.value)
         except ValueError as e:
             raise ZConfig.DataConversionError(e, self.value, self.position)
 
 
-class BaseInfo(object):
+class BaseInfo:
     """Information about a single configuration key."""
 
     description = None
     example = None
     metadefault = None
 
     def __init__(self, name, datatype, minOccurs, maxOccurs, handler,
@@ -81,27 +81,27 @@
         self.minOccurs = minOccurs
         self.maxOccurs = maxOccurs
         self.handler = handler
         self.attribute = attribute
 
     def __repr__(self):
         clsname = self.__class__.__name__
-        return "<%s for %s>" % (clsname, repr(self.name))
+        return "<{} for {}>".format(clsname, repr(self.name))
 
     def isabstract(self):
         return False
 
     def ismulti(self):
         return self.maxOccurs > 1
 
     def issection(self):
         return False
 
 
-class BaseKeyInfo(AbstractBaseClass, BaseInfo):
+class BaseKeyInfo(ABC, BaseInfo):
 
     _rawdefaults = None
 
     def __init__(self, name, datatype, minOccurs, maxOccurs, handler,
                  attribute):
         BaseInfo.__init__(self, name, datatype, minOccurs, maxOccurs,
                           handler, attribute)
@@ -240,15 +240,15 @@
             datatype = sectiontype.datatype
         BaseInfo.__init__(self, name, datatype,
                           minOccurs, maxOccurs, handler, attribute)
         self.sectiontype = sectiontype
 
     def __repr__(self):
         clsname = self.__class__.__name__
-        return "<%s for %s (%s)>" % (
+        return "<{} for {} ({})>".format(
             clsname, self.sectiontype.name, repr(self.name))
 
     def issection(self):
         return True
 
     def allowUnnamed(self):
         return self.name == "*"
@@ -267,15 +267,15 @@
         # sections cannot have defaults
         if self.maxOccurs > 1:
             return []
         else:
             return None
 
 
-class AbstractType(object):
+class AbstractType:
     # This isn't actually "abstract" in the Python ABC sense,
     # it's only abstract from the schema sense. This class is
     # instantiated, and not expected to be subclassed.
     __slots__ = '_subtypes', 'name', 'description'
 
     def __init__(self, name):
         self._subtypes = OrderedDict()
@@ -303,15 +303,15 @@
         """Return the names of all concrete types as a sorted list."""
         return sorted(self._subtypes.keys())
 
     def isabstract(self):
         return True
 
 
-class SectionType(object):
+class SectionType:
     def __init__(self, name, keytype, valuetype, datatype, registry, types):
         # name      - name of the section, or '*' or '+'
         # datatype  - type for the section itself
         # keytype   - type for the keys themselves
         # valuetype - default type for key values
         self.name = name
         self.datatype = datatype
```

### Comparing `ZConfig-3.6.1/src/ZConfig/loader.py` & `ZConfig-4.0/src/ZConfig/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,29 +12,27 @@
 #
 ##############################################################################
 """Schema loader utility."""
 
 import os.path
 import re
 import sys
+import urllib.request
+from abc import ABC
 from abc import abstractmethod
 from io import StringIO
+from urllib.request import pathname2url
 
 import ZConfig
 import ZConfig.cfgparser
 import ZConfig.datatypes
 import ZConfig.info
 import ZConfig.matcher
 import ZConfig.schema
 import ZConfig.url
-from ZConfig._compat import AbstractBaseClass
-from ZConfig._compat import pathname2url
-from ZConfig._compat import raise_with_same_tb
-from ZConfig._compat import reraise
-from ZConfig._compat import urllib2
 
 
 def loadSchema(url):
     """Load a schema definition from the URL *url*.
 
     *url* may be a URL, absolute pathname, or relative pathname.
     Fragment identifiers are not supported.
@@ -120,15 +118,15 @@
         for opt in overrides:
             loader.addOption(opt)
     else:
         loader = ConfigLoader(schema)
     return loader
 
 
-class BaseLoader(AbstractBaseClass):
+class BaseLoader(ABC):
     """Base class for loader objects.
 
     This should not be instantiated
     directly, as the :meth:`loadResource` method must be overridden
     for the instance to be used via the public API.
     """
 
@@ -180,15 +178,15 @@
         actually load the resource and return the appropriate
         application-level object.
         """
 
     def openResource(self, url):
         """Returns a resource object that represents the URL *url*.
 
-        The URL is opened using the :func:`urllib2.urlopen` function,
+        The URL is opened using the :func:`urllib.request.urlopen` function,
         and the returned resource object is created using
         :meth:`createResource`. If the URL cannot be opened,
         :exc:`~.ConfigurationError` is raised.
         """
         # ConfigurationError exceptions raised here should be
         # str()able to generate a message for an end user.
         #
@@ -198,52 +196,42 @@
         # resource is not accessible.
         url = str(url)
         if url.startswith("package:"):
             _, package, filename = url.split(":", 2)
             file = openPackageResource(package, filename)
         else:
             try:
-                file = urllib2.urlopen(url)
-            except urllib2.URLError as e:
-                # urllib2.URLError has a particularly hostile str(), so we
-                # generally don't want to pass it along to the user.
+                file = urllib.request.urlopen(url)
+            except urllib.request.URLError as e:
+                # urllib.request.URLError has a particularly hostile str(), so
+                # we generally don't want to pass it along to the user.
                 self._raise_open_error(url, e.reason)  # pragma: no cover
-            except (IOError, OSError) as e:
-                # Python 2.1 raises a different error from Python 2.2+,
-                # so we catch both to make sure we detect the situation.
+            except OSError as e:
                 self._raise_open_error(url, str(e))
 
-            # Python 3 support: file.read() returns bytes, so we convert it
-            # to an StringIO.  (Can't use io.TextIOWrapper because of
-            # http://bugs.python.org/issue16723 and probably other bugs).
-            # Do this even on Python 2 to avoid keeping a network connection
-            # open for an unbounded amount of time and to catch IOErrors here,
-            # where they make sense.
             try:
                 data = file.read()
             finally:
                 file.close()
             if isinstance(data, bytes):
                 # Be sure to specify an (useful) encoding so we don't get
                 # the system default, typically ascii.
                 data = data.decode('utf-8')
             file = StringIO(data)
         return self.createResource(file, url)
 
     def _raise_open_error(self, url, message):
         if url[:7].lower() == "file://":
             what = "file"
-            ident = urllib2.url2pathname(url[7:])
+            ident = urllib.request.url2pathname(url[7:])
         else:
             what = "URL"
             ident = url
-        error = ZConfig.ConfigurationError(
-            "error opening %s %s: %s" % (what, ident, message),
-            url)
-        raise_with_same_tb(error)
+        raise ZConfig.ConfigurationError(
+            "error opening {} {}: {}".format(what, ident, message), url)
 
     def normalizeURL(self, url):
         """Return a URL for *url*
 
         If *url* refers to an existing file, the corresponding
         ``file:`` URL is returned. Otherwise *url* is checked
         for sanity: if it does not have a schema, :exc:`ValueError` is
@@ -297,15 +285,15 @@
         else:
             raise ZConfig.SchemaResourceError("schema component not found",
                                               filename=path,
                                               package=package,
                                               path=pkg.__path__)
         url = "file:" + pathname2url(filename)
         url = ZConfig.url.urlnormalize(url)
-        return urllib2.urlopen(url)
+        return urllib.parse.urlopen(url)
     else:
         v, tb = (None, None)
         for dirname in pkg.__path__:
             loadpath = os.path.join(dirname, path)
             try:
                 return StringIO(
                     loader.get_data(loadpath).decode('utf-8'))
@@ -315,15 +303,15 @@
                     filename=path,
                     package=package,
                     path=pkg.__path__)
                 tb = sys.exc_info()[2]
 
         if v is not None:
             try:
-                reraise(type(v), v, tb)
+                raise v.with_traceback(tb)
             finally:
                 del tb
 
         raise ZConfig.SchemaResourceError("schema component not found",
                                           filename=path,
                                           package=package,
                                           path=pkg.__path__)
@@ -371,23 +359,23 @@
             raise ZConfig.SchemaError(
                 "illegal schema component name: " + repr(package))
         filename = filename or "component.xml"
         try:
             __import__(package)
         except ImportError as e:
             raise ZConfig.SchemaResourceError(
-                "could not load package %s: %s" % (package, str(e)),
+                "could not load package {}: {}".format(package, str(e)),
                 filename=filename,
                 package=package)
         pkg = sys.modules[package]
         if not hasattr(pkg, "__path__"):
             raise ZConfig.SchemaResourceError(
                 "import name does not refer to a package",
                 filename=filename, package=package)
-        return "package:%s:%s" % (package, filename)
+        return "package:{}:{}".format(package, filename)
 
 
 class ConfigLoader(BaseLoader):
     """Loader for configuration files.
 
     Each configuration file must
     conform to the schema *schema*.  The ``load*()`` methods
@@ -450,15 +438,15 @@
     # internal helper
 
     def _parse_resource(self, matcher, resource, defines=None):
         parser = ZConfig.cfgparser.ZConfigParser(resource, self, defines)
         parser.parse(matcher)
 
 
-class CompositeHandler(object):
+class CompositeHandler:
 
     def __init__(self, handlers, schema):
         self._handlers = handlers
         self._convert = schema.registry.get("basic-key")
 
     def __call__(self, handlermap):
         d = {}
@@ -481,15 +469,15 @@
             if f is not None:
                 f(value)
 
     def __len__(self):
         return len(self._handlers)
 
 
-class Resource(object):
+class Resource:
     """Object that allows an open file object and a URL to be bound
     together to ease handling.
 
     Instances have the attributes :attr:`file` and :attr:`url`, which
     store the constructor arguments. These objects also have a
     :meth:`close` method which will call :meth:`~file.close` on
     *file*, then set the :attr:`file` attribute to ``None`` and the
```

### Comparing `ZConfig-3.6.1/src/ZConfig/matcher.py` & `ZConfig-4.0/src/ZConfig/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Utility that manages the binding of configuration data to a section."""
 
 import ZConfig
-from ZConfig._compat import raise_with_same_tb
 from ZConfig.info import ValueInfo
 
 
-class BaseMatcher(object):
+class BaseMatcher:
     def __init__(self, info, type_, handlers):
         self.info = info
         self.type = type_
         self._values = {}
         for _type_key, type_info in type_:
             if type_info.name == "+" and not type_info.issection():
                 v = {}
@@ -34,15 +33,15 @@
             self._values[type_info.attribute] = v
         self._sectionnames = {}
         self.handlers = handlers if handlers is not None else []
 
     def __repr__(self):
         clsname = self.__class__.__name__
         extra = "type " + repr(self.type.name)
-        return "<%s for %s>" % (clsname, extra)
+        return "<{} for {}>".format(clsname, extra)
 
     def addSection(self, type_, name, sectvalue):
         if name:
             if name in self._sectionnames:
                 raise ZConfig.ConfigurationError(
                     "section names must not be re-used within the"
                     " same container:" + repr(name))
@@ -77,15 +76,15 @@
             k, ci = arbkey_info
         if ci.issection():  # pragma: no cover
             if ci.name:
                 extra = " in %s sections" % repr(self.type.name)
             else:
                 extra = ""
             raise ZConfig.ConfigurationError(
-                "%s is not a valid key name%s" % (repr(key), extra))
+                "{} is not a valid key name{}".format(repr(key), extra))
 
         ismulti = ci.ismulti()
         attr = ci.attribute
         assert attr is not None
         v = self._values[attr]
         if v is None:
             if k == '+':
@@ -148,15 +147,15 @@
                     raise ZConfig.ConfigurationError(
                         "no keys defined for the %s key/value map; at least %d"
                         " must be specified" % (attr, ci.minOccurs))
             if v is None and ci.minOccurs:
                 default = ci.getdefault()
                 if default is None:
                     raise ZConfig.ConfigurationError(
-                        "no values for %s; %s required" % (key, ci.minOccurs))
+                        f"no values for {key}; {ci.minOccurs} required")
                 else:
                     v = values[attr] = default[:]  # pragma: no cover
             if ci.ismulti():
                 if not v:
                     default = ci.getdefault()
                     if isinstance(default, dict):
                         v.update(default)
@@ -184,32 +183,32 @@
                     v = []
                     for s in values[attr]:
                         if s is not None:
                             st = s.getSectionDefinition()
                             try:
                                 s = st.datatype(s)
                             except ValueError as e:
-                                raise_with_same_tb(ZConfig.DataConversionError(
-                                    e, s, (-1, -1, None)))
+                                raise ZConfig.DataConversionError(
+                                    e, s, (-1, -1, None))
 
                         v.append(s)
                 elif ci.name == '+':
                     v = values[attr]
                     for key, val in v.items():
                         v[key] = [vi.convert(ci.datatype) for vi in val]
                 else:
                     v = [vi.convert(ci.datatype) for vi in values[attr]]
             elif ci.issection():
                 if values[attr] is not None:
                     st = values[attr].getSectionDefinition()
                     try:
                         v = st.datatype(values[attr])
                     except ValueError as e:
-                        raise_with_same_tb(ZConfig.DataConversionError(
-                            e, values[attr], (-1, -1, None)))
+                        raise ZConfig.DataConversionError(
+                            e, values[attr], (-1, -1, None))
 
                 else:
                     v = None
             elif name == '+':
                 v = values[attr]
                 if not v:
                     for key, val in ci.getdefault().items():
@@ -253,15 +252,15 @@
         v = BaseMatcher.finish(self)
         v = self.type.datatype(v)
         if self.type.handler is not None:
             self.handlers.append((self.type.handler, v))
         return v
 
 
-class SectionValue(object):
+class SectionValue:
     """Generic 'bag-of-values' object for a section.
 
     Derived classes should always call the SectionValue constructor
     before attempting to modify self.
     """
 
     def __init__(self, values, name, matcher):
@@ -274,15 +273,15 @@
         if self._name:
             # probably unique for a given config file; more readable than id()
             name = repr(self._name)
         else:
             # identify uniquely
             name = "at %#x" % id(self)
         clsname = self.__class__.__name__
-        return "<%s for %s %s>" % (clsname, self._matcher.type.name, name)
+        return "<{} for {} {}>".format(clsname, self._matcher.type.name, name)
 
     def __str__(self):
         lst = []
         attrnames = sorted([s for s in self.__dict__ if s[0] != "_"])
         for k in attrnames:
             v = getattr(self, k)
             lst.append('%-40s: %s' % (k, v))
```

### Comparing `ZConfig-3.6.1/src/ZConfig/pygments.py` & `ZConfig-4.0/src/ZConfig/pygments.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 #
 ##############################################################################
 """\
 pygments-compatible lexer.
 
 """
 
-from __future__ import absolute_import
-from __future__ import print_function
 
 import pygments.lexer
 import pygments.token
 
 import ZConfig.substitution
```

### Comparing `ZConfig-3.6.1/src/ZConfig/schema.py` & `ZConfig-4.0/src/ZConfig/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,44 +10,32 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Parser for ZConfig schemas."""
 
 import os
-import sys
 import xml.sax
 
 import ZConfig
 from ZConfig import info
 from ZConfig import url
-from ZConfig._compat import raise_with_same_tb
-
-
-BLANK = u''
 
 
 def parseResource(resource, loader):
     parser = SchemaParser(loader, resource.url)
     xml.sax.parse(resource.file, parser)
     return parser._schema
 
 
 def parseComponent(resource, loader, schema):
     parser = ComponentParser(loader, resource.url, schema)
     xml.sax.parse(resource.file, parser)
 
 
-def _srepr(ob):
-    if isinstance(ob, type(BLANK)) and sys.version_info[0] < 3:
-        # drop the leading "u" from a unicode repr
-        return repr(ob)[1:]
-    return repr(ob)
-
-
 class BaseParser(xml.sax.ContentHandler):
 
     _cdata_tags = "description", "metadefault", "example", "default"
     _handled_tags = ("import", "abstracttype", "sectiontype",
                      "key", "multikey", "section", "multisection")
 
     _allowed_parents = {
@@ -88,16 +76,17 @@
     def startElement(self, name, attrs):
         attrs = dict(attrs)
         if self._elem_stack:
             parent = self._elem_stack[-1]
             if name not in self._allowed_parents:
                 self.error("Unknown tag " + name)
             if parent not in self._allowed_parents[name]:
-                self.error("%s elements may not be nested in %s elements"
-                           % (_srepr(name), _srepr(parent)))
+                self.error(
+                    f"{name!r} elements may not be nested"
+                    " in {parent!r} elements")
         elif name != self._top_level:
             self.error("Unknown document type " + name,
                        ZConfig.UnknownDocumentTypeError)
 
         self._elem_stack.append(name)
 
         # self._schema is assigned to in self.start_<_top_level>, so
@@ -164,16 +153,15 @@
             if self._prefixes:
                 convert = self._registry.get("dotted-suffix")
             else:
                 convert = self._registry.get("dotted-name")
             try:
                 name = convert(name)
             except ValueError as err:
-                self.error("not a valid prefix: %s (%s)"
-                           % (_srepr(name), str(err)))
+                self.error(f"not a valid prefix: {name!r} ({err})")
             if name[0] == ".":
                 prefix = self._prefixes[-1] + name
             else:
                 prefix = name
         elif self._prefixes:
             prefix = self._prefixes[-1]
         else:
@@ -464,15 +452,15 @@
             e.lineno = self._locator.getLineNumber()
             e.url = self._locator.getSystemId()
         return e
 
     def error(self, message, kind=None):
         # Can't do this as a default value because of import order
         kind = kind or ZConfig.SchemaError
-        raise_with_same_tb(self.initerror(kind(message)))
+        raise self.initerror(kind(message))
 
 
 class SchemaParser(BaseParser):
 
     # needed by startElement() and endElement()
     _handled_tags = BaseParser._handled_tags + ("schema",)
     _top_level = "schema"
```

### Comparing `ZConfig-3.6.1/src/ZConfig/schema2html.py` & `ZConfig-4.0/src/ZConfig/schema2html.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,17 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 import argparse
-from contextlib import contextmanager
-
-
-try:
-    import html
-except ImportError:
-    # Py2
-    import cgi as html
-
+import html
 import sys
+from contextlib import contextmanager
 
 from ZConfig._schema_utils import MARKER
 from ZConfig._schema_utils import AbstractSchemaFormatter
 from ZConfig._schema_utils import AbstractSchemaPrinter
 from ZConfig._schema_utils import load_schema
 from ZConfig.sphinx import RstSchemaPrinter
```

### Comparing `ZConfig-3.6.1/src/ZConfig/schemaless.py` & `ZConfig-4.0/src/ZConfig/schemaless.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def loadConfigFile(file, url=None):
     c = Context()
     Parser(Resource(file, url), c).parse(c.top)
     return c.top
 
 
-class Resource(object):
+class Resource:
 
     def __init__(self, file, url=''):
         self.file, self.url = file, url
 
 
 class Section(dict):
 
@@ -55,43 +55,43 @@
         if self.imports:
             for pkgname in self.imports:
                 result.append('%import ' + pkgname)
             result.append('')
 
         if self.type:
             if self.name:
-                start = '%s<%s %s>' % (pre, self.type, self.name)
+                start = '{}<{} {}>'.format(pre, self.type, self.name)
             else:
-                start = '%s<%s>' % (pre, self.type)
+                start = '{}<{}>'.format(pre, self.type)
             result.append(start)
             pre += '  '
 
         lst = sorted(self.items())
         for name, values in lst:
             for value in values:
-                result.append('%s%s %s' % (pre, name, value))
+                result.append('{}{} {}'.format(pre, name, value))
 
         if self.sections and self:
             result.append('')
 
         for section in self.sections:
             result.append(section.__str__(pre))
 
         if self.type:
             pre = pre[:-2]
-            result.append('%s</%s>' % (pre, self.type))
+            result.append('{}</{}>'.format(pre, self.type))
             result.append('')
 
         result = '\n'.join(result).rstrip()
         if not pre:
             result += '\n'
         return result
 
 
-class Context(object):
+class Context:
 
     def __init__(self):
         self.top = Section()
         self.sections = []
 
     def startSection(self, container, type_, name):
         newsec = Section(type_, name)
```

### Comparing `ZConfig-3.6.1/src/ZConfig/schemaless.txt` & `ZConfig-4.0/src/ZConfig/schemaless.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   ...
   ... <another named>
   ...   nothing here
   ... </another>
   ...
   ... '''
 
-  >>> from ZConfig._compat import NStringIO as StringIO
+  >>> from io import StringIO
   >>> config = schemaless.loadConfigFile(StringIO(config_text))
 
 The `config` object is a mapping from top-level keys to lists of
 values::
 
   >>> config["some-key"]
   ['some-value', 'another-value']
```

### Comparing `ZConfig-3.6.1/src/ZConfig/sphinx.py` & `ZConfig-4.0/src/ZConfig/sphinx.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from __future__ import absolute_import
-from __future__ import print_function
 
 from contextlib import contextmanager
 
 
 try:
     import docutils.frontend
     import docutils.parsers.rst
@@ -24,26 +22,25 @@
     from docutils import nodes
     from docutils.parsers.rst import Directive
 except ImportError:  # pragma: no cover
     RstSchemaPrinter = None
     RstSchemaFormatter = None
 else:
 
-    from ZConfig._compat import string_types
     from ZConfig._schema_utils import MARKER
     from ZConfig._schema_utils import AbstractSchemaFormatter
     from ZConfig._schema_utils import AbstractSchemaPrinter
     from ZConfig._schema_utils import load_schema
 
     class RstSchemaFormatter(AbstractSchemaFormatter):
 
         settings = None
 
         def __init__(self, schema, stream=None):
-            super(RstSchemaFormatter, self).__init__(schema, stream)
+            super().__init__(schema, stream)
             self.document = None
             self._current_node = None
             self._nodes = []
             self.settings = docutils.frontend.OptionParser(
                 components=(docutils.parsers.rst.Parser,)).get_default_values()
 
         def esc(self, text):
@@ -56,15 +53,15 @@
 
             parser = docutils.parsers.rst.Parser()
             parser.parse(text, document)
             return document.children
 
         def write(self, *texts):
             for text in texts:
-                if isinstance(text, string_types):
+                if isinstance(text, str):
                     self._current_node += nodes.Text(' ' + text + ' ', text)
                 else:
                     # Already parsed
                     self._current_node += text
 
         def description(self, text):
             if not text:
@@ -141,15 +138,15 @@
                 settings=self.settings)
             yield
 
     class RstSchemaPrinter(AbstractSchemaPrinter):
         _schema_formatter = RstSchemaFormatter
 
         def printSchema(self):
-            super(RstSchemaPrinter, self).printSchema()
+            super().printSchema()
             print(self.fmt.document.pformat(), file=self.fmt.stream)
 
     class SchemaToRstDirective(Directive):
         required_arguments = 1
         optional_arguments = 0
         option_spec = {
             'file': str,
```

### Comparing `ZConfig-3.6.1/src/ZConfig/substitution.py` & `ZConfig-4.0/src/ZConfig/substitution.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/__init__.py` & `ZConfig-4.0/src/ZConfig/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/foosample.zip` & `ZConfig-4.0/src/ZConfig/tests/foosample.zip`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/input/simple.xml` & `ZConfig-4.0/src/ZConfig/tests/input/simple.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/input/simplesections.xml` & `ZConfig-4.0/src/ZConfig/tests/input/simplesections.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/library/thing/__init__.py` & `ZConfig-4.0/src/ZConfig/tests/library/thing/__init__.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/sphinx_test_schema.xml` & `ZConfig-4.0/src/ZConfig/tests/sphinx_test_schema.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/support.py` & `ZConfig-4.0/src/ZConfig/tests/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 """Support code shared among the tests."""
 
 import contextlib
 import os
 import sys
 import unittest
+from io import StringIO
+from urllib.request import pathname2url
 
 import ZConfig
-from ZConfig._compat import NStringIO as StringIO
-from ZConfig._compat import pathname2url
 from ZConfig.loader import ConfigLoader
 from ZConfig.url import urljoin
 
 
 INPUT_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), "input"))
 CONFIG_BASE = "file://%s/" % pathname2url(INPUT_DIR)
 
@@ -72,15 +72,15 @@
             with stdin_replaced():
                 f(self)
         return f2
 
     return make_wrapper
 
 
-class TestHelper(object):
+class TestHelper:
     """Utility methods which can be used with the schema support."""
 
     # Not derived from unittest.TestCase; some test runners seem to
     # think that means this class contains tests.
 
     assertRaisesRegex = getattr(unittest.TestCase, 'assertRaisesRegex',
                                 unittest.TestCase.assertRaisesRegexp)
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_cfgimports.py` & `ZConfig-4.0/src/ZConfig/tests/test_cfgimports.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests of the %import mechanism.
 """
 
 import unittest
+from io import StringIO
 
 import ZConfig
 import ZConfig.tests.support
-from ZConfig._compat import NStringIO as StringIO
 
 
 class TestImportFromConfiguration(ZConfig.tests.support.TestHelper,
                                   unittest.TestCase):
 
     def test_simple_import(self):
         schema = self.load_schema_text("<schema/>")
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_cmdline.py` & `ZConfig-4.0/src/ZConfig/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_config.py` & `ZConfig-4.0/src/ZConfig/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests of the configuration data structures and loader."""
 import os
 import tempfile
 import unittest
+from io import StringIO
 
 import ZConfig
-from ZConfig._compat import NStringIO as StringIO
 from ZConfig.tests.support import CONFIG_BASE
 from ZConfig.tests.support import TestHelper
 
 
 class ConfigurationTestCase(TestHelper, unittest.TestCase):
 
     schema = None
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_cookbook.py` & `ZConfig-4.0/src/ZConfig/tests/test_cookbook.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_datatypes.py` & `ZConfig-4.0/src/ZConfig/tests/test_datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import os
 import shutil
 import socket
 import sys
 import tempfile
 import unittest
 
-import ZConfig._compat
 import ZConfig.datatypes
 from ZConfig.tests.support import TestHelper
 
 
 here = os.path.abspath(__file__)
 
 
@@ -65,30 +64,28 @@
 
     def test_datatype_float(self):
         convert = self.types.get("float")
         eq = self.assertEqual
         raises = self.assertRaises
 
         eq(convert("1"), 1.0)
-        self.assertIs(type(convert(1)), type(1.0))
+        self.assertIs(type(convert(1)), float)
         eq(convert("1.1"), 1.1)
         eq(convert("50.50"), 50.50)
         eq(convert("-50.50"), -50.50)
         eq(convert(0), 0.0)
         eq(convert("0"), 0.0)
         eq(convert("-0"), 0.0)
         eq(convert("0.0"), 0.0)
 
         raises(ValueError, convert, "junk")
         raises(ValueError, convert, "0x234.1.9")
         raises(ValueError, convert, "0.9-")
 
-        # float handles inf/nan portably in both bytes and
-        # unicode on both Python 2.6+ and Python 3. Make sure conversion
-        # does too.
+        # float handles inf/nan. Make sure conversion does too.
         for literal in ("inf", "-inf", b"inf", b"-inf"):
             eq(convert(literal), float(literal))
 
         # notably, nan is not equal to itself
         self.assertNotEqual(convert("nan"), float("nan"))
         self.assertNotEqual(convert(b"nan"), float(b"nan"))
 
@@ -109,19 +106,14 @@
         eq(convert, "_123")
         eq(convert, "__dict__")
 
     def assert_ascii_equal(self, convert, value):
         v = convert(value)
         self.assertEqual(v, value)
         self.assertTrue(isinstance(v, str))
-        if ZConfig._compat.have_unicode:
-            unicode_value = ZConfig._compat.text_type(value)
-            v = convert(unicode_value)
-            self.assertEqual(v, value)
-            self.assertTrue(isinstance(v, str))
 
     def check_never_namelike(self, convert):
         raises = self.assertRaises
         raises(ValueError, convert, "2345")
         raises(ValueError, convert, "23.45")
         raises(ValueError, convert, ".45")
         raises(ValueError, convert, "23.")
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_info.py` & `ZConfig-4.0/src/ZConfig/tests/test_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                                'value', None)
 
 
 class SectionInfoTestCase(InfoMixin, unittest.TestCase):
 
     Class = SectionInfo
 
-    class MockSectionType(object):
+    class MockSectionType:
         name = None
 
         @classmethod
         def isabstract(cls):
             return True
 
     default_kwargs = InfoMixin.default_kwargs.copy()
@@ -175,15 +175,15 @@
 
     def test_required_types_with_name(self):
         info = self.make_one(name='foo')
         self.assertEqual(['foo'], info.getrequiredtypes())
 
     def test_getsectioninfo(self):
 
-        class MockChild(object):
+        class MockChild:
             _issection = False
 
             def issection(self):
                 return self._issection
 
         child = MockChild()
 
@@ -201,15 +201,15 @@
                                info.getsectioninfo,
                                None, 'baz')
 
 
 class SchemaTypeTestCase(TestHelper, unittest.TestCase):
 
     def test_various(self):
-        class Mock(object):
+        class Mock:
             pass
 
         mock = Mock()
         schema = SchemaType(None, None, None, None, 'url', {})
 
         mock.name = 'name'
         schema.addtype(mock)
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_loader.py` & `ZConfig-4.0/src/ZConfig/tests/test_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 ##############################################################################
 """Tests of ZConfig.loader classes and helper functions."""
 
 import os.path
 import sys
 import tempfile
 import unittest
+import urllib.request
+from io import StringIO
 
 import ZConfig
 import ZConfig.loader
 import ZConfig.url
-from ZConfig._compat import NStringIO as StringIO
-from ZConfig._compat import urllib2
 from ZConfig.tests.support import CONFIG_BASE
 from ZConfig.tests.support import TestHelper
 
 
 myfile = os.path.abspath(__file__)
 LIBRARY_DIR = os.path.join(os.path.dirname(myfile), "library")
 
@@ -37,16 +37,16 @@
         # Files are decoded using utf-8 on open
         loader = ZConfig.loader.SchemaLoader()
         url = ZConfig.url.urljoin(CONFIG_BASE, "non-ascii.txt")
         with loader.openResource(url) as stream:
             val = stream.read()
         self.assertEqual(
             val,
-            u'# -*-coding: utf-8; mode: conf-*-\n'
-            u'This file contains a snowman, U+2603: \u2603\n'
+            '# -*-coding: utf-8; mode: conf-*-\n'
+            'This file contains a snowman, U+2603: \u2603\n'
         )
 
     def test_schema_caching(self):
         loader = ZConfig.loader.SchemaLoader()
         url = ZConfig.url.urljoin(CONFIG_BASE, "simple.xml")
         schema1 = loader.loadURL(url)
         schema2 = loader.loadURL(url)
@@ -73,15 +73,15 @@
         self.assertRaisesRegex(ZConfig.SchemaError,
                                "illegal schema component name",
                                loader.schemaComponentSource,
                                'foo..bar', None)
 
     def test_config_loader_abstract_schema(self):
 
-        class MockSchema(object):
+        class MockSchema:
             _abstract = True
 
             def isabstract(self):
                 return self._abstract
 
             def gettype(self, _t):
                 return self
@@ -219,39 +219,14 @@
                        "  <import package='ZConfig.tests.library.widget' />"
                        "</schema>")
         schema = loader.loadFile(sio)
         loader = ZConfig.loader.ConfigLoader(schema)
         sio = StringIO("%import ZConfig.tests.library.widget")
         loader.loadFile(sio)
 
-    def test_urlsplit_urlunsplit(self):
-        # Extracted from Python's test.test_urlparse module:
-        samples = [
-            ('http://www.python.org',
-             ('http', 'www.python.org', '', '', '', ''),
-             ('http', 'www.python.org', '', '', '')),
-            ('http://www.python.org#abc',
-             ('http', 'www.python.org', '', '', '', 'abc'),
-             ('http', 'www.python.org', '', '', 'abc')),
-            ('http://www.python.org/#abc',
-             ('http', 'www.python.org', '/', '', '', 'abc'),
-             ('http', 'www.python.org', '/', '', 'abc')),
-            ("http://a/b/c/d;p?q#f",
-             ('http', 'a', '/b/c/d', 'p', 'q', 'f'),
-             ('http', 'a', '/b/c/d;p', 'q', 'f')),
-            ('file:///tmp/junk.txt',
-             ('file', '', '/tmp/junk.txt', '', '', ''),
-             ('file', '', '/tmp/junk.txt', '', '')),
-        ]
-        for url, parsed, split in samples:
-            result = ZConfig.url.urlsplit(url)
-            self.assertEqual(result, split)
-            result2 = ZConfig.url.urlunsplit(result)
-            self.assertEqual(result2, url)
-
     def test_file_url_normalization(self):
         self.assertEqual(
             ZConfig.url.urlnormalize("file:/abc/def"),
             "file:///abc/def")
         self.assertEqual(
             ZConfig.url.urlunsplit(("file", "", "/abc/def", "", "")),
             "file:///abc/def")
@@ -259,15 +234,15 @@
             ZConfig.url.urljoin("file:/abc/", "def"),
             "file:///abc/def")
         self.assertEqual(
             ZConfig.url.urldefrag("file:/abc/def#frag"),
             ("file:///abc/def", "frag"))
 
     def test_url_from_file(self):
-        class MockFile(object):
+        class MockFile:
             name = 'path'
         self.assertEqual('file://',
                          ZConfig.loader._url_from_file(MockFile)[:7])
 
     def test_isPath(self):
         assertTrue = self.assertTrue
         isPath = ZConfig.loader.SchemaLoader().isPath
@@ -298,19 +273,19 @@
     # replace that function with one that always raises an exception.
     # Since urllib2.urlopen() can raise either IOError or OSError
     # (depending on the version of Python), we run test for each
     # exception.  urllib2.urlopen() is restored after running the
     # test.
 
     def setUp(self):
-        self.urllib2_urlopen = urllib2.urlopen
-        urllib2.urlopen = self.fake_urlopen
+        self.urllib2_urlopen = urllib.request.urlopen
+        urllib.request.urlopen = self.fake_urlopen
 
     def tearDown(self):
-        urllib2.urlopen = self.urllib2_urlopen
+        urllib.request.urlopen = self.urllib2_urlopen
 
     def fake_urlopen(self, url):
         raise self.error()
 
     def test_nonexistent_file_ioerror(self):
         self.error = IOError
         self.check_nonexistent_file()
@@ -398,15 +373,15 @@
     def setUp(self):
         sys.modules[self.magic_name] = self
 
     def tearDown(self):
         del sys.modules[self.magic_name]
 
     def test_package_loader_resource_error(self):
-        class MockLoader(object):
+        class MockLoader:
             pass
         self.__loader__ = MockLoader()
         self.__path__ = ['dir']
 
         self.assertRaisesRegex(ZConfig.SchemaResourceError,
                                "error opening schema component",
                                ZConfig.loader.openPackageResource,
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_matcher.py` & `ZConfig-4.0/src/ZConfig/tests/test_matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from ZConfig.tests.support import TestHelper
 
 
 class SectionValueTestCase(unittest.TestCase):
 
     def test_repr(self):
 
-        class MockMatcher(object):
+        class MockMatcher:
             type = None
 
         matcher = MockMatcher()
         matcher.type = MockMatcher()
         matcher.type.name = 'matcher'
 
         sv = SectionValue({}, 'name', matcher)
@@ -49,15 +49,15 @@
             str(sv))
 
 
 class SectionMatcherTestCase(TestHelper, unittest.TestCase):
 
     def test_constructor_error(self):
 
-        class Mock(object):
+        class Mock:
             name = 'name'
 
             def allowUnnamed(self):
                 return False
 
         mock = Mock()
         self.assertRaisesRegex(ConfigurationError,
@@ -87,15 +87,15 @@
         self.assertRaisesRegex(ConfigurationError,
                                "section names must not be re-used",
                                matcher.addSection,
                                None, 'foo', None)
 
     def test_construct_errors(self):
 
-        class MockType(object):
+        class MockType:
             attribute = 'attr'
 
             _multi = True
             _section = True
 
             def ismulti(self):
                 return self._multi
@@ -103,15 +103,15 @@
             def issection(self):
                 return self._section
 
         type_ = []
         matcher = BaseMatcher(None, type_, None)
         type_.append(('key', MockType()))
 
-        class MockSection(object):
+        class MockSection:
             def getSectionDefinition(self):
                 return self
 
             def datatype(self, _s):
                 raise ValueError()
 
         matcher._values['attr'] = [MockSection()]
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_pygments.py` & `ZConfig-4.0/src/ZConfig/tests/test_pygments.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 #
 ##############################################################################
 """\
 Tests for ZConfig.pygments.ZConfigLexer.
 
 """
 
-from __future__ import absolute_import
-from __future__ import print_function
 
 import unittest
 
 
 try:
     import pygments.lexer
     import pygments.token
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_readme.py` & `ZConfig-4.0/src/ZConfig/tests/test_readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         if here == prev:
             # Let's avoid infinite loops at root
             raise AssertionError('could not find my setup.py')
     return here
 
 
 def docSetUp(test):
-    # Python 2 makes __path__ and __file__ relative in some
+    # Python makes __path__ and __file__ relative in some
     # cases (such as when we're executing with the 'ZConfig'
     # directory on sys.path as CWD). This breaks finding
     # schema components when we change directories.
     import ZConfig.components.logger as logger
     logger.__file__ = os.path.abspath(logger.__file__)
     logger.__path__ = [os.path.abspath(x) for x in logger.__path__]
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_schema.py` & `ZConfig-4.0/src/ZConfig/tests/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,27 +73,27 @@
         check(not conf.false_var_2)
         check(not conf.false_var_3)
 
     def test_app_datatype(self):
         dtname = __name__ + ".uppercase"
         schema = self.load_schema_text("""\
             <schema>
-              <key name='a' datatype='%s'/>
-              <key name='b' datatype='%s' default='abc'/>
-              <multikey name='c' datatype='%s'>
+              <key name='a' datatype='{}'/>
+              <key name='b' datatype='{}' default='abc'/>
+              <multikey name='c' datatype='{}'>
                 <default>abc</default>
                 <default>abc</default>
                 </multikey>
-              <multikey name='d' datatype='%s'>
+              <multikey name='d' datatype='{}'>
                 <default>not</default>
                 <default>lower</default>
                 <default>case</default>
                 </multikey>
             </schema>
-            """ % (dtname, dtname, dtname, dtname))
+            """.format(dtname, dtname, dtname, dtname))
         conf = self.load_config_text(schema, """\
                                      a qwerty
                                      c upp
                                      c er
                                      c case
                                      """)
         eq = self.assertEqual
@@ -991,101 +991,95 @@
                           """)
 
     def test_datatype_casesensitivity(self):
         self.load_schema_text("<schema datatype='NULL'/>")
 
     def test_simple_extends(self):
         schema = self.load_schema_text("""\
-           <schema extends='%s/simple.xml %s/library.xml'>
+           <schema extends='{}/simple.xml {}/library.xml'>
              <section name='A' type='type-a' />
            </schema>
-           """ % (CONFIG_BASE, CONFIG_BASE))
+           """.format(CONFIG_BASE, CONFIG_BASE))
         self._verifySimpleConf(self.load_config(schema, "simple.conf"))
 
     def test_extends_fragment_failure(self):
         self.assertRaises(
             ZConfig.SchemaError, self.load_schema_text,
             "<schema extends='%s/library.xml#foo'/>" % CONFIG_BASE)
 
     def test_extends_description_override(self):
         schema = self.load_schema_text("""\
-           <schema extends='%s/base.xml %s/library.xml'>
+           <schema extends='{}/base.xml {}/library.xml'>
              <description>
                overriding description
              </description>
              <section name='A' type='type-a' />
              <section name='X' type='type-X' />
            </schema>
-           """ % (CONFIG_BASE, CONFIG_BASE))
+           """.format(CONFIG_BASE, CONFIG_BASE))
         description = schema.description.strip()
         self.assertEqual(description, "overriding description")
 
     def test_extends_description_first_extended_wins(self):
         schema = self.load_schema_text("""\
-           <schema extends='%s/base.xml %s/library.xml'>
+           <schema extends='{}/base.xml {}/library.xml'>
              <section name='A' type='type-a' />
              <section name='X' type='type-X' />
            </schema>
-           """ % (CONFIG_BASE, CONFIG_BASE))
+           """.format(CONFIG_BASE, CONFIG_BASE))
         description = schema.description.strip()
         self.assertEqual(description, "base description")
 
     def test_multi_extends_implicit_OK(self):
         self.load_schema_text("""\
-           <schema extends='%s/base.xml %s/library.xml'>
+           <schema extends='{}/base.xml {}/library.xml'>
              <section name='A' type='type-a' />
              <section name='X' type='type-X' />
            </schema>
-           """ % (CONFIG_BASE, CONFIG_BASE))
+           """.format(CONFIG_BASE, CONFIG_BASE))
 
     def test_multi_extends_explicit_datatype_OK(self):
         self.load_schema_text("""\
-           <schema extends='%s/base-datatype1.xml %s/base-datatype2.xml'
+           <schema extends='{}/base-datatype1.xml {}/base-datatype2.xml'
                    datatype='null'>
              <section name='One' type='type-1' />
              <section name='Two' type='type-2' />
            </schema>
-           """ % (CONFIG_BASE, CONFIG_BASE))
+           """.format(CONFIG_BASE, CONFIG_BASE))
 
     def test_multi_extends_explicit_keytype_OK(self):
         self.load_schema_text("""\
-           <schema extends='%s/base-keytype1.xml %s/base-keytype2.xml'
-                   keytype='%s.uppercase'>
+           <schema extends='{}/base-keytype1.xml {}/base-keytype2.xml'
+                   keytype='{}.uppercase'>
              <section name='One' type='type-1' />
              <section name='Two' type='type-2' />
            </schema>
-           """ % (CONFIG_BASE, CONFIG_BASE, __name__))
+           """.format(CONFIG_BASE, CONFIG_BASE, __name__))
 
     def test_multi_extends_datatype_conflict(self):
         self.assertRaises(ZConfig.SchemaError,
                           self.load_schema_text, """\
-            <schema extends='%s/base-datatype1.xml %s/base-datatype2.xml'/>
-            """ % (CONFIG_BASE, CONFIG_BASE))
+            <schema extends='{}/base-datatype1.xml {}/base-datatype2.xml'/>
+            """.format(CONFIG_BASE, CONFIG_BASE))
 
     def test_multi_extends_keytype_conflict(self):
         self.assertRaises(ZConfig.SchemaError,
                           self.load_schema_text, """\
-            <schema extends='%s/base-keytype1.xml %s/base-keytype2.xml'/>
-            """ % (CONFIG_BASE, CONFIG_BASE))
+            <schema extends='{}/base-keytype1.xml {}/base-keytype2.xml'/>
+            """.format(CONFIG_BASE, CONFIG_BASE))
 
     def test_multiple_descriptions_is_error(self):
         self.assertRaises(ZConfig.SchemaError,
                           self.load_schema_text, """\
             <schema>
               <description>  foo  </description>
               <description>  bar  </description>
             </schema>
             """)
 
-    def test_srepr(self):
-        from ZConfig.schema import _srepr
-        FOO = u'foo'
-        self.assertEqual(_srepr('foo'), "'foo'")
-        self.assertEqual(_srepr(FOO), "'foo'")
-
     def test_schema_example(self):
         schema = self.load_schema_text("""\
             <schema>
                 <example>  This is an example  </example>
             </schema>
             """)
         self.assertEqual(schema.example, 'This is an example')
@@ -1181,15 +1175,15 @@
         self.checkErrorText("<schema>text",
                             "non-blank character data")
 
     def test_error_subclass(self):
         import ZConfig.datatypes
         import ZConfig.schema
 
-        class MockLoader(object):
+        class MockLoader:
             registry = ZConfig.datatypes.Registry()
 
         parser = ZConfig.schema.SchemaParser(MockLoader(), 'url')
         parser.push_prefix({'prefix': __name__})
         parser.push_prefix({'prefix': '.' + __name__})
 
         def cv(n):
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_schema2html.py` & `ZConfig-4.0/src/ZConfig/tests/test_schema2html.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,35 +7,25 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from __future__ import absolute_import
 
 import textwrap
 import unittest
+from io import StringIO
 
 import docutils
 import docutils.frontend
 import docutils.parsers.rst
 import docutils.parsers.rst.directives
 import docutils.utils
 
-
-try:
-    # Note that we're purposely using the old
-    # StringIO object on Python 2 because it auto-converts
-    # Unicode to str, which io.BytesIO and io.StringIO don't
-    # but which normal printing to default sys.stdout *does*
-    from cStringIO import StringIO
-except ImportError:
-    from ZConfig._compat import NStringIO as StringIO
-
 from ZConfig import schema2html
 from ZConfig.sphinx import RstSchemaFormatter
 from ZConfig.sphinx import SchemaToRstDirective
 from ZConfig.tests import support
 
 
 docutils.parsers.rst.directives.register_directive("zconfig",
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_schemaless.py` & `ZConfig-4.0/src/ZConfig/tests/test_schemaless.py`

 * *Files identical despite different names*

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_subst.py` & `ZConfig-4.0/src/ZConfig/tests/test_subst.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests of the string interpolation module."""
 
-# This is needed to support Python 2.1.
-from __future__ import nested_scopes
-
 import os
 import unittest
 
 from ZConfig import SubstitutionReplacementError
 from ZConfig import SubstitutionSyntaxError
 from ZConfig.substitution import isname
 from ZConfig.substitution import substitute
```

### Comparing `ZConfig-3.6.1/src/ZConfig/tests/test_validator.py` & `ZConfig-4.0/src/ZConfig/tests/test_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from __future__ import absolute_import
 
 import unittest
+from io import StringIO
 
 from ZConfig import validator
-from ZConfig._compat import NStringIO as StringIO
 from ZConfig.tests import support
 
 
 def run_validator(*args):
     return validator.main(args)
```

### Comparing `ZConfig-3.6.1/src/ZConfig/url.py` & `ZConfig-4.0/src/ZConfig/url.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,49 +10,47 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """urlparse-like helpers that normalize file: URLs.
 
 ZConfig and urllib2 expect file: URLs to consistently use the '//'
-hostpart seperator; the functions here enforce this constraint.
+hostpart separator; the functions here enforce this constraint.
 
 """
 
-from ZConfig._compat import urlparse as _urlparse
-
-
-urlsplit = _urlparse.urlsplit
+import urllib.parse
+import urllib.request
 
 
 def urlnormalize(url):
     lc = url.lower()
     if lc.startswith("file:/") and not lc.startswith("file:///"):
         url = "file://" + url[5:]
     return url
 
 
 def urlunsplit(parts):
     parts = list(parts)
     parts.insert(3, '')
-    url = _urlparse.urlunparse(tuple(parts))
+    url = urllib.request.urlunparse(tuple(parts))
     if (parts[0] == "file"
             and url.startswith("file:/")
             and not url.startswith("file:///")):
         # It may not be possible to get here anymore with
         # modern urlparse, at least not on posix?
         url = "file://" + url[5:]  # pragma: no cover
     return url
 
 
 def urldefrag(url):
-    url, fragment = _urlparse.urldefrag(url)
+    url, fragment = urllib.parse.urldefrag(url)
     return urlnormalize(url), fragment
 
 
 def urljoin(base, relurl):
-    url = _urlparse.urljoin(base, relurl)
+    url = urllib.request.urljoin(base, relurl)
     if url.startswith("file:/") and not url.startswith("file:///"):
         # It may not be possible to get here anymore with
         # modern urlparse, at least not on posix?
         url = "file://" + url[5:]  # pragma: no cover
     return url
```

### Comparing `ZConfig-3.6.1/src/ZConfig/validator.py` & `ZConfig-4.0/src/ZConfig/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 """Script to check validity of a configuration file.
 """
 
-from __future__ import print_function
 
 import argparse
 import sys
 
 import ZConfig
```

### Comparing `ZConfig-3.6.1/tox.ini` & `ZConfig-4.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
     py311
-    pypy
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
 deps =
@@ -38,14 +34,15 @@
     check-python-versions >= 0.19.1
     wheel
     flake8
     isort
 
 [testenv:isort-apply]
 basepython = python3
+skip_install = true
 commands_pre =
 deps =
     isort
 commands =
     isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
@@ -59,24 +56,22 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
     coverage html --ignore-errors
-    coverage report --ignore-errors --show-missing --fail-under=95
+    coverage report --ignore-errors --show-missing --fail-under=98
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = ZConfig
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

