# Comparing `tmp/wllegal-2023.1.tar.gz` & `tmp/wllegal-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wllegal-2023.1.tar", last modified: Fri Mar  3 14:36:46 2023, max compression
+gzip compressed data, was "wllegal-2023.2.tar", last modified: Fri May  5 06:56:38 2023, max compression
```

## Comparing `wllegal-2023.1.tar` & `wllegal-2023.2.tar`

### file list

```diff
@@ -1,364 +1,364 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-03 14:36:28.000000 wllegal-2023.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-03 14:36:28.000000 wllegal-2023.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-03-03 14:36:46.051635 wllegal-2023.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-03 14:36:28.000000 wllegal-2023.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-03 14:36:28.000000 wllegal-2023.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-03 14:36:28.000000 wllegal-2023.1/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-03 14:36:28.000000 wllegal-2023.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-03-03 14:36:46.055635 wllegal-2023.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2152 2023-03-03 14:36:28.000000 wllegal-2023.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.023635 wllegal-2023.1/wllegal/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.023635 wllegal-2023.1/wllegal/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/ab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.023635 wllegal-2023.1/wllegal/locale/ab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/afh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.023635 wllegal-2023.1/wllegal/locale/afh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/afh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/ang/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.023635 wllegal-2023.1/wllegal/locale/ang/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ang/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.023635 wllegal-2023.1/wllegal/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    30571 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/ar_LY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.023635 wllegal-2023.1/wllegal/locale/ar_LY/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19839 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ar_LY/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/ars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.023635 wllegal-2023.1/wllegal/locale/ars/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ars/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/ast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/ast/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21100 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ast/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/az/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/az/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    23995 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/az/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/be/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/be/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    49097 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/be/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/be@latin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/be@latin/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    24165 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/be@latin/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/ber/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/ber/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20082 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ber/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.995635 wllegal-2023.1/wllegal/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/bn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20035 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/bn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/bn_BD/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/bn_BD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19883 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/bn_BD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/bo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/bo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/bo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/br/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/br/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21706 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/br/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    40384 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/ce/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/ce/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ce/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/ckb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/ckb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39177 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ckb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/crh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.027635 wllegal-2023.1/wllegal/locale/crh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/crh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39464 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/cv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/cv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/cv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/cy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/cy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/dv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/dv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/dv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    27741 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/en_GB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/en_GB/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/en_GB/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/enm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/enm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/enm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/eo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:45.999635 wllegal-2023.1/wllegal/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    40427 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    23250 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21750 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20673 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/fil/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/fil/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/fil/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.031635 wllegal-2023.1/wllegal/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    41734 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/fur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/fur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/fur/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/fy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/fy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/fy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39757 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    41481 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20168 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/hi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    38256 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    29280 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/hy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/ia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/ia/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ia/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    38613 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/ie/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/ie/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ie/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.003635 wllegal-2023.1/wllegal/locale/is/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/is/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39821 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.035635 wllegal-2023.1/wllegal/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    40600 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20076 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ka/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/kab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/kab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    27980 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/kab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/kk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/kk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    45839 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/kk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/km/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/km/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/km/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/kmr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/kmr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/kmr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39992 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/ksh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/ksh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ksh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/ln/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/ln/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20625 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ln/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    25725 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/lzh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/lzh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/lzh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/mk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/mk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/mk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/ml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20014 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ml/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/mr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/mr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/ms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ms/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/my/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/my/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/my/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.007635 wllegal-2023.1/wllegal/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    38799 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.039635 wllegal-2023.1/wllegal/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    40487 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/oc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/oc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19880 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/oc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/or/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/or/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/or/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/pa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/pa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20490 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/pa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/pa_PK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/pa_PK/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20075 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/pa_PK/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/peo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/peo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/peo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    40075 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/ps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/ps/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ps/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    40478 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39738 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    32480 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    34204 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/ro_MD/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/ro_MD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ro_MD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    51485 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/sc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/sc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19881 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/sc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.011635 wllegal-2023.1/wllegal/locale/si/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.043635 wllegal-2023.1/wllegal/locale/si/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    36711 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/skr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/skr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/skr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    22592 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    40694 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    24408 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    22694 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/sr_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/ta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ta/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/te/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/te/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20718 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/tlh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/tlh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20146 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/tlh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/tok/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/tok/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/tok/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39725 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.015635 wllegal-2023.1/wllegal/locale/tt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/tt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/tt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.019635 wllegal-2023.1/wllegal/locale/tzm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.047635 wllegal-2023.1/wllegal/locale/tzm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20075 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/tzm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.019635 wllegal-2023.1/wllegal/locale/ug/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/locale/ug/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/ug/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.019635 wllegal-2023.1/wllegal/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    49609 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.019635 wllegal-2023.1/wllegal/locale/uz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/locale/uz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/uz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.019635 wllegal-2023.1/wllegal/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.019635 wllegal-2023.1/wllegal/locale/yue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/locale/yue/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19977 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/yue/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.019635 wllegal-2023.1/wllegal/locale/zgh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/locale/zgh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/zgh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.019635 wllegal-2023.1/wllegal/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    36131 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.019635 wllegal-2023.1/wllegal/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    35749 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/settings_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.019635 wllegal-2023.1/wllegal/templates/legal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/templates/legal/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/templates/legal/documents/contracts.html
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/templates/legal/documents/privacy.html
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/templates/legal/documents/summary.html
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/templates/legal/documents/tos.html
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/templates/security.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/templates/weblate_503.html
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/templates/weblate_50x.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.051635 wllegal-2023.1/wllegal/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/templatetags/lawlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-03 14:36:28.000000 wllegal-2023.1/wllegal/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:36:46.023635 wllegal-2023.1/wllegal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-03-03 14:36:45.000000 wllegal-2023.1/wllegal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-03-03 14:36:45.000000 wllegal-2023.1/wllegal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 14:36:45.000000 wllegal-2023.1/wllegal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-03 14:36:45.000000 wllegal-2023.1/wllegal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-03 14:36:45.000000 wllegal-2023.1/wllegal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.603996 wllegal-2023.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-05 06:56:23.000000 wllegal-2023.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-05 06:56:23.000000 wllegal-2023.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-05 06:56:38.603996 wllegal-2023.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-05 06:56:23.000000 wllegal-2023.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-05 06:56:23.000000 wllegal-2023.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 06:56:23.000000 wllegal-2023.2/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:56:23.000000 wllegal-2023.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-05 06:56:38.603996 wllegal-2023.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-05-05 06:56:23.000000 wllegal-2023.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/ab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/locale/ab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/afh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/locale/afh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/afh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/ang/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/locale/ang/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ang/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    41125 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/ar_LY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/locale/ar_LY/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19839 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ar_LY/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/ars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/locale/ars/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ars/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/ast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/locale/ast/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21100 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ast/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/az/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/locale/az/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    23995 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/az/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/be/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/be/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    49097 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/be/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/be_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/be_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    24165 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/be_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/ber/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/ber/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20082 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ber/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/bn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20035 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/bn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/bn_BD/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/bn_BD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19883 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/bn_BD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/bo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/bo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/bo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/br/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/br/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21706 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/br/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.567995 wllegal-2023.2/wllegal/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    40384 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/ce/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/ce/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ce/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/ckb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/ckb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39177 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ckb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/crh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/crh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/crh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39436 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/cv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/cv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/cv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/cy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21140 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/cy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/dv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/dv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/dv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    27741 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/en_GB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/en_GB/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    32465 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/en_GB/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/enm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/enm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/enm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/eo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    40427 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    23107 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21750 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.587996 wllegal-2023.2/wllegal/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20673 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/fil/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/fil/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/fil/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    41707 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/fur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/fur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/fur/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/fy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/fy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/fy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39757 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    41481 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20168 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/hi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    38256 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    29280 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/hy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.571995 wllegal-2023.2/wllegal/locale/ia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/ia/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ia/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    38613 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/ie/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/ie/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ie/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/is/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/is/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39821 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    40600 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20076 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ka/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/kab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/kab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    27980 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/kab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/kk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/kk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    45839 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/kk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/km/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/km/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/km/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/kmr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/kmr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/kmr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39964 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/ksh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/ksh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ksh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/ln/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/ln/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20625 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ln/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.591996 wllegal-2023.2/wllegal/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    25725 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/lzh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/lzh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/lzh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/mk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/mk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/mk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/ml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20014 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ml/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/mr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/mr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/ms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ms/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/my/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/my/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/my/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    38799 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    40487 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/oc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/oc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19880 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/oc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/or/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/or/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/or/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/pa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/pa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20490 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/pa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/pa_PK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/pa_PK/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20075 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/pa_PK/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/peo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/peo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/peo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    40075 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/ps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/ps/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ps/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.575996 wllegal-2023.2/wllegal/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    40478 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39738 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    32480 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    34204 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/ro_MD/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/ro_MD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ro_MD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    51485 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/sc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/sc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19881 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/sc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/si/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/si/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    36711 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/skr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.595996 wllegal-2023.2/wllegal/locale/skr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/skr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    22592 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    40694 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    24408 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    22694 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/sr_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/ta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ta/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/te/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/te/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20718 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/tlh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/tlh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20146 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/tlh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/tok/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/tok/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/tok/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39725 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/tt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/tt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/tt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/tzm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/tzm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20075 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/tzm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/ug/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/ug/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/ug/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    49609 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/uz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/uz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/uz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/yue_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/yue_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19977 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/yue_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/zgh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/zgh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20269 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/zgh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    36131 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.579995 wllegal-2023.2/wllegal/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    35749 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/settings_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.599996 wllegal-2023.2/wllegal/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal/templates/legal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.603996 wllegal-2023.2/wllegal/templates/legal/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/templates/legal/documents/contracts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/templates/legal/documents/privacy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/templates/legal/documents/summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/templates/legal/documents/tos.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/templates/security.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/templates/weblate_503.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/templates/weblate_50x.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.603996 wllegal-2023.2/wllegal/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/templatetags/lawlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-05 06:56:23.000000 wllegal-2023.2/wllegal/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:38.583995 wllegal-2023.2/wllegal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-05 06:56:38.000000 wllegal-2023.2/wllegal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-05 06:56:38.000000 wllegal-2023.2/wllegal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:56:38.000000 wllegal-2023.2/wllegal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:56:38.000000 wllegal-2023.2/wllegal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 06:56:38.000000 wllegal-2023.2/wllegal.egg-info/top_level.txt
```

### Comparing `wllegal-2023.1/LICENSE` & `wllegal-2023.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/PKG-INFO` & `wllegal-2023.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wllegal
-Version: 2023.1
+Version: 2023.2
 Summary: Hosted Weblate legal stuff
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/wllegal
 Author: Michal Čihař
 Author-email: michal@cihar.com
 License: GPL-3.0-or-later
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/wllegal/issues
@@ -26,24 +26,24 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
    :alt: Weblate
    :target: https://weblate.org/
    :height: 80px
 
-**Weblate is a copylefted libre software web-based continuous localization system,
+**Weblate is libre software web-based continuous localization system,
 used by over 2500 libre projects and companies in more than 165 countries.**
 
 
 This is legal module used on the `Hosted Weblate service
 <https://weblate.org/hosting/>`_.
 
 You can use them as an example how to customize `Weblate
```

### Comparing `wllegal-2023.1/README.rst` & `wllegal-2023.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
    :alt: Weblate
    :target: https://weblate.org/
    :height: 80px
 
-**Weblate is a copylefted libre software web-based continuous localization system,
+**Weblate is libre software web-based continuous localization system,
 used by over 2500 libre projects and companies in more than 165 countries.**
 
 
 This is legal module used on the `Hosted Weblate service
 <https://weblate.org/hosting/>`_.
 
 You can use them as an example how to customize `Weblate
```

### Comparing `wllegal-2023.1/setup.cfg` & `wllegal-2023.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wllegal
-version = 2023.1
+version = 2023.2
 description = Hosted Weblate legal stuff
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://weblate.org/
 author = Michal Čihař
 author_email = michal@cihar.com
 license = GPL-3.0-or-later
@@ -34,15 +34,15 @@
 	Issue Tracker=https://github.com/WeblateOrg/wllegal/issues
 	Documentation=https://docs.weblate.org/
 	Source Code=https://github.com/WeblateOrg/wllegal
 	Twitter=https://twitter.com/WeblateOrg
 
 [options]
 packages = wllegal
-python_requires = >=3.6
+python_requires = >=3.9
 include_package_data = 1
 package_dir = wllegal=wllegal
 
 [flake8]
 max-complexity = 16
 extend-select = E,W1,W2,W3,W504,W505,W6
 enable-extensions = B,C,D,DJ,F,G,I,M,N,R,SF
@@ -51,20 +51,11 @@
 max-line-length = 88
 
 [pycodestyle]
 extend-select = E,W1,W2,W3,W504,W505,W6
 exclude = migrations,settings.py,settings_test.py,.git,data,data-test,settings_test_nose.py,docs,.venv,build,node_modules
 max-line-length = 88
 
-[isort]
-multi_line_output = 3
-include_trailing_comma = True
-force_grid_wrap = 0
-use_parentheses = True
-line_length = 88
-known_first_party = wllegal
-known_third_party = weblate,django,translate
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wllegal-2023.1/wllegal/locale/ab/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ab/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/afh/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/afh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ang/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ang/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ar/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/lv/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,476 +1,512 @@
-# Arabic translations for PACKAGE package.
-# Copyright (C) 2014 THE PACKAGE'S COPYRIGHT HOLDER
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Automatically generated, 2014.
-# ButterflyOfFire <ButterflyOfFire@protonmail.com>, 2018, 2019, 2020.
-# mohammadA <mohammadAbdulhadi1@gmail.com>, 2018, 2019.
-# Omar Aglan <omar.aglan91@yahoo.com>, 2019.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2021-01-28 08:54+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Arabic <https://hosted.weblate.org/projects/weblate/legal/ar/"
+"PO-Revision-Date: 2022-11-07 19:02+0000\n"
+"Last-Translator: Coool (github.com/Coool) <coool@mail.lv>\n"
+"Language-Team: Latvian <https://hosted.weblate.org/projects/weblate/legal/lv/"
 ">\n"
-"Language: ar\n"
+"Language: lv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
-"&& n%100<=10 ? 3 : n%100>=11 ? 4 : 5;\n"
-"X-Generator: Weblate 4.5-dev\n"
+"Plural-Forms: nplurals=3; plural=(n % 10 == 0 || n % 100 >= 11 && n % 100 <= "
+"19) ? 0 : ((n % 10 == 1 && n % 100 != 11) ? 1 : 2);\n"
+"X-Generator: Weblate 4.14.2\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr ""
+msgstr "Apakšuzņēmēji saskaņā ar GDPR 28. pantu"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
-msgstr ""
+msgstr "2020. gada oktobra statuss."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
+"Mēs ievērojam regulu Nr. %(law_679_2016)s, Vispārīgo datu aizsardzības "
+"regulu, kas pazīstama arī kā GDPR. Šis dokuments iekļauj nepieciešamās "
+"specifikācijas."
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr "التحكم في البيانات الشخصية"
+msgstr "Personas datu pārvaldnieks"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s، رقم التسجيل %(reg_no)s"
+msgstr "%(provider)s, Reģ. Nr. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
-"لقد قامت Weblate بتعيين ضابط حماية للبيانات ويمكنم الاتصال به عن طريق "
+"Weblate ir datu aizsardzības speciālists, ar kuru var sazināties, izmantojot "
 "%(privacy_contact)s."
 
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
-msgstr "البيانات الشخصية التي تقوم بمعالجتها ويب لايت"
+msgstr "Personas dati, ko apstrādā Weblate"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
-"لا تقوم ويب لايت بمعالجة إلا البيانات الشخصية التي يقدمها المستخدم فقط وذلك "
-"عند استعمال المنصة:"
+"Weblate vietne apstrādā tikai tos Personas datus, ko Lietotājs pats "
+"iesniedzis, izmantojot mūsu pakalpojumu:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
-#, fuzzy
-#| msgid "Name and e-mail"
 msgid "Name and e-mail address"
-msgstr "الإسم و البريد الإلكتروني"
+msgstr "Vārds un e-pasta adrese"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits"
 msgstr ""
+"Tie tiek izmantoti, lai identificētu jūs VCS iesniegtajās izmaiņās (commits)"
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events"
 msgstr ""
+"Turklāt e-pasts tiek izmantots, lai nosūtītu notikumu paziņojumus, kuriem "
+"jūs sekojiet"
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr "كلمة المرور في شكل مجزأ"
+msgstr "Parole šifrētā (hashed) formā"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
-msgstr "يُستخدم لمصادقة المستخدم إن تم إعداده"
+msgstr "Ja tas ir konfigurēts, izmanto, lai autorizētu lietotāju"
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
-msgstr ""
+msgstr "Paroles tiek saglabātas šifrētas, izmantojot Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr "اسم المتصفح وعنوان IP"
+msgstr "IP adrese un pārlūkprogrammas nosaukums"
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen"
 msgstr ""
-"ستُسجل هذه في حال وجود تغييرات مهمة في حسابك (مثل تغيير كلمة السر) لكي يسمح "
-"بتشخيص حالات سرقة الحساب"
+"Tie tiek reģistrēti, ja tiek veiktas svarīgas izmaiņas jūsu kontā (piemēram, "
+"paroles maiņa), lai varētu veikt diagnostiku konta nozagšanas gadījumā"
 
 #: wllegal/templates/legal/documents/privacy.html:36
 msgid "Billing information"
-msgstr "معلومات الفوترة"
+msgstr "Rēķinu informācija"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "In case you purchase service from us, we collect additional billing "
 "information necessary for issuing an invoice"
 msgstr ""
-"في حالة إذا ما قمتم بشراء خدمة منا ، نقوم بجمع معلومات إضافية لازمة للفوترة "
-"قصد إصدار فاتورة"
+"Ja iegādājaties pakalpojumu no mums, mēs ievācam papildus informāciju, kas "
+"nepieciešama rēķina izrakstīšanai"
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
-msgstr "الغرض والأساس القانوني لمعالجة البيانات الشخصية"
+msgstr "Personas datu apstrādes mērķis un juridiskais pamats"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr "سيتم استخدام بياناتك الشخصية لأغراض الخدمة:"
+msgstr "Jūsu personas dati tiks izmantoti pakalpojuma vajadzībām:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
 "contractual or pre-contractual obligations (<a href=\"%(url)s\">Article 6 "
 "(1) b. GDPR</a>)"
 msgstr ""
+"nodrošināt mūsu pakalpojumus, kas saistīti ar pakalpojumu, un sazināties ar "
+"jums jautājumos par mūsu pakalpojumiem (tostarp izmantojot e-pastu un "
+"ziņojumapmaiņu) un būt pārliecinātiem par mūsu pakalpojumu tehnisko "
+"funkcionalitāti, pildot līgumsaistības vai pirmslīguma saistības (<a href=\""
+"%(url)s\">VDAR(GDPR) 6. panta 1. punkta b) apakšpunkts</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:48
 #, python-format
 msgid ""
 "to analyze your use of our services and improve our services (<a href="
 "\"%(url)s\">Article 6 (1) b. and f. GDPR</a>)"
 msgstr ""
+"lai analizētu mūsu pakalpojumu izmantošanu un uzlabotu mūsu pakalpojumus (<a "
+"href=\"%(url)s\">VDAR(GDPR) 6. panta 1. punkta b) un f) apakšpunkts</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:49
 #, python-format
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
+"ar jūsu nepārprotamu piekrišanu vai norādījumiem, lai veiktu mūsu "
+"uzņēmējdarbību vai nosūtītu jums informatīvos izdevumus (<a href=\"%(url)s\""
+">VDAR(GDPR) 6. panta 1. punkts a.</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
-msgstr "الوصول إلى البيانات الشخصية"
+msgstr "Piekļuve personas datiem"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
+"Pārvaldnieks ir veicis visus saprātīgos tehniskos pasākumus personas datu "
+"aizsardzībai. Personas datiem var piekļūt tikai pilnvarotas personas."
 
 #: wllegal/templates/legal/documents/privacy.html:56
 msgid ""
 "Third parties which can gain access to the Personal Data when necessary are:"
-msgstr "الأطراف الثالثة التي يمكن أن تنفذ إلى البيانات الشحصية عند الضرورة هي:"
+msgstr "Trešās personas, kuras vajadzības gadījumā var piekļūt personas datiem:"
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
-msgstr "الأشخاص المتعاقَد معهم للحصول على الضمان التقني للخدمة."
+msgstr "Personas, ar kurām noslēgts līgums par pakalpojuma tehnisko drošību."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors."
-msgstr ""
+msgstr "Maksājumu apstrādātāji."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
-msgstr "كل البيانات الشخصية مخزنة في الاتحاد الأوروبي."
+msgstr "Visi personas dati tiek glabāti Eiropas Savienībā."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 msgid "The Personal Data retention"
-msgstr "الاحتفاظ بالبيانات الشخصية"
+msgstr "Tiesības uz personas datu glabāšanu"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
-msgstr "تخزن البيانات الشخصية في الخدمة إلى أن يحذف المستخدم حسابه في الخدمة."
+msgstr ""
+"Personas datus pakalpojums uzglabā līdz brīdim, kad lietotājs izdzēš savu "
+"kontu."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "Access log information might be collected for a longer period for the "
 "purpose of establishing, exercising or defending legal claims."
 msgstr ""
+"Piekļuves žurnāla informācija var tikt vākta ilgāku laika periodu, lai "
+"celtu, izskatītu vai aizstāvētu juridiskās prasības tiesvedībā."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "Your rights"
-msgstr "حقوقك"
+msgstr "Jūsu tiesības"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
-"يقوم المستخدم بتقديم البيانات الشخصية طوعا. دون هذه البيانات يتعذر على ويب "
-"لايت تقديم خدماتنا."
+"Lietotājs savus personas datu sniedz brīvprātīgi. Weblate nevar sniegt "
+"pakalpojumus bez šiem personas datiem."
 
 #: wllegal/templates/legal/documents/privacy.html:75
 msgid ""
 "We want you to always be in control of your Personal Data. To this end, you "
 "have certain rights that allow for it. Under certain conditions, you may:"
 msgstr ""
-"نريد أن تكون السيطرة على بياناتكم الشخصية دائما بين أيديكم . وتحقيقا لهذه "
-"الغاية ، لديكم بعض الحقوق التي تتيح لكم ذلك. ففي ظل ظروف معينه ، يمكنكم:"
+"Mēs vēlamies, lai jūs vienmēr varētu kontrolēt savu personisko informāciju. "
+"Šajā nolūkā jums ir atbilstošas tiesības, kas to atļauj. Noteiktos apstākļos "
+"jūs varat:"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 #, python-format
 msgid ""
 "Gain access to all your Personal Data that Weblate uses or processes, and "
 "even get a copy of all of it (<a href=\"%(url)s\">Article 15 GDPR</a>)"
 msgstr ""
+"Iegūt piekļuvi visiem saviem personas datiem, kurus Weblate izmanto vai "
+"apstrādā, kā arī iegūt to pilno kopiju (<a href=\"%(url)s\">VDAR(GDPR) 15. "
+"pants</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:80
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
 msgstr ""
-"تصحيح البيانات الشخصية التي يعالجها ويب لايت إن كنت تظن أنها تحتوي على أخطاء"
+"Labot personas datus, kurus Weblate apstrādā, ja domājat, ka tie satur kļūdas"
 
 #: wllegal/templates/legal/documents/privacy.html:81
 msgid "Order us to delete your Personal Data"
-msgstr "طلب حذف بياناتك الشخصية منا"
+msgstr "Pieprasīt mūs dzēst jūsu personas datus"
 
 #: wllegal/templates/legal/documents/privacy.html:82
 msgid "Restrict the Personal Data processing"
-msgstr "تقييد معالجة البيانات الشخصية"
+msgstr "Ierobežot personas datu apstrādi"
 
 #: wllegal/templates/legal/documents/privacy.html:83
 msgid "Object to processing"
-msgstr "الاعتراض على المعالجة"
+msgstr "Iebilst pret apstrādi"
 
 #: wllegal/templates/legal/documents/privacy.html:84
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
-"الحصول على بياناتك الشخصية في تنسيق شائع ومقروء آليا ، أو لنقل هذه البيانات "
-"الشخصية إلى موفر آخر."
+"Iegūt savus personas datus parastā un mašīnlasāmā formātā vai pārsūtīt šos "
+"personas datus citam pakalpojuma sniedzējam."
 
 #: wllegal/templates/legal/documents/privacy.html:87
 msgid ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
+"Jūsu personas datu dzēšanu, labošanu vai ieguvi var veikt no kontu "
+"pārvaldības, un tā ir pilnībā automatizēta."
 
 #: wllegal/templates/legal/documents/summary.html:4
 msgid ""
 "The services are provided “as is”, at your own risk, without any warranty."
 msgstr ""
-"الخدمة مقدمة \"كما هي\"، لكي تستخدمها على مسئوليتك الخاصة، من غير أي ضمانات."
+"Pakalpojumi tiek sniegti “tādi, kādi tie ir”, uz jūsu risku un atbildības, "
+"bez jebkādas garantijas."
 
 #: wllegal/templates/legal/documents/summary.html:5
 msgid ""
 "Additional guarantees might apply to commercial customers, those are "
 "expressed in corresponding contracts."
 msgstr ""
-"ربما تُطبق ضمانات إضافية على المستخدمين التجارين، وهي مُوضحة في العقد الموضح."
+"Papildu garantijas var būt spēkā maksas (komerciāliem) klientiem, tās ir "
+"aprakstītas attiecīgajos līgumos."
 
 #: wllegal/templates/legal/documents/summary.html:6
 msgid ""
 "We process private data (such as your e-mail address), those will be "
 "discarded from our database as soon as you remove your account."
 msgstr ""
-"نحن نتعامل مع المعلومات الخاصة (مثل عنوان بريدك الإلكتروني)، وهي ستُخلى من "
-"قاعدة بياناتنا حينما تحذف حسابك."
+"Mēs apstrādājam privātos datus (piemēram, jūsu e-pasta adresi), tie tiks "
+"izdzēsti no mūsu datu bāzes, tiklīdz izdzēsīsit savu kontu."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your translations are made under license which is specified by each "
 "translation."
-msgstr "تُنشأ ترجماتك تحت ترخيص يحدد في كل مشروع."
+msgstr ""
+"Jūsu veiktie tulkojumi tiek izdoti saskaņā ar licenci, kas norādīta katram "
+"tulkošanas projektam."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
-msgstr "يُستخدم اسمك و بريدك الإلكتروني في تطبيقات VCS، وسيبقى هناك للتعريف."
+msgstr ""
+"Jūsu vārds un e-pasta adrese tiks izmantota versiju kontroles (VCS) "
+"iesniegtajās izmaiņās (commits), un tie paliek tur uz visiem laikiem."
 
 #: wllegal/templates/legal/documents/summary.html:9
 msgid "We use cookies to deliver our services."
-msgstr "نحن نستخدم ملفات تعريف الارتباط لتقديم خدماتنا."
+msgstr "Mēs izmantojam sīkfailus, lai nodrošinātu mūsu pakalpojumus."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
-msgstr "عرض النسخة الإنجليزية"
+msgstr "Skatīt angļu valodas versiju"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
-msgstr "وثيقة شروط الخدمة موثوقة باللغة الانجليزية. تم توفير الترجمات لراحتك."
+msgstr ""
+"Pakalpojuma oficiālie lietošanas noteikumi ir dokumentēti angļu valodā, jūsu "
+"ērtībai tiek sniegti tulkojumi."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
+"Šie pakalpojuma noteikumi regulē lietotāja un pakalpojuma sniedzēja tiesības "
+"un pienākumus, kas rodas pakalpojuma izmantošanas rezultātā."
 
 #: wllegal/templates/legal/documents/tos.html:20
 msgid "Definitions"
-msgstr "التعاريف"
+msgstr "Definīcijas"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
-msgstr "في شروط الخدمة هذه:"
+msgstr "Šajos pakalpojumu sniegšanas noteikumos:"
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
-msgstr "الاتفاق"
+msgstr "Līgums"
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
+"licences līgums (tādā nozīmē, kādā to interpretē ar Civilkodeksa 2358. pantu)"
+", kas noslēgts starp lietotāju un pakalpojuma sniedzēju ar viņu piekrišanu"
 
 #: wllegal/templates/legal/documents/tos.html:29
 msgid "Civil Code"
-msgstr "القانون المدني"
+msgstr "Civilkodekss"
 
 #: wllegal/templates/legal/documents/tos.html:30
 #, python-format
 msgid "means Act No. %(law_89_2012)s Coll., the Civil Code, as amended"
-msgstr ""
+msgstr "likums Nr. %(law_89_2012)s Coll., Čehijas Civilkodekss ar grozījumiem"
 
 #: wllegal/templates/legal/documents/tos.html:32
 msgid "Consent"
-msgstr "الرضى"
+msgstr "Vienošanās"
 
 #: wllegal/templates/legal/documents/tos.html:33
 msgid ""
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
-"يعني موافقة المستخدم على شروط الخدمة هذه والمستندات القانونية الأخرى التي "
-"يتم التعبير عنها من خلال النقر على خانة الاختيار أثناء التسجيل"
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "ملفات تعريف الإرتباط"
+msgstr "Sīkdatnes"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr ""
+msgstr "VDAR(GDPR)"
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr "الرخصة"
+msgstr "Licence"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
-msgstr "يعني الترخيص غير الحصري الممنوح من قبل الموفر للمستخدم لاستخدام الخدمة"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr "المُزَوّد"
+msgstr "Pakalpojumu sniedzējs"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
-msgstr ""
+msgstr "%(provider)s ar reģ. Nr. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "البيانات الشخصية"
+msgstr "Personas dati, Personiskie dati"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr "المالك"
+msgstr "Īpašnieks"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
-msgstr "يعني المستخدم الذي يمكنه إدارة مشروع"
+msgstr "lietotājs, kurš var pārvaldīt projektu"
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "المشروع"
+msgstr "Projekts"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
-msgstr "يُعنى بذلك مشروع الترجمة المُدار بفضل الخدمة"
+msgstr "tulkošanas projekts, kas tiek realizēts, izmantojot Pakalpojumu"
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "الخدمة"
+msgstr "Pakalpojums"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
-"يُعنى بذلك موقع الويب والخدمات القائمة على أساس Weblate والتي يديرها المزوّد"
+"uz Weblate balstīta tīmekļa vietne un pakalpojumi, ko nodrošina Pakalpojumu "
+"sniedzējs"
 
 #: wllegal/templates/legal/documents/tos.html:60
 msgid "Translation Memory"
-msgstr "ذاكرة الترجمة"
+msgstr "Tulkojumu atmiņa"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
-msgstr "يُعنى بذلك خدمة ذاكرة الترجمة الاختيارية المقدمة ضمن Weblate"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "المستخدم"
+msgstr "Lietotājs"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
-msgstr "يعني أي كيان قانوني أو فرد آَخر مِن غير مزوّد الخدمة والذي يستعمل الخدمة"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "نظام تحكم بالمراجعات"
+msgstr "Versiju kontroles sistēma (VCS)"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
+"projektā izmantotā versiju kontroles sistēma, piemēram, Git vai Mercurial"
 
 #: wllegal/templates/legal/documents/tos.html:71
 msgid "License Agreement Conclusion"
-msgstr "إبرام اتفاقية الترخيص"
+msgstr "Licences līguma noslēgšana"
 
 #: wllegal/templates/legal/documents/tos.html:73
 msgid ""
 "The License Agreement is concluded upon the User’s Acceptance of the "
 "Provider’s Offer."
-msgstr "يتم إبرام اتفاقية الترخيص بناءً على قبول المستخدم لعرض المزوّد."
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:76
 msgid "License Agreement"
-msgstr "اتفاقية الترخيص"
+msgstr "Licences līgums"
 
 #: wllegal/templates/legal/documents/tos.html:78
 msgid ""
 "By concluding Agreement under Article 2.1 of this Agreement, the following "
 "provisions of this Article 3 of the Terms of Service come into force."
 msgstr ""
 
@@ -504,15 +540,15 @@
 msgid ""
 "The User agrees to refrain from bypassing the Service’s software and/or "
 "technical hardware means, in particular the security systems."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:91
 msgid "Liability for Damage"
-msgstr "المسؤولية عن الأضرار"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:93
 msgid ""
 "The User hereby renders it undisputed that the Provider shall not be liable "
 "for any damage caused to the User resulting from the use of the Service."
 msgstr ""
 
@@ -587,15 +623,15 @@
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr "الترجمات"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -613,16 +649,14 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:126
 msgid ""
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
-"يوافق المستخدم على إثر مساهمته في أي مشروع كان ، على الرخصة الذي حددها ذات "
-"المشروع."
 
 #: wllegal/templates/legal/documents/tos.html:128
 msgid ""
 "The User agrees to use of own name and e-mail as authorship in the VCS "
 "commits. The User understands that this grant is non revocable due to nature "
 "of the VCS."
 msgstr ""
@@ -637,187 +671,31 @@
 
 #: wllegal/templates/legal/documents/tos.html:135
 msgid "The Service uses Cookies to personalise content."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:138
 msgid "Governing Law"
-msgstr "القانون الحاكم"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:140
 msgid ""
 "These Terms of Service shall be governed by the laws of the Czech Republic "
 "with exclusion of conflict rules."
 msgstr ""
-"تخضع شروط الخدمة هذه لقوانين الجمهورية التشيكية باستثناء القواعد المخالفة."
 
 #: wllegal/templates/legal/documents/tos.html:142
 msgid ""
 "Any disputes arising on the basis of the Agreement and/or these Terms of "
 "Service shall be resolved by the court of the Czech republic having "
 "substantive and local jurisdiction."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:145
 msgid "Effect"
-msgstr "التأثير"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:147
 msgid ""
 "These Terms of Service shall come into force and effect on 1st September "
 "2017."
 msgstr ""
-
-#~ msgid "Reset all changes in the local repository"
-#~ msgstr "إعادة تعيين كل التغييرات في المستودع المحلي"
-
-#~ msgid "Billing"
-#~ msgstr "الفَوترة"
-
-#~ msgid "Choose the billing plan you want to update"
-#~ msgstr "اختر خطة الفوترة التي تريد تحديثها"
-
-#~ msgid "Create new billing plan"
-#~ msgstr "إنشاء خطة فوترة جديدة"
-
-#~ msgid "Create billing plan"
-#~ msgstr "إنشاء خطة الفوترة"
-
-#~ msgid "New billing plan"
-#~ msgstr "خطة فوترة جديدة"
-
-#~ msgid "Please choose a hosting plan that fits the size of your project."
-#~ msgstr "الرجاء اختيار خطة الاستضافة التي تناسب حجم مشروعك."
-
-#~ msgid "Current billing status"
-#~ msgstr "حالة الفوترة الحالية"
-
-#~ msgid "Too small for your project."
-#~ msgstr "صغير جدا بالنسبة لمشروعكم."
-
-#~ msgid "Too small"
-#~ msgstr "صغير جدا"
-
-#~ msgid "Selected plan"
-#~ msgstr "الخطة المختارة"
-
-#~ msgid "Current plan"
-#~ msgstr "الخطة الحالية"
-
-#~ msgid "Strings limit"
-#~ msgstr "حد السلاسل"
-
-#~ msgid "Unlimited"
-#~ msgstr "غير محدود"
-
-#~ msgid "Languages limit"
-#~ msgstr "حد اللغات"
-
-#~ msgid "Component limit"
-#~ msgstr "حد المُكوّن"
-
-#~ msgid "Projects limit"
-#~ msgstr "حد المشاريع"
-
-#~ msgid "%(price)s EUR / month"
-#~ msgstr "%(price)s يورو / شهر"
-
-#~ msgid "%(price)s EUR including VAT"
-#~ msgstr "%(price)s يورو بما في ذلك ضريبة القيمة المضافة"
-
-#~ msgid "%(price)s EUR / year"
-#~ msgstr "%(price)s يورو / سنة"
-
-#~ msgid ""
-#~ "Pricing is based on the number of source strings and target languages. "
-#~ "The source string is a text unit defined in a translation format, it can "
-#~ "be a word, sentence or paragraph."
-#~ msgstr ""
-#~ "يعتمد التسعير على عدد كلمات المصدر واللغات المستهدفة. كلمات المصدر هي "
-#~ "وحدة كتابية محددة في صيغة الترجمة، يمكن أن تكون كلمة أو جملة أو فقرة."
-
-#~ msgid "All listed prices exclude VAT."
-#~ msgstr "جميع الأسعار المدرجة لا تشمل ضريبة القيمة المضافة."
-
-#~ msgid ""
-#~ "EU end users and Czech companies will be charged with additional 21%% VAT."
-#~ msgstr ""
-#~ "سيتم فرض رسوم إضافية على ضريبة القيمة المضافة بنسبة 21%% على المستخدمين "
-#~ "النهائيين في الاتحاد الأوروبي والشركات التشيكية."
-
-#~ msgid ""
-#~ "The reverse charge applies to invoices issued to businesses within the EU."
-#~ msgstr ""
-#~ "ينطبق الرسم العكسي على الفواتير الصادرة للشركات داخل الاتحاد الأوروبي."
-
-#~ msgid "No matching payment found."
-#~ msgstr "لم أجد دفعا مطابقا."
-
-#~ msgid "Thank you for purchasing a hosting plan, it is now active."
-#~ msgstr "شكرا لكم على شراء خطة الاستضافة، هي الآن نشطة."
-
-#~ msgid ""
-#~ "Thank you for purchasing a hosting plan, the payment for it is pending "
-#~ "and will be processed in the background."
-#~ msgstr ""
-#~ "شكرا لكم على شراء خطة الاستضافة، وعملية الدفع هي قيد الانتظار وستُعالج في "
-#~ "الخلفية."
-
-#~ msgid "The payment was rejected: {}"
-#~ msgstr "رُفض الدفع: {}"
-
-#~ msgid "Unknown reason"
-#~ msgstr "سبب مجهول"
-
-#~ msgid "Payments are temporarily inactive."
-#~ msgstr "لقد تم تعطيل الدفع مؤقتا."
-
-#~ msgid "Payment card"
-#~ msgstr "بطاقة الدفع"
-
-#~ msgid "Payment cancelled"
-#~ msgstr "تم إلغاء الدفع"
-
-#~ msgid "Payment error"
-#~ msgstr "خطأ في الدفع"
-
-#~ msgid "Bitcoin"
-#~ msgstr "البتكوين"
-
-#~ msgid "European VAT ID"
-#~ msgstr "معرف ضريبة القيمة المضافة الأوروبية"
-
-#~ msgid "Tax registration"
-#~ msgstr "التسجيل الضريبي"
-
-#~ msgid "Company or individual name"
-#~ msgstr "اسم الشركة أو اسم الفرد"
-
-#~ msgid "Address"
-#~ msgstr "العنوان البريدي"
-
-#~ msgid "Postcode and city"
-#~ msgstr "الرمز البريدي و المدينة"
-
-#~ msgid "Country"
-#~ msgstr "البلد"
-
-#~ msgid "The country has to match your VAT code"
-#~ msgstr "على البلد ان يطابق رمز ضريبة القيمة المضافة"
-
-#~ msgid "Annual"
-#~ msgstr "سنوي"
-
-#~ msgid "Biannual"
-#~ msgstr "نصف سنوي"
-
-#~ msgid "Quarterly"
-#~ msgstr "فصليا"
-
-#~ msgid "Monthly"
-#~ msgstr "شهرياً"
-
-#~ msgid "Onetime"
-#~ msgstr "مرة واحدة"
-
-#~ msgid "Repositories limit"
-#~ msgstr "حد المستودعات"
```

### Comparing `wllegal-2023.1/wllegal/locale/ar_LY/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ar_LY/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ars/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ars/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ast/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ast/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/az/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/az/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/be/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/be/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/be@latin/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/be_Latn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ber/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ber/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/bg/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/bn/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/bn_BD/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/bn_BD/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/bo/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/bo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/br/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/br/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ca/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ce/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ce/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ckb/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ckb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/crh/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/crh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/cs/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/cs/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # Michal Čihař <michal@cihar.com>, 2012, 2018, 2019.
 # Pavel Borecki <pavel.borecki@gmail.com>, 2018, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2021-09-22 06:48+0000\n"
-"Last-Translator: Michal Čihař <michal@weblate.org>\n"
+"PO-Revision-Date: 2023-03-09 22:56+0000\n"
+"Last-Translator: Petr Branberger <petr@webrun.cz>\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/weblate/legal/cs/>"
 "\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"X-Generator: Weblate 4.9-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subdodavatelé v souladu s článkem 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
@@ -320,16 +320,16 @@
 msgstr "Zobrazit anglickou verzi"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
-"Všeobecné smluvní podmínky jsou autoritativní v angličtině. Překlad do "
-"češtiny je poskytován pro vaše pohodlí."
+"Smluvní podmínky jsou závazné v angličtině, pro vaše pohodlí jsou k "
+"dispozici překlady."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 "Práva a povinnosti Uživatele a Provozovatele pramenící z užívání Služby se "
```

### Comparing `wllegal-2023.1/wllegal/locale/cv/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/cv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/cy/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/mk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Weblate <noreply@weblate.org>, 2019.
-# anonymous <noreply@weblate.org>, 2019.
-# Rhoslyn Prys <rprys@posteo.net>, 2019.
+# Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2021-05-16 22:32+0000\n"
-"Last-Translator: Christine Long <lilmamachrislong33@gmail.com>\n"
-"Language-Team: Welsh <https://hosted.weblate.org/projects/weblate/legal/cy/"
-">\n"
-"Language: cy\n"
+"PO-Revision-Date: 2019-07-22 07:40+0000\n"
+"Last-Translator: Michal Čihař <michal@cihar.com>\n"
+"Language-Team: Macedonian <https://hosted.weblate.org/projects/weblate/"
+"hosted/mk/>\n"
+"Language: mk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=(n==0) ? 0 : (n==1) ? 1 : (n==2) ? 2 : "
-"(n==3) ? 3 :(n==6) ? 4 : 5;\n"
-"X-Generator: Weblate 4.7-dev\n"
+"Plural-Forms: nplurals=2; plural=n==1 || n%10==1 ? 0 : 1;\n"
+"X-Generator: Weblate 3.8-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
@@ -58,16 +55,18 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:25
+#, fuzzy
+#| msgid "Username or email"
 msgid "Name and e-mail address"
-msgstr ""
+msgstr "Корисничко име или е-пошта"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events"
@@ -90,20 +89,18 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen"
 msgstr ""
-"Mae'r rhain wedi'u logio rhag ofn y bydd newidiadau pwysig i'ch cyfrif (e.e. "
-"newid cyfrinair) i ganiatáu diagnosis rhag ofn i'ch cyfrif gael ei ddwyn"
 
 #: wllegal/templates/legal/documents/privacy.html:36
 msgid "Billing information"
-msgstr "bilio gwybodaeth"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "In case you purchase service from us, we collect additional billing "
 "information necessary for issuing an invoice"
 msgstr ""
 
@@ -322,15 +319,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "Cwcis"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -363,16 +360,18 @@
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
+#, fuzzy
+#| msgid "Personal info"
 msgid "Personal Data"
-msgstr ""
+msgstr "Лични податоци"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -383,15 +382,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Prosiect"
+msgstr "Проект"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
@@ -399,35 +398,37 @@
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
+#, fuzzy
+#| msgid "Translation notifications"
 msgid "Translation Memory"
-msgstr ""
+msgstr "Преведувачки известувања"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr ""
+msgstr "Корисник"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "VCS"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
@@ -564,15 +565,15 @@
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr ""
+msgstr "Превод"
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -637,9 +638,16 @@
 
 #: wllegal/templates/legal/documents/tos.html:147
 msgid ""
 "These Terms of Service shall come into force and effect on 1st September "
 "2017."
 msgstr ""
 
-#~ msgid "Billing"
-#~ msgstr "Bilio"
+#, fuzzy
+#~| msgid "Subject"
+#~ msgid "Component limit"
+#~ msgstr "Предмет"
+
+#, fuzzy
+#~| msgid "Subject"
+#~ msgid "Projects limit"
+#~ msgstr "Предмет"
```

### Comparing `wllegal-2023.1/wllegal/locale/da/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/de/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/django.pot` & `wllegal-2023.2/wllegal/locale/django.pot`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/dv/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/dv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/el/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/en_GB/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/eo/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
+# Esperanto translations for PACKAGE package.
+# Copyright (C) 2015 THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Robert Readman <robert_readman@hotmail.com>, 2018.
-# anonymous <noreply@weblate.org>, 2019.
+# Automatically generated, 2015.
+# Jorge Maldonado Ventura <jorgesumle@freakspot.net>, 2019.
+# Michal Čihař <michal@cihar.com>, 2019.
+# Pierre Soubourou <pierre.soubourou@gmail.com>, 2019.
+# tuxayo/Victor Grousset <victor@tuxayo.net>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate\n"
+"Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2023-02-21 08:39+0000\n"
-"Last-Translator: Andi Chandler <andi@gowling.com>\n"
-"Language-Team: English (United Kingdom) <https://hosted.weblate.org/projects/"
-"weblate/legal/en_GB/>\n"
-"Language: en_GB\n"
+"PO-Revision-Date: 2019-08-18 06:22+0000\n"
+"Last-Translator: tuxayo/Victor Grousset <victor@tuxayo.net>\n"
+"Language-Team: Esperanto <https://hosted.weblate.org/projects/weblate/hosted/"
+"eo/>\n"
+"Language: eo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 3.8\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
@@ -32,82 +35,78 @@
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
-#, fuzzy
-#| msgid "Version control"
 msgid "Personal Data Controller"
-msgstr "Version control"
+msgstr "Kontrolilo de personaj datumoj"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:15
-#, python-format
+#, fuzzy, python-format
+#| msgid ""
+#| "We have appointed a data protection officer who may be reached via "
+#| "%(privacy_contact)s."
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
+"Ni nomumis datumprotektiston, kiun vi povas kontakti per %(privacy_contact)s."
 
 #: wllegal/templates/legal/documents/privacy.html:17
 #, fuzzy
-#| msgid "Translation process"
+#| msgid "Personal Data we process"
 msgid "Personal Data processed by Weblate"
-msgstr "Translation process"
+msgstr "Traktitaj personaj datumoj"
 
 #: wllegal/templates/legal/documents/privacy.html:20
-#, fuzzy
-#| msgid "We process only Personal Data User provides us by using our service:"
 msgid "Weblate only processes Personal Data the User provides by using it:"
-msgstr "We process only Personal Data User provides us by using our service:"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:25
 #, fuzzy
 #| msgid "Name and e-mail"
 msgid "Name and e-mail address"
-msgstr "Name and e-mail"
+msgstr "Uzantnomo kaj retpoŝtadreso"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits"
-msgstr "These are used to identify you in the VCS commits"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events"
-msgstr "Additionally, e-mail is used for notification of watched events"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr "Password in hashed form"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:30
-#, fuzzy
-#| msgid "Used to authenticate user if configured"
 msgid "Used to authenticate the User, if configured"
-msgstr "Used to authenticate user if configured"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr "IP address and browser name"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen"
 msgstr ""
-"These are logged in case of important changes to your account (e.g. password "
-"change) to allow diagnosis in case your account is stolen"
 
 #: wllegal/templates/legal/documents/privacy.html:36
 msgid "Billing information"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
@@ -145,18 +144,16 @@
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:52
-#, fuzzy
-#| msgid "Access the internal repository"
 msgid "Access to the Personal Data"
-msgstr "Access the internal repository"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
 
@@ -166,18 +163,16 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:60
-#, fuzzy
-#| msgid "Failed to process form!"
 msgid "Payment processors."
-msgstr "Failed to process form!"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 msgid "The Personal Data retention"
@@ -192,18 +187,16 @@
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "Access log information might be collected for a longer period for the "
 "purpose of establishing, exercising or defending legal claims."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:71
-#, fuzzy
-#| msgid "Your profile"
 msgid "Your rights"
-msgstr "Your profile"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
 
@@ -231,18 +224,16 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:82
 msgid "Restrict the Personal Data processing"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:83
-#, fuzzy
-#| msgid "Languages processing"
 msgid "Object to processing"
-msgstr "Languages processing"
+msgstr "Aferoj traktotaj"
 
 #: wllegal/templates/legal/documents/privacy.html:84
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
 
@@ -252,51 +243,42 @@
 "from the account management, and is fully automated."
 msgstr ""
 
 #: wllegal/templates/legal/documents/summary.html:4
 msgid ""
 "The services are provided “as is”, at your own risk, without any warranty."
 msgstr ""
-"The services are provided “as is”, at your own risk, without any warranty."
 
 #: wllegal/templates/legal/documents/summary.html:5
 msgid ""
 "Additional guarantees might apply to commercial customers, those are "
 "expressed in corresponding contracts."
 msgstr ""
-"Additional guarantees might apply to commercial customers, those are "
-"expressed in corresponding contracts."
 
 #: wllegal/templates/legal/documents/summary.html:6
 msgid ""
 "We process private data (such as your e-mail address), those will be "
 "discarded from our database as soon as you remove your account."
 msgstr ""
-"We process private data (such as your e-mail address), those will be "
-"discarded from our database as soon as you remove your account."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your translations are made under license which is specified by each "
 "translation."
 msgstr ""
-"Your translations are made under license which is specified by each "
-"translation."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
-"Your name and e-mail address is used in VCS commits, it will stay there "
-"indefinitely."
 
 #: wllegal/templates/legal/documents/summary.html:9
 msgid "We use cookies to deliver our services."
-msgstr "We use cookies to deliver our services."
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -307,30 +289,24 @@
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:20
-#, fuzzy
-#| msgid "Description"
 msgid "Definitions"
-msgstr "Description"
+msgstr "Difinoj"
 
 #: wllegal/templates/legal/documents/tos.html:22
-#, fuzzy
-#| msgid "Terms of Service"
 msgid "In these Terms of Service:"
-msgstr "Terms of Service"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:26
-#, fuzzy
-#| msgid "Advertisement"
 msgid "Agreement"
-msgstr "Advertisement"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
@@ -353,15 +329,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "Cookies"
+msgstr "Kuketoj"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -375,15 +351,15 @@
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr "License"
+msgstr "Permesilo"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
@@ -395,15 +371,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "Personal Data"
+msgstr "Personaj datumoj"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -414,55 +390,51 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Project"
+msgstr "Projekto"
 
 #: wllegal/templates/legal/documents/tos.html:55
-#, fuzzy
-#| msgid ""
-#| "However, the following translation projects are available on this server:"
 msgid "means translation project operated on the Service"
 msgstr ""
-"However, the following translation projects are available on this server:"
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "Service"
+msgstr "Servo"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
 msgid "Translation Memory"
-msgstr "Translation memory"
+msgstr "Traduka memoro"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "User"
+msgstr "Uzanto"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "VCS"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
@@ -599,15 +571,15 @@
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr "Translations"
+msgstr "Tradukoj"
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -672,65 +644,81 @@
 
 #: wllegal/templates/legal/documents/tos.html:147
 msgid ""
 "These Terms of Service shall come into force and effect on 1st September "
 "2017."
 msgstr ""
 
-#~ msgid "Reset all changes in the local repository"
-#~ msgstr "Reset all changes in the local repository"
+#~ msgid "Generate Unknown Horizons scenario data"
+#~ msgstr "Krei scenarajn datumojn pri nekonataj horizontoj"
 
 #~ msgid "Billing"
-#~ msgstr "Billing"
+#~ msgstr "Fakturado"
+
+#~ msgid "Choose the billing plan you want to update"
+#~ msgstr "Elektu la fakturadon, kiun vi volas ĝisdatigi"
+
+#~ msgid "Create new billing plan"
+#~ msgstr "Krei novan fakturadan planon"
+
+#~ msgid "Create billing plan"
+#~ msgstr "Krei fakturadan planon"
+
+#~ msgid "New billing plan"
+#~ msgstr "Nova fakturada plano"
+
+#~ msgid "Please choose a hosting plan that fits the size of your project."
+#~ msgstr ""
+#~ "Bonvolu elekti gastigantan planon kiu konvenas la grandecon de via "
+#~ "projekto."
+
+#~ msgid "Current billing status"
+#~ msgstr "Nuna fakturada statuso"
+
+#~ msgid "Too small for your project."
+#~ msgstr "Tro malgranda por via projekto."
+
+#~ msgid "Too small"
+#~ msgstr "Tro malgranda"
+
+#~ msgid "Selected plan"
+#~ msgstr "Elektita plano"
 
 #~ msgid "Current plan"
-#~ msgstr "Current plan"
+#~ msgstr "Nuna plano"
 
 #~ msgid "Strings limit"
-#~ msgstr "Strings limit"
+#~ msgstr "Tekstoĉena limo"
 
 #~ msgid "Unlimited"
-#~ msgstr "Unlimited"
+#~ msgstr "Senlima"
 
 #~ msgid "Languages limit"
-#~ msgstr "Languages limit"
+#~ msgstr "Lingvaj limoj"
 
 #, fuzzy
 #~| msgid "Projects limit"
 #~ msgid "Component limit"
-#~ msgstr "Projects limit"
+#~ msgstr "Projekta limo"
 
 #~ msgid "Projects limit"
-#~ msgstr "Projects limit"
+#~ msgstr "Projekta limo"
 
 #~ msgid "%(price)s EUR / month"
-#~ msgstr "%(price)s EUR / month"
-
-#~ msgid "%(price)s EUR / year"
-#~ msgstr "%(price)s EUR / year"
+#~ msgstr "%(price)s EUR / monate"
 
 #, fuzzy
 #~| msgid ""
-#~| "The pricing is based on number of source strings and number of target "
-#~| "languages. The source string is a text unit defined in a translation "
-#~| "format, it can be word, sentence or a paragraph."
+#~| "The pricing is based on number of source strings and target languages. "
+#~| "The source string is a text unit defined in a translation format, it can "
+#~| "be a word, sentence or paragraph."
 #~ msgid ""
 #~ "Pricing is based on the number of source strings and target languages. "
 #~ "The source string is a text unit defined in a translation format, it can "
 #~ "be a word, sentence or paragraph."
 #~ msgstr ""
-#~ "The pricing is based on number of source strings and number of target "
-#~ "languages. The source string is a text unit defined in a translation "
-#~ "format, it can be word, sentence or a paragraph."
-
-#, fuzzy
-#~| msgid "Failed to process form!"
-#~ msgid "Payment card"
-#~ msgstr "Failed to process form!"
-
-#, fuzzy
-#~| msgid "Failed to process form!"
-#~ msgid "Payment error"
-#~ msgstr "Failed to process form!"
+#~ "La prezo baziĝas sur iuj fontaj tekstoĉenoj kaj celaj lingvoj. Fonta "
+#~ "tekstoĉeno estas teksto-unuo difinita en traduka formato, vorto, frazo aŭ "
+#~ "alineo."
 
 #~ msgid "Repositories limit"
-#~ msgstr "Repositories limit"
+#~ msgstr "Limo de deponejoj"
```

### Comparing `wllegal-2023.1/wllegal/locale/enm/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/enm/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/eo/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/sl/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-# Esperanto translations for PACKAGE package.
-# Copyright (C) 2015 THE PACKAGE'S COPYRIGHT HOLDER
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Automatically generated, 2015.
-# Jorge Maldonado Ventura <jorgesumle@freakspot.net>, 2019.
-# Michal Čihař <michal@cihar.com>, 2019.
-# Pierre Soubourou <pierre.soubourou@gmail.com>, 2019.
-# tuxayo/Victor Grousset <victor@tuxayo.net>, 2019.
+# Domen <mitenem@outlook.com>, 2018, 2019.
+# anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2019-08-18 06:22+0000\n"
-"Last-Translator: tuxayo/Victor Grousset <victor@tuxayo.net>\n"
-"Language-Team: Esperanto <https://hosted.weblate.org/projects/weblate/hosted/"
-"eo/>\n"
-"Language: eo\n"
+"PO-Revision-Date: 2022-01-07 02:39+0000\n"
+"Last-Translator: Matej U <mateju@src.gnome.org>\n"
+"Language-Team: Slovenian <https://hosted.weblate.org/projects/weblate/legal/"
+"sl/>\n"
+"Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 3.8\n"
+"Plural-Forms: nplurals=4; plural=n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n"
+"%100==4 ? 2 : 3;\n"
+"X-Generator: Weblate 4.10.1\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
@@ -35,60 +33,60 @@
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
+#, fuzzy
+#| msgid "Version control"
 msgid "Personal Data Controller"
-msgstr "Kontrolilo de personaj datumoj"
+msgstr "Nadzor različic"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:15
-#, fuzzy, python-format
-#| msgid ""
-#| "We have appointed a data protection officer who may be reached via "
-#| "%(privacy_contact)s."
+#, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
-"Ni nomumis datumprotektiston, kiun vi povas kontakti per %(privacy_contact)s."
 
 #: wllegal/templates/legal/documents/privacy.html:17
 #, fuzzy
-#| msgid "Personal Data we process"
+#| msgid "Translation process"
 msgid "Personal Data processed by Weblate"
-msgstr "Traktitaj personaj datumoj"
+msgstr "Postopek prevajanja"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:25
 #, fuzzy
 #| msgid "Name and e-mail"
 msgid "Name and e-mail address"
-msgstr "Uzantnomo kaj retpoŝtadreso"
+msgstr "Ime in e-pošta"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:29
+#, fuzzy
+#| msgid "Password changed"
 msgid "Password in hashed form"
-msgstr ""
+msgstr "Geslo sem spremenil"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
@@ -102,15 +100,15 @@
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:36
 msgid "Billing information"
-msgstr ""
+msgstr "Podatki obračunavanja"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "In case you purchase service from us, we collect additional billing "
 "information necessary for issuing an invoice"
 msgstr ""
 
@@ -144,16 +142,18 @@
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:52
+#, fuzzy
+#| msgid "Allow changes in the local repository"
 msgid "Access to the Personal Data"
-msgstr ""
+msgstr "Dovoli spremembe v lokalni shrambi"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
 
@@ -163,16 +163,18 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:60
+#, fuzzy
+#| msgid "Failed to process form!"
 msgid "Payment processors."
-msgstr ""
+msgstr "Nismo uspeli obdelati obrazca!"
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 msgid "The Personal Data retention"
@@ -187,16 +189,18 @@
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "Access log information might be collected for a longer period for the "
 "purpose of establishing, exercising or defending legal claims."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:71
+#, fuzzy
+#| msgid "Your profile"
 msgid "Your rights"
-msgstr ""
+msgstr "Vaš profil"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
 
@@ -224,16 +228,18 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:82
 msgid "Restrict the Personal Data processing"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:83
+#, fuzzy
+#| msgid "Languages processing"
 msgid "Object to processing"
-msgstr "Aferoj traktotaj"
+msgstr "Jeziki v obdelavi"
 
 #: wllegal/templates/legal/documents/privacy.html:84
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
 
@@ -289,24 +295,30 @@
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:20
+#, fuzzy
+#| msgid "Description"
 msgid "Definitions"
-msgstr "Difinoj"
+msgstr "Opis"
 
 #: wllegal/templates/legal/documents/tos.html:22
+#, fuzzy
+#| msgid "Terms of Service"
 msgid "In these Terms of Service:"
-msgstr ""
+msgstr "Pogoji storitev"
 
 #: wllegal/templates/legal/documents/tos.html:26
+#, fuzzy
+#| msgid "Advertisement"
 msgid "Agreement"
-msgstr ""
+msgstr "Oglas"
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
@@ -329,15 +341,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "Kuketoj"
+msgstr "Piškotki"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -351,90 +363,93 @@
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr "Permesilo"
+msgstr "Licenca"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr ""
+msgstr "Ponudnik"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "Personaj datumoj"
+msgstr "Osebni podatki"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr ""
+msgstr "Lastnik"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Projekto"
+msgstr "Projekt"
 
 #: wllegal/templates/legal/documents/tos.html:55
+#, fuzzy
+#| msgid ""
+#| "However, the following translation projects are available on this server:"
 msgid "means translation project operated on the Service"
-msgstr ""
+msgstr "Kakor koli, na strežniku so na voljo naslednji prevajalski projekti:"
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "Servo"
+msgstr "Storitev"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
 msgid "Translation Memory"
-msgstr "Traduka memoro"
+msgstr "Spomin prevodov"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Uzanto"
+msgstr "Uporabnik"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr ""
+msgstr "VCS"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
@@ -571,15 +586,15 @@
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr "Tradukoj"
+msgstr "Prevodi"
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -644,81 +659,68 @@
 
 #: wllegal/templates/legal/documents/tos.html:147
 msgid ""
 "These Terms of Service shall come into force and effect on 1st September "
 "2017."
 msgstr ""
 
-#~ msgid "Generate Unknown Horizons scenario data"
-#~ msgstr "Krei scenarajn datumojn pri nekonataj horizontoj"
+#~ msgid "Reset all changes in the local repository"
+#~ msgstr "Ponastavi vse spremembe v lokalni shrambi"
 
 #~ msgid "Billing"
-#~ msgstr "Fakturado"
-
-#~ msgid "Choose the billing plan you want to update"
-#~ msgstr "Elektu la fakturadon, kiun vi volas ĝisdatigi"
-
-#~ msgid "Create new billing plan"
-#~ msgstr "Krei novan fakturadan planon"
-
-#~ msgid "Create billing plan"
-#~ msgstr "Krei fakturadan planon"
-
-#~ msgid "New billing plan"
-#~ msgstr "Nova fakturada plano"
-
-#~ msgid "Please choose a hosting plan that fits the size of your project."
-#~ msgstr ""
-#~ "Bonvolu elekti gastigantan planon kiu konvenas la grandecon de via "
-#~ "projekto."
-
-#~ msgid "Current billing status"
-#~ msgstr "Nuna fakturada statuso"
-
-#~ msgid "Too small for your project."
-#~ msgstr "Tro malgranda por via projekto."
-
-#~ msgid "Too small"
-#~ msgstr "Tro malgranda"
-
-#~ msgid "Selected plan"
-#~ msgstr "Elektita plano"
+#~ msgstr "Zaračunavanje"
 
 #~ msgid "Current plan"
-#~ msgstr "Nuna plano"
+#~ msgstr "Trenutni načrt"
 
 #~ msgid "Strings limit"
-#~ msgstr "Tekstoĉena limo"
+#~ msgstr "Omejitev nizov"
 
 #~ msgid "Unlimited"
-#~ msgstr "Senlima"
+#~ msgstr "Neomejeno"
 
 #~ msgid "Languages limit"
-#~ msgstr "Lingvaj limoj"
+#~ msgstr "Omejitev jezikov"
 
 #, fuzzy
 #~| msgid "Projects limit"
 #~ msgid "Component limit"
-#~ msgstr "Projekta limo"
+#~ msgstr "Omejitev projektov"
 
 #~ msgid "Projects limit"
-#~ msgstr "Projekta limo"
+#~ msgstr "Omejitev projektov"
 
 #~ msgid "%(price)s EUR / month"
-#~ msgstr "%(price)s EUR / monate"
+#~ msgstr "%(price)s EUR/mesec"
+
+#~ msgid "%(price)s EUR / year"
+#~ msgstr "%(price)s EUR/leto"
 
 #, fuzzy
 #~| msgid ""
-#~| "The pricing is based on number of source strings and target languages. "
-#~| "The source string is a text unit defined in a translation format, it can "
-#~| "be a word, sentence or paragraph."
+#~| "The pricing is based on number of source strings and number of target "
+#~| "languages. The source string is a text unit defined in a translation "
+#~| "format, it can be word, sentence or a paragraph."
 #~ msgid ""
 #~ "Pricing is based on the number of source strings and target languages. "
 #~ "The source string is a text unit defined in a translation format, it can "
 #~ "be a word, sentence or paragraph."
 #~ msgstr ""
-#~ "La prezo baziĝas sur iuj fontaj tekstoĉenoj kaj celaj lingvoj. Fonta "
-#~ "tekstoĉeno estas teksto-unuo difinita en traduka formato, vorto, frazo aŭ "
-#~ "alineo."
+#~ "Cena temelji na številu izvirnih nizov in številu ciljnih jezikov. "
+#~ "Izvirni niz je besedilna enota, opredeljena v prevajalski obliki; lahko "
+#~ "je beseda, poved ali odstavek."
+
+#, fuzzy
+#~| msgid "Failed to process form!"
+#~ msgid "Payment card"
+#~ msgstr "Nismo uspeli obdelati obrazca!"
+
+#, fuzzy
+#~| msgid "Failed to process form!"
+#~ msgid "Payment error"
+#~ msgstr "Nismo uspeli obdelati obrazca!"
+
+#~ msgid "Monthly"
+#~ msgstr "Mesečno"
 
 #~ msgid "Repositories limit"
-#~ msgstr "Limo de deponejoj"
+#~ msgstr "Omejitev shramb"
```

### Comparing `wllegal-2023.1/wllegal/locale/es/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/et/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/et/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Michal Čihař <michal@cihar.com>, 2019.
 # Janar Leas <janar.leas@gmail.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2021-04-27 16:32+0000\n"
+"PO-Revision-Date: 2023-03-10 11:02+0000\n"
 "Last-Translator: Priit Jõerüüt <hwlate@joeruut.com>\n"
 "Language-Team: Estonian <https://hosted.weblate.org/projects/weblate/legal/"
 "et/>\n"
 "Language: et\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.7-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 "Alltöövõtjate tegevus toimub vastavalt Isikuandmete Kaitse Üldmääruse "
 "artiklile 28"
 
@@ -626,22 +626,16 @@
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:135
-#, fuzzy
-#| msgid ""
-#| "The Service uses Cookies to personalise content, and to analyse our "
-#| "traffic."
 msgid "The Service uses Cookies to personalise content."
-msgstr ""
-"See teenus kasutab sisu isikustamiseks ja veebiliikluse analüüsiks "
-"küpsisefaile."
+msgstr "See teenus kasutab sisu isikustamiseks küpsisefaile."
 
 #: wllegal/templates/legal/documents/tos.html:138
 msgid "Governing Law"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:140
 msgid ""
```

### Comparing `wllegal-2023.1/wllegal/locale/eu/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/fa/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/fi/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/fil/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/fil/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/fr/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 # Julien Humbert <julroy67@gmail.com>, 2020.
 # Localisation Lab <ao@localizationlab.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2021-11-18 02:52+0000\n"
-"Last-Translator: Julien Humbert <julroy67@gmail.com>\n"
+"PO-Revision-Date: 2023-03-21 06:01+0000\n"
+"Last-Translator: Ldm Public <ldmpub@gmail.com>\n"
 "Language-Team: French <https://hosted.weblate.org/projects/weblate/legal/fr/>"
 "\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.9.1-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Sous-traitant conformément à l’art. 28 de la RGPD"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
@@ -579,24 +579,24 @@
 "Fournisseur et/ou l’utilisation de ces moyens par le Fournisseur."
 
 #: wllegal/templates/legal/documents/tos.html:86
 msgid ""
 "The User agrees to refrain from use of the Service in bad faith and/or "
 "deliberately causing any damage to the Service."
 msgstr ""
-"L’Utilisateur s’engage à s’abstenir d’utiliser le Service de mauvaise foi et/"
-"ou de causer délibérément des dommages au Service."
+"L’Utilisateur s’engage à ne pas utiliser le Service de mauvaise foi et / ou "
+"à causer délibérément des dommages au Service."
 
 #: wllegal/templates/legal/documents/tos.html:88
 msgid ""
 "The User agrees to refrain from bypassing the Service’s software and/or "
 "technical hardware means, in particular the security systems."
 msgstr ""
-"L’Utilisateur s’engage à ne pas contourner les moyens logiciels et/ou "
-"matériels techniques du Service, notamment les systèmes de sécurité."
+"L’Utilisateur s’engage à ne pas contourner les moyens logiciels et matériels "
+"du Service, notamment les systèmes de sécurité."
 
 #: wllegal/templates/legal/documents/tos.html:91
 msgid "Liability for Damage"
 msgstr "Responsabilités en cas de dommages"
 
 #: wllegal/templates/legal/documents/tos.html:93
 msgid ""
```

### Comparing `wllegal-2023.1/wllegal/locale/fur/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/fur/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/fy/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/fy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/gl/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/he/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/hi/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/hr/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/hu/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/hy/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/hy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ia/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ia/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/id/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ie/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ie/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/is/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/it/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ja/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ka/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/kab/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/kab/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/kk/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/kk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/km/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/km/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/kmr/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/kmr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ko/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ko/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 # Jun Hyung Shin <shmishmi79@gmail.com>, 2019.
 # Lee Yunseok <ironyunseok@protonmail.com>, 2019, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2021-12-06 21:44+0000\n"
-"Last-Translator: OctopusET <sumoon@seoulsaram.org>\n"
+"PO-Revision-Date: 2023-03-05 16:40+0000\n"
+"Last-Translator: 이정희 <daemul72@gmail.com>\n"
 "Language-Team: Korean <https://hosted.weblate.org/projects/weblate/legal/ko/>"
 "\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "GDPR Art. 28에 따른 협력업체"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
@@ -50,21 +50,20 @@
 msgstr "%(provider)s, 등록 번호. No. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
-msgstr ""
-"웨블레이트는 %(privacy_contact)s을 통해 연락할 수 있는 자료 보호 책임자를 임"
-"명했습니다."
+msgstr "Weblate는 %(privacy_contact)s을 통해 연락할 수 있는 자료 보호 책임자를 "
+"임명했습니다."
 
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
-msgstr "웨블레이트의 개인 자료가 처리됨"
+msgstr "Weblate의 개인 자료가 처리됨"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr "우리는 사용자가 제공한 개인 정보만 처리합니다:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
@@ -207,16 +206,15 @@
 msgid "Your rights"
 msgstr "당신의 권리"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
-msgstr ""
-"사용자는 개인 자료를 자발적으로 사용합니다. 이 개인 자료 없이는 웨블레이트는 "
+msgstr "사용자는 개인 자료를 자발적으로 사용합니다. 이 개인 자료 없이는 Weblate는 "
 "서비스를 제공할 수 없습니다."
 
 #: wllegal/templates/legal/documents/privacy.html:75
 msgid ""
 "We want you to always be in control of your Personal Data. To this end, you "
 "have certain rights that allow for it. Under certain conditions, you may:"
 msgstr ""
@@ -443,23 +441,23 @@
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
 msgstr "서비스"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
-msgstr "공급자에 의해 운영되는 웨블레이트 기반 누리집과 서비스를 의미"
+msgstr "공급자가 운영하는 Weblate 기반 웹사이트 및 서비스를 의미합니다"
 
 #: wllegal/templates/legal/documents/tos.html:60
 msgid "Translation Memory"
 msgstr "번역 메모리"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
-msgstr "웨블레이트에서 제공되는 선택적 번역 메모리 서비스를 의미"
+msgstr "Weblate 내에서 제공되는 선택적 번역 메모리 서비스를 의미합니다"
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
 msgstr "사용자"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
```

### Comparing `wllegal-2023.1/wllegal/locale/ksh/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ksh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ln/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ln/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/lt/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/lv/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/en_GB/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,701 +1,844 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# Robert Readman <robert_readman@hotmail.com>, 2018.
+# anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2022-11-07 19:02+0000\n"
-"Last-Translator: Coool (github.com/Coool) <coool@mail.lv>\n"
-"Language-Team: Latvian <https://hosted.weblate.org/projects/weblate/legal/lv/"
-">\n"
-"Language: lv\n"
+"PO-Revision-Date: 2023-04-02 13:34+0000\n"
+"Last-Translator: Andi Chandler <andi@gowling.com>\n"
+"Language-Team: English (United Kingdom) <https://hosted.weblate.org/projects/"
+"weblate/legal/en_GB/>\n"
+"Language: en_GB\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n % 10 == 0 || n % 100 >= 11 && n % 100 <= "
-"19) ? 0 : ((n % 10 == 1 && n % 100 != 11) ? 1 : 2);\n"
-"X-Generator: Weblate 4.14.2\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr "Apakšuzņēmēji saskaņā ar GDPR 28. pantu"
+msgstr "Subcontractors in accordance with Art. 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
-msgstr "2020. gada oktobra statuss."
+msgstr "Status as of October 2020."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
-"Mēs ievērojam regulu Nr. %(law_679_2016)s, Vispārīgo datu aizsardzības "
-"regulu, kas pazīstama arī kā GDPR. Šis dokuments iekļauj nepieciešamās "
-"specifikācijas."
+"We comply with the Regulation No. %(law_679_2016)s, the General Data "
+"Protection Regulation, also known as GDPR. This document includes necessary "
+"specifications."
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr "Personas datu pārvaldnieks"
+msgstr "Personal Data Controller"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s, Reģ. Nr. %(reg_no)s"
+msgstr "%(provider)s, Reg. No. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
-"Weblate ir datu aizsardzības speciālists, ar kuru var sazināties, izmantojot "
+"Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
-msgstr "Personas dati, ko apstrādā Weblate"
+msgstr "Personal Data processed by Weblate"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
-msgstr ""
-"Weblate vietne apstrādā tikai tos Personas datus, ko Lietotājs pats "
-"iesniedzis, izmantojot mūsu pakalpojumu:"
+msgstr "Weblate only processes Personal Data the User provides by using it:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
-msgstr "Vārds un e-pasta adrese"
+msgstr "Name and e-mail address"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits"
-msgstr ""
-"Tie tiek izmantoti, lai identificētu jūs VCS iesniegtajās izmaiņās (commits)"
+msgstr "These are used to identify you in the VCS commits"
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events"
-msgstr ""
-"Turklāt e-pasts tiek izmantots, lai nosūtītu notikumu paziņojumus, kuriem "
-"jūs sekojiet"
+msgstr "Additionally, e-mail is used for notification of watched events"
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr "Parole šifrētā (hashed) formā"
+msgstr "Password in hashed form"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
-msgstr "Ja tas ir konfigurēts, izmanto, lai autorizētu lietotāju"
+msgstr "Used to authenticate the User, if configured"
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
-msgstr "Paroles tiek saglabātas šifrētas, izmantojot Argon2."
+msgstr "Passwords are stored hashed using Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr "IP adrese un pārlūkprogrammas nosaukums"
+msgstr "IP address and browser name"
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen"
 msgstr ""
-"Tie tiek reģistrēti, ja tiek veiktas svarīgas izmaiņas jūsu kontā (piemēram, "
-"paroles maiņa), lai varētu veikt diagnostiku konta nozagšanas gadījumā"
+"These are logged in case of important changes to your account (e.g. password "
+"change) to allow diagnosis in case your account is stolen"
 
 #: wllegal/templates/legal/documents/privacy.html:36
 msgid "Billing information"
-msgstr "Rēķinu informācija"
+msgstr "Billing information"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "In case you purchase service from us, we collect additional billing "
 "information necessary for issuing an invoice"
 msgstr ""
-"Ja iegādājaties pakalpojumu no mums, mēs ievācam papildus informāciju, kas "
-"nepieciešama rēķina izrakstīšanai"
+"In case you purchase service from us, we collect additional billing "
+"information necessary for issuing an invoice"
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
-msgstr "Personas datu apstrādes mērķis un juridiskais pamats"
+msgstr "Purpose and legal basis of processing Personal Data"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr "Jūsu personas dati tiks izmantoti pakalpojuma vajadzībām:"
+msgstr "Your Personal Data will be used for the purposes of the Service:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
 "contractual or pre-contractual obligations (<a href=\"%(url)s\">Article 6 "
 "(1) b. GDPR</a>)"
 msgstr ""
-"nodrošināt mūsu pakalpojumus, kas saistīti ar pakalpojumu, un sazināties ar "
-"jums jautājumos par mūsu pakalpojumiem (tostarp izmantojot e-pastu un "
-"ziņojumapmaiņu) un būt pārliecinātiem par mūsu pakalpojumu tehnisko "
-"funkcionalitāti, pildot līgumsaistības vai pirmslīguma saistības (<a href=\""
-"%(url)s\">VDAR(GDPR) 6. panta 1. punkta b) apakšpunkts</a>)"
+"for providing our services on the Service, to contact you in matters "
+"regarding our services (also by means of e-mails and messaging) and to "
+"ensure the technical functionality of our services fulfillment of "
+"contractual or pre-contractual obligations (<a href=\"%(url)s\">Article 6 (1)"
+" b. GDPR</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:48
 #, python-format
 msgid ""
 "to analyze your use of our services and improve our services (<a href="
 "\"%(url)s\">Article 6 (1) b. and f. GDPR</a>)"
 msgstr ""
-"lai analizētu mūsu pakalpojumu izmantošanu un uzlabotu mūsu pakalpojumus (<a "
-"href=\"%(url)s\">VDAR(GDPR) 6. panta 1. punkta b) un f) apakšpunkts</a>)"
+"to analyze your use of our services and improve our services (<a href=\""
+"%(url)s\">Article 6 (1) b. and f. GDPR</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:49
 #, python-format
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
-"ar jūsu nepārprotamu piekrišanu vai norādījumiem, lai veiktu mūsu "
-"uzņēmējdarbību vai nosūtītu jums informatīvos izdevumus (<a href=\"%(url)s\""
-">VDAR(GDPR) 6. panta 1. punkts a.</a>)"
+"with your express consent or instruction to carry out our business "
+"activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
+"GDPR</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
-msgstr "Piekļuve personas datiem"
+msgstr "Access to the Personal Data"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
-"Pārvaldnieks ir veicis visus saprātīgos tehniskos pasākumus personas datu "
-"aizsardzībai. Personas datiem var piekļūt tikai pilnvarotas personas."
+"The Controller has made all reasonable technical means to protect the "
+"Personal Data. Only authorised persons can access the Personal Data."
 
 #: wllegal/templates/legal/documents/privacy.html:56
 msgid ""
 "Third parties which can gain access to the Personal Data when necessary are:"
-msgstr "Trešās personas, kuras vajadzības gadījumā var piekļūt personas datiem:"
+msgstr ""
+"Third parties which can gain access to the Personal Data when necessary are:"
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
-msgstr "Personas, ar kurām noslēgts līgums par pakalpojuma tehnisko drošību."
+msgstr "Persons which are contracted for technical assurance of the service."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors."
-msgstr "Maksājumu apstrādātāji."
+msgstr "Payment processors."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
-msgstr "Visi personas dati tiek glabāti Eiropas Savienībā."
+msgstr "All Personal Data is stored in the European Union."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 msgid "The Personal Data retention"
-msgstr "Tiesības uz personas datu glabāšanu"
+msgstr "The Personal Data retention"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
-"Personas datus pakalpojums uzglabā līdz brīdim, kad lietotājs izdzēš savu "
-"kontu."
+"The Personal Data is stored in the Service until the User deletes their "
+"account on the service."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "Access log information might be collected for a longer period for the "
 "purpose of establishing, exercising or defending legal claims."
 msgstr ""
-"Piekļuves žurnāla informācija var tikt vākta ilgāku laika periodu, lai "
-"celtu, izskatītu vai aizstāvētu juridiskās prasības tiesvedībā."
+"Access log information might be collected for a longer period for the "
+"purpose of establishing, exercising or defending legal claims."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "Your rights"
-msgstr "Jūsu tiesības"
+msgstr "Your rights"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
-"Lietotājs savus personas datu sniedz brīvprātīgi. Weblate nevar sniegt "
-"pakalpojumus bez šiem personas datiem."
+"The User provides use of Personal Data voluntarily. Without this Personal "
+"Data Weblate is not able to provide our services."
 
 #: wllegal/templates/legal/documents/privacy.html:75
 msgid ""
 "We want you to always be in control of your Personal Data. To this end, you "
 "have certain rights that allow for it. Under certain conditions, you may:"
 msgstr ""
-"Mēs vēlamies, lai jūs vienmēr varētu kontrolēt savu personisko informāciju. "
-"Šajā nolūkā jums ir atbilstošas tiesības, kas to atļauj. Noteiktos apstākļos "
-"jūs varat:"
+"We want you to always be in control of your Personal Data. To this end, you "
+"have certain rights that allow for it. Under certain conditions, you may:"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 #, python-format
 msgid ""
 "Gain access to all your Personal Data that Weblate uses or processes, and "
 "even get a copy of all of it (<a href=\"%(url)s\">Article 15 GDPR</a>)"
 msgstr ""
-"Iegūt piekļuvi visiem saviem personas datiem, kurus Weblate izmanto vai "
-"apstrādā, kā arī iegūt to pilno kopiju (<a href=\"%(url)s\">VDAR(GDPR) 15. "
-"pants</a>)"
+"Gain access to all your Personal Data that Weblate uses or processes, and "
+"even get a copy of all of it (<a href=\"%(url)s\">Article 15 GDPR</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:80
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
 msgstr ""
-"Labot personas datus, kurus Weblate apstrādā, ja domājat, ka tie satur kļūdas"
+"Correct the Personal Data that Weblate processes if you think that there are "
+"mistakes"
 
 #: wllegal/templates/legal/documents/privacy.html:81
 msgid "Order us to delete your Personal Data"
-msgstr "Pieprasīt mūs dzēst jūsu personas datus"
+msgstr "Order us to delete your Personal Data"
 
 #: wllegal/templates/legal/documents/privacy.html:82
 msgid "Restrict the Personal Data processing"
-msgstr "Ierobežot personas datu apstrādi"
+msgstr "Restrict the Personal Data processing"
 
 #: wllegal/templates/legal/documents/privacy.html:83
 msgid "Object to processing"
-msgstr "Iebilst pret apstrādi"
+msgstr "Object to processing"
 
 #: wllegal/templates/legal/documents/privacy.html:84
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
-"Iegūt savus personas datus parastā un mašīnlasāmā formātā vai pārsūtīt šos "
-"personas datus citam pakalpojuma sniedzējam."
+"Receive your Personal Data in a commonly used and machine-readable format or "
+"to transmit this Personal Data to a different provider."
 
 #: wllegal/templates/legal/documents/privacy.html:87
 msgid ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
-"Jūsu personas datu dzēšanu, labošanu vai ieguvi var veikt no kontu "
-"pārvaldības, un tā ir pilnībā automatizēta."
+"The removal, correction, and retrieval of your Personal Data can be done "
+"from the account management, and is fully automated."
 
 #: wllegal/templates/legal/documents/summary.html:4
 msgid ""
 "The services are provided “as is”, at your own risk, without any warranty."
 msgstr ""
-"Pakalpojumi tiek sniegti “tādi, kādi tie ir”, uz jūsu risku un atbildības, "
-"bez jebkādas garantijas."
+"The services are provided “as is”, at your own risk, without any warranty."
 
 #: wllegal/templates/legal/documents/summary.html:5
 msgid ""
 "Additional guarantees might apply to commercial customers, those are "
 "expressed in corresponding contracts."
 msgstr ""
-"Papildu garantijas var būt spēkā maksas (komerciāliem) klientiem, tās ir "
-"aprakstītas attiecīgajos līgumos."
+"Additional guarantees might apply to commercial customers, those are "
+"expressed in corresponding contracts."
 
 #: wllegal/templates/legal/documents/summary.html:6
 msgid ""
 "We process private data (such as your e-mail address), those will be "
 "discarded from our database as soon as you remove your account."
 msgstr ""
-"Mēs apstrādājam privātos datus (piemēram, jūsu e-pasta adresi), tie tiks "
-"izdzēsti no mūsu datu bāzes, tiklīdz izdzēsīsit savu kontu."
+"We process private data (such as your e-mail address), those will be "
+"discarded from our database as soon as you remove your account."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your translations are made under license which is specified by each "
 "translation."
 msgstr ""
-"Jūsu veiktie tulkojumi tiek izdoti saskaņā ar licenci, kas norādīta katram "
-"tulkošanas projektam."
+"Your translations are made under license which is specified by each "
+"translation."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
-"Jūsu vārds un e-pasta adrese tiks izmantota versiju kontroles (VCS) "
-"iesniegtajās izmaiņās (commits), un tie paliek tur uz visiem laikiem."
+"Your name and e-mail address is used in VCS commits, it will stay there "
+"indefinitely."
 
 #: wllegal/templates/legal/documents/summary.html:9
 msgid "We use cookies to deliver our services."
-msgstr "Mēs izmantojam sīkfailus, lai nodrošinātu mūsu pakalpojumus."
+msgstr "We use cookies to deliver our services."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
-msgstr "Skatīt angļu valodas versiju"
+msgstr "View English version"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
-"Pakalpojuma oficiālie lietošanas noteikumi ir dokumentēti angļu valodā, jūsu "
-"ērtībai tiek sniegti tulkojumi."
+"The Terms of Service document is authoritative in English, translations are "
+"provided for your convenience."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
-"Šie pakalpojuma noteikumi regulē lietotāja un pakalpojuma sniedzēja tiesības "
-"un pienākumus, kas rodas pakalpojuma izmantošanas rezultātā."
+"The rights and obligations of the User and the Provider resulting from the "
+"use of the Service are governed by these Terms of Service."
 
 #: wllegal/templates/legal/documents/tos.html:20
 msgid "Definitions"
-msgstr "Definīcijas"
+msgstr "Definitions"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
-msgstr "Šajos pakalpojumu sniegšanas noteikumos:"
+msgstr "In these Terms of Service:"
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
-msgstr "Līgums"
+msgstr "Agreement"
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
-"licences līgums (tādā nozīmē, kādā to interpretē ar Civilkodeksa 2358. pantu)"
-", kas noslēgts starp lietotāju un pakalpojuma sniedzēju ar viņu piekrišanu"
+"means Licence Agreement within the meaning of Article 2358 et seq. of the "
+"Civil Code concluded by and between the User and the Provider upon the "
+"Consent"
 
 #: wllegal/templates/legal/documents/tos.html:29
 msgid "Civil Code"
-msgstr "Civilkodekss"
+msgstr "Civil Code"
 
 #: wllegal/templates/legal/documents/tos.html:30
 #, python-format
 msgid "means Act No. %(law_89_2012)s Coll., the Civil Code, as amended"
-msgstr "likums Nr. %(law_89_2012)s Coll., Čehijas Civilkodekss ar grozījumiem"
+msgstr "means Act No. %(law_89_2012)s Coll., the Civil Code, as amended"
 
 #: wllegal/templates/legal/documents/tos.html:32
 msgid "Consent"
-msgstr "Vienošanās"
+msgstr "Consent"
 
 #: wllegal/templates/legal/documents/tos.html:33
 msgid ""
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
+"means the User’s consent with these Terms of Service and other legal "
+"documents expressed by checking the checkbox during the registration"
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "Sīkdatnes"
+msgstr "Cookies"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
+"means any datafile sent by the web server of the Service to the User’s "
+"computer or other device connected to the Internet, which enable obtaining "
+"unique identification of the User’s web browser"
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr "VDAR(GDPR)"
+msgstr "GDPR"
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
+"means EU Regulation No. %(law_679_2016)s, the General Data Protection "
+"Regulation"
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr "Licence"
+msgstr "License"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
+"means non-exclusive license granted by the Provider to the User for use of "
+"the Service"
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr "Pakalpojumu sniedzējs"
+msgstr "Provider"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s ar reģ. Nr. %(reg_no)s"
+msgstr "means %(provider)s, Reg. No. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "Personas dati, Personiskie dati"
+msgstr "Personal Data"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
+"means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
+"inserted by the User into the Service and/or Cookies"
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr "Īpašnieks"
+msgstr "Owner"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
-msgstr "lietotājs, kurš var pārvaldīt projektu"
+msgstr "means the User who can manage Project"
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Projekts"
+msgstr "Project"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
-msgstr "tulkošanas projekts, kas tiek realizēts, izmantojot Pakalpojumu"
+msgstr "means translation project operated on the Service"
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "Pakalpojums"
+msgstr "Service"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
-"uz Weblate balstīta tīmekļa vietne un pakalpojumi, ko nodrošina Pakalpojumu "
-"sniedzējs"
+"means the website and services based on Weblate operated by the Provider"
 
 #: wllegal/templates/legal/documents/tos.html:60
 msgid "Translation Memory"
-msgstr "Tulkojumu atmiņa"
+msgstr "Translation memory"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
-msgstr ""
+msgstr "means the optional translation memory service provided within Weblate"
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Lietotājs"
+msgstr "User"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
+"means any legal entity or an individual other than the Provider, who is "
+"using the Service"
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "Versiju kontroles sistēma (VCS)"
+msgstr "VCS"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
-"projektā izmantotā versiju kontroles sistēma, piemēram, Git vai Mercurial"
+"means distributed version control system used by the Project such as Git or "
+"Mercurial"
 
 #: wllegal/templates/legal/documents/tos.html:71
 msgid "License Agreement Conclusion"
-msgstr "Licences līguma noslēgšana"
+msgstr "Licence Agreement Conclusion"
 
 #: wllegal/templates/legal/documents/tos.html:73
 msgid ""
 "The License Agreement is concluded upon the User’s Acceptance of the "
 "Provider’s Offer."
 msgstr ""
+"The Licence Agreement is concluded upon the User’s Acceptance of the "
+"Provider’s Offer."
 
 #: wllegal/templates/legal/documents/tos.html:76
 msgid "License Agreement"
-msgstr "Licences līgums"
+msgstr "Licence Agreement"
 
 #: wllegal/templates/legal/documents/tos.html:78
 msgid ""
 "By concluding Agreement under Article 2.1 of this Agreement, the following "
 "provisions of this Article 3 of the Terms of Service come into force."
 msgstr ""
+"By concluding Agreement under Article 2.1 of this Agreement, the following "
+"provisions of this Article 3 of the Terms of Service come into force."
 
 #: wllegal/templates/legal/documents/tos.html:80
 msgid ""
 "The Provider presents the User with a License Agreement and the User accepts "
 "this License Agreement, all this under the terms and conditions stated in "
 "these Terms of Service."
 msgstr ""
+"The Provider presents the User with a Licence Agreement and the User accepts "
+"this Licence Agreement, all this under the terms and conditions stated in "
+"these Terms of Service."
 
 #: wllegal/templates/legal/documents/tos.html:82
 msgid ""
 "The Provider shall have the right to shut down, adjust, modify or make the "
 "Service unavailable on the web address at any time."
 msgstr ""
+"The Provider shall have the right to shut down, adjust, modify or make the "
+"Service unavailable on the web address at any time."
 
 #: wllegal/templates/legal/documents/tos.html:84
 msgid ""
 "The User agrees to use the Service only in a manner not jeopardizing "
 "technical software and/or hardware means of the Provider and/or such means "
 "in the Provider’s use."
 msgstr ""
+"The User agrees to use the Service only in a manner not jeopardising "
+"technical software and/or hardware means of the Provider and/or such means "
+"in the Provider’s use."
 
 #: wllegal/templates/legal/documents/tos.html:86
 msgid ""
 "The User agrees to refrain from use of the Service in bad faith and/or "
 "deliberately causing any damage to the Service."
 msgstr ""
+"The User agrees to refrain from use of the Service in bad faith and/or "
+"deliberately causing any damage to the Service."
 
 #: wllegal/templates/legal/documents/tos.html:88
 msgid ""
 "The User agrees to refrain from bypassing the Service’s software and/or "
 "technical hardware means, in particular the security systems."
 msgstr ""
+"The User agrees to refrain from bypassing the Service’s software and/or "
+"technical hardware means, in particular the security systems."
 
 #: wllegal/templates/legal/documents/tos.html:91
 msgid "Liability for Damage"
-msgstr ""
+msgstr "Liability for Damage"
 
 #: wllegal/templates/legal/documents/tos.html:93
 msgid ""
 "The User hereby renders it undisputed that the Provider shall not be liable "
 "for any damage caused to the User resulting from the use of the Service."
 msgstr ""
+"The User hereby renders it undisputed that the Provider shall not be liable "
+"for any damage caused to the User resulting from the use of the Service."
 
 #: wllegal/templates/legal/documents/tos.html:95
 msgid ""
 "If the User is an entrepreneur, it hereby expressly waives its right to "
 "compensation from the Provider for damage unintentionally caused by the "
 "Provider to the User through a breach of any obligation contained in these "
 "Terms of Service and/or resulting from the use of the Service."
 msgstr ""
+"If the User is an entrepreneur, it hereby expressly waives its right to "
+"compensation from the Provider for damage unintentionally caused by the "
+"Provider to the User through a breach of any obligation contained in these "
+"Terms of Service and/or resulting from the use of the Service."
 
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to the collecting, storage and processing of the "
 "Personal Data provided by the User to the administrator, who is the "
 "Provider, through the use of the Service; the User gives consent to the "
 "processing and use of the User’s Personal Data by the Provider, the "
 "Provider’s employees and/or the Provider’s authorised business partners. "
 "This consent is given as long as User does not remove their account from the "
 "Service."
 msgstr ""
+"Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
+"hereby gives consent to the collecting, storage and processing of the "
+"Personal Data provided by the User to the administrator, who is the "
+"Provider, through the use of the Service; the User gives consent to the "
+"processing and use of the User’s Personal Data by the Provider, the Provider’"
+"s employees and/or the Provider’s authorised business partners. This consent "
+"is given as long as User does not remove their account from the Service."
 
 #: wllegal/templates/legal/documents/tos.html:103
 #, python-format
 msgid ""
 "The purpose of the processing of Personal Data as determined by the Provider "
 "is the use of Personal Data for sending commercial communications to the "
 "subject of the data (the User) through electronic means under Act No. "
 "%(law_480_2004)s Coll., on certain services of the information society, as "
 "amended, and further for business needs of the Provider’s contractual "
 "partners and for statistical purposes of the Provider."
 msgstr ""
+"The purpose of the processing of Personal Data as determined by the Provider "
+"is the use of Personal Data for sending commercial communications to the "
+"subject of the data (the User) through electronic means under Act No. "
+"%(law_480_2004)s Coll., on certain services of the information society, as "
+"amended, and further for business needs of the Provider’s contractual "
+"partners and for statistical purposes of the Provider."
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "If the User directly and effectively informs the Provider of no longer "
 "wishing to receive business information from the Provider, the Provider "
 "shall refrain from sending further unsolicited business communications."
 msgstr ""
+"If the User directly and effectively informs the Provider of no longer "
+"wishing to receive business information from the Provider, the Provider "
+"shall refrain from sending further unsolicited business communications."
 
 #: wllegal/templates/legal/documents/tos.html:109
 #, python-format
 msgid ""
 "The User declares awareness of own rights under <a href=\"%(url_15)s"
 "\">Article 15</a> and <a href=\"%(url_17)s\">Article 17</a> of the GDPR and "
 "declares that all the Personal Data is accurate and true and has been "
 "provided voluntarily."
 msgstr ""
+"The User declares awareness of own rights under <a href=\"%(url_15)s\""
+">Article 15</a> and <a href=\"%(url_17)s\">Article 17</a> of the GDPR and "
+"declares that all the Personal Data is accurate and true and has been "
+"provided voluntarily."
 
 #: wllegal/templates/legal/documents/tos.html:111
 msgid ""
 "The Provider declares that it will collect Personal Data only in the extent "
 "necessary for meeting the above-specified purpose and process the Personal "
 "Data in accordance with the purpose for which it was collected. The "
 "Provider’s employees and other individuals who process the Personal Data on "
 "the basis of a contract with the Provider shall maintain confidentiality of "
 "the Personal Data, even after the termination of their employment or "
 "business relationship with the Provider."
 msgstr ""
+"The Provider declares that it will collect Personal Data only in the extent "
+"necessary for meeting the above-specified purpose and process the Personal "
+"Data in accordance with the purpose for which it was collected. The Provider’"
+"s employees and other individuals who process the Personal Data on the basis "
+"of a contract with the Provider shall maintain confidentiality of the "
+"Personal Data, even after the termination of their employment or business "
+"relationship with the Provider."
 
 #: wllegal/templates/legal/documents/tos.html:113
 msgid ""
 "The Provider declares that it will process the Personal Data by electronic "
 "means (automatically) via computer programs for which the Provider has "
 "secured the right of use, in particular the Service."
 msgstr ""
+"The Provider declares that it will process the Personal Data by electronic "
+"means (automatically) via computer programs for which the Provider has "
+"secured the right of use, in particular the Service."
 
 #: wllegal/templates/legal/documents/tos.html:115
 msgid ""
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
+"The User’s consent under this Article 5 of the Terms of Service constitutes "
+"a free and informed juridical act which concerns the consent of the subject "
+"of the data (the User) with processing of the Personal Data."
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr ""
+msgstr "Translations"
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
+"The Service organises translation into individual Projects, where the Owner "
+"is responsible for managing them and for specifying accurately the licence "
+"of the Project."
 
 #: wllegal/templates/legal/documents/tos.html:122
 msgid ""
 "Not specifying translation license means that the translations are available "
 "under same license as the given Project itself."
 msgstr ""
+"Not specifying the translation licence means that the translations are "
+"available under the same licence as the given Project itself."
 
 #: wllegal/templates/legal/documents/tos.html:124
 msgid ""
 "Should the Project opt in for the Translation Memory, license to use the "
 "translation is granted to all Translation Memory users."
 msgstr ""
+"Should the Project opt in for the Translation Memory, license to use the "
+"translation is granted to all Translation Memory users."
 
 #: wllegal/templates/legal/documents/tos.html:126
 msgid ""
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
+"The User agrees, upon contributing to a Project, to the licence the Project "
+"has specified."
 
 #: wllegal/templates/legal/documents/tos.html:128
 msgid ""
 "The User agrees to use of own name and e-mail as authorship in the VCS "
 "commits. The User understands that this grant is non revocable due to nature "
 "of the VCS."
 msgstr ""
+"The User agrees to use of own name and e-mail as authorship in the VCS "
+"commits. The User understands that this grant is non revocable due to nature "
+"of the VCS."
 
 #: wllegal/templates/legal/documents/tos.html:133
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
 msgstr ""
+"Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
+"electronic communication, as amended, the User is informed that the Service "
+"uses Cookies."
 
 #: wllegal/templates/legal/documents/tos.html:135
 msgid "The Service uses Cookies to personalise content."
-msgstr ""
+msgstr "The Service uses Cookies to personalise content."
 
 #: wllegal/templates/legal/documents/tos.html:138
 msgid "Governing Law"
-msgstr ""
+msgstr "Governing Law"
 
 #: wllegal/templates/legal/documents/tos.html:140
 msgid ""
 "These Terms of Service shall be governed by the laws of the Czech Republic "
 "with exclusion of conflict rules."
 msgstr ""
+"These Terms of Service shall be governed by the laws of the Czech Republic "
+"with exclusion of conflict rules."
 
 #: wllegal/templates/legal/documents/tos.html:142
 msgid ""
 "Any disputes arising on the basis of the Agreement and/or these Terms of "
 "Service shall be resolved by the court of the Czech republic having "
 "substantive and local jurisdiction."
 msgstr ""
+"Any disputes arising on the basis of the Agreement and/or these Terms of "
+"Service shall be resolved by the court of the Czech republic having "
+"substantive and local jurisdiction."
 
 #: wllegal/templates/legal/documents/tos.html:145
 msgid "Effect"
-msgstr ""
+msgstr "Effect"
 
 #: wllegal/templates/legal/documents/tos.html:147
 msgid ""
 "These Terms of Service shall come into force and effect on 1st September "
 "2017."
 msgstr ""
+"These Terms of Service shall come into force and effect on 1st September "
+"2017."
+
+#~ msgid "Reset all changes in the local repository"
+#~ msgstr "Reset all changes in the local repository"
+
+#~ msgid "Billing"
+#~ msgstr "Billing"
+
+#~ msgid "Current plan"
+#~ msgstr "Current plan"
+
+#~ msgid "Strings limit"
+#~ msgstr "Strings limit"
+
+#~ msgid "Unlimited"
+#~ msgstr "Unlimited"
+
+#~ msgid "Languages limit"
+#~ msgstr "Languages limit"
+
+#, fuzzy
+#~| msgid "Projects limit"
+#~ msgid "Component limit"
+#~ msgstr "Projects limit"
+
+#~ msgid "Projects limit"
+#~ msgstr "Projects limit"
+
+#~ msgid "%(price)s EUR / month"
+#~ msgstr "%(price)s EUR / month"
+
+#~ msgid "%(price)s EUR / year"
+#~ msgstr "%(price)s EUR / year"
+
+#, fuzzy
+#~| msgid ""
+#~| "The pricing is based on number of source strings and number of target "
+#~| "languages. The source string is a text unit defined in a translation "
+#~| "format, it can be word, sentence or a paragraph."
+#~ msgid ""
+#~ "Pricing is based on the number of source strings and target languages. "
+#~ "The source string is a text unit defined in a translation format, it can "
+#~ "be a word, sentence or paragraph."
+#~ msgstr ""
+#~ "The pricing is based on number of source strings and number of target "
+#~ "languages. The source string is a text unit defined in a translation "
+#~ "format, it can be word, sentence or a paragraph."
+
+#, fuzzy
+#~| msgid "Failed to process form!"
+#~ msgid "Payment card"
+#~ msgstr "Failed to process form!"
+
+#, fuzzy
+#~| msgid "Failed to process form!"
+#~ msgid "Payment error"
+#~ msgstr "Failed to process form!"
+
+#~ msgid "Repositories limit"
+#~ msgstr "Repositories limit"
```

### Comparing `wllegal-2023.1/wllegal/locale/lzh/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/lzh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/mk/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/zgh/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Michal Čihař <michal@cihar.com>, 2019.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2019-07-22 07:40+0000\n"
-"Last-Translator: Michal Čihař <michal@cihar.com>\n"
-"Language-Team: Macedonian <https://hosted.weblate.org/projects/weblate/"
-"hosted/mk/>\n"
-"Language: mk\n"
+"PO-Revision-Date: 2023-04-02 01:08+0000\n"
+"Last-Translator: ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ ZOUHIR DEHBI <zouhirdehbi56@gmail.com>\n"
+"Language-Team: Tamazight (Standard Moroccan) <https://hosted.weblate.org/"
+"projects/weblate/legal/zgh/>\n"
+"Language: zgh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n==1 || n%10==1 ? 0 : 1;\n"
-"X-Generator: Weblate 3.8-dev\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
-msgstr ""
+msgstr "ⴰⵙⵓⵔⵙ ⵙⴳ ⴽⵟⵓⴱⵕ 2020."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr ""
+msgstr "ⵜⵉⴹⴰⴼ ⵏ ⵜⵎⵓⵛⴰ ⵜⵉⵏⵉⵎⴰⵏⵉⵏ"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr ""
+msgstr "%(provider)s,ⵓⵟⵟⵓⵏ ⵏ ⵓⵣⵎⵎⴻⵎ. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
@@ -55,18 +56,16 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:25
-#, fuzzy
-#| msgid "Username or email"
 msgid "Name and e-mail address"
-msgstr "Корисничко име или е-пошта"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events"
@@ -360,18 +359,16 @@
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
-#, fuzzy
-#| msgid "Personal info"
 msgid "Personal Data"
-msgstr "Лични податоци"
+msgstr "ⵜⵉⵎⵓⵛⴰ ⵜⵓⴷⵎⴰⵡⴰⵏⵉⵏ"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -382,15 +379,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Проект"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
@@ -398,26 +395,24 @@
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
-#, fuzzy
-#| msgid "Translation notifications"
 msgid "Translation Memory"
-msgstr "Преведувачки известувања"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Корисник"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
@@ -565,15 +560,15 @@
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr "Превод"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -637,17 +632,7 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:147
 msgid ""
 "These Terms of Service shall come into force and effect on 1st September "
 "2017."
 msgstr ""
-
-#, fuzzy
-#~| msgid "Subject"
-#~ msgid "Component limit"
-#~ msgstr "Предмет"
-
-#, fuzzy
-#~| msgid "Subject"
-#~ msgid "Projects limit"
-#~ msgstr "Предмет"
```

### Comparing `wllegal-2023.1/wllegal/locale/ml/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ml/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/mr/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/mr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ms/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ms/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/my/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/my/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/nb/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/nl/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/nn/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/nn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/oc/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/oc/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/or/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/or/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/pa/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/pa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/pa_PK/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/pa_PK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/peo/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/peo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/pl/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ps/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ps/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/pt/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/pt_BR/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/pt_PT/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ro/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ro_MD/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ro_MD/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ru/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/sc/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/sc/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/si/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/sk/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/skr/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/uz/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2023-02-14 10:36+0000\n"
-"Last-Translator: پرویز قادر <mpqadir@gmail.com>\n"
-"Language-Team: Saraiki <https://hosted.weblate.org/projects/weblate/legal/"
-"skr/>\n"
-"Language: skr\n"
+"PO-Revision-Date: 2023-02-12 16:39+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Uzbek <https://hosted.weblate.org/projects/weblate/legal/uz/>"
+"\n"
+"Language: uz\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.16-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
@@ -33,15 +33,15 @@
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr "ذاتی ڈیٹا کنٹرولر"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:15
@@ -318,15 +318,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "کوکیاں"
+msgstr "Cookies"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -360,15 +360,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "ذاتی ڈیٹا"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
```

### Comparing `wllegal-2023.1/wllegal/locale/sl/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/sr_Latn/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,114 +1,108 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Domen <mitenem@outlook.com>, 2018, 2019.
-# anonymous <noreply@weblate.org>, 2019.
+# Nikola Perović <nikolaperovicccc@gmail.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate\n"
+"Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2022-01-07 02:39+0000\n"
-"Last-Translator: Matej U <mateju@src.gnome.org>\n"
-"Language-Team: Slovenian <https://hosted.weblate.org/projects/weblate/legal/"
-"sl/>\n"
-"Language: sl\n"
+"PO-Revision-Date: 2021-02-09 02:02+0000\n"
+"Last-Translator: Слободан Симић(Slobodan Simić) <slsimic@gmail.com>\n"
+"Language-Team: Serbian (latin) <https://hosted.weblate.org/projects/weblate/"
+"legal/sr_Latn/>\n"
+"Language: sr_Latn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n"
-"%100==4 ? 2 : 3;\n"
-"X-Generator: Weblate 4.10.1\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
+"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr ""
+msgstr "Podizvođači u skladu sa članom 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
-msgstr ""
+msgstr "Status od oktobra 2020."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
+"Usklađeni smo sa regulativom br. %(law_679_2016)s, „Opštom regulativom "
+"zaštite podataka“, poznatom i kao GDPR (GDPR). Ovaj dokument sadrži "
+"neophodne specifikacije."
 
 #: wllegal/templates/legal/documents/privacy.html:9
-#, fuzzy
-#| msgid "Version control"
 msgid "Personal Data Controller"
-msgstr "Nadzor različic"
+msgstr "Kontrolor ličnih podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr ""
+msgstr "%(provider)s, reg. br. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:17
-#, fuzzy
-#| msgid "Translation process"
 msgid "Personal Data processed by Weblate"
-msgstr "Postopek prevajanja"
+msgstr "Lični podaci koje Veblejt obrađuje"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:25
-#, fuzzy
-#| msgid "Name and e-mail"
 msgid "Name and e-mail address"
-msgstr "Ime in e-pošta"
+msgstr "Ime i adresa e-pošte"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:29
-#, fuzzy
-#| msgid "Password changed"
 msgid "Password in hashed form"
-msgstr "Geslo sem spremenil"
+msgstr "Lozinka u heširanom obliku"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr ""
+msgstr "IP adresa i naziv pregledača"
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:36
 msgid "Billing information"
-msgstr "Podatki obračunavanja"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "In case you purchase service from us, we collect additional billing "
 "information necessary for issuing an invoice"
 msgstr ""
 
@@ -142,18 +136,16 @@
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:52
-#, fuzzy
-#| msgid "Allow changes in the local repository"
 msgid "Access to the Personal Data"
-msgstr "Dovoli spremembe v lokalni shrambi"
+msgstr "Pristup ličnim podacima"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
 
@@ -163,44 +155,40 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:60
-#, fuzzy
-#| msgid "Failed to process form!"
 msgid "Payment processors."
-msgstr "Nismo uspeli obdelati obrazca!"
+msgstr "Obrađivači plaćanja."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
-msgstr ""
+msgstr "Svi lični podaci su smešteni u Evropskoj uniji."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 msgid "The Personal Data retention"
-msgstr ""
+msgstr "Povlačenje ličnih podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "Access log information might be collected for a longer period for the "
 "purpose of establishing, exercising or defending legal claims."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:71
-#, fuzzy
-#| msgid "Your profile"
 msgid "Your rights"
-msgstr "Vaš profil"
+msgstr "Vaša prava"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
 
@@ -221,25 +209,23 @@
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:81
 msgid "Order us to delete your Personal Data"
-msgstr ""
+msgstr "Zahtev da obrišemo vaše lične podatke"
 
 #: wllegal/templates/legal/documents/privacy.html:82
 msgid "Restrict the Personal Data processing"
-msgstr ""
+msgstr "Ograničite obradu ličnih podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:83
-#, fuzzy
-#| msgid "Languages processing"
 msgid "Object to processing"
-msgstr "Jeziki v obdelavi"
+msgstr "Predmet obrade"
 
 #: wllegal/templates/legal/documents/privacy.html:84
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
 
@@ -276,49 +262,45 @@
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 
 #: wllegal/templates/legal/documents/summary.html:9
 msgid "We use cookies to deliver our services."
-msgstr ""
+msgstr "Koristimo kolačiće da isporučimo naše usluge."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
-msgstr ""
+msgstr "Pogledaj verziju na engleskom"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
+"Dokument Uslova korišćenja je zvaničan na engleskom. Prevod je omogućen da "
+"vam olakša uvid."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:20
-#, fuzzy
-#| msgid "Description"
 msgid "Definitions"
-msgstr "Opis"
+msgstr "Definicije"
 
 #: wllegal/templates/legal/documents/tos.html:22
-#, fuzzy
-#| msgid "Terms of Service"
 msgid "In these Terms of Service:"
-msgstr "Pogoji storitev"
+msgstr "U ovim uslovima korišćenja:"
 
 #: wllegal/templates/legal/documents/tos.html:26
-#, fuzzy
-#| msgid "Advertisement"
 msgid "Agreement"
-msgstr "Oglas"
+msgstr "Sporazum"
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
@@ -341,115 +323,114 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "Piškotki"
+msgstr "Kolačići"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr ""
+msgstr "GDPR(GDPR)"
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
+"označava EU regulativu br. %(law_679_2016)s, „Opšta regulativa zaštite "
+"podataka“"
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
 msgstr "Licenca"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr "Ponudnik"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "Osebni podatki"
+msgstr "Lični podaci"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr "Lastnik"
+msgstr "Vlasnik"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
-msgstr ""
+msgstr "označava korisnika koji upravlja projektom"
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Projekt"
+msgstr "Projekat"
 
 #: wllegal/templates/legal/documents/tos.html:55
-#, fuzzy
-#| msgid ""
-#| "However, the following translation projects are available on this server:"
 msgid "means translation project operated on the Service"
-msgstr "Kakor koli, na strežniku so na voljo naslednji prevajalski projekti:"
+msgstr "označava projekat prevođenja obrađivan na Pružaocu usluga"
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "Storitev"
+msgstr "Servis"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
 msgid "Translation Memory"
-msgstr "Spomin prevodov"
+msgstr "Prevodilačka memorija"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Uporabnik"
+msgstr "Korisnik"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "VCS"
+msgstr "Sistem kontrole verzija"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
@@ -659,68 +640,66 @@
 
 #: wllegal/templates/legal/documents/tos.html:147
 msgid ""
 "These Terms of Service shall come into force and effect on 1st September "
 "2017."
 msgstr ""
 
-#~ msgid "Reset all changes in the local repository"
-#~ msgstr "Ponastavi vse spremembe v lokalni shrambi"
-
 #~ msgid "Billing"
-#~ msgstr "Zaračunavanje"
+#~ msgstr "Naplata"
 
-#~ msgid "Current plan"
-#~ msgstr "Trenutni načrt"
+#~ msgid "Choose the billing plan you want to update"
+#~ msgstr "Izaberite plan plaćanja koji želite da ažurirate"
+
+#~ msgid "Create new billing plan"
+#~ msgstr "Napravite novi plan plaćanja"
+
+#~ msgid "Create billing plan"
+#~ msgstr "Napravite plan plaćanja"
+
+#~ msgid "New billing plan"
+#~ msgstr "Novi plan plaćanja"
+
+#~ msgid "Please choose a hosting plan that fits the size of your project."
+#~ msgstr ""
+#~ "Molimo vas izaberite hosting plan koji odgovara veličini vašeg projekta."
+
+#~ msgid "Current billing status"
+#~ msgstr "Trenutni status plaćanja"
+
+#~ msgid "Too small for your project."
+#~ msgstr "Prviše mali za vaš projekat."
+
+#~ msgid "Too small"
+#~ msgstr "Previše mali"
 
-#~ msgid "Strings limit"
-#~ msgstr "Omejitev nizov"
+#~ msgid "Selected plan"
+#~ msgstr "Izabrani plan"
+
+#~ msgid "Current plan"
+#~ msgstr "Trenutni plan"
 
 #~ msgid "Unlimited"
-#~ msgstr "Neomejeno"
+#~ msgstr "Neograničen"
 
 #~ msgid "Languages limit"
-#~ msgstr "Omejitev jezikov"
+#~ msgstr "Limit jezika"
 
 #, fuzzy
 #~| msgid "Projects limit"
 #~ msgid "Component limit"
-#~ msgstr "Omejitev projektov"
+#~ msgstr "Limit projekata"
 
 #~ msgid "Projects limit"
-#~ msgstr "Omejitev projektov"
+#~ msgstr "Limit projekata"
 
 #~ msgid "%(price)s EUR / month"
-#~ msgstr "%(price)s EUR/mesec"
-
-#~ msgid "%(price)s EUR / year"
-#~ msgstr "%(price)s EUR/leto"
+#~ msgstr "%(price)s EUR/ mesečno"
 
-#, fuzzy
-#~| msgid ""
-#~| "The pricing is based on number of source strings and number of target "
-#~| "languages. The source string is a text unit defined in a translation "
-#~| "format, it can be word, sentence or a paragraph."
-#~ msgid ""
-#~ "Pricing is based on the number of source strings and target languages. "
-#~ "The source string is a text unit defined in a translation format, it can "
-#~ "be a word, sentence or paragraph."
-#~ msgstr ""
-#~ "Cena temelji na številu izvirnih nizov in številu ciljnih jezikov. "
-#~ "Izvirni niz je besedilna enota, opredeljena v prevajalski obliki; lahko "
-#~ "je beseda, poved ali odstavek."
+#~ msgid "%(price)s EUR including VAT"
+#~ msgstr "%(price)s EUR uključujući VAT"
 
-#, fuzzy
-#~| msgid "Failed to process form!"
-#~ msgid "Payment card"
-#~ msgstr "Nismo uspeli obdelati obrazca!"
-
-#, fuzzy
-#~| msgid "Failed to process form!"
-#~ msgid "Payment error"
-#~ msgstr "Nismo uspeli obdelati obrazca!"
-
-#~ msgid "Monthly"
-#~ msgstr "Mesečno"
+#~ msgid "%(price)s EUR / year"
+#~ msgstr "%(price)s EUR / godišnje"
 
 #~ msgid "Repositories limit"
-#~ msgstr "Omejitev shramb"
+#~ msgstr "Ograničenje skladišta"
```

### Comparing `wllegal-2023.1/wllegal/locale/sq/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/sr/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/sr_Latn/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/th/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,98 +1,99 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Nikola Perović <nikolaperovicccc@gmail.com>, 2019.
+# Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2021-02-09 02:02+0000\n"
-"Last-Translator: Слободан Симић(Slobodan Simić) <slsimic@gmail.com>\n"
-"Language-Team: Serbian (latin) <https://hosted.weblate.org/projects/weblate/"
-"legal/sr_Latn/>\n"
-"Language: sr_Latn\n"
+"PO-Revision-Date: 2022-04-05 12:11+0000\n"
+"Last-Translator: TopTheWorst <topbkk57@gmail.com>\n"
+"Language-Team: Thai <https://hosted.weblate.org/projects/weblate/legal/th/>\n"
+"Language: th\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.5-dev\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 4.12-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr "Podizvođači u skladu sa članom 28 GDPR"
+msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
-msgstr "Status od oktobra 2020."
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
-"Usklađeni smo sa regulativom br. %(law_679_2016)s, „Opštom regulativom "
-"zaštite podataka“, poznatom i kao GDPR (GDPR). Ovaj dokument sadrži "
-"neophodne specifikacije."
 
 #: wllegal/templates/legal/documents/privacy.html:9
+#, fuzzy
+#| msgid "Versions"
 msgid "Personal Data Controller"
-msgstr "Kontrolor ličnih podataka"
+msgstr "รุ่น"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s, reg. br. %(reg_no)s"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
+"Weblate ได้แต่งตั้งเจ้าหน้าที่คุ้มครองข้อมูล โดยสามารถติดต่อได้ผ่าน "
+"%(privacy_contact)s"
 
 #: wllegal/templates/legal/documents/privacy.html:17
+#, fuzzy
+#| msgid "Administration"
 msgid "Personal Data processed by Weblate"
-msgstr "Lični podaci koje Veblejt obrađuje"
+msgstr "การดูแลระบบ"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
-msgstr "Ime i adresa e-pošte"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr "Lozinka u heširanom obliku"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr "IP adresa i naziv pregledača"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen"
 msgstr ""
 
@@ -137,15 +138,15 @@
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
-msgstr "Pristup ličnim podacima"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
 
@@ -156,23 +157,23 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors."
-msgstr "Obrađivači plaćanja."
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
-msgstr "Svi lični podaci su smešteni u Evropskoj uniji."
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 msgid "The Personal Data retention"
-msgstr "Povlačenje ličnih podataka"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 
@@ -180,15 +181,15 @@
 msgid ""
 "Access log information might be collected for a longer period for the "
 "purpose of establishing, exercising or defending legal claims."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "Your rights"
-msgstr "Vaša prava"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
 
@@ -209,23 +210,25 @@
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:81
 msgid "Order us to delete your Personal Data"
-msgstr "Zahtev da obrišemo vaše lične podatke"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:82
 msgid "Restrict the Personal Data processing"
-msgstr "Ograničite obradu ličnih podataka"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:83
+#, fuzzy
+#| msgid "Language"
 msgid "Object to processing"
-msgstr "Predmet obrade"
+msgstr "ภาษา"
 
 #: wllegal/templates/legal/documents/privacy.html:84
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
 
@@ -262,45 +265,45 @@
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 
 #: wllegal/templates/legal/documents/summary.html:9
 msgid "We use cookies to deliver our services."
-msgstr "Koristimo kolačiće da isporučimo naše usluge."
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
-msgstr "Pogledaj verziju na engleskom"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
-"Dokument Uslova korišćenja je zvaničan na engleskom. Prevod je omogućen da "
-"vam olakša uvid."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:20
+#, fuzzy
+#| msgid "Description"
 msgid "Definitions"
-msgstr "Definicije"
+msgstr "คำอธิบาย"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
-msgstr "U ovim uslovima korišćenja:"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
-msgstr "Sporazum"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
@@ -323,39 +326,37 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "Kolačići"
+msgstr "คุกกี้"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr "GDPR(GDPR)"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
-"označava EU regulativu br. %(law_679_2016)s, „Opšta regulativa zaštite "
-"podataka“"
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr "Licenca"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
@@ -366,71 +367,75 @@
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
+#, fuzzy
+#| msgid "Personal info"
 msgid "Personal Data"
-msgstr "Lični podaci"
+msgstr "ข้อมูลส่วนบุคคล"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr "Vlasnik"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
-msgstr "označava korisnika koji upravlja projektom"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Projekat"
+msgstr "โครงการ"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
-msgstr "označava projekat prevođenja obrađivan na Pružaocu usluga"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "Servis"
+msgstr "บริการ"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
+#, fuzzy
+#| msgid "Administration"
 msgid "Translation Memory"
-msgstr "Prevodilačka memorija"
+msgstr "การดูแลระบบ"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Korisnik"
+msgstr "ผู้ใช้"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "Sistem kontrole verzija"
+msgstr "VCS"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
@@ -567,15 +572,15 @@
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr "Prevodi"
+msgstr "การแปล"
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -640,66 +645,11 @@
 
 #: wllegal/templates/legal/documents/tos.html:147
 msgid ""
 "These Terms of Service shall come into force and effect on 1st September "
 "2017."
 msgstr ""
 
-#~ msgid "Billing"
-#~ msgstr "Naplata"
-
-#~ msgid "Choose the billing plan you want to update"
-#~ msgstr "Izaberite plan plaćanja koji želite da ažurirate"
-
-#~ msgid "Create new billing plan"
-#~ msgstr "Napravite novi plan plaćanja"
-
-#~ msgid "Create billing plan"
-#~ msgstr "Napravite plan plaćanja"
-
-#~ msgid "New billing plan"
-#~ msgstr "Novi plan plaćanja"
-
-#~ msgid "Please choose a hosting plan that fits the size of your project."
-#~ msgstr ""
-#~ "Molimo vas izaberite hosting plan koji odgovara veličini vašeg projekta."
-
-#~ msgid "Current billing status"
-#~ msgstr "Trenutni status plaćanja"
-
-#~ msgid "Too small for your project."
-#~ msgstr "Prviše mali za vaš projekat."
-
-#~ msgid "Too small"
-#~ msgstr "Previše mali"
-
-#~ msgid "Selected plan"
-#~ msgstr "Izabrani plan"
-
-#~ msgid "Current plan"
-#~ msgstr "Trenutni plan"
-
-#~ msgid "Unlimited"
-#~ msgstr "Neograničen"
-
-#~ msgid "Languages limit"
-#~ msgstr "Limit jezika"
-
 #, fuzzy
-#~| msgid "Projects limit"
-#~ msgid "Component limit"
-#~ msgstr "Limit projekata"
-
-#~ msgid "Projects limit"
-#~ msgstr "Limit projekata"
-
-#~ msgid "%(price)s EUR / month"
-#~ msgstr "%(price)s EUR/ mesečno"
-
-#~ msgid "%(price)s EUR including VAT"
-#~ msgstr "%(price)s EUR uključujući VAT"
-
-#~ msgid "%(price)s EUR / year"
-#~ msgstr "%(price)s EUR / godišnje"
-
-#~ msgid "Repositories limit"
-#~ msgstr "Ograničenje skladišta"
+#~| msgid "Language"
+#~ msgid "Languages limit"
+#~ msgstr "ภาษา"
```

### Comparing `wllegal-2023.1/wllegal/locale/sv/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/sw/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/ta/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ta/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/te/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/te/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/th/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/cy/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,123 +1,128 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Michal Čihař <michal@cihar.com>, 2019.
+# Weblate <noreply@weblate.org>, 2019.
+# anonymous <noreply@weblate.org>, 2019.
+# Rhoslyn Prys <rprys@posteo.net>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2022-04-05 12:11+0000\n"
-"Last-Translator: TopTheWorst <topbkk57@gmail.com>\n"
-"Language-Team: Thai <https://hosted.weblate.org/projects/weblate/legal/th/>\n"
-"Language: th\n"
+"PO-Revision-Date: 2023-04-23 20:04+0000\n"
+"Last-Translator: dreigiau <sterilgrimed23@gmail.com>\n"
+"Language-Team: Welsh <https://hosted.weblate.org/projects/weblate/legal/cy/>"
+"\n"
+"Language: cy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.12-dev\n"
+"Plural-Forms: nplurals=6; plural=(n==0) ? 0 : (n==1) ? 1 : (n==2) ? 2 : "
+"(n==3) ? 3 :(n==6) ? 4 : 5;\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
-msgstr ""
+msgstr "Statws ym mis Hydref 2020."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
-#, fuzzy
-#| msgid "Versions"
 msgid "Personal Data Controller"
-msgstr "รุ่น"
+msgstr "Rheolydd Data Personol"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr ""
+msgstr "%(provider)s, Reg. No. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
-"Weblate ได้แต่งตั้งเจ้าหน้าที่คุ้มครองข้อมูล โดยสามารถติดต่อได้ผ่าน "
-"%(privacy_contact)s"
+"Mae Weblate wedi penodi swyddog diogelu data y gellir ei gyrraedd trwy "
+"%(privacy_contact)s."
 
 #: wllegal/templates/legal/documents/privacy.html:17
-#, fuzzy
-#| msgid "Administration"
 msgid "Personal Data processed by Weblate"
-msgstr "การดูแลระบบ"
+msgstr "Data Personol wedi'i brosesu gan Weblate"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
+"Mae Weblate yn prosesu Data Personol y mae'r Defnyddiwr yn ei ddarparu trwy "
+"ei ddefnyddio:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
-msgstr ""
+msgstr "Enw a chyfeiriad e-bost"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits"
-msgstr ""
+msgstr "Defnyddir y rhain i'ch adnabod yn yr ymrwymiadau VCS"
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events"
-msgstr ""
+msgstr "Yn ogystal, defnyddir e-bost ar gyfer hysbysu am ddigwyddiadau a wylir"
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr ""
+msgstr "Cyfrinair ar ffurf hash"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
-msgstr ""
+msgstr "Fe'i defnyddir i ddilysu'r Defnyddiwr, os ffurfweddir"
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
-msgstr ""
+msgstr "Storir cyfrineiriau ar ffurf hash gan ddefnyddio Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr ""
+msgstr "Cyfeiriad IP ac enw porwr"
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen"
 msgstr ""
+"Mae'r rhain wedi'u logio rhag ofn y bydd newidiadau pwysig i'ch cyfrif (e.e. "
+"newid cyfrinair) i ganiatáu diagnosis rhag ofn i'ch cyfrif gael ei ddwyn"
 
 #: wllegal/templates/legal/documents/privacy.html:36
 msgid "Billing information"
-msgstr ""
+msgstr "bilio gwybodaeth"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "In case you purchase service from us, we collect additional billing "
 "information necessary for issuing an invoice"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
-msgstr ""
+msgstr "Pwrpas a sail gyfreithiol prosesu Data Personol"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
 msgstr ""
+"Bydd eich Data Personol yn cael ei ddefnyddio at ddibenion y Gwasanaeth:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
@@ -138,15 +143,15 @@
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
-msgstr ""
+msgstr "Mynediad i'r Data Personol"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
 
@@ -217,18 +222,16 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:82
 msgid "Restrict the Personal Data processing"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:83
-#, fuzzy
-#| msgid "Language"
 msgid "Object to processing"
-msgstr "ภาษา"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:84
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
 
@@ -284,18 +287,16 @@
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:20
-#, fuzzy
-#| msgid "Description"
 msgid "Definitions"
-msgstr "คำอธิบาย"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
@@ -326,15 +327,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "คุกกี้"
+msgstr "Cwcis"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -348,15 +349,15 @@
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr ""
+msgstr "Trwydded"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
@@ -367,18 +368,16 @@
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
-#, fuzzy
-#| msgid "Personal info"
 msgid "Personal Data"
-msgstr "ข้อมูลส่วนบุคคล"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -389,42 +388,40 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "โครงการ"
+msgstr "Prosiect"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "บริการ"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
-#, fuzzy
-#| msgid "Administration"
 msgid "Translation Memory"
-msgstr "การดูแลระบบ"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "ผู้ใช้"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
@@ -572,15 +569,15 @@
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr "การแปล"
+msgstr "Cyfieithiadau"
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -645,11 +642,9 @@
 
 #: wllegal/templates/legal/documents/tos.html:147
 msgid ""
 "These Terms of Service shall come into force and effect on 1st September "
 "2017."
 msgstr ""
 
-#, fuzzy
-#~| msgid "Language"
-#~ msgid "Languages limit"
-#~ msgstr "ภาษา"
+#~ msgid "Billing"
+#~ msgstr "Bilio"
```

### Comparing `wllegal-2023.1/wllegal/locale/tlh/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/tlh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/tok/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/tt/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: tok\n"
+"Language: tt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
```

### Comparing `wllegal-2023.1/wllegal/locale/tr/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/tt/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/tzm/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate\n"
+"Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: tt\n"
+"PO-Revision-Date: 2021-01-28 08:55+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Tamazight (Central Atlas) <https://hosted.weblate.org/"
+"projects/weblate/legal/tzm/>\n"
+"Language: tzm\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n >= 2 && (n < 11 || n > 99);\n"
+"X-Generator: Weblate 4.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
@@ -326,26 +329,26 @@
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr ""
+msgstr "GDPR"
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr ""
+msgstr "Turagt"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
@@ -368,31 +371,31 @@
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr ""
+msgstr "Bab"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr ""
+msgstr "Asefaṛ"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr ""
+msgstr "Tanafut"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
@@ -401,26 +404,26 @@
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr ""
+msgstr "Anessemres"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr ""
+msgstr "VCS"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
@@ -557,15 +560,15 @@
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr ""
+msgstr "Tisuɣal"
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
```

### Comparing `wllegal-2023.1/wllegal/locale/tzm/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/tok/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2021-01-28 08:55+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Tamazight (Central Atlas) <https://hosted.weblate.org/"
-"projects/weblate/legal/tzm/>\n"
-"Language: tzm\n"
+"PO-Revision-Date: 2023-04-28 16:51+0000\n"
+"Last-Translator: Sena <jn-sena@proton.me>\n"
+"Language-Team: Toki Pona <https://hosted.weblate.org/projects/weblate/legal/"
+"tok/>\n"
+"Language: tok\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n >= 2 && (n < 11 || n > 99);\n"
-"X-Generator: Weblate 4.5-dev\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
@@ -329,26 +329,26 @@
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr "GDPR"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr "Turagt"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
@@ -360,42 +360,42 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr ""
+msgstr "sona jan"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr "Bab"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Asefaṛ"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "Tanafut"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
@@ -404,26 +404,26 @@
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Anessemres"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "VCS"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
@@ -560,15 +560,15 @@
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr "Tisuɣal"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
```

### Comparing `wllegal-2023.1/wllegal/locale/ug/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/ug/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/uk/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/uz/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/yue_Hant/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2023-02-12 16:39+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Uzbek <https://hosted.weblate.org/projects/weblate/legal/uz/>"
-"\n"
-"Language: uz\n"
+"PO-Revision-Date: 2022-08-21 08:34+0000\n"
+"Last-Translator: Ray <ray.cfu@protonmail.com>\n"
+"Language-Team: Yue <https://hosted.weblate.org/projects/weblate/legal/yue/>\n"
+"Language: yue\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 4.14-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
@@ -318,15 +317,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "Cookies"
+msgstr "Cookie"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
```

### Comparing `wllegal-2023.1/wllegal/locale/vi/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/yue/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/skr/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,115 +4,116 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2021-09-22 06:40+0000\n"
-"PO-Revision-Date: 2022-08-21 08:34+0000\n"
-"Last-Translator: Ray <ray.cfu@protonmail.com>\n"
-"Language-Team: Yue <https://hosted.weblate.org/projects/weblate/legal/yue/>\n"
-"Language: yue\n"
+"PO-Revision-Date: 2023-04-01 00:26+0000\n"
+"Last-Translator: پرویز قادر <mpqadir@gmail.com>\n"
+"Language-Team: Saraiki <https://hosted.weblate.org/projects/weblate/legal/"
+"skr/>\n"
+"Language: skr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.14-dev\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of October 2020."
-msgstr ""
+msgstr "اکتوبر ٢٠٢٠دا سٹیٹس۔"
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr ""
+msgstr "ذاتی ڈیٹا کنٹرولر"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr ""
+msgstr "%(provider)s، رجصٹڑیشن نمبر %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
-msgstr ""
+msgstr "Weblate ولوں عمل تھیا ذاتی ڈیٹا"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
-msgstr ""
+msgstr "ناں تے ای میل پتہ"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr ""
+msgstr "ہیش تھئی شکل وچ پاس ورڈ"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr ""
+msgstr "آئی پی پتہ تے براؤزر ناں"
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:36
 msgid "Billing information"
-msgstr ""
+msgstr "ٻلنگ معلومات"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "In case you purchase service from us, we collect additional billing "
 "information necessary for issuing an invoice"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr ""
+msgstr "تہاݙا ذاتی ڈیٹا ایں خدمت دے مقصد کیتے ورتیا ویسی:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
@@ -133,15 +134,15 @@
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
-msgstr ""
+msgstr "ذاتی ڈیٹا تے رسائی"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
 
@@ -152,23 +153,23 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors."
-msgstr ""
+msgstr "ادائیگی دے پراسیسر۔"
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
-msgstr ""
+msgstr "سارا ذاتی ڈیٹا یورپی یونین وچ سٹور تھیندا ہے۔"
 
 #: wllegal/templates/legal/documents/privacy.html:65
 msgid "The Personal Data retention"
-msgstr ""
+msgstr "ذاتی ڈیٹا دی بقا"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 
@@ -176,15 +177,15 @@
 msgid ""
 "Access log information might be collected for a longer period for the "
 "purpose of establishing, exercising or defending legal claims."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "Your rights"
-msgstr ""
+msgstr "تہاݙے حقوق"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
 
@@ -205,15 +206,15 @@
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:81
 msgid "Order us to delete your Personal Data"
-msgstr ""
+msgstr "آپݨا ذاتی ڈیٹا مٹاوݨ کیتے ساکوں حکم ݙیوو"
 
 #: wllegal/templates/legal/documents/privacy.html:82
 msgid "Restrict the Personal Data processing"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:83
 msgid "Object to processing"
@@ -258,19 +259,19 @@
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 
 #: wllegal/templates/legal/documents/summary.html:9
 msgid "We use cookies to deliver our services."
-msgstr ""
+msgstr "اساں آپݨیاں خدمتاں حوالے کرݨ کیتے کوکیاں ورتیندے ہیں۔"
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
-msgstr ""
+msgstr "انگریزی ورشن ݙیکھو"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
 
@@ -278,171 +279,171 @@
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:20
 msgid "Definitions"
-msgstr ""
+msgstr "تعریفاں"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
-msgstr ""
+msgstr "انہاں خدمت شرطاں وچ:"
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
-msgstr ""
+msgstr "معاہدہ"
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:29
 msgid "Civil Code"
-msgstr ""
+msgstr "سول کوڈ"
 
 #: wllegal/templates/legal/documents/tos.html:30
 #, python-format
 msgid "means Act No. %(law_89_2012)s Coll., the Civil Code, as amended"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:32
 msgid "Consent"
-msgstr ""
+msgstr "رضامندی"
 
 #: wllegal/templates/legal/documents/tos.html:33
 msgid ""
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:131
 msgid "Cookies"
-msgstr "Cookie"
+msgstr "کوکیاں"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr ""
+msgstr "جی ڈی پی آر"
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr ""
+msgstr "لائسنس"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr ""
+msgstr "پرووائیڈر"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr ""
+msgstr "ذاتی ڈیٹا"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr ""
+msgstr "مالک"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr ""
+msgstr "منصوبہ"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr ""
+msgstr "خدمت"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
 msgid "Translation Memory"
-msgstr ""
+msgstr "ترجمہ یادداشت"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr ""
+msgstr "ورتݨ آلا"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr ""
+msgstr "وی سی ایس"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:71
 msgid "License Agreement Conclusion"
-msgstr ""
+msgstr "لائسنس معاہدہ نتیجہ"
 
 #: wllegal/templates/legal/documents/tos.html:73
 msgid ""
 "The License Agreement is concluded upon the User’s Acceptance of the "
 "Provider’s Offer."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:76
 msgid "License Agreement"
-msgstr ""
+msgstr "لائسنس معاہدہ"
 
 #: wllegal/templates/legal/documents/tos.html:78
 msgid ""
 "By concluding Agreement under Article 2.1 of this Agreement, the following "
 "provisions of this Article 3 of the Terms of Service come into force."
 msgstr ""
 
@@ -476,15 +477,15 @@
 msgid ""
 "The User agrees to refrain from bypassing the Service’s software and/or "
 "technical hardware means, in particular the security systems."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:91
 msgid "Liability for Damage"
-msgstr ""
+msgstr "نقصان دی ذمے واری"
 
 #: wllegal/templates/legal/documents/tos.html:93
 msgid ""
 "The User hereby renders it undisputed that the Provider shall not be liable "
 "for any damage caused to the User resulting from the use of the Service."
 msgstr ""
 
@@ -559,15 +560,15 @@
 "The User’s consent under this Article 5 of the Terms of Service constitutes "
 "a free and informed juridical act which concerns the consent of the subject "
 "of the data (the User) with processing of the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:118
 msgid "Translations"
-msgstr ""
+msgstr "ترجمے"
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -603,19 +604,19 @@
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:135
 msgid "The Service uses Cookies to personalise content."
-msgstr ""
+msgstr "مواد کوں ذاتی بݨاوݨ کیتے ایہ خدمت کوکیاں ورتیندی ہے۔"
 
 #: wllegal/templates/legal/documents/tos.html:138
 msgid "Governing Law"
-msgstr ""
+msgstr "گورننگ قنون"
 
 #: wllegal/templates/legal/documents/tos.html:140
 msgid ""
 "These Terms of Service shall be governed by the laws of the Czech Republic "
 "with exclusion of conflict rules."
 msgstr ""
 
@@ -624,14 +625,14 @@
 "Any disputes arising on the basis of the Agreement and/or these Terms of "
 "Service shall be resolved by the court of the Czech republic having "
 "substantive and local jurisdiction."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:145
 msgid "Effect"
-msgstr ""
+msgstr "اثر"
 
 #: wllegal/templates/legal/documents/tos.html:147
 msgid ""
 "These Terms of Service shall come into force and effect on 1st September "
 "2017."
-msgstr ""
+msgstr "خدمت شرطاں یکم ستمبر ٢٠١٧ کوں لاگو تھیسن تے مؤثر ہوسن۔"
```

### Comparing `wllegal-2023.1/wllegal/locale/zh_Hans/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/locale/zh_Hant/LC_MESSAGES/django.po` & `wllegal-2023.2/wllegal/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/templates/legal/documents/privacy.html` & `wllegal-2023.2/wllegal/templates/legal/documents/privacy.html`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 <p>
 {% trans "Weblate only processes Personal Data the User provides by using it:" %}
 </p>
 
 <dl>
 
 <dt>{% trans "Name and e-mail address" %}</dt>
-<dd>{% trans "These are used to identify you in the VCS commits" %}</dd>
-<dd>{% trans "Additionally, e-mail is used for notification of watched events" %}</dd>
+<dd>{% trans "These are used to identify you in the VCS commits." %}</dd>
+<dd>{% trans "Additionally, e-mail is used for notification of watched events." %}</dd>
 
 <dt>{% trans "Password in hashed form" %}</dt>
 <dd>{% trans "Used to authenticate the User, if configured" %}</dd>
 <dd>{% trans "Passwords are stored hashed using Argon2." %}</dd>
 
 <dt>{% trans "IP address and browser name" %}</dt>
-<dd>{% trans "These are logged in case of important changes to your account (e.g. password change) to allow diagnosis in case your account is stolen" %}</dd>
+<dd>{% trans "These are logged in case of important changes to your account (e.g. password change) to allow diagnosis in case your account is stolen." %}</dd>
 
-<dt>{% trans "Billing information" %}</dt>
-<dd>{% trans "In case you purchase service from us, we collect additional billing information necessary for issuing an invoice" %}</dd>
+<dt>{% trans "Billing info" %}</dt>
+<dd>{% trans "Necessary details to issue an invoice is collected when purchasing a service from us." %}</dd>
 
 </dl>
 
 <h2>{% blocktrans %}Purpose and legal basis of processing Personal Data{% endblocktrans %}</h2>
 
 <p>{% blocktrans %}Your Personal Data will be used for the purposes of the Service:{% endblocktrans %}</p>
 
@@ -62,15 +62,15 @@
 
 <p>{% blocktrans %}All Personal Data is stored in the European Union.{% endblocktrans %}</p>
 
 <h2>{% blocktrans %}The Personal Data retention{% endblocktrans %}</h2>
 
 <p>{% blocktrans %}The Personal Data is stored in the Service until the User deletes their account on the service.{% endblocktrans %}</p>
 
-<p>{% blocktrans %}Access log information might be collected for a longer period for the purpose of establishing, exercising or defending legal claims.{% endblocktrans %}</p>
+<p>{% blocktrans %}Access log info might be collected for a longer period for the purpose of establishing, exercising or defending legal claims.{% endblocktrans %}</p>
 
 <h2 id="rights">{% blocktrans %}Your rights{% endblocktrans %}</h2>
 
 <p>{% blocktrans %}The User provides use of Personal Data voluntarily. Without this Personal Data Weblate is not able to provide our services.{% endblocktrans %}</p>
 
 <p>{% blocktrans %}We want you to always be in control of your Personal Data. To this end, you have certain rights that allow for it. Under certain conditions, you may:{% endblocktrans %}</p>
```

#### html2text {}

```diff
@@ -11,27 +11,27 @@
 appointed a data protection officer who may be reached via {{privacy_contact}}.
 {% endblocktrans %}
 ***** {% blocktrans %}Personal Data processed by Weblate{% endblocktrans %}
 *****
 {% trans "Weblate only processes Personal Data the User provides by using it:
 " %}
   {% trans "Name and e-mail address" %}
-      {% trans "These are used to identify you in the VCS commits" %}
+      {% trans "These are used to identify you in the VCS commits." %}
       {% trans "Additionally, e-mail is used for notification of watched
-      events" %}
+      events." %}
   {% trans "Password in hashed form" %}
       {% trans "Used to authenticate the User, if configured" %}
       {% trans "Passwords are stored hashed using Argon2." %}
   {% trans "IP address and browser name" %}
       {% trans "These are logged in case of important changes to your account
-      (e.g. password change) to allow diagnosis in case your account is stolen"
-      %}
-  {% trans "Billing information" %}
-      {% trans "In case you purchase service from us, we collect additional
-      billing information necessary for issuing an invoice" %}
+      (e.g. password change) to allow diagnosis in case your account is
+      stolen." %}
+  {% trans "Billing info" %}
+      {% trans "Necessary details to issue an invoice is collected when
+      purchasing a service from us." %}
 ***** {% blocktrans %}Purpose and legal basis of processing Personal Data{%
 endblocktrans %} *****
 {% blocktrans %}Your Personal Data will be used for the purposes of the
 Service:{% endblocktrans %}
     * {% law_url 6 scope="GDPR" as url %}
     * {% blocktrans %}for providing our services on the Service, to contact you
       in matters regarding our services (also by means of e-mails and
@@ -53,17 +53,17 @@
       the service.{% endblocktrans %}
     * {% blocktrans %}Payment processors.{% endblocktrans %}
 {% blocktrans %}All Personal Data is stored in the European Union.{%
 endblocktrans %}
 ***** {% blocktrans %}The Personal Data retention{% endblocktrans %} *****
 {% blocktrans %}The Personal Data is stored in the Service until the User
 deletes their account on the service.{% endblocktrans %}
-{% blocktrans %}Access log information might be collected for a longer period
-for the purpose of establishing, exercising or defending legal claims.{%
-endblocktrans %}
+{% blocktrans %}Access log info might be collected for a longer period for the
+purpose of establishing, exercising or defending legal claims.{% endblocktrans
+%}
 ***** {% blocktrans %}Your rights{% endblocktrans %} *****
 {% blocktrans %}The User provides use of Personal Data voluntarily. Without
 this Personal Data Weblate is not able to provide our services.{% endblocktrans
 %}
 {% blocktrans %}We want you to always be in control of your Personal Data. To
 this end, you have certain rights that allow for it. Under certain conditions,
 you may:{% endblocktrans %}
```

### Comparing `wllegal-2023.1/wllegal/templates/legal/documents/tos.html` & `wllegal-2023.2/wllegal/templates/legal/documents/tos.html`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/templates/security.txt` & `wllegal-2023.2/wllegal/templates/security.txt`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/templates/weblate_503.html` & `wllegal-2023.2/wllegal/templates/weblate_503.html`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal/templates/weblate_50x.html` & `wllegal-2023.2/wllegal/templates/weblate_50x.html`

 * *Files identical despite different names*

### Comparing `wllegal-2023.1/wllegal.egg-info/PKG-INFO` & `wllegal-2023.2/wllegal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wllegal
-Version: 2023.1
+Version: 2023.2
 Summary: Hosted Weblate legal stuff
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/wllegal
 Author: Michal Čihař
 Author-email: michal@cihar.com
 License: GPL-3.0-or-later
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/wllegal/issues
@@ -26,24 +26,24 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
    :alt: Weblate
    :target: https://weblate.org/
    :height: 80px
 
-**Weblate is a copylefted libre software web-based continuous localization system,
+**Weblate is libre software web-based continuous localization system,
 used by over 2500 libre projects and companies in more than 165 countries.**
 
 
 This is legal module used on the `Hosted Weblate service
 <https://weblate.org/hosting/>`_.
 
 You can use them as an example how to customize `Weblate
```

### Comparing `wllegal-2023.1/wllegal.egg-info/SOURCES.txt` & `wllegal-2023.2/wllegal.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 wllegal/locale/ang/LC_MESSAGES/django.po
 wllegal/locale/ar/LC_MESSAGES/django.po
 wllegal/locale/ar_LY/LC_MESSAGES/django.po
 wllegal/locale/ars/LC_MESSAGES/django.po
 wllegal/locale/ast/LC_MESSAGES/django.po
 wllegal/locale/az/LC_MESSAGES/django.po
 wllegal/locale/be/LC_MESSAGES/django.po
-wllegal/locale/be@latin/LC_MESSAGES/django.po
+wllegal/locale/be_Latn/LC_MESSAGES/django.po
 wllegal/locale/ber/LC_MESSAGES/django.po
 wllegal/locale/bg/LC_MESSAGES/django.po
 wllegal/locale/bn/LC_MESSAGES/django.po
 wllegal/locale/bn_BD/LC_MESSAGES/django.po
 wllegal/locale/bo/LC_MESSAGES/django.po
 wllegal/locale/br/LC_MESSAGES/django.po
 wllegal/locale/ca/LC_MESSAGES/django.po
@@ -118,15 +118,15 @@
 wllegal/locale/tr/LC_MESSAGES/django.po
 wllegal/locale/tt/LC_MESSAGES/django.po
 wllegal/locale/tzm/LC_MESSAGES/django.po
 wllegal/locale/ug/LC_MESSAGES/django.po
 wllegal/locale/uk/LC_MESSAGES/django.po
 wllegal/locale/uz/LC_MESSAGES/django.po
 wllegal/locale/vi/LC_MESSAGES/django.po
-wllegal/locale/yue/LC_MESSAGES/django.po
+wllegal/locale/yue_Hant/LC_MESSAGES/django.po
 wllegal/locale/zgh/LC_MESSAGES/django.po
 wllegal/locale/zh_Hans/LC_MESSAGES/django.po
 wllegal/locale/zh_Hant/LC_MESSAGES/django.po
 wllegal/templates/security.txt
 wllegal/templates/weblate_503.html
 wllegal/templates/weblate_50x.html
 wllegal/templates/legal/documents/contracts.html
```

