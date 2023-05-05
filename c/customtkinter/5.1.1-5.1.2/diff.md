# Comparing `tmp/customtkinter-5.1.1.tar.gz` & `tmp/customtkinter-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tomschimansky/Documents/Projekte/CustomTkinter/dist/.tmp-wwf2uvk8/customtkinter-5.1.1.tar", last modified: Mon Feb  6 11:56:20 2023, max compression
+gzip compressed data, was "/Users/tomschimansky/Documents/Projekte/CustomTkinter/dist/.tmp-weq8jypm/customtkinter-5.1.2.tar", last modified: Mon Feb  6 19:08:11 2023, max compression
```

## Comparing `customtkinter-5.1.1.tar` & `customtkinter-5.1.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.773712 customtkinter-5.1.1/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1071 2023-02-04 15:54:12.000000 customtkinter-5.1.1/LICENSE
--rw-r--r--   0 tomschimansky   (501) staff       (20)      187 2022-12-10 12:40:29.000000 customtkinter-5.1.1/MANIFEST.in
--rw-r--r--   0 tomschimansky   (501) staff       (20)      606 2023-02-06 11:56:20.773996 customtkinter-5.1.1/PKG-INFO
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.696050 customtkinter-5.1.1/customtkinter/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2739 2023-02-06 11:55:59.000000 customtkinter-5.1.1/customtkinter/__init__.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.701822 customtkinter-5.1.1/customtkinter/assets/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2022-12-10 12:27:18.000000 customtkinter-5.1.1/customtkinter/assets/.DS_Store
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.703005 customtkinter-5.1.1/customtkinter/assets/fonts/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     3528 2022-11-30 22:56:26.000000 customtkinter-5.1.1/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.706987 customtkinter-5.1.1/customtkinter/assets/fonts/Roboto/
--rw-r--r--   0 tomschimansky   (501) staff       (20)   168644 2022-11-30 22:56:26.000000 customtkinter-5.1.1/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0 tomschimansky   (501) staff       (20)   168260 2022-11-30 22:56:26.000000 customtkinter-5.1.1/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.711687 customtkinter-5.1.1/customtkinter/assets/icons/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2022-12-11 00:44:28.000000 customtkinter-5.1.1/customtkinter/assets/icons/.DS_Store
--rw-r--r--   0 tomschimansky   (501) staff       (20)    13238 2022-12-10 12:28:54.000000 customtkinter-5.1.1/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.715298 customtkinter-5.1.1/customtkinter/assets/themes/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4520 2023-02-05 21:39:24.000000 customtkinter-5.1.1/customtkinter/assets/themes/blue.json
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4440 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/assets/themes/dark-blue.json
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4441 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/assets/themes/green.json
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.720965 customtkinter-5.1.1/customtkinter/windows/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      107 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     5532 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/ctk_input_dialog.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    15580 2023-02-05 02:02:38.000000 customtkinter-5.1.1/customtkinter/windows/ctk_tk.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    14717 2023-02-05 02:02:38.000000 customtkinter-5.1.1/customtkinter/windows/ctk_toplevel.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.746254 customtkinter-5.1.1/customtkinter/windows/widgets/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      622 2023-02-04 13:59:22.000000 customtkinter-5.1.1/customtkinter/windows/widgets/__init__.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.750241 customtkinter-5.1.1/customtkinter/windows/widgets/appearance_mode/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      172 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/appearance_mode/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2602 2023-02-05 02:02:38.000000 customtkinter-5.1.1/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4097 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.753809 customtkinter-5.1.1/customtkinter/windows/widgets/core_rendering/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      324 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/core_rendering/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     5894 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/core_rendering/ctk_canvas.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    91030 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/core_rendering/draw_engine.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.758363 customtkinter-5.1.1/customtkinter/windows/widgets/core_widget_classes/
--rw-r--r--   0 tomschimansky   (501) staff       (20)       81 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/core_widget_classes/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    15788 2023-02-05 21:39:24.000000 customtkinter-5.1.1/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     8516 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    27663 2023-02-05 21:39:24.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_button.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    22074 2022-12-06 18:23:05.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_checkbox.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    20598 2023-01-10 14:02:46.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_combobox.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    17893 2023-02-05 02:02:38.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_entry.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     9510 2023-02-04 15:05:29.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_frame.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    12066 2022-12-08 09:34:10.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_label.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    19456 2023-01-07 17:35:48.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_optionmenu.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    14115 2022-12-06 18:23:05.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_progressbar.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    20211 2023-01-21 13:20:54.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_radiobutton.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    15102 2023-02-06 10:16:38.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_scrollable_frame.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    13856 2022-12-06 18:23:05.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_scrollbar.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    19712 2022-12-06 17:47:07.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_segmented_button.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    18308 2022-12-06 18:23:05.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_slider.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    23089 2023-01-21 13:20:54.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_switch.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    17685 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_tabview.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    24566 2023-01-22 18:21:09.000000 customtkinter-5.1.1/customtkinter/windows/widgets/ctk_textbox.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.762363 customtkinter-5.1.1/customtkinter/windows/widgets/font/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1302 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/font/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     3764 2022-12-06 17:25:00.000000 customtkinter-5.1.1/customtkinter/windows/widgets/font/ctk_font.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2268 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/font/font_manager.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.764876 customtkinter-5.1.1/customtkinter/windows/widgets/image/
--rw-r--r--   0 tomschimansky   (501) staff       (20)       32 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/image/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     5306 2022-12-01 08:30:44.000000 customtkinter-5.1.1/customtkinter/windows/widgets/image/ctk_image.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.768298 customtkinter-5.1.1/customtkinter/windows/widgets/scaling/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      287 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/scaling/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     7060 2022-12-06 17:27:05.000000 customtkinter-5.1.1/customtkinter/windows/widgets/scaling/scaling_base_class.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     8745 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/scaling/scaling_tracker.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.770530 customtkinter-5.1.1/customtkinter/windows/widgets/theme/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      473 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/theme/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1813 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/theme/theme_manager.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.772766 customtkinter-5.1.1/customtkinter/windows/widgets/utility/
--rw-r--r--   0 tomschimansky   (501) staff       (20)       72 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/utility/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)      766 2022-11-30 23:02:26.000000 customtkinter-5.1.1/customtkinter/windows/widgets/utility/utility_functions.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 11:56:20.700915 customtkinter-5.1.1/customtkinter.egg-info/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      606 2023-02-06 11:56:20.000000 customtkinter-5.1.1/customtkinter.egg-info/PKG-INFO
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2793 2023-02-06 11:56:20.000000 customtkinter-5.1.1/customtkinter.egg-info/SOURCES.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)        1 2023-02-06 11:56:20.000000 customtkinter-5.1.1/customtkinter.egg-info/dependency_links.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)       57 2023-02-06 11:56:20.000000 customtkinter-5.1.1/customtkinter.egg-info/requires.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)       14 2023-02-06 11:56:20.000000 customtkinter-5.1.1/customtkinter.egg-info/top_level.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1186 2023-02-06 11:55:59.000000 customtkinter-5.1.1/pyproject.toml
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1172 2023-02-06 11:56:20.775304 customtkinter-5.1.1/setup.cfg
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.015873 customtkinter-5.1.2/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1071 2023-02-06 12:16:00.000000 customtkinter-5.1.2/LICENSE
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      187 2023-02-06 12:16:00.000000 customtkinter-5.1.2/MANIFEST.in
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      606 2023-02-06 19:08:11.016213 customtkinter-5.1.2/PKG-INFO
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.893060 customtkinter-5.1.2/customtkinter/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2739 2023-02-06 19:07:47.000000 customtkinter-5.1.2/customtkinter/__init__.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.898879 customtkinter-5.1.2/customtkinter/assets/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2022-12-10 12:27:18.000000 customtkinter-5.1.2/customtkinter/assets/.DS_Store
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.900775 customtkinter-5.1.2/customtkinter/assets/fonts/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     3528 2022-11-30 22:56:26.000000 customtkinter-5.1.2/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.904682 customtkinter-5.1.2/customtkinter/assets/fonts/Roboto/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)   168644 2022-11-30 22:56:26.000000 customtkinter-5.1.2/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0 tomschimansky   (501) staff       (20)   168260 2022-11-30 22:56:26.000000 customtkinter-5.1.2/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.908942 customtkinter-5.1.2/customtkinter/assets/icons/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2022-12-11 00:44:28.000000 customtkinter-5.1.2/customtkinter/assets/icons/.DS_Store
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    13238 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.912461 customtkinter-5.1.2/customtkinter/assets/themes/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4520 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/assets/themes/blue.json
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4514 2023-02-06 19:06:41.000000 customtkinter-5.1.2/customtkinter/assets/themes/dark-blue.json
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4515 2023-02-06 19:05:55.000000 customtkinter-5.1.2/customtkinter/assets/themes/green.json
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.917181 customtkinter-5.1.2/customtkinter/windows/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      107 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     5532 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/ctk_input_dialog.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    15580 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/ctk_tk.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    14717 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/ctk_toplevel.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.981827 customtkinter-5.1.2/customtkinter/windows/widgets/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      622 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/__init__.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.986772 customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      172 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2602 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4097 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.991358 customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      324 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     5894 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/ctk_canvas.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    91030 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/draw_engine.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.995975 customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       81 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    15788 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     8516 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    27663 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_button.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    22074 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_checkbox.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    20598 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_combobox.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    17893 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_entry.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     9510 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_frame.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    12066 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_label.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    19456 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_optionmenu.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    14115 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_progressbar.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    20211 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_radiobutton.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    15102 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_scrollable_frame.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    13856 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_scrollbar.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    19712 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_segmented_button.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    18308 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_slider.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    23089 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_switch.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    17685 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_tabview.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    24566 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_textbox.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.001970 customtkinter-5.1.2/customtkinter/windows/widgets/font/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1302 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/font/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     3764 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/font/ctk_font.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2268 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/font/font_manager.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.004603 customtkinter-5.1.2/customtkinter/windows/widgets/image/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       32 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/image/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     5306 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/image/ctk_image.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.009144 customtkinter-5.1.2/customtkinter/windows/widgets/scaling/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      287 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/scaling/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     7060 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/scaling/scaling_base_class.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     8745 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/scaling/scaling_tracker.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.011641 customtkinter-5.1.2/customtkinter/windows/widgets/theme/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      473 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/theme/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1813 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/theme/theme_manager.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.014643 customtkinter-5.1.2/customtkinter/windows/widgets/utility/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       72 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/utility/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      766 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/utility/utility_functions.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.897811 customtkinter-5.1.2/customtkinter.egg-info/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      606 2023-02-06 19:08:10.000000 customtkinter-5.1.2/customtkinter.egg-info/PKG-INFO
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2793 2023-02-06 19:08:10.000000 customtkinter-5.1.2/customtkinter.egg-info/SOURCES.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)        1 2023-02-06 19:08:10.000000 customtkinter-5.1.2/customtkinter.egg-info/dependency_links.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       57 2023-02-06 19:08:10.000000 customtkinter-5.1.2/customtkinter.egg-info/requires.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       14 2023-02-06 19:08:10.000000 customtkinter-5.1.2/customtkinter.egg-info/top_level.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1186 2023-02-06 19:07:47.000000 customtkinter-5.1.2/pyproject.toml
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1172 2023-02-06 19:08:11.017972 customtkinter-5.1.2/setup.cfg
```

### Comparing `customtkinter-5.1.1/LICENSE` & `customtkinter-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/PKG-INFO` & `customtkinter-5.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinter
-Version: 5.1.1
+Version: 5.1.2
 Summary: Create modern looking GUIs with Python
 Home-page: https://github.com/TomSchimansky/CustomTkinter
 Author: Tom Schimansky
 License: Creative Commons Zero v1.0 Universal
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `customtkinter-5.1.1/customtkinter/__init__.py` & `customtkinter-5.1.2/customtkinter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "5.1.1"
+__version__ = "5.1.2"
 
 import os
 import sys
 from tkinter import Variable, StringVar, IntVar, DoubleVar, BooleanVar
 from tkinter.constants import *
 import tkinter.filedialog as filedialog
```

### Comparing `customtkinter-5.1.1/customtkinter/assets/.DS_Store` & `customtkinter-5.1.2/customtkinter/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf` & `customtkinter-5.1.2/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf` & `customtkinter-5.1.2/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf` & `customtkinter-5.1.2/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/assets/icons/.DS_Store` & `customtkinter-5.1.2/customtkinter/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico` & `customtkinter-5.1.2/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/assets/themes/blue.json` & `customtkinter-5.1.2/customtkinter/assets/themes/blue.json`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/assets/themes/dark-blue.json` & `customtkinter-5.1.2/customtkinter/assets/themes/dark-blue.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9473684210526315%*

 * *Differences: {"'CTkScrollableFrame'": "OrderedDict([('label_fg_color', ['gray80', 'gray21'])])"}*

```diff
@@ -206,14 +206,20 @@
             "gray84"
         ],
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
+    "CTkScrollableFrame": {
+        "label_fg_color": [
+            "gray80",
+            "gray21"
+        ]
+    },
     "CTkScrollbar": {
         "border_spacing": 4,
         "button_color": [
             "gray55",
             "gray41"
         ],
         "button_hover_color": [
```

### Comparing `customtkinter-5.1.1/customtkinter/assets/themes/green.json` & `customtkinter-5.1.2/customtkinter/assets/themes/green.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9473684210526315%*

 * *Differences: {"'CTkScrollableFrame'": "OrderedDict([('label_fg_color', ['gray78', 'gray23'])])"}*

```diff
@@ -206,14 +206,20 @@
             "#DCE4EE"
         ],
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
+    "CTkScrollableFrame": {
+        "label_fg_color": [
+            "gray78",
+            "gray23"
+        ]
+    },
     "CTkScrollbar": {
         "border_spacing": 4,
         "button_color": [
             "gray55",
             "gray41"
         ],
         "button_hover_color": [
```

### Comparing `customtkinter-5.1.1/customtkinter/windows/ctk_input_dialog.py` & `customtkinter-5.1.2/customtkinter/windows/ctk_input_dialog.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/ctk_tk.py` & `customtkinter-5.1.2/customtkinter/windows/ctk_tk.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/ctk_toplevel.py` & `customtkinter-5.1.2/customtkinter/windows/ctk_toplevel.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/__init__.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/core_rendering/ctk_canvas.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/ctk_canvas.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/core_rendering/draw_engine.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/draw_engine.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_button.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_button.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_checkbox.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_checkbox.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_combobox.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_combobox.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_entry.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_entry.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_frame.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_frame.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_label.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_label.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_optionmenu.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_optionmenu.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_progressbar.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_progressbar.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_radiobutton.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_radiobutton.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_scrollable_frame.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_scrollable_frame.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_scrollbar.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_scrollbar.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_segmented_button.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_segmented_button.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_slider.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_slider.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_switch.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_switch.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_tabview.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_tabview.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/ctk_textbox.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_textbox.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/font/__init__.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/font/__init__.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/font/ctk_font.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/font/ctk_font.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/font/font_manager.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/font/font_manager.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/image/ctk_image.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/image/ctk_image.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/scaling/scaling_base_class.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/scaling/scaling_base_class.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/scaling/scaling_tracker.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/scaling/scaling_tracker.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/theme/theme_manager.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter/windows/widgets/utility/utility_functions.py` & `customtkinter-5.1.2/customtkinter/windows/widgets/utility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/customtkinter.egg-info/PKG-INFO` & `customtkinter-5.1.2/customtkinter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinter
-Version: 5.1.1
+Version: 5.1.2
 Summary: Create modern looking GUIs with Python
 Home-page: https://github.com/TomSchimansky/CustomTkinter
 Author: Tom Schimansky
 License: Creative Commons Zero v1.0 Universal
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `customtkinter-5.1.1/customtkinter.egg-info/SOURCES.txt` & `customtkinter-5.1.2/customtkinter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.1/pyproject.toml` & `customtkinter-5.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/TomSchimansky/CustomTkinter"
 
 [tool.tbump.version]
-current = "5.1.1"
+current = "5.1.2"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `customtkinter-5.1.1/setup.cfg` & `customtkinter-5.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = customtkinter
-version = 5.1.1
+version = 5.1.2
 description = Create modern looking GUIs with Python
 long_description = A modern and customizable python UI-library based on Tkinter: https://github.com/TomSchimansky/CustomTkinter
 long_description_content_type = text/markdown
 url = https://github.com/TomSchimansky/CustomTkinter
 author = Tom Schimansky
 license = Creative Commons Zero v1.0 Universal
 license_file = LICENSE
```

