# Comparing `tmp/pygame_gameover-0.0.3.tar.gz` & `tmp/pygame_gameover-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_gameover-0.0.3.tar", last modified: Wed May  3 12:26:39 2023, max compression
+gzip compressed data, was "pygame_gameover-0.0.4.tar", last modified: Fri May  5 07:15:47 2023, max compression
```

## Comparing `pygame_gameover-0.0.3.tar` & `pygame_gameover-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:39.541924 pygame_gameover-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-05-02 11:13:56.000000 pygame_gameover-0.0.3/LICENSE.TXT
--rw-rw-rw-   0        0        0      694 2023-05-03 12:26:39.541924 pygame_gameover-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:39.503375 pygame_gameover-0.0.3/pygame_gameover/
--rw-rw-rw-   0        0        0        0 2023-05-03 06:53:42.000000 pygame_gameover-0.0.3/pygame_gameover/__init__.py
--rw-rw-rw-   0        0        0     2635 2023-05-03 08:42:50.000000 pygame_gameover-0.0.3/pygame_gameover/gameover.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:39.539739 pygame_gameover-0.0.3/pygame_gameover.egg-info/
--rw-rw-rw-   0        0        0      694 2023-05-03 12:26:39.000000 pygame_gameover-0.0.3/pygame_gameover.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-03 12:26:39.000000 pygame_gameover-0.0.3/pygame_gameover.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 12:26:39.000000 pygame_gameover-0.0.3/pygame_gameover.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-03 12:26:39.000000 pygame_gameover-0.0.3/pygame_gameover.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 12:26:39.544433 pygame_gameover-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-05-03 12:24:23.000000 pygame_gameover-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:15:47.257049 pygame_gameover-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-05-02 11:13:56.000000 pygame_gameover-0.0.4/LICENSE.TXT
+-rw-rw-rw-   0        0        0     1350 2023-05-05 07:15:47.256030 pygame_gameover-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 07:15:47.200113 pygame_gameover-0.0.4/pygame_gameover/
+-rw-rw-rw-   0        0        0        0 2023-05-03 06:53:42.000000 pygame_gameover-0.0.4/pygame_gameover/__init__.py
+-rw-rw-rw-   0        0        0     2635 2023-05-03 08:42:50.000000 pygame_gameover-0.0.4/pygame_gameover/gameover.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:15:47.248911 pygame_gameover-0.0.4/pygame_gameover.egg-info/
+-rw-rw-rw-   0        0        0     1350 2023-05-05 07:15:47.000000 pygame_gameover-0.0.4/pygame_gameover.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-05 07:15:47.000000 pygame_gameover-0.0.4/pygame_gameover.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 07:15:47.000000 pygame_gameover-0.0.4/pygame_gameover.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-05 07:15:47.000000 pygame_gameover-0.0.4/pygame_gameover.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 07:15:47.257049 pygame_gameover-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2023-05-05 07:15:13.000000 pygame_gameover-0.0.4/setup.py
```

### Comparing `pygame_gameover-0.0.3/LICENSE.TXT` & `pygame_gameover-0.0.4/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `pygame_gameover-0.0.3/pygame_gameover/gameover.py` & `pygame_gameover-0.0.4/pygame_gameover/gameover.py`

 * *Files identical despite different names*

