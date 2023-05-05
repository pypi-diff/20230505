# Comparing `tmp/customtkinter-5.1.2.tar.gz` & `tmp/customtkinter-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tomschimansky/Documents/Projekte/CustomTkinter/dist/.tmp-weq8jypm/customtkinter-5.1.2.tar", last modified: Mon Feb  6 19:08:11 2023, max compression
+gzip compressed data, was "/Users/tomschimansky/Documents/Projekte/CustomTkinter/dist/.tmp-g81nkl_2/customtkinter-5.1.3.tar", last modified: Fri May  5 17:12:37 2023, max compression
```

## Comparing `customtkinter-5.1.2.tar` & `customtkinter-5.1.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.015873 customtkinter-5.1.2/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1071 2023-02-06 12:16:00.000000 customtkinter-5.1.2/LICENSE
--rw-r--r--   0 tomschimansky   (501) staff       (20)      187 2023-02-06 12:16:00.000000 customtkinter-5.1.2/MANIFEST.in
--rw-r--r--   0 tomschimansky   (501) staff       (20)      606 2023-02-06 19:08:11.016213 customtkinter-5.1.2/PKG-INFO
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.893060 customtkinter-5.1.2/customtkinter/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2739 2023-02-06 19:07:47.000000 customtkinter-5.1.2/customtkinter/__init__.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.898879 customtkinter-5.1.2/customtkinter/assets/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2022-12-10 12:27:18.000000 customtkinter-5.1.2/customtkinter/assets/.DS_Store
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.900775 customtkinter-5.1.2/customtkinter/assets/fonts/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     3528 2022-11-30 22:56:26.000000 customtkinter-5.1.2/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.904682 customtkinter-5.1.2/customtkinter/assets/fonts/Roboto/
--rw-r--r--   0 tomschimansky   (501) staff       (20)   168644 2022-11-30 22:56:26.000000 customtkinter-5.1.2/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0 tomschimansky   (501) staff       (20)   168260 2022-11-30 22:56:26.000000 customtkinter-5.1.2/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.908942 customtkinter-5.1.2/customtkinter/assets/icons/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2022-12-11 00:44:28.000000 customtkinter-5.1.2/customtkinter/assets/icons/.DS_Store
--rw-r--r--   0 tomschimansky   (501) staff       (20)    13238 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.912461 customtkinter-5.1.2/customtkinter/assets/themes/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4520 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/assets/themes/blue.json
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4514 2023-02-06 19:06:41.000000 customtkinter-5.1.2/customtkinter/assets/themes/dark-blue.json
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4515 2023-02-06 19:05:55.000000 customtkinter-5.1.2/customtkinter/assets/themes/green.json
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.917181 customtkinter-5.1.2/customtkinter/windows/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      107 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     5532 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/ctk_input_dialog.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    15580 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/ctk_tk.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    14717 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/ctk_toplevel.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.981827 customtkinter-5.1.2/customtkinter/windows/widgets/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      622 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/__init__.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.986772 customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      172 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2602 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4097 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.991358 customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      324 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     5894 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/ctk_canvas.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    91030 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/draw_engine.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.995975 customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/
--rw-r--r--   0 tomschimansky   (501) staff       (20)       81 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    15788 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     8516 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    27663 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_button.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    22074 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_checkbox.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    20598 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_combobox.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    17893 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_entry.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     9510 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_frame.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    12066 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_label.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    19456 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_optionmenu.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    14115 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_progressbar.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    20211 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_radiobutton.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    15102 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_scrollable_frame.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    13856 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_scrollbar.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    19712 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_segmented_button.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    18308 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_slider.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    23089 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_switch.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    17685 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_tabview.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    24566 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/ctk_textbox.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.001970 customtkinter-5.1.2/customtkinter/windows/widgets/font/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1302 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/font/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     3764 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/font/ctk_font.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2268 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/font/font_manager.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.004603 customtkinter-5.1.2/customtkinter/windows/widgets/image/
--rw-r--r--   0 tomschimansky   (501) staff       (20)       32 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/image/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     5306 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/image/ctk_image.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.009144 customtkinter-5.1.2/customtkinter/windows/widgets/scaling/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      287 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/scaling/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     7060 2023-02-06 12:16:01.000000 customtkinter-5.1.2/customtkinter/windows/widgets/scaling/scaling_base_class.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     8745 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/scaling/scaling_tracker.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.011641 customtkinter-5.1.2/customtkinter/windows/widgets/theme/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      473 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/theme/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1813 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/theme/theme_manager.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:11.014643 customtkinter-5.1.2/customtkinter/windows/widgets/utility/
--rw-r--r--   0 tomschimansky   (501) staff       (20)       72 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/utility/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)      766 2022-11-30 23:02:26.000000 customtkinter-5.1.2/customtkinter/windows/widgets/utility/utility_functions.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-02-06 19:08:10.897811 customtkinter-5.1.2/customtkinter.egg-info/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      606 2023-02-06 19:08:10.000000 customtkinter-5.1.2/customtkinter.egg-info/PKG-INFO
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2793 2023-02-06 19:08:10.000000 customtkinter-5.1.2/customtkinter.egg-info/SOURCES.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)        1 2023-02-06 19:08:10.000000 customtkinter-5.1.2/customtkinter.egg-info/dependency_links.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)       57 2023-02-06 19:08:10.000000 customtkinter-5.1.2/customtkinter.egg-info/requires.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)       14 2023-02-06 19:08:10.000000 customtkinter-5.1.2/customtkinter.egg-info/top_level.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1186 2023-02-06 19:07:47.000000 customtkinter-5.1.2/pyproject.toml
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1172 2023-02-06 19:08:11.017972 customtkinter-5.1.2/setup.cfg
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.901600 customtkinter-5.1.3/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1071 2023-02-06 12:16:00.000000 customtkinter-5.1.3/LICENSE
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      187 2023-02-06 12:16:00.000000 customtkinter-5.1.3/MANIFEST.in
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      592 2023-05-05 17:12:37.901909 customtkinter-5.1.3/PKG-INFO
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.868297 customtkinter-5.1.3/customtkinter/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2739 2023-05-05 16:55:53.000000 customtkinter-5.1.3/customtkinter/__init__.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.871190 customtkinter-5.1.3/customtkinter/assets/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2023-04-20 16:40:50.000000 customtkinter-5.1.3/customtkinter/assets/.DS_Store
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.871666 customtkinter-5.1.3/customtkinter/assets/fonts/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     3528 2022-11-30 22:56:26.000000 customtkinter-5.1.3/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.873519 customtkinter-5.1.3/customtkinter/assets/fonts/Roboto/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)   168644 2022-11-30 22:56:26.000000 customtkinter-5.1.3/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0 tomschimansky   (501) staff       (20)   168260 2022-11-30 22:56:26.000000 customtkinter-5.1.3/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.875515 customtkinter-5.1.3/customtkinter/assets/icons/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2022-12-11 00:44:28.000000 customtkinter-5.1.3/customtkinter/assets/icons/.DS_Store
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    13238 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.877528 customtkinter-5.1.3/customtkinter/assets/themes/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4520 2023-04-23 09:36:19.000000 customtkinter-5.1.3/customtkinter/assets/themes/blue.json
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4514 2023-04-23 09:36:19.000000 customtkinter-5.1.3/customtkinter/assets/themes/dark-blue.json
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4515 2023-04-23 09:36:19.000000 customtkinter-5.1.3/customtkinter/assets/themes/green.json
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.879545 customtkinter-5.1.3/customtkinter/windows/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      107 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     5532 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/ctk_input_dialog.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    15580 2023-03-26 14:22:30.000000 customtkinter-5.1.3/customtkinter/windows/ctk_tk.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    14727 2023-04-20 23:43:47.000000 customtkinter-5.1.3/customtkinter/windows/ctk_toplevel.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.888855 customtkinter-5.1.3/customtkinter/windows/widgets/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      622 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/__init__.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.890708 customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      172 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2602 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4097 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.892130 customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      324 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     5894 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/ctk_canvas.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    91030 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/draw_engine.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.893662 customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       81 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    15788 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     8516 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    27663 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_button.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    22074 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_checkbox.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    20598 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_combobox.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    17893 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_entry.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     9510 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_frame.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    12136 2023-05-05 16:54:04.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_label.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    19456 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_optionmenu.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    14115 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_progressbar.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    20211 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_radiobutton.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    15116 2023-04-26 08:52:31.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_scrollable_frame.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    13856 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_scrollbar.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    19712 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_segmented_button.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    18308 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_slider.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    23416 2023-04-24 11:44:24.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_switch.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    17700 2023-04-26 09:33:02.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_tabview.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    24566 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_textbox.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.895072 customtkinter-5.1.3/customtkinter/windows/widgets/font/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1302 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/font/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     3764 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/font/ctk_font.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2268 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/font/font_manager.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.895969 customtkinter-5.1.3/customtkinter/windows/widgets/image/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       32 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/image/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     5306 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/image/ctk_image.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.897782 customtkinter-5.1.3/customtkinter/windows/widgets/scaling/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      287 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/scaling/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     7060 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/scaling/scaling_base_class.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     8745 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/scaling/scaling_tracker.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.899354 customtkinter-5.1.3/customtkinter/windows/widgets/theme/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      471 2023-04-24 11:36:20.000000 customtkinter-5.1.3/customtkinter/windows/widgets/theme/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1906 2023-04-24 11:32:27.000000 customtkinter-5.1.3/customtkinter/windows/widgets/theme/theme_manager.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.900920 customtkinter-5.1.3/customtkinter/windows/widgets/utility/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       72 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/utility/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      766 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/utility/utility_functions.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.870598 customtkinter-5.1.3/customtkinter.egg-info/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      592 2023-05-05 17:12:37.000000 customtkinter-5.1.3/customtkinter.egg-info/PKG-INFO
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2793 2023-05-05 17:12:37.000000 customtkinter-5.1.3/customtkinter.egg-info/SOURCES.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)        1 2023-05-05 17:12:37.000000 customtkinter-5.1.3/customtkinter.egg-info/dependency_links.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       57 2023-05-05 17:12:37.000000 customtkinter-5.1.3/customtkinter.egg-info/requires.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       14 2023-05-05 17:12:37.000000 customtkinter-5.1.3/customtkinter.egg-info/top_level.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      757 2023-05-05 16:55:53.000000 customtkinter-5.1.3/pyproject.toml
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1355 2023-05-05 17:12:37.903208 customtkinter-5.1.3/setup.cfg
```

### Comparing `customtkinter-5.1.2/LICENSE` & `customtkinter-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/__init__.py` & `customtkinter-5.1.3/customtkinter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "5.1.2"
+__version__ = "5.1.3"
 
 import os
 import sys
 from tkinter import Variable, StringVar, IntVar, DoubleVar, BooleanVar
 from tkinter.constants import *
 import tkinter.filedialog as filedialog
```

### Comparing `customtkinter-5.1.2/customtkinter/assets/.DS_Store` & `customtkinter-5.1.3/customtkinter/assets/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 00000270: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
 00000280: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
 00000290: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 000002a0: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
 000002b0: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
 000002c0: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
 000002d0: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-000002e0: 6465 6261 7208 0908 095f 1018 7b7b 3239  debar...._..{{29
-000002f0: 302c 2031 3936 7d2c 207b 3932 382c 2036  0, 196}, {928, 6
-00000300: 3934 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  94}}...#/;R_klmn
+000002e0: 6465 6261 7208 0908 095f 1018 7b7b 3338  debar...._..{{38
+000002f0: 302c 2039 367d 2c20 7b31 3039 392c 2038  0, 96}, {1099, 8
+00000300: 3030 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  00}}...#/;R_klmn
 00000310: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
 00000320: 000d 0000 0000 0000 0000 0000 0000 0000  ................
 00000330: 008b 0000 0005 0069 0063 006f 006e 0073  .......i.c.o.n.s
 00000340: 7653 726e 6c6f 6e67 0000 0001 0000 0006  vSrnlong........
 00000350: 0074 0068 0065 006d 0065 0073 496c 6f63  .t.h.e.m.e.sIloc
 00000360: 626c 6f62 0000 0010 0000 011d 0000 002e  blob............
 00000370: ffff ffff ffff 0000 0000 0000 0000 0000  ................
```

### Comparing `customtkinter-5.1.2/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf` & `customtkinter-5.1.3/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf` & `customtkinter-5.1.3/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf` & `customtkinter-5.1.3/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/assets/icons/.DS_Store` & `customtkinter-5.1.3/customtkinter/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico` & `customtkinter-5.1.3/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/assets/themes/blue.json` & `customtkinter-5.1.3/customtkinter/assets/themes/blue.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994736842105263%*

 * *Differences: {"'CTkSwitch'": "{'fg_color': ['#939BA2', '#4A4D50'], delete: ['fg_Color']}"}*

```diff
@@ -291,15 +291,15 @@
         ],
         "button_hover_color": [
             "gray20",
             "gray100"
         ],
         "button_length": 0,
         "corner_radius": 1000,
-        "fg_Color": [
+        "fg_color": [
             "#939BA2",
             "#4A4D50"
         ],
         "progress_color": [
             "#3B8ED0",
             "#1F6AA5"
         ],
```

### Comparing `customtkinter-5.1.2/customtkinter/assets/themes/dark-blue.json` & `customtkinter-5.1.3/customtkinter/assets/themes/dark-blue.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994736842105263%*

 * *Differences: {"'CTkSwitch'": "{'fg_color': ['#939BA2', '#4A4D50'], delete: ['fg_Color']}"}*

```diff
@@ -291,15 +291,15 @@
         ],
         "button_hover_color": [
             "gray20",
             "gray100"
         ],
         "button_length": 0,
         "corner_radius": 1000,
-        "fg_Color": [
+        "fg_color": [
             "#939BA2",
             "#4A4D50"
         ],
         "progress_color": [
             "#3a7ebf",
             "#1f538d"
         ],
```

### Comparing `customtkinter-5.1.2/customtkinter/assets/themes/green.json` & `customtkinter-5.1.3/customtkinter/assets/themes/green.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994736842105263%*

 * *Differences: {"'CTkSwitch'": "{'fg_color': ['#939BA2', '#4A4D50'], delete: ['fg_Color']}"}*

```diff
@@ -291,15 +291,15 @@
         ],
         "button_hover_color": [
             "gray20",
             "gray100"
         ],
         "button_length": 0,
         "corner_radius": 1000,
-        "fg_Color": [
+        "fg_color": [
             "#939BA2",
             "#4A4D50"
         ],
         "progress_color": [
             "#2CC985",
             "#2FA572"
         ],
```

### Comparing `customtkinter-5.1.2/customtkinter/windows/ctk_input_dialog.py` & `customtkinter-5.1.3/customtkinter/windows/ctk_input_dialog.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/ctk_tk.py` & `customtkinter-5.1.3/customtkinter/windows/ctk_tk.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/ctk_toplevel.py` & `customtkinter-5.1.3/customtkinter/windows/ctk_toplevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class CTkToplevel(tkinter.Toplevel, CTkAppearanceModeBaseClass, CTkScalingBaseClass):
     """
     Toplevel window with dark titlebar on Windows and macOS.
     For detailed information check out the documentation.
     """
 
-    _valid_tk_toplevel_arguments: set = {"bd", "borderwidth", "class", "container", "cursor", "height",
+    _valid_tk_toplevel_arguments: set = {"master", "bd", "borderwidth", "class", "container", "cursor", "height",
                                          "highlightbackground", "highlightthickness", "menu", "relief",
                                          "screen", "takefocus", "use", "visual", "width"}
 
     _deactivate_macos_window_header_manipulation: bool = False
     _deactivate_windows_window_header_manipulation: bool = False
 
     def __init__(self, *args,
```

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/__init__.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/ctk_canvas.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/ctk_canvas.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/core_rendering/draw_engine.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/draw_engine.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_button.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_button.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_checkbox.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_checkbox.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_combobox.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_combobox.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_entry.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_entry.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_frame.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_frame.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_label.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .utility import pop_from_dict_by_set, check_kwargs_empty
 
 
 class CTkLabel(CTkBaseClass):
     """
     Label with rounded corners. Default is fg_color=None (transparent fg_color).
     For detailed information check out the documentation.
+
+    state argument will probably be removed because it has no effect
     """
 
     # attributes that are passed to and managed by the tkinter entry only:
     _valid_tk_label_attributes = {"cursor", "justify", "padx", "pady",
                                   "textvariable", "state", "takefocus", "underline"}
 
     def __init__(self,
```

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_optionmenu.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_optionmenu.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_progressbar.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_progressbar.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_radiobutton.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_radiobutton.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_scrollable_frame.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_scrollable_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,18 +177,18 @@
                 if isinstance(child, CTkBaseClass):
                     child.configure(bg_color=self._parent_frame.cget("fg_color"))
 
         if "scrollbar_fg_color" in kwargs:
             self._scrollbar.configure(fg_color=kwargs.pop("scrollbar_fg_color"))
 
         if "scrollbar_button_color" in kwargs:
-            self._scrollbar.configure(fg_color=kwargs.pop("scrollbar_button_color"))
+            self._scrollbar.configure(button_color=kwargs.pop("scrollbar_button_color"))
 
         if "scrollbar_button_hover_color" in kwargs:
-            self._scrollbar.configure(fg_color=kwargs.pop("scrollbar_button_hover_color"))
+            self._scrollbar.configure(button_hover_color=kwargs.pop("scrollbar_button_hover_color"))
 
         if "label_text" in kwargs:
             self._label_text = kwargs.pop("label_text")
             self._label.configure(text=self._label_text)
             self._create_grid()
 
         if "label_font" in kwargs:
```

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_scrollbar.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_scrollbar.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_segmented_button.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_segmented_button.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_slider.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_slider.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_switch.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_switch.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         # dimensions
         self._switch_width = switch_width
         self._switch_height = switch_height
 
         # color
         self._border_color = self._check_color_type(border_color, transparency=True)
-        self._fg_color = ThemeManager.theme["CTkSwitch"]["fg_Color"] if fg_color is None else self._check_color_type(fg_color)
+        self._fg_color = ThemeManager.theme["CTkSwitch"]["fg_color"] if fg_color is None else self._check_color_type(fg_color)
         self._progress_color = ThemeManager.theme["CTkSwitch"]["progress_color"] if progress_color is None else self._check_color_type(progress_color, transparency=True)
         self._button_color = ThemeManager.theme["CTkSwitch"]["button_color"] if button_color is None else self._check_color_type(button_color)
         self._button_hover_color = ThemeManager.theme["CTkSwitch"]["button_hover_color"] if button_hover_color is None else self._check_color_type(button_hover_color)
         self._text_color = ThemeManager.theme["CTkSwitch"]["text_color"] if text_color is None else self._check_color_type(text_color)
         self._text_color_disabled = ThemeManager.theme["CTkSwitch"]["text_color_disabled"] if text_color_disabled is None else self._check_color_type(text_color_disabled)
 
         # text
@@ -295,28 +295,36 @@
             self._set_cursor()
             require_redraw = True
 
         if "fg_color" in kwargs:
             self._fg_color = self._check_color_type(kwargs.pop("fg_color"))
             require_redraw = True
 
+        if "border_color" in kwargs:
+            self._border_color = self._check_color_type(kwargs.pop("border_color"), transparency=True)
+            require_redraw = True
+
         if "progress_color" in kwargs:
             self._progress_color = self._check_color_type(kwargs.pop("progress_color"), transparency=True)
             require_redraw = True
 
         if "button_color" in kwargs:
             self._button_color = self._check_color_type(kwargs.pop("button_color"))
             require_redraw = True
 
         if "button_hover_color" in kwargs:
             self._button_hover_color = self._check_color_type(kwargs.pop("button_hover_color"))
             require_redraw = True
 
-        if "border_color" in kwargs:
-            self._border_color = self._check_color_type(kwargs.pop("border_color"), transparency=True)
+        if "text_color" in kwargs:
+            self._text_color = self._check_color_type(kwargs.pop("text_color"))
+            require_redraw = True
+
+        if "text_color_disabled" in kwargs:
+            self._text_color_disabled = self._check_color_type(kwargs.pop("text_color_disabled"))
             require_redraw = True
 
         if "hover" in kwargs:
             self._hover = kwargs.pop("hover")
 
         if "command" in kwargs:
             self._command = kwargs.pop("command")
```

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_tabview.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_tabview.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,17 +95,17 @@
         self._name_list: List[str] = []  # list of unique tab names in order of tabs
         self._current_name: str = ""
         self._command = command
 
         self._draw()
 
     def _segmented_button_callback(self, selected_name):
+        self._set_grid_tab_by_name(selected_name)
+        self._tab_dict[self._current_name].grid_forget()
         self._current_name = selected_name
-        self._grid_forget_all_tabs()
-        self._set_grid_tab_by_name(self._current_name)
 
         if self._command is not None:
             self._command()
 
     def winfo_children(self) -> List[any]:
         """
         winfo_children of CTkTabview without canvas and segmented button widgets,
```

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/ctk_textbox.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_textbox.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/font/__init__.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/font/__init__.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/font/ctk_font.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/font/ctk_font.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/font/font_manager.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/font/font_manager.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/image/ctk_image.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/image/ctk_image.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/scaling/scaling_base_class.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/scaling/scaling_base_class.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/scaling/scaling_tracker.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/scaling/scaling_tracker.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/theme/theme_manager.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/theme/theme_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 import os
+import pathlib
 import json
 from typing import List, Union
 
 
 class ThemeManager:
 
     theme: dict = {}  # contains all the theme data
@@ -11,15 +12,16 @@
     _currently_loaded_theme: Union[str, None] = None
 
     @classmethod
     def load_theme(cls, theme_name_or_path: str):
         script_directory = os.path.dirname(os.path.abspath(__file__))
 
         if theme_name_or_path in cls._built_in_themes:
-            with open(os.path.join(script_directory, "../../../assets", "themes", f"{theme_name_or_path}.json"), "r") as f:
+            customtkinter_path = pathlib.Path(script_directory).parent.parent.parent
+            with open(os.path.join(customtkinter_path, "assets", "themes", f"{theme_name_or_path}.json"), "r") as f:
                 cls.theme = json.load(f)
         else:
             with open(theme_name_or_path, "r") as f:
                 cls.theme = json.load(f)
 
         # store theme path for saving
         cls._currently_loaded_theme = theme_name_or_path
```

### Comparing `customtkinter-5.1.2/customtkinter/windows/widgets/utility/utility_functions.py` & `customtkinter-5.1.3/customtkinter/windows/widgets/utility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/customtkinter.egg-info/SOURCES.txt` & `customtkinter-5.1.3/customtkinter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.2/setup.cfg` & `customtkinter-5.1.3/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [metadata]
 name = customtkinter
-version = 5.1.2
+version = 5.1.3
 description = Create modern looking GUIs with Python
-long_description = A modern and customizable python UI-library based on Tkinter: https://github.com/TomSchimansky/CustomTkinter
+long_description = A modern and customizable python UI-library based on Tkinter: https://customtkinter.tomschimansky.com
 long_description_content_type = text/markdown
-url = https://github.com/TomSchimansky/CustomTkinter
+url = https://customtkinter.tomschimansky.com
 author = Tom Schimansky
 license = Creative Commons Zero v1.0 Universal
 license_file = LICENSE
 classifiers = 
 	License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 
+[project.urls]
+homepage = https://customtkinter.tomschimansky.com
+documentation = https://customtkinter.tomschimansky.com/documentation
+repository = https://github.com/tomschimansky/customtkinter
+
 [options]
 python_requires = >=3.7
 packages = 
 	customtkinter
 	customtkinter.windows
 	customtkinter.windows.widgets
 	customtkinter.windows.widgets.appearance_mode
```

