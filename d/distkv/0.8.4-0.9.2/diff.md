# Comparing `tmp/distkv-0.8.4.tar.gz` & `tmp/distkv-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/distkv-0.8.4.tar", last modified: Sat Jul 27 18:27:44 2019, max compression
+gzip compressed data, was "dist/distkv-0.9.2.tar", last modified: Thu Aug  1 11:06:11 2019, max compression
```

## Comparing `distkv-0.8.4.tar` & `distkv-0.9.2.tar`

### file list

```diff
@@ -1,141 +1,133 @@
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/
--rw-r--r--   0 smurf      (501) smurf      (501)      734 2019-03-20 14:29:08.000000 distkv-0.8.4/.appveyor.yml
--rw-r--r--   0 smurf      (501) smurf      (501)      112 2019-03-20 14:29:08.000000 distkv-0.8.4/.coveragerc
--rw-r--r--   0 smurf      (501) smurf      (501)      632 2019-07-19 19:52:02.000000 distkv-0.8.4/.gitignore
--rw-r--r--   0 smurf      (501) smurf      (501)      111 2019-07-19 19:52:02.000000 distkv-0.8.4/.pylintrc
--rw-r--r--   0 smurf      (501) smurf      (501)      364 2019-03-20 14:29:08.000000 distkv-0.8.4/.readthedocs.yml
--rw-r--r--   0 smurf      (501) smurf      (501)      508 2019-04-26 11:54:12.000000 distkv-0.8.4/.travis.yml
--rw-r--r--   0 smurf      (501) smurf      (501)      185 2019-03-20 14:29:08.000000 distkv-0.8.4/LICENSE
--rw-r--r--   0 smurf      (501) smurf      (501)    11358 2019-03-20 14:29:08.000000 distkv-0.8.4/LICENSE.APACHE2
--rw-r--r--   0 smurf      (501) smurf      (501)     1046 2019-03-20 14:29:08.000000 distkv-0.8.4/LICENSE.MIT
--rw-r--r--   0 smurf      (501) smurf      (501)      166 2019-04-29 09:10:26.000000 distkv-0.8.4/MANIFEST.in
--rw-r--r--   0 smurf      (501) smurf      (501)     1685 2019-07-26 20:07:10.000000 distkv-0.8.4/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)     2923 2019-07-27 18:27:44.000000 distkv-0.8.4/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)     1463 2019-07-19 19:52:02.000000 distkv-0.8.4/README.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/bin/
--rwxr-xr-x   0 smurf      (501) smurf      (501)      349 2019-07-26 20:06:57.000000 distkv-0.8.4/bin/distkv
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/ci/
--rw-r--r--   0 smurf      (501) smurf      (501)      123 2019-03-20 14:29:08.000000 distkv-0.8.4/ci/rtd-requirements.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       57 2019-04-29 09:10:26.000000 distkv-0.8.4/ci/test-requirements.txt
--rwxr-xr-x   0 smurf      (501) smurf      (501)     3290 2019-04-29 09:10:26.000000 distkv-0.8.4/ci/travis.sh
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/debian/
--rw-r--r--   0 smurf      (501) smurf      (501)       96 2019-07-27 12:42:13.000000 distkv-0.8.4/debian/.gitignore
--rw-r--r--   0 smurf      (501) smurf      (501)     1727 2019-07-27 18:27:40.000000 distkv-0.8.4/debian/changelog
--rw-r--r--   0 smurf      (501) smurf      (501)        2 2019-07-19 19:51:58.000000 distkv-0.8.4/debian/compat
--rw-r--r--   0 smurf      (501) smurf      (501)     1121 2019-07-27 13:24:16.000000 distkv-0.8.4/debian/control
--rw-r--r--   0 smurf      (501) smurf      (501)       32 2019-07-27 12:51:13.000000 distkv-0.8.4/debian/distkv.postinst
--rwxr-xr-x   0 smurf      (501) smurf      (501)      368 2019-07-27 12:41:51.000000 distkv-0.8.4/debian/rules
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/debian/source/
--rw-r--r--   0 smurf      (501) smurf      (501)       12 2019-07-19 19:51:58.000000 distkv-0.8.4/debian/source/format
--rw-r--r--   0 smurf      (501) smurf      (501)      191 2019-07-19 19:51:58.000000 distkv-0.8.4/debian/watch
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv/
--rw-r--r--   0 smurf      (501) smurf      (501)      338 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/__init__.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv/actor/
--rw-r--r--   0 smurf      (501) smurf      (501)     1591 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/actor/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4362 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/actor/deletor.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv/auth/
--rw-r--r--   0 smurf      (501) smurf      (501)    12427 2019-07-27 13:53:18.000000 distkv-0.8.4/distkv/auth/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4136 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/auth/_test.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5839 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/auth/password.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1196 2019-04-26 11:54:12.000000 distkv-0.8.4/distkv/auth/root.py
--rw-r--r--   0 smurf      (501) smurf      (501)    27042 2019-07-27 18:18:20.000000 distkv-0.8.4/distkv/client.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6333 2019-07-20 09:33:26.000000 distkv-0.8.4/distkv/code.py
--rw-r--r--   0 smurf      (501) smurf      (501)      601 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/codec.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv/command/
--rw-r--r--   0 smurf      (501) smurf      (501)     6644 2019-07-27 13:57:34.000000 distkv-0.8.4/distkv/command/__init__.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv/command/client/
--rw-r--r--   0 smurf      (501) smurf      (501)     2155 2019-07-27 13:59:43.000000 distkv-0.8.4/distkv/command/client/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5376 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/command/client/acl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5922 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/command/client/auth.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4693 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/command/client/code.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4438 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/command/client/codec.py
--rw-r--r--   0 smurf      (501) smurf      (501)     9211 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/command/client/data.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5269 2019-07-17 08:58:38.000000 distkv-0.8.4/distkv/command/client/error.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4408 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/command/client/internal.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1622 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/command/client/log.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6737 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/command/client/run.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5106 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/command/client/type.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2225 2019-07-20 14:27:06.000000 distkv-0.8.4/distkv/command/dump.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3538 2019-07-27 09:40:59.000000 distkv-0.8.4/distkv/command/server.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3859 2019-07-27 15:48:00.000000 distkv-0.8.4/distkv/default.py
--rw-r--r--   0 smurf      (501) smurf      (501)    14049 2019-07-20 09:33:33.000000 distkv-0.8.4/distkv/errors.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1485 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/exceptions.py
--rw-r--r--   0 smurf      (501) smurf      (501)    29145 2019-07-27 14:49:55.000000 distkv-0.8.4/distkv/model.py
--rw-r--r--   0 smurf      (501) smurf      (501)    14910 2019-07-20 09:34:07.000000 distkv-0.8.4/distkv/obj.py
--rw-r--r--   0 smurf      (501) smurf      (501)    22955 2019-07-20 09:33:37.000000 distkv-0.8.4/distkv/runner.py
--rw-r--r--   0 smurf      (501) smurf      (501)    85223 2019-07-27 18:23:53.000000 distkv-0.8.4/distkv/server.py
--rw-r--r--   0 smurf      (501) smurf      (501)    13558 2019-07-19 19:52:02.000000 distkv-0.8.4/distkv/types.py
--rw-r--r--   0 smurf      (501) smurf      (501)    16175 2019-07-20 14:07:21.000000 distkv-0.8.4/distkv/util.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv.egg-info/
--rw-r--r--   0 smurf      (501) smurf      (501)     2923 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv.egg-info/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)     2595 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv.egg-info/SOURCES.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv.egg-info/dependency_links.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       59 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv.egg-info/entry_points.txt
--rw-r--r--   0 smurf      (501) smurf      (501)      134 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv.egg-info/requires.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       13 2019-07-27 18:27:44.000000 distkv-0.8.4/distkv.egg-info/top_level.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2019-07-19 19:51:51.000000 distkv-0.8.4/distkv.egg-info/zip-safe
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/docs/
--rw-r--r--   0 smurf      (501) smurf      (501)      608 2019-03-20 14:29:08.000000 distkv-0.8.4/docs/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)      778 2019-03-20 14:29:08.000000 distkv-0.8.4/docs/make.bat
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/docs/source/
--rw-r--r--   0 smurf      (501) smurf      (501)     1619 2019-07-20 13:08:57.000000 distkv-0.8.4/docs/source/TODO.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/docs/source/_static/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2019-03-20 14:29:08.000000 distkv-0.8.4/docs/source/_static/.gitkeep
--rw-r--r--   0 smurf      (501) smurf      (501)     2020 2019-07-19 19:52:02.000000 distkv-0.8.4/docs/source/acls.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     1512 2019-07-19 19:52:02.000000 distkv-0.8.4/docs/source/auth.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    12006 2019-07-19 19:52:02.000000 distkv-0.8.4/docs/source/client_protocol.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     3681 2019-07-19 19:52:02.000000 distkv-0.8.4/docs/source/code.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    28186 2019-07-27 14:07:22.000000 distkv-0.8.4/docs/source/command_line.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     6022 2019-07-19 19:52:02.000000 distkv-0.8.4/docs/source/conf.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2206 2019-07-19 19:52:02.000000 distkv-0.8.4/docs/source/debugging.rst
--rw-r--r--   0 smurf      (501) smurf      (501)       93 2019-03-20 14:29:08.000000 distkv-0.8.4/docs/source/history.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     1743 2019-07-20 14:35:01.000000 distkv-0.8.4/docs/source/index.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     1562 2019-07-19 19:52:02.000000 distkv-0.8.4/docs/source/model.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     3438 2019-07-19 19:52:02.000000 distkv-0.8.4/docs/source/overview.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    15460 2019-07-19 19:52:02.000000 distkv-0.8.4/docs/source/server_protocol.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     1110 2019-07-27 06:36:15.000000 distkv-0.8.4/docs/source/startup.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     7110 2019-07-19 19:52:02.000000 distkv-0.8.4/docs/source/translator.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    17115 2019-07-20 09:33:55.000000 distkv-0.8.4/docs/source/tutorial.rst
--rwxr-xr-x   0 smurf      (501) smurf      (501)      195 2019-03-20 14:29:08.000000 distkv-0.8.4/mktag
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/newsfragments/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2019-03-20 14:29:08.000000 distkv-0.8.4/newsfragments/.gitkeep
--rw-r--r--   0 smurf      (501) smurf      (501)     1393 2019-03-20 14:29:08.000000 distkv-0.8.4/newsfragments/README.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      211 2019-03-20 14:29:08.000000 distkv-0.8.4/pyproject.toml
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/scripts/
--rwxr-xr-x   0 smurf      (501) smurf      (501)      374 2019-07-27 12:49:54.000000 distkv-0.8.4/scripts/current
--rw-r--r--   0 smurf      (501) smurf      (501)      111 2019-07-27 06:20:40.000000 distkv-0.8.4/scripts/env
--rwxr-xr-x   0 smurf      (501) smurf      (501)      782 2019-07-27 13:27:11.000000 distkv-0.8.4/scripts/init
--rwxr-xr-x   0 smurf      (501) smurf      (501)      331 2019-07-27 06:24:30.000000 distkv-0.8.4/scripts/recover
--rwxr-xr-x   0 smurf      (501) smurf      (501)      381 2019-07-27 14:10:16.000000 distkv-0.8.4/scripts/rotate
--rwxr-xr-x   0 smurf      (501) smurf      (501)      359 2019-07-27 09:52:40.000000 distkv-0.8.4/scripts/run
--rwxr-xr-x   0 smurf      (501) smurf      (501)       33 2019-07-27 06:23:19.000000 distkv-0.8.4/scripts/success
--rw-r--r--   0 smurf      (501) smurf      (501)      237 2019-07-27 18:27:44.000000 distkv-0.8.4/setup.cfg
--rw-r--r--   0 smurf      (501) smurf      (501)     1858 2019-07-20 10:58:08.000000 distkv-0.8.4/setup.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/systemd/
--rw-r--r--   0 smurf      (501) smurf      (501)      322 2019-07-27 06:29:21.000000 distkv-0.8.4/systemd/distkv-recover.service
--rw-r--r--   0 smurf      (501) smurf      (501)      314 2019-07-27 18:12:38.000000 distkv-0.8.4/systemd/distkv-rotate.service
--rw-r--r--   0 smurf      (501) smurf      (501)      158 2019-07-26 20:22:49.000000 distkv-0.8.4/systemd/distkv-rotate.timer
--rw-r--r--   0 smurf      (501) smurf      (501)      421 2019-07-27 06:12:55.000000 distkv-0.8.4/systemd/distkv.service
--rw-r--r--   0 smurf      (501) smurf      (501)      169 2019-07-27 07:52:22.000000 distkv-0.8.4/systemd/postinst
--rw-r--r--   0 smurf      (501) smurf      (501)       49 2019-07-21 10:08:12.000000 distkv-0.8.4/systemd/sysusers
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-07-27 18:27:44.000000 distkv-0.8.4/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)     1040 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)      175 2019-04-29 09:10:26.000000 distkv-0.8.4/tests/conftest.py
--rw-r--r--   0 smurf      (501) smurf      (501)      446 2019-03-20 14:29:08.000000 distkv-0.8.4/tests/logging.cfg
--rw-r--r--   0 smurf      (501) smurf      (501)     8439 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/mock_serf.py
--rw-r--r--   0 smurf      (501) smurf      (501)      704 2019-07-27 14:01:20.000000 distkv-0.8.4/tests/run.py
--rw-r--r--   0 smurf      (501) smurf      (501)    12598 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_basic.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1573 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_feature_acl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4812 2019-07-27 14:01:36.000000 distkv-0.8.4/tests/test_feature_auth.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1328 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_feature_code.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3302 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_feature_convert.py
--rw-r--r--   0 smurf      (501) smurf      (501)      532 2019-04-29 09:10:26.000000 distkv-0.8.4/tests/test_feature_dh.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2573 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_feature_error.py
--rw-r--r--   0 smurf      (501) smurf      (501)      750 2019-04-29 09:10:26.000000 distkv-0.8.4/tests/test_feature_mirror.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2055 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_feature_runner.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2079 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_feature_singlerunner.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3338 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_feature_ssl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7297 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_feature_typecheck.py
--rw-r--r--   0 smurf      (501) smurf      (501)    11834 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_load_save.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6188 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_multi.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1891 2019-07-19 19:52:02.000000 distkv-0.8.4/tests/test_passthru.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/
+-rw-r--r--   0 smurf      (501) smurf      (501)      734 2019-03-20 14:29:08.000000 distkv-0.9.2/.appveyor.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)      112 2019-03-20 14:29:08.000000 distkv-0.9.2/.coveragerc
+-rw-r--r--   0 smurf      (501) smurf      (501)      621 2019-08-01 11:06:02.000000 distkv-0.9.2/.gitignore
+-rw-r--r--   0 smurf      (501) smurf      (501)      111 2019-07-19 19:52:02.000000 distkv-0.9.2/.pylintrc
+-rw-r--r--   0 smurf      (501) smurf      (501)      364 2019-03-20 14:29:08.000000 distkv-0.9.2/.readthedocs.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)      508 2019-04-26 11:54:12.000000 distkv-0.9.2/.travis.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)      185 2019-03-20 14:29:08.000000 distkv-0.9.2/LICENSE
+-rw-r--r--   0 smurf      (501) smurf      (501)    11358 2019-03-20 14:29:08.000000 distkv-0.9.2/LICENSE.APACHE2
+-rw-r--r--   0 smurf      (501) smurf      (501)     1046 2019-03-20 14:29:08.000000 distkv-0.9.2/LICENSE.MIT
+-rw-r--r--   0 smurf      (501) smurf      (501)      166 2019-04-29 09:10:26.000000 distkv-0.9.2/MANIFEST.in
+-rw-r--r--   0 smurf      (501) smurf      (501)     1685 2019-08-01 11:04:48.000000 distkv-0.9.2/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)     2923 2019-08-01 11:06:11.000000 distkv-0.9.2/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)     1463 2019-07-19 19:52:02.000000 distkv-0.9.2/README.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/bin/
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      349 2019-08-01 11:04:48.000000 distkv-0.9.2/bin/distkv
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/ci/
+-rw-r--r--   0 smurf      (501) smurf      (501)      123 2019-03-20 14:29:08.000000 distkv-0.9.2/ci/rtd-requirements.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       57 2019-04-29 09:10:26.000000 distkv-0.9.2/ci/test-requirements.txt
+-rwxr-xr-x   0 smurf      (501) smurf      (501)     3290 2019-04-29 09:10:26.000000 distkv-0.9.2/ci/travis.sh
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv/
+-rw-r--r--   0 smurf      (501) smurf      (501)      338 2019-07-19 19:52:02.000000 distkv-0.9.2/distkv/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv/actor/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1591 2019-07-19 19:52:02.000000 distkv-0.9.2/distkv/actor/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4362 2019-07-19 19:52:02.000000 distkv-0.9.2/distkv/actor/deletor.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv/auth/
+-rw-r--r--   0 smurf      (501) smurf      (501)    12427 2019-08-01 11:04:48.000000 distkv-0.9.2/distkv/auth/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4136 2019-07-19 19:52:02.000000 distkv-0.9.2/distkv/auth/_test.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5839 2019-07-19 19:52:02.000000 distkv-0.9.2/distkv/auth/password.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1196 2019-04-26 11:54:12.000000 distkv-0.9.2/distkv/auth/root.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    28829 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/client.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6333 2019-08-01 11:04:48.000000 distkv-0.9.2/distkv/code.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      601 2019-07-19 19:52:02.000000 distkv-0.9.2/distkv/codec.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv/command/
+-rw-r--r--   0 smurf      (501) smurf      (501)     6644 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv/command/client/
+-rw-r--r--   0 smurf      (501) smurf      (501)     2165 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/client/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5140 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/client/acl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5727 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/client/auth.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4680 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/client/code.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4425 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/client/codec.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     9198 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/client/data.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5269 2019-07-17 08:58:38.000000 distkv-0.9.2/distkv/command/client/error.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4395 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/client/internal.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1609 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/client/log.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6724 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/client/run.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5093 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/client/type.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3269 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/dump.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3525 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/command/server.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1192 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/config.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3910 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/default.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    14049 2019-08-01 11:04:48.000000 distkv-0.9.2/distkv/errors.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1485 2019-07-19 19:52:02.000000 distkv-0.9.2/distkv/exceptions.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    29145 2019-08-01 11:04:48.000000 distkv-0.9.2/distkv/model.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    14750 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/obj.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    22955 2019-08-01 11:04:48.000000 distkv-0.9.2/distkv/runner.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    85235 2019-08-01 11:05:52.000000 distkv-0.9.2/distkv/server.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    13558 2019-07-19 19:52:02.000000 distkv-0.9.2/distkv/types.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    16175 2019-08-01 11:04:48.000000 distkv-0.9.2/distkv/util.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)     2923 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv.egg-info/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)     2507 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       59 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv.egg-info/entry_points.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)      134 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       13 2019-08-01 11:06:11.000000 distkv-0.9.2/distkv.egg-info/top_level.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2019-07-19 19:51:51.000000 distkv-0.9.2/distkv.egg-info/zip-safe
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/docs/
+-rw-r--r--   0 smurf      (501) smurf      (501)      608 2019-03-20 14:29:08.000000 distkv-0.9.2/docs/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)      778 2019-03-20 14:29:08.000000 distkv-0.9.2/docs/make.bat
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/docs/source/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1663 2019-08-01 11:05:52.000000 distkv-0.9.2/docs/source/TODO.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/docs/source/_static/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2019-03-20 14:29:08.000000 distkv-0.9.2/docs/source/_static/.gitkeep
+-rw-r--r--   0 smurf      (501) smurf      (501)     2020 2019-07-19 19:52:02.000000 distkv-0.9.2/docs/source/acls.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     1512 2019-07-19 19:52:02.000000 distkv-0.9.2/docs/source/auth.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    12006 2019-07-19 19:52:02.000000 distkv-0.9.2/docs/source/client_protocol.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     3681 2019-07-19 19:52:02.000000 distkv-0.9.2/docs/source/code.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    28828 2019-08-01 11:04:48.000000 distkv-0.9.2/docs/source/command_line.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     6022 2019-07-19 19:52:02.000000 distkv-0.9.2/docs/source/conf.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2206 2019-07-19 19:52:02.000000 distkv-0.9.2/docs/source/debugging.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)       93 2019-03-20 14:29:08.000000 distkv-0.9.2/docs/source/history.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     1743 2019-08-01 11:04:48.000000 distkv-0.9.2/docs/source/index.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     1562 2019-07-19 19:52:02.000000 distkv-0.9.2/docs/source/model.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     3438 2019-07-19 19:52:02.000000 distkv-0.9.2/docs/source/overview.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    15460 2019-07-19 19:52:02.000000 distkv-0.9.2/docs/source/server_protocol.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     1110 2019-08-01 11:04:48.000000 distkv-0.9.2/docs/source/startup.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     7110 2019-07-19 19:52:02.000000 distkv-0.9.2/docs/source/translator.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    17806 2019-08-01 11:05:52.000000 distkv-0.9.2/docs/source/tutorial.rst
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      195 2019-03-20 14:29:08.000000 distkv-0.9.2/mktag
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/newsfragments/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2019-03-20 14:29:08.000000 distkv-0.9.2/newsfragments/.gitkeep
+-rw-r--r--   0 smurf      (501) smurf      (501)     1393 2019-03-20 14:29:08.000000 distkv-0.9.2/newsfragments/README.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      211 2019-03-20 14:29:08.000000 distkv-0.9.2/pyproject.toml
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/scripts/
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      374 2019-08-01 11:04:48.000000 distkv-0.9.2/scripts/current
+-rw-r--r--   0 smurf      (501) smurf      (501)      111 2019-08-01 11:04:48.000000 distkv-0.9.2/scripts/env
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      782 2019-08-01 11:04:48.000000 distkv-0.9.2/scripts/init
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      331 2019-08-01 11:04:48.000000 distkv-0.9.2/scripts/recover
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      381 2019-08-01 11:04:48.000000 distkv-0.9.2/scripts/rotate
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      359 2019-08-01 11:04:48.000000 distkv-0.9.2/scripts/run
+-rwxr-xr-x   0 smurf      (501) smurf      (501)       33 2019-08-01 11:04:48.000000 distkv-0.9.2/scripts/success
+-rw-r--r--   0 smurf      (501) smurf      (501)      237 2019-08-01 11:06:11.000000 distkv-0.9.2/setup.cfg
+-rw-r--r--   0 smurf      (501) smurf      (501)     1858 2019-08-01 11:05:52.000000 distkv-0.9.2/setup.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/systemd/
+-rw-r--r--   0 smurf      (501) smurf      (501)      322 2019-08-01 11:04:48.000000 distkv-0.9.2/systemd/distkv-recover.service
+-rw-r--r--   0 smurf      (501) smurf      (501)      314 2019-08-01 11:04:48.000000 distkv-0.9.2/systemd/distkv-rotate.service
+-rw-r--r--   0 smurf      (501) smurf      (501)      158 2019-08-01 11:04:48.000000 distkv-0.9.2/systemd/distkv-rotate.timer
+-rw-r--r--   0 smurf      (501) smurf      (501)      421 2019-08-01 11:04:48.000000 distkv-0.9.2/systemd/distkv.service
+-rw-r--r--   0 smurf      (501) smurf      (501)      169 2019-08-01 11:04:48.000000 distkv-0.9.2/systemd/postinst
+-rw-r--r--   0 smurf      (501) smurf      (501)       49 2019-08-01 11:04:48.000000 distkv-0.9.2/systemd/sysusers
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2019-08-01 11:06:11.000000 distkv-0.9.2/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1040 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      175 2019-04-29 09:10:26.000000 distkv-0.9.2/tests/conftest.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      446 2019-03-20 14:29:08.000000 distkv-0.9.2/tests/logging.cfg
+-rw-r--r--   0 smurf      (501) smurf      (501)     8453 2019-08-01 11:05:52.000000 distkv-0.9.2/tests/mock_serf.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      704 2019-08-01 11:05:52.000000 distkv-0.9.2/tests/run.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    12597 2019-08-01 11:05:52.000000 distkv-0.9.2/tests/test_basic.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1573 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_feature_acl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4812 2019-07-27 14:01:36.000000 distkv-0.9.2/tests/test_feature_auth.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1328 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_feature_code.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      738 2019-08-01 11:05:52.000000 distkv-0.9.2/tests/test_feature_config.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3302 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_feature_convert.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      532 2019-04-29 09:10:26.000000 distkv-0.9.2/tests/test_feature_dh.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2573 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_feature_error.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      750 2019-04-29 09:10:26.000000 distkv-0.9.2/tests/test_feature_mirror.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2055 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_feature_runner.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2079 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_feature_singlerunner.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3338 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_feature_ssl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7297 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_feature_typecheck.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    11834 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_load_save.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6188 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_multi.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1891 2019-07-19 19:52:02.000000 distkv-0.9.2/tests/test_passthru.py
```

### Comparing `distkv-0.8.4/.appveyor.yml` & `distkv-0.9.2/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/.gitignore` & `distkv-0.9.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -57,8 +57,7 @@
 
 # Django stuff:
 *.log
 *.pot
 
 # Local test tools
 /kv
-/.pybuild/
```

### Comparing `distkv-0.8.4/LICENSE.APACHE2` & `distkv-0.9.2/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/LICENSE.MIT` & `distkv-0.9.2/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/Makefile` & `distkv-0.9.2/Makefile`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/PKG-INFO` & `distkv-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: distkv
-Version: 0.8.4
+Version: 0.9.2
 Summary: A distributed no-master key-value store
 Home-page: https://github.com/smurfix/distkv
 Author: Matthias Urlichs
 Author-email: matthias@urlichs.de
 License: MIT -or- Apache License 2.0
 Description: ======
         DistKV
```

### Comparing `distkv-0.8.4/README.rst` & `distkv-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/ci/travis.sh` & `distkv-0.9.2/ci/travis.sh`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/actor/__init__.py` & `distkv-0.9.2/distkv/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/actor/deletor.py` & `distkv-0.9.2/distkv/actor/deletor.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/auth/__init__.py` & `distkv-0.9.2/distkv/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/auth/_test.py` & `distkv-0.9.2/distkv/auth/_test.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/auth/password.py` & `distkv-0.9.2/distkv/auth/password.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/auth/root.py` & `distkv-0.9.2/distkv/auth/root.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/client.py` & `distkv-0.9.2/distkv/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,62 @@
         """
         return await self.q.get()
 
     async def cancel(self):
         pass
 
 
+class _ClientConfig:
+    """Accessor for configuration, possibly stored in DistKV.
+    """
+    def __init__(self, client, *a, **k):
+        self._init(client)
+        super().__init__(client, *a, **k)
+
+    def _init(self, client):
+        self._client = client
+        self._current = {}
+        self._changed = anyio.create_event()
+
+    def __getattr__(self, k):
+        if k.startswith('_'):
+            return object.__getattribute__(self, k)
+        v = self._current.get(k, NotGiven)
+        if v is NotGiven:
+            try:
+                v = self._client._cfg[k]
+            except KeyError:
+                raise AttributeError(k) from None
+        return v
+
+    def __contains__(self, k):
+        return k in self._current or k in self._client._cfg
+
+    async def _update(self, k, v):
+        """
+        Update this config entry. The new data is combined with the static
+        configuration; the old data is discarded.
+        """
+        self._current[k] = combine_dict(v, self._client._cfg.get(k, {}))
+        c, self._changed = self._changed, anyio.create_event()
+        await c.set()
+
+    async def _watch(self):
+        class CfgWatcher:
+            def __ainit__(slf):
+                return slf
+            async def __anext__(slf):
+                await self._changed.wait()
+        return CfgWatcher()
+
+class ClientConfig(_ClientConfig):
+    def __init__(self, client):
+        self._init(client)
+
+
 class Client:
     """
     The client side of a DistKV connection.
 
     Use :func:`open_client` to use this class.
     """
 
@@ -257,15 +305,16 @@
     _dh_key = None
     exit_stack = None
 
     server_name = None
     client_name = None
 
     def __init__(self, cfg: dict):
-        self._cfg = combine_dict(cfg, CFG.connect, cls=attrdict)
+        self._cfg = combine_dict(cfg, CFG, cls=attrdict)
+        self.config = ClientConfig(self)
 
         self._seq = 0
         self._handlers = {}
         self._send_lock = anyio.create_lock()
         self._helpers = {}
         self._name = "".join(random.choices("abcdefghjkmnopqrstuvwxyz23456789", k=9))
 
@@ -531,22 +580,23 @@
         """
         This async context manager handles the actual TCP connection to
         the DistKV server.
         """
         hello = ValueEvent()
         self._handlers[0] = hello
 
-        host = self._cfg["host"]
-        port = self._cfg["port"]
-        auth = self._cfg["auth"]
+        cfg = self._cfg['connect']
+        host = cfg["host"]
+        port = cfg["port"]
+        auth = cfg["auth"]
         if auth is not None:
             from .auth import gen_auth
             auth = gen_auth(auth)
-        init_timeout = self._cfg["init_timeout"]
-        ssl = gen_ssl(self._cfg["ssl"], server=False)
+        init_timeout = cfg["init_timeout"]
+        ssl = gen_ssl(cfg["ssl"], server=False)
 
         # logger.debug("Conn %s %s",self.host,self.port)
         async with AsyncExitStack() as ex:
             self.exit_stack = ex
             try:
                 ctx = await anyio.connect_tcp(
                     host, port, ssl_context=ssl, autostart_tls=False
@@ -560,26 +610,37 @@
             try:
                 self.tg = tg
                 self._socket = stream
                 await self.tg.spawn(self._reader)
                 async with anyio.fail_after(init_timeout):
                     self._server_init = await hello.get()
                     self.server_name = self._server_init.node
-                    self.client_name = self._cfg["name"] or self.server_name
+                    self.client_name = cfg["name"] or self.server_name
                     await self._run_auth(auth)
+
+                from .config import ConfigRoot
+                self._config = await ConfigRoot.as_handler(self)
+
                 yield self
             except socket.error as e:
                 raise ServerConnectionError(host, port) from e
             else:
                 # This is intentionally not in the error path
                 # cancelling the nursey causes open_client() to
                 # exit without a yield which triggers an async error,
                 # which masks the exception
                 pass
             finally:
+                # Clean up our hacked config
+                try:
+                    del self._config
+                except AttributeError:
+                    pass
+                self.config = ClientConfig(self)
+
                 async with anyio.open_cancel_scope(shield=True):
                     await self.tg.cancel_scope.cancel()
                     if self._socket is not None:
                         async with self._send_lock:
                             await self._socket.close()
                         self._socket = None
                     self.tg = None
```

### Comparing `distkv-0.8.4/distkv/code.py` & `distkv-0.9.2/distkv/code.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/codec.py` & `distkv-0.9.2/distkv/codec.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/command/__init__.py` & `distkv-0.9.2/distkv/command/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 import yaml
 from functools import partial
 
 from ..util import attrdict, combine_dict, NotGiven
 from ..default import CFG
 
 from ..exceptions import ClientError, ServerError
```

### Comparing `distkv-0.8.4/distkv/command/client/__init__.py` & `distkv-0.9.2/distkv/command/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 import json
 from functools import partial
 
 from distkv.util import (
     attrdict,
     combine_dict,
     PathLongener,
@@ -78,15 +78,15 @@
         cfg.port = port
 
     if auth is not None:
         cfg.auth = gen_auth(auth)
         if obj._DEBUG:
             cfg.auth._DEBUG = True
 
-    cfg = combine_dict(cfg, obj.cfg.connect, cls=attrdict)
+    cfg = combine_dict(attrdict(connect=cfg), obj.cfg, cls=attrdict)
 
     obj.meta = 3 if metadata else False
 
     try:
         obj.client = await ctx.enter_async_context(open_client(**cfg))
     except OSError as exc:
         obj.client = NullObj(exc)
```

### Comparing `distkv-0.8.4/distkv/command/client/acl.py` & `distkv-0.9.2/distkv/command/client/acl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 import json
 
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
-from distkv.command import Loader
-from distkv.default import CFG
-from distkv.server import Server
-from distkv.auth import loader, gen_auth
-from distkv.exceptions import ClientError
 from distkv.util import yprint
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 ACL = set("rwdcxena")
```

### Comparing `distkv-0.8.4/distkv/command/client/auth.py` & `distkv-0.9.2/distkv/command/client/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 import json
 
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
-from distkv.command import Loader
-from distkv.default import CFG
-from distkv.server import Server
 from distkv.auth import loader, gen_auth
-from distkv.exceptions import ClientError
 from distkv.util import yprint
 
 import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `distkv-0.8.4/distkv/command/client/code.py` & `distkv-0.9.2/distkv/command/client/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 import yaml
 
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
+from distkv.client import StreamedRequest
 from distkv.command import Loader
 from distkv.default import CFG
 from distkv.server import Server
 from distkv.auth import loader, gen_auth
 from distkv.exceptions import ClientError
 from distkv.util import yprint
```

### Comparing `distkv-0.8.4/distkv/command/client/codec.py` & `distkv-0.9.2/distkv/command/client/codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 import yaml
 
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
+from distkv.client import StreamedRequest
 from distkv.command import Loader
 from distkv.default import CFG
 from distkv.server import Server
 from distkv.auth import loader, gen_auth
 from distkv.exceptions import ClientError
 from distkv.util import yprint
```

### Comparing `distkv-0.8.4/distkv/command/client/data.py` & `distkv-0.9.2/distkv/command/client/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
+from distkv.client import StreamedRequest
 from distkv.command import Loader
 from distkv.default import CFG
 from distkv.server import Server
 from distkv.auth import loader, gen_auth
 from distkv.exceptions import ClientError
 from distkv.util import yprint
```

### Comparing `distkv-0.8.4/distkv/command/client/error.py` & `distkv-0.9.2/distkv/command/client/error.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/command/client/internal.py` & `distkv-0.9.2/distkv/command/client/internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 
 from range_set import RangeSet
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
+from distkv.client import StreamedRequest
 from distkv.command import Loader
 from distkv.default import CFG
 from distkv.server import Server
 from distkv.auth import loader, gen_auth
 from distkv.exceptions import ClientError
 from distkv.util import yprint
```

### Comparing `distkv-0.8.4/distkv/command/client/log.py` & `distkv-0.9.2/distkv/command/client/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 import json
 
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
+from distkv.client import StreamedRequest
 from distkv.command import Loader
 from distkv.default import CFG
 from distkv.server import Server
 from distkv.auth import loader, gen_auth
 from distkv.exceptions import ClientError
 
 import logging
```

### Comparing `distkv-0.8.4/distkv/command/client/run.py` & `distkv-0.9.2/distkv/command/client/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 import time
 import anyio
 
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
+from distkv.client import StreamedRequest
 from distkv.command import Loader
 from distkv.default import CFG
 from distkv.server import Server
 from distkv.auth import loader, gen_auth
 from distkv.exceptions import ClientError, ServerError
 from distkv.code import CodeRoot
 from distkv.runner import AnyRunnerRoot, SingleRunnerRoot
```

### Comparing `distkv-0.8.4/distkv/command/client/type.py` & `distkv-0.9.2/distkv/command/client/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 import json
 import yaml
 
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
+from distkv.client import StreamedRequest
 from distkv.command import Loader
 from distkv.default import CFG
 from distkv.server import Server
 from distkv.auth import loader, gen_auth
 from distkv.exceptions import ClientError
 from distkv.util import yprint
```

### Comparing `distkv-0.8.4/distkv/command/dump.py` & `distkv-0.9.2/distkv/command/dump.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
+from distkv.util import MsgReader
+from functools import partial
 from distkv.util import MsgReader, MsgWriter
 
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
+from distkv.client import StreamedRequest
 from distkv.default import CFG
 from distkv.server import Server
 from distkv.auth import loader, gen_auth
 from distkv.exceptions import ClientError
 from distkv.util import yprint
 
 import logging
@@ -82,7 +84,38 @@
 
     Using this command, followed by "distkv server -l <outfile> <node>", is
     equivalent to running "distkv server -i 'Initial data' <node>.
     """
     async with MsgWriter(path=file) as f:
         await f(dict(chain=dict(node=node,tick=1,prev=None),depth=0,path=[],tock=1,value="Initial data"))
 
+@cli.command()
+@click.pass_obj
+async def serf(obj):
+    """Monitor the Serf messafge stream.
+    """
+    from asyncserf import NoopCodec, serf_client
+    import msgpack
+
+    async with serf_client(codec=NoopCodec(), **obj.cfg.server.serf) as client:  # pylint: disable=not-async-context-manager
+        async with client.stream("*") as stream:
+            async for resp in stream:
+                c=vars(resp)
+                c.pop('client', None)
+                c.pop('coalesce', None)
+                p=c['payload']
+                if c.get('event','').startswith('member-'):
+                    m = partial(msgpack.unpackb,raw=True, use_list=False)
+                    p = m(p)
+                else:
+                    m = partial(msgpack.unpackb,raw=False, use_list=False)
+                    p = m(p)
+                c['payload'] = p
+
+                yprint(c)
+                print("---")
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level=logging.DEBUG)
+    anyio.run(main)
+
```

### Comparing `distkv-0.8.4/distkv/command/server.py` & `distkv-0.9.2/distkv/command/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # command line interface
 
 import os
 import sys
-import trio_click as click
+import asyncclick as click
 import anyio
 
 from distkv.util import (
     attrdict,
     PathLongener,
     MsgReader,
     PathShortener,
     split_one,
     NotGiven,
 )
-from distkv.client import open_client, StreamedRequest
+from distkv.client import StreamedRequest
 from distkv.default import CFG
 from distkv.server import Server
 from distkv.auth import loader, gen_auth
 from distkv.exceptions import ClientError
 
 import logging
```

### Comparing `distkv-0.8.4/distkv/default.py` & `distkv-0.9.2/distkv/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         port=PORT,
         ssl=False,
         # ssl=attrdict(cert='/path/to/cert.pem',key='/path/to/cert.key'),
         init_timeout=5,  # time to wait for connection plus greeting
         auth=None,  # no auth used by default
         name=None,  # defaults to the server's name
     ),
+    config=attrdict(prefix=(".distkv", "config")),
     errors=attrdict(prefix=(".distkv", "error")),
     codes=attrdict(prefix=(".distkv", "code", "proc")),
     modules=attrdict(prefix=(".distkv", "code", "module")),
     anyrunner=attrdict(  # for distkv.runner.RunnerRoot
         prefix=(".distkv", "run", "any"),  # storage location
         state=(".distkv", "state", "any"),  # for distkv.runner.SingleRunnerRoot
         name="run-any",  # Serf event name, must be unique
```

### Comparing `distkv-0.8.4/distkv/errors.py` & `distkv-0.9.2/distkv/errors.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/exceptions.py` & `distkv-0.9.2/distkv/exceptions.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/model.py` & `distkv-0.9.2/distkv/model.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/obj.py` & `distkv-0.9.2/distkv/obj.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
-Client code.
+Object interface to distkv data
 
-Main entry point: :func:`open_client`.
 """
 
 import anyio
 import outcome
 import msgpack
 import socket
 import weakref
@@ -381,15 +380,14 @@
 
             async def monitor():
                 pl = PathLongener(())
                 await self.run_starting()
                 async with self.client._stream(
                     "watch", nchain=3, path=self._path, fetch=True
                 ) as w:
-
                     async for r in w:
                         if "path" not in r:
                             if r.get("state", "") == "uptodate":
                                 await self.running()
                             continue
                         pl(r)
                         val = r.get("value", NotGiven)
@@ -427,18 +425,15 @@
                                     if entry:
                                         break
 
                         if not self._need_wait or "chain" not in r:
                             continue
                         c = r.chain
                         while c is not None:
-                            try:
-                                if self._seen[c.node] < c.tick:
-                                    self._seen[c.node] = c.tick
-                            except KeyError:
+                            if self._seen.get(c.node, 0) < c.tick:
                                 self._seen[c.node] = c.tick
                             try:
                                 w = self._waiters[c.node]
                             except KeyError:
                                 pass
                             else:
                                 while w and w[0][0] <= c.tick:
```

### Comparing `distkv-0.8.4/distkv/runner.py` & `distkv-0.9.2/distkv/runner.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/server.py` & `distkv-0.9.2/distkv/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1452,15 +1452,15 @@
                     cls=attrdict,
                 )
                 auth = cfg.get("auth", None)
                 from .auth import gen_auth
                 cfg["auth"] = gen_auth(auth)
 
                 self.logger.debug("DelSync: connecting %s", cfg)
-                async with distkv_client.open_client(**cfg) as client:
+                async with distkv_client.open_client(connect=cfg) as client:
                     # TODO auth this client
                     nodes = NodeSet()
                     n_nodes = 0
 
                     async def send_nodes():
                         nonlocal nodes, n_nodes
                         await client._request(
@@ -1893,15 +1893,15 @@
                     self.cfg.connect,
                     cls=attrdict,
                 )
                 auth = cfg.get("auth", None)
                 from .auth import gen_auth
                 cfg["auth"] = gen_auth(auth)
 
-                async with distkv_client.open_client(**cfg) as client:
+                async with distkv_client.open_client(connect=cfg) as client:
                     # TODO auth this client
 
                     pl = PathLongener(())
                     res = await client._request(
                         "get_tree",
                         iter=True,
                         from_server=self.node.name,
```

### Comparing `distkv-0.8.4/distkv/types.py` & `distkv-0.9.2/distkv/types.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv/util.py` & `distkv-0.9.2/distkv/util.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/distkv.egg-info/PKG-INFO` & `distkv-0.9.2/distkv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: distkv
-Version: 0.8.4
+Version: 0.9.2
 Summary: A distributed no-master key-value store
 Home-page: https://github.com/smurfix/distkv
 Author: Matthias Urlichs
 Author-email: matthias@urlichs.de
 License: MIT -or- Apache License 2.0
 Description: ======
         DistKV
```

### Comparing `distkv-0.8.4/distkv.egg-info/SOURCES.txt` & `distkv-0.9.2/distkv.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,26 +14,19 @@
 pyproject.toml
 setup.cfg
 setup.py
 bin/distkv
 ci/rtd-requirements.txt
 ci/test-requirements.txt
 ci/travis.sh
-debian/.gitignore
-debian/changelog
-debian/compat
-debian/control
-debian/distkv.postinst
-debian/rules
-debian/watch
-debian/source/format
 distkv/__init__.py
 distkv/client.py
 distkv/code.py
 distkv/codec.py
+distkv/config.py
 distkv/default.py
 distkv/errors.py
 distkv/exceptions.py
 distkv/model.py
 distkv/obj.py
 distkv/runner.py
 distkv/server.py
@@ -105,14 +98,15 @@
 tests/logging.cfg
 tests/mock_serf.py
 tests/run.py
 tests/test_basic.py
 tests/test_feature_acl.py
 tests/test_feature_auth.py
 tests/test_feature_code.py
+tests/test_feature_config.py
 tests/test_feature_convert.py
 tests/test_feature_dh.py
 tests/test_feature_error.py
 tests/test_feature_mirror.py
 tests/test_feature_runner.py
 tests/test_feature_singlerunner.py
 tests/test_feature_ssl.py
```

### Comparing `distkv-0.8.4/docs/Makefile` & `distkv-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/make.bat` & `distkv-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/TODO.rst` & `distkv-0.9.2/docs/source/TODO.rst`

 * *Files 3% similar despite different names*

```diff
@@ -39,7 +39,10 @@
 
 * Runner: switch to monotonic time (except for target time!)
 
 * Error consolidation: if a conflict doesn't get resolved on its own, do it
   anyway when we are "it" next and >1 cycle has passed
 
 * Add a command to cleanly flush the server log and stop the server.
+
+* Test iterator on changed config entries
+
```

### Comparing `distkv-0.8.4/docs/source/acls.rst` & `distkv-0.9.2/docs/source/acls.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/auth.rst` & `distkv-0.9.2/docs/source/auth.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/client_protocol.rst` & `distkv-0.9.2/docs/source/client_protocol.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/code.rst` & `distkv-0.9.2/docs/source/code.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/command_line.rst` & `distkv-0.9.2/docs/source/command_line.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1103,14 +1103,52 @@
    Nodes to add or delete. If none are given, list the current state, or (with
    ``--delete``) clear the list, disabling node deletion.
 
    If you want to shut deletion down temporarily, you can also add a
    nonexistent node to the list.
 
 
+.. program:: distkv dump
+
+Various low-level data handling commands.
+
+
+.. program:: distkv dump cfg
+
+Display the current configuration data.
+
+
+.. program:: distkv dump file
+
+Unpack a file and show its contents as YAML.
+
+.. option:: <file>
+
+   The name of the file to decode.
+
+
+.. program:: distkv dump init
+
+Create an initial data file.
+
+.. option:: <node>
+
+   The node name of the DistKV server that should load the initial file.
+
+.. option:: <file>
+
+   The file to write. Typically ``/var/lib/distkv/%Y-%m-%d/0.dkv``.
+
+
+.. program:: distkv dump serf
+
+Monitor all ``serf`` user messages. (I.e. not just those from DistKV.)
+Display as YAML.
+
+
 .. program:: distkv pdb
 
 This subcommand imports the debugger and then continues to process arguments.
 
 This can be used to drop into the debugger when an exception occurs, set
 breakpoints, or whatever.
```

### Comparing `distkv-0.8.4/docs/source/conf.py` & `distkv-0.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/debugging.rst` & `distkv-0.9.2/docs/source/debugging.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/index.rst` & `distkv-0.9.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/model.rst` & `distkv-0.9.2/docs/source/model.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/overview.rst` & `distkv-0.9.2/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/server_protocol.rst` & `distkv-0.9.2/docs/source/server_protocol.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/startup.rst` & `distkv-0.9.2/docs/source/startup.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/translator.rst` & `distkv-0.9.2/docs/source/translator.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/docs/source/tutorial.rst` & `distkv-0.9.2/docs/source/tutorial.rst`

 * *Files 3% similar despite different names*

```diff
@@ -551,7 +551,25 @@
 * Don't change a value that didn't in fact change; otherwise you'll generate an endless loop.
 
 * You need to verify that the two trees match when you start up, and decide
   which is more correct. (The ``tock`` stamp will help you here.) Don't
 overwrite changes that arrive while you do that.
 
 
+Dynamic configuration
+=====================
+
+For some use cases, you might want to configure DistKV dynamically instead
+of by a static configuration file.
+
+This is not always feasible; in particular, the "logging" and "server"
+sections are imported once. Also, options used for connecting to another
+DistKV server cannot be set dynamically because you need them before the
+data are available.
+
+Other options may be overridden by storing a new values at ``.distkv config
+<name>``. It is not possible to be more specific. (TODO)
+
+If a client's ACLs do not allow reading a config entry, it will be silently
+ignored.
+
+A config entry's ``_watch`` property will trigger when the entry is updated.
```

### Comparing `distkv-0.8.4/newsfragments/README.rst` & `distkv-0.9.2/newsfragments/README.rst`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/scripts/init` & `distkv-0.9.2/scripts/init`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/setup.py` & `distkv-0.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description=LONG_DESC,
     author="Matthias Urlichs",
     author_email="matthias@urlichs.de",
     license="MIT -or- Apache License 2.0",
     packages=find_packages(),
     setup_requires=["setuptools_scm", "pytest-runner", "trustme >= 0.5"],
     install_requires=[
-        "trio_click",
+        "asyncclick",
         "trio >= 0.11",
         "range_set >= 0.2",
         "attrs >= 18.2",
         "asyncserf >= 0.15.2",
         "jsonschema >= 2.5",
         "pyyaml >= 3",
         # "argon2 >= 18.3",
```

### Comparing `distkv-0.8.4/tests/__init__.py` & `distkv-0.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/mock_serf.py` & `distkv-0.9.2/tests/mock_serf.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,16 @@
         async def client(self, i: int = 0, **kv):
             """Get a client for the i'th server."""
             await self.s[i].is_serving
             for host, port, *_ in st.s[i].ports:
                 if host[0] == ":":
                     continue
                 try:
-                    async with open_client(
-                        host=host, port=port, ssl=client_ctx, **kv
+                    async with open_client(connect=dict(
+                        host=host, port=port, ssl=client_ctx, **kv)
                     ) as c:
                         yield c
                         return
                 except socket.gaierror:
                     pass
             raise RuntimeError("Duh? no connection")
```

### Comparing `distkv-0.8.4/tests/run.py` & `distkv-0.9.2/tests/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# from trio_click.testing import CliRunner
+# from asyncclick.testing import CliRunner
 import io
 import sys
 
 from distkv.command import main
 from distkv.default import CFG
```

### Comparing `distkv-0.8.4/tests/test_basic.py` & `distkv-0.9.2/tests/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,21 +174,21 @@
             r = await run("client", "-h", h, "-p", p, "data", "get", "foo", "bar")
             assert r.stdout == "'baz'\n"
 
             r = await c._request(
                 "get_state", nodes=True, known=True, missing=True, remote_missing=True
             )
             del r["tock"]
+            del r["seq"]
             assert r == {
                 "node": "test_0",
                 "nodes": {"test_0": 3},
                 "known": {"test_0": ((1, 4),)},
                 "missing": {},
                 "remote_missing": {},
-                "seq": 2,
             }
 
             assert (await c._request("get_value", node="test_0", tick=1)).value == 123
             assert (
                 await c._request("get_value", node="test_0", tick=2)
             ).value == "hello"
             assert (await c._request("get_value", node="test_0", tick=3)).value == "baz"
```

### Comparing `distkv-0.8.4/tests/test_feature_acl.py` & `distkv-0.9.2/tests/test_feature_acl.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_feature_auth.py` & `distkv-0.9.2/tests/test_feature_auth.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_feature_code.py` & `distkv-0.9.2/tests/test_feature_code.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_feature_convert.py` & `distkv-0.9.2/tests/test_feature_convert.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_feature_dh.py` & `distkv-0.9.2/tests/test_feature_dh.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_feature_error.py` & `distkv-0.9.2/tests/test_feature_error.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_feature_mirror.py` & `distkv-0.9.2/tests/test_feature_mirror.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_feature_runner.py` & `distkv-0.9.2/tests/test_feature_runner.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_feature_singlerunner.py` & `distkv-0.9.2/tests/test_feature_singlerunner.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_feature_ssl.py` & `distkv-0.9.2/tests/test_feature_ssl.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_feature_typecheck.py` & `distkv-0.9.2/tests/test_feature_typecheck.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_load_save.py` & `distkv-0.9.2/tests/test_load_save.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_multi.py` & `distkv-0.9.2/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `distkv-0.8.4/tests/test_passthru.py` & `distkv-0.9.2/tests/test_passthru.py`

 * *Files identical despite different names*

