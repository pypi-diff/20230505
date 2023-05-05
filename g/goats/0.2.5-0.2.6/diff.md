# Comparing `tmp/goats-0.2.5.tar.gz` & `tmp/goats-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goats-0.2.5.tar", max compression
+gzip compressed data, was "goats-0.2.6.tar", max compression
```

## Comparing `goats-0.2.5.tar` & `goats-0.2.6.tar`

### file list

```diff
@@ -1,106 +1,36 @@
--rwxr-xr-x   0        0        0    35092 2021-12-16 18:46:50.226668 goats-0.2.5/LICENSE
--rw-r--r--   0        0        0     5763 2023-03-31 13:27:39.249957 goats-0.2.5/README.md
--rw-r--r--   0        0        0      891 2023-05-04 13:39:43.759096 goats-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      180 2023-03-31 13:27:39.253957 goats-0.2.5/src/goats/__init__.py
--rw-r--r--   0        0        0        0 2022-03-09 16:57:39.661704 goats-0.2.5/src/goats/core/__init__.py
--rw-r--r--   0        0        0      144 2022-03-09 16:59:28.059858 goats-0.2.5/src/goats/core/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    22130 2022-03-22 17:16:46.881022 goats-0.2.5/src/goats/core/__pycache__/_variable.cpython-38.pyc
--rw-r--r--   0        0        0    21994 2022-03-22 16:02:31.451964 goats-0.2.5/src/goats/core/__pycache__/_variable_dev.cpython-38.pyc
--rw-r--r--   0        0        0    48757 2022-07-01 20:52:22.023182 goats-0.2.5/src/goats/core/__pycache__/algebra.cpython-38.pyc
--rw-r--r--   0        0        0    14774 2022-11-10 16:11:39.965870 goats-0.2.5/src/goats/core/__pycache__/algebraic.cpython-38.pyc
--rw-r--r--   0        0        0    38829 2023-04-19 01:16:02.493983 goats-0.2.5/src/goats/core/__pycache__/aliased.cpython-38.pyc
--rw-r--r--   0        0        0     8386 2022-03-10 15:11:47.686199 goats-0.2.5/src/goats/core/__pycache__/arrays.cpython-38.pyc
--rw-r--r--   0        0        0     5943 2023-04-19 01:16:02.509983 goats-0.2.5/src/goats/core/__pycache__/axis.cpython-38.pyc
--rw-r--r--   0        0        0     9827 2022-07-27 17:26:43.898490 goats-0.2.5/src/goats/core/__pycache__/base.cpython-38.pyc
--rw-r--r--   0        0        0     2170 2022-01-07 17:19:07.111938 goats-0.2.5/src/goats/core/__pycache__/basetypes.cpython-38.pyc
--rw-r--r--   0        0        0    16338 2022-11-22 17:36:06.196703 goats-0.2.5/src/goats/core/__pycache__/computable.cpython-38.pyc
--rw-r--r--   0        0        0    16292 2023-04-19 01:16:02.677982 goats-0.2.5/src/goats/core/__pycache__/computed.cpython-38.pyc
--rw-r--r--   0        0        0     3729 2023-04-19 01:16:02.689983 goats-0.2.5/src/goats/core/__pycache__/constant.cpython-38.pyc
--rw-r--r--   0        0        0     5189 2022-01-10 22:56:00.293599 goats-0.2.5/src/goats/core/__pycache__/constants.cpython-38.pyc
--rw-r--r--   0        0        0     6968 2022-01-18 23:56:53.599652 goats-0.2.5/src/goats/core/__pycache__/core.cpython-38.pyc
--rw-r--r--   0        0        0    12442 2022-11-21 14:51:28.746827 goats-0.2.5/src/goats/core/__pycache__/data.cpython-38.pyc
--rw-r--r--   0        0        0     9787 2022-11-17 22:41:35.409111 goats-0.2.5/src/goats/core/__pycache__/data_wip.cpython-38.pyc
--rw-r--r--   0        0        0    10730 2023-04-19 01:16:02.509983 goats-0.2.5/src/goats/core/__pycache__/datafile.cpython-38.pyc
--rw-r--r--   0        0        0    16991 2022-07-19 14:55:33.814895 goats-0.2.5/src/goats/core/__pycache__/dataset.cpython-38.pyc
--rw-r--r--   0        0        0     7253 2022-07-14 16:49:22.056633 goats-0.2.5/src/goats/core/__pycache__/datasets.cpython-38.pyc
--rw-r--r--   0        0        0    19522 2022-07-14 17:56:57.431202 goats-0.2.5/src/goats/core/__pycache__/datatypes.cpython-38.pyc
--rw-r--r--   0        0        0     8611 2021-12-16 21:31:48.045904 goats-0.2.5/src/goats/core/__pycache__/elements.cpython-38.pyc
--rw-r--r--   0        0        0    19068 2022-09-19 16:09:37.838562 goats-0.2.5/src/goats/core/__pycache__/function.cpython-38.pyc
--rw-r--r--   0        0        0    12864 2022-07-27 14:57:58.805104 goats-0.2.5/src/goats/core/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0        0        0    11294 2023-04-19 01:16:02.681983 goats-0.2.5/src/goats/core/__pycache__/fundamental.cpython-38.pyc
--rw-r--r--   0        0        0     6737 2023-04-19 01:16:02.521983 goats-0.2.5/src/goats/core/__pycache__/index.cpython-38.pyc
--rw-r--r--   0        0        0     5421 2022-07-15 14:27:32.568725 goats-0.2.5/src/goats/core/__pycache__/indexing.cpython-38.pyc
--rw-r--r--   0        0        0     5075 2022-09-20 17:28:55.057583 goats-0.2.5/src/goats/core/__pycache__/interpolated.cpython-38.pyc
--rw-r--r--   0        0        0     4118 2023-04-19 01:16:02.689983 goats-0.2.5/src/goats/core/__pycache__/interpolation.cpython-38.pyc
--rw-r--r--   0        0        0     7926 2022-11-10 16:11:39.805872 goats-0.2.5/src/goats/core/__pycache__/iotools.cpython-38.pyc
--rw-r--r--   0        0        0    65776 2023-04-19 01:16:02.501983 goats-0.2.5/src/goats/core/__pycache__/iterables.cpython-38.pyc
--rw-r--r--   0        0        0    16929 2023-04-19 01:16:02.673982 goats-0.2.5/src/goats/core/__pycache__/measurable.cpython-38.pyc
--rw-r--r--   0        0        0    31766 2022-04-06 20:23:37.149629 goats-0.2.5/src/goats/core/__pycache__/measurables.cpython-38.pyc
--rw-r--r--   0        0        0    36538 2022-04-08 14:09:59.622538 goats-0.2.5/src/goats/core/__pycache__/measured.cpython-38.pyc
--rw-r--r--   0        0        0    36552 2023-04-19 01:16:02.525983 goats-0.2.5/src/goats/core/__pycache__/metadata.cpython-38.pyc
--rw-r--r--   0        0        0    75499 2023-02-15 17:54:20.005897 goats-0.2.5/src/goats/core/__pycache__/metric.cpython-38.pyc
--rw-r--r--   0        0        0     8229 2022-11-10 16:11:39.813872 goats-0.2.5/src/goats/core/__pycache__/numerical.cpython-38.pyc
--rw-r--r--   0        0        0     5915 2022-11-22 17:36:06.264703 goats-0.2.5/src/goats/core/__pycache__/observable.cpython-38.pyc
--rw-r--r--   0        0        0     2171 2022-07-01 20:54:36.643243 goats-0.2.5/src/goats/core/__pycache__/observables.cpython-38.pyc
--rw-r--r--   0        0        0     3479 2023-04-19 01:16:02.701983 goats-0.2.5/src/goats/core/__pycache__/observed.cpython-38.pyc
--rw-r--r--   0        0        0     4548 2023-04-19 01:16:02.701983 goats-0.2.5/src/goats/core/__pycache__/observer.cpython-38.pyc
--rw-r--r--   0        0        0    19375 2023-04-19 01:16:02.705983 goats-0.2.5/src/goats/core/__pycache__/observing.cpython-38.pyc
--rw-r--r--   0        0        0     8003 2023-04-19 01:16:02.713982 goats-0.2.5/src/goats/core/__pycache__/operational.cpython-38.pyc
--rw-r--r--   0        0        0    38511 2022-06-28 21:57:39.878542 goats-0.2.5/src/goats/core/__pycache__/operations.cpython-38.pyc
--rw-r--r--   0        0        0    11659 2022-04-22 15:47:42.430493 goats-0.2.5/src/goats/core/__pycache__/operator.cpython-38.pyc
--rw-r--r--   0        0        0     7089 2022-04-19 16:26:49.203113 goats-0.2.5/src/goats/core/__pycache__/operators.cpython-38.pyc
--rw-r--r--   0        0        0     4139 2022-07-28 20:56:17.884099 goats-0.2.5/src/goats/core/__pycache__/parameter.cpython-38.pyc
--rw-r--r--   0        0        0    25100 2023-04-19 01:16:02.681983 goats-0.2.5/src/goats/core/__pycache__/physical.cpython-38.pyc
--rw-r--r--   0        0        0     2419 2022-11-10 16:11:40.509863 goats-0.2.5/src/goats/core/__pycache__/plasma.cpython-38.pyc
--rw-r--r--   0        0        0    31765 2022-04-06 20:13:29.693312 goats-0.2.5/src/goats/core/__pycache__/quantified.cpython-38.pyc
--rw-r--r--   0        0        0     3027 2022-07-20 22:48:20.145171 goats-0.2.5/src/goats/core/__pycache__/quantities.cpython-38.pyc
--rw-r--r--   0        0        0     2720 2023-04-19 01:16:02.509983 goats-0.2.5/src/goats/core/__pycache__/reference.cpython-38.pyc
--rw-r--r--   0        0        0     5546 2022-11-10 16:11:40.513863 goats-0.2.5/src/goats/core/__pycache__/spelling.cpython-38.pyc
--rw-r--r--   0        0        0    59951 2023-04-19 01:16:02.533983 goats-0.2.5/src/goats/core/__pycache__/symbolic.cpython-38.pyc
--rw-r--r--   0        0        0     4228 2023-04-19 01:16:02.665983 goats-0.2.5/src/goats/core/__pycache__/utilities.cpython-38.pyc
--rw-r--r--   0        0        0    26742 2023-04-19 01:16:02.669983 goats-0.2.5/src/goats/core/__pycache__/variable.cpython-38.pyc
--rw-r--r--   0        0        0    11231 2022-11-10 16:10:01.591199 goats-0.2.5/src/goats/core/algebraic.py
--rw-r--r--   0        0        0    34484 2023-03-31 13:27:39.253957 goats-0.2.5/src/goats/core/aliased.py
--rw-r--r--   0        0        0     5465 2023-03-31 13:27:39.253957 goats-0.2.5/src/goats/core/axis.py
--rw-r--r--   0        0        0    16025 2023-03-31 13:27:39.253957 goats-0.2.5/src/goats/core/computed.py
--rw-r--r--   0        0        0     3107 2023-03-31 13:27:39.253957 goats-0.2.5/src/goats/core/constant.py
--rw-r--r--   0        0        0     8617 2023-03-31 13:27:39.253957 goats-0.2.5/src/goats/core/datafile.py
--rw-r--r--   0        0        0    14395 2023-03-31 13:27:39.253957 goats-0.2.5/src/goats/core/fundamental.py
--rw-r--r--   0        0        0     5772 2023-03-31 22:32:43.725018 goats-0.2.5/src/goats/core/index.py
--rw-r--r--   0        0        0     4610 2023-03-31 13:27:39.253957 goats-0.2.5/src/goats/core/interpolation.py
--rw-r--r--   0        0        0     6215 2022-11-10 16:10:01.595199 goats-0.2.5/src/goats/core/iotools.py
--rw-r--r--   0        0        0    55446 2023-03-31 13:27:39.253957 goats-0.2.5/src/goats/core/iterables.py
--rw-r--r--   0        0        0    15041 2023-03-31 13:27:39.257957 goats-0.2.5/src/goats/core/measurable.py
--rw-r--r--   0        0        0    36155 2023-03-31 13:27:39.257957 goats-0.2.5/src/goats/core/metadata.py
--rw-r--r--   0        0        0    88816 2023-02-10 19:09:53.043771 goats-0.2.5/src/goats/core/metric.py
--rw-r--r--   0        0        0     7769 2022-11-10 16:10:01.595199 goats-0.2.5/src/goats/core/numerical.py
--rw-r--r--   0        0        0     3066 2023-03-31 13:27:39.257957 goats-0.2.5/src/goats/core/observed.py
--rw-r--r--   0        0        0     3932 2023-03-31 13:27:39.257957 goats-0.2.5/src/goats/core/observer.py
--rw-r--r--   0        0        0    18362 2023-03-31 13:27:39.257957 goats-0.2.5/src/goats/core/observing.py
--rw-r--r--   0        0        0     7363 2023-03-31 13:27:39.257957 goats-0.2.5/src/goats/core/operational.py
--rw-r--r--   0        0        0    23342 2023-03-31 13:27:39.257957 goats-0.2.5/src/goats/core/physical.py
--rw-r--r--   0        0        0     1998 2022-11-10 16:10:01.599199 goats-0.2.5/src/goats/core/plasma.py
--rw-r--r--   0        0        0     3748 2023-03-31 16:19:23.081623 goats-0.2.5/src/goats/core/reference.py
--rw-r--r--   0        0        0     3835 2022-11-10 16:10:01.599199 goats-0.2.5/src/goats/core/spelling.py
--rw-r--r--   0        0        0    60269 2023-03-31 13:27:39.257957 goats-0.2.5/src/goats/core/symbolic.py
--rw-r--r--   0        0        0     3793 2023-03-31 13:27:39.257957 goats-0.2.5/src/goats/core/utilities.py
--rw-r--r--   0        0        0    26013 2023-03-31 13:27:39.257957 goats-0.2.5/src/goats/core/variable.py
--rw-r--r--   0        0        0    28638 2023-05-04 13:36:34.367335 goats-0.2.5/src/goats/eprem/__init__.py
--rw-r--r--   0        0        0    26457 2023-05-04 13:36:42.815326 goats-0.2.5/src/goats/eprem/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4460 2022-03-16 13:21:58.429352 goats-0.2.5/src/goats/eprem/__pycache__/_datasets.cpython-38.pyc
--rw-r--r--   0        0        0     4646 2022-03-16 19:13:43.202027 goats-0.2.5/src/goats/eprem/__pycache__/_observing.cpython-38.pyc
--rw-r--r--   0        0        0     6048 2022-01-27 03:28:43.616605 goats-0.2.5/src/goats/eprem/__pycache__/base.cpython-38.pyc
--rw-r--r--   0        0        0    13674 2022-01-10 18:23:13.849348 goats-0.2.5/src/goats/eprem/__pycache__/basetypes.cpython-38.pyc
--rw-r--r--   0        0        0    11857 2022-03-16 19:13:43.698048 goats-0.2.5/src/goats/eprem/__pycache__/datasets.cpython-38.pyc
--rw-r--r--   0        0        0     5867 2022-07-19 15:10:34.590171 goats-0.2.5/src/goats/eprem/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0        0        0     4021 2022-09-23 14:19:24.386407 goats-0.2.5/src/goats/eprem/__pycache__/interpolation.cpython-38.pyc
--rw-r--r--   0        0        0     6376 2022-07-29 20:37:44.046549 goats-0.2.5/src/goats/eprem/__pycache__/observable.cpython-38.pyc
--rw-r--r--   0        0        0    17900 2022-07-19 15:10:34.590171 goats-0.2.5/src/goats/eprem/__pycache__/observables.cpython-38.pyc
--rw-r--r--   0        0        0     5420 2021-12-16 22:12:31.012722 goats-0.2.5/src/goats/eprem/__pycache__/observers.cpython-38.pyc
--rw-r--r--   0        0        0     5908 2022-02-11 03:31:57.237338 goats-0.2.5/src/goats/eprem/__pycache__/observing.cpython-38.pyc
--rw-r--r--   0        0        0    35437 2022-07-28 20:56:25.812120 goats-0.2.5/src/goats/eprem/__pycache__/parameters.cpython-38.pyc
--rw-r--r--   0        0        0    47613 2023-04-19 01:16:02.713982 goats-0.2.5/src/goats/eprem/__pycache__/runtime.cpython-38.pyc
--rw-r--r--   0        0        0    19888 2022-12-22 19:26:13.402833 goats-0.2.5/src/goats/eprem/runtime.json
--rw-r--r--   0        0        0    52655 2023-03-31 13:27:39.261958 goats-0.2.5/src/goats/eprem/runtime.py
--rw-r--r--   0        0        0     6765 2023-05-04 13:41:22.104295 goats-0.2.5/setup.py
--rw-r--r--   0        0        0     6411 2023-05-04 13:41:22.104787 goats-0.2.5/PKG-INFO
+-rwxr-xr-x   0        0        0    35092 2021-12-16 18:46:50.226668 goats-0.2.6/LICENSE
+-rw-r--r--   0        0        0     5763 2023-03-31 13:27:39.249957 goats-0.2.6/README.md
+-rw-r--r--   0        0        0      891 2023-05-05 14:25:07.491691 goats-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-09 16:57:39.661704 goats-0.2.6/src/goats/core/__init__.py
+-rw-r--r--   0        0        0    11231 2022-11-10 16:10:01.591199 goats-0.2.6/src/goats/core/algebraic.py
+-rw-r--r--   0        0        0    34484 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/aliased.py
+-rw-r--r--   0        0        0     5465 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/axis.py
+-rw-r--r--   0        0        0    16025 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/computed.py
+-rw-r--r--   0        0        0     3107 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/constant.py
+-rw-r--r--   0        0        0     8617 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/datafile.py
+-rw-r--r--   0        0        0    14395 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/fundamental.py
+-rw-r--r--   0        0        0     5772 2023-03-31 22:32:43.725018 goats-0.2.6/src/goats/core/index.py
+-rw-r--r--   0        0        0     4610 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/interpolation.py
+-rw-r--r--   0        0        0     6215 2022-11-10 16:10:01.595199 goats-0.2.6/src/goats/core/iotools.py
+-rw-r--r--   0        0        0    55446 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/iterables.py
+-rw-r--r--   0        0        0    15041 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/measurable.py
+-rw-r--r--   0        0        0    36155 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/metadata.py
+-rw-r--r--   0        0        0    88816 2023-02-10 19:09:53.043771 goats-0.2.6/src/goats/core/metric.py
+-rw-r--r--   0        0        0     7769 2022-11-10 16:10:01.595199 goats-0.2.6/src/goats/core/numerical.py
+-rw-r--r--   0        0        0     3066 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/observed.py
+-rw-r--r--   0        0        0     3932 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/observer.py
+-rw-r--r--   0        0        0    18362 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/observing.py
+-rw-r--r--   0        0        0     7363 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/operational.py
+-rw-r--r--   0        0        0    23342 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/physical.py
+-rw-r--r--   0        0        0     1998 2022-11-10 16:10:01.599199 goats-0.2.6/src/goats/core/plasma.py
+-rw-r--r--   0        0        0     3748 2023-03-31 16:19:23.081623 goats-0.2.6/src/goats/core/reference.py
+-rw-r--r--   0        0        0     3835 2022-11-10 16:10:01.599199 goats-0.2.6/src/goats/core/spelling.py
+-rw-r--r--   0        0        0    60269 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/symbolic.py
+-rw-r--r--   0        0        0     3793 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/utilities.py
+-rw-r--r--   0        0        0    26013 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/variable.py
+-rw-r--r--   0        0        0    28499 2023-05-05 14:24:14.383449 goats-0.2.6/src/goats/eprem/__init__.py
+-rw-r--r--   0        0        0    19888 2022-12-22 19:26:13.402833 goats-0.2.6/src/goats/eprem/runtime.json
+-rw-r--r--   0        0        0    52655 2023-03-31 13:27:39.261958 goats-0.2.6/src/goats/eprem/runtime.py
+-rw-r--r--   0        0        0     6765 2023-05-05 14:27:46.254380 goats-0.2.6/setup.py
+-rw-r--r--   0        0        0     6411 2023-05-05 14:27:46.255319 goats-0.2.6/PKG-INFO
```

### Comparing `goats-0.2.5/LICENSE` & `goats-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/README.md` & `goats-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/pyproject.toml` & `goats-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goats"
-version = "0.2.5"
+version = "0.2.6"
 description = "A set of tools for analyzing heliophysical datasets"
 authors = ["Matt Young"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `goats-0.2.5/src/goats/core/__pycache__/utilities.cpython-38.pyc` & `goats-0.2.6/src/goats/core/utilities.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,265 +1,238 @@
-00000000: 550d 0d0a 0000 0000 cbdf 2664 d10e 0000  U.........&d....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6500 a001 6402 a101 5a02  d.l.Z.e...d...Z.
-00000040: 6502 6503 6500 6a04 6500 6a05 6502 6602  e.e.e.j.e.j.e.f.
-00000050: 1900 6403 9c03 6404 6405 8404 5a06 6500  ..d...d.d...Z.e.
-00000060: 6a07 6502 6503 6401 6403 9c03 6406 6407  j.e.e.d.d...d.d.
-00000070: 8404 8301 5a08 6500 6a07 6502 6503 6401  ....Z.e.j.e.e.d.
-00000080: 6403 9c03 6408 6407 8404 8301 5a08 6500  d...d.d.....Z.e.
-00000090: 6a07 6502 6503 6401 6403 9c03 6409 6407  j.e.e.d.d...d.d.
-000000a0: 8404 8301 5a08 640a 6407 8400 5a08 6503  ....Z.d.d...Z.e.
-000000b0: 640b 9c01 640c 640d 8404 5a09 6401 5300  d...d.d...Z.d.S.
-000000c0: 290e e900 0000 004e da01 5429 03da 085f  )......N..T)..._
-000000d0: 5f6f 626a 6563 74da 065f 5f6e 616d 65da  _object..__name.
-000000e0: 0672 6574 7572 6e63 0200 0000 0000 0000  .returnc........
-000000f0: 0000 0000 0500 0000 0400 0000 4f00 0000  ............O...
-00000100: 7322 0000 0074 007c 007c 017c 0083 037d  s"...t.|.|.|...}
-00000110: 0474 017c 0483 0172 1e7c 047c 027c 038e  .t.|...r.|.|.|..
-00000120: 0153 007c 0453 0029 0161 bd04 0000 4765  .S.|.S.).a....Ge
-00000130: 7420 616e 2061 7070 726f 7072 6961 7465  t an appropriate
-00000140: 2076 616c 7565 2062 6173 6564 206f 6e20   value based on 
-00000150: 7468 6520 6769 7665 6e20 6f62 6a65 6374  the given object
-00000160: 2074 7970 652e 0a20 2020 200a 2020 2020   type..    .    
-00000170: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00000180: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 5f5f  ---------.    __
-00000190: 6f62 6a65 6374 203a 2041 6e79 0a20 2020  object : Any.   
-000001a0: 2020 2020 2054 6865 206f 626a 6563 7420       The object 
-000001b0: 6672 6f6d 2077 6869 6368 2074 6f20 7265  from which to re
-000001c0: 7472 6965 7665 2074 6865 2074 6172 6765  trieve the targe
-000001d0: 7420 6174 7472 6962 7574 652c 2069 6620  t attribute, if 
-000001e0: 6176 6169 6c61 626c 652e 0a0a 2020 2020  available...    
-000001f0: 5f5f 6e61 6d65 203a 2073 7472 696e 670a  __name : string.
-00000200: 2020 2020 2020 2020 5468 6520 6e61 6d65          The name
-00000210: 206f 6620 7468 6520 7461 7267 6574 2061   of the target a
-00000220: 7474 7269 6275 7465 2e0a 0a20 2020 202a  ttribute...    *
-00000230: 6172 6773 0a20 2020 2020 2020 204f 7074  args.        Opt
-00000240: 696f 6e61 6c20 706f 7369 7469 6f6e 616c  ional positional
-00000250: 2061 7267 756d 656e 7473 2074 6f20 7061   arguments to pa
-00000260: 7373 2074 6f20 7468 6520 7461 7267 6574  ss to the target
-00000270: 2061 7474 7269 6275 7465 2c20 6966 2069   attribute, if i
-00000280: 7420 6973 0a20 2020 2020 2020 2063 616c  t is.        cal
-00000290: 6c61 626c 652e 0a0a 2020 2020 2a2a 6b77  lable...    **kw
-000002a0: 6172 6773 0a20 2020 2020 2020 204f 7074  args.        Opt
-000002b0: 696f 6e61 6c20 6b65 7977 6f72 6420 6172  ional keyword ar
-000002c0: 6775 6d65 6e74 7320 746f 2070 6173 7320  guments to pass 
-000002d0: 746f 2074 6865 2074 6172 6765 7420 6174  to the target at
-000002e0: 7472 6962 7574 652c 2069 6620 6974 2069  tribute, if it i
-000002f0: 730a 2020 2020 2020 2020 6361 6c6c 6162  s.        callab
-00000300: 6c65 2e0a 0a20 2020 2052 6574 7572 6e73  le...    Returns
-00000310: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00000320: 2041 6e79 0a20 2020 2020 2020 2054 6865   Any.        The
-00000330: 2076 616c 7565 206f 6620 7468 6520 6174   value of the at
-00000340: 7472 6962 7574 6520 6f6e 2074 6865 2067  tribute on the g
-00000350: 6976 656e 206f 626a 6563 742c 206f 7220  iven object, or 
-00000360: 7468 6520 6f62 6a65 6374 2069 7473 656c  the object itsel
-00000370: 662e 0a20 2020 2020 2020 2053 6565 204e  f..        See N
-00000380: 6f74 6573 2066 6f72 2066 7572 7468 6572  otes for further
-00000390: 2065 7870 6c61 6e61 7469 6f6e 2e0a 0a20   explanation... 
-000003a0: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
-000003b0: 2d2d 0a20 2020 2054 6869 7320 6675 6e63  --.    This func
-000003c0: 7469 6f6e 2077 696c 6c20 6174 7465 6d70  tion will attemp
-000003d0: 7420 746f 2072 6574 7269 6576 6520 7468  t to retrieve th
-000003e0: 6520 6e61 6d65 6420 6174 7472 6962 7574  e named attribut
-000003f0: 6520 6672 6f6d 2074 6865 2067 6976 656e  e from the given
-00000400: 0a20 2020 206f 626a 6563 742e 2049 6620  .    object. If 
-00000410: 7468 6520 6174 7472 6962 7574 6520 6578  the attribute ex
-00000420: 6973 7473 2061 6e64 2069 7320 6361 6c6c  ists and is call
-00000430: 6162 6c65 2028 652e 672e 2c20 6120 636c  able (e.g., a cl
-00000440: 6173 7320 6d65 7468 6f64 292c 2074 6869  ass method), thi
-00000450: 730a 2020 2020 6675 6e63 7469 6f6e 2077  s.    function w
-00000460: 696c 6c20 6361 6c6c 2074 6865 2061 7474  ill call the att
-00000470: 7269 6275 7465 2077 6974 6820 602a 6172  ribute with `*ar
-00000480: 6773 6020 616e 6420 602a 2a6b 7761 7267  gs` and `**kwarg
-00000490: 7360 2c20 616e 6420 7265 7475 726e 2074  s`, and return t
-000004a0: 6865 0a20 2020 2072 6573 756c 742e 2049  he.    result. I
-000004b0: 6620 7468 6520 6174 7472 6962 7574 6520  f the attribute 
-000004c0: 6578 6973 7473 2061 6e64 2069 7320 6e6f  exists and is no
-000004d0: 7420 6361 6c6c 6162 6c65 2c20 7468 6973  t callable, this
-000004e0: 2066 756e 6374 696f 6e20 7769 6c6c 0a20   function will. 
-000004f0: 2020 2072 6574 7572 6e20 6974 2061 732d     return it as-
-00000500: 6973 2e20 4966 2074 6865 2061 7474 7269  is. If the attri
-00000510: 6275 7465 2064 6f65 7320 6e6f 7420 6578  bute does not ex
-00000520: 6973 742c 2074 6869 7320 6675 6e63 7469  ist, this functi
-00000530: 6f6e 2077 696c 6c20 7265 7475 726e 0a20  on will return. 
-00000540: 2020 2074 6865 2067 6976 656e 206f 626a     the given obj
-00000550: 6563 742e 2054 6869 7320 6361 7365 2073  ect. This case s
-00000560: 7570 706f 7274 7320 7072 6f67 7261 6d6d  upports programm
-00000570: 6174 6963 2075 7365 2077 6865 6e20 7468  atic use when th
-00000580: 6520 6361 6c6c 696e 6720 636f 6465 0a20  e calling code. 
-00000590: 2020 2064 6f65 7320 6e6f 7420 6b6e 6f77     does not know
-000005a0: 2074 6865 2074 7970 6520 6f66 206f 626a   the type of obj
-000005b0: 6563 7420 756e 7469 6c20 7275 6e74 696d  ect until runtim
-000005c0: 652e 0a0a 2020 2020 4578 616d 706c 6573  e...    Examples
-000005d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-000005e0: 2020 544f 444f 0a20 2020 2029 02da 0767    TODO.    )...g
-000005f0: 6574 6174 7472 da08 6361 6c6c 6162 6c65  etattr..callable
-00000600: 2905 7203 0000 0072 0400 0000 da04 6172  ).r....r......ar
-00000610: 6773 da06 6b77 6172 6773 da04 6174 7472  gs..kwargs..attr
-00000620: a900 720b 0000 00fa 362f 686f 6d65 2f6d  ..r.....6/home/m
-00000630: 6174 7468 6577 2f70 7974 686f 6e2f 676f  atthew/python/go
-00000640: 6174 732f 7372 632f 676f 6174 732f 636f  ats/src/goats/co
-00000650: 7265 2f75 7469 6c69 7469 6573 2e70 79da  re/utilities.py.
-00000660: 0a67 6574 6174 7472 7661 6c06 0000 0073  .getattrval....s
-00000670: 0400 0000 002c 0c01 720d 0000 0063 0300  .....,..r....c..
-00000680: 0000 0000 0000 0000 0000 0300 0000 0100  ................
-00000690: 0000 4300 0000 7304 0000 0064 0053 00a9  ..C...s....d.S..
-000006a0: 014e 720b 0000 0029 0372 0300 0000 7204  .Nr....).r....r.
-000006b0: 0000 00da 075f 5f76 616c 7565 720b 0000  .....__valuer...
-000006c0: 0072 0b00 0000 720c 0000 00da 0a73 6574  .r....r......set
-000006d0: 6174 7472 7661 6c36 0000 0073 0200 0000  attrval6...s....
-000006e0: 0001 7210 0000 0063 0300 0000 0000 0000  ..r....c........
-000006f0: 0000 0000 0500 0000 0100 0000 4f00 0000  ............O...
-00000700: 7304 0000 0064 0053 0072 0e00 0000 720b  s....d.S.r....r.
-00000710: 0000 0029 0572 0300 0000 7204 0000 0072  ...).r....r....r
-00000720: 0f00 0000 7208 0000 0072 0900 0000 720b  ....r....r....r.
-00000730: 0000 0072 0b00 0000 720c 0000 0072 1000  ...r....r....r..
-00000740: 0000 3a00 0000 7302 0000 0000 0163 0200  ..:...s......c..
-00000750: 0000 0000 0000 0000 0000 0400 0000 0100  ................
-00000760: 0000 4f00 0000 7304 0000 0064 0053 0072  ..O...s....d.S.r
-00000770: 0e00 0000 720b 0000 0029 0472 0300 0000  ....r....).r....
-00000780: 7204 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-00000790: 0b00 0000 720b 0000 0072 0c00 0000 7210  ....r....r....r.
-000007a0: 0000 003e 0000 0073 0200 0000 0001 6300  ...>...s......c.
-000007b0: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-000007c0: 0000 004f 0000 0073 3c00 0000 7c00 5e02  ...O...s<...|.^.
-000007d0: 7d02 7d03 7d00 7400 7c02 7c03 8302 7d04  }.}.}.t.|.|...}.
-000007e0: 7401 7c04 8301 7228 7c04 7c00 7c01 8e01  t.|...r(|.|.|...
-000007f0: 0100 6e10 7402 7c02 7c03 7c00 6401 1900  ..n.t.|.|.|.d...
-00000800: 8303 0100 6402 5300 2903 6157 0500 0053  ....d.S.).aW...S
-00000810: 6574 2061 6e20 6170 7072 6f70 7269 6174  et an appropriat
-00000820: 6520 7661 6c75 6520 6261 7365 6420 6f6e  e value based on
-00000830: 2074 6865 2067 6976 656e 206f 626a 6563   the given objec
-00000840: 7420 7479 7065 2e0a 2020 2020 0a20 2020  t type..    .   
-00000850: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00000860: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 205f  ----------.    _
-00000870: 5f6f 626a 6563 7420 3a20 416e 790a 2020  _object : Any.  
-00000880: 2020 2020 2020 5468 6520 6f62 6a65 6374        The object
-00000890: 206f 6e20 7768 6963 6820 746f 2073 6574   on which to set
-000008a0: 2074 6865 2074 6172 6765 7420 6174 7472   the target attr
-000008b0: 6962 7574 652e 0a0a 2020 2020 5f5f 6e61  ibute...    __na
-000008c0: 6d65 203a 2073 7472 696e 670a 2020 2020  me : string.    
-000008d0: 2020 2020 5468 6520 6e61 6d65 206f 6620      The name of 
-000008e0: 7468 6520 7461 7267 6574 2061 7474 7269  the target attri
-000008f0: 6275 7465 2e0a 0a20 2020 205f 5f76 616c  bute...    __val
-00000900: 7565 203a 2041 6e79 0a20 2020 2020 2020  ue : Any.       
-00000910: 2054 6865 206e 6577 2076 616c 7565 206f   The new value o
-00000920: 6620 7468 6520 7461 7267 6574 2061 7474  f the target att
-00000930: 7269 6275 7465 2e0a 0a20 2020 202a 6172  ribute...    *ar
-00000940: 6773 0a20 2020 2020 2020 2050 6f73 6974  gs.        Posit
-00000950: 696f 6e61 6c20 6172 6775 6d65 6e74 7320  ional arguments 
-00000960: 746f 2070 6173 7320 7468 6520 7461 7267  to pass the targ
-00000970: 6574 2061 7474 7269 6275 7465 2c20 6966  et attribute, if
-00000980: 2069 7420 6973 2063 616c 6c61 626c 652e   it is callable.
-00000990: 0a20 2020 2020 2020 2053 6565 204e 6f74  .        See Not
-000009a0: 6573 2066 6f72 2066 7572 7468 6572 2065  es for further e
-000009b0: 7870 6c61 6e61 7469 6f6e 2e0a 0a20 2020  xplanation...   
-000009c0: 202a 2a6b 7761 7267 730a 2020 2020 2020   **kwargs.      
-000009d0: 2020 4b65 7977 6f72 6420 6172 6775 6d65    Keyword argume
-000009e0: 6e74 7320 746f 2070 6173 7320 746f 2074  nts to pass to t
-000009f0: 6865 2074 6172 6765 7420 6174 7472 6962  he target attrib
-00000a00: 7574 652c 2069 6620 6974 2069 7320 6361  ute, if it is ca
-00000a10: 6c6c 6162 6c65 2e0a 2020 2020 2020 2020  llable..        
-00000a20: 5365 6520 4e6f 7465 7320 666f 7220 6675  See Notes for fu
-00000a30: 7274 6865 7220 6578 706c 616e 6174 696f  rther explanatio
-00000a40: 6e2e 0a0a 2020 2020 5265 7475 726e 730a  n...    Returns.
-00000a50: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00000a60: 4e6f 6e65 0a0a 2020 2020 4e6f 7465 730a  None..    Notes.
-00000a70: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5468      -----.    Th
-00000a80: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
-00000a90: 2061 7474 656d 7074 2074 6f20 7365 7420   attempt to set 
-00000aa0: 7468 6520 6e61 6d65 6420 6174 7472 6962  the named attrib
-00000ab0: 7574 6520 6f6e 2074 6865 2067 6976 656e  ute on the given
-00000ac0: 206f 626a 6563 742e 0a20 2020 2049 6620   object..    If 
-00000ad0: 7468 6520 6174 7472 6962 7574 6520 6578  the attribute ex
-00000ae0: 6973 7473 2061 6e64 2069 7320 6361 6c6c  ists and is call
-00000af0: 6162 6c65 2028 652e 672e 2c20 6120 636c  able (e.g., a cl
-00000b00: 6173 7320 6d65 7468 6f64 292c 2074 6869  ass method), thi
-00000b10: 730a 2020 2020 6675 6e63 7469 6f6e 2077  s.    function w
-00000b20: 696c 6c20 6361 6c6c 2074 6865 2061 7474  ill call the att
-00000b30: 7269 6275 7465 2077 6974 6820 616c 6c20  ribute with all 
-00000b40: 706f 7369 7469 6f6e 616c 2061 7267 756d  positional argum
-00000b50: 656e 7473 2061 6674 6572 0a20 2020 2060  ents after.    `
-00000b60: 5f5f 6f62 6a65 6374 6020 616e 6420 605f  __object` and `_
-00000b70: 5f6e 616d 6560 2c20 6173 2077 656c 6c20  _name`, as well 
-00000b80: 6173 2061 6e79 2067 6976 656e 206b 6579  as any given key
-00000b90: 776f 7264 2061 7267 756d 656e 7473 2e20  word arguments. 
-00000ba0: 5468 6520 7573 6572 0a20 2020 206d 6179  The user.    may
-00000bb0: 2070 6173 7320 7468 6520 6e65 7720 7661   pass the new va
-00000bc0: 6c75 6520 6173 2074 6865 2066 6972 7374  lue as the first
-00000bd0: 2070 6f73 6974 696f 6e61 6c20 6172 6775   positional argu
-00000be0: 6d65 6e74 206f 7220 6173 2061 206b 6579  ment or as a key
-00000bf0: 776f 7264 0a20 2020 2061 7267 756d 656e  word.    argumen
-00000c00: 742c 2069 6e20 6f72 6465 7220 746f 2073  t, in order to s
-00000c10: 7570 706f 7274 2061 7320 6d61 6e79 2066  upport as many f
-00000c20: 6f72 6d73 206f 6620 6361 6c6c 6162 6c65  orms of callable
-00000c30: 2061 7474 7269 6275 7465 7320 6173 0a20   attributes as. 
-00000c40: 2020 2070 6f73 7369 626c 652e 2049 6620     possible. If 
-00000c50: 7468 6520 6174 7472 6962 7574 6520 6578  the attribute ex
-00000c60: 6973 7473 2061 6e64 2069 7320 6e6f 7420  ists and is not 
-00000c70: 6361 6c6c 6162 6c65 2c20 7468 6973 2066  callable, this f
-00000c80: 756e 6374 696f 6e20 7769 6c6c 0a20 2020  unction will.   
-00000c90: 2073 6574 2074 6865 206e 6577 2076 616c   set the new val
-00000ca0: 7565 2066 726f 6d20 7468 6520 6669 7273  ue from the firs
-00000cb0: 7420 706f 7369 7469 6f6e 616c 2061 7267  t positional arg
-00000cc0: 756d 656e 7420 6166 7465 7220 605f 5f6f  ument after `__o
-00000cd0: 626a 6563 7460 2061 6e64 0a20 2020 2060  bject` and.    `
-00000ce0: 5f5f 6e61 6d65 602e 2049 6620 7468 6520  __name`. If the 
-00000cf0: 6174 7472 6962 7574 6520 646f 6573 206e  attribute does n
-00000d00: 6f74 2065 7869 7374 2c20 7468 6973 2066  ot exist, this f
-00000d10: 756e 6374 696f 6e20 7769 6c6c 2072 6169  unction will rai
-00000d20: 7365 2061 6e0a 2020 2020 6060 4174 7472  se an.    ``Attr
-00000d30: 6962 7574 6545 7272 6f72 6060 2e0a 0a20  ibuteError``... 
-00000d40: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-00000d50: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2054 4f44  --------.    TOD
-00000d60: 4f0a 2020 2020 7201 0000 004e 2903 7206  O.    r....N).r.
-00000d70: 0000 0072 0700 0000 da07 7365 7461 7474  ...r......setatt
-00000d80: 7229 0572 0800 0000 7209 0000 00da 036f  r).r....r......o
-00000d90: 626a da04 6e61 6d65 720a 0000 0072 0b00  bj..namer....r..
-00000da0: 0000 720b 0000 0072 0c00 0000 7210 0000  ..r....r....r...
-00000db0: 0042 0000 0073 0a00 0000 002b 0a01 0a01  .B...s.....+....
-00000dc0: 0801 0c02 2901 7213 0000 0063 0100 0000  ....).r....c....
-00000dd0: 0000 0000 0000 0000 0300 0000 0800 0000  ................
-00000de0: 0700 0000 738e 0000 0074 007c 0183 0164  ....s....t.|...d
-00000df0: 016b 0272 1474 0164 0283 0182 017a 1274  .k.r.t.d.....z.t
-00000e00: 027c 0164 0119 0088 0083 0289 0157 006e  .|.d.........W.n
-00000e10: 1604 0074 036b 0a72 3c01 0001 0001 0059  ...t.k.r<......Y
-00000e20: 0064 0353 0058 0074 007c 0183 0164 046b  .d.S.X.t.|...d.k
-00000e30: 0272 4e64 0553 007a 2474 0487 0087 0166  .rNd.S.z$t.....f
-00000e40: 0264 0664 0784 087c 0164 0464 0885 0219  .d.d...|.d.d....
-00000e50: 0044 0083 0183 017d 0257 006e 1604 0074  .D.....}.W.n...t
-00000e60: 036b 0a72 8801 0001 0001 0059 0064 0353  .k.r.......Y.d.S
-00000e70: 0058 007c 0253 0029 097a 3f54 7275 6520  .X.|.S.).z?True 
-00000e80: 6966 2061 6c6c 206f 626a 6563 7473 2068  if all objects h
-00000e90: 6176 6520 7468 6520 6e61 6d65 6420 6174  ave the named at
-00000ea0: 7472 6962 7574 6520 7769 7468 2065 7175  tribute with equ
-00000eb0: 616c 2076 616c 7565 732e 7201 0000 007a  al values.r....z
-00000ec0: 154e 6f20 6f62 6a65 6374 7320 746f 2063  .No objects to c
-00000ed0: 6f6d 7061 7265 46e9 0100 0000 5463 0100  ompareF.....Tc..
-00000ee0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000ef0: 0000 3300 0000 731c 0000 007c 005d 147d  ..3...s....|.].}
-00000f00: 0174 007c 0188 0083 0288 016b 0256 0001  .t.|.......k.V..
-00000f10: 0071 0264 0053 0072 0e00 0000 2901 7206  .q.d.S.r....).r.
-00000f20: 0000 0029 02da 022e 30da 0169 a902 7213  ...)....0..i..r.
-00000f30: 0000 00da 0176 720b 0000 0072 0c00 0000  .....vr....r....
-00000f40: da09 3c67 656e 6578 7072 3e80 0000 0073  ..<genexpr>....s
-00000f50: 0400 0000 0400 0200 7a1e 6571 7561 6c5f  ........z.equal_
-00000f60: 6174 7472 732e 3c6c 6f63 616c 733e 2e3c  attrs.<locals>.<
-00000f70: 6765 6e65 7870 723e 4e29 05da 036c 656e  genexpr>N)...len
-00000f80: da0a 5661 6c75 6545 7272 6f72 7206 0000  ..ValueErrorr...
-00000f90: 00da 0e41 7474 7269 6275 7465 4572 726f  ...AttributeErro
-00000fa0: 72da 0361 6c6c 2903 7213 0000 00da 076f  r..all).r......o
-00000fb0: 626a 6563 7473 da05 7472 7574 6872 0b00  bjects..truthr..
-00000fc0: 0000 7217 0000 0072 0c00 0000 da0b 6571  ..r....r......eq
-00000fd0: 7561 6c5f 6174 7472 7375 0000 0073 1a00  ual_attrsu...s..
-00000fe0: 0000 0002 0c01 0801 0201 1201 0e01 0801  ................
-00000ff0: 0c01 0401 0201 2401 0e01 0801 7220 0000  ......$.....r ..
-00001000: 0029 0ada 0674 7970 696e 67da 0754 7970  .)...typing..Typ
-00001010: 6556 6172 7202 0000 00da 0373 7472 da05  eVarr......str..
-00001020: 556e 696f 6eda 0341 6e79 720d 0000 00da  Union..Anyr.....
-00001030: 086f 7665 726c 6f61 6472 1000 0000 7220  .overloadr....r 
-00001040: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
-00001050: 0000 720c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00001060: 3e01 0000 0073 1a00 0000 0802 0a04 0201  >....s..........
-00001070: 0203 0efb 0c30 0401 1403 0401 1403 0401  .....0..........
-00001080: 1403 0833                                ...3
+00000000: 696d 706f 7274 2074 7970 696e 670a 0a54  import typing..T
+00000010: 203d 2074 7970 696e 672e 5479 7065 5661   = typing.TypeVa
+00000020: 7228 2754 2729 0a0a 0a64 6566 2067 6574  r('T')...def get
+00000030: 6174 7472 7661 6c28 0a20 2020 205f 5f6f  attrval(.    __o
+00000040: 626a 6563 743a 2054 2c0a 2020 2020 5f5f  bject: T,.    __
+00000050: 6e61 6d65 3a20 7374 722c 0a20 2020 202a  name: str,.    *
+00000060: 6172 6773 2c0a 2020 2020 2a2a 6b77 6172  args,.    **kwar
+00000070: 6773 0a29 202d 3e20 7479 7069 6e67 2e55  gs.) -> typing.U
+00000080: 6e69 6f6e 5b74 7970 696e 672e 416e 792c  nion[typing.Any,
+00000090: 2054 5d3a 0a20 2020 2022 2222 4765 7420   T]:.    """Get 
+000000a0: 616e 2061 7070 726f 7072 6961 7465 2076  an appropriate v
+000000b0: 616c 7565 2062 6173 6564 206f 6e20 7468  alue based on th
+000000c0: 6520 6769 7665 6e20 6f62 6a65 6374 2074  e given object t
+000000d0: 7970 652e 0a20 2020 200a 2020 2020 5061  ype..    .    Pa
+000000e0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+000000f0: 2d2d 2d2d 2d2d 2d0a 2020 2020 5f5f 6f62  -------.    __ob
+00000100: 6a65 6374 203a 2041 6e79 0a20 2020 2020  ject : Any.     
+00000110: 2020 2054 6865 206f 626a 6563 7420 6672     The object fr
+00000120: 6f6d 2077 6869 6368 2074 6f20 7265 7472  om which to retr
+00000130: 6965 7665 2074 6865 2074 6172 6765 7420  ieve the target 
+00000140: 6174 7472 6962 7574 652c 2069 6620 6176  attribute, if av
+00000150: 6169 6c61 626c 652e 0a0a 2020 2020 5f5f  ailable...    __
+00000160: 6e61 6d65 203a 2073 7472 696e 670a 2020  name : string.  
+00000170: 2020 2020 2020 5468 6520 6e61 6d65 206f        The name o
+00000180: 6620 7468 6520 7461 7267 6574 2061 7474  f the target att
+00000190: 7269 6275 7465 2e0a 0a20 2020 202a 6172  ribute...    *ar
+000001a0: 6773 0a20 2020 2020 2020 204f 7074 696f  gs.        Optio
+000001b0: 6e61 6c20 706f 7369 7469 6f6e 616c 2061  nal positional a
+000001c0: 7267 756d 656e 7473 2074 6f20 7061 7373  rguments to pass
+000001d0: 2074 6f20 7468 6520 7461 7267 6574 2061   to the target a
+000001e0: 7474 7269 6275 7465 2c20 6966 2069 7420  ttribute, if it 
+000001f0: 6973 0a20 2020 2020 2020 2063 616c 6c61  is.        calla
+00000200: 626c 652e 0a0a 2020 2020 2a2a 6b77 6172  ble...    **kwar
+00000210: 6773 0a20 2020 2020 2020 204f 7074 696f  gs.        Optio
+00000220: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
+00000230: 6d65 6e74 7320 746f 2070 6173 7320 746f  ments to pass to
+00000240: 2074 6865 2074 6172 6765 7420 6174 7472   the target attr
+00000250: 6962 7574 652c 2069 6620 6974 2069 730a  ibute, if it is.
+00000260: 2020 2020 2020 2020 6361 6c6c 6162 6c65          callable
+00000270: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+00000280: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2041     -------.    A
+00000290: 6e79 0a20 2020 2020 2020 2054 6865 2076  ny.        The v
+000002a0: 616c 7565 206f 6620 7468 6520 6174 7472  alue of the attr
+000002b0: 6962 7574 6520 6f6e 2074 6865 2067 6976  ibute on the giv
+000002c0: 656e 206f 626a 6563 742c 206f 7220 7468  en object, or th
+000002d0: 6520 6f62 6a65 6374 2069 7473 656c 662e  e object itself.
+000002e0: 0a20 2020 2020 2020 2053 6565 204e 6f74  .        See Not
+000002f0: 6573 2066 6f72 2066 7572 7468 6572 2065  es for further e
+00000300: 7870 6c61 6e61 7469 6f6e 2e0a 0a20 2020  xplanation...   
+00000310: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
+00000320: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
+00000330: 6f6e 2077 696c 6c20 6174 7465 6d70 7420  on will attempt 
+00000340: 746f 2072 6574 7269 6576 6520 7468 6520  to retrieve the 
+00000350: 6e61 6d65 6420 6174 7472 6962 7574 6520  named attribute 
+00000360: 6672 6f6d 2074 6865 2067 6976 656e 0a20  from the given. 
+00000370: 2020 206f 626a 6563 742e 2049 6620 7468     object. If th
+00000380: 6520 6174 7472 6962 7574 6520 6578 6973  e attribute exis
+00000390: 7473 2061 6e64 2069 7320 6361 6c6c 6162  ts and is callab
+000003a0: 6c65 2028 652e 672e 2c20 6120 636c 6173  le (e.g., a clas
+000003b0: 7320 6d65 7468 6f64 292c 2074 6869 730a  s method), this.
+000003c0: 2020 2020 6675 6e63 7469 6f6e 2077 696c      function wil
+000003d0: 6c20 6361 6c6c 2074 6865 2061 7474 7269  l call the attri
+000003e0: 6275 7465 2077 6974 6820 602a 6172 6773  bute with `*args
+000003f0: 6020 616e 6420 602a 2a6b 7761 7267 7360  ` and `**kwargs`
+00000400: 2c20 616e 6420 7265 7475 726e 2074 6865  , and return the
+00000410: 0a20 2020 2072 6573 756c 742e 2049 6620  .    result. If 
+00000420: 7468 6520 6174 7472 6962 7574 6520 6578  the attribute ex
+00000430: 6973 7473 2061 6e64 2069 7320 6e6f 7420  ists and is not 
+00000440: 6361 6c6c 6162 6c65 2c20 7468 6973 2066  callable, this f
+00000450: 756e 6374 696f 6e20 7769 6c6c 0a20 2020  unction will.   
+00000460: 2072 6574 7572 6e20 6974 2061 732d 6973   return it as-is
+00000470: 2e20 4966 2074 6865 2061 7474 7269 6275  . If the attribu
+00000480: 7465 2064 6f65 7320 6e6f 7420 6578 6973  te does not exis
+00000490: 742c 2074 6869 7320 6675 6e63 7469 6f6e  t, this function
+000004a0: 2077 696c 6c20 7265 7475 726e 0a20 2020   will return.   
+000004b0: 2074 6865 2067 6976 656e 206f 626a 6563   the given objec
+000004c0: 742e 2054 6869 7320 6361 7365 2073 7570  t. This case sup
+000004d0: 706f 7274 7320 7072 6f67 7261 6d6d 6174  ports programmat
+000004e0: 6963 2075 7365 2077 6865 6e20 7468 6520  ic use when the 
+000004f0: 6361 6c6c 696e 6720 636f 6465 0a20 2020  calling code.   
+00000500: 2064 6f65 7320 6e6f 7420 6b6e 6f77 2074   does not know t
+00000510: 6865 2074 7970 6520 6f66 206f 626a 6563  he type of objec
+00000520: 7420 756e 7469 6c20 7275 6e74 696d 652e  t until runtime.
+00000530: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
+00000540: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+00000550: 544f 444f 0a20 2020 2022 2222 0a20 2020  TODO.    """.   
+00000560: 2061 7474 7220 3d20 6765 7461 7474 7228   attr = getattr(
+00000570: 5f5f 6f62 6a65 6374 2c20 5f5f 6e61 6d65  __object, __name
+00000580: 2c20 5f5f 6f62 6a65 6374 290a 2020 2020  , __object).    
+00000590: 7265 7475 726e 2061 7474 7228 2a61 7267  return attr(*arg
+000005a0: 732c 202a 2a6b 7761 7267 7329 2069 6620  s, **kwargs) if 
+000005b0: 6361 6c6c 6162 6c65 2861 7474 7229 2065  callable(attr) e
+000005c0: 6c73 6520 6174 7472 0a0a 0a40 7479 7069  lse attr...@typi
+000005d0: 6e67 2e6f 7665 726c 6f61 640a 6465 6620  ng.overload.def 
+000005e0: 7365 7461 7474 7276 616c 285f 5f6f 626a  setattrval(__obj
+000005f0: 6563 743a 2054 2c20 5f5f 6e61 6d65 3a20  ect: T, __name: 
+00000600: 7374 722c 205f 5f76 616c 7565 2920 2d3e  str, __value) ->
+00000610: 204e 6f6e 653a 202e 2e2e 0a0a 0a40 7479   None: ......@ty
+00000620: 7069 6e67 2e6f 7665 726c 6f61 640a 6465  ping.overload.de
+00000630: 6620 7365 7461 7474 7276 616c 285f 5f6f  f setattrval(__o
+00000640: 626a 6563 743a 2054 2c20 5f5f 6e61 6d65  bject: T, __name
+00000650: 3a20 7374 722c 205f 5f76 616c 7565 2c20  : str, __value, 
+00000660: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00000670: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a0a   -> None: ......
+00000680: 4074 7970 696e 672e 6f76 6572 6c6f 6164  @typing.overload
+00000690: 0a64 6566 2073 6574 6174 7472 7661 6c28  .def setattrval(
+000006a0: 5f5f 6f62 6a65 6374 3a20 542c 205f 5f6e  __object: T, __n
+000006b0: 616d 653a 2073 7472 2c20 2a61 7267 732c  ame: str, *args,
+000006c0: 202a 2a6b 7761 7267 7329 202d 3e20 4e6f   **kwargs) -> No
+000006d0: 6e65 3a20 2e2e 2e0a 0a0a 6465 6620 7365  ne: ......def se
+000006e0: 7461 7474 7276 616c 282a 6172 6773 2c20  tattrval(*args, 
+000006f0: 2a2a 6b77 6172 6773 293a 0a20 2020 2022  **kwargs):.    "
+00000700: 2222 5365 7420 616e 2061 7070 726f 7072  ""Set an appropr
+00000710: 6961 7465 2076 616c 7565 2062 6173 6564  iate value based
+00000720: 206f 6e20 7468 6520 6769 7665 6e20 6f62   on the given ob
+00000730: 6a65 6374 2074 7970 652e 0a20 2020 200a  ject type..    .
+00000740: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00000750: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00000760: 2020 5f5f 6f62 6a65 6374 203a 2041 6e79    __object : Any
+00000770: 0a20 2020 2020 2020 2054 6865 206f 626a  .        The obj
+00000780: 6563 7420 6f6e 2077 6869 6368 2074 6f20  ect on which to 
+00000790: 7365 7420 7468 6520 7461 7267 6574 2061  set the target a
+000007a0: 7474 7269 6275 7465 2e0a 0a20 2020 205f  ttribute...    _
+000007b0: 5f6e 616d 6520 3a20 7374 7269 6e67 0a20  _name : string. 
+000007c0: 2020 2020 2020 2054 6865 206e 616d 6520         The name 
+000007d0: 6f66 2074 6865 2074 6172 6765 7420 6174  of the target at
+000007e0: 7472 6962 7574 652e 0a0a 2020 2020 5f5f  tribute...    __
+000007f0: 7661 6c75 6520 3a20 416e 790a 2020 2020  value : Any.    
+00000800: 2020 2020 5468 6520 6e65 7720 7661 6c75      The new valu
+00000810: 6520 6f66 2074 6865 2074 6172 6765 7420  e of the target 
+00000820: 6174 7472 6962 7574 652e 0a0a 2020 2020  attribute...    
+00000830: 2a61 7267 730a 2020 2020 2020 2020 506f  *args.        Po
+00000840: 7369 7469 6f6e 616c 2061 7267 756d 656e  sitional argumen
+00000850: 7473 2074 6f20 7061 7373 2074 6865 2074  ts to pass the t
+00000860: 6172 6765 7420 6174 7472 6962 7574 652c  arget attribute,
+00000870: 2069 6620 6974 2069 7320 6361 6c6c 6162   if it is callab
+00000880: 6c65 2e0a 2020 2020 2020 2020 5365 6520  le..        See 
+00000890: 4e6f 7465 7320 666f 7220 6675 7274 6865  Notes for furthe
+000008a0: 7220 6578 706c 616e 6174 696f 6e2e 0a0a  r explanation...
+000008b0: 2020 2020 2a2a 6b77 6172 6773 0a20 2020      **kwargs.   
+000008c0: 2020 2020 204b 6579 776f 7264 2061 7267       Keyword arg
+000008d0: 756d 656e 7473 2074 6f20 7061 7373 2074  uments to pass t
+000008e0: 6f20 7468 6520 7461 7267 6574 2061 7474  o the target att
+000008f0: 7269 6275 7465 2c20 6966 2069 7420 6973  ribute, if it is
+00000900: 2063 616c 6c61 626c 652e 0a20 2020 2020   callable..     
+00000910: 2020 2053 6565 204e 6f74 6573 2066 6f72     See Notes for
+00000920: 2066 7572 7468 6572 2065 7870 6c61 6e61   further explana
+00000930: 7469 6f6e 2e0a 0a20 2020 2052 6574 7572  tion...    Retur
+00000940: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00000950: 2020 204e 6f6e 650a 0a20 2020 204e 6f74     None..    Not
+00000960: 6573 0a20 2020 202d 2d2d 2d2d 0a20 2020  es.    -----.   
+00000970: 2054 6869 7320 6675 6e63 7469 6f6e 2077   This function w
+00000980: 696c 6c20 6174 7465 6d70 7420 746f 2073  ill attempt to s
+00000990: 6574 2074 6865 206e 616d 6564 2061 7474  et the named att
+000009a0: 7269 6275 7465 206f 6e20 7468 6520 6769  ribute on the gi
+000009b0: 7665 6e20 6f62 6a65 6374 2e0a 2020 2020  ven object..    
+000009c0: 4966 2074 6865 2061 7474 7269 6275 7465  If the attribute
+000009d0: 2065 7869 7374 7320 616e 6420 6973 2063   exists and is c
+000009e0: 616c 6c61 626c 6520 2865 2e67 2e2c 2061  allable (e.g., a
+000009f0: 2063 6c61 7373 206d 6574 686f 6429 2c20   class method), 
+00000a00: 7468 6973 0a20 2020 2066 756e 6374 696f  this.    functio
+00000a10: 6e20 7769 6c6c 2063 616c 6c20 7468 6520  n will call the 
+00000a20: 6174 7472 6962 7574 6520 7769 7468 2061  attribute with a
+00000a30: 6c6c 2070 6f73 6974 696f 6e61 6c20 6172  ll positional ar
+00000a40: 6775 6d65 6e74 7320 6166 7465 720a 2020  guments after.  
+00000a50: 2020 605f 5f6f 626a 6563 7460 2061 6e64    `__object` and
+00000a60: 2060 5f5f 6e61 6d65 602c 2061 7320 7765   `__name`, as we
+00000a70: 6c6c 2061 7320 616e 7920 6769 7665 6e20  ll as any given 
+00000a80: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+00000a90: 732e 2054 6865 2075 7365 720a 2020 2020  s. The user.    
+00000aa0: 6d61 7920 7061 7373 2074 6865 206e 6577  may pass the new
+00000ab0: 2076 616c 7565 2061 7320 7468 6520 6669   value as the fi
+00000ac0: 7273 7420 706f 7369 7469 6f6e 616c 2061  rst positional a
+00000ad0: 7267 756d 656e 7420 6f72 2061 7320 6120  rgument or as a 
+00000ae0: 6b65 7977 6f72 640a 2020 2020 6172 6775  keyword.    argu
+00000af0: 6d65 6e74 2c20 696e 206f 7264 6572 2074  ment, in order t
+00000b00: 6f20 7375 7070 6f72 7420 6173 206d 616e  o support as man
+00000b10: 7920 666f 726d 7320 6f66 2063 616c 6c61  y forms of calla
+00000b20: 626c 6520 6174 7472 6962 7574 6573 2061  ble attributes a
+00000b30: 730a 2020 2020 706f 7373 6962 6c65 2e20  s.    possible. 
+00000b40: 4966 2074 6865 2061 7474 7269 6275 7465  If the attribute
+00000b50: 2065 7869 7374 7320 616e 6420 6973 206e   exists and is n
+00000b60: 6f74 2063 616c 6c61 626c 652c 2074 6869  ot callable, thi
+00000b70: 7320 6675 6e63 7469 6f6e 2077 696c 6c0a  s function will.
+00000b80: 2020 2020 7365 7420 7468 6520 6e65 7720      set the new 
+00000b90: 7661 6c75 6520 6672 6f6d 2074 6865 2066  value from the f
+00000ba0: 6972 7374 2070 6f73 6974 696f 6e61 6c20  irst positional 
+00000bb0: 6172 6775 6d65 6e74 2061 6674 6572 2060  argument after `
+00000bc0: 5f5f 6f62 6a65 6374 6020 616e 640a 2020  __object` and.  
+00000bd0: 2020 605f 5f6e 616d 6560 2e20 4966 2074    `__name`. If t
+00000be0: 6865 2061 7474 7269 6275 7465 2064 6f65  he attribute doe
+00000bf0: 7320 6e6f 7420 6578 6973 742c 2074 6869  s not exist, thi
+00000c00: 7320 6675 6e63 7469 6f6e 2077 696c 6c20  s function will 
+00000c10: 7261 6973 6520 616e 0a20 2020 2060 6041  raise an.    ``A
+00000c20: 7474 7269 6275 7465 4572 726f 7260 602e  ttributeError``.
+00000c30: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
+00000c40: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+00000c50: 544f 444f 0a20 2020 2022 2222 0a20 2020  TODO.    """.   
+00000c60: 206f 626a 2c20 6e61 6d65 2c20 2a61 7267   obj, name, *arg
+00000c70: 7320 3d20 6172 6773 0a20 2020 2061 7474  s = args.    att
+00000c80: 7220 3d20 6765 7461 7474 7228 6f62 6a2c  r = getattr(obj,
+00000c90: 206e 616d 6529 0a20 2020 2069 6620 6361   name).    if ca
+00000ca0: 6c6c 6162 6c65 2861 7474 7229 3a0a 2020  llable(attr):.  
+00000cb0: 2020 2020 2020 6174 7472 282a 6172 6773        attr(*args
+00000cc0: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+00000cd0: 656c 7365 3a0a 2020 2020 2020 2020 7365  else:.        se
+00000ce0: 7461 7474 7228 6f62 6a2c 206e 616d 652c  tattr(obj, name,
+00000cf0: 2061 7267 735b 305d 290a 0a0a 6465 6620   args[0])...def 
+00000d00: 6571 7561 6c5f 6174 7472 7328 6e61 6d65  equal_attrs(name
+00000d10: 3a20 7374 722c 202a 6f62 6a65 6374 7329  : str, *objects)
+00000d20: 3a0a 2020 2020 2222 2254 7275 6520 6966  :.    """True if
+00000d30: 2061 6c6c 206f 626a 6563 7473 2068 6176   all objects hav
+00000d40: 6520 7468 6520 6e61 6d65 6420 6174 7472  e the named attr
+00000d50: 6962 7574 6520 7769 7468 2065 7175 616c  ibute with equal
+00000d60: 2076 616c 7565 732e 2222 220a 2020 2020   values.""".    
+00000d70: 6966 206c 656e 286f 626a 6563 7473 2920  if len(objects) 
+00000d80: 3d3d 2030 3a0a 2020 2020 2020 2020 7261  == 0:.        ra
+00000d90: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00000da0: 4e6f 206f 626a 6563 7473 2074 6f20 636f  No objects to co
+00000db0: 6d70 6172 6522 290a 2020 2020 7472 793a  mpare").    try:
+00000dc0: 0a20 2020 2020 2020 2076 203d 2067 6574  .        v = get
+00000dd0: 6174 7472 286f 626a 6563 7473 5b30 5d2c  attr(objects[0],
+00000de0: 206e 616d 6529 0a20 2020 2065 7863 6570   name).    excep
+00000df0: 7420 4174 7472 6962 7574 6545 7272 6f72  t AttributeError
+00000e00: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00000e10: 2046 616c 7365 0a20 2020 2069 6620 6c65   False.    if le
+00000e20: 6e28 6f62 6a65 6374 7329 203d 3d20 313a  n(objects) == 1:
+00000e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000e40: 5472 7565 0a20 2020 2074 7279 3a0a 2020  True.    try:.  
+00000e50: 2020 2020 2020 7472 7574 6820 3d20 616c        truth = al
+00000e60: 6c28 6765 7461 7474 7228 692c 206e 616d  l(getattr(i, nam
+00000e70: 6529 203d 3d20 7620 666f 7220 6920 696e  e) == v for i in
+00000e80: 206f 626a 6563 7473 5b31 3a5d 290a 2020   objects[1:]).  
+00000e90: 2020 6578 6365 7074 2041 7474 7269 6275    except Attribu
+00000ea0: 7465 4572 726f 723a 0a20 2020 2020 2020  teError:.       
+00000eb0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+00000ec0: 2020 7265 7475 726e 2074 7275 7468 0a0a    return truth..
+00000ed0: 0a                                       .
```

### Comparing `goats-0.2.5/src/goats/core/algebraic.py` & `goats-0.2.6/src/goats/core/algebraic.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/aliased.py` & `goats-0.2.6/src/goats/core/aliased.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/axis.py` & `goats-0.2.6/src/goats/core/axis.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/computed.py` & `goats-0.2.6/src/goats/core/computed.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/constant.py` & `goats-0.2.6/src/goats/core/constant.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/datafile.py` & `goats-0.2.6/src/goats/core/datafile.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/fundamental.py` & `goats-0.2.6/src/goats/core/fundamental.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/index.py` & `goats-0.2.6/src/goats/core/index.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/interpolation.py` & `goats-0.2.6/src/goats/core/interpolation.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/iotools.py` & `goats-0.2.6/src/goats/core/iotools.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/iterables.py` & `goats-0.2.6/src/goats/core/iterables.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/measurable.py` & `goats-0.2.6/src/goats/core/measurable.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/metadata.py` & `goats-0.2.6/src/goats/core/metadata.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/metric.py` & `goats-0.2.6/src/goats/core/metric.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/numerical.py` & `goats-0.2.6/src/goats/core/numerical.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/observed.py` & `goats-0.2.6/src/goats/core/observed.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/observer.py` & `goats-0.2.6/src/goats/core/observer.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/observing.py` & `goats-0.2.6/src/goats/core/observing.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/operational.py` & `goats-0.2.6/src/goats/core/operational.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/physical.py` & `goats-0.2.6/src/goats/core/physical.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/plasma.py` & `goats-0.2.6/src/goats/core/plasma.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/reference.py` & `goats-0.2.6/src/goats/core/reference.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/spelling.py` & `goats-0.2.6/src/goats/core/spelling.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/symbolic.py` & `goats-0.2.6/src/goats/core/symbolic.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/core/variable.py` & `goats-0.2.6/src/goats/core/variable.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/eprem/__init__.py` & `goats-0.2.6/src/goats/eprem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,22 +194,18 @@
             ) -> index.Data:
                 s = self.species.compute([species]).points
                 t = (
                     numpy.squeeze(targets[s, :])
                     if getattr(targets, 'ndim', None) == 2
                     else targets
                 )
-                compute = self._build_coordinate(numpy.squeeze(this[s, :]))
+                array = numpy.squeeze(this[s, :]) if this.ndim == 2 else this
+                compute = self._build_coordinate(array)
                 return compute(t, unit)
-            try:
-                # Versions of EPREM with logically 2D egrid.
-                size = this.shape[1]
-            except IndexError:
-                # Versions of EPREM with truly 1D egrid.
-                size = this.shape[0]
+            size = this.shape[this.ndim-1]
             self._energy = axis.Indexer(method, size)
         return self._energy
 
     @property
     def species(self):
         """Indexer for the EPREM species dimension."""
         if self._species is None:
```

### Comparing `goats-0.2.5/src/goats/eprem/runtime.json` & `goats-0.2.6/src/goats/eprem/runtime.json`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/src/goats/eprem/runtime.py` & `goats-0.2.6/src/goats/eprem/runtime.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.5/setup.py` & `goats-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['matplotlib>=3.5.1,<4.0.0',
  'netCDF4>=1.5.8,<2.0.0',
  'numpy>=1.21.4,<1.23',
  'scipy>=1.7.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'goats',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'A set of tools for analyzing heliophysical datasets',
     'long_description': "# GOATS\n\nA set of tools for analyzing heliophysical datasets\n\nThe Generalized Observing Application Tool Suite (GOATS) is a collection of objects that support interactive and scripted analysis of simulated and observed data in heliophysics.\n\n## Installation\n\n```bash\n$ pip install goats\n```\n\n## Usage Example: EPREM\n\nThe [Energetic Particle Radiation Environment Module](https://github.com/myoung-space-science/eprem) (EPREM) simulates acceleration and transport of energetic particles throughout the heliosphere by modeling the focused transport equation on a Lagragian grid in the frame co-moving with the solar wind. It was the primary motivation for developing this package.\n\nThe first thing we'll do is import the packages we need.\n\n* `pathlib` is the built-in package for working with system paths  \n* `matplotlib` is a popular third-party package for creating figures  \n* `eprem` is the GOATS subpackage for working with EPREM output  \n\n\n```python\nimport pathlib\n\nimport matplotlib.pyplot as plt\n\nfrom goats import eprem\n```\n\nNext, we'll create a stream observer, which is the type of observer that corresponds to an EPREM output file with a name like `obs######.nc`. This invokation assumes that the data file, as well as an EPREM runtime parameter file called `eprem_input_file`, are in a local subdirectory called `data`.\n\nNote that if the data file is in the current directory, you can omit `source=<path/to/data>`.\n\n\n```python\nstream = eprem.Stream(350, source='data/example', config='eprem_input_file')\n```\n\nWe can request the value of simulation runtime parameters by aliased keyword. For example, let's check the assumed mean free path at 1 au.\n\n\n```python\nprint(stream['lambda0'])\n```\n\n    'lam0 | lambda0 | lamo': [1.] [au]\n\n\nThe text tells us that this simulation run used a value of 1.0 au (astronomical unit) for this parameter. It also suggests that we could have requested this value by the keywords 'lamo' or 'lam0'.\n\n\n```python\nprint(stream['lamo'])\nprint(stream['lam0'])\n```\n\n    'lam0 | lambda0 | lamo': [1.] [au]\n    'lam0 | lambda0 | lamo': [1.] [au]\n\n\nWe can also request observable quantities by aliased keyword. Here is the radial velocity.\n\n\n```python\nvr = stream['Vr']\nprint(vr)\n```\n\n    Observable('Vr', unit='m s^-1')\n\n\nThe text tells us that the radial velocity output array has a time axis and a shell axis. EPREM shells are logical surface of nodes in the Lagrangian grid. Each shell index along a given stream represents one node. We can observe radial velocity at a single time (e.g., 1 hour of real time since simulation start) on a single node as follows:\n\n\n```python\nt0 = 1.0, 'hour'\nvr.observe(time=t0, shell=1000)\n```\n\n\n\n\n    Observation(unit='m s^-1', dimensions=['time', 'shell'])\n\n\n\nIn the case of a constant isotropic solar wind, the stream nodes would extend radially outward from the Sun; with some trial-and-error, we could figure out which shell is closest to a particular radius (e.g., 1 au).\n\nInstead, we often want to interpolate an observation to the radius of interest.\n\n\n```python\nobserved = vr.observe(radius=[0.1, 'au'])\n```\n\nNow that we have an observation of the radial velocity at 0.1 au as a function of time, we can plot it. First, we'll define intermediate variables to hold the time in hours and the radial velocity in kilometers per second.\n\n\n```python\ntime = observed['time']\n```\n\nNext, we'll make sure there's a `figures` directory (to avoid cluttering the current directory) and load the plotting library.\n\n\n```python\nfigpath = pathlib.Path('figures').resolve()\nfigpath.mkdir(exist_ok=True)\n```\n\nFinally, we'll create and save the plot.\n\n\n```python\nplt.plot(time['hour'], observed['km / s'].array)\nplt.xlabel('Time [hours]')\nplt.ylabel('Vr [km/s]')\nplt.savefig(figpath / 'vr-hours.png')\n```\n\n\n    \n![png](readme_files/readme_25_0.png)\n    \n\n\nThere are many other observable quantities available to an observer, and they are not limited to those in the observer's source data.\n\n\n```python\nprint('flux' in stream.observables)\nprint('mean free path' in stream.observables)\n```\n\n    True\n    True\n\n\n\n```python\nstream['flux']\n```\n\n\n\n\n    Observable('flux', unit='J^-1 s^-1 sr^-1 m^-2')\n\n\n\n\n```python\nstream['mean free path']\n```\n\n\n\n\n    Observable('mean free path', unit='m')\n\n\n\nWe can even create observable quantities by symbolically composing existing observable quantities\n\n\n```python\nstream['mfp / Vr']\n```\n\n\n\n\n    Observable('mfp / Vr', unit='s')\n\n\n\n\n```python\nstream['rho * energy']\n```\n\n\n\n\n    Observable('rho * energy', unit='kg m^-1 s^-2')\n\n\n\nNote that the unit is consistent with the composed quantity and that the axes of the composed quantity represent the union of the axes of the component quantities.\n\nTo illustrate full use of a composed quantity, consider observing the ratio of the mean free path of protons with 1 and 5 MeV to the radial velocity of the solar wind.\n\n\n```python\nobserved = stream['mfp / Vr'].observe(radius=[0.1, 'au'], energy=[1, 5, 'MeV'])\nlines = plt.plot(observed['time']['hour'], observed.array)\nlines[0].set_label('1 MeV')\nlines[1].set_label('5 MeV')\nplt.xlabel('Time [hours]')\nplt.ylabel('mfp / Vr [s]')\nplt.legend()\nplt.savefig(figpath / 'mfp_vr-hours.png')\n```\n\n\n    \n![png](readme_files/readme_35_0.png)\n    \n\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`goats` was created by Matt Young. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`goats` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n\n",
     'author': 'Matt Young',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `goats-0.2.5/PKG-INFO` & `goats-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goats
-Version: 0.2.5
+Version: 0.2.6
 Summary: A set of tools for analyzing heliophysical datasets
 License: GNU General Public License v3.0
 Author: Matt Young
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

