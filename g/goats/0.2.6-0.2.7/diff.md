# Comparing `tmp/goats-0.2.6.tar.gz` & `tmp/goats-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goats-0.2.6.tar", max compression
+gzip compressed data, was "goats-0.2.7.tar", max compression
```

## Comparing `goats-0.2.6.tar` & `goats-0.2.7.tar`

### file list

```diff
@@ -1,36 +1,106 @@
--rwxr-xr-x   0        0        0    35092 2021-12-16 18:46:50.226668 goats-0.2.6/LICENSE
--rw-r--r--   0        0        0     5763 2023-03-31 13:27:39.249957 goats-0.2.6/README.md
--rw-r--r--   0        0        0      891 2023-05-05 14:25:07.491691 goats-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      180 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/__init__.py
--rw-r--r--   0        0        0        0 2022-03-09 16:57:39.661704 goats-0.2.6/src/goats/core/__init__.py
--rw-r--r--   0        0        0    11231 2022-11-10 16:10:01.591199 goats-0.2.6/src/goats/core/algebraic.py
--rw-r--r--   0        0        0    34484 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/aliased.py
--rw-r--r--   0        0        0     5465 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/axis.py
--rw-r--r--   0        0        0    16025 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/computed.py
--rw-r--r--   0        0        0     3107 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/constant.py
--rw-r--r--   0        0        0     8617 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/datafile.py
--rw-r--r--   0        0        0    14395 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/fundamental.py
--rw-r--r--   0        0        0     5772 2023-03-31 22:32:43.725018 goats-0.2.6/src/goats/core/index.py
--rw-r--r--   0        0        0     4610 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/interpolation.py
--rw-r--r--   0        0        0     6215 2022-11-10 16:10:01.595199 goats-0.2.6/src/goats/core/iotools.py
--rw-r--r--   0        0        0    55446 2023-03-31 13:27:39.253957 goats-0.2.6/src/goats/core/iterables.py
--rw-r--r--   0        0        0    15041 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/measurable.py
--rw-r--r--   0        0        0    36155 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/metadata.py
--rw-r--r--   0        0        0    88816 2023-02-10 19:09:53.043771 goats-0.2.6/src/goats/core/metric.py
--rw-r--r--   0        0        0     7769 2022-11-10 16:10:01.595199 goats-0.2.6/src/goats/core/numerical.py
--rw-r--r--   0        0        0     3066 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/observed.py
--rw-r--r--   0        0        0     3932 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/observer.py
--rw-r--r--   0        0        0    18362 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/observing.py
--rw-r--r--   0        0        0     7363 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/operational.py
--rw-r--r--   0        0        0    23342 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/physical.py
--rw-r--r--   0        0        0     1998 2022-11-10 16:10:01.599199 goats-0.2.6/src/goats/core/plasma.py
--rw-r--r--   0        0        0     3748 2023-03-31 16:19:23.081623 goats-0.2.6/src/goats/core/reference.py
--rw-r--r--   0        0        0     3835 2022-11-10 16:10:01.599199 goats-0.2.6/src/goats/core/spelling.py
--rw-r--r--   0        0        0    60269 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/symbolic.py
--rw-r--r--   0        0        0     3793 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/utilities.py
--rw-r--r--   0        0        0    26013 2023-03-31 13:27:39.257957 goats-0.2.6/src/goats/core/variable.py
--rw-r--r--   0        0        0    28499 2023-05-05 14:24:14.383449 goats-0.2.6/src/goats/eprem/__init__.py
--rw-r--r--   0        0        0    19888 2022-12-22 19:26:13.402833 goats-0.2.6/src/goats/eprem/runtime.json
--rw-r--r--   0        0        0    52655 2023-03-31 13:27:39.261958 goats-0.2.6/src/goats/eprem/runtime.py
--rw-r--r--   0        0        0     6765 2023-05-05 14:27:46.254380 goats-0.2.6/setup.py
--rw-r--r--   0        0        0     6411 2023-05-05 14:27:46.255319 goats-0.2.6/PKG-INFO
+-rwxr-xr-x   0        0        0    35092 2021-12-16 18:46:50.226668 goats-0.2.7/LICENSE
+-rw-r--r--   0        0        0     5763 2023-03-31 13:27:39.249957 goats-0.2.7/README.md
+-rw-r--r--   0        0        0      891 2023-05-05 15:25:52.330653 goats-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-03-31 13:27:39.253957 goats-0.2.7/src/goats/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-09 16:57:39.661704 goats-0.2.7/src/goats/core/__init__.py
+-rw-r--r--   0        0        0      144 2022-03-09 16:59:28.059858 goats-0.2.7/src/goats/core/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    22130 2022-03-22 17:16:46.881022 goats-0.2.7/src/goats/core/__pycache__/_variable.cpython-38.pyc
+-rw-r--r--   0        0        0    21994 2022-03-22 16:02:31.451964 goats-0.2.7/src/goats/core/__pycache__/_variable_dev.cpython-38.pyc
+-rw-r--r--   0        0        0    48757 2022-07-01 20:52:22.023182 goats-0.2.7/src/goats/core/__pycache__/algebra.cpython-38.pyc
+-rw-r--r--   0        0        0    14774 2022-11-10 16:11:39.965870 goats-0.2.7/src/goats/core/__pycache__/algebraic.cpython-38.pyc
+-rw-r--r--   0        0        0    38829 2023-04-19 01:16:02.493983 goats-0.2.7/src/goats/core/__pycache__/aliased.cpython-38.pyc
+-rw-r--r--   0        0        0     8386 2022-03-10 15:11:47.686199 goats-0.2.7/src/goats/core/__pycache__/arrays.cpython-38.pyc
+-rw-r--r--   0        0        0     5943 2023-04-19 01:16:02.509983 goats-0.2.7/src/goats/core/__pycache__/axis.cpython-38.pyc
+-rw-r--r--   0        0        0     9827 2022-07-27 17:26:43.898490 goats-0.2.7/src/goats/core/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0     2170 2022-01-07 17:19:07.111938 goats-0.2.7/src/goats/core/__pycache__/basetypes.cpython-38.pyc
+-rw-r--r--   0        0        0    16338 2022-11-22 17:36:06.196703 goats-0.2.7/src/goats/core/__pycache__/computable.cpython-38.pyc
+-rw-r--r--   0        0        0    16292 2023-04-19 01:16:02.677982 goats-0.2.7/src/goats/core/__pycache__/computed.cpython-38.pyc
+-rw-r--r--   0        0        0     3729 2023-04-19 01:16:02.689983 goats-0.2.7/src/goats/core/__pycache__/constant.cpython-38.pyc
+-rw-r--r--   0        0        0     5189 2022-01-10 22:56:00.293599 goats-0.2.7/src/goats/core/__pycache__/constants.cpython-38.pyc
+-rw-r--r--   0        0        0     6968 2022-01-18 23:56:53.599652 goats-0.2.7/src/goats/core/__pycache__/core.cpython-38.pyc
+-rw-r--r--   0        0        0    12442 2022-11-21 14:51:28.746827 goats-0.2.7/src/goats/core/__pycache__/data.cpython-38.pyc
+-rw-r--r--   0        0        0     9787 2022-11-17 22:41:35.409111 goats-0.2.7/src/goats/core/__pycache__/data_wip.cpython-38.pyc
+-rw-r--r--   0        0        0    10730 2023-04-19 01:16:02.509983 goats-0.2.7/src/goats/core/__pycache__/datafile.cpython-38.pyc
+-rw-r--r--   0        0        0    16991 2022-07-19 14:55:33.814895 goats-0.2.7/src/goats/core/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0     7253 2022-07-14 16:49:22.056633 goats-0.2.7/src/goats/core/__pycache__/datasets.cpython-38.pyc
+-rw-r--r--   0        0        0    19522 2022-07-14 17:56:57.431202 goats-0.2.7/src/goats/core/__pycache__/datatypes.cpython-38.pyc
+-rw-r--r--   0        0        0     8611 2021-12-16 21:31:48.045904 goats-0.2.7/src/goats/core/__pycache__/elements.cpython-38.pyc
+-rw-r--r--   0        0        0    19068 2022-09-19 16:09:37.838562 goats-0.2.7/src/goats/core/__pycache__/function.cpython-38.pyc
+-rw-r--r--   0        0        0    12864 2022-07-27 14:57:58.805104 goats-0.2.7/src/goats/core/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0        0        0    11294 2023-04-19 01:16:02.681983 goats-0.2.7/src/goats/core/__pycache__/fundamental.cpython-38.pyc
+-rw-r--r--   0        0        0     6737 2023-04-19 01:16:02.521983 goats-0.2.7/src/goats/core/__pycache__/index.cpython-38.pyc
+-rw-r--r--   0        0        0     5421 2022-07-15 14:27:32.568725 goats-0.2.7/src/goats/core/__pycache__/indexing.cpython-38.pyc
+-rw-r--r--   0        0        0     5075 2022-09-20 17:28:55.057583 goats-0.2.7/src/goats/core/__pycache__/interpolated.cpython-38.pyc
+-rw-r--r--   0        0        0     4118 2023-04-19 01:16:02.689983 goats-0.2.7/src/goats/core/__pycache__/interpolation.cpython-38.pyc
+-rw-r--r--   0        0        0     7926 2022-11-10 16:11:39.805872 goats-0.2.7/src/goats/core/__pycache__/iotools.cpython-38.pyc
+-rw-r--r--   0        0        0    65776 2023-04-19 01:16:02.501983 goats-0.2.7/src/goats/core/__pycache__/iterables.cpython-38.pyc
+-rw-r--r--   0        0        0    16929 2023-04-19 01:16:02.673982 goats-0.2.7/src/goats/core/__pycache__/measurable.cpython-38.pyc
+-rw-r--r--   0        0        0    31766 2022-04-06 20:23:37.149629 goats-0.2.7/src/goats/core/__pycache__/measurables.cpython-38.pyc
+-rw-r--r--   0        0        0    36538 2022-04-08 14:09:59.622538 goats-0.2.7/src/goats/core/__pycache__/measured.cpython-38.pyc
+-rw-r--r--   0        0        0    36552 2023-04-19 01:16:02.525983 goats-0.2.7/src/goats/core/__pycache__/metadata.cpython-38.pyc
+-rw-r--r--   0        0        0    75499 2023-02-15 17:54:20.005897 goats-0.2.7/src/goats/core/__pycache__/metric.cpython-38.pyc
+-rw-r--r--   0        0        0     8229 2022-11-10 16:11:39.813872 goats-0.2.7/src/goats/core/__pycache__/numerical.cpython-38.pyc
+-rw-r--r--   0        0        0     5915 2022-11-22 17:36:06.264703 goats-0.2.7/src/goats/core/__pycache__/observable.cpython-38.pyc
+-rw-r--r--   0        0        0     2171 2022-07-01 20:54:36.643243 goats-0.2.7/src/goats/core/__pycache__/observables.cpython-38.pyc
+-rw-r--r--   0        0        0     3479 2023-04-19 01:16:02.701983 goats-0.2.7/src/goats/core/__pycache__/observed.cpython-38.pyc
+-rw-r--r--   0        0        0     4548 2023-04-19 01:16:02.701983 goats-0.2.7/src/goats/core/__pycache__/observer.cpython-38.pyc
+-rw-r--r--   0        0        0    19375 2023-04-19 01:16:02.705983 goats-0.2.7/src/goats/core/__pycache__/observing.cpython-38.pyc
+-rw-r--r--   0        0        0     8003 2023-04-19 01:16:02.713982 goats-0.2.7/src/goats/core/__pycache__/operational.cpython-38.pyc
+-rw-r--r--   0        0        0    38511 2022-06-28 21:57:39.878542 goats-0.2.7/src/goats/core/__pycache__/operations.cpython-38.pyc
+-rw-r--r--   0        0        0    11659 2022-04-22 15:47:42.430493 goats-0.2.7/src/goats/core/__pycache__/operator.cpython-38.pyc
+-rw-r--r--   0        0        0     7089 2022-04-19 16:26:49.203113 goats-0.2.7/src/goats/core/__pycache__/operators.cpython-38.pyc
+-rw-r--r--   0        0        0     4139 2022-07-28 20:56:17.884099 goats-0.2.7/src/goats/core/__pycache__/parameter.cpython-38.pyc
+-rw-r--r--   0        0        0    25100 2023-04-19 01:16:02.681983 goats-0.2.7/src/goats/core/__pycache__/physical.cpython-38.pyc
+-rw-r--r--   0        0        0     2419 2022-11-10 16:11:40.509863 goats-0.2.7/src/goats/core/__pycache__/plasma.cpython-38.pyc
+-rw-r--r--   0        0        0    31765 2022-04-06 20:13:29.693312 goats-0.2.7/src/goats/core/__pycache__/quantified.cpython-38.pyc
+-rw-r--r--   0        0        0     3027 2022-07-20 22:48:20.145171 goats-0.2.7/src/goats/core/__pycache__/quantities.cpython-38.pyc
+-rw-r--r--   0        0        0     2720 2023-04-19 01:16:02.509983 goats-0.2.7/src/goats/core/__pycache__/reference.cpython-38.pyc
+-rw-r--r--   0        0        0     5546 2022-11-10 16:11:40.513863 goats-0.2.7/src/goats/core/__pycache__/spelling.cpython-38.pyc
+-rw-r--r--   0        0        0    59951 2023-04-19 01:16:02.533983 goats-0.2.7/src/goats/core/__pycache__/symbolic.cpython-38.pyc
+-rw-r--r--   0        0        0     4228 2023-04-19 01:16:02.665983 goats-0.2.7/src/goats/core/__pycache__/utilities.cpython-38.pyc
+-rw-r--r--   0        0        0    26742 2023-04-19 01:16:02.669983 goats-0.2.7/src/goats/core/__pycache__/variable.cpython-38.pyc
+-rw-r--r--   0        0        0    11231 2022-11-10 16:10:01.591199 goats-0.2.7/src/goats/core/algebraic.py
+-rw-r--r--   0        0        0    34484 2023-03-31 13:27:39.253957 goats-0.2.7/src/goats/core/aliased.py
+-rw-r--r--   0        0        0     5465 2023-03-31 13:27:39.253957 goats-0.2.7/src/goats/core/axis.py
+-rw-r--r--   0        0        0    16025 2023-03-31 13:27:39.253957 goats-0.2.7/src/goats/core/computed.py
+-rw-r--r--   0        0        0     3107 2023-03-31 13:27:39.253957 goats-0.2.7/src/goats/core/constant.py
+-rw-r--r--   0        0        0     8617 2023-03-31 13:27:39.253957 goats-0.2.7/src/goats/core/datafile.py
+-rw-r--r--   0        0        0    14395 2023-03-31 13:27:39.253957 goats-0.2.7/src/goats/core/fundamental.py
+-rw-r--r--   0        0        0     5772 2023-03-31 22:32:43.725018 goats-0.2.7/src/goats/core/index.py
+-rw-r--r--   0        0        0     4610 2023-03-31 13:27:39.253957 goats-0.2.7/src/goats/core/interpolation.py
+-rw-r--r--   0        0        0     6215 2022-11-10 16:10:01.595199 goats-0.2.7/src/goats/core/iotools.py
+-rw-r--r--   0        0        0    55446 2023-03-31 13:27:39.253957 goats-0.2.7/src/goats/core/iterables.py
+-rw-r--r--   0        0        0    15041 2023-03-31 13:27:39.257957 goats-0.2.7/src/goats/core/measurable.py
+-rw-r--r--   0        0        0    36155 2023-03-31 13:27:39.257957 goats-0.2.7/src/goats/core/metadata.py
+-rw-r--r--   0        0        0    88816 2023-02-10 19:09:53.043771 goats-0.2.7/src/goats/core/metric.py
+-rw-r--r--   0        0        0     7769 2022-11-10 16:10:01.595199 goats-0.2.7/src/goats/core/numerical.py
+-rw-r--r--   0        0        0     3066 2023-03-31 13:27:39.257957 goats-0.2.7/src/goats/core/observed.py
+-rw-r--r--   0        0        0     3932 2023-03-31 13:27:39.257957 goats-0.2.7/src/goats/core/observer.py
+-rw-r--r--   0        0        0    18362 2023-03-31 13:27:39.257957 goats-0.2.7/src/goats/core/observing.py
+-rw-r--r--   0        0        0     7363 2023-03-31 13:27:39.257957 goats-0.2.7/src/goats/core/operational.py
+-rw-r--r--   0        0        0    23342 2023-03-31 13:27:39.257957 goats-0.2.7/src/goats/core/physical.py
+-rw-r--r--   0        0        0     1998 2022-11-10 16:10:01.599199 goats-0.2.7/src/goats/core/plasma.py
+-rw-r--r--   0        0        0     3748 2023-03-31 16:19:23.081623 goats-0.2.7/src/goats/core/reference.py
+-rw-r--r--   0        0        0     3835 2022-11-10 16:10:01.599199 goats-0.2.7/src/goats/core/spelling.py
+-rw-r--r--   0        0        0    60269 2023-03-31 13:27:39.257957 goats-0.2.7/src/goats/core/symbolic.py
+-rw-r--r--   0        0        0     3793 2023-03-31 13:27:39.257957 goats-0.2.7/src/goats/core/utilities.py
+-rw-r--r--   0        0        0    26013 2023-03-31 13:27:39.257957 goats-0.2.7/src/goats/core/variable.py
+-rw-r--r--   0        0        0    28499 2023-05-05 15:25:52.330653 goats-0.2.7/src/goats/eprem/__init__.py
+-rw-r--r--   0        0        0    26443 2023-05-05 15:14:09.937871 goats-0.2.7/src/goats/eprem/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4460 2022-03-16 13:21:58.429352 goats-0.2.7/src/goats/eprem/__pycache__/_datasets.cpython-38.pyc
+-rw-r--r--   0        0        0     4646 2022-03-16 19:13:43.202027 goats-0.2.7/src/goats/eprem/__pycache__/_observing.cpython-38.pyc
+-rw-r--r--   0        0        0     6048 2022-01-27 03:28:43.616605 goats-0.2.7/src/goats/eprem/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0    13674 2022-01-10 18:23:13.849348 goats-0.2.7/src/goats/eprem/__pycache__/basetypes.cpython-38.pyc
+-rw-r--r--   0        0        0    11857 2022-03-16 19:13:43.698048 goats-0.2.7/src/goats/eprem/__pycache__/datasets.cpython-38.pyc
+-rw-r--r--   0        0        0     5867 2022-07-19 15:10:34.590171 goats-0.2.7/src/goats/eprem/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0        0        0     4021 2022-09-23 14:19:24.386407 goats-0.2.7/src/goats/eprem/__pycache__/interpolation.cpython-38.pyc
+-rw-r--r--   0        0        0     6376 2022-07-29 20:37:44.046549 goats-0.2.7/src/goats/eprem/__pycache__/observable.cpython-38.pyc
+-rw-r--r--   0        0        0    17900 2022-07-19 15:10:34.590171 goats-0.2.7/src/goats/eprem/__pycache__/observables.cpython-38.pyc
+-rw-r--r--   0        0        0     5420 2021-12-16 22:12:31.012722 goats-0.2.7/src/goats/eprem/__pycache__/observers.cpython-38.pyc
+-rw-r--r--   0        0        0     5908 2022-02-11 03:31:57.237338 goats-0.2.7/src/goats/eprem/__pycache__/observing.cpython-38.pyc
+-rw-r--r--   0        0        0    35437 2022-07-28 20:56:25.812120 goats-0.2.7/src/goats/eprem/__pycache__/parameters.cpython-38.pyc
+-rw-r--r--   0        0        0    47613 2023-04-19 01:16:02.713982 goats-0.2.7/src/goats/eprem/__pycache__/runtime.cpython-38.pyc
+-rw-r--r--   0        0        0    19888 2022-12-22 19:26:13.402833 goats-0.2.7/src/goats/eprem/runtime.json
+-rw-r--r--   0        0        0    52655 2023-03-31 13:27:39.261958 goats-0.2.7/src/goats/eprem/runtime.py
+-rw-r--r--   0        0        0     6765 2023-05-05 15:27:51.989500 goats-0.2.7/setup.py
+-rw-r--r--   0        0        0     6411 2023-05-05 15:27:51.989994 goats-0.2.7/PKG-INFO
```

### Comparing `goats-0.2.6/LICENSE` & `goats-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/README.md` & `goats-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/pyproject.toml` & `goats-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goats"
-version = "0.2.6"
+version = "0.2.7"
 description = "A set of tools for analyzing heliophysical datasets"
 authors = ["Matt Young"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `goats-0.2.6/src/goats/core/algebraic.py` & `goats-0.2.7/src/goats/core/algebraic.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/aliased.py` & `goats-0.2.7/src/goats/core/aliased.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/axis.py` & `goats-0.2.7/src/goats/core/axis.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/computed.py` & `goats-0.2.7/src/goats/core/computed.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/constant.py` & `goats-0.2.7/src/goats/core/constant.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/datafile.py` & `goats-0.2.7/src/goats/core/datafile.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/fundamental.py` & `goats-0.2.7/src/goats/core/fundamental.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/index.py` & `goats-0.2.7/src/goats/core/index.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/interpolation.py` & `goats-0.2.7/src/goats/core/interpolation.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/iotools.py` & `goats-0.2.7/src/goats/core/iotools.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/iterables.py` & `goats-0.2.7/src/goats/core/iterables.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/measurable.py` & `goats-0.2.7/src/goats/core/measurable.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/metadata.py` & `goats-0.2.7/src/goats/core/metadata.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/metric.py` & `goats-0.2.7/src/goats/core/metric.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/numerical.py` & `goats-0.2.7/src/goats/core/numerical.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/observed.py` & `goats-0.2.7/src/goats/core/observed.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/observer.py` & `goats-0.2.7/src/goats/core/observer.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/observing.py` & `goats-0.2.7/src/goats/core/observing.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/operational.py` & `goats-0.2.7/src/goats/core/operational.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/physical.py` & `goats-0.2.7/src/goats/core/physical.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/plasma.py` & `goats-0.2.7/src/goats/core/plasma.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/reference.py` & `goats-0.2.7/src/goats/core/reference.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/spelling.py` & `goats-0.2.7/src/goats/core/spelling.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/symbolic.py` & `goats-0.2.7/src/goats/core/symbolic.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/utilities.py` & `goats-0.2.7/src/goats/core/utilities.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/core/variable.py` & `goats-0.2.7/src/goats/core/variable.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/eprem/__init__.py` & `goats-0.2.7/src/goats/eprem/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,10 +814,10 @@
     ]
 
 
 class Point(Observer):
     """An EPREM point observer."""
 
     _templates = [
-        lambda n: f'p_obs{n:06}.nc',
+        lambda n: f'p_obs{n:03}.nc',
     ]
```

### Comparing `goats-0.2.6/src/goats/eprem/runtime.json` & `goats-0.2.7/src/goats/eprem/runtime.json`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/src/goats/eprem/runtime.py` & `goats-0.2.7/src/goats/eprem/runtime.py`

 * *Files identical despite different names*

### Comparing `goats-0.2.6/setup.py` & `goats-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['matplotlib>=3.5.1,<4.0.0',
  'netCDF4>=1.5.8,<2.0.0',
  'numpy>=1.21.4,<1.23',
  'scipy>=1.7.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'goats',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': 'A set of tools for analyzing heliophysical datasets',
     'long_description': "# GOATS\n\nA set of tools for analyzing heliophysical datasets\n\nThe Generalized Observing Application Tool Suite (GOATS) is a collection of objects that support interactive and scripted analysis of simulated and observed data in heliophysics.\n\n## Installation\n\n```bash\n$ pip install goats\n```\n\n## Usage Example: EPREM\n\nThe [Energetic Particle Radiation Environment Module](https://github.com/myoung-space-science/eprem) (EPREM) simulates acceleration and transport of energetic particles throughout the heliosphere by modeling the focused transport equation on a Lagragian grid in the frame co-moving with the solar wind. It was the primary motivation for developing this package.\n\nThe first thing we'll do is import the packages we need.\n\n* `pathlib` is the built-in package for working with system paths  \n* `matplotlib` is a popular third-party package for creating figures  \n* `eprem` is the GOATS subpackage for working with EPREM output  \n\n\n```python\nimport pathlib\n\nimport matplotlib.pyplot as plt\n\nfrom goats import eprem\n```\n\nNext, we'll create a stream observer, which is the type of observer that corresponds to an EPREM output file with a name like `obs######.nc`. This invokation assumes that the data file, as well as an EPREM runtime parameter file called `eprem_input_file`, are in a local subdirectory called `data`.\n\nNote that if the data file is in the current directory, you can omit `source=<path/to/data>`.\n\n\n```python\nstream = eprem.Stream(350, source='data/example', config='eprem_input_file')\n```\n\nWe can request the value of simulation runtime parameters by aliased keyword. For example, let's check the assumed mean free path at 1 au.\n\n\n```python\nprint(stream['lambda0'])\n```\n\n    'lam0 | lambda0 | lamo': [1.] [au]\n\n\nThe text tells us that this simulation run used a value of 1.0 au (astronomical unit) for this parameter. It also suggests that we could have requested this value by the keywords 'lamo' or 'lam0'.\n\n\n```python\nprint(stream['lamo'])\nprint(stream['lam0'])\n```\n\n    'lam0 | lambda0 | lamo': [1.] [au]\n    'lam0 | lambda0 | lamo': [1.] [au]\n\n\nWe can also request observable quantities by aliased keyword. Here is the radial velocity.\n\n\n```python\nvr = stream['Vr']\nprint(vr)\n```\n\n    Observable('Vr', unit='m s^-1')\n\n\nThe text tells us that the radial velocity output array has a time axis and a shell axis. EPREM shells are logical surface of nodes in the Lagrangian grid. Each shell index along a given stream represents one node. We can observe radial velocity at a single time (e.g., 1 hour of real time since simulation start) on a single node as follows:\n\n\n```python\nt0 = 1.0, 'hour'\nvr.observe(time=t0, shell=1000)\n```\n\n\n\n\n    Observation(unit='m s^-1', dimensions=['time', 'shell'])\n\n\n\nIn the case of a constant isotropic solar wind, the stream nodes would extend radially outward from the Sun; with some trial-and-error, we could figure out which shell is closest to a particular radius (e.g., 1 au).\n\nInstead, we often want to interpolate an observation to the radius of interest.\n\n\n```python\nobserved = vr.observe(radius=[0.1, 'au'])\n```\n\nNow that we have an observation of the radial velocity at 0.1 au as a function of time, we can plot it. First, we'll define intermediate variables to hold the time in hours and the radial velocity in kilometers per second.\n\n\n```python\ntime = observed['time']\n```\n\nNext, we'll make sure there's a `figures` directory (to avoid cluttering the current directory) and load the plotting library.\n\n\n```python\nfigpath = pathlib.Path('figures').resolve()\nfigpath.mkdir(exist_ok=True)\n```\n\nFinally, we'll create and save the plot.\n\n\n```python\nplt.plot(time['hour'], observed['km / s'].array)\nplt.xlabel('Time [hours]')\nplt.ylabel('Vr [km/s]')\nplt.savefig(figpath / 'vr-hours.png')\n```\n\n\n    \n![png](readme_files/readme_25_0.png)\n    \n\n\nThere are many other observable quantities available to an observer, and they are not limited to those in the observer's source data.\n\n\n```python\nprint('flux' in stream.observables)\nprint('mean free path' in stream.observables)\n```\n\n    True\n    True\n\n\n\n```python\nstream['flux']\n```\n\n\n\n\n    Observable('flux', unit='J^-1 s^-1 sr^-1 m^-2')\n\n\n\n\n```python\nstream['mean free path']\n```\n\n\n\n\n    Observable('mean free path', unit='m')\n\n\n\nWe can even create observable quantities by symbolically composing existing observable quantities\n\n\n```python\nstream['mfp / Vr']\n```\n\n\n\n\n    Observable('mfp / Vr', unit='s')\n\n\n\n\n```python\nstream['rho * energy']\n```\n\n\n\n\n    Observable('rho * energy', unit='kg m^-1 s^-2')\n\n\n\nNote that the unit is consistent with the composed quantity and that the axes of the composed quantity represent the union of the axes of the component quantities.\n\nTo illustrate full use of a composed quantity, consider observing the ratio of the mean free path of protons with 1 and 5 MeV to the radial velocity of the solar wind.\n\n\n```python\nobserved = stream['mfp / Vr'].observe(radius=[0.1, 'au'], energy=[1, 5, 'MeV'])\nlines = plt.plot(observed['time']['hour'], observed.array)\nlines[0].set_label('1 MeV')\nlines[1].set_label('5 MeV')\nplt.xlabel('Time [hours]')\nplt.ylabel('mfp / Vr [s]')\nplt.legend()\nplt.savefig(figpath / 'mfp_vr-hours.png')\n```\n\n\n    \n![png](readme_files/readme_35_0.png)\n    \n\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`goats` was created by Matt Young. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`goats` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n\n",
     'author': 'Matt Young',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `goats-0.2.6/PKG-INFO` & `goats-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goats
-Version: 0.2.6
+Version: 0.2.7
 Summary: A set of tools for analyzing heliophysical datasets
 License: GNU General Public License v3.0
 Author: Matt Young
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

