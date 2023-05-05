# Comparing `tmp/tsutils-8.0.3.tar.gz` & `tmp/tsutils-8.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsutils-8.0.3.tar", last modified: Thu May  4 07:46:44 2023, max compression
+gzip compressed data, was "tsutils-8.0.4.tar", last modified: Fri May  5 02:05:09 2023, max compression
```

## Comparing `tsutils-8.0.3.tar` & `tsutils-8.0.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.972689 tsutils-8.0.3/
--rw-r--r--   0 chasehult   (501) staff       (20)     1075 2021-09-27 07:51:44.000000 tsutils-8.0.3/LICENSE
--rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-05-04 07:46:44.972562 tsutils-8.0.3/PKG-INFO
--rw-r--r--   0 chasehult   (501) staff       (20)      174 2021-09-27 07:51:44.000000 tsutils-8.0.3/README.md
--rw-r--r--   0 chasehult   (501) staff       (20)       38 2023-05-04 07:46:44.972730 tsutils-8.0.3/setup.cfg
--rw-r--r--   0 chasehult   (501) staff       (20)      842 2023-04-14 01:13:39.000000 tsutils-8.0.3/setup.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.967604 tsutils-8.0.3/tsutils/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3920 2022-06-03 03:58:49.000000 tsutils-8.0.3/tsutils/cog_mixins.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1888 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/cog_settings.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.968791 tsutils-8.0.3/tsutils/cogs/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/cogs/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      565 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/cogs/donations.py
--rw-r--r--   0 chasehult   (501) staff       (20)      761 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/cogs/globaladmin.py
--rw-r--r--   0 chasehult   (501) staff       (20)      523 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/cogs/userpreferences.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1220 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/converters.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3436 2022-08-31 20:43:03.000000 tsutils-8.0.3/tsutils/emoji.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1009 2022-03-02 22:25:01.000000 tsutils-8.0.3/tsutils/enums.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1133 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/errors.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2456 2023-02-20 15:48:19.000000 tsutils-8.0.3/tsutils/formatting.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1942 2022-02-14 03:50:39.000000 tsutils-8.0.3/tsutils/helper_classes.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3286 2022-06-03 03:07:59.000000 tsutils-8.0.3/tsutils/helper_functions.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2433 2022-11-11 00:42:14.000000 tsutils-8.0.3/tsutils/json_utils.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.969480 tsutils-8.0.3/tsutils/menu/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/menu/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      616 2022-08-31 20:46:20.000000 tsutils-8.0.3/tsutils/menu/closable_embed_base.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.970174 tsutils-8.0.3/tsutils/menu/components/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.3/tsutils/menu/components/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      604 2022-03-02 23:07:15.000000 tsutils-8.0.3/tsutils/menu/components/config.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1342 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/menu/components/footers.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2320 2022-01-11 05:08:45.000000 tsutils-8.0.3/tsutils/menu/components/panes.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3348 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/menu/pad_view.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1624 2022-08-31 20:46:20.000000 tsutils-8.0.3/tsutils/menu/simple_text.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.970894 tsutils-8.0.3/tsutils/menu/view/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.3/tsutils/menu/view/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      429 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/menu/view/closable_embed.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1790 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/menu/view/simple_text.py
--rw-r--r--   0 chasehult   (501) staff       (20)      597 2022-01-11 05:08:45.000000 tsutils-8.0.3/tsutils/menu/view/view_state_base.py
--rw-r--r--   0 chasehult   (501) staff       (20)     5868 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/old_menu.py
--rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/pad.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.971581 tsutils-8.0.3/tsutils/query_settings/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 22:16:59.000000 tsutils-8.0.3/tsutils/query_settings/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2017 2022-12-01 06:04:20.000000 tsutils-8.0.3/tsutils/query_settings/converters.py
--rw-r--r--   0 chasehult   (501) staff       (20)      802 2022-11-11 00:42:14.000000 tsutils-8.0.3/tsutils/query_settings/enums.py
--rw-r--r--   0 chasehult   (501) staff       (20)     7507 2023-02-20 15:48:19.000000 tsutils-8.0.3/tsutils/query_settings/query_settings.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1943 2022-06-03 03:07:59.000000 tsutils-8.0.3/tsutils/time.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.972305 tsutils-8.0.3/tsutils/tsubaki/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 21:15:46.000000 tsutils-8.0.3/tsutils/tsubaki/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)     4708 2023-05-04 07:35:57.000000 tsutils-8.0.3/tsutils/tsubaki/custom_emoji.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3620 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/tsubaki/links.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2736 2023-04-14 01:12:54.000000 tsutils-8.0.3/tsutils/tsubaki/monster_header.py
--rw-r--r--   0 chasehult   (501) staff       (20)     6874 2022-08-31 20:46:20.000000 tsutils-8.0.3/tsutils/user_interaction.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.968284 tsutils-8.0.3/tsutils.egg-info/
--rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-05-04 07:46:44.000000 tsutils-8.0.3/tsutils.egg-info/PKG-INFO
--rw-r--r--   0 chasehult   (501) staff       (20)     1260 2023-05-04 07:46:44.000000 tsutils-8.0.3/tsutils.egg-info/SOURCES.txt
--rw-r--r--   0 chasehult   (501) staff       (20)        1 2023-05-04 07:46:44.000000 tsutils-8.0.3/tsutils.egg-info/dependency_links.txt
--rw-r--r--   0 chasehult   (501) staff       (20)       61 2023-05-04 07:46:44.000000 tsutils-8.0.3/tsutils.egg-info/requires.txt
--rw-r--r--   0 chasehult   (501) staff       (20)        8 2023-05-04 07:46:44.000000 tsutils-8.0.3/tsutils.egg-info/top_level.txt
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:05:09.326810 tsutils-8.0.4/
+-rw-r--r--   0 chasehult   (501) staff       (20)     1075 2021-09-27 07:51:44.000000 tsutils-8.0.4/LICENSE
+-rw-r--r--   0 chasehult   (501) staff       (20)      619 2023-05-05 02:05:09.326705 tsutils-8.0.4/PKG-INFO
+-rw-r--r--   0 chasehult   (501) staff       (20)      174 2021-09-27 07:51:44.000000 tsutils-8.0.4/README.md
+-rw-r--r--   0 chasehult   (501) staff       (20)       38 2023-05-05 02:05:09.326841 tsutils-8.0.4/setup.cfg
+-rw-r--r--   0 chasehult   (501) staff       (20)      790 2023-05-05 00:26:41.000000 tsutils-8.0.4/setup.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:05:09.322366 tsutils-8.0.4/tsutils/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.4/tsutils/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3940 2023-05-04 15:15:12.000000 tsutils-8.0.4/tsutils/cog_mixins.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1888 2021-09-27 07:51:44.000000 tsutils-8.0.4/tsutils/cog_settings.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:05:09.323375 tsutils-8.0.4/tsutils/cogs/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.4/tsutils/cogs/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      565 2021-09-27 07:51:44.000000 tsutils-8.0.4/tsutils/cogs/donations.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      761 2021-09-27 07:51:44.000000 tsutils-8.0.4/tsutils/cogs/globaladmin.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      523 2021-09-27 07:51:44.000000 tsutils-8.0.4/tsutils/cogs/userpreferences.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1220 2021-09-27 07:51:44.000000 tsutils-8.0.4/tsutils/converters.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3436 2022-08-31 20:43:03.000000 tsutils-8.0.4/tsutils/emoji.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1009 2022-03-02 22:25:01.000000 tsutils-8.0.4/tsutils/enums.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1133 2021-09-27 07:51:44.000000 tsutils-8.0.4/tsutils/errors.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2456 2023-02-20 15:48:19.000000 tsutils-8.0.4/tsutils/formatting.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1942 2022-02-14 03:50:39.000000 tsutils-8.0.4/tsutils/helper_classes.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3289 2023-05-04 15:15:12.000000 tsutils-8.0.4/tsutils/helper_functions.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2433 2022-11-11 00:42:14.000000 tsutils-8.0.4/tsutils/json_utils.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:05:09.323881 tsutils-8.0.4/tsutils/menu/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.4/tsutils/menu/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      616 2022-08-31 20:46:20.000000 tsutils-8.0.4/tsutils/menu/closable_embed_base.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:05:09.324784 tsutils-8.0.4/tsutils/menu/components/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.4/tsutils/menu/components/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      604 2022-03-02 23:07:15.000000 tsutils-8.0.4/tsutils/menu/components/config.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1291 2023-05-04 15:15:12.000000 tsutils-8.0.4/tsutils/menu/components/footers.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2320 2022-01-11 05:08:45.000000 tsutils-8.0.4/tsutils/menu/components/panes.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3332 2023-05-04 15:15:12.000000 tsutils-8.0.4/tsutils/menu/pad_view.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1624 2022-08-31 20:46:20.000000 tsutils-8.0.4/tsutils/menu/simple_text.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:05:09.325303 tsutils-8.0.4/tsutils/menu/view/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.4/tsutils/menu/view/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      429 2023-03-14 02:42:07.000000 tsutils-8.0.4/tsutils/menu/view/closable_embed.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1790 2023-03-14 02:42:07.000000 tsutils-8.0.4/tsutils/menu/view/simple_text.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      597 2022-01-11 05:08:45.000000 tsutils-8.0.4/tsutils/menu/view/view_state_base.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     5868 2021-09-27 07:51:44.000000 tsutils-8.0.4/tsutils/old_menu.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-03-14 02:42:07.000000 tsutils-8.0.4/tsutils/pad.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:05:09.325901 tsutils-8.0.4/tsutils/query_settings/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 22:16:59.000000 tsutils-8.0.4/tsutils/query_settings/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2017 2022-12-01 06:04:20.000000 tsutils-8.0.4/tsutils/query_settings/converters.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      802 2022-11-11 00:42:14.000000 tsutils-8.0.4/tsutils/query_settings/enums.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     7507 2023-02-20 15:48:19.000000 tsutils-8.0.4/tsutils/query_settings/query_settings.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1943 2022-06-03 03:07:59.000000 tsutils-8.0.4/tsutils/time.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:05:09.326575 tsutils-8.0.4/tsutils/tsubaki/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 21:15:46.000000 tsutils-8.0.4/tsutils/tsubaki/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     4708 2023-05-04 15:15:12.000000 tsutils-8.0.4/tsutils/tsubaki/custom_emoji.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3620 2023-03-14 02:42:07.000000 tsutils-8.0.4/tsutils/tsubaki/links.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2736 2023-05-04 15:15:12.000000 tsutils-8.0.4/tsutils/tsubaki/monster_header.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     6874 2022-08-31 20:46:20.000000 tsutils-8.0.4/tsutils/user_interaction.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:05:09.322965 tsutils-8.0.4/tsutils.egg-info/
+-rw-r--r--   0 chasehult   (501) staff       (20)      619 2023-05-05 02:05:09.000000 tsutils-8.0.4/tsutils.egg-info/PKG-INFO
+-rw-r--r--   0 chasehult   (501) staff       (20)     1260 2023-05-05 02:05:09.000000 tsutils-8.0.4/tsutils.egg-info/SOURCES.txt
+-rw-r--r--   0 chasehult   (501) staff       (20)        1 2023-05-05 02:05:09.000000 tsutils-8.0.4/tsutils.egg-info/dependency_links.txt
+-rw-r--r--   0 chasehult   (501) staff       (20)       60 2023-05-05 02:05:09.000000 tsutils-8.0.4/tsutils.egg-info/requires.txt
+-rw-r--r--   0 chasehult   (501) staff       (20)        8 2023-05-05 02:05:09.000000 tsutils-8.0.4/tsutils.egg-info/top_level.txt
```

### Comparing `tsutils-8.0.3/LICENSE` & `tsutils-8.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/PKG-INFO` & `tsutils-8.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tsutils
-Version: 8.0.3
+Version: 8.0.4
 Summary: A collection of helper commands for Red-DiscordBot
-Home-page: https://github.com/TsubakiBotPad/tsutils
 Author: The Tsubotki Team
-Author-email: 69992611+TsubakiBotPad@users.noreply.github.com
+Author-email: 69992611+TsubakiBotPAD@users.noreply.github.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This code started out as rpadutils as part of Mirubot and later padbot-cogs/misc-cogs for Tsubaki Bot. It's now a library in order to improve the startup process of the bot.
```

### Comparing `tsutils-8.0.3/setup.py` & `tsutils-8.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tsutils",
-    version="8.0.3",
+    version="8.0.4",
     author="The Tsubotki Team",
-    author_email="69992611+TsubakiBotPad@users.noreply.github.com",
+    author_email="69992611+TsubakiBotPAD@users.noreply.github.com",
     license="MIT",
     description="A collection of helper commands for Red-DiscordBot",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/TsubakiBotPad/tsutils",
     packages=setuptools.find_packages(),
     install_requires=[
         "backoff==1.10.0",
         "discord_menu>=0.16.13",
-        "Red-DiscordBot>=3.4.14",
+        "Red-DiscordBot>=3.5.1",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.11',
 )
```

### Comparing `tsutils-8.0.3/tsutils/cog_mixins.py` & `tsutils-8.0.4/tsutils/cog_mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     cog.__cog_commands__ = (*cog.__cog_commands__, command)
     setattr(cog, command.callback.__name__, command)
 
     lookup = {cmd.qualified_name: cmd for cmd in cog.__cog_commands__}
 
     parent = command.parent
     if parent is not None:
-        parent = lookup[parent.qualified_name]
+        parent = lookup[parent.qualified_name]  # noqa (red sucks)
         parent.remove_command(command.name)
         parent.add_command(command)
 
 
 def mixin_command(parent: Optional[str], **kwargs) -> Callable[[Callable], MixinCommand]:
     def _decorator(func: Callable) -> MixinCommand:
         return MixinCommand(func, parent, **kwargs)
```

### Comparing `tsutils-8.0.3/tsutils/cog_settings.py` & `tsutils-8.0.4/tsutils/cog_settings.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/cogs/donations.py` & `tsutils-8.0.4/tsutils/cogs/donations.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/cogs/globaladmin.py` & `tsutils-8.0.4/tsutils/cogs/globaladmin.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/cogs/userpreferences.py` & `tsutils-8.0.4/tsutils/cogs/userpreferences.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/converters.py` & `tsutils-8.0.4/tsutils/converters.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/emoji.py` & `tsutils-8.0.4/tsutils/emoji.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/enums.py` & `tsutils-8.0.4/tsutils/enums.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/errors.py` & `tsutils-8.0.4/tsutils/errors.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/formatting.py` & `tsutils-8.0.4/tsutils/formatting.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/helper_classes.py` & `tsutils-8.0.4/tsutils/helper_classes.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/helper_functions.py` & `tsutils-8.0.4/tsutils/helper_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import asyncio
-import discord.ext
 import errno
 import os
 import signal
 from functools import wraps
 from typing import Any, AsyncGenerator, Callable, Coroutine, Iterable, Mapping, Optional, TypeVar
 
+import discord.ext
+
 Decorator = Callable[[Callable], Callable]
 DecoratorFunction = Callable[..., Decorator]
 
 R = TypeVar("R")
 
 
-def timeout_after(seconds: int = 10,
+def timeout_after(seconds: float = 10,
                   error_message: str = os.strerror(errno.ETIME)) \
         -> Decorator:
     """A decorator to give a timeout to a synchronous function"""
 
     def decorator(func):
         def _handle_timeout(signum, frame):
             raise TimeoutError(error_message)
```

### Comparing `tsutils-8.0.3/tsutils/json_utils.py` & `tsutils-8.0.4/tsutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/menu/closable_embed_base.py` & `tsutils-8.0.4/tsutils/menu/closable_embed_base.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/menu/components/config.py` & `tsutils-8.0.4/tsutils/menu/components/config.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/menu/components/footers.py` & `tsutils-8.0.4/tsutils/menu/components/footers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from discordmenu.embed.components import EmbedFooter
-from discordmenu.embed.view_state import ViewState
 from discordmenu.intra_message_state import IntraMessageState
-from tsutils.query_settings.query_settings import QuerySettings
 
+from tsutils.query_settings.query_settings import QuerySettings
 from tsutils.tsubaki.links import CLOUDFRONT_URL, MonsterImage
 
 TSUBAKI_FLOWER_ICON_URL = CLOUDFRONT_URL + '/tsubaki/tsubakiflower.png'
 
 
 def embed_footer():
     return EmbedFooter('Requester may click the reactions below to switch tabs')
```

### Comparing `tsutils-8.0.3/tsutils/menu/components/panes.py` & `tsutils-8.0.4/tsutils/menu/components/panes.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/menu/pad_view.py` & `tsutils-8.0.4/tsutils/menu/pad_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from abc import abstractmethod, ABCMeta
-from typing import List, Optional, Dict, Any, Union
+from abc import ABCMeta
+from typing import Any, Dict, List, Optional, Union
 
 from discord import Colour
 from discordmenu.embed.base import Box
-from discordmenu.embed.components import EmbedMain, EmbedField, EmbedFooter, EmbedThumbnail, EmbedBodyImage, EmbedAuthor
+from discordmenu.embed.components import EmbedAuthor, EmbedBodyImage, EmbedField, EmbedFooter, EmbedMain, EmbedThumbnail
 from discordmenu.embed.view import EmbedView
 
 from tsutils.menu.components.config import UserConfig
 from tsutils.menu.components.footers import embed_footer_with_state
 from tsutils.query_settings.query_settings import QuerySettings
```

### Comparing `tsutils-8.0.3/tsutils/menu/simple_text.py` & `tsutils-8.0.4/tsutils/menu/simple_text.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/menu/view/simple_text.py` & `tsutils-8.0.4/tsutils/menu/view/simple_text.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/menu/view/view_state_base.py` & `tsutils-8.0.4/tsutils/menu/view/view_state_base.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/old_menu.py` & `tsutils-8.0.4/tsutils/old_menu.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/pad.py` & `tsutils-8.0.4/tsutils/pad.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/query_settings/converters.py` & `tsutils-8.0.4/tsutils/query_settings/converters.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/query_settings/enums.py` & `tsutils-8.0.4/tsutils/query_settings/enums.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/query_settings/query_settings.py` & `tsutils-8.0.4/tsutils/query_settings/query_settings.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/time.py` & `tsutils-8.0.4/tsutils/time.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/tsubaki/custom_emoji.py` & `tsutils-8.0.4/tsutils/tsubaki/custom_emoji.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/tsubaki/links.py` & `tsutils-8.0.4/tsutils/tsubaki/links.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/tsubaki/monster_header.py` & `tsutils-8.0.4/tsutils/tsubaki/monster_header.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils/user_interaction.py` & `tsutils-8.0.4/tsutils/user_interaction.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.3/tsutils.egg-info/PKG-INFO` & `tsutils-8.0.4/tsutils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tsutils
-Version: 8.0.3
+Version: 8.0.4
 Summary: A collection of helper commands for Red-DiscordBot
-Home-page: https://github.com/TsubakiBotPad/tsutils
 Author: The Tsubotki Team
-Author-email: 69992611+TsubakiBotPad@users.noreply.github.com
+Author-email: 69992611+TsubakiBotPAD@users.noreply.github.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This code started out as rpadutils as part of Mirubot and later padbot-cogs/misc-cogs for Tsubaki Bot. It's now a library in order to improve the startup process of the bot.
```

### Comparing `tsutils-8.0.3/tsutils.egg-info/SOURCES.txt` & `tsutils-8.0.4/tsutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

