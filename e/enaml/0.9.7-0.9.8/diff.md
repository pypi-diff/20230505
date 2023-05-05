# Comparing `tmp/enaml-0.9.7.tar.gz` & `tmp/enaml-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/enaml-0.9.7.tar", last modified: Sun Jun 15 17:18:46 2014, max compression
+gzip compressed data, was "dist/enaml-0.9.8.tar", last modified: Sun Aug 17 11:22:00 2014, max compression
```

## Comparing `enaml-0.9.7.tar` & `enaml-0.9.8.tar`

### file list

```diff
@@ -1,741 +1,671 @@
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3731 2014-02-01 16:00:44.000000 enaml-0.9.7/COPYING.txt
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml.egg-info/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)        6 2014-06-15 17:18:42.000000 enaml-0.9.7/enaml.egg-info/top_level.txt
--rw-rw-r--   0 silvester  (1000) silvester  (1000)       49 2014-06-15 17:18:42.000000 enaml-0.9.7/enaml.egg-info/entry_points.txt
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    22005 2014-06-15 17:18:42.000000 enaml-0.9.7/enaml.egg-info/SOURCES.txt
--rw-rw-r--   0 silvester  (1000) silvester  (1000)       55 2014-06-15 17:18:42.000000 enaml-0.9.7/enaml.egg-info/requires.txt
--rw-rw-r--   0 silvester  (1000) silvester  (1000)        1 2014-06-15 17:18:42.000000 enaml-0.9.7/enaml.egg-info/dependency_links.txt
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1512 2014-06-15 17:18:42.000000 enaml-0.9.7/enaml.egg-info/PKG-INFO
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/licenses/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    24485 2014-02-01 16:00:45.000000 enaml-0.9.7/licenses/byteplay.txt
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/tools/
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/vim/
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/vim/ftdetect/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)       62 2014-06-15 01:02:22.000000 enaml-0.9.7/tools/vim/ftdetect/enaml.vim
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/vim/indent/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      419 2014-02-01 16:00:45.000000 enaml-0.9.7/tools/vim/indent/enaml.vim
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/vim/syntax/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1402 2014-02-01 16:00:45.000000 enaml-0.9.7/tools/vim/syntax/enaml.vim
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      431 2014-02-01 16:00:45.000000 enaml-0.9.7/tools/vim/README.txt
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/emacs/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1191 2014-02-01 16:00:45.000000 enaml-0.9.7/tools/emacs/enaml.el
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      503 2014-02-01 16:00:45.000000 enaml-0.9.7/tools/emacs/README.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/sublimetext/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    17200 2014-06-15 01:02:22.000000 enaml-0.9.7/tools/sublimetext/Enaml.tmLanguage
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    10530 2014-06-15 01:02:22.000000 enaml-0.9.7/tools/sublimetext/Enaml.JSON-tmLanguage
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/pygments/
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/tools/pygments/build/
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/tools/pygments/build/lib/
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/pygments/build/lib/enamllexer/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3639 2014-02-01 16:00:45.000000 enaml-0.9.7/tools/pygments/build/lib/enamllexer/lexer.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:45.000000 enaml-0.9.7/tools/pygments/build/lib/enamllexer/__init__.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/pygments/dist/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3981 2014-02-17 13:12:41.000000 enaml-0.9.7/tools/pygments/dist/enamllexer-0.0.0-py2.7.egg
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/pygments/enamllexer.egg-info/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)       11 2014-02-17 13:12:41.000000 enaml-0.9.7/tools/pygments/enamllexer.egg-info/top_level.txt
--rw-rw-r--   0 silvester  (1000) silvester  (1000)       63 2014-02-17 13:12:41.000000 enaml-0.9.7/tools/pygments/enamllexer.egg-info/entry_points.txt
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      224 2014-02-17 13:12:41.000000 enaml-0.9.7/tools/pygments/enamllexer.egg-info/SOURCES.txt
--rw-rw-r--   0 silvester  (1000) silvester  (1000)        1 2014-02-17 13:12:41.000000 enaml-0.9.7/tools/pygments/enamllexer.egg-info/dependency_links.txt
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      195 2014-02-01 16:00:45.000000 enaml-0.9.7/tools/pygments/setup.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tools/pygments/enamllexer/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3639 2014-02-01 16:00:45.000000 enaml-0.9.7/tools/pygments/enamllexer/lexer.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:45.000000 enaml-0.9.7/tools/pygments/enamllexer/__init__.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/tests/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      705 2014-02-01 16:00:45.000000 enaml-0.9.7/tests/test_q_resource_helpers.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    16900 2014-02-01 16:00:45.000000 enaml-0.9.7/tests/test_template.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    15290 2014-02-01 16:00:45.000000 enaml-0.9.7/tests/test_stylesheet.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    16403 2014-02-01 16:00:45.000000 enaml-0.9.7/tests/test_alias.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1115 2014-02-01 16:00:45.000000 enaml-0.9.7/tests/utils.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2745 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/index.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/api_ref/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      750 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/index.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      323 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/validator.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/api_ref/core/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      367 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/core/index.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      292 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/core/object.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      300 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/core/declarative.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      185 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/core/include.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      185 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/core/pattern.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      209 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/core/conditional.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      179 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/core/looper.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      537 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/application.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      171 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/version.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/api_ref/widgets/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2868 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/index.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      207 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/combo_box.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      225 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/action_group.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      201 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/spin_box.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      201 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/tool_bar.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      203 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/calendar.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      225 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/radio_button.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      265 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/dock_events.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      207 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/dock_area.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      213 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/mpl_canvas.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      219 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/frame.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      207 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/group_box.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      185 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/field.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      213 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/image_view.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      179 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/page.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      207 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/check_box.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      191 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/action.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      225 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/bounded_time.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      203 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/notebook.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      185 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/timer.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      225 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/color_dialog.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      243 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/multiline_field.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      207 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/dock_item.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      213 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/raw_widget.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      225 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/object_combo.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      219 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/scroll_area.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      261 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/constraints_widget.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      219 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/main_window.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      201 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/web_view.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      179 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/menu.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      219 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/file_dialog.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      219 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/status_item.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      237 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/toolkit_dialog.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      235 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/file_dialog_ex.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      191 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/widget.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      237 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/toolkit_object.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      213 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/split_item.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      179 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/form.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      179 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/html.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      243 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/abstract_button.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      209 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/container.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      213 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/status_bar.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      219 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/dual_slider.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      191 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/dialog.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      231 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/time_selector.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      201 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/mdi_area.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      209 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/separator.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      207 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/flow_item.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      249 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/bounded_datetime.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      225 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/bounded_date.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      185 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/label.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      255 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/datetime_selector.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      191 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/slider.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      213 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/popup_view.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      231 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/date_selector.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      225 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/progress_bar.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      207 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/dock_pane.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      201 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/menu_bar.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      203 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/splitter.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      207 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/flow_area.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      191 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/window.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      219 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/push_button.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      213 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/mdi_window.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      197 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/control.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      227 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/stack.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      213 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/widgets/stack_item.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      317 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/styling.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      153 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/image.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/api_ref/scintilla/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      248 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/scintilla/index.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      273 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/scintilla/scintilla.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      219 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/scintilla/idle_theme.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      282 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/colors.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      189 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/nodevisitor.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      273 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/fonts.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/api_ref/stdlib/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      230 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/stdlib/index.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      275 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/stdlib/fields.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      215 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/stdlib/mapped_view.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/api_ref/applib/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      278 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/applib/index.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      433 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/applib/live_editor_view.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      249 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/applib/live_editor_model.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      187 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/icon.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/api_ref/layout/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      254 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/layout/index.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      193 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/layout/layout_helpers.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1127 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/api_ref/layout/dock_layout.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/dev_guides/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      766 2014-06-15 01:02:29.000000 enaml-0.9.7/docs/source/dev_guides/index.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/dev_guides/code/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      679 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/dev_guides/code/pseudo_class_style.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1157 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/dev_guides/code/cascade_style.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      603 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/dev_guides/code/pseudo_element_style.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1455 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/dev_guides/code/specificity_style.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      484 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/dev_guides/code/simple_style.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1079 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/dev_guides/code/selector_style.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    13067 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/dev_guides/stylesheets.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/faqs/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      185 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/faqs/index.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/get_started/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2017 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/get_started/index.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5596 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/get_started/installation.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/get_started/code/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      127 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/get_started/code/person_model.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      559 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/get_started/code/win_hierarchy.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      355 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/get_started/code/main.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      357 2014-06-15 01:02:22.000000 enaml-0.9.7/docs/source/get_started/code/person_view.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)       91 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/get_started/layout.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)       70 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/get_started/models.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7242 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/get_started/anatomy.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9877 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/get_started/introduction.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/images/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2638 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/images/simple_style.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2494 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/images/pseudo_class_style.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3817 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/images/specificity_style.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    13813 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/images/abs_hierarchy.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3000 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/images/pseudo_element_style.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2987 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/images/win_hierarchy.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3271 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/images/selector_style.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2474 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/images/person_view.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3272 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/images/cascade_style.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    10464 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/conf.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/arch_ref/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      105 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/arch_ref/index.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/examples/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2476 2014-06-15 01:02:29.000000 enaml-0.9.7/docs/source/examples/index.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7540 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/tut_person.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4307 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/tut_hello_world.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5173 2014-02-17 12:38:06.000000 enaml-0.9.7/docs/source/examples/example_doc_generator.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9567 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/tut_employee.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/examples/images/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    99379 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/img3.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   137280 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/img2.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    31531 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/tut_employee_layout_nested_container.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    12171 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/tut_john_doe_error.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    29825 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/tut_employee_layout.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    10978 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/tut_john_doe_jr.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11486 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/tut_hello_world_python.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    29819 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/tut_employee_layout_no_midline.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    10268 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/tut_john_doe.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   107532 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/img1.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    10013 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/examples/images/tut_hello_world.png
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/docs/source/_sphinxext/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6889 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/_sphinxext/enamldoc.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)        0 2014-02-13 02:12:28.000000 enaml-0.9.7/docs/source/_sphinxext/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2466 2014-06-15 01:02:22.000000 enaml-0.9.7/setup.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    21500 2014-06-15 01:02:22.000000 enaml-0.9.7/releasenotes.rst
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      997 2014-02-01 16:00:44.000000 enaml-0.9.7/README.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    21812 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/styling.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1435 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/icon.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      669 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/objectdict.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/core/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5382 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/core/standard_tracer.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4474 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/declarative_meta.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    22451 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/compiler_helpers.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    19555 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/compiler_common.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2371 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/core/standard_inverter.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    13677 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/code_generator.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9763 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/enaml_ast.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5092 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/dynamic_template.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11984 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/compiler_nodes.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3754 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/core/pattern.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9473 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/operators.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    12062 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/enaml_compiler.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7863 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/expression_engine.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    13127 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/object.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11514 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/core/template_compiler.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      565 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/api.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    24433 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/lexer.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      542 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/core/template_.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5027 2014-06-15 01:02:29.000000 enaml-0.9.7/enaml/core/declarative_function.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5730 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/looper.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5974 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/block_compiler.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3943 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/core/standard_handlers.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3085 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/conditional.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    14994 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/import_hooks.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8843 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/enamldef_compiler.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   101454 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/parser.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2554 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/enamldef_meta.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/core/parse_tab/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)        0 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/parse_tab/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   190702 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/parse_tab/parsetab.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6224 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/parse_tab/lextab.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    14868 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/code_tracing.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4758 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/core/declarative.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8361 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/core/template.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    33903 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/byteplay.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4965 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/core/include.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2288 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/runner.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    13101 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/colors.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/enaml/widgets/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2494 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/action_group.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5496 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/color_dialog.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2924 2014-02-17 03:35:34.000000 enaml-0.9.7/enaml/widgets/combo_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1591 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/mdi_area.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1467 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/radio_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1343 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/check_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1565 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/html.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2308 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/v_group.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7666 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/dock_area.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3667 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/separator.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3251 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/flow_area.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1030 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/menu_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2098 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/datetime_selector.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5506 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/tool_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3114 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/multiline_field.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2885 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/status_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4792 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/dock_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2678 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/timer.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6972 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/file_dialog_ex.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5697 2014-06-15 01:02:29.000000 enaml-0.9.7/enaml/widgets/container.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7247 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/slider.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4343 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/form.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1721 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/dock_events.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2032 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/tool_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3331 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/stack.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7566 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/dual_slider.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2000 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/raw_widget.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5341 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/file_dialog.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4527 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/dock_pane.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2922 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/abstract_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2093 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/web_view.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9289 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/popup_view.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2382 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/api.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3549 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/bounded_time.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4673 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/spin_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11906 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/widgets/window.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1969 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/group_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3817 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/bounded_date.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2962 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/scroll_area.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2140 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/date_selector.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3036 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/menu.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2048 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/mpl_canvas.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2257 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/frame.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1630 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/mdi_window.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      888 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/calendar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2624 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/dialog.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9448 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/widget.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5720 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/field.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3482 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/page.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2441 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/split_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2404 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/ipython_console.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1213 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/focus_tracker.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1748 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/push_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3745 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/bounded_datetime.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3242 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/notebook.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2441 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/splitter.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2300 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/main_window.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2430 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/widgets/vtk_canvas.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3099 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/object_combo.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1282 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/stack_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5269 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/toolkit_dialog.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4186 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/constraints_widget.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1058 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/control.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3176 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/flow_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8491 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/toolkit_object.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2312 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/image_view.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2100 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/label.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2098 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/status_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3836 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/action.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1806 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/widgets/time_selector.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5107 2014-02-17 03:35:34.000000 enaml-0.9.7/enaml/widgets/progress_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2500 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/widgets/h_group.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1228 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/version.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2417 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/image.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    16584 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/application.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5762 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/fonts.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/src/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6998 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/callableref.cpp
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    27916 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/signaling.cpp
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9697 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/alias.cpp
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6848 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/winutil.cpp
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7219 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/colorext.cpp
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      738 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/inttypes.h
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    26300 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/dynamicscope.cpp
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11200 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/pythonhelpers.h
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3244 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/funchelper.cpp
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    12075 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/src/declfunction.cpp
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9561 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/fontext.cpp
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11326 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/weakmethod.cpp
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    16846 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/pythonhelpersex.h
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    18656 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/src/compiler_helpers.cpp
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/scintilla/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1682 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/scintilla/idle_theme.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      402 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/scintilla/api.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/scintilla/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      520 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/scintilla/mono_font.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5711 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/scintilla/scintilla.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2392 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/__init__.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/stdlib/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6967 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/stdlib/task_dialog.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7353 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/stdlib/slider_transform.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3144 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/stdlib/dialog_buttons.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    19181 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/stdlib/dock_area_styles.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/stdlib/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2133 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/stdlib/mapped_view.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9550 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/stdlib/message_box.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1621 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/stdlib/fields.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5132 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/validator.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/enaml/workbench/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1482 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/extension_point.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2072 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/plugin_manifest.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/enaml/workbench/core/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      901 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/core/execution_event.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      379 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/core/api.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/core/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      865 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/core/command.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5423 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/workbench/core/core_plugin.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1262 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/core/core_manifest.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1598 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/plugin.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      531 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/api.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2602 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/workbench/extension.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    10608 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/workbench.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/enaml/workbench/ui/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1744 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/workspace.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      710 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/branding.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1147 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/workbench_window.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1413 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/ui_workbench.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2034 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/workbench_menus.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    13926 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/ui_plugin.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      633 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/autostart.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      587 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/api.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      863 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/item_group.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1330 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/menu_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    10191 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/workbench/ui/menu_helper.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1800 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/action_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      854 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/window_model.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5737 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/workbench/ui/ui_manifest.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/applib/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3923 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/applib/live_editor_view.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:44.000000 enaml-0.9.7/enaml/applib/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7972 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/applib/live_editor_model.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/layout/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2067 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/layout/factory_helper.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    22147 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/dock_layout.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3843 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/layout/layout_helpers.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9542 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/geometry.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3019 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/constraint_helper.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5627 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/constrainable.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6898 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/linear_box_helper.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    17035 2014-06-15 01:02:29.000000 enaml-0.9.7/enaml/layout/layout_manager.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      804 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/layout/api.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    10620 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/grid_helper.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6860 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/sequence_helper.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6604 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/spacers.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      658 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/linear_symbolic.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1463 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/box_helper.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1234 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/layout/strength_member.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3370 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/nodevisitor.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/enaml/wx/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9965 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_page.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1782 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_html.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3598 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_toolkit_object.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2599 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_deferred_caller.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2329 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/wx/wx_label.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    16857 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_spin_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1338 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_frame.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    14368 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_action.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2146 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/wx/wx_single_widget_sizer.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4031 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_factories.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11313 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_action_group.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      647 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_control.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    21743 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_dock_pane.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4221 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_check_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3608 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_bounded_date.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8127 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_group_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2927 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_application.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3288 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_date_selector.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8699 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_menu_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2136 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_push_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7825 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/wx/wx_scroll_area.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6823 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_radio_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    14723 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_main_window.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5080 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/wx/wx_widget.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2631 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_calendar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      660 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_layout_request.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2724 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_combo_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3639 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/wx/wx_abstract_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3558 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/wx/wx_constraints_widget.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    12503 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/wx/wx_window.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    23128 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/wx/wx_menu.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    16741 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/wx/wx_notebook.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3324 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/wx/wx_mpl_canvas.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    10017 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/wx/wx_splitter.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2212 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_progress_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5316 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_resource_helpers.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/enaml/wx/wx_upstream/
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   370070 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/framemanager.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    33685 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/aui_switcherdialog.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   169381 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/aui_constants.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   135311 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/auibar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    16381 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   201431 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/auibook.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    46060 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/dockart.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   108900 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/tabart.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    20945 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/aui_utilities.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    18049 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/aui/tabmdi.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_upstream/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    21408 2014-06-15 01:02:29.000000 enaml-0.9.7/enaml/wx/wx_container.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4826 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_split_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    15855 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/wx/wx_tool_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11226 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_field.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8078 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/wx/wx_slider.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/qt/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2555 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_calendar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    13276 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_widget.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3341 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/qt_dialog.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8948 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_image_view.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7117 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_ipython_console.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8030 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/qt_scroll_area.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1548 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_html.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      647 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_control.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5775 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_object_combo.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5352 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_popup_view.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9280 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/qt_window.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4337 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_multiline_field.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1669 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_focus_tracker.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1806 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_web_view.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3505 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_datetime_selector.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    21020 2014-06-15 01:02:29.000000 enaml-0.9.7/enaml/qt/qt_container.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    39042 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/q_flow_layout.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1444 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/q_file_dialog_helper.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4676 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_group_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9400 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/qt_main_window.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3835 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_spin_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4770 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_mdi_window.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3902 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_stack_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4504 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_slider.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    14565 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/q_pixmap_transition.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3101 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_application.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4844 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_action.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11610 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_page.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    14227 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_dual_slider.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5075 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/q_window_base.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5330 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/q_resource_helpers.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    14017 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/qt_stack.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3618 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_separator.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6321 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_file_dialog_ex.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3042 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_push_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3051 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_bounded_datetime.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2878 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_toolkit_dialog.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      941 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/QtCore.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2877 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_bounded_date.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3133 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_menu_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    12433 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_scintilla.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5957 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_split_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      463 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/QtTest.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2976 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_time_selector.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      859 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_check_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3776 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_constraints_widget.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2373 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_file_dialog.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      881 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_radio_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3232 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_mdi_area.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      467 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/QtScript.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9363 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/qt_dock_area.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2879 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_label.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1150 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5546 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_color_dialog.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4571 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_abstract_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2105 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_progress_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6840 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/q_single_widget_layout.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4666 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_toolkit_object.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11572 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_dock_pane.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2851 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_status_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1029 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_raw_widget.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4167 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/scintilla_lexers.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2899 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_bounded_time.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2639 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_timer.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    24526 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/scintilla_tokens.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8700 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_flow_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    18218 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/qt_notebook.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    11917 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_tool_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6992 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_action_group.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3305 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_date_selector.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    31111 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/q_popup_view.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3206 2014-02-17 14:15:03.000000 enaml-0.9.7/enaml/qt/qt_vtk_canvas.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7103 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/qt_field.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2880 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/q_pixmap_painter.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2084 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/focus_registry.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      469 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/QtNetwork.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7895 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_factories.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     9943 2014-06-15 01:02:29.000000 enaml-0.9.7/enaml/qt/styleutil.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8359 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_menu.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      467 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/QtWebKit.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/qt/docking/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5092 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/layout_saver.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    29657 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_dock_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      766 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/enaml_dock_resources.qrc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1872 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_dock_splitter.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2170 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/event_types.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6914 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_bitmap_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    26686 2014-06-15 01:02:29.000000 enaml-0.9.7/enaml/qt/docking/q_dock_container.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2855 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_icon_widget.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    20544 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/layout_handling.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    19977 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/layout_builder.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    20737 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_dock_title_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      350 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/__init__.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    21690 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/docking/dock_manager.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2406 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_dock_frame_layout.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    33027 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_resources.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    16941 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_dock_window.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    14405 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_dock_area.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1210 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/style_sheets.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    26806 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/docking/q_dock_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    15416 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_dock_frame.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      474 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/center.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      237 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/bar_horizontal.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      715 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/cross_ex_box.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      450 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/split_vertical.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      319 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/thin_horizontal.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      443 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/arrow_south.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      546 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/arrow_east.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      610 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/background.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    14712 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/guide_render.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      548 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/split_horizontal.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      194 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/guide_box.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      609 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/cross_box.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      334 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/bar_vertical.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      481 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/thin_vertical.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      440 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/arrow_north.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      550 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_images/arrow_west.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    23686 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_guide_rose.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3871 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/xbms.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    18455 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/dock_overlay.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4115 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_text_label.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      613 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/utils.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    15506 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/q_dock_tab_widget.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5910 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/docking/proximity_handler.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4543 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_status_bar.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3159 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_combo_box.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3669 2014-02-13 02:07:57.000000 enaml-0.9.7/enaml/qt/qt_mpl_canvas.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      467 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/QtOpenGL.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      461 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/QtSvg.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2252 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/q_deferred_caller.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3882 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_tool_button.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7302 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_dock_item.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6516 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_flow_area.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      461 2014-02-17 13:38:01.000000 enaml-0.9.7/enaml/qt/QtGui.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2010 2014-02-01 16:00:45.000000 enaml-0.9.7/enaml/qt/qt_frame.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8227 2014-06-15 01:02:22.000000 enaml-0.9.7/enaml/qt/qt_splitter.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/examples/
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/styling/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2571 2014-02-17 03:35:34.000000 enaml-0.9.7/examples/styling/banner.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2221 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/styling/gradient_push_button.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5356 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/styling/dock_item_alerts.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/widgets/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1781 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/dock_pane.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1498 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/popup_menu.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2030 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/group_box.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     5065 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/main_window.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2853 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/scroll_area.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/widgets/__enamlcache__/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3462 2014-02-17 13:42:22.000000 enaml-0.9.7/examples/widgets/__enamlcache__/vtk_canvas.enaml-py27-cv20.enamlc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7093 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/flow_area.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2419 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/focus_traversal.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      925 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/slider.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1570 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/v_group.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1802 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/dual_slider.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1279 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/mpl_canvas.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1534 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/form.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      623 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/window.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6227 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/dock_area.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1815 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/buttons.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      937 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/spin_box.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1713 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/h_group.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      899 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/window_closing.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3663 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/menu_bar.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1716 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/form_spacing.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2836 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/notebook.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1428 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/progress_bar.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1073 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/context_menu.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2345 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/tool_bar.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/widgets/images/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1550 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/images/document-open.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2215 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/images/system-search.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    99379 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/images/img3.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   137280 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/images/img2.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1008 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/images/document-new.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      317 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/images/list-remove.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2240 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/images/emblem-system.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)   107532 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/images/img1.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1200 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/images/go-previous.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      601 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/images/list-add.png
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2600 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/splitter.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3954 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/widgets/popup_view.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1432 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/window_children.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2449 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/widgets/tool_buttons.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1131 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/file_dialog.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1265 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/widgets/image_view.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1742 2014-02-17 13:16:55.000000 enaml-0.9.7/examples/widgets/vtk_canvas.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/templates/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     6919 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/templates/advanced.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2466 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/templates/basic.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/dynamic/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2777 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/dynamic/notebook_pages.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1669 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/dynamic/looper.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3216 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/dynamic/fields.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2620 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/dynamic/conditional.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/aliases/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1274 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/aliases/simple_attribute_alias.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1437 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/aliases/chained_widget_alias.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1667 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/aliases/chained_attribute_alias.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1050 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/aliases/simple_widget_alias.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/examples/tutorial/
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/tutorial/employee/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3502 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/tutorial/employee/employee_view.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2243 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/tutorial/employee/employee.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1760 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/tutorial/employee/phone_validator.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/tutorial/hello_world/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      688 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/tutorial/hello_world/hello_world.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      522 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/tutorial/hello_world/hello_world_view.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/tutorial/person/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1297 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/tutorial/person/person.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      848 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/tutorial/person/person_view.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/stdlib/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3801 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/stdlib/task_dialog.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      946 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/stdlib/slider_transform.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2506 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/stdlib/mapped_view.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3001 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/stdlib/message_box.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/workbench/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     4792 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/workbench/persistent_view.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    26500 2014-02-17 23:09:36.000000 enaml-0.9.7/examples/workbench/crash_course.rst
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/workbench/__enamlcache__/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7960 2014-06-15 01:03:40.000000 enaml-0.9.7/examples/workbench/__enamlcache__/first_view.enaml-py27-cv22.enamlc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8979 2014-02-17 12:10:47.000000 enaml-0.9.7/examples/workbench/__enamlcache__/second_view.enaml-py27-cv20.enamlc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    15101 2014-06-15 01:03:53.000000 enaml-0.9.7/examples/workbench/__enamlcache__/persistent_view.enaml-py27-cv22.enamlc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     7960 2014-02-17 12:10:44.000000 enaml-0.9.7/examples/workbench/__enamlcache__/first_view.enaml-py27-cv20.enamlc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    15142 2014-02-17 12:10:37.000000 enaml-0.9.7/examples/workbench/__enamlcache__/sample_plugin.enaml-py27-cv20.enamlc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    14403 2014-02-17 12:11:00.000000 enaml-0.9.7/examples/workbench/__enamlcache__/third_view.enaml-py27-cv20.enamlc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)    15028 2014-06-15 01:03:37.000000 enaml-0.9.7/examples/workbench/__enamlcache__/sample_plugin.enaml-py27-cv22.enamlc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     8979 2014-06-15 01:03:42.000000 enaml-0.9.7/examples/workbench/__enamlcache__/second_view.enaml-py27-cv22.enamlc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      765 2014-06-15 01:02:29.000000 enaml-0.9.7/examples/workbench/sample.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2036 2014-02-17 12:10:44.000000 enaml-0.9.7/examples/workbench/sample_workspace.pyc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3726 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/workbench/sample_plugin.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1566 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/workbench/first_view.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2535 2014-06-15 01:03:53.000000 enaml-0.9.7/examples/workbench/persistent_workspace.pyc
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2096 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/workbench/persistent_workspace.py
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1758 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/workbench/second_view.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1857 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/workbench/sample_workspace.py
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/applib/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2707 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/applib/live_editor.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:45.000000 enaml-0.9.7/examples/layout/
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/layout/basic/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1911 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/basic/align.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1120 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/basic/hbox_equal_widths.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1072 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/basic/horizontal.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2812 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/basic/grid.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1065 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/basic/vertical.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1662 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/basic/hbox.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1694 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/basic/linear_relations.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      958 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/basic/hbox_spacing.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1167 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/basic/vbox.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1870 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/basic/align_offset.enaml
-drwxrwxr-x   0 silvester  (1000) silvester  (1000)        0 2014-06-15 17:18:46.000000 enaml-0.9.7/examples/layout/advanced/
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2594 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/layout/advanced/nested_containers.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     3703 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/advanced/button_ring.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1646 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/layout/advanced/manual_vbox.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2062 2014-06-15 01:02:22.000000 enaml-0.9.7/examples/layout/advanced/factory_func.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2386 2014-02-01 16:00:45.000000 enaml-0.9.7/examples/layout/advanced/fluid.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1660 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/layout/advanced/nested_boxes.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1648 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/layout/advanced/manual_hbox.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     2206 2014-02-13 02:07:57.000000 enaml-0.9.7/examples/layout/advanced/find_replace.enaml
--rw-rw-r--   0 silvester  (1000) silvester  (1000)     1512 2014-06-15 17:18:46.000000 enaml-0.9.7/PKG-INFO
--rw-rw-r--   0 silvester  (1000) silvester  (1000)       59 2014-06-15 17:18:46.000000 enaml-0.9.7/setup.cfg
--rw-rw-r--   0 silvester  (1000) silvester  (1000)      413 2014-02-17 03:35:34.000000 enaml-0.9.7/MANIFEST.in
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      413 2014-08-17 11:18:55.000000 enaml-0.9.8/MANIFEST.in
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2466 2014-08-17 11:19:50.000000 enaml-0.9.8/setup.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1512 2014-08-17 11:22:00.000000 enaml-0.9.8/PKG-INFO
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       59 2014-08-17 11:22:00.000000 enaml-0.9.8/setup.cfg
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/templates/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2466 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/templates/basic.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6919 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/templates/advanced.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/tutorial/
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/tutorial/employee/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3502 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/tutorial/employee/employee_view.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2243 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/tutorial/employee/employee.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1760 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/tutorial/employee/phone_validator.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/tutorial/person/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      848 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/tutorial/person/person_view.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1297 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/tutorial/person/person.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/tutorial/hello_world/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      688 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/tutorial/hello_world/hello_world.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      522 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/tutorial/hello_world/hello_world_view.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/dynamic/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1669 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/dynamic/looper.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2620 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/dynamic/conditional.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3216 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/dynamic/fields.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2777 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/dynamic/notebook_pages.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/workbench/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    26500 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/workbench/crash_course.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3726 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/workbench/sample_plugin.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1857 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/workbench/sample_workspace.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1566 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/workbench/first_view.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2096 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/workbench/persistent_workspace.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4792 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/workbench/persistent_view.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      765 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/workbench/sample.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1758 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/workbench/second_view.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/aliases/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1437 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/aliases/chained_widget_alias.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1274 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/aliases/simple_attribute_alias.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1667 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/aliases/chained_attribute_alias.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1050 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/aliases/simple_widget_alias.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/styling/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5356 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/styling/dock_item_alerts.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2571 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/styling/banner.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2221 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/styling/gradient_push_button.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/applib/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2707 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/applib/live_editor.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/layout/
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/layout/basic/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1120 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/basic/hbox_equal_widths.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1662 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/basic/hbox.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1072 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/basic/horizontal.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1065 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/basic/vertical.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1911 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/basic/align.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      958 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/basic/hbox_spacing.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1694 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/basic/linear_relations.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1870 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/basic/align_offset.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1167 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/basic/vbox.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2812 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/basic/grid.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/layout/advanced/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1648 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/advanced/manual_hbox.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2062 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/advanced/factory_func.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2206 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/advanced/find_replace.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1646 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/advanced/manual_vbox.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3703 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/advanced/button_ring.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2386 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/advanced/fluid.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1660 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/advanced/nested_boxes.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2594 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/layout/advanced/nested_containers.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/widgets/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6227 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/dock_area.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1713 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/h_group.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1498 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/popup_menu.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1781 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/dock_pane.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2600 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/splitter.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1428 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/progress_bar.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5065 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/main_window.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7093 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/flow_area.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1570 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/v_group.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1131 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/file_dialog.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1742 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/vtk_canvas.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2030 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/group_box.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3663 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/menu_bar.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1432 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/window_children.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2345 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/tool_bar.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      623 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/window.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      937 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/spin_box.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2449 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/tool_buttons.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1265 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/image_view.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3954 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/popup_view.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2853 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/scroll_area.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3546 2014-08-17 11:19:50.000000 enaml-0.9.8/examples/widgets/drag_and_drop.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1073 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/context_menu.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2419 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/focus_traversal.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1815 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/buttons.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1716 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/form_spacing.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1802 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/dual_slider.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1279 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/mpl_canvas.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2836 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/notebook.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/widgets/images/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1008 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/images/document-new.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      601 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/images/list-add.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1550 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/images/document-open.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1200 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/images/go-previous.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)   107532 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/images/img1.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2215 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/images/system-search.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      317 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/images/list-remove.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    99379 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/images/img3.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2240 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/images/emblem-system.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)   137280 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/images/img2.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      899 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/window_closing.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      925 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/slider.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1534 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/widgets/form.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/examples/stdlib/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2506 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/stdlib/mapped_view.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3801 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/stdlib/task_dialog.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3001 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/stdlib/message_box.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      946 2014-08-17 11:18:55.000000 enaml-0.9.8/examples/stdlib/slider_transform.enaml
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/tests/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1115 2014-08-17 11:18:55.000000 enaml-0.9.8/tests/utils.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      705 2014-08-17 11:18:55.000000 enaml-0.9.8/tests/test_q_resource_helpers.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    15290 2014-08-17 11:18:55.000000 enaml-0.9.8/tests/test_stylesheet.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    16403 2014-08-17 11:18:55.000000 enaml-0.9.8/tests/test_alias.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    16900 2014-08-17 11:18:55.000000 enaml-0.9.8/tests/test_template.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      997 2014-08-17 11:18:55.000000 enaml-0.9.8/README.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    21858 2014-08-17 11:19:50.000000 enaml-0.9.8/releasenotes.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml.egg-info/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1512 2014-08-17 11:21:57.000000 enaml-0.9.8/enaml.egg-info/PKG-INFO
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    19825 2014-08-17 11:21:57.000000 enaml-0.9.8/enaml.egg-info/SOURCES.txt
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       49 2014-08-17 11:21:57.000000 enaml-0.9.8/enaml.egg-info/entry_points.txt
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       55 2014-08-17 11:21:57.000000 enaml-0.9.8/enaml.egg-info/requires.txt
+-rw-r--r--   0 silvester  (1000) silvester  (1000)        1 2014-08-17 11:21:57.000000 enaml-0.9.8/enaml.egg-info/dependency_links.txt
+-rw-r--r--   0 silvester  (1000) silvester  (1000)        6 2014-08-17 11:21:57.000000 enaml-0.9.8/enaml.egg-info/top_level.txt
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/tools/
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/tools/sublimetext/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    17200 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/sublimetext/Enaml.tmLanguage
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    10530 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/sublimetext/Enaml.JSON-tmLanguage
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/tools/emacs/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1191 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/emacs/enaml.el
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      503 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/emacs/README.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/tools/vim/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      431 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/vim/README.txt
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/tools/vim/indent/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      419 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/vim/indent/enaml.vim
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/tools/vim/syntax/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1402 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/vim/syntax/enaml.vim
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/tools/vim/ftdetect/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       62 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/vim/ftdetect/enaml.vim
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/tools/pygments/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      195 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/pygments/setup.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/tools/pygments/enamllexer/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3639 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/pygments/enamllexer/lexer.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/tools/pygments/enamllexer/__init__.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/licenses/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    24485 2014-08-17 11:18:55.000000 enaml-0.9.8/licenses/byteplay.txt
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/scintilla/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1682 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/scintilla/idle_theme.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      402 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/scintilla/api.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/scintilla/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      520 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/scintilla/mono_font.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5711 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/scintilla/scintilla.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5762 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/fonts.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4639 2014-08-17 11:19:50.000000 enaml-0.9.8/enaml/drag_drop.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3370 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/nodevisitor.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/workbench/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    10608 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/workbench.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/workbench/core/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      901 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/core/execution_event.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5423 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/core/core_plugin.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      379 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/core/api.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/core/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1262 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/core/core_manifest.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      865 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/core/command.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2602 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/extension.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1482 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/extension_point.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      531 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/api.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2072 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/plugin_manifest.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/workbench/ui/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      633 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/autostart.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5737 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/ui_manifest.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2034 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/workbench_menus.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      863 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/item_group.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1800 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/action_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    10191 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/menu_helper.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1330 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/menu_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      587 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/api.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1744 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/workspace.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      854 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/window_model.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1147 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/workbench_window.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      710 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/branding.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    13926 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/ui_plugin.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1413 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/ui/ui_workbench.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1598 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/workbench/plugin.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2417 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/image.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/core/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    33903 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/byteplay.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    11984 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/compiler_nodes.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    11514 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/template_compiler.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     8361 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/template.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2371 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/standard_inverter.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      542 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/template_.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3754 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/pattern.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2554 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/enamldef_meta.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5382 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/standard_tracer.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4965 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/include.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5092 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/dynamic_template.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    22451 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/compiler_helpers.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    24433 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/lexer.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    14994 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/import_hooks.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/core/parse_tab/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)   190702 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/parse_tab/parsetab.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/parse_tab/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6224 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/parse_tab/lextab.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3943 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/standard_handlers.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      565 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/api.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5730 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/looper.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9763 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/enaml_ast.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    13127 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/object.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    14868 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/code_tracing.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    13677 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/code_generator.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)   101454 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/parser.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4758 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/declarative.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3085 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/conditional.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    12062 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/enaml_compiler.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    19555 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/compiler_common.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5974 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/block_compiler.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     8843 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/enamldef_compiler.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5028 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/declarative_function.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9473 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/operators.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7863 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/expression_engine.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4474 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/core/declarative_meta.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      669 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/objectdict.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/qt/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7103 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_field.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2879 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_label.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      461 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/QtGui.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      467 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/QtScript.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9400 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_main_window.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    11917 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_tool_bar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      463 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/QtTest.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9363 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_dock_area.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5546 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_color_dialog.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      461 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/QtSvg.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2877 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_bounded_date.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6321 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_file_dialog_ex.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      881 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_radio_button.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     8030 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_scroll_area.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6516 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_flow_area.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/qt/docking/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    19977 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/layout_builder.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    20544 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/layout_handling.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    29657 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_dock_bar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      613 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/utils.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2170 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/event_types.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1210 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/style_sheets.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5092 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/layout_saver.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    23686 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_guide_rose.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5910 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/proximity_handler.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/qt/docking/dock_images/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      237 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/bar_horizontal.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      450 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/split_vertical.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      610 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/background.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      194 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/guide_box.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      550 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/arrow_west.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      546 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/arrow_east.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      334 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/bar_vertical.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      440 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/arrow_north.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      609 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/cross_box.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      481 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/thin_vertical.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      474 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/center.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      548 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/split_horizontal.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      715 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/cross_ex_box.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    14712 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/guide_render.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      319 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/thin_horizontal.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      443 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_images/arrow_south.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    14405 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_dock_area.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    33027 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_resources.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    18455 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_overlay.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    26754 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_dock_container.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    15416 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_dock_frame.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2406 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_dock_frame_layout.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6914 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_bitmap_button.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    16941 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_dock_window.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    15506 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_dock_tab_widget.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    20737 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_dock_title_bar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    26806 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_dock_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      766 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/enaml_dock_resources.qrc
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3871 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/xbms.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    21690 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/dock_manager.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2855 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_icon_widget.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1872 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_dock_splitter.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4115 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/docking/q_text_label.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      469 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/QtNetwork.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6992 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_action_group.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    11610 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_page.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1444 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/q_file_dialog_helper.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5775 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_object_combo.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4770 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_mdi_window.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4337 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_multiline_field.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3305 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_date_selector.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3042 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_push_button.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7302 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_dock_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2252 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/q_deferred_caller.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     8359 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_menu.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3232 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_mdi_area.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3902 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_stack_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3835 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_spin_box.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7117 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_ipython_console.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3552 2014-08-17 11:19:50.000000 enaml-0.9.8/enaml/qt/qt_drag_drop.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1029 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_raw_widget.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1669 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_focus_tracker.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    14017 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_stack.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9280 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_window.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    12433 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_scintilla.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1548 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_html.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      859 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_check_box.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2373 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_file_dialog.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3669 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_mpl_canvas.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3505 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_datetime_selector.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     8227 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_splitter.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2976 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_time_selector.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4844 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_action.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     8700 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_flow_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2880 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/q_pixmap_painter.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2878 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_toolkit_dialog.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3776 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_constraints_widget.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7895 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_factories.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      467 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/QtOpenGL.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    24526 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/scintilla_tokens.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    18218 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_notebook.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2899 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_bounded_time.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      647 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_control.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1806 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_web_view.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3882 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_tool_button.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2010 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_frame.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    10510 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/styleutil.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    11572 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_dock_pane.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2639 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_timer.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    39042 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/q_flow_layout.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2105 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_progress_bar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    17416 2014-08-17 11:19:50.000000 enaml-0.9.8/enaml/qt/qt_widget.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5330 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/q_resource_helpers.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2555 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_calendar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1150 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4571 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_abstract_button.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2768 2014-08-17 11:19:50.000000 enaml-0.9.8/enaml/qt/qt_mime_data.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6840 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/q_single_widget_layout.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      941 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/QtCore.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    31111 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/q_popup_view.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3051 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_bounded_datetime.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3618 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_separator.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4666 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_toolkit_object.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    14227 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_dual_slider.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5352 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_popup_view.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5957 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_split_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     8948 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_image_view.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4676 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_group_box.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3133 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_menu_bar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2851 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_status_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4543 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_status_bar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5075 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/q_window_base.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3159 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_combo_box.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    14565 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/q_pixmap_transition.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    21021 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_container.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2084 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/focus_registry.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3341 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_dialog.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4504 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_slider.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3402 2014-08-17 11:19:50.000000 enaml-0.9.8/enaml/qt/qt_application.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4167 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/scintilla_lexers.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3206 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/qt_vtk_canvas.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      467 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/qt/QtWebKit.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    13101 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/colors.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1435 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/icon.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2288 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/runner.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2306 2014-08-17 11:19:50.000000 enaml-0.9.8/enaml/mime_data.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5132 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/validator.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    21812 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/styling.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2392 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/__init__.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/src/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7219 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/colorext.cpp
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    12075 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/declfunction.cpp
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6998 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/callableref.cpp
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    27916 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/signaling.cpp
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    11326 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/weakmethod.cpp
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9697 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/alias.cpp
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    26300 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/dynamicscope.cpp
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      738 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/inttypes.h
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6848 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/winutil.cpp
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    11200 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/pythonhelpers.h
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3244 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/funchelper.cpp
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    16846 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/pythonhelpersex.h
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9561 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/fontext.cpp
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    18656 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/src/compiler_helpers.cpp
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/applib/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3923 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/applib/live_editor_view.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/applib/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7972 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/applib/live_editor_model.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1228 2014-08-17 11:19:50.000000 enaml-0.9.8/enaml/version.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/layout/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6604 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/spacers.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1463 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/box_helper.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    10620 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/grid_helper.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    22147 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/dock_layout.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1234 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/strength_member.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6860 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/sequence_helper.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6898 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/linear_box_helper.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      804 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/api.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9542 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/geometry.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3843 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/layout_helpers.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2067 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/factory_helper.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3019 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/constraint_helper.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5627 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/constrainable.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    17036 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/layout_manager.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      658 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/layout/linear_symbolic.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/widgets/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2678 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/timer.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1343 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/check_box.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1630 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/mdi_window.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5269 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/toolkit_dialog.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3176 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/flow_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2430 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/vtk_canvas.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2100 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/label.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1030 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/menu_bar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4343 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/form.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6972 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/file_dialog_ex.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5698 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/container.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2300 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/main_window.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1282 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/stack_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2308 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/v_group.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2048 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/mpl_canvas.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3114 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/multiline_field.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1721 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/dock_events.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1748 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/push_button.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5725 2014-08-17 11:19:50.000000 enaml-0.9.8/enaml/widgets/field.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2098 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/status_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2312 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/image_view.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4673 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/spin_box.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      888 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/calendar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9289 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/popup_view.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3036 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/menu.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3099 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/object_combo.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2962 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/scroll_area.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3331 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/stack.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5506 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/tool_bar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3251 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/flow_area.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2093 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/web_view.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7666 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/dock_area.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2924 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/combo_box.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3549 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/bounded_time.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2140 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/date_selector.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1467 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/radio_button.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1591 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/mdi_area.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1565 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/html.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5341 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/file_dialog.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1969 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/group_box.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1806 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/time_selector.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2382 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/api.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     8491 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/toolkit_object.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2257 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/frame.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2885 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/status_bar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5496 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/color_dialog.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2000 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/raw_widget.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3836 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/action.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4527 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/dock_pane.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2441 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/split_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2098 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/datetime_selector.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2500 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/h_group.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2922 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/abstract_button.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3745 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/bounded_datetime.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2494 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/action_group.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3242 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/notebook.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1213 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/focus_tracker.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7247 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/slider.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1058 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/control.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2624 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/dialog.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    12903 2014-08-17 11:19:50.000000 enaml-0.9.8/enaml/widgets/widget.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2441 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/splitter.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3817 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/bounded_date.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3667 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/separator.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7566 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/dual_slider.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2404 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/ipython_console.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3482 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/page.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2032 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/tool_button.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    11906 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/window.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4186 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/constraints_widget.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5107 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/progress_bar.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4792 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/widgets/dock_item.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    16852 2014-08-17 11:19:50.000000 enaml-0.9.8/enaml/application.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/enaml/stdlib/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2133 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/stdlib/mapped_view.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6967 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/stdlib/task_dialog.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3144 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/stdlib/dialog_buttons.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1621 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/stdlib/fields.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7353 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/stdlib/slider_transform.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9550 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/stdlib/message_box.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      350 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/stdlib/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    19181 2014-08-17 11:18:55.000000 enaml-0.9.8/enaml/stdlib/dock_area_styles.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3731 2014-08-17 11:18:55.000000 enaml-0.9.8/COPYING.txt
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/examples/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2607 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/index.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7540 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/tut_person.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4307 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/tut_hello_world.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5173 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/example_doc_generator.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9567 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/tut_employee.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/examples/images/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    15176 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/wb_third.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6890 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/wb_main.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    31531 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/tut_employee_layout_nested_container.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    10978 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/tut_john_doe_jr.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)   107532 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/img1.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    29819 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/tut_employee_layout_no_midline.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    11486 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/tut_hello_world_python.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    12727 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/wb_first.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    10013 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/tut_hello_world.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    15157 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/wb_second.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    99379 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/img3.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    12171 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/tut_john_doe_error.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)   137280 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/img2.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    29825 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/tut_employee_layout.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    10268 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/images/tut_john_doe.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      596 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/examples/wb_sample.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2745 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/index.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/api_ref/
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/api_ref/scintilla/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      248 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/scintilla/index.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      219 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/scintilla/idle_theme.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      273 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/scintilla/scintilla.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      750 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/index.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/api_ref/core/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      300 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/core/declarative.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      367 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/core/index.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      179 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/core/looper.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      292 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/core/object.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      185 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/core/include.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      209 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/core/conditional.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      185 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/core/pattern.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      187 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/icon.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      317 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/styling.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      171 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/version.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      323 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/validator.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      282 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/colors.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      153 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/image.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      273 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/fonts.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/api_ref/applib/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      278 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/applib/index.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      433 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/applib/live_editor_view.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      249 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/applib/live_editor_model.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      189 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/nodevisitor.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/api_ref/layout/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      254 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/layout/index.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      193 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/layout/layout_helpers.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1127 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/layout/dock_layout.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/api_ref/widgets/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      185 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/label.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      225 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/progress_bar.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      237 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/toolkit_dialog.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      219 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/dual_slider.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      249 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/bounded_datetime.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      225 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/bounded_date.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      225 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/radio_button.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      191 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/widget.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      227 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/stack.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      179 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/form.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      219 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/file_dialog.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      225 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/object_combo.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2868 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/index.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      231 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/time_selector.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      213 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/mpl_canvas.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      185 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/timer.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      213 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/status_bar.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      179 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/menu.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      197 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/control.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      203 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/notebook.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      243 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/abstract_button.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      213 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/split_item.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      203 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/splitter.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      255 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/datetime_selector.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      191 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/action.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      225 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/color_dialog.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      203 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/calendar.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      207 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/flow_area.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      209 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/container.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      219 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/status_item.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      207 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/group_box.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      191 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/window.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      265 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/dock_events.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      219 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/frame.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      213 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/raw_widget.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      207 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/dock_area.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      185 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/field.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      179 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/html.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      213 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/mdi_window.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      201 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/spin_box.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      207 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/check_box.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      207 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/combo_box.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      207 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/dock_item.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      231 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/date_selector.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      191 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/dialog.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      209 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/separator.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      219 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/scroll_area.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      219 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/main_window.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      225 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/action_group.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      201 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/mdi_area.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      213 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/stack_item.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      207 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/dock_pane.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      235 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/file_dialog_ex.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      179 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/page.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      207 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/flow_item.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      213 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/popup_view.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      237 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/toolkit_object.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      201 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/menu_bar.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      191 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/slider.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      201 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/tool_bar.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      219 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/push_button.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      243 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/multiline_field.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      261 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/constraints_widget.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      225 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/bounded_time.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      201 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/web_view.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      213 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/widgets/image_view.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      537 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/application.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/api_ref/stdlib/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      275 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/stdlib/fields.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      230 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/stdlib/index.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      215 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/api_ref/stdlib/mapped_view.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/get_started/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       91 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/get_started/layout.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2017 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/get_started/index.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       70 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/get_started/models.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/get_started/code/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      355 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/get_started/code/main.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      357 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/get_started/code/person_view.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      127 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/get_started/code/person_model.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      559 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/get_started/code/win_hierarchy.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     5596 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/get_started/installation.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     7242 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/get_started/anatomy.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9877 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/get_started/introduction.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/arch_ref/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      105 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/arch_ref/index.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/_sphinxext/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     6889 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/_sphinxext/enamldoc.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/_sphinxext/__init__.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/dev_guides/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1065 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/dev_guides/index.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/dev_guides/code/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1157 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/dev_guides/code/cascade_style.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      484 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/dev_guides/code/simple_style.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      603 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/dev_guides/code/pseudo_element_style.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      679 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/dev_guides/code/pseudo_class_style.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1079 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/dev_guides/code/selector_style.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1455 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/dev_guides/code/specificity_style.enaml
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    13067 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/dev_guides/stylesheets.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       76 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/dev_guides/workbenches.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/faqs/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      185 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/faqs/index.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    10464 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/conf.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2014-08-17 11:22:00.000000 enaml-0.9.8/docs/source/images/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)    13813 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/images/abs_hierarchy.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3000 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/images/pseudo_element_style.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2474 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/images/person_view.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2638 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/images/simple_style.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3272 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/images/cascade_style.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3817 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/images/specificity_style.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2987 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/images/win_hierarchy.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     3271 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/images/selector_style.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2494 2014-08-17 11:18:55.000000 enaml-0.9.8/docs/source/images/pseudo_class_style.png
```

### Comparing `enaml-0.9.7/COPYING.txt` & `enaml-0.9.8/COPYING.txt`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml.egg-info/SOURCES.txt` & `enaml-0.9.8/enaml.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -101,36 +101,42 @@
 docs/source/api_ref/widgets/toolkit_object.rst
 docs/source/api_ref/widgets/web_view.rst
 docs/source/api_ref/widgets/widget.rst
 docs/source/api_ref/widgets/window.rst
 docs/source/arch_ref/index.rst
 docs/source/dev_guides/index.rst
 docs/source/dev_guides/stylesheets.rst
+docs/source/dev_guides/workbenches.rst
 docs/source/dev_guides/code/cascade_style.enaml
 docs/source/dev_guides/code/pseudo_class_style.enaml
 docs/source/dev_guides/code/pseudo_element_style.enaml
 docs/source/dev_guides/code/selector_style.enaml
 docs/source/dev_guides/code/simple_style.enaml
 docs/source/dev_guides/code/specificity_style.enaml
 docs/source/examples/example_doc_generator.py
 docs/source/examples/index.rst
 docs/source/examples/tut_employee.rst
 docs/source/examples/tut_hello_world.rst
 docs/source/examples/tut_person.rst
+docs/source/examples/wb_sample.rst
 docs/source/examples/images/img1.png
 docs/source/examples/images/img2.png
 docs/source/examples/images/img3.png
 docs/source/examples/images/tut_employee_layout.png
 docs/source/examples/images/tut_employee_layout_nested_container.png
 docs/source/examples/images/tut_employee_layout_no_midline.png
 docs/source/examples/images/tut_hello_world.png
 docs/source/examples/images/tut_hello_world_python.png
 docs/source/examples/images/tut_john_doe.png
 docs/source/examples/images/tut_john_doe_error.png
 docs/source/examples/images/tut_john_doe_jr.png
+docs/source/examples/images/wb_first.png
+docs/source/examples/images/wb_main.png
+docs/source/examples/images/wb_second.png
+docs/source/examples/images/wb_third.png
 docs/source/faqs/index.rst
 docs/source/get_started/anatomy.rst
 docs/source/get_started/index.rst
 docs/source/get_started/installation.rst
 docs/source/get_started/introduction.rst
 docs/source/get_started/layout.rst
 docs/source/get_started/models.rst
@@ -146,17 +152,19 @@
 docs/source/images/selector_style.png
 docs/source/images/simple_style.png
 docs/source/images/specificity_style.png
 docs/source/images/win_hierarchy.png
 enaml/__init__.py
 enaml/application.py
 enaml/colors.py
+enaml/drag_drop.py
 enaml/fonts.py
 enaml/icon.py
 enaml/image.py
+enaml/mime_data.py
 enaml/nodevisitor.py
 enaml/objectdict.py
 enaml/runner.py
 enaml/styling.py
 enaml/validator.py
 enaml/version.py
 enaml.egg-info/PKG-INFO
@@ -255,14 +263,15 @@
 enaml/qt/qt_control.py
 enaml/qt/qt_date_selector.py
 enaml/qt/qt_datetime_selector.py
 enaml/qt/qt_dialog.py
 enaml/qt/qt_dock_area.py
 enaml/qt/qt_dock_item.py
 enaml/qt/qt_dock_pane.py
+enaml/qt/qt_drag_drop.py
 enaml/qt/qt_dual_slider.py
 enaml/qt/qt_factories.py
 enaml/qt/qt_field.py
 enaml/qt/qt_file_dialog.py
 enaml/qt/qt_file_dialog_ex.py
 enaml/qt/qt_flow_area.py
 enaml/qt/qt_flow_item.py
@@ -274,14 +283,15 @@
 enaml/qt/qt_ipython_console.py
 enaml/qt/qt_label.py
 enaml/qt/qt_main_window.py
 enaml/qt/qt_mdi_area.py
 enaml/qt/qt_mdi_window.py
 enaml/qt/qt_menu.py
 enaml/qt/qt_menu_bar.py
+enaml/qt/qt_mime_data.py
 enaml/qt/qt_mpl_canvas.py
 enaml/qt/qt_multiline_field.py
 enaml/qt/qt_notebook.py
 enaml/qt/qt_object_combo.py
 enaml/qt/qt_page.py
 enaml/qt/qt_popup_view.py
 enaml/qt/qt_progress_bar.py
@@ -479,67 +489,14 @@
 enaml/workbench/ui/ui_manifest.enaml
 enaml/workbench/ui/ui_plugin.py
 enaml/workbench/ui/ui_workbench.py
 enaml/workbench/ui/window_model.py
 enaml/workbench/ui/workbench_menus.enaml
 enaml/workbench/ui/workbench_window.enaml
 enaml/workbench/ui/workspace.py
-enaml/wx/__init__.py
-enaml/wx/wx_abstract_button.py
-enaml/wx/wx_action.py
-enaml/wx/wx_action_group.py
-enaml/wx/wx_application.py
-enaml/wx/wx_bounded_date.py
-enaml/wx/wx_calendar.py
-enaml/wx/wx_check_box.py
-enaml/wx/wx_combo_box.py
-enaml/wx/wx_constraints_widget.py
-enaml/wx/wx_container.py
-enaml/wx/wx_control.py
-enaml/wx/wx_date_selector.py
-enaml/wx/wx_deferred_caller.py
-enaml/wx/wx_dock_pane.py
-enaml/wx/wx_factories.py
-enaml/wx/wx_field.py
-enaml/wx/wx_frame.py
-enaml/wx/wx_group_box.py
-enaml/wx/wx_html.py
-enaml/wx/wx_label.py
-enaml/wx/wx_layout_request.py
-enaml/wx/wx_main_window.py
-enaml/wx/wx_menu.py
-enaml/wx/wx_menu_bar.py
-enaml/wx/wx_mpl_canvas.py
-enaml/wx/wx_notebook.py
-enaml/wx/wx_page.py
-enaml/wx/wx_progress_bar.py
-enaml/wx/wx_push_button.py
-enaml/wx/wx_radio_button.py
-enaml/wx/wx_resource_helpers.py
-enaml/wx/wx_scroll_area.py
-enaml/wx/wx_single_widget_sizer.py
-enaml/wx/wx_slider.py
-enaml/wx/wx_spin_box.py
-enaml/wx/wx_split_item.py
-enaml/wx/wx_splitter.py
-enaml/wx/wx_tool_bar.py
-enaml/wx/wx_toolkit_object.py
-enaml/wx/wx_widget.py
-enaml/wx/wx_window.py
-enaml/wx/wx_upstream/__init__.py
-enaml/wx/wx_upstream/aui/__init__.py
-enaml/wx/wx_upstream/aui/aui_constants.py
-enaml/wx/wx_upstream/aui/aui_switcherdialog.py
-enaml/wx/wx_upstream/aui/aui_utilities.py
-enaml/wx/wx_upstream/aui/auibar.py
-enaml/wx/wx_upstream/aui/auibook.py
-enaml/wx/wx_upstream/aui/dockart.py
-enaml/wx/wx_upstream/aui/framemanager.py
-enaml/wx/wx_upstream/aui/tabart.py
-enaml/wx/wx_upstream/aui/tabmdi.py
 examples/aliases/chained_attribute_alias.enaml
 examples/aliases/chained_widget_alias.enaml
 examples/aliases/simple_attribute_alias.enaml
 examples/aliases/simple_widget_alias.enaml
 examples/applib/live_editor.enaml
 examples/dynamic/conditional.enaml
 examples/dynamic/fields.enaml
@@ -579,14 +536,15 @@
 examples/tutorial/hello_world/hello_world_view.enaml
 examples/tutorial/person/person.py
 examples/tutorial/person/person_view.enaml
 examples/widgets/buttons.enaml
 examples/widgets/context_menu.enaml
 examples/widgets/dock_area.enaml
 examples/widgets/dock_pane.enaml
+examples/widgets/drag_and_drop.enaml
 examples/widgets/dual_slider.enaml
 examples/widgets/file_dialog.enaml
 examples/widgets/flow_area.enaml
 examples/widgets/focus_traversal.enaml
 examples/widgets/form.enaml
 examples/widgets/form_spacing.enaml
 examples/widgets/group_box.enaml
@@ -606,60 +564,42 @@
 examples/widgets/tool_bar.enaml
 examples/widgets/tool_buttons.enaml
 examples/widgets/v_group.enaml
 examples/widgets/vtk_canvas.enaml
 examples/widgets/window.enaml
 examples/widgets/window_children.enaml
 examples/widgets/window_closing.enaml
-examples/widgets/__enamlcache__/vtk_canvas.enaml-py27-cv20.enamlc
 examples/widgets/images/document-new.png
 examples/widgets/images/document-open.png
 examples/widgets/images/emblem-system.png
 examples/widgets/images/go-previous.png
 examples/widgets/images/img1.png
 examples/widgets/images/img2.png
 examples/widgets/images/img3.png
 examples/widgets/images/list-add.png
 examples/widgets/images/list-remove.png
 examples/widgets/images/system-search.png
 examples/workbench/crash_course.rst
 examples/workbench/first_view.enaml
 examples/workbench/persistent_view.enaml
 examples/workbench/persistent_workspace.py
-examples/workbench/persistent_workspace.pyc
 examples/workbench/sample.py
 examples/workbench/sample_plugin.enaml
 examples/workbench/sample_workspace.py
-examples/workbench/sample_workspace.pyc
 examples/workbench/second_view.enaml
-examples/workbench/__enamlcache__/first_view.enaml-py27-cv20.enamlc
-examples/workbench/__enamlcache__/first_view.enaml-py27-cv22.enamlc
-examples/workbench/__enamlcache__/persistent_view.enaml-py27-cv22.enamlc
-examples/workbench/__enamlcache__/sample_plugin.enaml-py27-cv20.enamlc
-examples/workbench/__enamlcache__/sample_plugin.enaml-py27-cv22.enamlc
-examples/workbench/__enamlcache__/second_view.enaml-py27-cv20.enamlc
-examples/workbench/__enamlcache__/second_view.enaml-py27-cv22.enamlc
-examples/workbench/__enamlcache__/third_view.enaml-py27-cv20.enamlc
 licenses/byteplay.txt
 tests/test_alias.py
 tests/test_q_resource_helpers.py
 tests/test_stylesheet.py
 tests/test_template.py
 tests/utils.py
 tools/emacs/README.rst
 tools/emacs/enaml.el
 tools/pygments/setup.py
-tools/pygments/build/lib/enamllexer/__init__.py
-tools/pygments/build/lib/enamllexer/lexer.py
-tools/pygments/dist/enamllexer-0.0.0-py2.7.egg
 tools/pygments/enamllexer/__init__.py
 tools/pygments/enamllexer/lexer.py
-tools/pygments/enamllexer.egg-info/SOURCES.txt
-tools/pygments/enamllexer.egg-info/dependency_links.txt
-tools/pygments/enamllexer.egg-info/entry_points.txt
-tools/pygments/enamllexer.egg-info/top_level.txt
 tools/sublimetext/Enaml.JSON-tmLanguage
 tools/sublimetext/Enaml.tmLanguage
 tools/vim/README.txt
 tools/vim/ftdetect/enaml.vim
 tools/vim/indent/enaml.vim
 tools/vim/syntax/enaml.vim
```

### Comparing `enaml-0.9.7/enaml.egg-info/PKG-INFO` & `enaml-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: enaml
-Version: 0.9.7
+Version: 0.9.8
 Summary: Declarative DSL for building rich user interfaces in Python
 Home-page: https://github.com/nucleic/enaml
 Author: The Nucleic Development Team
 Author-email: sccolbert@gmail.com
 License: UNKNOWN
 Description: Welcome to Enaml
         ================
```

### Comparing `enaml-0.9.7/licenses/byteplay.txt` & `enaml-0.9.8/licenses/byteplay.txt`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/tools/vim/syntax/enaml.vim` & `enaml-0.9.8/tools/vim/syntax/enaml.vim`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/tools/emacs/enaml.el` & `enaml-0.9.8/tools/emacs/enaml.el`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/tools/sublimetext/Enaml.tmLanguage` & `enaml-0.9.8/tools/sublimetext/Enaml.tmLanguage`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/tools/sublimetext/Enaml.JSON-tmLanguage` & `enaml-0.9.8/tools/sublimetext/Enaml.JSON-tmLanguage`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/tools/pygments/build/lib/enamllexer/lexer.py` & `enaml-0.9.8/tools/pygments/enamllexer/lexer.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/tests/test_q_resource_helpers.py` & `enaml-0.9.8/tests/test_q_resource_helpers.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/tests/test_template.py` & `enaml-0.9.8/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/tests/test_stylesheet.py` & `enaml-0.9.8/tests/test_stylesheet.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/tests/test_alias.py` & `enaml-0.9.8/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/tests/utils.py` & `enaml-0.9.8/tests/utils.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/index.rst` & `enaml-0.9.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/api_ref/index.rst` & `enaml-0.9.8/docs/source/api_ref/index.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/api_ref/application.rst` & `enaml-0.9.8/docs/source/api_ref/application.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/api_ref/widgets/index.rst` & `enaml-0.9.8/docs/source/api_ref/widgets/index.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/api_ref/layout/dock_layout.rst` & `enaml-0.9.8/docs/source/api_ref/layout/dock_layout.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/dev_guides/code/pseudo_class_style.enaml` & `enaml-0.9.8/docs/source/dev_guides/code/pseudo_class_style.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/dev_guides/code/cascade_style.enaml` & `enaml-0.9.8/docs/source/dev_guides/code/cascade_style.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/dev_guides/code/pseudo_element_style.enaml` & `enaml-0.9.8/docs/source/dev_guides/code/pseudo_element_style.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/dev_guides/code/specificity_style.enaml` & `enaml-0.9.8/docs/source/dev_guides/code/specificity_style.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/dev_guides/code/selector_style.enaml` & `enaml-0.9.8/docs/source/dev_guides/code/selector_style.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/dev_guides/stylesheets.rst` & `enaml-0.9.8/docs/source/dev_guides/stylesheets.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/get_started/index.rst` & `enaml-0.9.8/docs/source/get_started/index.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/get_started/installation.rst` & `enaml-0.9.8/docs/source/get_started/installation.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/get_started/code/win_hierarchy.enaml` & `enaml-0.9.8/docs/source/get_started/code/win_hierarchy.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/get_started/anatomy.rst` & `enaml-0.9.8/docs/source/get_started/anatomy.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/get_started/introduction.rst` & `enaml-0.9.8/docs/source/get_started/introduction.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/images/simple_style.png` & `enaml-0.9.8/docs/source/images/simple_style.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/images/pseudo_class_style.png` & `enaml-0.9.8/docs/source/images/pseudo_class_style.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/images/specificity_style.png` & `enaml-0.9.8/docs/source/images/specificity_style.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/images/abs_hierarchy.png` & `enaml-0.9.8/docs/source/images/abs_hierarchy.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/images/pseudo_element_style.png` & `enaml-0.9.8/docs/source/images/pseudo_element_style.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/images/win_hierarchy.png` & `enaml-0.9.8/docs/source/images/win_hierarchy.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/images/selector_style.png` & `enaml-0.9.8/docs/source/images/selector_style.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/images/person_view.png` & `enaml-0.9.8/docs/source/images/person_view.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/images/cascade_style.png` & `enaml-0.9.8/docs/source/images/cascade_style.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/conf.py` & `enaml-0.9.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/index.rst` & `enaml-0.9.8/docs/source/examples/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -136,7 +136,15 @@
 
 Applib Examples
 --------------------------------------------------------------------------------
 
 .. toctree::
 
     ex_live_editor
+
+
+Workbench Examples
+--------------------------------------------------------------------------------
+
+.. toctree::
+
+    wb_sample
```

### Comparing `enaml-0.9.7/docs/source/examples/tut_person.rst` & `enaml-0.9.8/docs/source/examples/tut_person.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/tut_hello_world.rst` & `enaml-0.9.8/docs/source/examples/tut_hello_world.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/example_doc_generator.py` & `enaml-0.9.8/docs/source/examples/example_doc_generator.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/tut_employee.rst` & `enaml-0.9.8/docs/source/examples/tut_employee.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/img3.png` & `enaml-0.9.8/examples/widgets/images/img3.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/img2.png` & `enaml-0.9.8/examples/widgets/images/img2.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/tut_employee_layout_nested_container.png` & `enaml-0.9.8/docs/source/examples/images/tut_employee_layout_nested_container.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/tut_john_doe_error.png` & `enaml-0.9.8/docs/source/examples/images/tut_john_doe_error.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/tut_employee_layout.png` & `enaml-0.9.8/docs/source/examples/images/tut_employee_layout.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/tut_john_doe_jr.png` & `enaml-0.9.8/docs/source/examples/images/tut_john_doe_jr.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/tut_hello_world_python.png` & `enaml-0.9.8/docs/source/examples/images/tut_hello_world_python.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/tut_employee_layout_no_midline.png` & `enaml-0.9.8/docs/source/examples/images/tut_employee_layout_no_midline.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/tut_john_doe.png` & `enaml-0.9.8/docs/source/examples/images/tut_john_doe.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/img1.png` & `enaml-0.9.8/examples/widgets/images/img1.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/examples/images/tut_hello_world.png` & `enaml-0.9.8/docs/source/examples/images/tut_hello_world.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/docs/source/_sphinxext/enamldoc.py` & `enaml-0.9.8/docs/source/_sphinxext/enamldoc.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/setup.py` & `enaml-0.9.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             language='c++'
         )
     )
 
 
 setup(
     name='enaml',
-    version='0.9.7',
+    version='0.9.8',
     author='The Nucleic Development Team',
     author_email='sccolbert@gmail.com',
     url='https://github.com/nucleic/enaml',
     description='Declarative DSL for building rich user interfaces in Python',
     long_description=open('README.rst').read(),
     requires=['atom', 'PyQt', 'ply', 'kiwisolver'],
     install_requires=['distribute', 'atom >= 0.3.8', 'kiwisolver >= 0.1.2', 'ply >= 3.4'],
```

### Comparing `enaml-0.9.7/releasenotes.rst` & `enaml-0.9.8/releasenotes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Enaml Release Notes
 ===================
 
+0.9.8 - 08/04/2014
+------------------
+- Add drag and drop support. 56a2127e714c_
+- Remove the Wx backend and free the people from their misery. bab233ff9782_
+
+.. _56a2127e714c: https://github.com/nucleic/enaml/commit/56a2127e714cef2a22b65b00f2afd6b8024f36ec
+.. _bab233ff9782: https://github.com/nucleic/enaml/commit/bab233ff9782011185730f9dcaccd7113817a297
+
 0.9.7 - 05/18/2014
 ------------------
 - Add an IPythonConsole widget.
 - Add support for widgets in tool bars and menus.
 - Add a ToolButton widget.
 - Removed the 'focus_policy' attribute.
 - Removed the 'show_focus_rect' attribute.
```

### Comparing `enaml-0.9.7/README.rst` & `enaml-0.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/styling.py` & `enaml-0.9.8/enaml/styling.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/icon.py` & `enaml-0.9.8/enaml/icon.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/objectdict.py` & `enaml-0.9.8/enaml/objectdict.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/standard_tracer.py` & `enaml-0.9.8/enaml/core/standard_tracer.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/declarative_meta.py` & `enaml-0.9.8/enaml/core/declarative_meta.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/compiler_helpers.py` & `enaml-0.9.8/enaml/core/compiler_helpers.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/compiler_common.py` & `enaml-0.9.8/enaml/core/compiler_common.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/standard_inverter.py` & `enaml-0.9.8/enaml/core/standard_inverter.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/code_generator.py` & `enaml-0.9.8/enaml/core/code_generator.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/enaml_ast.py` & `enaml-0.9.8/enaml/core/enaml_ast.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/dynamic_template.py` & `enaml-0.9.8/enaml/core/dynamic_template.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/compiler_nodes.py` & `enaml-0.9.8/enaml/core/compiler_nodes.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/pattern.py` & `enaml-0.9.8/enaml/core/pattern.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/operators.py` & `enaml-0.9.8/enaml/core/operators.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/enaml_compiler.py` & `enaml-0.9.8/enaml/core/enaml_compiler.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/expression_engine.py` & `enaml-0.9.8/enaml/core/expression_engine.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/object.py` & `enaml-0.9.8/enaml/core/object.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/template_compiler.py` & `enaml-0.9.8/enaml/core/template_compiler.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/api.py` & `enaml-0.9.8/enaml/core/api.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/lexer.py` & `enaml-0.9.8/enaml/core/lexer.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/template_.py` & `enaml-0.9.8/enaml/core/template_.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/declarative_function.py` & `enaml-0.9.8/enaml/core/declarative_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     func : FunctionType
         The Python function to invoke.
 
     key : object
         The local scope key for the scope locals.
 
     self : Declarative
-        The declartive context 'self' object.
+        The declarative context 'self' object.
 
     args : tuple
         The positional arguments to pass to the function.
 
     kwargs : dict
         The keyword arguments to pass to the function.
```

### Comparing `enaml-0.9.7/enaml/core/looper.py` & `enaml-0.9.8/enaml/core/looper.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/block_compiler.py` & `enaml-0.9.8/enaml/core/block_compiler.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/standard_handlers.py` & `enaml-0.9.8/enaml/core/standard_handlers.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/conditional.py` & `enaml-0.9.8/enaml/core/conditional.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/import_hooks.py` & `enaml-0.9.8/enaml/core/import_hooks.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/enamldef_compiler.py` & `enaml-0.9.8/enaml/core/enamldef_compiler.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/parser.py` & `enaml-0.9.8/enaml/core/parser.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/enamldef_meta.py` & `enaml-0.9.8/enaml/core/enamldef_meta.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/parse_tab/parsetab.py` & `enaml-0.9.8/enaml/core/parse_tab/parsetab.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/parse_tab/lextab.py` & `enaml-0.9.8/enaml/core/parse_tab/lextab.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/code_tracing.py` & `enaml-0.9.8/enaml/core/code_tracing.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/declarative.py` & `enaml-0.9.8/enaml/core/declarative.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/template.py` & `enaml-0.9.8/enaml/core/template.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/byteplay.py` & `enaml-0.9.8/enaml/core/byteplay.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/core/include.py` & `enaml-0.9.8/enaml/core/include.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/runner.py` & `enaml-0.9.8/enaml/runner.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/colors.py` & `enaml-0.9.8/enaml/colors.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/action_group.py` & `enaml-0.9.8/enaml/widgets/action_group.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/color_dialog.py` & `enaml-0.9.8/enaml/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/combo_box.py` & `enaml-0.9.8/enaml/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/mdi_area.py` & `enaml-0.9.8/enaml/widgets/mdi_area.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/radio_button.py` & `enaml-0.9.8/enaml/widgets/radio_button.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/check_box.py` & `enaml-0.9.8/enaml/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/html.py` & `enaml-0.9.8/enaml/widgets/html.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/v_group.py` & `enaml-0.9.8/enaml/widgets/v_group.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/dock_area.py` & `enaml-0.9.8/enaml/widgets/dock_area.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/separator.py` & `enaml-0.9.8/enaml/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/flow_area.py` & `enaml-0.9.8/enaml/widgets/flow_area.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/menu_bar.py` & `enaml-0.9.8/enaml/widgets/menu_bar.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/datetime_selector.py` & `enaml-0.9.8/enaml/widgets/datetime_selector.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/tool_bar.py` & `enaml-0.9.8/enaml/widgets/tool_bar.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/multiline_field.py` & `enaml-0.9.8/enaml/widgets/multiline_field.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/status_bar.py` & `enaml-0.9.8/enaml/widgets/status_bar.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/dock_item.py` & `enaml-0.9.8/enaml/widgets/dock_item.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/timer.py` & `enaml-0.9.8/enaml/widgets/timer.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/file_dialog_ex.py` & `enaml-0.9.8/enaml/widgets/file_dialog_ex.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/container.py` & `enaml-0.9.8/enaml/widgets/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     #: A box object which holds the padding for this component. The
     #: padding is the amount of space between the outer boundary box
     #: and the content box. The default padding is 10 pixels a side.
     #: Certain subclasses, such as GroupBox, may provide additional
     #: margin than what is specified by the padding.
     padding = d_(Coerced(Box, (10, 10, 10, 10)))
 
-    #: A Container does not generate contraints for its size hint by
+    #: A Container does not generate constraints for its size hint by
     #: default. The minimum and maximum size constraints are sufficient
     #: to supply size limits and make for the most natural interaction
     #: between nested containers.
     resist_width = set_default('ignore')
     resist_height = set_default('ignore')
     hug_width = set_default('ignore')
     hug_height = set_default('ignore')
```

### Comparing `enaml-0.9.7/enaml/widgets/slider.py` & `enaml-0.9.8/enaml/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/form.py` & `enaml-0.9.8/enaml/widgets/form.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/dock_events.py` & `enaml-0.9.8/enaml/widgets/dock_events.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/tool_button.py` & `enaml-0.9.8/enaml/widgets/tool_button.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/stack.py` & `enaml-0.9.8/enaml/widgets/stack.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/dual_slider.py` & `enaml-0.9.8/enaml/widgets/dual_slider.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/raw_widget.py` & `enaml-0.9.8/enaml/widgets/raw_widget.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/file_dialog.py` & `enaml-0.9.8/enaml/widgets/file_dialog.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/dock_pane.py` & `enaml-0.9.8/enaml/widgets/dock_pane.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/abstract_button.py` & `enaml-0.9.8/enaml/widgets/abstract_button.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/web_view.py` & `enaml-0.9.8/enaml/widgets/web_view.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/popup_view.py` & `enaml-0.9.8/enaml/widgets/popup_view.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/api.py` & `enaml-0.9.8/enaml/widgets/api.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/bounded_time.py` & `enaml-0.9.8/enaml/widgets/bounded_time.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/spin_box.py` & `enaml-0.9.8/enaml/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/window.py` & `enaml-0.9.8/enaml/widgets/window.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/group_box.py` & `enaml-0.9.8/enaml/widgets/group_box.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/bounded_date.py` & `enaml-0.9.8/enaml/widgets/bounded_date.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/scroll_area.py` & `enaml-0.9.8/enaml/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/date_selector.py` & `enaml-0.9.8/enaml/widgets/date_selector.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/menu.py` & `enaml-0.9.8/enaml/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/mpl_canvas.py` & `enaml-0.9.8/enaml/widgets/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/frame.py` & `enaml-0.9.8/enaml/widgets/frame.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/mdi_window.py` & `enaml-0.9.8/enaml/widgets/mdi_window.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/calendar.py` & `enaml-0.9.8/enaml/widgets/calendar.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/dialog.py` & `enaml-0.9.8/enaml/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/widget.py` & `enaml-0.9.8/enaml/widgets/widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 from atom.api import (
-    Bool, Enum, IntEnum, Unicode, Coerced, Typed, ForwardTyped, observe
+    Bool, IntEnum, Unicode, Coerced, Typed, ForwardTyped, observe
 )
 
 from enaml.colors import ColorMember
 from enaml.core.declarative import d_, d_func
 from enaml.fonts import FontMember
 from enaml.layout.geometry import Size
 from enaml.styling import Stylable
@@ -83,14 +83,20 @@
     """
     #: Enables support for custom focus traversal functions.
     FocusTraversal = 0x1
 
     #: Enables support for focus events.
     FocusEvents = 0x2
 
+    #: Enables support for drag operations.
+    DragEnabled = 0x4
+
+    #: Enables support for drop operations.
+    DropEnabled = 0x8
+
 
 class Widget(ToolkitObject, Stylable):
     """ The base class of visible widgets in Enaml.
 
     """
     #: Whether or not the widget is enabled.
     enabled = d_(Bool(True))
@@ -129,15 +135,15 @@
     #: A reference to the ProxyWidget object.
     proxy = Typed(ProxyWidget)
 
     #--------------------------------------------------------------------------
     # Observers
     #--------------------------------------------------------------------------
     @observe('enabled', 'visible', 'background', 'foreground', 'font',
-        'minimum_size', 'maximum_size', 'tool_tip', 'status_tip')
+             'minimum_size', 'maximum_size', 'tool_tip', 'status_tip')
     def _update_proxy(self, change):
         """ Update the proxy widget when the Widget data changes.
 
         This method only updates the proxy when an attribute is updated;
         not when it is created or deleted.
 
         """
@@ -306,7 +312,117 @@
         """ A method invoked when the widget loses input focus.
 
         ** The FocusEvents feature must be enabled for the widget in
         order for this method to be called. **
 
         """
         pass
+
+    @d_func
+    def drag_start(self):
+        """ A method called at the start of a drag-drop operation.
+
+        This method is called when the user starts a drag operation
+        by dragging the widget with the left mouse button. It returns
+        the drag data for the drag operation.
+
+        ** The DragEnabled feature must be enabled for the widget in
+        order for this method to be called. **
+
+        Returns
+        -------
+        result : DragData
+            An Enaml DragData object which holds the drag data. If
+            this is not provided, no drag operation will occur.
+
+        """
+        return None
+
+    @d_func
+    def drag_end(self, drag_data, result):
+        """ A method called at the end of a drag-drop operation.
+
+        This method is called after the user has completed the drop
+        operation by releasing the left mouse button. It is passed
+        the original drag data object along with the resulting drop
+        action of the operation.
+
+        ** The DragEnabled feature must be enabled for the widget in
+        order for this method to be called. **
+
+        Parameters
+        ----------
+        data : DragData
+            The drag data created by the `drag_start` method.
+
+        result : DropAction
+            The requested drop action when the drop completed.
+
+        """
+        pass
+
+    @d_func
+    def drag_enter(self, event):
+        """ A method invoked when a drag operation enters the widget.
+
+        The widget should inspect the mime data of the event and
+        accept the event if it can handle the drop action. The event
+        must be accepted in order to receive further drag-drop events.
+
+        ** The DropEnabled feature must be enabled for the widget in
+        order for this method to be called. **
+
+        Parameters
+        ----------
+        event : DropEvent
+            The event representing the drag-drop operation.
+
+        """
+        pass
+
+    @d_func
+    def drag_move(self, event):
+        """ A method invoked when a drag operation moves in the widget.
+
+        This method will not normally be implemented, but it can be
+        useful for supporting advanced drag-drop interactions.
+
+        ** The DropEnabled feature must be enabled for the widget in
+        order for this method to be called. **
+
+        Parameters
+        ----------
+        event : DropEvent
+            The event representing the drag-drop operation.
+
+        """
+        pass
+
+    @d_func
+    def drag_leave(self):
+        """ A method invoked when a drag operation leaves the widget.
+
+        ** The DropEnabled feature must be enabled for the widget in
+        order for this method to be called. **
+
+        """
+        pass
+
+    @d_func
+    def drop(self, event):
+        """ A method invoked when the user drops the data on the widget.
+
+        The widget should either accept the proposed action, or set
+        the drop action to an appropriate action before accepting the
+        event, or set the drop action to DropAction.Ignore and then
+        ignore the event.
+
+        ** The DropEnabled feature must be enabled for the widget in
+        order for this method to be called. **
+
+        Parameters
+        ----------
+        event : DropEvent
+            The event representing the drag-drop operation.
+
+        """
+        pass
```

### Comparing `enaml-0.9.7/enaml/widgets/field.py` & `enaml-0.9.8/enaml/widgets/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     #: The validator to use for this field. If the validator provides
     #: a client side validator, then text will only be submitted if it
     #: passes that validator.
     validator = d_(Typed(Validator))
 
     #: The list of actions which should cause the client to submit its
     #: text to the server for validation and update. The currently
-    #: supported values are 'lost_focus', 'return_pressed', and 'auto'.
+    #: supported values are 'lost_focus', 'return_pressed', and 'auto_sync'.
     #: The 'auto_sync' mode will attempt to validate and synchronize the
     #: text when the user stops typing.
     submit_triggers = d_(List(
         Enum('lost_focus', 'return_pressed', 'auto_sync'),
         ['lost_focus', 'return_pressed']
     ))
```

### Comparing `enaml-0.9.7/enaml/widgets/page.py` & `enaml-0.9.8/enaml/widgets/page.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/split_item.py` & `enaml-0.9.8/enaml/widgets/split_item.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/ipython_console.py` & `enaml-0.9.8/enaml/widgets/ipython_console.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/focus_tracker.py` & `enaml-0.9.8/enaml/widgets/focus_tracker.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/push_button.py` & `enaml-0.9.8/enaml/widgets/push_button.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/bounded_datetime.py` & `enaml-0.9.8/enaml/widgets/bounded_datetime.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/notebook.py` & `enaml-0.9.8/enaml/widgets/notebook.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/splitter.py` & `enaml-0.9.8/enaml/widgets/splitter.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/main_window.py` & `enaml-0.9.8/enaml/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/vtk_canvas.py` & `enaml-0.9.8/enaml/widgets/vtk_canvas.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/object_combo.py` & `enaml-0.9.8/enaml/widgets/object_combo.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/stack_item.py` & `enaml-0.9.8/enaml/widgets/stack_item.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/toolkit_dialog.py` & `enaml-0.9.8/enaml/widgets/toolkit_dialog.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/constraints_widget.py` & `enaml-0.9.8/enaml/widgets/constraints_widget.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/control.py` & `enaml-0.9.8/enaml/widgets/control.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/flow_item.py` & `enaml-0.9.8/enaml/widgets/flow_item.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/toolkit_object.py` & `enaml-0.9.8/enaml/widgets/toolkit_object.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/image_view.py` & `enaml-0.9.8/enaml/widgets/image_view.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/label.py` & `enaml-0.9.8/enaml/widgets/label.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/status_item.py` & `enaml-0.9.8/enaml/widgets/status_item.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/action.py` & `enaml-0.9.8/enaml/widgets/action.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/time_selector.py` & `enaml-0.9.8/enaml/widgets/time_selector.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/progress_bar.py` & `enaml-0.9.8/enaml/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/widgets/h_group.py` & `enaml-0.9.8/enaml/widgets/h_group.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/version.py` & `enaml-0.9.8/enaml/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # possibly small differences in the API, but these changes will come
 # backwards compatibility support when possible. Minor releases are
 # typically used for large feature additions.
 MINOR = 9
 
 # The micro release number. The micro release number is incremented
 # for bug fix releases and small feature additions.
-MICRO = 7
+MICRO = 8
 
 #: A namedtuple of the version info for the current release.
 version_info = namedtuple('version_info', 'major minor micro')
 version_info = version_info(MAJOR, MINOR, MICRO)
 
 # Remove everything but the 'version_info' from this module.
 del namedtuple, MAJOR, MINOR, MICRO
```

### Comparing `enaml-0.9.7/enaml/image.py` & `enaml-0.9.8/enaml/image.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/application.py` & `enaml-0.9.8/enaml/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2013, Nucleic Development Team.
+# Copyright (c) 2014, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 from heapq import heappush, heappop
 from itertools import count
@@ -304,14 +304,25 @@
         -------
         result : bool
             True if called from the main gui thread. False otherwise.
 
         """
         raise NotImplementedError
 
+    def create_mime_data(self):
+        """ Create a new mime data object to be filled by the user.
+
+        Returns
+        -------
+        result : MimeData
+            A concrete implementation of the MimeData class.
+
+        """
+        raise NotImplementedError
+
     #--------------------------------------------------------------------------
     # Public API
     #--------------------------------------------------------------------------
     def resolve_proxy_class(self, declaration_class):
         """ Resolve the proxy implementation class for a declaration.
 
         This can be reimplemented by Application subclasses if more
```

### Comparing `enaml-0.9.7/enaml/fonts.py` & `enaml-0.9.8/enaml/fonts.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/callableref.cpp` & `enaml-0.9.8/enaml/src/callableref.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/signaling.cpp` & `enaml-0.9.8/enaml/src/signaling.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/alias.cpp` & `enaml-0.9.8/enaml/src/alias.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/winutil.cpp` & `enaml-0.9.8/enaml/src/winutil.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/colorext.cpp` & `enaml-0.9.8/enaml/src/colorext.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/inttypes.h` & `enaml-0.9.8/enaml/src/inttypes.h`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/dynamicscope.cpp` & `enaml-0.9.8/enaml/src/dynamicscope.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/pythonhelpers.h` & `enaml-0.9.8/enaml/src/pythonhelpers.h`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/funchelper.cpp` & `enaml-0.9.8/enaml/src/funchelper.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/declfunction.cpp` & `enaml-0.9.8/enaml/src/declfunction.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/fontext.cpp` & `enaml-0.9.8/enaml/src/fontext.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/weakmethod.cpp` & `enaml-0.9.8/enaml/src/weakmethod.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/pythonhelpersex.h` & `enaml-0.9.8/enaml/src/pythonhelpersex.h`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/src/compiler_helpers.cpp` & `enaml-0.9.8/enaml/src/compiler_helpers.cpp`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/scintilla/idle_theme.py` & `enaml-0.9.8/enaml/scintilla/idle_theme.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/scintilla/mono_font.py` & `enaml-0.9.8/enaml/scintilla/mono_font.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/scintilla/scintilla.py` & `enaml-0.9.8/enaml/scintilla/scintilla.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/__init__.py` & `enaml-0.9.8/enaml/__init__.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/stdlib/task_dialog.enaml` & `enaml-0.9.8/enaml/stdlib/task_dialog.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/stdlib/slider_transform.py` & `enaml-0.9.8/enaml/stdlib/slider_transform.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/stdlib/dialog_buttons.enaml` & `enaml-0.9.8/enaml/stdlib/dialog_buttons.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/stdlib/dock_area_styles.enaml` & `enaml-0.9.8/enaml/stdlib/dock_area_styles.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/stdlib/mapped_view.enaml` & `enaml-0.9.8/enaml/stdlib/mapped_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/stdlib/message_box.enaml` & `enaml-0.9.8/enaml/stdlib/message_box.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/stdlib/fields.enaml` & `enaml-0.9.8/enaml/stdlib/fields.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/validator.py` & `enaml-0.9.8/enaml/validator.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/extension_point.py` & `enaml-0.9.8/enaml/workbench/extension_point.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/plugin_manifest.py` & `enaml-0.9.8/enaml/workbench/plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/core/execution_event.py` & `enaml-0.9.8/enaml/workbench/core/execution_event.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/core/command.py` & `enaml-0.9.8/enaml/workbench/core/command.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/core/core_plugin.py` & `enaml-0.9.8/enaml/workbench/core/core_plugin.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/core/core_manifest.enaml` & `enaml-0.9.8/enaml/workbench/core/core_manifest.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/plugin.py` & `enaml-0.9.8/enaml/workbench/plugin.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/api.py` & `enaml-0.9.8/enaml/workbench/api.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/extension.py` & `enaml-0.9.8/enaml/workbench/extension.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/workbench.py` & `enaml-0.9.8/enaml/workbench/workbench.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/workspace.py` & `enaml-0.9.8/enaml/workbench/ui/workspace.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/branding.py` & `enaml-0.9.8/enaml/workbench/ui/branding.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/workbench_window.enaml` & `enaml-0.9.8/enaml/workbench/ui/workbench_window.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/ui_workbench.py` & `enaml-0.9.8/enaml/workbench/ui/ui_workbench.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/workbench_menus.enaml` & `enaml-0.9.8/enaml/workbench/ui/workbench_menus.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/ui_plugin.py` & `enaml-0.9.8/enaml/workbench/ui/ui_plugin.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/autostart.py` & `enaml-0.9.8/enaml/workbench/ui/autostart.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/api.py` & `enaml-0.9.8/enaml/workbench/ui/api.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/item_group.py` & `enaml-0.9.8/enaml/workbench/ui/item_group.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/menu_item.py` & `enaml-0.9.8/enaml/workbench/ui/menu_item.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/menu_helper.py` & `enaml-0.9.8/enaml/workbench/ui/menu_helper.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/action_item.py` & `enaml-0.9.8/enaml/workbench/ui/action_item.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/window_model.py` & `enaml-0.9.8/enaml/workbench/ui/window_model.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/workbench/ui/ui_manifest.enaml` & `enaml-0.9.8/enaml/workbench/ui/ui_manifest.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/applib/live_editor_view.enaml` & `enaml-0.9.8/enaml/applib/live_editor_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/applib/live_editor_model.py` & `enaml-0.9.8/enaml/applib/live_editor_model.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/factory_helper.py` & `enaml-0.9.8/enaml/layout/factory_helper.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/dock_layout.py` & `enaml-0.9.8/enaml/layout/dock_layout.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/layout_helpers.py` & `enaml-0.9.8/enaml/layout/layout_helpers.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/geometry.py` & `enaml-0.9.8/enaml/layout/geometry.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/constraint_helper.py` & `enaml-0.9.8/enaml/layout/constraint_helper.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/constrainable.py` & `enaml-0.9.8/enaml/layout/constrainable.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/linear_box_helper.py` & `enaml-0.9.8/enaml/layout/linear_box_helper.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/layout_manager.py` & `enaml-0.9.8/enaml/layout/layout_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         This abstract method must be implemented by subclasses.
 
         Returns
         -------
         result : Contrainable or ContentsContrainable
             An object which implements the Constrainable interface.
             If the 'margins' method returns a non-empty tuple, then
-            the object must also implement the ContentsContrainable
+            the object must also implement the ContentsConstrainable
             interface.
 
         """
         raise NotImplementedError
 
     def constraints(self):
         """ Get the user-defined constraints for the item.
```

### Comparing `enaml-0.9.7/enaml/layout/api.py` & `enaml-0.9.8/enaml/layout/api.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/grid_helper.py` & `enaml-0.9.8/enaml/layout/grid_helper.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/sequence_helper.py` & `enaml-0.9.8/enaml/layout/sequence_helper.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/spacers.py` & `enaml-0.9.8/enaml/layout/spacers.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/linear_symbolic.py` & `enaml-0.9.8/enaml/layout/linear_symbolic.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/box_helper.py` & `enaml-0.9.8/enaml/layout/box_helper.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/layout/strength_member.py` & `enaml-0.9.8/enaml/layout/strength_member.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/nodevisitor.py` & `enaml-0.9.8/enaml/nodevisitor.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/wx/wx_page.py` & `enaml-0.9.8/enaml/qt/qt_page.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,318 +1,377 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-import wx.lib.newevent
-
 from atom.api import Typed
 
 from enaml.widgets.page import ProxyPage
 
-from .wx_container import WxContainer
-from .wx_widget import WxWidget
-from .wx_single_widget_sizer import wxSingleWidgetSizer
-
+from .QtCore import Signal
+from .QtGui import QFrame, QIcon
 
-#: An event emitted when the notebook page is closed.
-wxPageClosedEvent, EVT_PAGE_CLOSED = wx.lib.newevent.NewEvent()
+from .q_resource_helpers import get_cached_qicon
+from .q_single_widget_layout import QSingleWidgetLayout
+from .qt_container import QtContainer
+from .qt_widget import QtWidget
 
 
-class wxPage(wx.Panel):
-    """ A wxPanel subclass which acts as a page in a wx notebook.
+class QPage(QFrame):
+    """ A QFrame subclass which acts as a page in a QNotebook.
 
     """
+    #: A signal emitted when the page has been closed by the user.
+    pageClosed = Signal()
+
     def __init__(self, *args, **kwargs):
-        """ Initialize a wxPage.
+        """ Initialize a QPage.
 
         Parameters
         ----------
         *args, **kwargs
             The position and keyword arguments required to initialize
-            a wxContainer.
+            a QWidget.
 
         """
-        super(wxPage, self).__init__(*args, **kwargs)
+        super(QPage, self).__init__(*args, **kwargs)
         self._title = u''
+        self._tool_tip = u''
+        self._icon = QIcon()
         self._closable = True
         self._is_enabled = True
         self._is_open = True
         self._page_widget = None
-        self.SetSizer(wxSingleWidgetSizer())
-        self.Bind(wx.EVT_SHOW, self.OnShow)
+        self.setLayout(QSingleWidgetLayout())
 
     #--------------------------------------------------------------------------
-    # Event Handlers
+    # Private API
     #--------------------------------------------------------------------------
-    def OnClose(self, event):
-        """ Handle the page close event.
-
-        This event handler is called by the parent notebook. The parent
-        event is always be vetoed or else Wx will destroy the page. If
-        the page is closable, we close the page and emit the custom
-        close event.
-
-        """
-        event.Veto()
-        if self.GetClosable():
-            self.Close()
-            evt = wxPageClosedEvent()
-            wx.PostEvent(self, evt)
+    def _findNotebook(self):
+        """ Get the parent QNotebook for this page.
 
-    def OnShow(self, event):
-        """ Handle the show event.
-
-        Wx will not emit an EVT_SHOW on the child of this page. So, this
-        event handler passes the show event along to the contained page
-        widget, so that it can disable its layout when not visible.
-
-        """
-        page = self._page_widget
-        if page:
-            wx.PostEvent(page, event)
+        Returns
+        -------
+        result : QNotebook or None
+            The parent QNotebook for this page, or None if one cannot
+            be found.
+
+        """
+        # Avoid a circular import with the qt_notebook module
+        from .qt_notebook import QNotebook
+        # Depending on where we are during initialization, the notebook
+        # will be either our parent or grandparent because of how the
+        # QTabWidget reparents things internally.
+        parent = self.parent()
+        if isinstance(parent, QNotebook):
+            return parent
+        if parent is not None:
+            parent = parent.parent()
+            if isinstance(parent, QNotebook):
+                return parent
 
-    #--------------------------------------------------------------------------
-    # Private API
-    #--------------------------------------------------------------------------
-    def _PageIndexOperation(self, closure):
+    def _pageIndexOperation(self, closure):
         """ A private method which will run the given closure if there
         is a valid index for this page.
 
         """
-        parent = self.GetParent()
-        if parent:
-            index = parent.GetPageIndex(self)
+        notebook = self._findNotebook()
+        if notebook is not None:
+            index = notebook.indexOf(self)
             if index != -1:
-                closure(parent, index)
+                closure(notebook, index)
 
     #--------------------------------------------------------------------------
     # Public API
     #--------------------------------------------------------------------------
-    def GetPageWidget(self):
+    def requestClose(self):
+        """ A method called by the parent notebook when the user has
+        requested that this page be closed.
+
+        If the page is marked as closable, then it will be closed and
+        the 'pageClosed' signal will be emitted.
+
+        """
+        if self.isClosable():
+            self.close()
+            self.pageClosed.emit()
+
+    def pageWidget(self):
         """ Get the page widget for this page.
 
         Returns
         -------
-        result : wxWindow or None
+        result : QWidget or None
             The page widget being managed by this page.
 
         """
         return self._page_widget
 
-    def SetPageWidget(self, widget):
+    def setPageWidget(self, widget):
         """ Set the page widget for this page.
 
         Parameters
         ----------
-        widget : wxWindow
-            The wx widget to use as the page widget in this page.
+        widget : QWudget
+            The Qt widget to use as the page widget in this page.
 
         """
         self._page_widget = widget
-        self.GetSizer().Add(widget)
+        self.layout().setWidget(widget)
 
-    def IsOpen(self):
+    def isOpen(self):
         """ Get whether or not the page is open.
 
         Returns
         -------
         result : bool
             True if the page is open, False otherwise.
 
         """
         return self._is_open
 
-    def Open(self):
-        """ Open the page in the notebook.
+    def show(self):
+        """ Show the page in the notebook.
 
         """
         self._is_open = True
-        parent = self.GetParent()
-        if parent:
-            parent.ShowWxPage(self)
+        notebook = self._findNotebook()
+        if notebook is not None:
+            notebook.showPage(self)
 
-    def Close(self):
-        """ Close the page in the notebook.
+    def hide(self):
+        """ Hide the page in the notebook.
 
         """
         self._is_open = False
-        parent = self.GetParent()
-        if parent:
-            parent.HideWxPage(self)
+        notebook = self._findNotebook()
+        if notebook is not None:
+            notebook.hidePage(self)
 
-    def GetEnabled(self):
-        """ Get the enabled state of the page.
+    def isTabEnabled(self):
+        """ Return whether or not the tab for this page is enabled.
 
-        This method should be used in favor of IsEnabled.
+        This method should be used in favor of isEnabled.
 
         Returns
         -------
         result : bool
-            True the page is enabled, False otherwise.
+            True if the tab for this page is enabled, False otherwise.
 
         """
         return self._is_enabled
 
-    def SetEnabled(self, enabled):
-        """ Set the enabled state of the page.
+    def setTabEnabled(self, enabled):
+        """ Set whether the tab for this page is enabled.
 
-        This method should be used in favor of Enable.
+        This method should be used in favor of isEnabled.
 
         Parameters
-        ---------
+        ----------
         enabled : bool
-            Whether or not the page should be enabled.
+            True if the tab should be enabled, False otherwise.
 
         """
         self._is_enabled = enabled
         def closure(nb, index):
-            nb.EnableTab(index, enabled)
-        self._PageIndexOperation(closure)
+            nb.setTabEnabled(index, enabled)
+        self._pageIndexOperation(closure)
 
-    def GetTitle(self):
-        """ Returns tab title for this page.
+    def title(self):
+        """ Returns the tab title for this page.
 
         Returns
         -------
         result : unicode
             The title string for the page's tab.
 
         """
         return self._title
 
-    def SetTitle(self, title):
-        """ Set the title for this page.
+    def setTitle(self, title):
+        """ Set the title for the tab for this page.
 
         Parameters
         ----------
         title : unicode
             The string to use for this page's tab title.
 
         """
         self._title = title
         def closure(nb, index):
-            nb.SetPageText(index, title)
-        self._PageIndexOperation(closure)
+            nb.setTabText(index, title)
+        self._pageIndexOperation(closure)
 
-    def GetClosable(self):
-        """ Returns whether or not this page is closable.
+    def isClosable(self):
+        """ Returns whether or not the tab for this page is closable.
 
         Returns
         -------
         result : bool
-            True if this page is closable, False otherwise.
+            True if this page's tab is closable, False otherwise.
 
         """
         return self._closable
 
-    def SetClosable(self, closable):
-        """ Set whether this page is closable.
+    def setClosable(self, closable):
+        """ Set whether the tab for this page is closable.
 
         Parameters
         ----------
         closable : bool
-            True if this page should be closable, False otherwise.
+            True if the tab should be closable, False otherwise.
 
         """
         self._closable = closable
         def closure(nb, index):
-            nb.SetCloseButton(index, closable)
-        self._PageIndexOperation(closure)
+            nb.setTabCloseButtonVisible(index, closable)
+        self._pageIndexOperation(closure)
 
+    def toolTip(self):
+        """ Returns the tool tip for the tab for this page.
+
+        Returns
+        -------
+        result : unicode
+            The tool tip string for the page's tab.
+
+        """
+        return self._tool_tip
 
-class WxPage(WxWidget, ProxyPage):
-    """ A Wx implementation of an Enaml notebook ProxyPage.
+    def setToolTip(self, tool_tip):
+        """ Set the tool tip for the tab for this page.
+
+        This overrides the default implementation to set the tool tip
+        on the notebook tab.
+
+        Parameters
+        ----------
+        title : unicode
+            The string to use for this page's tab tool tip.
+
+        """
+        self._tool_tip = tool_tip
+        def closure(nb, index):
+            nb.setTabToolTip(index, tool_tip)
+        self._pageIndexOperation(closure)
+
+    def icon(self):
+        """ Get the icon for the page.
+
+        Returns
+        -------
+        result : QIcon
+            The icon for the page.
+
+        """
+        return self._icon
+
+    def setIcon(self, icon):
+        """ Set the icon for the page.
+
+        Parameters
+        ----------
+        icon : QIcon
+            The icon for the page.
+
+        """
+        self._icon = icon
+        def closure(nb, index):
+            nb.setTabIcon(index, icon)
+        self._pageIndexOperation(closure)
+
+
+class QtPage(QtWidget, ProxyPage):
+    """ A Qt implementation of an Enaml ProxyPage.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(wxPage)
+    widget = Typed(QPage)
 
     #--------------------------------------------------------------------------
-    # Setup Methods
+    # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying wxPage widget.
+        """ Create the underlying page widget.
 
         """
-        self.widget = wxPage(self.parent_widget())
+        self.widget = QPage(self.parent_widget())
 
     def init_widget(self):
-        """ Create and initialize the page control.
+        """ Initialize the underlying widget.
 
         """
-        super(WxPage, self).init_widget()
+        super(QtPage, self).init_widget()
         d = self.declaration
         self.set_title(d.title)
         self.set_closable(d.closable)
         if d.icon:
             self.set_icon(d.icon)
-        self.widget.Bind(EVT_PAGE_CLOSED, self.on_page_closed)
+        self.widget.pageClosed.connect(self.on_page_closed)
 
     def init_layout(self):
-        """ Initialize the layout of the notebook page.
+        """ Initialize the layout for the underyling widget.
 
         """
-        super(WxPage, self).init_layout()
-        self.widget.SetPageWidget(self.page_widget())
+        super(QtPage, self).init_layout()
+        self.widget.setPageWidget(self.page_widget())
 
     #--------------------------------------------------------------------------
     # Utility Methods
     #--------------------------------------------------------------------------
     def page_widget(self):
         """ Find and return the page widget child for this widget.
 
         """
         p = self.declaration.page_widget()
         if p is not None:
-            return p.proxy.widget or None
+            return p.proxy.widget
 
     #--------------------------------------------------------------------------
     # Child Events
     #--------------------------------------------------------------------------
     def child_added(self, child):
-        """ Handle the child added event for a WxPage.
+        """ Handle the child added event for a QtPage.
 
         """
-        super(WxPage, self).child_removed(child)
-        if isinstance(child, WxContainer):
-            self.widget.SetPageWidget(self.page_widget())
+        super(QtPage, self).child_removed(child)
+        if isinstance(child, QtContainer):
+            self.widget.setPageWidget(self.page_widget())
 
     def child_removed(self, child):
-        """ Handle the child removed event for a WxPage.
+        """ Handle the child removed event for a QtPage.
 
         """
-        super(WxPage, self).child_removed(child)
-        if isinstance(child, WxContainer):
-            self.widget.SetPageWidget(self.page_widget())
+        super(QtPage, self).child_removed(child)
+        if isinstance(child, QtContainer):
+            self.widget.setPageWidget(self.page_widget())
 
     #--------------------------------------------------------------------------
-    # Event Handlers
+    # Signal Handlers
     #--------------------------------------------------------------------------
-    def on_page_closed(self, event):
-        """ The event handler for the EVT_PAGE_CLOSED event.
+    def on_page_closed(self):
+        """ The signal handler for the 'pageClosed' signal.
 
         """
         self.declaration._handle_close()
 
     #--------------------------------------------------------------------------
     # ProxyPage API
     #--------------------------------------------------------------------------
     def set_visible(self, visible):
         """ An overridden visibility setter which to opens|closes the
         notebook page.
 
         """
         if visible:
-            self.widget.Open()
+            self.widget.show()
         else:
-            self.widget.Close()
+            self.widget.hide()
 
     def ensure_visible(self):
         """ An overridden visibility setter which to opens|closes the
         notebook page.
 
         """
         self.set_visible(True)
@@ -325,28 +384,30 @@
         self.set_visible(False)
 
     def set_enabled(self, enabled):
         """ An overridden enabled setter which sets the tab enabled
         state.
 
         """
-        self.widget.SetEnabled(enabled)
+        self.widget.setTabEnabled(enabled)
 
     def set_title(self, title):
         """ Set the title of the tab for this page.
 
         """
-        self.widget.SetTitle(title)
+        self.widget.setTitle(title)
 
     def set_icon(self, icon):
         """ Sets the widget's icon to the provided image.
 
-        This is not supported on Wx.
-
         """
-        pass
+        if icon:
+            qicon = get_cached_qicon(icon)
+        else:
+            qicon = QIcon()
+        self.widget.setIcon(qicon)
 
     def set_closable(self, closable):
         """ Set whether or not this page is closable.
 
         """
-        self.widget.SetClosable(closable)
+        self.widget.setClosable(closable)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_html.py` & `enaml-0.9.8/enaml/qt/qt_calendar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,89 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx.html
-
 from atom.api import Typed
 
-from enaml.widgets.html import ProxyHtml
-
-from .wx_control import WxControl
-
-
-class wxProperHtmlWindow(wx.html.HtmlWindow):
-    """ A custom wx Html window that returns a non-braindead best size.
-
-    """
-    _best_size = wx.Size(256, 192)
+from enaml.widgets.calendar import ProxyCalendar
 
-    def GetBestSize(self):
-        """ Returns the best size for the html window.
+from .QtGui import QCalendarWidget
 
-        """
-        return self._best_size
+from .qt_bounded_date import QtBoundedDate, CHANGED_GUARD
 
 
-class WxHtml(WxControl, ProxyHtml):
-    """ A Wx implementation of the Enaml ProxyHtml widget.
+class QtCalendar(QtBoundedDate, ProxyCalendar):
+    """ A Qt implementation of an Enaml ProxyCalendar.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(wxProperHtmlWindow)
+    widget = Typed(QCalendarWidget)
 
     #--------------------------------------------------------------------------
-    # Setup Methods
+    # Initialization
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying html widget.
+        """ Create the calender widget.
 
         """
-        self.widget = wxProperHtmlWindow(self.parent_widget())
+        self.widget = QCalendarWidget(self.parent_widget())
 
     def init_widget(self):
-        """ Initialize the underlying widget.
+        """ Initialize the widget.
 
         """
-        super(WxHtml, self).init_widget()
-        self.set_source(self.declaration.source)
+        super(QtCalendar, self).init_widget()
+        self.widget.activated.connect(self.on_date_changed)
 
     #--------------------------------------------------------------------------
-    # ProxyHtml API
+    # Abstract API Implementation
     #--------------------------------------------------------------------------
-    def set_source(self, source):
-        """ Set the source of the html widget
+    def get_date(self):
+        """ Return the current date in the control.
+
+        Returns
+        -------
+        result : date
+            The current control date as a Python date object.
+
+        """
+        return self.widget.selectedDate().toPython()
+
+    def set_minimum(self, date):
+        """ Set the widget's minimum date.
+
+        Parameters
+        ----------
+        date : date
+            The date object to use for setting the minimum date.
+
+        """
+        self.widget.setMinimumDate(date)
+
+    def set_maximum(self, date):
+        """ Set the widget's maximum date.
+
+        Parameters
+        ----------
+        date : date
+            The date object to use for setting the maximum date.
+
+        """
+        self.widget.setMaximumDate(date)
+
+    def set_date(self, date):
+        """ Set the widget's current date.
+
+        Parameters
+        ----------
+        date : date
+            The date object to use for setting the date.
 
         """
-        self.widget.SetPage(source)
+        self._guard |= CHANGED_GUARD
+        try:
+            self.widget.setSelectedDate(date)
+        finally:
+            self._guard &= ~CHANGED_GUARD
```

### Comparing `enaml-0.9.7/enaml/wx/wx_toolkit_object.py` & `enaml-0.9.8/enaml/qt/qt_date_selector.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,116 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-
 from atom.api import Typed
 
-from enaml.widgets.toolkit_object import ProxyToolkitObject
+from enaml.widgets.date_selector import ProxyDateSelector
+
+from .QtGui import QDateEdit
+
+from .qt_bounded_date import QtBoundedDate, CHANGED_GUARD
 
 
-class WxToolkitObject(ProxyToolkitObject):
-    """ A Wx implementation of an Enaml ProxyToolkitObject.
+class QtDateSelector(QtBoundedDate, ProxyDateSelector):
+    """ A Qt implementation of an Enaml ProxyDateSelector.
 
     """
-    #: A reference to the toolkit widget created by the proxy.
-    widget = Typed(wx.Object)
+    #: A reference to the widget created by the proxy.
+    widget = Typed(QDateEdit)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the toolkit widget for the proxy object.
-
-        This method is called during the top-down pass, just before the
-        'init_widget()' method is called. This method should create the
-        toolkit widget and assign it to the 'widget' attribute.
+        """ Create the QDateEdit widget.
 
         """
-        self.widget = wx.Object()
+        self.widget = QDateEdit(self.parent_widget())
 
     def init_widget(self):
-        """ Initialize the state of the toolkit widget.
-
-        This method is called during the top-down pass, just after the
-        'create_widget()' method is called. This method should init the
-        state of the widget. The child widgets will not yet be created.
+        """ Initialize the widget.
 
         """
-        pass
+        super(QtDateSelector, self).init_widget()
+        d = self.declaration
+        self.set_date_format(d.date_format)
+        self.set_calendar_popup(d.calendar_popup)
+        self.widget.dateChanged.connect(self.on_date_changed)
 
-    def init_layout(self):
-        """ Initialize the layout of the toolkit widget.
+    #--------------------------------------------------------------------------
+    # Abstract API Implementation
+    #--------------------------------------------------------------------------
+    def get_date(self):
+        """ Return the current date in the control.
 
-        This method is called during the bottom-up pass. This method
-        should initialize the layout of the widget. The child widgets
-        will be fully initialized and layed out when this is called.
+        Returns
+        -------
+        result : date
+            The current control date as a date object.
 
         """
-        pass
+        return self.widget.date().toPython()
 
-    #--------------------------------------------------------------------------
-    # ProxyToolkitObject API
-    #--------------------------------------------------------------------------
-    def activate_top_down(self):
-        """ Activate the proxy tree for the top-down pass.
+    def set_minimum(self, date):
+        """ Set the widget's minimum date.
+
+        Parameters
+        ----------
+        date : date
+            The date object to use for setting the minimum date.
 
         """
-        self.create_widget()
-        self.init_widget()
+        self.widget.setMinimumDate(date)
+
+    def set_maximum(self, date):
+        """ Set the widget's maximum date.
 
-    def activate_bottom_up(self):
-        """ Activate the proxy tree for the bottom-up pass.
+        Parameters
+        ----------
+        date : date
+            The date object to use for setting the maximum date.
 
         """
-        self.init_layout()
+        self.widget.setMaximumDate(date)
 
-    def destroy(self):
-        """ A reimplemented destructor.
+    def set_date(self, date):
+        """ Set the widget's current date.
 
-        This destructor will drop the reference to the toolkit widget.
+        Parameters
+        ----------
+        date : date
+            The date object to use for setting the date.
 
         """
-        if self.widget:
-            try:
-                self.widget.Destroy()
-            except AttributeError:
-                pass
-            del self.widget
-        super(WxToolkitObject, self).destroy()
+        self._guard |= CHANGED_GUARD
+        try:
+            self.widget.setDate(date)
+        finally:
+            self._guard &= ~CHANGED_GUARD
 
-    #--------------------------------------------------------------------------
-    # Public API
-    #--------------------------------------------------------------------------
-    def parent_widget(self):
-        """ Get the parent toolkit widget for this object.
+    def set_date_format(self, format):
+        """ Set the widget's date format.
 
-        Returns
-        -------
-        result : wxObject or None
-            The toolkit widget declared on the declaration parent, or
-            None if there is no such parent.
+        Parameters
+        ----------
+        format : string
+            A Python time formatting string.
 
         """
-        parent = self.parent()
-        if parent is not None:
-            if parent.widget:
-                return parent.widget
+        # XXX make sure Python's and Qt's format strings are the
+        # same, or convert between the two.
+        self.widget.setDisplayFormat(format)
 
-    def child_widgets(self):
-        """ Get the child toolkit widgets for this object.
+    def set_calendar_popup(self, popup):
+        """ Set whether a calendar popup is available on the widget.
 
-        Returns
-        -------
-        result : iterable of wxObject
-            The child widgets defined for this object.
+        Parameters
+        ----------
+        popup : bool
+            Whether the calendar popup is enabled.
 
         """
-        for child in self.children():
-            if child.widget:
-                yield child.widget
+        self.widget.setCalendarPopup(popup)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_label.py` & `enaml-0.9.8/enaml/qt/qt_bounded_time.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,100 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
+from atom.api import Int
 
-from atom.api import Typed
+from enaml.widgets.bounded_time import ProxyBoundedTime
 
-from enaml.widgets.label import ProxyLabel
+from .qt_control import QtControl
 
-from .wx_control import WxControl
 
+# cyclic notification guard flags
+CHANGED_GUARD = 0x1
 
-ALIGN_MAP = {
-    'left': wx.ALIGN_LEFT,
-    'right': wx.ALIGN_RIGHT,
-    'center': wx.ALIGN_CENTER,
-    'justify': wx.ALIGN_LEFT,  # wx doesn't support justification
-}
 
-
-ALIGN_MASK = wx.ALIGN_LEFT | wx.ALIGN_RIGHT | wx.ALIGN_CENTER
-
-
-class WxLabel(WxControl, ProxyLabel):
-    """ A Wx implementation of an Enaml ProxyLabel.
+class QtBoundedTime(QtControl, ProxyBoundedTime):
+    """ A base class for implementing Qt-Enaml time widgets.
 
     """
-     #: A reference to the widget created by the proxy.
-    widget = Typed(wx.StaticText)
+    #: Cyclic notification guard. This a bitfield of multiple guards.
+    _guard = Int(0)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying label widget.
+        """ Implement in a subclass to create the time widget.
 
         """
-        self.widget = wx.StaticText(self.parent_widget())
+        raise NotImplementedError
 
     def init_widget(self):
-        """ Initialize the underlying widget.
+        """ Create and initialize the underlying time widget.
 
         """
-        super(WxLabel, self).init_widget()
+        super(QtBoundedTime, self).init_widget()
         d = self.declaration
-        self.set_text(d.text)
-        self.set_align(d.align)
-        self.set_vertical_align(d.vertical_align)
+        self.set_minimum(d.minimum)
+        self.set_maximum(d.maximum)
+        self.set_time(d.time)
+
+    #--------------------------------------------------------------------------
+    # Signal Handlers
+    #--------------------------------------------------------------------------
+    def on_time_changed(self):
+        """ A signal handler for the time changed signal.
+
+        """
+        if not self._guard & CHANGED_GUARD:
+            self.declaration.time = self.get_time()
 
     #--------------------------------------------------------------------------
-    # ProxyLabel API
+    # Abstract Methods and ProxyBoundedDate API
     #--------------------------------------------------------------------------
-    def set_text(self, text):
-        """ Set the text in the underlying widget.
+    def get_time(self):
+        """ Return the current time in the control.
+
+        Returns
+        -------
+        result : time
+            The current control time as a time object.
 
         """
-        with self.geometry_guard():
-            self.widget.SetLabel(text)
+        raise NotImplementedError
+
+    def set_minimum(self, time):
+        """ Set the widget's minimum time.
+
+        Parameters
+        ----------
+        time : time
+            The time object to use for setting the minimum time.
+
+        """
+        raise NotImplementedError
+
+    def set_maximum(self, time):
+        """ Set the widget's maximum time.
 
-    def set_align(self, align):
-        """ Set the alignment of the text in the underlying widget.
+        Parameters
+        ----------
+        time : time
+            The time object to use for setting the maximum time.
 
         """
-        widget = self.widget
-        style = widget.GetWindowStyle()
-        style &= ~ALIGN_MASK
-        style |= ALIGN_MAP[align]
-        widget.SetWindowStyle(style)
-        widget.Refresh()
+        raise NotImplementedError
 
-    def set_vertical_align(self, align):
-        """ Set the vertical alignment of the text in the widget.
+    def set_time(self, time):
+        """ Set the widget's current time.
 
-        This is not supported on Wx.
+        Parameters
+        ----------
+        time : time
+            The time object to use for setting the time.
 
         """
-        pass
+        raise NotImplementedError
```

### Comparing `enaml-0.9.7/enaml/wx/wx_spin_box.py` & `enaml-0.9.8/enaml/qt/qt_widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,550 +1,546 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2013, Nucleic Development Team.
+# Copyright (c) 2014, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-import wx.lib.newevent
+from atom.api import Typed, Coerced
 
-from atom.api import Int, Typed
+from enaml.drag_drop import DropAction
+from enaml.styling import StyleCache
+from enaml.widgets.widget import Feature, ProxyWidget
+
+from .QtCore import Qt, QSize, QPoint
+from .QtGui import QFont, QWidget, QWidgetAction, QApplication, QDrag, QPixmap
+
+from . import focus_registry
+from .q_resource_helpers import (
+    get_cached_qcolor, get_cached_qfont, get_cached_qimage
+)
+from .qt_drag_drop import QtDropEvent
+from .qt_toolkit_object import QtToolkitObject
+from .styleutil import translate_style
 
-from enaml.widgets.spin_box import ProxySpinBox
 
-from .wx_control import WxControl
+class QtWidget(QtToolkitObject, ProxyWidget):
+    """ A Qt implementation of an Enaml ProxyWidget.
 
+    """
+    #: A reference to the toolkit widget created by the proxy.
+    widget = Typed(QWidget)
 
-#: The changed event for the custom spin box
-wxSpinBoxEvent, EVT_SPIN_BOX = wx.lib.newevent.NewEvent()
-
-
-class wxProperSpinBox(wx.SpinCtrl):
-    """ A custom wx spin control that acts more like QSpinBox.
-
-    The standard wx.SpinCtrl doesn't support too many features, and
-    the ones it does support are (like wrapping) are limited. So,
-    this custom control hard codes the internal range to the maximum
-    range of the wx.SpinCtrl and implements wrapping manually.
-
-    For changed events, users should bind to EVT_SPIN_BOX rather than
-    EVT_SPINCTRL.
-
-    See the method docstrings for supported functionality.
-
-    This control is really a god awful hack and needs to be rewritten
-    using a combination wx.SpinButton and wx.TextCtrl.
+    #: A private copy of the declaration features. This ensures that
+    #: feature cleanup will proceed correctly in the event that user
+    #: code modifies the declaration features value at runtime.
+    _features = Coerced(Feature.Flags)
 
-    """
-    def __init__(self, *args, **kwargs):
-        """ CustomSpinCtrl constructor.
+    #: Internal storage for the shared widget action.
+    _widget_action = Typed(QWidgetAction)
 
-        Parameters
-        ----------
-        *args, **kwargs
-            The positional and keyword arguments for initializing a
-            wx.SpinCtrl.
-
-        """
-        # The max range of the wx.SpinCtrl is the range of a signed
-        # 32bit integer. We don't care about wx's internal value of
-        # the control, since we maintain our own internal counter.
-        # and because the internal value of the widget gets reset to
-        # the minimum of the range whenever SetValueString is called.
-        self._hard_min = -(1 << 31)
-        self._hard_max = (1 << 31) - 1
-        self._internal_value = 0
-        self._low = 0
-        self._high = 100
-        self._step = 1
-        self._prefix = u''
-        self._suffix = u''
-        self._special_value_text = u''
-        self._value_string = unicode(self._low)
-        self._wrap = False
-        self._read_only = False
-
-        # Stores whether spin-up or spin-down was pressed.
-        self._spin_state = None
-
-        super(wxProperSpinBox, self).__init__(*args, **kwargs)
-        super(wxProperSpinBox, self).SetRange(self._hard_min, self._hard_max)
-
-        # Setting the spin control to process the enter key removes
-        # its processing of the Tab key. This is desired for two reasons:
-        # 1) It is consistent with the Qt version of the control.
-        # 2) The default tab processing is kinda wacky in that when
-        #    tab is pressed, it emits a text event with the string
-        #    representation of the integer value of the control,
-        #    regardless of the value of the user supplied string.
-        #    This is definitely not correct and so processing on
-        #    Enter allows us to avoid the issue entirely.
-        self.WindowStyle |= wx.TE_PROCESS_ENTER
-
-        self.Bind(wx.EVT_SPIN_UP, self.OnSpinUp)
-        self.Bind(wx.EVT_SPIN_DOWN, self.OnSpinDown)
-        self.Bind(wx.EVT_SPINCTRL, self.OnSpinCtrl)
-        self.Bind(wx.EVT_TEXT, self.OnText)
-        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
-        self.Bind(wx.EVT_TEXT_ENTER, self.OnEnterPressed)
+    #: Internal storage for the drag origin position.
+    _drag_origin = Typed(QPoint)
 
     #--------------------------------------------------------------------------
-    # Event Handlers
+    # Initialization API
     #--------------------------------------------------------------------------
-    def OnEnterPressed(self, event):
-        """ The event handler for an enter key press. It forces an
-        interpretation of the current text control value.
+    def create_widget(self):
+        """ Create the underlying QWidget object.
 
         """
-        self.InterpretText()
+        self.widget = QWidget(self.parent_widget())
 
-    def OnKillFocus(self, event):
-        """ Handles evaluating the text in the control when the control
-        loses focus.
+    def init_widget(self):
+        """ Initialize the underlying QWidget object.
 
         """
-        # The spin control doesn't emit a spin event when losing focus
-        # to process typed input change unless it results in a different
-        # value, so we have to handle it manually and update the control
-        # again after the event. It must be invoked on a CallAfter or it
-        # doesn't work properly. The lambda avoids a DeadObjectError if
-        # the app is exited before the callback executes.
-        wx.CallAfter(lambda: self.InterpretText() if self else None)
+        super(QtWidget, self).init_widget()
+        widget = self.widget
+        focus_registry.register(widget, self)
+        self._setup_features()
+        d = self.declaration
+        if d.background:
+            self.set_background(d.background)
+        if d.foreground:
+            self.set_foreground(d.foreground)
+        if d.font:
+            self.set_font(d.font)
+        if -1 not in d.minimum_size:
+            self.set_minimum_size(d.minimum_size)
+        if -1 not in d.maximum_size:
+            self.set_maximum_size(d.maximum_size)
+        if d.tool_tip:
+            self.set_tool_tip(d.tool_tip)
+        if d.status_tip:
+            self.set_status_tip(d.status_tip)
+        if not d.enabled:
+            self.set_enabled(d.enabled)
+        self.refresh_style_sheet()
+        # Don't make toplevel widgets visible during init or they will
+        # flicker onto the screen. This applies particularly for things
+        # like status bar widgets which are created with no parent and
+        # then reparented by the status bar. Real top-level widgets must
+        # be explicitly shown by calling their .show() method after they
+        # are created.
+        if widget.parent() or not d.visible:
+            self.set_visible(d.visible)
+
+    def destroy(self):
+        """ Destroy the underlying QWidget object.
+
+        """
+        self._teardown_features()
+        focus_registry.unregister(self.widget)
+        super(QtWidget, self).destroy()
+        # If a QWidgetAction was created for this widget, then it has
+        # taken ownership of the widget and the widget will be deleted
+        # when the QWidgetAction is garbage collected. This means the
+        # superclass destroy() method must run before the reference to
+        # the QWidgetAction is dropped.
+        del self._widget_action
 
-    def OnText(self, event):
-        """ Handles the text event of the spin control to store away the
-        user typed text for later conversion.
+    #--------------------------------------------------------------------------
+    # Private API
+    #--------------------------------------------------------------------------
+    def _setup_features(self):
+        """ Setup the advanced widget feature handlers.
 
         """
-        if self._read_only:
+        features = self._features = self.declaration.features
+        if not features:
             return
-        # Do not be tempted to try to implement the 'tracking' feature
-        # by adding logic to this method. Wx emits this event at weird
-        # times such as ctrl-a select all as well as when SetValueString
-        # is called. Granted, this can be avoided with a recursion guard,
-        # however, there is no way to get/set the caret position on the
-        # control and every call to SetValueString resets the caret
-        # position to Zero. So, there is really no possible way to
-        # implement 'tracking' without creating an entirely new custom
-        # control. So for now, the wx backend just lacks that feature.
-        self._value_string = event.GetString()
-
-    def OnSpinUp(self, event):
-        """ The event handler for the spin up event. We veto the spin
-        event to prevent the control from changing it's internal value.
-        Instead, we maintain complete control of the value.
+        if features & Feature.FocusTraversal:
+            self.hook_focus_traversal()
+        if features & Feature.FocusEvents:
+            self.hook_focus_events()
+        if features & Feature.DragEnabled:
+            self.hook_drag()
+        if features & Feature.DropEnabled:
+            self.hook_drop()
 
-        """
-        event.Veto()
-        if self._read_only:
-            return
-        self._spin_state = 'up'
-        self.OnSpinCtrl(event)
-        self._spin_state = None
-
-    def OnSpinDown(self, event):
-        """ The event handler for the spin down event. We veto the spin
-        event to prevent the control from changing it's internal value.
-        Instead, we maintain complete control of the value.
+    def _teardown_features(self):
+        """ Teardowns the advanced widget feature handlers.
 
         """
-        event.Veto()
-        if self._read_only:
+        features = self._features
+        if not features:
             return
-        self._spin_state = 'down'
-        self.OnSpinCtrl(event)
-        self._spin_state = None
+        if features & Feature.FocusTraversal:
+            self.unhook_focus_traversal()
+        if features & Feature.FocusEvents:
+            self.unhook_focus_events()
+        if features & Feature.DragEnabled:
+            self.unhook_drag()
+        if features & Feature.DropEnabled:
+            self.unhook_drop()
+
+    #--------------------------------------------------------------------------
+    # Protected API
+    #--------------------------------------------------------------------------
+    def refresh_style_sheet(self):
+        """ Refresh the widget style sheet with the current style data.
+
+        """
+        parts = []
+        name = self.widget.objectName()
+        for style in StyleCache.styles(self.declaration):
+            t = translate_style(name, style)
+            if t:
+                parts.append(t)
+        if len(parts) > 0:
+            stylesheet = u'\n\n'.join(parts)
+        else:
+            stylesheet = u''
+        self.widget.setStyleSheet(stylesheet)
 
-    def OnSpinCtrl(self, event):
-        """ Handles the spin control being changed by user interaction.
-        All of the manual stepping and wrapping logic is computed by
-        this method.
+    def tab_focus_request(self, reason):
+        """ Handle a custom tab focus request.
 
-        """
-        if self._read_only:
-            return
-        last = self._internal_value
-        low = self._low
-        high = self._high
-        step = self._step
-        wrap = self._wrap
-        spin_state = self._spin_state
-        if spin_state == 'down':
-            if last == low:
-                if wrap:
-                    computed = high
-                else:
-                    computed = low
-            else:
-                computed = last - step
-                if computed < low:
-                    computed = low
-            self.SetValue(computed)
-        elif spin_state == 'up':
-            if last == high:
-                if wrap:
-                    computed = low
-                else:
-                    computed = high
-            else:
-                computed = last + step
-                if computed > high:
-                    computed = high
-            self.SetValue(computed)
-        else:
-            # A suprious spin event generated by wx when the widget loses
-            # focus. We can safetly ignore it.
-            pass
+        This method is called when focus is being set on the proxy
+        as a result of a user-implemented focus traversal handler.
+        This can be reimplemented by subclasses as needed.
 
-    #--------------------------------------------------------------------------
-    # Getters/Setters
-    #--------------------------------------------------------------------------
-    def GetLow(self):
-        """ Returns the minimum value of the control.
+        Parameters
+        ----------
+        reason : Qt.FocusReason
+            The reason value for the focus request.
+
+        Returns
+        -------
+        result : bool
+            True if focus was set, False otherwise.
 
         """
-        return self._low
+        widget = self.focus_target()
+        if not widget.focusPolicy & Qt.TabFocus:
+            return False
+        if not widget.isEnabled():
+            return False
+        if not widget.isVisibleTo(widget.window()):
+            return False
+        widget.setFocus(reason)
+        return False
 
-    def GetMin(self):
-        """ Equivalent to GetLow().
+    def focus_target(self):
+        """ Return the current focus target for a focus request.
+
+        This can be reimplemented by subclasses as needed. The default
+        implementation of this method returns the current proxy widget.
 
         """
-        return self._low
+        return self.widget
+
+    def hook_focus_traversal(self):
+        """ Install the hooks for focus traversal.
 
-    def SetLow(self, low):
-        """ Sets the minimum value of the control and changes the
-        value to the min if the current value would be out of range.
+        This method may be overridden by subclasses as needed.
 
         """
-        if low < self._hard_min:
-            raise ValueError('%s is too low for wxProperSpinBox.' % low)
-        self._low = low
-        if self.GetValue() < low:
-            self.SetValue(low)
+        self.widget.focusNextPrevChild = self.focusNextPrevChild
+
+    def unhook_focus_traversal(self):
+        """ Remove the hooks for the next/prev child focusing.
 
-    def GetHigh(self):
-        """ Returns the maximum value of the control.
+        This method may be overridden by subclasses as needed.
 
         """
-        return self._high
+        del self.widget.focusNextPrevChild
 
-    def GetMax(self):
-        """ Equivalent to GetHigh().
+    def hook_focus_events(self):
+        """ Install the hooks for focus events.
+
+        This method may be overridden by subclasses as needed.
 
         """
-        return self._high
+        widget = self.widget
+        widget.focusInEvent = self.focusInEvent
+        widget.focusOutEvent = self.focusOutEvent
+
+    def unhook_focus_events(self):
+        """ Remove the hooks for the focus events.
 
-    def SetHigh(self, high):
-        """ Sets the maximum value of the control and changes the
-        value to the max if the current value would be out of range.
+        This method may be overridden by subclasses as needed.
 
         """
-        if high > self._hard_max:
-            raise ValueError('%s is too high for wxProperSpinBox.' % high)
-        self._high = high
-        if self.GetValue() > high:
-            self.SetValue(high)
+        widget = self.widget
+        del widget.focusInEvent
+        del widget.focusOutEvent
 
-    def SetRange(self, low, high):
-        """ Sets the low and high values of the control.
+    def focusNextPrevChild(self, next_child):
+        """ The default 'focusNextPrevChild' implementation.
 
         """
-        self.SetLow(low)
-        self.SetHigh(high)
+        fd = focus_registry.focused_declaration()
+        if next_child:
+            child = self.declaration.next_focus_child(fd)
+            reason = Qt.TabFocusReason
+        else:
+            child = self.declaration.previous_focus_child(fd)
+            reason = Qt.BacktabFocusReason
+        if child is not None and child.proxy_is_active:
+            return child.proxy.tab_focus_request(reason)
+        widget = self.widget
+        return type(widget).focusNextPrevChild(widget, next_child)
 
-    def GetStep(self):
-        """ Returns the step size of the control.
+    def focusInEvent(self, event):
+        """ The default 'focusInEvent' implementation.
 
         """
-        return self._step
+        widget = self.widget
+        type(widget).focusInEvent(widget, event)
+        self.declaration.focus_gained()
 
-    def SetStep(self, step):
-        """ Sets the step size of the control.
+    def focusOutEvent(self, event):
+        """ The default 'focusOutEvent' implementation.
 
         """
-        self._step = step
+        widget = self.widget
+        type(widget).focusOutEvent(widget, event)
+        self.declaration.focus_lost()
 
-    def GetWrap(self):
-        """ Gets the wrap flag of the control.
+    def hook_drag(self):
+        """ Install the hooks for drag operations.
 
         """
-        return self._wrap
+        widget = self.widget
+        widget.mousePressEvent = self.mousePressEvent
+        widget.mouseMoveEvent = self.mouseMoveEvent
+        widget.mouseReleaseEvent = self.mouseReleaseEvent
 
-    def SetWrap(self, wrap):
-        """ Sets the wrap flag of the control.
+    def unhook_drag(self):
+        """ Remove the hooks for drag operations.
 
         """
-        self._wrap = wrap
+        widget = self.widget
+        del widget.mousePressEvent
+        del widget.mouseMoveEvent
+        del widget.mouseReleaseEvent
 
-    def GetPrefix(self):
-        """ Get the prefix text for the control.
-
-        Returns
-        -------
-        result : unicode
-            The unicode prefix text.
+    def mousePressEvent(self, event):
+        """ Handle the mouse press event for a drag operation.
 
         """
-        return self._prefix
+        if event.button() == Qt.LeftButton:
+            self._drag_origin = event.pos()
+        widget = self.widget
+        type(widget).mousePressEvent(widget, event)
 
-    def SetPrefix(self, prefix):
-        """ Set the prefix text for the control.
-
-        Parameters
-        ----------
-        prefix : unicode
-            The unicode prefix text for the control.
+    def mouseMoveEvent(self, event):
+        """ Handle the mouse move event for a drag operation.
 
         """
-        self._prefix = prefix
+        if event.buttons() & Qt.LeftButton and self._drag_origin is not None:
+            dist = (event.pos() - self._drag_origin).manhattanLength()
+            if dist >= QApplication.startDragDistance():
+                self.do_drag()
+                self._drag_origin = None
+                return
+        widget = self.widget
+        type(widget).mouseMoveEvent(widget, event)
 
-    def GetSuffix(self):
-        """ Get the suffix text for the control.
-
-        Returns
-        -------
-        result : unicode
-            The unicode suffix text.
+    def mouseReleaseEvent(self, event):
+        """ Handle the mouse release event for the drag operation.
 
         """
-        return self._suffix
+        if event.button() == Qt.LeftButton:
+            self._drag_origin = None
+        widget = self.widget
+        type(widget).mouseReleaseEvent(widget, event)
 
-    def SetSuffix(self, suffix):
-        """ Set the suffix text for the control.
-
-        Parameters
-        ----------
-        suffix : unicode
-            The unicode suffix text for the control.
+    def hook_drop(self):
+        """ Install hooks for drop operations.
 
         """
-        self._suffix = suffix
-
-    def GetSpecialValueText(self):
-        """ Returns the special value text for the spin box.
+        widget = self.widget
+        widget.setAcceptDrops(True)
+        widget.dragEnterEvent = self.dragEnterEvent
+        widget.dragMoveEvent = self.dragMoveEvent
+        widget.dragLeaveEvent = self.dragLeaveEvent
+        widget.dropEvent = self.dropEvent
 
-        Returns
-        -------
-        result : unicode
-            The unicode special value text.
+    def unhook_drop(self):
+        """ Remove hooks for drop operations.
 
         """
-        return self._special_value_text
-
-    def SetSpecialValueText(self, text):
-        """ Set the special value text for the control.
+        widget = self.widget
+        widget.setAcceptDrops(False)
+        del widget.dragEnterEvent
+        del widget.dragMoveEvent
+        del widget.dragLeaveEvent
+        del widget.dropEvent
 
-        Parameters
-        ----------
-        text : unicode
-            The unicode special value text for the control.
+    def do_drag(self):
+        """ Perform the drag operation for the widget.
 
         """
-        self._special_value_text = text
+        drag_data = self.declaration.drag_start()
+        if drag_data is None:
+            return
+        widget = self.widget
+        qdrag = QDrag(widget)
+        qdrag.setMimeData(drag_data.mime_data.q_data())
+        if drag_data.image is not None:
+            qimg = get_cached_qimage(drag_data.image)
+            qdrag.setPixmap(QPixmap.fromImage(qimg))
+        else:
+            qdrag.setPixmap(QPixmap.grabWidget(widget))
+        default = Qt.DropAction(drag_data.default_drop_action)
+        supported = Qt.DropActions(drag_data.supported_actions)
+        qresult = qdrag.exec_(supported, default)
+        self.declaration.drag_end(drag_data, DropAction(int(qresult)))
 
-    def GetReadOnly(self):
-        """ Get the read only flag for the control.
-
-        Returns
-        -------
-        result : bool
-            True if the control is read only, False otherwise.
+    def dragEnterEvent(self, event):
+        """ Handle the drag enter event for the widget.
 
         """
-        return self._suffix
-
-    def SetReadOnly(self, read_only):
-        """ Set the read only flag for the control
+        self.declaration.drag_enter(QtDropEvent(event))
 
-        Parameters
-        ----------
-        read_only : bool
-            True if the control should be read only, False otherwise.
+    def dragMoveEvent(self, event):
+        """ Handle the drag move event for the widget.
 
         """
-        self._read_only = read_only
+        self.declaration.drag_move(QtDropEvent(event))
 
-    def GetValue(self):
-        """ Returns the internal integer value of the control.
+    def dragLeaveEvent(self, event):
+        """ Handle the drag leave event for the widget.
 
         """
-        return self._internal_value
+        self.declaration.drag_leave()
 
-    def SetValue(self, value):
-        """ Sets the value of the control to the given value, provided
-        that the value is within the range of the control. If the
-        given value is within range, and is different from the current
-        value of the control, an EVT_SPIN_BOX will be emitted.
+    def dropEvent(self, event):
+        """ Handle the drop event for the widget.
 
         """
-        different = False
-        if self._low <= value <= self._high:
-            different = (self._internal_value != value)
-            self._internal_value = value
+        self.declaration.drop(QtDropEvent(event))
+
+    #--------------------------------------------------------------------------
+    # Framework API
+    #--------------------------------------------------------------------------
+    def get_action(self, create=False):
+        """ Get the shared widget action for this widget.
+
+        This API is used to support widgets in tool bars and menus.
+
+        Parameters
+        ----------
+        create : bool, optional
+            Whether to create the action if it doesn't already exist.
+            The default is False.
 
-        # Always set the value string, just to be overly
-        # safe that we don't fall out of sync.
-        self._value_string = self.TextFromValue(self._internal_value)
-        self.SetValueString(self._value_string)
+        Returns
+        -------
+        result : QWidgetAction or None
+            The cached widget action or None, depending on arguments.
 
-        if different:
-            evt = wxSpinBoxEvent()
-            wx.PostEvent(self, evt)
+        """
+        action = self._widget_action
+        if action is None and create:
+            action = self._widget_action = QWidgetAction(None)
+            action.setDefaultWidget(self.widget)
+        return action
 
     #--------------------------------------------------------------------------
-    # Support Methods
+    # ProxyWidget API
     #--------------------------------------------------------------------------
-    def InterpretText(self):
-        """ Interprets the user supplied text and updates the control.
+    def set_minimum_size(self, min_size):
+        """ Sets the minimum size of the widget.
 
         """
-        prefix = self._prefix
-        suffix = self._suffix
-        svt = self._special_value_text
-        text = self._value_string
-        if svt and text == svt:
-            self.SetValue(self._low)
-            return
-        if prefix and text.startswith(prefix):
-            text = text[len(prefix):]
-        if suffix and text.endswith(suffix):
-            text = text[:-len(suffix)]
-        try:
-            value = int(text)
-        except ValueError:
-            value = self._internal_value
-        self.SetValue(value)
-
-    def TextFromValue(self, value):
-        """ Converts the given integer to a string for display.
-
-        """
-        prefix = self._prefix
-        suffix = self._suffix
-        svt = self._special_value_text
-        if value == self._low and svt:
-            return svt
-        text = unicode(value)
-        if prefix:
-            text = '%s%s' % (prefix, text)
-        if suffix:
-            text = '%s%s' % (text, suffix)
-        return text
+        # QWidget uses (0, 0) as the minimum size.
+        if -1 in min_size:
+            min_size = (0, 0)
+        self.widget.setMinimumSize(QSize(*min_size))
 
+    def set_maximum_size(self, max_size):
+        """ Sets the maximum size of the widget.
 
-#: Cyclic guard flag
-VALUE_FLAG = 0x1
+        """
+        # QWidget uses 16777215 as the max size
+        if -1 in max_size:
+            max_size = (16777215, 16777215)
+        self.widget.setMaximumSize(QSize(*max_size))
 
+    def set_enabled(self, enabled):
+        """ Set the enabled state of the widget.
 
-class WxSpinBox(WxControl, ProxySpinBox):
-    """ A Wx implementation of an Enaml ProxySpinBox.
+        """
+        self.widget.setEnabled(enabled)
+        action = self._widget_action
+        if action is not None:
+            action.setEnabled(enabled)
 
-    """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(wxProperSpinBox)
+    def set_visible(self, visible):
+        """ Set the visibility of the widget.
 
-    #: Cyclic guard flags
-    _guard = Int(0)
+        """
+        self.widget.setVisible(visible)
+        action = self._widget_action
+        if action is not None:
+            action.setVisible(visible)
 
-    #--------------------------------------------------------------------------
-    # Initialization API
-    #--------------------------------------------------------------------------
-    def create_widget(self):
-        """ Create the underlying wxProperSpinBox widget.
+    def set_background(self, background):
+        """ Set the background color of the widget.
 
         """
-        self.widget = wxProperSpinBox(self.parent_widget())
-
-    def init_widget(self, ):
-        """ Create and initialize the slider control.
+        widget = self.widget
+        role = widget.backgroundRole()
+        if background is not None:
+            qcolor = get_cached_qcolor(background)
+            widget.setAutoFillBackground(True)
+        else:
+            app_palette = QApplication.instance().palette(widget)
+            qcolor = app_palette.color(role)
+            widget.setAutoFillBackground(False)
+        palette = widget.palette()
+        palette.setColor(role, qcolor)
+        widget.setPalette(palette)
+
+    def set_foreground(self, foreground):
+        """ Set the foreground color of the widget.
 
         """
-        super(WxSpinBox, self).init_widget()
-        d = self.declaration
-        self.set_maximum(d.maximum)
-        self.set_minimum(d.minimum)
-        self.set_value(d.value)
-        self.set_prefix(d.prefix)
-        self.set_suffix(d.suffix)
-        self.set_special_value_text(d.special_value_text)
-        self.set_single_step(d.single_step)
-        self.set_read_only(d.read_only)
-        self.set_wrapping(d.wrapping)
-        self.widget.Bind(EVT_SPIN_BOX, self.on_value_changed)
+        widget = self.widget
+        role = widget.foregroundRole()
+        if foreground is not None:
+            qcolor = get_cached_qcolor(foreground)
+        else:
+            app_palette = QApplication.instance().palette(widget)
+            qcolor = app_palette.color(role)
+        palette = widget.palette()
+        palette.setColor(role, qcolor)
+        widget.setPalette(palette)
 
-    #--------------------------------------------------------------------------
-    # Event Handlers
-    #--------------------------------------------------------------------------
-    def on_value_changed(self, event):
-        """ The event handler for the 'EVT_SPIN_BOX' event.
+    def set_font(self, font):
+        """ Set the font of the widget.
 
         """
-        if not self._guard & VALUE_FLAG:
-            self._guard |= VALUE_FLAG
-            try:
-                self.declaration.value = self.widget.GetValue()
-            finally:
-                self._guard &= ~VALUE_FLAG
+        if font is not None:
+            self.widget.setFont(get_cached_qfont(font))
+        else:
+            self.widget.setFont(QFont())
 
-    #--------------------------------------------------------------------------
-    # ProxySpinBox API
-    #--------------------------------------------------------------------------
-    def set_maximum(self, maximum):
-        """ Set the widget's maximum value.
+    def set_tool_tip(self, tool_tip):
+        """ Set the tool tip for the widget.
 
         """
-        self.widget.SetHigh(maximum)
+        self.widget.setToolTip(tool_tip)
 
-    def set_minimum(self, minimum):
-        """ Set the widget's minimum value.
+    def set_status_tip(self, status_tip):
+        """ Set the status tip for the widget.
 
         """
-        self.widget.SetLow(minimum)
+        self.widget.setStatusTip(status_tip)
 
-    def set_value(self, value):
-        """ Set the spin box's value.
+    def ensure_visible(self):
+        """ Ensure the widget is visible.
 
         """
-        if not self._guard & VALUE_FLAG:
-            self._guard |= VALUE_FLAG
-            try:
-                self.widget.SetValue(value)
-            finally:
-                self._guard &= ~VALUE_FLAG
+        self.widget.setVisible(True)
+        action = self._widget_action
+        if action is not None:
+            action.setVisible(True)
 
+    def ensure_hidden(self):
+        """ Ensure the widget is hidden.
+
+        """
+        self.widget.setVisible(False)
+        action = self._widget_action
+        if action is not None:
+            action.setVisible(False)
 
-    def set_prefix(self, prefix):
-        """ Set the prefix for the spin box.
+    def restyle(self):
+        """ Restyle the widget with the current style data.
 
         """
-        self.widget.SetPrefix(prefix)
+        self.refresh_style_sheet()
 
-    def set_suffix(self, suffix):
-        """ Set the suffix for the spin box.
+    def set_focus(self):
+        """ Set the keyboard input focus to this widget.
 
         """
-        self.widget.SetSuffix(suffix)
+        self.focus_target().setFocus(Qt.OtherFocusReason)
 
-    def set_special_value_text(self, text):
-        """ Set the special value text for the spin box.
+    def clear_focus(self):
+        """ Clear the keyboard input focus from this widget.
 
         """
-        self.widget.SetSpecialValueText(text)
+        self.focus_target().clearFocus()
 
-    def set_single_step(self, step):
-        """ Set the widget's single step value.
+    def has_focus(self):
+        """ Test whether this widget has input focus.
 
         """
-        self.widget.SetStep(step)
+        return self.focus_target().hasFocus()
 
-    def set_read_only(self, read_only):
-        """ Set the widget's read only flag.
+    def focus_next_child(self):
+        """ Give focus to the next widget in the focus chain.
 
         """
-        self.widget.SetReadOnly(read_only)
+        self.focus_target().focusNextChild()
 
-    def set_wrapping(self, wrapping):
-        """ Set the widget's wrapping flag.
+    def focus_previous_child(self):
+        """ Give focus to the previous widget in the focus chain.
 
         """
-        self.widget.SetWrap(wrapping)
+        self.focus_target().focusPreviousChild()
```

### Comparing `enaml-0.9.7/enaml/wx/wx_frame.py` & `enaml-0.9.8/enaml/qt/qt_html.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,40 +3,47 @@
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 from atom.api import Typed
 
-from enaml.widgets.frame import ProxyFrame
+from enaml.widgets.html import ProxyHtml
 
-import wx
+from .QtGui import QTextEdit
 
-from .wx_constraints_widget import WxConstraintsWidget
+from .qt_control import QtControl
 
 
-class WxFrame(WxConstraintsWidget, ProxyFrame):
-    """ A Wx implementation of an Enaml ProxyFrame.
+class QtHtml(QtControl, ProxyHtml):
+    """ A Qt implementation of an Enaml ProxyHtml widget.
 
     """
-    #: A reference to the toolkit widget created by the proxy.
-    widget = Typed(wx.Panel)
+    #: A reference to the widget created by the proxy.
+    widget = Typed(QTextEdit)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Creates the QContainer widget.
+        """ Create the underlying html widget.
 
         """
-        self.widget = wx.Panel(self.parent_widget())
+        widget = QTextEdit(self.parent_widget())
+        widget.setReadOnly(True)
+        self.widget = widget
+
+    def init_widget(self):
+        """ Initialize the underlying widget.
+
+        """
+        super(QtHtml, self).init_widget()
+        self.set_source(self.declaration.source)
 
     #--------------------------------------------------------------------------
-    # ProxyFrame API
+    # ProxyHtml API
     #--------------------------------------------------------------------------
-    def set_border(self, border):
-        """ Set the border for the widget.
-
-        This is not supported on Wx.
+    def set_source(self, source):
+        """ Set the source of the html widget
 
         """
-        pass
+        self.widget.setHtml(source)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_single_widget_sizer.py` & `enaml-0.9.8/enaml/qt/qt_frame.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,68 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
+from atom.api import Typed
 
+from enaml.widgets.frame import ProxyFrame
 
-class wxSingleWidgetSizer(wx.PySizer):
-    """ A custom wx Sizer for sizing a single child widget.
+from .QtGui import QFrame
 
-    There can only be one widget in this sizer at a time and it should
-    be added via the .Add(...) method. Old items will be removed
-    automatically (but not destroyed).
+from .qt_constraints_widget import QtConstraintsWidget
 
-    """
-    _default_size = wx.Size(-1, -1)
 
-    _widget = None
+STYLE = {
+    'box': QFrame.Box,
+    'panel': QFrame.Panel,
+    'styled_panel': QFrame.StyledPanel,
+}
 
-    def CalcMax(self):
-        """ A method to compute the maximum size allowed by the sizer.
 
-        This is not a native wx sizer method, but is included for
-        convenience.
+LINE_STYLE = {
+    'plain': QFrame.Plain,
+    'sunken': QFrame.Sunken,
+    'raised': QFrame.Raised,
+}
 
-        """
-        widget = self._widget
-        if not widget:
-            return self._default_size
-        return widget.GetMaxSize()
 
-    def GetWidget(self):
-        """ Get a reference tot he underlying widget.
+class QtFrame(QtConstraintsWidget, ProxyFrame):
+    """ A Qt implementation of an Enaml ProxyFrame.
 
-        """
-        return self._widget
+    """
+    #: A reference to the toolkit widget created by the proxy.
+    widget = Typed(QFrame)
 
-    def Add(self, widget):
-        """ Adds the given widget to the sizer, removing the old widget
-        if present. The old widget is not destroyed.
+    #--------------------------------------------------------------------------
+    # Initialization API
+    #--------------------------------------------------------------------------
+    def create_widget(self):
+        """ Creates the QContainer widget.
 
         """
-        if self._widget is not widget:
-            self.Clear(deleteWindows=False)
-            old = self._widget
-            if old:
-                old.Hide()
-            self._widget = widget
-            if widget:
-                widget.Show()
-                res = super(wxSingleWidgetSizer, self).Add(widget)
-                self.Layout()
-                return res
-
-    def CalcMin(self):
-        """ Returns the minimum size for the children this sizer is
-        managing.
+        self.widget = QFrame(self.parent_widget())
+
+    def init_widget(self):
+        """ Initialize the widget.
 
         """
-        widget = self._widget
-        if not widget:
-            return self._default_size
-        return widget.GetEffectiveMinSize()
+        super(QtFrame, self).init_widget()
+        self.set_border(self.declaration.border)
 
-    def RecalcSizes(self):
-        """ Resizes the child to fit the available space of the window.
+    #--------------------------------------------------------------------------
+    # ProxyFrame API
+    #--------------------------------------------------------------------------
+    def set_border(self, border):
+        """ Set the border for the widget.
 
         """
-        widget = self._widget
-        if widget:
-            widget.SetSize(self.GetSize())
+        widget = self.widget
+        if border is None:
+            widget.setFrameShape(QFrame.NoFrame)
+            return
+        widget.setFrameShape(STYLE[border.style])
+        widget.setFrameShadow(LINE_STYLE[border.line_style])
+        widget.setLineWidth(border.line_width)
+        widget.setMidLineWidth(border.midline_width)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_control.py` & `enaml-0.9.8/enaml/qt/qt_control.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 from enaml.widgets.control import ProxyControl
 
-from .wx_constraints_widget import WxConstraintsWidget
+from .qt_constraints_widget import QtConstraintsWidget
 
 
-class WxControl(WxConstraintsWidget, ProxyControl):
-    """ A Wx implementation of an Enaml Control.
+class QtControl(QtConstraintsWidget, ProxyControl):
+    """ A Qt implementation of an Enaml Control.
 
     """
-    # The WxConstraintsWidget superclass is a sufficient implementation.
+    # The QtConstraintsWidget superclass is a sufficient implementation.
     pass
```

### Comparing `enaml-0.9.7/enaml/wx/wx_bounded_date.py` & `enaml-0.9.8/enaml/qt/qt_bounded_date.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,27 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import datetime
-
-import wx
-
 from atom.api import Int
 
 from enaml.widgets.bounded_date import ProxyBoundedDate
 
-from .wx_control import WxControl
-
-
-def as_wx_date(py_date):
-    """ Convert an iso date string to a wxDateTime.
-
-    """
-    day = py_date.day
-    month = py_date.month - 1  # wx peculiarity!
-    year = py_date.year
-    return wx.DateTimeFromDMY(day, month, year)
-
-
-def as_py_date(wx_date):
-    """ Convert a QDate object into and iso date string.
-
-    """
-    day = wx_date.GetDay()
-    month = wx_date.GetMonth() + 1  # wx peculiarity!
-    year = wx_date.GetYear()
-    return datetime.date(year, month, day)
+from .qt_control import QtControl
 
 
 # cyclic notification guard flags
 CHANGED_GUARD = 0x1
 
 
-class WxBoundedDate(WxControl, ProxyBoundedDate):
-    """ A base class for use with Wx widgets implementing behavior
-    for subclasses of BoundedDate.
+class QtBoundedDate(QtControl, ProxyBoundedDate):
+    """ A base class for implementing Qt Enaml date widgets.
 
     """
     #: Cyclic notification guard. This a bitfield of multiple guards.
     _guard = Int(0)
 
     #--------------------------------------------------------------------------
     # Initialization API
@@ -54,32 +29,28 @@
     def create_widget(self):
         """ Implement in a subclass to create the date widget.
 
         """
         raise NotImplementedError
 
     def init_widget(self):
-        """ Create and initialize the bounded date widget.
+        """ Initialize the date widget.
 
         """
-        super(WxBoundedDate, self).init_widget()
+        super(QtBoundedDate, self).init_widget()
         d = self.declaration
         self.set_minimum(d.minimum)
         self.set_maximum(d.maximum)
         self.set_date(d.date)
 
     #--------------------------------------------------------------------------
-    # Event Handlers
+    # Signal Handlers
     #--------------------------------------------------------------------------
-    def on_date_changed(self, event):
-        """ An event handler to connect to the date changed signal of
-        the underlying widget.
-
-        This will convert the wxDateTime to iso format and send the Enaml
-        widget the 'date_changed' action.
+    def on_date_changed(self):
+        """ A signal handler for the date changed signal.
 
         """
         if not self._guard & CHANGED_GUARD:
             self.declaration.date = self.get_date()
 
     #--------------------------------------------------------------------------
     # Abstract Methods and ProxyBoundedDate API
```

### Comparing `enaml-0.9.7/enaml/wx/wx_group_box.py` & `enaml-0.9.8/enaml/qt/qt_image_view.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,269 +1,264 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-
 from atom.api import Typed
 
-from enaml.widgets.group_box import ProxyGroupBox
-
-from .wx_container import WxContainer, wxContainer
+from enaml.widgets.image_view import ProxyImageView
 
+from .QtGui import QFrame, QPainter, QPixmap
 
-WX_ALIGNMENTS = {
-    'left': wx.ALIGN_LEFT,
-    'center': wx.ALIGN_CENTER,
-    'right': wx.ALIGN_RIGHT,
-}
+from .q_resource_helpers import get_cached_qimage
+from .qt_control import QtControl
 
 
-class wxGroupBox(wxContainer):
-    """ A wxContainer sublcass that implements GroupBox functionality.
+class QImageView(QFrame):
+    """ A custom QFrame that will paint a QPixmap as an image. The
+    api is similar to QLabel, but with a few more options to control
+    how the image scales.
 
     """
-    def __init__(self, *args, **kwargs):
-        """ Initialize a wxGroupBox.
+    def __init__(self, parent=None):
+        """ Initialize a QImageView.
 
         Parameters
         ----------
-        *args, **kwargs
-            The positional and keyword arguments to initialize a
-            wxContainer.
-
-        """
-        super(wxGroupBox, self).__init__(*args, **kwargs)
-        self._title = ''
-        self._border = wx.StaticBox(self)
-        self._line = wx.StaticLine(self)
-        self._label = wx.StaticText(self)
-        self._label.Raise()
-        self._label_size = self._label.GetBestSize()
-        self._title_alignment = wx.ALIGN_LEFT
-        self._flat = False
-        # Set the panel to double buffered or suffer terrible
-        # rendering artifacts
-        self.SetDoubleBuffered(True)
+        parent : QWidget or None, optional
+            The parent widget of this image viewer.
+
+        """
+        super(QImageView, self).__init__(parent)
+        self._pixmap = None
+        self._scaled_contents = False
+        self._allow_upscaling = False
+        self._preserve_aspect_ratio = False
+
+    #--------------------------------------------------------------------------
+    # Private API
+    #--------------------------------------------------------------------------
+    def paintEvent(self, event):
+        """ A custom paint event handler which draws the image according
+        to the current size constraints.
+
+        """
+        pixmap = self._pixmap
+        if pixmap is None:
+            return
+
+        pm_size = pixmap.size()
+        pm_width = pm_size.width()
+        pm_height = pm_size.height()
+        if pm_width == 0 or pm_height == 0:
+            return
+
+        # Use the widget rect instead of the event rect so the image
+        # paints properly in a scroll area where it may be clipped.
+        evt_rect = self.rect()
+        evt_x = evt_rect.x()
+        evt_y = evt_rect.y()
+        evt_width = evt_rect.width()
+        evt_height = evt_rect.height()
+
+        if not self._scaled_contents:
+            # If the image isn't scaled, it is centered if possible.
+            # Otherwise, it's painted at the origin and clipped.
+            paint_x = max(0, int((evt_width / 2. - pm_width / 2.) + evt_x))
+            paint_y = max(0, int((evt_height / 2. - pm_height / 2.) + evt_y))
+            paint_width = pm_width
+            paint_height = pm_height
+        else:
+            # If the image *is* scaled, it's scaled size depends on the
+            # size of the paint area as well as the other scaling flags.
+            if self._preserve_aspect_ratio:
+                pm_ratio = float(pm_width) / pm_height
+                evt_ratio = float(evt_width) / evt_height
+                if evt_ratio >= pm_ratio:
+                    if self._allow_upscaling:
+                        paint_height = evt_height
+                    else:
+                        paint_height = min(pm_height, evt_height)
+                    paint_width = int(paint_height * pm_ratio)
+                else:
+                    if self._allow_upscaling:
+                        paint_width = evt_width
+                    else:
+                        paint_width = min(pm_width, evt_width)
+                    paint_height = int(paint_width / pm_ratio)
+            else:
+                if self._allow_upscaling:
+                    paint_height = evt_height
+                    paint_width = evt_width
+                else:
+                    paint_height = min(pm_height, evt_height)
+                    paint_width = min(pm_width, evt_width)
+            # In all cases of scaling, we know that the scaled image is
+            # no larger than the paint area, and can thus be centered.
+            paint_x = int((evt_width / 2. - paint_width / 2.) + evt_x)
+            paint_y = int((evt_height / 2. - paint_height / 2.) + evt_y)
+
+        # Finally, draw the pixmap into the calculated rect.
+        painter = QPainter(self)
+        painter.setRenderHint(QPainter.SmoothPixmapTransform)
+        painter.drawPixmap(paint_x, paint_y, paint_width, paint_height, pixmap)
 
     #--------------------------------------------------------------------------
     # Public API
     #--------------------------------------------------------------------------
-    def GetAlignment(self):
-        """ Return the wx alignment flag for the current alignment
-        of the group box title.
+    def sizeHint(self):
+        """ Returns a appropriate size hint for the image based on the
+        underlying QPixmap.
 
         """
-        return self._title_alignment
+        pixmap = self._pixmap
+        if pixmap is not None:
+            return pixmap.size()
+        return super(QImageView, self).sizeHint()
 
-    def SetAlignment(self, alignment):
-        """ Set the alignment of the title of the group box. Should
-        be one of wx.ALIGN_LEFT, wx.ALIGN_RIGHT, wx.ALIGN_CENTER.
+    def pixmap(self):
+        """ Returns the underlying pixmap for the image view.
 
         """
-        self._title_alignment = alignment
-        self._update_layout()
+        return self._pixmap
 
-    def GetFlat(self):
-        """ Returns a boolean indicating whether the group box is using
-        a flat style.
+    def setPixmap(self, pixmap):
+        """ Set the pixmap to use as the image in the widget.
+
+        Parameters
+        ----------
+        pixamp : QPixmap
+            The QPixmap to use as the image in the widget.
 
         """
-        return self._flat
+        self._pixmap = pixmap
+        self.update()
 
-    def SetFlat(self, flat):
-        """ Set whether or not the group box should be displayed using
-        a flat style.
+    def scaledContents(self):
+        """ Returns whether or not the contents scale with the widget
+        size.
 
         """
-        self._flat = flat
-        if flat:
-            self._border.Show(False)
-            self._line.Show(True)
-        else:
-            self._border.Show(True)
-            self._line.Show(False)
-        self._update_layout()
-
-    def GetTitle(self):
-        """ Return the current title text in the group box.
-
-        """
-        # Undo the hack applied in SetTitle(...)
-        title = self._title
-        if title:
-            title = title[1:-1]
-        return title
-
-    def SetTitle(self, title):
-        """ Set the current title text in the group box.
-
-        """
-        # A bit of a hack to give us a little padding around the label
-        if title:
-            title = ' %s ' % title
-        self._title = title
-        self._label.SetLabel(title)
-        self._label_size = self._label.GetBestSize()
-        if not title:
-            self._label.Show(False)
-        else:
-            self._label.Show(True)
-        self._update_layout()
+        return self._scaled_contents
 
-    def SetDimensions(self, x, y, width, height):
-        """ Overridden parent class method to synchronize the group
-        box decorations.
+    def setScaledContents(self, scaled):
+        """ Set whether the contents scale with the widget size.
+
+        Parameters
+        ----------
+        scaled : bool
+            If True, the image will be scaled to fit the widget size,
+            subject to the other sizing constraints in place. If False,
+            the image will not scale and will be clipped as required.
 
         """
-        super(wxGroupBox, self).SetDimensions(x, y, width, height)
-        self._update_layout()
+        self._scaled_contents = scaled
+        self.update()
 
-    def SetSize(self, size):
-        """ Overridden parent class method to synchronize the group
-        box decorations.
+    def allowUpscaling(self):
+        """ Returns whether or not the image can be scaled greater than
+        its natural size.
 
         """
-        super(wxGroupBox, self).SetSize(size)
-        self._update_layout()
+        return self._allow_upscaling
+
+    def setAllowUpscaling(self, allow):
+        """ Set whether or not to allow the image to be scaled beyond
+        its natural size.
 
-    def GetContentsMargins(self):
-        """ Get the contents margins for the group box.
+        Parameters
+        ----------
+        allow : bool
+            If True, then the image may be scaled larger than its
+            natural if it is scaled to fit. If False, the image will
+            never be scaled larger than its natural size. In either
+            case, the image may be scaled smaller.
 
-        These margins are computed empirically so that they look similar
-        to the margins provided by Qt on Windows.
+        """
+        self._allow_upscaling = allow
+        self.update()
 
-        Returns
-        -------
-        result : tuple
-            The top, right, bottom, and left margin values.
+    def preserveAspectRatio(self):
+        """ Returns whether or not the aspect ratio of the image is
+        maintained during a resize.
 
         """
-        label = self._label
-        height = label.GetCharHeight()
-        if not label.IsShown():
-            height /= 2
-        return (height, 1, 1, 1)
+        return self._preserve_aspect_ratio
 
-    #--------------------------------------------------------------------------
-    # Private API
-    #--------------------------------------------------------------------------
-    def _update_layout(self):
-        """ Synchronizes the drawing of the group box decorations with
-        the panel.
+    def setPreserveAspectRatio(self, preserve):
+        """ Set whether or not to preserve the image aspect ratio.
+
+        Parameters
+        ----------
+        preserve : bool
+            If True then the aspect ratio of the image will be preserved
+            if it is scaled to fit. Otherwise, the aspect ratio will be
+            ignored.
 
         """
-        if self._flat:
-            self._update_line_geometry()
-        else:
-            self._update_border_geometry()
-        self._update_title_geometry()
-        self.Refresh()
-
-    def _update_border_geometry(self):
-        """ Updates the geometry of the border.
-
-        """
-        width, height = self.GetSizeTuple()
-        self._border.SetSizeWH(width, height)
-
-    def _update_line_geometry(self):
-        """ Updates the geometry of the line.
-
-        """
-        y = self._label_size.GetHeight() / 2
-        width, _ = self.GetSizeTuple()
-        self._line.SetDimensions(0, y, width, 2)
-
-    def _update_title_geometry(self):
-        """ Updates the geometry of the title.
-
-        """
-        label = self._label
-        flat = self._flat
-        align = self._title_alignment
-        text_width, _ = self._label_size
-        width, _ = self.GetSizeTuple()
-        # These offsets are determined empirically to look similar
-        # in form to Qt on Windows
-        if align == wx.ALIGN_LEFT:
-            x = 0 if flat else 8
-            label.Move((x, 0))
-        elif align == wx.ALIGN_RIGHT:
-            right = width
-            right -= 0 if flat else 8
-            x = right - text_width
-            label.Move((x, 0))
-        elif align == wx.ALIGN_CENTER:
-            label.CenterOnParent(dir=wx.HORIZONTAL)
-        else:
-            raise ValueError('Invalid title alignment %s' % align)
+        self._preserve_aspect_ratio = preserve
+        self.update()
 
 
-class WxGroupBox(WxContainer, ProxyGroupBox):
-    """ A Wx implementation of an Enaml ProxyGroupBox.
+class QtImageView(QtControl, ProxyImageView):
+    """ A Qt implementation of an Enaml ProxyImageView.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(wxGroupBox)
+    widget = Typed(QImageView)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Creates the underlying QGroupBox control.
+        """ Create the underlying QImageView widget.
 
         """
-        self.widget = wxGroupBox(self.parent_widget())
+        self.widget = QImageView(self.parent_widget())
 
     def init_widget(self):
-        """ Initialize the underlying widget.
+        """ Initialize the underlying control.
 
         """
-        super(WxGroupBox, self).init_widget()
+        super(QtImageView, self).init_widget()
         d = self.declaration
-        self.set_title(d.title, cm_update=False)
-        self.set_flat(d.flat)
-        self.set_title_align(d.title_align)
+        self.set_image(d.image)
+        self.set_scale_to_fit(d.scale_to_fit)
+        self.set_allow_upscaling(d.allow_upscaling)
+        self.set_preserve_aspect_ratio(d.preserve_aspect_ratio)
 
     #--------------------------------------------------------------------------
-    # Layout Handling
+    # Widget Update Methods
     #--------------------------------------------------------------------------
-    @staticmethod
-    def margins_func(widget):
-        """ Get the current contents margins for the group box.
+    def set_image(self, image):
+        """ Set the image on the underlying widget.
 
         """
-        return widget.GetContentsMargins()
+        qpixmap = None
+        if image:
+            qimage = get_cached_qimage(image)
+            qpixmap = QPixmap.fromImage(qimage)
+        with self.geometry_guard():
+            self.widget.setPixmap(qpixmap)
 
-    #--------------------------------------------------------------------------
-    # ProxyGroupBox API
-    #--------------------------------------------------------------------------
-    def set_title(self, title, cm_update=True):
-        """ Update the title of the group box.
+    def set_scale_to_fit(self, scale):
+        """ Sets whether or not the image scales with the underlying
+        control.
 
         """
-        if not cm_update:
-            self.widget.SetTitle(title)
-            return
-        widget = self.widget
-        old_margins = widget.GetContentsMargins()
-        widget.SetTitle(title)
-        new_margins = widget.GetContentsMargins()
-        if old_margins != new_margins:
-            self.margins_updated()
+        self.widget.setScaledContents(scale)
 
-    def set_flat(self, flat):
-        """ Updates the flattened appearance of the group box.
+    def set_allow_upscaling(self, allow):
+        """ Sets whether or not the image will scale beyond its natural
+        size.
 
         """
-        self.widget.SetFlat(flat)
+        self.widget.setAllowUpscaling(allow)
 
-    def set_title_align(self, align):
-        """ Updates the alignment of the title of the group box.
+    def set_preserve_aspect_ratio(self, preserve):
+        """ Sets whether or not to preserve the aspect ratio of the
+        image when scaling.
 
         """
-        wx_align = WX_ALIGNMENTS[align]
-        self.widget.SetAlignment(wx_align)
+        self.widget.setPreserveAspectRatio(preserve)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_application.py` & `enaml-0.9.8/enaml/qt/qt_application.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2013, Nucleic Development Team.
+# Copyright (c) 2014, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-
 from atom.api import Typed
 
 from enaml.application import Application, ProxyResolver
 
-from .wx_deferred_caller import DeferredCall, TimedCall
-from .wx_factories import WX_FACTORIES
+from .QtCore import QThread
+from .QtGui import QApplication
+
+from .q_deferred_caller import deferredCall, timedCall
+from .qt_factories import QT_FACTORIES
+from .qt_mime_data import QtMimeData
 
 
-class WxApplication(Application):
-    """ A Wx implementation of an Enaml application.
+class QtApplication(Application):
+    """ A Qt implementation of an Enaml application.
 
-    A WxApplication uses the Wx toolkit to implement an Enaml UI that
+    A QtApplication uses the Qt toolkit to implement an Enaml UI that
     runs in the local process.
 
     """
     #: The private QApplication instance.
-    _wxapp = Typed(wx.App)
+    _qapp = Typed(QApplication)
 
     def __init__(self):
-        """ Initialize a WxApplication.
+        """ Initialize a QtApplication.
 
         """
-        super(WxApplication, self).__init__()
-        self._wxapp = wx.GetApp() or wx.PySimpleApp()
-        self.resolver = ProxyResolver(factories=WX_FACTORIES)
+        super(QtApplication, self).__init__()
+        self._qapp = QApplication.instance() or QApplication([])
+        self.resolver = ProxyResolver(factories=QT_FACTORIES)
 
     #--------------------------------------------------------------------------
     # Abstract API Implementation
     #--------------------------------------------------------------------------
     def start(self):
         """ Start the application's main event loop.
 
         """
-        app = self._wxapp
-        if not app.IsMainLoopRunning():
-            app.MainLoop()
+        app = self._qapp
+        if not getattr(app, '_in_event_loop', False):
+            app._in_event_loop = True
+            app.exec_()
+            app._in_event_loop = False
 
     def stop(self):
         """ Stop the application's main event loop.
 
         """
-        app = self._wxapp
-        if app.IsMainLoopRunning():
-            app.Exit()
+        app = self._qapp
+        app.exit()
+        app._in_event_loop = False
 
     def deferred_call(self, callback, *args, **kwargs):
         """ Invoke a callable on the next cycle of the main event loop
         thread.
 
         Parameters
         ----------
@@ -62,15 +66,15 @@
             The callable object to execute at some point in the future.
 
         *args, **kwargs
             Any additional positional and keyword arguments to pass to
             the callback.
 
         """
-        DeferredCall(callback, *args, **kwargs)
+        deferredCall(callback, *args, **kwargs)
 
     def timed_call(self, ms, callback, *args, **kwargs):
         """ Invoke a callable on the main event loop thread at a
         specified time in the future.
 
         Parameters
         ----------
@@ -82,19 +86,30 @@
             The callable object to execute at some point in the future.
 
         *args, **kwargs
             Any additional positional and keyword arguments to pass to
             the callback.
 
         """
-        TimedCall(ms, callback, *args, **kwargs)
+        timedCall(ms, callback, *args, **kwargs)
 
     def is_main_thread(self):
         """ Indicates whether the caller is on the main gui thread.
 
         Returns
         -------
         result : bool
             True if called from the main gui thread. False otherwise.
 
         """
-        return wx.Thread_IsMain()
+        return QThread.currentThread() == self._qapp.thread()
+
+    def create_mime_data(self):
+        """ Create a new mime data object to be filled by the user.
+
+        Returns
+        -------
+        result : QtMimeData
+            A concrete implementation of the MimeData class.
+
+        """
+        return QtMimeData()
```

### Comparing `enaml-0.9.7/enaml/wx/wx_date_selector.py` & `enaml-0.9.8/enaml/qt/qt_time_selector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,104 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-
 from atom.api import Typed
 
-from enaml.widgets.date_selector import ProxyDateSelector
+from enaml.widgets.time_selector import ProxyTimeSelector
+
+from .QtGui import QTimeEdit
 
-from .wx_bounded_date import (
-    WxBoundedDate, CHANGED_GUARD, as_wx_date, as_py_date
-)
+from .qt_bounded_time import QtBoundedTime, CHANGED_GUARD
 
 
-class WxDateSelector(WxBoundedDate, ProxyDateSelector):
-    """ A Wx implementation of an Enaml ProxyDateSelector.
+class QtTimeSelector(QtBoundedTime, ProxyTimeSelector):
+    """ A Qt implementation of an Enaml ProxyTimeSelector.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(wx.DatePickerCtrl)
+    widget = Typed(QTimeEdit)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the wx.DatePickerCtrl widget.
+        """ Create the QTimeEdit widget.
 
         """
-        self.widget = wx.DatePickerCtrl(self.parent_widget())
+        self.widget = QTimeEdit(self.parent_widget())
 
     def init_widget(self):
         """ Initialize the widget.
 
         """
-        super(WxDateSelector, self).init_widget()
+        super(QtTimeSelector, self).init_widget()
         d = self.declaration
-        self.set_date_format(d.date_format)
-        self.set_calendar_popup(d.calendar_popup)
-        self.widget.Bind(wx.EVT_DATE_CHANGED, self.on_date_changed)
+        self.set_time_format(d.time_format)
+        self.widget.timeChanged.connect(self.on_time_changed)
 
     #--------------------------------------------------------------------------
     # Abstract API Implementation
     #--------------------------------------------------------------------------
-    def get_date(self):
-        """ Return the current date in the control.
+    def get_time(self):
+        """ Return the current time in the control.
 
         Returns
         -------
-        result : date
-            The current control date as a date object.
+        result : time
+            The current control time as a time object.
 
         """
-        return as_py_date(self.widget.GetValue())
+        return self.widget.time().toPython()
 
-    def set_minimum(self, date):
-        """ Set the widget's minimum date.
+    def set_minimum(self, time):
+        """ Set the widget's minimum time.
 
         Parameters
         ----------
-        date : date
-            The date object to use for setting the minimum date.
+        time : time
+            The time object to use for setting the minimum time.
 
         """
-        widget = self.widget
-        widget.SetRange(as_wx_date(date), widget.GetUpperLimit())
+        self.widget.setMinimumTime(time)
 
-
-    def set_maximum(self, date):
-        """ Set the widget's maximum date.
+    def set_maximum(self, time):
+        """ Set the widget's maximum time.
 
         Parameters
         ----------
-        date : date
-            The date object to use for setting the maximum date.
+        time : time
+            The time object to use for setting the maximum time.
 
         """
-        widget = self.widget
-        widget.SetRange(widget.GetLowerLimit(), as_wx_date(date))
+        self.widget.setMaximumTime(time)
 
-    def set_date(self, date):
-        """ Set the widget's current date.
+    def set_time(self, time):
+        """ Set the widget's current time.
 
         Parameters
         ----------
-        date : date
-            The date object to use for setting the date.
+        time : time
+            The time object to use for setting the date.
 
         """
         self._guard |= CHANGED_GUARD
         try:
-            self.widget.SetValue(as_wx_date(date))
+            self.widget.setTime(time)
         finally:
             self._guard &= ~CHANGED_GUARD
 
-    def set_date_format(self, format):
-        """ Set the widget's date format.
+    def set_time_format(self, format):
+        """ Set the widget's time format.
 
         Parameters
         ----------
         format : string
             A Python time formatting string.
 
-        .. note:: Changing the format on wx is not supported.
-                  See http://trac.wxwidgets.org/ticket/10988
-
-        """
-        pass
-
-    def set_calendar_popup(self, popup):
-        """ This is not supported on Wx.
-
         """
-        pass
+        # XXX make sure Python's and Qt's format strings are the
+        # same, or convert between the two.
+        self.widget.setDisplayFormat(format)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_menu_bar.py` & `enaml-0.9.8/enaml/qt/qt_menu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,268 +1,253 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-
 from atom.api import Typed
 
-from enaml.widgets.menu_bar import ProxyMenuBar
+from enaml.widgets.menu import ProxyMenu
+
+from .QtCore import Qt
+from .QtGui import QMenu, QCursor
 
-from .wx_menu import WxMenu, EVT_MENU_CHANGED
-from .wx_toolkit_object import WxToolkitObject
+from .qt_action import QtAction
+from .qt_action_group import QtActionGroup
+from .qt_toolkit_object import QtToolkitObject
+from .qt_widget import QtWidget
 
 
-class wxMenuBar(wx.MenuBar):
-    """ A wx.MenuBar subclass which exposes a more convenient api for
-    working with wxMenu children.
+class QCustomMenu(QMenu):
+    """ A custom subclass of QMenu which adds some convenience apis.
 
     """
     def __init__(self, *args, **kwargs):
-        """ Initialize a wxMenuBar.
+        """ Initialize a QCustomMenu.
 
         Parameters
         ----------
         *args, **kwargs
             The positional and keyword arguments needed to initialize
-            a wx.MenuBar.
+            a QMenu.
 
         """
-        super(wxMenuBar, self).__init__(*args, **kwargs)
-        self._menus = []
-        self._visible_menus = []
-        self._enabled = True
+        super(QCustomMenu, self).__init__(*args, **kwargs)
+        self._is_context_menu = False
 
     #--------------------------------------------------------------------------
     # Private API
     #--------------------------------------------------------------------------
-    def OnMenuChanged(self, event):
-        """ The event handler for the EVT_MENU_CHANGED event.
+    def _onShowContextMenu(self, pos):
+        """ A private signal handler for displaying the context menu.
 
-        This event handler will synchronize the menu changes with
-        the menu bar.
+        This handler is connected to the context menu requested signal
+        on the parent widget when this menu is marked as a context
+        menu.
 
         """
-        event.Skip()
-        if self.IsAttached():
-            menu = event.GetEventObject()
-
-            # First, check for a visibility change. This requires adding
-            # or removing the menu from the menu bar.
-            visible = menu.IsVisible()
-            was_visible = menu in self._visible_menus
-            if visible != was_visible:
-                if visible:
-                    index = self._menus.index(menu)
-                    index = min(index, len(self._visible_menus))
-                    self._visible_menus.insert(index, menu)
-                    self.Insert(index, menu, menu.GetTitle())
-                    self.EnableTop(index, menu.IsEnabled())
-                else:
-                    index = self._visible_menus.index(menu)
-                    self._visible_menus.pop(index)
-                    self.Remove(index)
-                return
-
-            # If the menu isn't visible, there's nothing to do.
-            if not visible:
-                return
-
-            # For all other state, the menu can be updated in-place.
-            index = self._visible_menus.index(menu)
-            self.SetMenuLabel(index, menu.GetTitle())
-            self.EnableTop(index, menu.IsEnabled())
+        parent = self.parentWidget()
+        if parent is not None:
+            global_pos = parent.mapToGlobal(pos)
+            self.exec_(global_pos)
 
     #--------------------------------------------------------------------------
     # Public API
     #--------------------------------------------------------------------------
-    def IsEnabled(self):
-        """ Get whether or not the menu bar is enabled.
+    def isContextMenu(self):
+        """ Whether this menu acts as a context menu for its parent.
 
         Returns
         -------
         result : bool
-            Whether or not the menu bar is enabled.
-
-        """
-        return self._enabled
-
-    def SetEnabled(self, enabled):
-        """ Set whether or not the menu bar is enabled.
-
-        Parameters
-        ----------
-        enabled : bool
-            Whether or not the menu bar is enabled.
-
-        """
-        # Wx does not provide a means for disabling the entire menu
-        # bar, so we must do it manually by disabling each menu.
-        if self._enabled != enabled:
-            self._enabled = enabled
-            for menu in self._menus:
-                menu._SetBarEnabled(enabled)
-
-    def AddMenu(self, menu):
-        """ Add a wxMenu to the menu bar.
-
-        If the menu already exists in the menu bar, this is a no-op.
-
-        Parameters
-        ----------
-        menu : wxMenu
-            The wxMenu instance to add to the menu bar.
+            True if this menu acts as a context menu, False otherwise.
 
         """
-        self.InsertMenu(None, menu)
-
-    def InsertMenu(self, before, menu):
-        """ Insert a wxMenu into the menu bar.
+        return self._is_context_menu
 
-        If the menu already exists in the menu bar, this is a no-op.
+    def setContextMenu(self, context):
+        """ Set whether this menu acts as a context menu for its parent.
 
         Parameters
         ----------
-        before : wxMenu
-            The menu before which to insert the given menu.
-
-        menu : wxMenu
-            The menu to insert into the menu bar.
+        context : bool
+            True if this menu should act as a context menu, False
+            otherwise.
 
         """
-        menus = self._menus
-        if menu not in menus:
-            if before in menus:
-                index = menus.index(before)
-            else:
-                index = len(menus)
-            menus.insert(index, menu)
-            if menu.IsVisible():
-                max_index = len(self._visible_menus)
-                index = min(index, max_index)
-                self._visible_menus.insert(index, menu)
-                self.Insert(index, menu, menu.GetTitle())
-            menu.Bind(EVT_MENU_CHANGED, self.OnMenuChanged)
-            menu._SetBarEnabled(self._enabled)
-
-    def RemoveMenu(self, menu):
-        """ Remove a wxMenu from the menu bar.
+        old_context = self._is_context_menu
+        self._is_context_menu = context
+        if old_context != context:
+            parent = self.parentWidget()
+            if parent is not None:
+                handler = self._onShowContextMenu
+                if context:
+                    parent.setContextMenuPolicy(Qt.CustomContextMenu)
+                    parent.customContextMenuRequested.connect(handler)
+                else:
+                    parent.setContextMenuPolicy(Qt.DefaultContextMenu)
+                    parent.customContextMenuRequested.disconnect(handler)
 
-        If the menu does not exist in the menu bar, this is a no-op.
+    def removeActions(self, actions):
+        """ Remove the given actions from the menu.
 
         Parameters
         ----------
-        menu : wxMenu
-            The menu to remove from the menu bar.
+        actions : iterable
+            An iterable of QActions to remove from the menu.
 
         """
-        menus = self._menus
-        if menu in menus:
-            menus.remove(menu)
-            menu.Unbind(EVT_MENU_CHANGED, handler=self.OnMenuChanged)
-            visible_menus = self._visible_menus
-            if menu in visible_menus:
-                index = visible_menus.index(menu)
-                visible_menus.remove(menu)
-                self.Remove(index)
-
-    def Update(self):
-        """ A method which can be called to update the menu bar.
-
-        Calling this method will manually refresh the state of the
-        items in the menu bar. This is useful to call just after
-        attaching the menu bar to a frame, since the menu bar state
-        cannot be updated prior to being attached.
-
-        """
-        if self.IsAttached():
-            for index, menu in enumerate(self._visible_menus):
-                self.SetMenuLabel(index, menu.GetTitle())
-                if not menu.IsEnabled():
-                    self.EnableTop(index, False)
+        remove = self.removeAction
+        for action in actions:
+            remove(action)
 
 
-class WxMenuBar(WxToolkitObject, ProxyMenuBar):
-    """ A Wx implementation of an Enaml ProxyMenuBar.
+class QtMenu(QtToolkitObject, ProxyMenu):
+    """ A Qt implementation of an Enaml ProxyMenu.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(wxMenuBar)
+    widget = Typed(QCustomMenu)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying menu bar widget.
+        """ Create the underlying menu widget.
 
         """
-        # Wx behaves better when creating the menu bar without a parent.
-        self.widget = wxMenuBar()
+        self.widget = QCustomMenu(self.parent_widget())
 
-    def init_layout(self):
-        """ Initialize the layout for the menu bar.
+    def init_widget(self):
+        """ Initialize the widget.
 
         """
-        super(WxMenuBar, self).init_layout()
-        widget = self.widget
-        for child in self.children():
-            if isinstance(child, WxMenu):
-                widget.AddMenu(child.widget)
+        super(QtMenu, self).init_widget()
+        d = self.declaration
+        self.set_title(d.title)
+        self.set_enabled(d.enabled)
+        self.set_visible(d.visible)
+        self.set_context_menu(d.context_menu)
 
-    def destroy(self):
-        """ A reimplemented destructor.
-
-        This destructor simply drops the reference to the menu bar and
-        the enaml declaration and clears the menus in the menu bar.
-        Destroying it will cause wx to segfault.
+    def init_layout(self):
+        """ Initialize the layout of the widget.
 
         """
-        if self.widget:
-            self.widget.SetMenus([])
-        del self.widget
-        del self.declaration
+        super(QtMenu, self).init_layout()
+        widget = self.widget
+        for child in self.children():
+            if isinstance(child, QtMenu):
+                widget.addMenu(child.widget)
+            elif isinstance(child, QtAction):
+                widget.addAction(child.widget)
+            elif isinstance(child, QtActionGroup):
+                widget.addActions(child.actions())
+            elif isinstance(child, QtWidget):
+                widget.addAction(child.get_action(True))
 
     #--------------------------------------------------------------------------
     # Child Events
     #--------------------------------------------------------------------------
-    def find_next_menu(self, child):
-        """ Get the wxMenu instance which follows the child.
+    def find_next_action(self, child):
+        """ Get the QAction instance which follows the child.
 
         Parameters
         ----------
-        child : WxMenu
-            The child menu of interest.
+        child : QtToolkitObject
+            The child of interest.
 
         Returns
         -------
-        result : wxMenu or None
-            The wxMenu which comes immediately after the actions of the
+        result : QAction or None
+            The QAction which comes immediately after the actions of the
             given child, or None if no actions follow the child.
 
         """
         found = False
         for dchild in self.children():
             if found:
-                if isinstance(dchild, WxMenu):
+                if isinstance(dchild, QtMenu):
+                    return dchild.widget.menuAction()
+                elif isinstance(dchild, QtAction):
                     return dchild.widget
+                elif isinstance(dchild, QtActionGroup):
+                    acts = dchild.actions()
+                    if len(acts) > 0:
+                        return acts[0]
+                elif isinstance(dchild, QtWidget):
+                    action = dchild.get_action(False)
+                    if action is not None:
+                        return action
             else:
                 found = dchild is child
 
     def child_added(self, child):
-        """ Handle the child added event for a WxMenuBar.
+        """ Handle the child added event for a QtMenu.
 
         """
-        super(WxMenuBar, self).child_added(child)
-        if isinstance(child, WxMenu):
-            before = self.find_next_menu(child)
-            self.widget.InsertMenu(before, child.widget)
+        super(QtMenu, self).child_added(child)
+        if isinstance(child, QtMenu):
+            before = self.find_next_action(child)
+            self.widget.insertMenu(before, child.widget)
+        elif isinstance(child, QtAction):
+            before = self.find_next_action(child)
+            self.widget.insertAction(before, child.widget)
+        elif isinstance(child, QtActionGroup):
+            before = self.find_next_action(child)
+            self.widget.insertActions(before, child.actions())
+        elif isinstance(child, QtWidget):
+            before = self.find_next_action(child)
+            self.widget.insertAction(before, child.get_action(True))
 
     def child_removed(self, child):
-        """ Handle the child removed event for a WxMenuBar.
+        """  Handle the child removed event for a QtMenu.
+
+        """
+        super(QtMenu, self).child_removed(child)
+        if isinstance(child, QtMenu):
+            self.widget.removeAction(child.widget.menuAction())
+        elif isinstance(child, QtAction):
+            self.widget.removeAction(child.widget)
+        elif isinstance(child, QtActionGroup):
+            self.widget.removeActions(child.actions())
+        elif isinstance(child, QtWidget):
+            self.widget.removeAction(child.get_action(False))
+
+    #--------------------------------------------------------------------------
+    # ProxyMenu API
+    #--------------------------------------------------------------------------
+    def set_title(self, title):
+        """ Set the title of the underlying widget.
+
+        """
+        self.widget.setTitle(title)
+
+    def set_visible(self, visible):
+        """ Set the visibility on the underlying widget.
+
+        """
+        self.widget.menuAction().setVisible(visible)
+
+    def set_enabled(self, enabled):
+        """ Set the enabled state of the widget.
+
+        """
+        self.widget.setEnabled(enabled)
+
+    def set_context_menu(self, context):
+        """ Set whether or not the menu is a context menu.
+
+        """
+        self.widget.setContextMenu(context)
+
+    def popup(self):
+        """ Popup the menu over the current mouse location.
+
+        """
+        self.widget.exec_(QCursor.pos())
+
+    def close(self):
+        """ Close the underlying menu.
 
         """
-        super(WxMenuBar, self).child_removed(child)
-        if isinstance(child, WxMenu):
-            self.widget.RemoveMenu(child.widget)
+        self.widget.close()
```

### Comparing `enaml-0.9.7/enaml/wx/wx_scroll_area.py` & `enaml-0.9.8/enaml/qt/qt_scroll_area.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,233 +1,221 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-
-from atom.api import Typed
+from atom.api import Typed, Value
 
 from enaml.widgets.scroll_area import ProxyScrollArea
 
-from .wx_container import WxContainer
-from .wx_frame import WxFrame
-from .wx_single_widget_sizer import wxSingleWidgetSizer
-
-
-# The 'always_on' scroll policy is not supported on wx, because it
-# requires setting a window style flag which does not dynamically
-# toggle in a reliable fashion. Since we only support 'off' or 'auto'
-# it's easiest to use this mapping to convert straight from policy
-# values into a respective scroll rate. A rate of Zero causes wx not
-# to show the scroll bar. A positive rate indicates to scroll that many
-# pixels per event. We set the rate to 1 to have smooth scrolling. Wx
-# doesn't make a distinction between scroll events caused by the mouse
-# or scrollbar and those caused by clicking the scroll buttons (ala qt),
-# and thus this rate applies the same to all of those events. Since we
-# expect that clicking on a scroll button happens much more infrequently
-# than scrolling by dragging the scroll bar, we opt for a lower rate
-# in order to get smooth drag scrolling and sacrifice some usability
-# on the scroll buttons.
-SCROLLBAR_MAP = {
-    'as_needed': 1,
-    'always_off': 0,
-    'always_on': 1,
-}
-
-
-class wxScrollAreaSizer(wxSingleWidgetSizer):
-    """ A wxSingleWidgetSizer subclass which makes adjusts the min
-    size to account for a 2 pixel error in Wx.
+from .QtCore import Qt, QEvent, QSize, QRect, QPoint, Signal
+from .QtGui import QApplication, QScrollArea, QPainter, QPalette
 
-    """
-    def CalcMin(self):
-        """ Returns the minimum size for the area owned by the sizer.
-
-        Returns
-        -------
-        result : wxSize
-            The wx size representing the minimum area required by the
-            sizer.
-
-        """
-        # The effective min size computation is correct, but the wx
-        # scrolled window interprets it with an error of 2px. That
-        # is we need to make wx think that the min size is 2px smaller
-        # than it actually is so that scroll bars should and hide at
-        # the appropriate sizes.
-        res = super(wxScrollAreaSizer, self).CalcMin()
-        if res.IsFullySpecified():
-            res.width -= 2
-            res.height -= 2
-        return res
+from .qt_container import QtContainer
+from .qt_frame import QtFrame
 
-    def RecalcSizes(self):
-        """ Resizes the child to fit the available space of the window.
 
-        This takes into account the maximum allowed size of the widget.
+POLICIES = {
+    'as_needed': Qt.ScrollBarAsNeeded,
+    'always_off': Qt.ScrollBarAlwaysOff,
+    'always_on': Qt.ScrollBarAlwaysOn
+}
 
-        """
-        widget = self.GetWidget()
-        if widget:
-            size = self.GetSize()
-            size.DecTo(self.CalcMax())
-            widget.SetSize(size)
 
+class QCustomScrollArea(QScrollArea):
+    """ A custom QScrollArea for use with the QtScrollArea.
 
-class wxScrollArea(wx.ScrolledWindow):
-    """ A custom wx.ScrolledWindow which is suits Enaml's use case.
+    This subclass fixes some bugs related to size hints.
 
     """
-    #: The internal best size. The same as QAbstractScrollArea.
-    _best_size = wx.Size(256, 192)
-
-    def __init__(self, *args, **kwargs):
-        """ Initialize a wxScrollArea.
-
-        Parameters
-        ----------
-        *args, **kwargs
-            The positional and keyword arguments needed to initialize
-            a wxScrolledWindow.
-
-        """
-        super(wxScrollArea, self).__init__(*args, **kwargs)
-        self._scroll_widget = None
-        self.SetSizer(wxScrollAreaSizer())
-
-    def GetBestSize(self):
-        """ An overridden parent class method which returns a sensible
-        best size.
-
-        The default wx implementation returns a best size of (16, 16)
-        on Windows; far too small to be useful. So, we just adopt the
-        size hint of (256, 192) used in Qt's QAbstractScrollArea.
-
-        """
-        return self._best_size
-
-    def GetScrollWidget(self):
-        """ Get the scroll widget for this scroll area.
-
-        Returns
-        -------
-        results : wxWindow
-            The wxWindow being scrolled by this scroll area.
-
-        """
-        return self._scroll_widget
+    #: A signal emitted when a LayoutRequest event is posted to the
+    #: scroll area. This will typically occur when the size hint of
+    #: the scroll area is no longer valid.
+    layoutRequested = Signal()
+
+    #: A private internally cached size hint.
+    _size_hint = QSize()
+
+    def event(self, event):
+        """ A custom event handler for the scroll area.
+
+        This handler dispatches layout requests and paints the empty
+        corner between the scroll bars.
+
+        """
+        res = super(QCustomScrollArea, self).event(event)
+        event_t = event.type()
+        if event_t == QEvent.Paint:
+            # Fill in the empty corner area with the app window color.
+            color = QApplication.palette().color(QPalette.Window)
+            tl = self.viewport().geometry().bottomRight()
+            fw = self.frameWidth()
+            br = self.rect().bottomRight() - QPoint(fw, fw)
+            QPainter(self).fillRect(QRect(tl, br), color)
+        elif event_t == QEvent.LayoutRequest:
+            self._size_hint = QSize()
+            self.layoutRequested.emit()
+        return res
 
-    def SetScrollWidget(self, widget):
-        """ Set the scroll widget for this scroll area.
+    def setWidget(self, widget):
+        """ Set the widget for this scroll area.
 
-        Parameters
-        ----------
-        widget : wxWindow
-            The wxWindow which should be scrolled by this area.
+        This is a reimplemented parent class method which invalidates
+        the cached size hint before setting the widget.
 
         """
-        self._scroll_widget = widget
-        self.GetSizer().Add(widget)
+        self._size_hint = QSize()
+        self.takeWidget()  # Let Python keep ownership of the old widget
+        super(QCustomScrollArea, self).setWidget(widget)
+
+    def sizeHint(self):
+        """ Get the size hint for the scroll area.
+
+        This reimplemented method fixes a Qt bug where the size hint
+        is not updated after the scroll widget is first shown. The
+        bug is documented on the Qt bug tracker:
+        https://bugreports.qt-project.org/browse/QTBUG-10545
+
+        """
+        # This code is ported directly from QScrollArea.cpp but instead
+        # of caching the size hint of the scroll widget, it caches the
+        # size hint for the entire scroll area, and invalidates it when
+        # the widget is changed or it receives a LayoutRequest event.
+        hint = self._size_hint
+        if hint.isValid():
+            return QSize(hint)
+        fw = 2 * self.frameWidth()
+        hint = QSize(fw, fw)
+        font_height = self.fontMetrics().height()
+        widget = self.widget()
+        if widget is not None:
+            if self.widgetResizable():
+                hint += widget.sizeHint()
+            else:
+                hint += widget.size()
+        else:
+            hint += QSize(12 * font_height, 8 * font_height)
+        if self.verticalScrollBarPolicy() == Qt.ScrollBarAlwaysOn:
+            vbar = self.verticalScrollBar()
+            hint.setWidth(hint.width() + vbar.sizeHint().width())
+        if self.horizontalScrollBarPolicy() == Qt.ScrollBarAlwaysOn:
+            hbar = self.horizontalScrollBar()
+            hint.setHeight(hint.height() + hbar.sizeHint().height())
+        hint = hint.boundedTo(QSize(36 * font_height, 24 * font_height))
+        self._size_hint = hint
+        return QSize(hint)
 
 
-class WxScrollArea(WxFrame, ProxyScrollArea):
-    """ A Wx implementation of an Enaml ScrollArea.
+class QtScrollArea(QtFrame, ProxyScrollArea):
+    """ A Qt implementation of an Enaml ProxyScrollArea.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(wxScrollArea)
+    widget = Typed(QCustomScrollArea)
 
+    #: A private cache of the old size hint for the scroll area.
+    _old_hint = Value()
+
+    #--------------------------------------------------------------------------
+    # Initialization API
+    #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying wxScrolledWindow widget.
+        """ Create the underlying QScrollArea widget.
 
         """
-        style = wx.HSCROLL | wx.VSCROLL | wx.BORDER_SIMPLE
-        self.widget = wxScrollArea(self.parent_widget(), style=style)
+        self.widget = QCustomScrollArea(self.parent_widget())
 
     def init_widget(self):
         """ Initialize the underlying widget.
 
         """
-        super(WxScrollArea, self).init_widget()
+        super(QtScrollArea, self).init_widget()
         d = self.declaration
         self.set_horizontal_policy(d.horizontal_policy)
         self.set_vertical_policy(d.vertical_policy)
         self.set_widget_resizable(d.widget_resizable)
 
     def init_layout(self):
-        """ Handle the layout initialization for the scroll area.
+        """ Initialize the layout of the underlying widget.
 
         """
-        super(WxScrollArea, self).init_layout()
-        self.widget.SetScrollWidget(self.scroll_widget())
+        super(QtScrollArea, self).init_layout()
+        widget = self.widget
+        widget.setWidget(self.scroll_widget())
+        widget.layoutRequested.connect(self.on_layout_requested)
 
     #--------------------------------------------------------------------------
     # Utility Methods
     #--------------------------------------------------------------------------
     def scroll_widget(self):
         """ Find and return the scroll widget child for this widget.
 
         """
         w = self.declaration.scroll_widget()
         if w is not None:
-            return w.proxy.widget or None
+            return w.proxy.widget
 
     #--------------------------------------------------------------------------
     # Child Events
     #--------------------------------------------------------------------------
     def child_added(self, child):
-        """ Handle the child added event for a WxScrollArea.
+        """ Handle the child added event for a QtScrollArea.
 
         """
-        super(WxScrollArea, self).child_added(child)
-        if isinstance(child, WxContainer):
-            self.widget.SetScrollWidget(self.scroll_widget())
+        super(QtScrollArea, self).child_added(child)
+        if isinstance(child, QtContainer):
+            self.widget.setWidget(self.scroll_widget())
 
     def child_removed(self, child):
-        """ Handle the child removed event for a WxScrollArea.
+        """ Handle the child removed event for a QtScrollArea.
+
+        """
+        super(QtScrollArea, self).child_removed(child)
+        if isinstance(child, QtContainer):
+            self.widget.setWidget(self.scroll_widget())
+
+    #--------------------------------------------------------------------------
+    # Signal Handlers
+    #--------------------------------------------------------------------------
+    def on_layout_requested(self):
+        """ Handle the `layoutRequested` signal from the QScrollArea.
 
         """
-        super(WxScrollArea, self).child_removed(child)
-        if isinstance(child, WxContainer):
-            self.widget.SetScrollWidget(self.scroll_widget())
+        new_hint = self.widget.sizeHint()
+        if new_hint != self._old_hint:
+            self._old_hint = new_hint
+            self.geometry_updated()
 
     #--------------------------------------------------------------------------
     # Overrides
     #--------------------------------------------------------------------------
     def replace_constraints(self, old_cns, new_cns):
-        """ A reimplemented WxConstraintsWidget layout method.
+        """ A reimplemented QtConstraintsWidget layout method.
 
         Constraints layout may not cross the boundary of a ScrollArea,
         so this method is no-op which stops the layout propagation.
 
         """
         pass
 
     #--------------------------------------------------------------------------
     # ProxyScrollArea API
     #--------------------------------------------------------------------------
     def set_horizontal_policy(self, policy):
         """ Set the horizontal scrollbar policy of the widget.
 
         """
-        horiz = SCROLLBAR_MAP[policy]
-        vert = SCROLLBAR_MAP[self.declaration.vertical_policy]
-        self.widget.SetScrollRate(horiz, vert)
+        self.widget.setHorizontalScrollBarPolicy(POLICIES[policy])
 
     def set_vertical_policy(self, policy):
         """ Set the vertical scrollbar policy of the widget.
 
         """
-        horiz = SCROLLBAR_MAP[self.declaration.horizontal_policy]
-        vert = SCROLLBAR_MAP[policy]
-        self.widget.SetScrollRate(horiz, vert)
+        self.widget.setVerticalScrollBarPolicy(POLICIES[policy])
 
     def set_widget_resizable(self, resizable):
         """ Set whether or not the scroll widget is resizable.
 
-        This is not supported on Wx.
-
         """
-        pass
+        self.widget.setWidgetResizable(resizable)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_widget.py` & `enaml-0.9.8/enaml/qt/qt_spin_box.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,168 +1,133 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
+from atom.api import Int, Typed
 
-from atom.api import Typed
+from enaml.widgets.spin_box import ProxySpinBox
 
-from enaml.widgets.widget import ProxyWidget
+from .QtGui import QSpinBox
 
-from .wx_layout_request import wxEvtLayoutRequested
-from .wx_resource_helpers import get_cached_wxcolor, get_cached_wxfont
-from .wx_toolkit_object import WxToolkitObject
+from .qt_control import QtControl
 
 
-class WxWidget(WxToolkitObject, ProxyWidget):
-    """ A Wx implementation of an Enaml ProxyWidget.
+#: Cyclic guard flag
+VALUE_FLAG = 0x1
+
+
+class QtSpinBox(QtControl, ProxySpinBox):
+    """ A Qt implementation of an Enaml SpinBox.
 
     """
-    #: A reference to the toolkit widget created by the proxy.
-    widget = Typed(wx.Window)
+    #: A reference to the widget created by the proxy.
+    widget = Typed(QSpinBox)
+
+    #: Cyclic guard flags
+    _guard = Int(0)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Creates the underlying wx.Window widget.
+        """ Create the underlying QSpinBox widget.
 
         """
-        self.widget = wx.Window(self.parent_widget())
+        widget = QSpinBox(self.parent_widget())
+        widget.setKeyboardTracking(False)
+        self.widget = widget
 
     def init_widget(self):
         """ Initialize the underlying widget.
 
         """
-        super(WxWidget, self).init_widget()
+        super(QtSpinBox, self).init_widget()
         d = self.declaration
-        if d.background:
-            self.set_background(d.background)
-        if d.foreground:
-            self.set_foreground(d.foreground)
-        if d.font:
-            self.set_font(d.font)
-        if -1 not in d.minimum_size:
-            self.set_minimum_size(d.minimum_size)
-        if -1 not in d.maximum_size:
-            self.set_maximum_size(d.maximum_size)
-        if d.tool_tip:
-            self.set_tool_tip(d.tool_tip)
-        if d.status_tip:
-            self.set_status_tip(d.status_tip)
-        self.set_enabled(d.enabled)
-        self.set_visible(d.visible)
+        self.set_maximum(d.maximum)
+        self.set_minimum(d.minimum)
+        self.set_value(d.value)
+        self.set_prefix(d.prefix)
+        self.set_suffix(d.suffix)
+        self.set_special_value_text(d.special_value_text)
+        self.set_single_step(d.single_step)
+        self.set_read_only(d.read_only)
+        self.set_wrapping(d.wrapping)
+        self.widget.valueChanged.connect(self.on_value_changed)
 
     #--------------------------------------------------------------------------
-    # Public API
+    # Signal Handlers
     #--------------------------------------------------------------------------
-    def post_wx_layout_request(self):
-        """ Post a wx layout request event to this widget's parent.
-
-        This method should be called when the geometry of the widget has
-        changed and the layout system should update the layout. This will
-        post a wxEvtLayoutRequested event to the parent of this widget.
+    def on_value_changed(self):
+        """ The signal handler for the 'valueChanged' signal.
 
         """
-        widget = self.widget
-        if widget:
-            parent = widget.GetParent()
-            if parent:
-                event = wxEvtLayoutRequested(widget.GetId())
-                wx.PostEvent(parent, event)
+        if not self._guard & VALUE_FLAG:
+            self._guard |= VALUE_FLAG
+            try:
+                self.declaration.value = self.widget.value()
+            finally:
+                self._guard &= ~VALUE_FLAG
 
     #--------------------------------------------------------------------------
-    # ProxyWidget API
+    # ProxySpinBox API
     #--------------------------------------------------------------------------
-    def set_minimum_size(self, min_size):
-        """ Sets the minimum size on the underlying widget.
-
-        """
-        self.widget.SetMinSize(wx.Size(*min_size))
-
-    def set_maximum_size(self, max_size):
-        """ Sets the maximum size on the underlying widget.
-
-        """
-        self.widget.SetMaxSize(wx.Size(*max_size))
-
-    def set_enabled(self, enabled):
-        """ Set the enabled state on the underlying widget.
-
-        """
-        self.widget.Enable(enabled)
-
-    def set_visible(self, visible):
-        """ Set the visibility state on the underlying widget.
+    def set_maximum(self, maximum):
+        """ Set the widget's maximum value.
 
         """
-        self.widget.Show(visible)
+        self.widget.setMaximum(maximum)
 
-    def set_background(self, background):
-        """ Set the background color on the underlying widget.
+    def set_minimum(self, minimum):
+        """ Set the widget's minimum value.
 
         """
-        if background is None:
-            wxcolor = wx.NullColour
-        else:
-            wxcolor = get_cached_wxcolor(background)
-        widget = self.widget
-        widget.SetBackgroundColour(wxcolor)
-        widget.Refresh()
+        self.widget.setMinimum(minimum)
 
-    def set_foreground(self, foreground):
-        """ Set the foreground color on the underlying widget.
+    def set_value(self, value):
+        """ Set the spin box's value.
 
         """
-        if foreground is None:
-            wxcolor = wx.NullColour
-        else:
-            wxcolor = get_cached_wxcolor(foreground)
-        widget = self.widget
-        widget.SetForegroundColour(wxcolor)
-        widget.Refresh()
+        if not self._guard & VALUE_FLAG:
+            self._guard |= VALUE_FLAG
+            try:
+                self.widget.setValue(value)
+            finally:
+                self._guard &= ~VALUE_FLAG
 
-    def set_font(self, font):
-        """ Set the font on the underlying widget.
+    def set_prefix(self, prefix):
+        """ Set the prefix for the spin box.
 
         """
-        if font is not None:
-            wxfont = get_cached_wxfont(font)
-        else:
-            index = wx.SYS_DEFAULT_GUI_FONT
-            wxfont = wx.SystemSettings.GetFont(index)
-        widget = self.widget
-        widget.SetFont(wxfont)
-        widget.Refresh()
+        self.widget.setPrefix(prefix)
 
-    def set_tool_tip(self, tool_tip):
-        """ Set the tool tip of for this widget.
+    def set_suffix(self, suffix):
+        """ Set the suffix for the spin box.
 
         """
-        self.widget.SetToolTipString(tool_tip)
+        self.widget.setSuffix(suffix)
 
-    def set_status_tip(self, status_tip):
-        """ This is not supported on Wx.
+    def set_special_value_text(self, text):
+        """ Set the special value text for the spin box.
 
         """
-        pass
+        self.widget.setSpecialValueText(text)
 
-    def ensure_visible(self):
-        """ Ensure the widget is visible.
+    def set_single_step(self, step):
+        """ Set the widget's single step value.
 
         """
-        self.widget.Show(True)
+        self.widget.setSingleStep(step)
 
-    def ensure_hidden(self):
-        """ Ensure the widget is hidden.
+    def set_read_only(self, read_only):
+        """ Set the widget's read only flag.
 
         """
-        self.widget.Show(False)
+        self.widget.setReadOnly(read_only)
 
-    def restyle(self):
-        """ Stylesheets are not supported on Wx.
+    def set_wrapping(self, wrapping):
+        """ Set the widget's wrapping flag.
 
         """
-        pass
+        self.widget.setWrapping(wrapping)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_combo_box.py` & `enaml-0.9.8/enaml/qt/qt_timer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,94 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
+from atom.api import Typed
 
-from atom.api import Int, Typed
+from enaml.widgets.timer import ProxyTimer
 
-from enaml.widgets.combo_box import ProxyComboBox
+from .QtCore import QTimer
 
-from .wx_control import WxControl
+from .qt_toolkit_object import QtToolkitObject
 
 
-# cyclic notification guard flags
-INDEX_GUARD = 0x1
-
-
-class WxComboBox(WxControl, ProxyComboBox):
-    """ A Wx implementation of an Enaml ProxyComboBox.
+class QtTimer(QtToolkitObject, ProxyTimer):
+    """ A Qt implementation of an Enaml ProxyTimer.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(wx.ComboBox)
-
-    #: Cyclic notification guard. This a bitfield of multiple guards.
-    _guard = Int(0)
+    widget = Typed(QTimer)
 
     #--------------------------------------------------------------------------
-    # Initialization API
+    # Initialization
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the QComboBox widget.
+        """ Create the underlying timer object.
 
         """
-        self.widget = wx.ComboBox(self.parent_widget(), style=wx.CB_READONLY)
+        self.widget = QTimer()
 
     def init_widget(self):
-        """ Create and initialize the underlying widget.
+        """ Initialize the widget.
 
         """
-        super(WxComboBox, self).init_widget()
+        super(QtTimer, self).init_widget()
         d = self.declaration
-        self.set_items(d.items)
-        self.set_index(d.index)
-        self.set_editable(d.editable)
-        self.widget.Bind(wx.EVT_COMBOBOX, self.on_index_changed)
+        self.set_interval(d.interval)
+        self.set_single_shot(d.single_shot)
+        self.widget.timeout.connect(self.on_timeout)
+
+    def destroy(self):
+        """ A reimplemented destructor.
+
+        This stops the timer before invoking the superclass destructor.
+
+        """
+        self.widget.stop()
+        super(QtTimer, self).destroy()
 
     #--------------------------------------------------------------------------
-    # Event Handlers
+    # Signal Handlers
     #--------------------------------------------------------------------------
-    def on_index_changed(self, event):
-        """ The signal handler for the index changed signal.
+    def on_timeout(self):
+        """ Handle the timeout signal for the timer.
 
         """
-        if not self._guard & INDEX_GUARD:
-            self.declaration.index = self.widget.GetCurrentSelection()
+        d = self.declaration
+        if d is not None:
+            d.timeout()
 
     #--------------------------------------------------------------------------
-    # ProxyComboBox API
+    # ProxyTimer API
     #--------------------------------------------------------------------------
-    def set_items(self, items):
-        """ Set the items of the ComboBox.
+    def set_interval(self, interval):
+        """ Set the interval on the timer.
+
+        """
+        self.widget.setInterval(interval)
+
+    def set_single_shot(self, single_shot):
+        """ Set the single shot flag on the timer.
 
         """
-        widget = self.widget
-        sel = widget.GetCurrentSelection()
-        widget.SetItems(items)
-        widget.SetSelection(sel)
+        self.widget.setSingleShot(single_shot)
 
-    def set_index(self, index):
-        """ Set the current index of the ComboBox
+    def start(self):
+        """ Start or restart the timer.
 
         """
-        self._guard |= INDEX_GUARD
-        try:
-            self.widget.SetSelection(index)
-        finally:
-            self._guard &= ~INDEX_GUARD
+        self.widget.start()
+
+    def stop(self):
+        """ Stop the timer.
 
-    def set_editable(self, editable):
-        """ Set whether the combo box is editable.
+        """
+        self.widget.stop()
 
-        This is not supported on wx.
+    def is_running(self):
+        """ Get whether or not the timer is running.
 
         """
-        pass
+        return self.widget.isActive()
```

### Comparing `enaml-0.9.7/enaml/wx/wx_abstract_button.py` & `enaml-0.9.8/enaml/qt/qt_abstract_button.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,123 +1,138 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from atom.api import Int
+from atom.api import Int, Typed
 
 from enaml.widgets.abstract_button import ProxyAbstractButton
 
-from .wx_control import WxControl
+from .QtCore import QSize
+from .QtGui import QAbstractButton, QIcon
+
+from .q_resource_helpers import get_cached_qicon
+from .qt_control import QtControl
 
 
 # cyclic notification guard flags
 CHECKED_GUARD = 0x1
 
 
-class WxAbstractButton(WxControl, ProxyAbstractButton):
-    """ A Wx implementation of an Enaml ProxyAbstractButton.
+class QtAbstractButton(QtControl, ProxyAbstractButton):
+    """ A Qt implementation of the Enaml ProxyAbstractButton.
 
     This class can serve as a base class for widgets that implement
     button behavior such as CheckBox, RadioButton and PushButtons.
     It is not meant to be used directly.
 
     """
+    #: A reference to the widget created by the proxy
+    widget = Typed(QAbstractButton)
+
     #: Cyclic notification guard. This a bitfield of multiple guards.
     _guard = Int(0)
 
     #--------------------------------------------------------------------------
-    # Setup Methods
+    # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
         """ Implement in a subclass to create the widget.
 
         """
         raise NotImplementedError
 
     def init_widget(self):
         """ Initialize the button widget.
 
         """
-        super(WxAbstractButton, self).init_widget()
+        super(QtAbstractButton, self).init_widget()
         d = self.declaration
         if d.text:
             self.set_text(d.text)
+        if d.icon:
+            self.set_icon(d.icon)
+        if -1 not in d.icon_size:
+            self.set_icon_size(d.icon_size)
         self.set_checkable(d.checkable)
         self.set_checked(d.checked)
+        widget = self.widget
+        widget.clicked.connect(self.on_clicked)
+        widget.toggled.connect(self.on_toggled)
 
     #--------------------------------------------------------------------------
-    # Event Handlers
+    # Signal Handlers
     #--------------------------------------------------------------------------
-    def on_clicked(self, event):
-        """ The event handler for the clicked event.
-
-        Parameters
-        ----------
-        event : wxEvent
-            The wx event object. This is ignored by the handler.
+    def on_clicked(self):
+        """ The signal handler for the 'clicked' signal.
 
         """
+        # PySide does pass the 'checked' arg to the slot like PyQt, so
+        # grab the checked attribute directly, which works on both.
+        checked = self.widget.isChecked()
         if not self._guard & CHECKED_GUARD:
-            checked = self.get_checked()
             self.declaration.checked = checked
             self.declaration.clicked(checked)
 
-    def on_toggled(self, event):
-        """ The event handler for the toggled event.
-
-        Parameters
-        ----------
-        event : wxEvent
-            The wx event object. This is ignored by the handler.
+    def on_toggled(self, checked):
+        """ The signal handler for the 'toggled' signal.
 
         """
         if not self._guard & CHECKED_GUARD:
-            checked = self.get_checked()
             self.declaration.checked = checked
             self.declaration.toggled(checked)
 
     #--------------------------------------------------------------------------
     # ProxyAbstractButton API
     #--------------------------------------------------------------------------
     def set_text(self, text):
         """ Sets the widget's text with the provided value.
 
         """
         with self.geometry_guard():
-            self.widget.SetLabel(text)
+            self.widget.setText(text)
 
     def set_icon(self, icon):
-        """ Sets the widget's icon to the provided image
-
-        This is not supported on wx.
+        """ Set the icon on the widget.
 
         """
-        pass
-
-    def set_icon_size(self, icon_size):
-        """ Sets the widget's icon size to the provided tuple
+        if icon:
+            qicon = get_cached_qicon(icon)
+        else:
+            qicon = QIcon()
+        with self.geometry_guard():
+            self.widget.setIcon(qicon)
 
-        This is not supported on wx.
+    def set_icon_size(self, size):
+        """ Sets the widget's icon size.
 
         """
-        pass
+        with self.geometry_guard():
+            self.widget.setIconSize(QSize(*size))
 
     def set_checkable(self, checkable):
         """ Sets whether or not the widget is checkable.
 
         """
-        raise NotImplementedError
-
-    def get_checked(self):
-        """ Returns the checked state of the widget.
-
-        """
-        raise NotImplementedError
+        self.widget.setCheckable(checkable)
 
     def set_checked(self, checked):
         """ Sets the widget's checked state with the provided value.
 
         """
-        raise NotImplementedError
+        widget = self.widget
+        # This handles the case where, by default, Qt will not allow
+        # all of the radio buttons in a group to be disabled. By
+        # temporarily turning off auto-exclusivity, we are able to
+        # handle that case.
+        self._guard |= CHECKED_GUARD
+        try:
+            if not checked and widget.isChecked() and widget.autoExclusive():
+                widget.setAutoExclusive(False)
+                widget.setChecked(checked)
+                widget.setAutoExclusive(True)
+            else:
+                widget.setChecked(checked)
+        finally:
+            self._guard &= ~CHECKED_GUARD
```

### Comparing `enaml-0.9.7/enaml/wx/wx_constraints_widget.py` & `enaml-0.9.8/enaml/qt/qt_constraints_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,101 +7,109 @@
 #------------------------------------------------------------------------------
 from contextlib import contextmanager
 
 from atom.api import Int, ForwardTyped
 
 from enaml.widgets.constraints_widget import ProxyConstraintsWidget
 
-from .wx_widget import WxWidget
+from .qt_widget import QtWidget
 
 
 # keep around for backwards compatibility
 def size_hint_guard(obj):
     return obj.geometry_guard()
 
 
-def WxContainer():
-    from .wx_container import WxContainer
-    return WxContainer
+def QtContainer():
+    from .qt_container import QtContainer
+    return QtContainer
 
 
-class WxConstraintsWidget(WxWidget, ProxyConstraintsWidget):
-    """ A Wx implementation of an Enaml ProxyConstraintsWidget.
+class QtConstraintsWidget(QtWidget, ProxyConstraintsWidget):
+    """ A Qt implementation of an Enaml ProxyConstraintsWidget.
 
     """
     #: The container which manages the layout for this widget. This
     #: is assigned during the layout building pass.
-    layout_container = ForwardTyped(WxContainer)
+    layout_container = ForwardTyped(QtContainer)
 
     #: The layout index for this widget's layout item. This is assigned
     #: during the layout building pass.
     layout_index = Int()
 
     def destroy(self):
         """ A reimplemented destructor.
 
         This destructor drops the reference to the layout container.
 
         """
         del self.layout_container
-        super(WxConstraintsWidget, self).destroy()
+        super(QtConstraintsWidget, self).destroy()
 
     #--------------------------------------------------------------------------
     # ProxyConstraintsWidget API
     #--------------------------------------------------------------------------
     def request_relayout(self):
         """ Request a relayout of the proxy widget.
 
         This method forwards the request to the layout container.
 
         """
         container = self.layout_container
         if container is not None:
             container.request_relayout()
 
+    def restyle(self):
+        """ Restyle the widget with the current style data.
+
+        This reimplementation restyles from within a geometry guard.
+
+        """
+        with self.geometry_guard():
+            super(QtConstraintsWidget, self).restyle()
+
     #--------------------------------------------------------------------------
     # Layout API
     #--------------------------------------------------------------------------
     def geometry_updated(self):
         """ Notify the layout system that the geometry has changed.
 
         This method forwards the update to the layout container.
 
         """
         container = self.layout_container
         if container is not None:
             container.geometry_updated(self)
-        self.post_wx_layout_request()
 
     @contextmanager
     def geometry_guard(self):
         """ A context manager for guarding the geometry of the widget.
 
         If the proxy is fully active, this context manager will call the
         'geometry_updated' method if the size hint, minimum, or maximum
         size of the widget changes during context execution.
 
         """
         if not self.is_active:
             yield
             return
         widget = self.widget
-        old_hint = widget.GetBestSize()
-        old_min = widget.GetMinSize()
-        old_max = widget.GetMaxSize()
+        old_hint = widget.sizeHint()
+        old_min = widget.minimumSize()
+        old_max = widget.maximumSize()
         yield
-        if (old_hint != widget.GetBestSize() or
-            old_min != widget.GetMinSize() or
-            old_max != widget.GetMaxSize()):
+        if (old_hint != widget.sizeHint() or
+            old_min != widget.minimumSize() or
+            old_max != widget.maximumSize()):
             self.geometry_updated()
 
     #--------------------------------------------------------------------------
     # Reimplementations
     #--------------------------------------------------------------------------
     def set_font(self, font):
         """ A reimplemented font setter.
 
         This method sets the font from within a geometry guard.
 
         """
         with self.geometry_guard():
-            super(WxConstraintsWidget, self).set_font(font)
+            super(QtConstraintsWidget, self).set_font(font)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_window.py` & `enaml-0.9.8/enaml/qt/qt_window.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
+import sys
 
-from atom.api import Typed
+from atom.api import Typed, atomref
 
 from enaml.layout.geometry import Pos, Rect, Size
 from enaml.widgets.window import ProxyWindow, CloseEvent
 
-from .wx_action import wxAction
-from .wx_container import WxContainer
-from .wx_layout_request import EVT_COMMAND_LAYOUT_REQUESTED
-from .wx_single_widget_sizer import wxSingleWidgetSizer
-from .wx_widget import WxWidget
+from .QtCore import Qt, QPoint, QRect, QSize
+from .QtGui import QApplication, QIcon
+
+from .q_deferred_caller import deferredCall
+from .q_resource_helpers import get_cached_qicon
+from .q_window_base import QWindowBase
+from .qt_container import QtContainer
+from .qt_widget import QtWidget
+
+
+MODALITY = {
+    'non_modal': Qt.NonModal,
+    'application_modal': Qt.ApplicationModal,
+    'window_modal': Qt.WindowModal,
+}
 
 
 def finalize_close(d):
     """ Finalize the closing of the declaration object.
 
     This is performed as a deferred call so that the window may fully
     close before the declaration is potentially destroyed.
@@ -28,391 +38,292 @@
     """
     d.visible = False
     d.closed()
     if d.destroy_on_close:
         d.destroy()
 
 
-class wxCustomWindow(wx.Frame):
-    """ A custom wxFrame which manages a central widget.
+class QWindow(QWindowBase):
+    """ A window base subclass which handles the close event.
 
     The window layout computes the min/max size of the window based
     on its central widget, unless the user explicitly changes them.
 
     """
-    def __init__(self, *args, **kwargs):
-        """ Initialize a wxCustomWindow.
+    def __init__(self, proxy, parent=None, flags=Qt.Widget):
+        """ Initialize a QWindow.
 
         Parameters
         ----------
-        *args, **kwargs
-            The positional and keyword arguments needed to initialize
-            a wxFrame.
+        proxy : QtWindow
+            The proxy object which owns this window. Only an atomref
+            will be maintained to this object.
 
-        """
-        super(wxCustomWindow, self).__init__(*args, **kwargs)
-        self._central_widget = None
-        self.SetSizer(wxSingleWidgetSizer())
-        self.Bind(wx.EVT_MENU, self.OnMenu)
-        self.Bind(wx.EVT_CLOSE, self.OnClose)
+        parent : QWidget, optional
+            The parent of the window.
 
-    #--------------------------------------------------------------------------
-    # Event Handlers
-    #--------------------------------------------------------------------------
-    def OnMenu(self, event):
-        """ The event handler for the EVT_MENU event.
-
-        This event handler will be called when an action is triggered
-        in a Menu or a ToolBar.
+        flags : Qt.WindowFlags, optional
+            The window flags to pass to the parent constructor.
 
         """
-        action = wxAction.FindById(event.GetId())
-        if action is not None:
-            if action.IsCheckable():
-                action.SetChecked(event.Checked())
-            action.Trigger()
+        super(QWindow, self).__init__(parent, Qt.Window | flags)
+        self._proxy_ref = atomref(proxy)
 
-    def OnClose(self, event):
-        """ The event handler for the EVT_CLOSE event.
-
-        This event handler prevents the frame from being destroyed on
-        close. Instead it just sets the visibility to False.
+    def closeEvent(self, event):
+        """ Handle the close event for the window.
 
         """
-        self.Hide()
-
-    #--------------------------------------------------------------------------
-    # Public API
-    #--------------------------------------------------------------------------
-    def UpdateClientSizeHints(self):
-        """ Update the client size hints for the window.
-
-        This will update the min and max sizes for the window according
-        to the current window state. This method is called automatically
-        when the central widget is changed.
-
-        """
-        sizer = self.GetSizer()
-        min_w, min_h = self.ClientToWindowSize(sizer.CalcMin())
-        max_w, max_h = self.ClientToWindowSize(sizer.CalcMax())
-        self.SetSizeHints(min_w, min_h, max_w, max_h)
-        cur_w, cur_h = self.GetSize()
-        new_w = min(max_w, max(min_w, cur_w))
-        new_h = min(max_h, max(min_h, cur_h))
-        if cur_w != new_w or cur_h != new_h:
-            self.SetSize(wx.Size(new_w, new_h))
-
-    def GetCentralWidget(self):
-        """ Returns the central widget for the window.
-
-        Returns
-        -------
-        result : wxWindow or None
-            The central widget of the window, or None if no widget
-            was provided.
-
-        """
-        return self._central_widget
-
-    def SetCentralWidget(self, widget):
-        """ Set the central widget for this window.
-
-        Parameters
-        ----------
-        widget : wxWindow
-            The widget to use as the content of the window.
-
-        """
-        self._central_widget = widget
-        self.GetSizer().Add(widget)
-        self.UpdateClientSizeHints()
+        event.accept()
+        if not self._proxy_ref:
+            return
+        proxy = self._proxy_ref()
+        d = proxy.declaration
+        d_event = CloseEvent()
+        d.closing(d_event)
+        if d_event.is_accepted():
+            deferredCall(finalize_close, d)
+        else:
+            event.ignore()
 
 
-class WxWindow(WxWidget, ProxyWindow):
-    """ A Wx implementation of an Enaml ProxyWindow.
+class QtWindow(QtWidget, ProxyWindow):
+    """ A Qt implementation of an Enaml ProxyWindow.
 
     """
-    #: A reference tot he toolkit widget created by the proxy.
-    widget = Typed(wxCustomWindow)
+    #: A reference to the toolkit widget created by the proxy.
+    widget = Typed(QWindow)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
-    def creation_style(self):
-        """ A convenience function for getting the creation style.
+    def creation_flags(self):
+        """ A convenience function for getting the creation flags.
 
         """
-        style = wx.DEFAULT_FRAME_STYLE
+        flags = Qt.Widget
         if self.declaration.always_on_top:
-            style |= wx.STAY_ON_TOP
-        return style
+            flags |= Qt.WindowStaysOnTopHint
+        return flags
 
     def create_widget(self):
-        """ Create the underlying wxCustomWindow widget.
+        """ Create the QWindow widget.
 
         """
-        style = self.creation_style()
-        self.widget = wxCustomWindow(self.parent_widget(), style=style)
+        flags = self.creation_flags()
+        self.widget = QWindow(self, self.parent_widget(), flags)
 
     def init_widget(self):
-        """ Initialize the window control.
+        """ Initialize the widget.
 
         """
-        super(WxWindow, self).init_widget()
+        super(QtWindow, self).init_widget()
         d = self.declaration
         if d.title:
             self.set_title(d.title)
         if -1 not in d.initial_size:
-            self.widget.SetClientSize(wx.Size(*d.initial_size))
+            self.widget.resize(*d.initial_size)
         if -1 not in d.initial_position:
-            self.widget.Move(wx.Point(*d.initial_position))
+            self.widget.move(*d.initial_position)
+        if d.modality != 'non_modal':
+            self.set_modality(d.modality)
         if d.icon:
             self.set_icon(d.icon)
-        self.widget.Bind(wx.EVT_CLOSE, self.on_close)
 
     def init_layout(self):
-        """ Perform layout initialization for the control.
+        """ Initialize the widget layout.
 
         """
-        super(WxWindow, self).init_layout()
-        widget = self.widget
-        widget.SetCentralWidget(self.central_widget())
-        widget.Bind(EVT_COMMAND_LAYOUT_REQUESTED, self.on_layout_requested)
+        super(QtWindow, self).init_layout()
+        self.widget.setCentralWidget(self.central_widget())
 
     #--------------------------------------------------------------------------
-    # Utility Methods
+    # Public API
     #--------------------------------------------------------------------------
     def central_widget(self):
         """ Find and return the central widget child for this widget.
 
         Returns
         -------
-        result : wxWindow or None
+        result : QWidget or None
             The central widget defined for this widget, or None if one
             is not defined.
 
         """
         d = self.declaration.central_widget()
         if d is not None:
-            return d.proxy.widget or None
+            return d.proxy.widget
 
     #--------------------------------------------------------------------------
     # Child Events
     #--------------------------------------------------------------------------
-    def child_removed(self, child):
-        """ Handle the child removed event for a QtWindow.
-
-        """
-        if isinstance(child, WxContainer):
-            self.widget.SetCentralWidget(self.central_widget())
-
     def child_added(self, child):
         """ Handle the child added event for a QtWindow.
 
         """
-        if isinstance(child, WxContainer):
-            self.widget.SetCentralWidget(self.central_widget())
-
-    #--------------------------------------------------------------------------
-    # Event Handlers
-    #--------------------------------------------------------------------------
-    def on_close(self, event):
-        """ The event handler for the EVT_CLOSE event.
-
-        """
-        d = self.declaration
-        d_event = CloseEvent()
-        d.closing(d_event)
-        if d_event.is_accepted():
-            event.Skip()
-            # Make sure the frame is not modal when closing, or no other
-            # windows will be unblocked.
-            self.widget.MakeModal(False)
-            wx.CallAfter(finalize_close, d)
-        else:
-            event.Veto()
+        super(QtWindow, self).child_added(child)
+        if isinstance(child, QtContainer):
+            self.widget.setCentralWidget(self.central_widget())
 
-    def on_layout_requested(self, event):
-        """ Handle the layout request event from the central widget.
+    def child_removed(self, child):
+        """ Handle the child added event for a QtWindow.
 
         """
-        # wx likes to send events after the widget is destroyed.
-        if self.widget:
-            self.widget.UpdateClientSizeHints()
+        super(QtWindow, self).child_removed(child)
+        if isinstance(child, QtContainer):
+            self.widget.setCentralWidget(self.central_widget())
 
     #--------------------------------------------------------------------------
     # ProxyWindow API
     #--------------------------------------------------------------------------
     def set_title(self, title):
         """ Set the title of the window.
 
         """
-        self.widget.SetTitle(title)
+        self.widget.setWindowTitle(title)
 
     def set_modality(self, modality):
         """ Set the modality of the window.
 
         """
-        if modality == 'non_modal':
-            self.widget.MakeModal(False)
-        else:
-            self.widget.MakeModal(True)
+        self.widget.setWindowModality(MODALITY[modality])
 
     def set_icon(self, icon):
-        """ This is not supported on Wx.
+        """ Set the window icon.
 
         """
-        pass
+        if icon:
+            qicon = get_cached_qicon(icon)
+        else:
+            qicon = QIcon()
+        self.widget.setWindowIcon(qicon)
 
     def position(self):
         """ Get the position of the of the window.
 
         """
-        point = self.widget.GetPosition()
-        return Pos(point.x, point.y)
+        point = self.widget.pos()
+        return Pos(point.x(), point.y())
 
     def set_position(self, pos):
         """ Set the position of the window.
 
         """
-        self.widget.SetPosition(wx.Point(*pos))
+        self.widget.move(*pos)
 
     def size(self):
         """ Get the size of the window.
 
         """
-        size = self.widget.GetClientSize()
-        return Size(size.GetWidth(), size.GetHeight())
+        size = self.widget.size()
+        return Size(size.width(), size.height())
 
     def set_size(self, size):
         """ Set the size of the window.
 
         """
-        size = wx.Size(*size)
-        if size.IsFullySpecified():
-            self.widget.SetClientSize(size)
+        size = QSize(*size)
+        if size.isValid():
+            self.widget.resize(size)
 
     def geometry(self):
         """ Get the geometry of the window.
 
         """
-        # Wx has no standard way of taking into account the size of
-        # the window frame. I'm not spending time on a workaround.
-        point = self.widget.GetPosition()
-        size = self.widget.GetClientSize()
-        return Rect(point.x, point.y, size.GetWidth(), size.GetHeight())
+        rect = self.widget.geometry()
+        return Rect(rect.x(), rect.y(), rect.width(), rect.height())
 
     def set_geometry(self, rect):
         """ Set the geometry of the window.
 
         """
-        self.set_position(rect[:2])
-        self.set_size(rect[2:])
+        rect = QRect(*rect)
+        if rect.isValid():
+            self.widget.setGeometry(rect)
 
     def frame_geometry(self):
         """ Get the geometry of the window.
 
         """
-        r = self.widget.GetRect()
-        return Rect(r.GetX(), r.GetY(), r.GetWidth(), r.GetHeight())
+        rect = self.widget.frameGeometry()
+        return Rect(rect.x(), rect.y(), rect.width(), rect.height())
 
     def maximize(self):
         """ Maximize the window.
 
         """
-        self.widget.Maximize(True)
+        self.widget.showMaximized()
 
     def is_maximized(self):
         """ Get whether the window is maximized.
 
         """
-        return self.widget.IsMaximized()
+        return bool(self.widget.windowState() & Qt.WindowMaximized)
 
     def minimize(self):
         """ Minimize the window.
 
         """
-        self.widget.Iconize(True)
+        self.widget.showMinimized()
 
     def is_minimized(self):
         """ Get whether the window is minimized.
 
         """
-        return self.widget.IsIconized()
+        return bool(self.widget.windowState() & Qt.WindowMinimized)
 
     def restore(self):
         """ Restore the window after a minimize or maximize.
 
         """
-        self.widget.Maximize(False)
+        self.widget.showNormal()
 
     def send_to_front(self):
         """ Move the window to the top of the Z order.
 
         """
-        self.widget.Raise()
+        self.widget.raise_()
 
     def send_to_back(self):
         """ Move the window to the bottom of the Z order.
 
         """
-        self.widget.Lower()
+        self.widget.lower()
 
     def activate_window(self):
         """ Activate the underlying window widget.
 
         """
-        # wx makes no distinction between raise and activate
-        self.widget.Raise()
+        self.widget.activateWindow()
+        if sys.platform == 'win32':
+            # For some reason, this needs to be called twice on Windows
+            # in order to get the taskbar entry to flash.
+            self.widget.activateWindow()
 
     def center_on_screen(self):
         """ Center the window on the screen.
 
         """
-        self.widget.CenterOnScreen()
+        widget = self.widget
+        rect = QRect(QPoint(0, 0), widget.frameGeometry().size())
+        geo = QApplication.desktop().screenGeometry(widget)
+        widget.move(geo.center() - rect.center())
 
     def center_on_widget(self, other):
         """ Center the window on another widget.
 
         """
         widget = self.widget
-        rect = widget.GetRect()
-        geo = other.proxy.widget.GetScreenRect()
-        widget.Move(rect.CenterIn(geo).GetPosition())
+        rect = QRect(QPoint(0, 0), widget.frameGeometry().size())
+        other_widget = other.proxy.widget
+        if other_widget.isWindow():
+            geo = other_widget.frameGeometry()
+        else:
+            size = other_widget.size()
+            point = other_widget.mapToGlobal(QPoint(0, 0))
+            geo = QRect(point, size)
+        widget.move(geo.center() - rect.center())
 
     def close(self):
-        """ Close the window
-
-        """
-        self.widget.Close()
-
-    #--------------------------------------------------------------------------
-    # Overrides
-    #--------------------------------------------------------------------------
-    def set_visible(self, visible):
-        """ Set the visibility state on the underlying widget.
-
-        This override sets the modality to false when hiding the window
-        and enabled it when showing the window (if requested).
-
-        """
-        modality = self.declaration.modality
-        self.widget.MakeModal(visible and modality != 'non_modal')
-        self.widget.Show(visible)
-
-    def ensure_visible(self):
-        """ Ensure the widget is visible.
-
-        This override forwards to the 'set_visible' method so that the
-        window modality is handled properly.
-
-        """
-        self.set_visible(True)
-
-    def ensure_hidden(self):
-        """ Ensure the widget is hidden.
-
-        This override forwards to the 'set_visible' method so that the
-        window modality is handled properly.
+        """ Close the window.
 
         """
-        self.set_visible(False)
+        self.widget.close()
```

### Comparing `enaml-0.9.7/enaml/wx/wx_notebook.py` & `enaml-0.9.8/enaml/qt/qt_notebook.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,511 +1,557 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import weakref
-import wx
+import sys
+from weakref import WeakKeyDictionary
 
-from atom.api import Instance
+from atom.api import Int, IntEnum, Typed
 
 from enaml.widgets.notebook import ProxyNotebook
 
-from .wx_constraints_widget import WxConstraintsWidget
-from .wx_layout_request import EVT_COMMAND_LAYOUT_REQUESTED
-from .wx_page import WxPage
-from .wx_upstream import aui
+from .QtCore import Qt, QEvent, QSize, Signal
+from .QtGui import (
+    QTabWidget, QTabBar, QResizeEvent, QApplication, QStackedWidget
+)
+
+from .qt_constraints_widget import QtConstraintsWidget
+from .qt_page import QtPage
 
 
-#: A mapping of notebook tab positions for the document style tabs.
-#: Wx currently only supports top and bottom tab positions.
-_TAB_POSITION_MAP = {
-    'top': aui.AUI_NB_TOP,
-    'left': aui.AUI_NB_TOP,
-    'bottom': aui.AUI_NB_BOTTOM,
-    'right': aui.AUI_NB_BOTTOM,
+TAB_POSITIONS = {
+    'top': QTabWidget.North,
+    'bottom': QTabWidget.South,
+    'left': QTabWidget.West,
+    'right': QTabWidget.East,
 }
 
 
-#: A mask of notebook tab positions for the document style tabs.
-_TAB_POSITION_MASK = aui.AUI_NB_TOP | aui.AUI_NB_BOTTOM
-
+DOCUMENT_MODES = {
+    'document': True,
+    'preferences': False,
+}
 
-class wxDocumentNotebook(aui.AuiNotebook):
-    """ A custom AuiNotebook which handles children of type wxPage.
 
-    This notebook is used to implement 'document' style tabs for an
-    Enaml Notebook control.
+class QNotebook(QTabWidget):
+    """ A custom QTabWidget which handles children of type QPage.
 
     """
-    def __init__(self, *args, **kwargs):
-        """ Initialize a wxDocumentNotebook.
-
-        Parameters
-        ----------
-        *args, **kwargs
-            The positional and keyword arguments to pass to the super
-            class.
+    class SizeHintMode(IntEnum):
+        """ An int enum defining the size hint modes of the notebook.
 
         """
-        super(wxDocumentNotebook, self).__init__(*args, **kwargs)
-        self.Bind(aui.EVT_AUINOTEBOOK_PAGE_CLOSE, self.OnPageClose)
-        self._hidden_pages = weakref.WeakKeyDictionary()
+        #: The size hint is the union of all tabs.
+        Union = 0
 
-    #--------------------------------------------------------------------------
-    # Event Handlers
-    #--------------------------------------------------------------------------
-    def OnPageClose(self, event):
-        """ The handler for the EVT_AUINOTEBOOK_PAGE_CLOSE event.
+        #: The size hint is the size hint of the current tab.
+        Current = 1
 
-        This handler forwards the event to the wxPage instance.
-
-        """
-        self.GetPage(event.GetSelection()).OnClose(event)
-
-    #--------------------------------------------------------------------------
-    # Public API
-    #--------------------------------------------------------------------------
-    def GetBestSize(self):
-        """ Overridden GetBestSize method which will return the best
-        size for the notebook.
-
-        """
-        size = wx.Size(256, 192)
-        for idx in xrange(self.GetPageCount()):
-            page = self.GetPage(idx)
-            psize = page.GetBestSize()
-            size.SetWidth(max(size.GetWidth(), psize.GetWidth()))
-            size.SetHeight(max(size.GetHeight(), psize.GetHeight()))
-        # On windows, there's an off by 2 error in the width.
-        height = self.GetHeightForPageHeight(size.GetHeight())
-        return wx.Size(size.GetWidth() + 2, height)
+    #: Proxy the SizeHintMode values as if it were an anonymous enum.
+    Union = SizeHintMode.Union
+    Current = SizeHintMode.Current
 
-    def ShowWxPage(self, page):
-        """ Show a hidden wxPage instance in the notebook.
+    #: A signal emitted when a LayoutRequest event is posted to the
+    #: notebook widget. This will typically occur when the size hint
+    #: of the notebook is no longer valid.
+    layoutRequested = Signal()
 
-        If the page is not owned by the notebook, this is a no-op.
+    def __init__(self, *args, **kwargs):
+        """ Initialize a QNotebook.
 
         Parameters
         ----------
-        page : wxPage
-            The hidden wxPage instance to show in the notebook.
+        *args, **kwargs
+            The positional and keyword arguments needed to create
+            a QTabWidget.
 
         """
-        index = self.GetPageIndex(page)
-        if index == -1:
-            index = self._hidden_pages.pop(page, -1)
-            if index != -1:
-                self.InsertWxPage(index, page)
+        super(QNotebook, self).__init__(*args, **kwargs)
+        self.tabCloseRequested.connect(self.onTabCloseRequested)
+        self._hidden_pages = WeakKeyDictionary()
+        self._size_hint = QSize()
+        self._min_size_hint = QSize()
+        self._size_hint_mode = QNotebook.Union
 
-    def HideWxPage(self, page):
-        """ Hide the given wxPage instance in the notebook.
-
-        If the page is not owned by the notebook, this is a no-op.
-
-        Parameters
-        ----------
-        page : wxPage
-            The wxPage instance to hide in the notebook.
+    #--------------------------------------------------------------------------
+    # Private API
+    #--------------------------------------------------------------------------
+    def _refreshTabBar(self):
+        """ Trigger an immediate relayout and refresh of the tab bar.
 
         """
-        index = self.GetPageIndex(page)
-        if index != -1:
-            self.RemovePage(index)
-            page.Show(False)
-            self._hidden_pages[page] = index
-
-    def AddWxPage(self, page):
-        """ Add a wxPage instance to the notebook.
-
-        This should be used in favor of AddPage for adding a wxPage
-        instance to the notebook, as it takes into account the current
-        page state.
+        # The public QTabBar api does not provide a way to trigger the
+        # 'layoutTabs' method of QTabBarPrivate and there are certain
+        # operations (such as modifying a tab close button) which need
+        # to have that happen. This method provides a workaround by
+        # sending a dummy resize event to the tab bar, followed by one
+        # to the tab widget.
+        app = QApplication.instance()
+        if app is not None:
+            bar = self.tabBar()
+            size = bar.size()
+            event = QResizeEvent(size, size)
+            app.sendEvent(bar, event)
+            size = self.size()
+            event = QResizeEvent(size, size)
+            app.sendEvent(self, event)
 
-        Parameters
-        ----------
-        page : wxPage
-            The wxPage instance to add to the notebook.
+    #--------------------------------------------------------------------------
+    # Signal Handlers
+    #--------------------------------------------------------------------------
+    def onTabCloseRequested(self, index):
+        """ The handler for the 'tabCloseRequested' signal.
 
         """
-        if page.IsOpen():
-            self.AddPage(page, page.GetTitle())
-            index = self.GetPageIndex(page)
-            if not page.GetEnabled():
-                self.EnableTab(index, False)
-            if not page.GetClosable():
-                self.SetCloseButton(index, False)
-        else:
-            page.Show(False)
-            self._hidden_pages[page] = self.GetPageCount()
-
-    def InsertWxPage(self, index, page):
-        """ Insert a wxPage instance into the notebook.
-
-        This should be used in favor of InsertPage for inserting a
-        wxPage instance into the notebook, as it takes into account the
-        current page state.
+        self.widget(index).requestClose()
 
-        Parameters
-        ----------
-        index : int
-            The index at which to insert the page.
-
-        page : wxPage
-            The wxPage instance to add to the notebook.
-
-        """
-        if page.IsOpen():
-            index = min(index, self.GetPageCount())
-            self.InsertPage(index, page, page.GetTitle())
-            if not page.GetEnabled():
-                self.EnableTab(index, False)
-            if not page.GetClosable():
-                self.SetCloseButton(index, False)
-        else:
-            page.Show(False)
-            self._hidden_pages[page] = index
+    #--------------------------------------------------------------------------
+    # Public API
+    #--------------------------------------------------------------------------
+    def event(self, event):
+        """ A custom event handler which handles LayoutRequest events.
 
-    def RemoveWxPage(self, page):
-        """ Remove a wxPage instance from the notebook.
+        When a LayoutRequest event is posted to this widget, it will
+        emit the `layoutRequested` signal. This allows an external
+        consumer of this widget to update their external layout.
+
+        """
+        res = super(QNotebook, self).event(event)
+        if event.type() == QEvent.LayoutRequest:
+            self._size_hint = QSize()
+            self._min_size_hint = QSize()
+            self.layoutRequested.emit()
+        return res
+
+    def sizeHint(self):
+        """ A reimplemented size hint handler.
+
+        """
+        # Cached for performance. Invalidated on a layout request.
+        hint = self._size_hint
+        if hint.isValid():
+            return hint
+        # QTabWidget does not allow assigning a custom QStackedWidget,
+        # so the default sizeHint is computed, and the effects of the
+        # stack size hint are replaced by the current tab's size hint.
+        hint = super(QNotebook, self).sizeHint()
+        if self._size_hint_mode == QNotebook.Current:
+            stack = self.findChild(QStackedWidget)
+            if stack is not None:
+                curr = stack.currentWidget()
+                if curr is not None:
+                    hint -= stack.sizeHint()
+                    hint += curr.sizeHint()
+        self._size_hint = hint
+        return hint
+
+    def minimumSizeHint(self):
+        """ A reimplemented minimum size hint handler.
+
+        """
+        # Cached for performance. Invalidated on a layout request.
+        hint = self._size_hint
+        if hint.isValid():
+            return hint
+        # QTabWidget does not allow assigning a custom QStackedWidget,
+        # so the default minimumSizeHint is computed, and the effects
+        # of the stack size hint are replaced by the current tab's
+        # minimum size hint.
+        hint = super(QNotebook, self).minimumSizeHint()
+        if self._size_hint_mode == QNotebook.Current:
+            stack = self.findChild(QStackedWidget)
+            if stack is not None:
+                curr = stack.currentWidget()
+                if curr is not None:
+                    hint -= stack.minimumSizeHint()
+                    hint += curr.minimumSizeHint()
+        self._size_hint = hint
+        return hint
 
-        If the page does not exist in the notebook, this is a no-op.
+    def sizeHintMode(self):
+        """ Get the size hint mode of the notebook.
 
-        Parameters
-        ----------
-        page : wxPage
-            The wxPage instance to remove from the notebook.
+        Returns
+        -------
+        result : QNotebook.SizeHintMode
+            The size hint mode enum value for the notebook.
 
         """
-        index = self.GetPageIndex(page)
-        if index != -1:
-            self.RemovePage(index)
-            page.Show(False)
-
-
-class wxPreferencesNotebook(wx.Notebook):
-    """ A custom wx.Notebook which handles children of type wxPage.
+        return self._size_hint_mode
 
-    This notebook is used to implement 'document' style tabs for an
-    Enaml Notebook control.
-
-    """
-    def __init__(self, *args, **kwargs):
-        """ Initialize a wxPreferencesNotebook.
+    def setSizeHintMode(self, mode):
+        """ Set the size hint mode of the notebook.
 
         Parameters
         ----------
-        *args, **kwargs
-            The positional and keyword arguments to pass to the super
-            class.
+        mode : QNotebook.SizeHintMode
+            The size hint mode for the notebook.
 
         """
-        super(wxPreferencesNotebook, self).__init__(*args, **kwargs)
-        self._hidden_pages = weakref.WeakKeyDictionary()
+        assert isinstance(mode, QNotebook.SizeHintMode)
+        self._size_hint = QSize()
+        self._min_size_hint = QSize()
+        self._size_hint_mode = mode
 
-    #--------------------------------------------------------------------------
-    # Public API
-    #--------------------------------------------------------------------------
-    def GetBestSize(self):
-        """ Overridden GetBestSize method which will return the best
-        size for the notebook.
-
-        """
-        size = wx.Size(256, 192)
-        for idx in xrange(self.GetPageCount()):
-            page = self.GetPage(idx)
-            psize = page.GetBestSize()
-            size.SetWidth(max(size.GetWidth(), psize.GetWidth()))
-            size.SetHeight(max(size.GetHeight(), psize.GetHeight()))
-        # On windows, the wx.Notebook renders each page with 2 pixels
-        # of padding on the top, and bottom, and 4 pixels of padding
-        # on the left and right (at least under the Windows 7 theme).
-        # We need to compensate for this padding along with the space
-        # taken up by the tab bar. The tab bar height was manually
-        # measured to be 21 pixels. I've found no way to have wx measure
-        # it for me (there's nothing in RendererNative for it), so its
-        # just hard-coded for now.
-        return wx.Size(size.GetWidth() + 8, size.GetHeight() + 25)
-
-    def ShowWxPage(self, page):
-        """ Show a hidden wxPage instance in the notebook.
+    def showPage(self, page):
+        """ Show a hidden QPage instance in the notebook.
 
         If the page is not owned by the notebook, this is a no-op.
 
         Parameters
         ----------
-        page : wxPage
-            The hidden wxPage instance to show in the notebook.
+        page : QPage
+            The hidden QPage instance to show in the notebook.
 
         """
-        index = self.GetPageIndex(page)
+        index = self.indexOf(page)
         if index == -1:
             index = self._hidden_pages.pop(page, -1)
             if index != -1:
-                self.InsertWxPage(index, page)
+                self.insertPage(index, page)
 
-    def HideWxPage(self, page):
-        """ Hide the given wxPage instance in the notebook.
+    def hidePage(self, page):
+        """ Hide the given QPage instance in the notebook.
 
         If the page is not owned by the notebook, this is a no-op.
 
         Parameters
         ----------
-        page : wxPage
-            The wxPage instance to hide in the notebook.
+        page : QPage
+            The QPage instance to hide in the notebook.
 
         """
-        index = self.GetPageIndex(page)
+        index = self.indexOf(page)
         if index != -1:
-            self.RemovePage(index)
-            page.Show(False)
+            self.removeTab(index)
+            page.hide()
             self._hidden_pages[page] = index
 
-    def AddWxPage(self, page):
-        """ Add a wxPage instance to the notebook.
+    def addPage(self, page):
+        """ Add a QPage instance to the notebook.
 
-        This should be used in favor of AddPage for adding a wxPage
-        instance to the notebook, as it takes into account the current
-        page state.
+        This method should be used in favor of the 'addTab' method.
 
         Parameters
         ----------
-        page : wxPage
-            The wxPage instance to add to the notebook.
+        page : QPage
+            The QPage instance to add to the notebook.
 
         """
-        if page.IsOpen():
-            self.AddPage(page, page.GetTitle())
-        else:
-            page.Show(False)
-            self._hidden_pages[page] = self.GetPageCount()
+        self.insertPage(self.count(), page)
 
-    def InsertWxPage(self, index, page):
-        """ Insert a wxPage instance into the notebook.
+    def insertPage(self, index, page):
+        """ Insert a QPage instance into the notebook.
 
-        This should be used in favor of InsertPage for inserting a
-        wxPage instance into the notebook, as it takes into account the
-        current page state.
+        This should be used in favor of the 'insertTab' method.
 
         Parameters
         ----------
         index : int
             The index at which to insert the page.
 
-        page : wxPage
-            The wxPage instance to add to the notebook.
+        page : QPage
+            The QPage instance to add to the notebook.
 
         """
-        if page.IsOpen():
-            index = min(index, self.GetPageCount())
-            self.InsertPage(index, page, page.GetTitle())
+        if page.isOpen():
+            index = min(index, self.count())
+            self.insertTab(index, page, page.title())
+            self.setTabIcon(index, page.icon())
+            self.setTabToolTip(index, page.toolTip())
+            self.setTabEnabled(index, page.isTabEnabled())
+            self.setTabCloseButtonVisible(index, page.isClosable())
         else:
-            page.Show(False)
+            page.hide()
             self._hidden_pages[page] = index
 
-    def RemoveWxPage(self, page):
-        """ Remove a wxPage instance from the notebook.
+    def removePage(self, page):
+        """ Remove a QPage instance from the notebook.
 
         If the page does not exist in the notebook, this is a no-op.
 
         Parameters
         ----------
-        page : wxPage
-            The wxPage instance to remove from the notebook.
+        page : QPage
+            The QPage instance to remove from the notebook.
 
         """
-        index = self.GetPageIndex(page)
+        index = self.indexOf(page)
         if index != -1:
-            self.RemovePage(index)
-            page.Show(False)
-
-    def GetPageIndex(self, page):
-        """ Returns the index of the page in the control.
+            self.removeTab(index)
+            page.hide()
 
-        Parameters
-        ----------
-        page : wxPage
-            The wxPage instance in the control.
-
-        Returns
-        -------
-        result : int
-            The index of the page in the control, or -1 if the page
-            is not found.
-
-        """
-        # Wx has no way of querying for the index of a page, so we must
-        # linear search ourselves. Hooray for brain-dead toolkits!
-        for idx in xrange(self.GetPageCount()):
-            if self.GetPage(idx) == page:
-                return idx
-        return -1
+    def setTabCloseButtonVisible(self, index, visible, refresh=True):
+        """ Set whether the close button for the given tab is visible.
 
-    def EnableTab(self, index, enabled):
-        """ Change the enabled state of the tab at the given index.
+        The 'tabsClosable' property must be set to True for this to
+        have effect.
 
         Parameters
         ----------
         index : int
-            The index of the target tab.
+            The index of the target page.
 
-        enabled : bool
-            Whether or not the tab should be enabled.
-
-        """
-        if index >= 0 and index < self.GetPageCount():
-            page = self.GetPage(index)
-            page.Enable(enabled)
+        visible : bool
+            Whether or not the close button for the tab should be
+            visible.
+
+        refresh : bool, optional
+            Whether or not to refresh the tab bar at the end of the
+            operation. The default is True.
+
+        """
+        # When changing the visibility of a button, we also change its
+        # size so that the tab can layout properly.
+        if index >= 0 and index < self.count():
+            tabBar = self.tabBar()
+            btn1 = tabBar.tabButton(index, QTabBar.LeftSide)
+            btn2 = tabBar.tabButton(index, QTabBar.RightSide)
+            if btn1 is not None:
+                btn1.setVisible(visible)
+                if not visible:
+                    btn1.resize(0, 0)
+                else:
+                    btn1.resize(btn1.sizeHint())
+            if btn2 is not None:
+                btn2.setVisible(visible)
+                if not visible:
+                    btn2.resize(0, 0)
+                else:
+                    btn2.resize(btn2.sizeHint())
+            if refresh:
+                self._refreshTabBar()
+
+    def setTabsClosable(self, closable):
+        """ Set the tab closable state for the widget.
+
+        This is an overridden parent class method which extends the
+        logic to account for the closable state on the individual
+        pages.
+
+        Parameters
+        ----------
+        closable : bool
+            Whether or not the tabs should be closable.
+
+        """
+        super(QNotebook, self).setTabsClosable(closable)
+        # When setting tabs closable to False, the default logic of
+        # QTabBar is to delete the close button on the tab. When the
+        # closable flag is set to True a new close button is created
+        # for every tab, unless one has already been provided. This
+        # means we need to make an extra pass over each tab to sync
+        # the state of the buttons when the flag is set to True.
+        if closable:
+            setVisible = self.setTabCloseButtonVisible
+            for index in xrange(self.count()):
+                page = self.widget(index)
+                setVisible(index, page.isClosable(), refresh=False)
+        self._refreshTabBar()
+
+
+#: A mapping Enaml -> Qt size hint modes.
+SIZE_HINT_MODE = {
+    'union': QNotebook.Union,
+    'current': QNotebook.Current,
+}
 
-    def SetCloseButton(self, index, closable):
-        """ A dummy method which makes the wxPreferencesNotebook api
-        compatible with the wxDocumentNotebook.
 
-        Close buttons cannot be set on a preferences notebook. This
-        method exists soley so that child wxPages do not need to
-        special case their implementation based on their parent.
+#: A guard flag for the tab change
+CHANGE_GUARD = 0x01
 
-        """
-        pass
 
-
-class WxNotebook(WxConstraintsWidget, ProxyNotebook):
-    """ A Wx implementation of an Enaml ProxyNotebook.
+class QtNotebook(QtConstraintsWidget, ProxyNotebook):
+    """ A Qt implementation of an Enaml ProxyNotebook.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Instance((wxPreferencesNotebook, wxDocumentNotebook))
+    widget = Typed(QNotebook)
+
+    #: A bitfield of guard flags for the object.
+    _guard = Int(0)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying wx notebook widget.
+        """ Create the underlying notebook widget.
 
         """
-        if self.declaration.tab_style == 'preferences':
-            w = wxPreferencesNotebook(self.parent_widget())
-        else:
-            style = aui.AUI_NB_SCROLL_BUTTONS
-            w = wxDocumentNotebook(self.parent_widget(), agwStyle=style)
-        self.widget = w
+        widget = QNotebook(self.parent_widget())
+        if sys.platform == 'darwin':
+            # On OSX, the widget item layout rect is too small.
+            # Setting this attribute forces the widget item to
+            # use the widget rect for layout.
+            widget.setAttribute(Qt.WA_LayoutUsesWidgetRect, True)
+        self.widget = widget
 
     def init_widget(self):
-        """ Create and initialize the notebook control
+        """ Initialize the underyling widget.
 
         """
-        super(WxNotebook, self).init_widget()
+        super(QtNotebook, self).init_widget()
         d = self.declaration
         self.set_tab_style(d.tab_style)
         self.set_tab_position(d.tab_position)
         self.set_tabs_closable(d.tabs_closable)
         self.set_tabs_movable(d.tabs_movable)
+        self.set_size_hint_mode(d.size_hint_mode, update=False)
+        # the selected tab is synchronized during init_layout
 
     def init_layout(self):
         """ Handle the layout initialization for the notebook.
 
         """
-        super(WxNotebook, self).init_layout()
+        super(QtNotebook, self).init_layout()
         widget = self.widget
         for page in self.pages():
-            widget.AddWxPage(page)
-        widget.Bind(EVT_COMMAND_LAYOUT_REQUESTED, self.on_layout_requested)
+            widget.addPage(page)
+        self.init_selected_tab()
+        widget.layoutRequested.connect(self.on_layout_requested)
+        widget.currentChanged.connect(self.on_current_changed)
 
     #--------------------------------------------------------------------------
     # Utility Methods
     #--------------------------------------------------------------------------
     def pages(self):
         """ Get the pages defined for the notebook.
 
         """
         for p in self.declaration.pages():
-            yield p.proxy.widget or None
+            w = p.proxy.widget
+            if w is not None:
+                yield w
+
+    def find_page(self, name):
+        """ Find the page with the given name.
+
+        Parameters
+        ----------
+        name : unicode
+            The object name for the page of interest.
+
+        Returns
+        -------
+        result : QPage or None
+            The target page or None if one is not found.
+
+        """
+        for page in self.pages():
+            if page.objectName() == name:
+                return page
+
+    def init_selected_tab(self):
+        """ Initialize the selected tab.
+
+        This should be called only during widget initialization.
+
+        """
+        d = self.declaration
+        if d.selected_tab:
+            self.set_selected_tab(d.selected_tab)
+        else:
+            current = self.widget.currentWidget()
+            name = current.objectName() if current is not None else u''
+            self._guard |= CHANGE_GUARD
+            try:
+                d.selected_tab = name
+            finally:
+                self._guard &= ~CHANGE_GUARD
 
     #--------------------------------------------------------------------------
     # Child Events
     #--------------------------------------------------------------------------
     def child_added(self, child):
-        """ Handle the child added event for a WxNotebook.
+        """ Handle the child added event for a QtNotebook.
 
         """
-        super(WxNotebook, self).child_added(child)
-        if isinstance(child, WxPage):
+        super(QtNotebook, self).child_added(child)
+        if isinstance(child, QtPage):
             for index, dchild in enumerate(self.children()):
                 if child is dchild:
-                    self.widget.InsertWxPage(index, child.widget)
+                    self.widget.insertPage(index, child.widget)
 
     def child_removed(self, child):
-        """ Handle the child removed event for a WxNotebook.
+        """ Handle the child removed event for a QtNotebook.
 
         """
-        super(WxNotebook, self).child_removed(child)
-        if isinstance(child, WxPage):
-            self.widget.RemoveWxPage(child.widget)
-            self.geometry_updated()
+        super(QtNotebook, self).child_removed(child)
+        if isinstance(child, QtPage):
+            self.widget.removePage(child.widget)
 
     #--------------------------------------------------------------------------
-    # Event Handlers
+    # Signal Handlers
     #--------------------------------------------------------------------------
-    def on_layout_requested(self, event):
-        """ Handle the layout request event from a child page.
+    def on_layout_requested(self):
+        """ Handle the `layoutRequested` signal from the QNotebook.
 
         """
         self.geometry_updated()
 
+    def on_current_changed(self):
+        """ Handle the 'currentChanged' signal from the QNotebook.
+
+        """
+        if not self._guard & CHANGE_GUARD:
+            self._guard |= CHANGE_GUARD
+            try:
+                page = self.widget.currentWidget()
+                name = page.objectName() if page is not None else u''
+                self.declaration.selected_tab = name
+            finally:
+                self._guard &= ~CHANGE_GUARD
+
     #--------------------------------------------------------------------------
     # ProxyNotebook API
     #--------------------------------------------------------------------------
     def set_tab_style(self, style):
-        """ Set the tab style for the underlying widget.
+        """ Set the tab style for the tab bar in the widget.
 
         """
-        # Changing the tab style on wx is not supported
-        pass
+        self.widget.setDocumentMode(DOCUMENT_MODES[style])
 
     def set_tab_position(self, position):
         """ Set the position of the tab bar in the widget.
 
         """
-        # Tab position changes only supported on the document notebook.
-        widget = self.widget
-        if isinstance(widget, wxDocumentNotebook):
-            flags = widget.GetAGWWindowStyleFlag()
-            flags &= ~_TAB_POSITION_MASK
-            flags |= _TAB_POSITION_MAP[position]
-            widget.SetAGWWindowStyleFlag(flags)
-            widget.Refresh()  # Avoids rendering artifacts
+        self.widget.setTabPosition(TAB_POSITIONS[position])
 
     def set_tabs_closable(self, closable):
         """ Set whether or not the tabs are closable.
 
         """
-        # Closable tabs are only supported on the document notebook.
-        widget = self.widget
-        if isinstance(widget, wxDocumentNotebook):
-            flags = widget.GetAGWWindowStyleFlag()
-            if closable:
-                flags |= aui.AUI_NB_CLOSE_ON_ALL_TABS
-            else:
-                flags &= ~aui.AUI_NB_CLOSE_ON_ALL_TABS
-            widget.SetAGWWindowStyleFlag(flags)
+        self.widget.setTabsClosable(closable)
 
     def set_tabs_movable(self, movable):
         """ Set whether or not the tabs are movable.
 
         """
-        # Movable tabs are only supported on the document notebook.
-        widget = self.widget
-        if isinstance(widget, wxDocumentNotebook):
-            flags = widget.GetAGWWindowStyleFlag()
-            if movable:
-                flags |= aui.AUI_NB_TAB_MOVE
-            else:
-                flags &= ~aui.AUI_NB_TAB_MOVE
-            widget.SetAGWWindowStyleFlag(flags)
+        self.widget.setMovable(movable)
+
+    def set_selected_tab(self, name):
+        """ Set the selected tab of the widget.
 
-    def set_size_hint_mode(self, mode):
-        """ This is not supported on Wx.
+        """
+        if not self._guard & CHANGE_GUARD:
+            page = self.find_page(name)
+            if page is None:
+                import warnings
+                msg = "cannot select tab '%s' - tab not found"
+                warnings.warn(msg % name, UserWarning)
+                return
+            self._guard |= CHANGE_GUARD
+            try:
+                self.widget.setCurrentWidget(page)
+            finally:
+                self._guard &= ~CHANGE_GUARD
+
+    def set_size_hint_mode(self, mode, update=True):
+        """ Set the size hint mode for the widget.
 
         """
-        pass
+        self.widget.setSizeHintMode(SIZE_HINT_MODE[mode])
+        if update:
+            self.geometry_updated()
```

### Comparing `enaml-0.9.7/enaml/wx/wx_mpl_canvas.py` & `enaml-0.9.8/enaml/qt/qt_mpl_canvas.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,99 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
+from atom.api import Typed
 
 from enaml.widgets.mpl_canvas import ProxyMPLCanvas
 
-from .wx_control import WxControl
+from matplotlib.backends.backend_qt4agg import FigureCanvasQTAgg
+from matplotlib.backends.backend_qt4agg import NavigationToolbar2QTAgg
 
-from matplotlib.backends.backend_wxagg import FigureCanvasWxAgg
-from matplotlib.backends.backend_wx import NavigationToolbar2Wx
+from .QtCore import Qt
+from .QtGui import QFrame, QVBoxLayout
 
+from .qt_control import QtControl
 
-class WxMPLCanvas(WxControl, ProxyMPLCanvas):
-    """ A Wx implementation of an Enaml MPLCanvas.
+
+class QtMPLCanvas(QtControl, ProxyMPLCanvas):
+    """ A Qt implementation of an Enaml ProxyMPLCanvas.
 
     """
+    #: A reference to the widget created by the proxy.
+    widget = Typed(QFrame)
+
     #--------------------------------------------------------------------------
-    # Setup Methods
+    # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
         """ Create the underlying widget.
 
         """
-        widget = wx.Panel(self.parent_widget())
-        sizer = wx.BoxSizer(wx.VERTICAL)
-        widget.SetSizer(sizer)
+        widget = QFrame(self.parent_widget())
+        layout = QVBoxLayout()
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(0)
+        widget.setLayout(layout)
         self.widget = widget
 
     def init_layout(self):
         """ Initialize the layout of the underlying widget.
 
         """
-        super(WxMPLCanvas, self).init_layout()
+        super(QtMPLCanvas, self).init_layout()
         self._refresh_mpl_widget()
 
     #--------------------------------------------------------------------------
-    # Message Handlers
+    # ProxyMPLCanvas API
     #--------------------------------------------------------------------------
     def set_figure(self, figure):
         """ Set the MPL figure for the widget.
 
         """
         with self.geometry_guard():
             self._refresh_mpl_widget()
 
     def set_toolbar_visible(self, visible):
         """ Set the toolbar visibility for the widget.
 
         """
-        widget = self.widget
-        sizer = widget.GetSizer()
-        children = sizer.GetChildren()
-        if len(children) == 2:
+        layout = self.widget.layout()
+        if layout.count() == 2:
             with self.geometry_guard():
-                widget.Freeze()
-                toolbar = children[0]
-                toolbar.Show(visible)
-                sizer.Layout()
-                widget.Thaw()
+                toolbar = layout.itemAt(0).widget()
+                toolbar.setVisible(visible)
 
     #--------------------------------------------------------------------------
     # Private API
     #--------------------------------------------------------------------------
     def _refresh_mpl_widget(self):
         """ Create the mpl widget and update the underlying control.
 
         """
         # Delete the old widgets in the layout, it's just shenanigans
         # to try to reuse the old widgets when the figure changes.
         widget = self.widget
-        widget.Freeze()
-        sizer = widget.GetSizer()
-        sizer.Clear(True)
+        layout = widget.layout()
+        while layout.count():
+            layout_item = layout.takeAt(0)
+            layout_item.widget().deleteLater()
 
         # Create the new figure and toolbar widgets. It seems that key
         # events will not be processed without an mpl figure manager.
         # However, a figure manager will create a new toplevel window,
         # which is certainly not desired in this case. This appears to
-        # be a limitation of matplotlib.
+        # be a limitation of matplotlib. The canvas is manually set to
+        # visible, or QVBoxLayout will ignore it for size hinting.
         figure = self.declaration.figure
         if figure:
-            canvas = FigureCanvasWxAgg(widget, -1, figure)
-            toolbar = NavigationToolbar2Wx(canvas)
-            toolbar.Show(self.declaration.toolbar_visible)
-            sizer.Add(toolbar, 0, wx.EXPAND)
-            sizer.Add(canvas, 1, wx.EXPAND)
-
-        sizer.Layout()
-        widget.Thaw()
+            canvas = FigureCanvasQTAgg(figure)
+            canvas.setParent(widget)
+            canvas.setFocusPolicy(Qt.ClickFocus)
+            canvas.setVisible(True)
+            toolbar = NavigationToolbar2QTAgg(canvas, widget)
+            toolbar.setVisible(self.declaration.toolbar_visible)
+            layout.addWidget(toolbar)
+            layout.addWidget(canvas)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_splitter.py` & `enaml-0.9.8/enaml/qt/qt_tool_bar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,270 +1,366 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-from wx.lib.splitter import MultiSplitterWindow
+import sys
 
-from atom.api import Typed
+from atom.api import Int, Typed
 
-from enaml.widgets.splitter import ProxySplitter
+from enaml.widgets.tool_bar import ProxyToolBar
 
-from .wx_constraints_widget import WxConstraintsWidget
-from .wx_split_item import WxSplitItem
+from .QtCore import Qt, Signal
+from .QtGui import QToolBar, QMainWindow
 
+from .qt_action import QtAction
+from .qt_action_group import QtActionGroup
+from .qt_constraints_widget import QtConstraintsWidget
+from .qt_widget import QtWidget
 
-_ORIENTATION_MAP = {
-    'horizontal': wx.HORIZONTAL,
-    'vertical': wx.VERTICAL,
+
+#: A mapping from Enaml dock area to Qt tool bar areas
+DOCK_AREAS = {
+    'top': Qt.TopToolBarArea,
+    'right': Qt.RightToolBarArea,
+    'bottom': Qt.BottomToolBarArea,
+    'left': Qt.LeftToolBarArea,
+    'all': Qt.AllToolBarAreas,
+}
+
+
+#: A mapping from Qt tool bar areas to Enaml dock areas
+DOCK_AREAS_INV = {
+    Qt.TopToolBarArea: 'top',
+    Qt.RightToolBarArea: 'right',
+    Qt.BottomToolBarArea: 'bottom',
+    Qt.LeftToolBarArea: 'left',
+    Qt.AllToolBarAreas: 'all',
 }
 
 
-class wxSplitter(MultiSplitterWindow):
-    """ A wx.lib.splitter.MultiSplitterWindow subclass that changes
-    the behavior of resizing neighbors to be consistent with Qt.
+#: A mapping from Enaml orientation to Qt Orientation
+ORIENTATIONS = {
+    'horizontal': Qt.Horizontal,
+    'vertical': Qt.Vertical,
+}
+
+
+#: A mapping from Enaml button style to Qt ToolButtonStyle
+BUTTON_STYLES = {
+    'icon_only': Qt.ToolButtonIconOnly,
+    'text_only': Qt.ToolButtonTextOnly,
+    'text_beside_icon': Qt.ToolButtonTextBesideIcon,
+    'text_under_icon': Qt.ToolButtonTextUnderIcon,
+}
+
+
+class QCustomToolBar(QToolBar):
+    """ A custom QToolBar which adds some Enaml specific features.
 
     """
-    def _OnMouse(self, event):
-        """ Overriden parent class mouse event handler which fakes the
-        state of the keyboard so that resize behavior is consistent
-        between wx and Qt.
-
-        """
-        # We modify the mouse event to "fake" like the shift key is
-        # always down. This causes the splitter to not adjust its
-        # neighbor when dragging the sash. This behavior is consistent
-        # with Qt's behavior. This is not *the best* way to handle this,
-        # but it's the easiest and quickest at the moment. The proper
-        # way would be to reimplement this method in its entirety and
-        # allow the adjustNeighbor computation to be based on keyboard
-        # state as well as attribute flags.
-        #
-        # TODO implement this properly (or just rewrite this entire
-        # control, because like everything else in Wx, it's crap).
-        event.m_shiftDown = True
-        return super(wxSplitter, self)._OnMouse(event)
-
-    def _GetWindowMin(self, window):
-        """ Overriden parent class method which properly computes the
-        window min size.
-
-        """
-        size = window.GetEffectiveMinSize()
-        if self._orient == wx.HORIZONTAL:
-            res = size.GetWidth()
-        else:
-            res = size.GetHeight()
-        return res
+    #: A signal emitted when the dock widget is floated.
+    floated = Signal()
 
-    def _GetSashSize(self):
-        """ Overridden parent class method to return a proper sash size
-        for the custom sash painting.
-
-        """
-        return 4
-
-    def _DrawSash(self, dc):
-        """ Overridden parent class method which draws a custom sash.
-
-        On Windows, the default themed sash drawing causes the sash to
-        not be visible; this method corrects that problem and draws a
-        sash which is visibly similar to Enaml's Qt Windows version.
-
-        """
-        sash_size = self._GetSashSize()
-        width, height = self.GetClientSize()
-        light_pen = wx.WHITE_PEN
-        dark_pen = wx.GREY_PEN
-        brush = wx.Brush(self.GetBackgroundColour())
-        if self._orient == wx.HORIZONTAL:
-            pos = 0
-            for sash in self._sashes[:-1]:
-                pos += sash
-                dc.SetPen(wx.TRANSPARENT_PEN)
-                dc.SetBrush(brush)
-                dc.DrawRectangle(pos, 0, sash_size, height)
-                dc.SetPen(light_pen)
-                dc.DrawLine(pos + 1, 0, pos + 1, height)
-                dc.SetPen(dark_pen)
-                dc.DrawLine(pos + 2, 0, pos + 2, height)
-                pos += sash_size
-        else:
-            pos = 0
-            for sash in self._sashes[:-1]:
-                pos += sash
-                dc.SetPen(wx.TRANSPARENT_PEN)
-                dc.SetBrush(brush)
-                dc.DrawRectangle(0, pos, width, sash_size)
-                dc.SetPen(light_pen)
-                dc.DrawLine(0, pos + 1, width, pos + 1)
-                dc.SetPen(dark_pen)
-                dc.DrawLine(0, pos + 2, width, pos + 2)
-                pos += sash_size
-
-    def _OnSize(self, event):
-        """ Overridden parent class method which resizes the sashes.
-
-        The default Wx behavior allocates all extra space to the last
-        split item, and it will clip the items when the window size is
-        reduced. This override uses a weighted algorithm to allocate
-        the free space among the items and will not allow the items
-        to be clipped by a window resize.
-
-        """
-        # Pre-fetch some commonly used objects
-        get_min = self._GetWindowMin
-        windows = self._windows
-        sashes = self._sashes
-
-        # Compute the total space available for the sashes
-        sash_widths = self._GetSashSize() * (len(windows) - 1)
-        offset = sash_widths + 2 * self._GetBorderSize()
-        if self._orient == wx.HORIZONTAL:
-            free_space = self.GetClientSize().GetWidth() - offset
+    #: A signal emitted when the dock widget is docked. The payload
+    #: will be the new dock area.
+    docked = Signal(object)
+
+    def __init__(self, *args, **kwargs):
+        """ Initialize a QCustomToolBar.
+
+        Parameters
+        ----------
+        *args, **kwargs
+            The positional and keyword arguments needed to initialize
+            a QToolBar.
+
+        """
+        super(QCustomToolBar, self).__init__(*args, **kwargs)
+        self._tool_bar_area = Qt.TopToolBarArea
+        self.topLevelChanged.connect(self._onTopLevelChanged)
+
+    #--------------------------------------------------------------------------
+    # Private API
+    #--------------------------------------------------------------------------
+    def _onTopLevelChanged(self, top_level):
+        """ The signal handler for the the 'topLevelChanged' signal.
+
+        """
+        if top_level:
+            self.floated.emit()
         else:
-            free_space = self.GetClientSize().GetHeight() - offset
+            parent = self.parent()
+            if parent is not None and isinstance(parent, QMainWindow):
+                self._tool_bar_area = parent.toolBarArea(self)
+            self.docked.emit(self._tool_bar_area)
+
+    #--------------------------------------------------------------------------
+    # Public API
+    #--------------------------------------------------------------------------
+    def removeActions(self, actions):
+        """ Remove the given actions from the tool bar.
+
+        Parameters
+        ----------
+        actions : iterable
+            An iterable of QActions to remove from the tool bar.
+
+        """
+        remove = self.removeAction
+        for action in actions:
+            remove(action)
+
+    def toolBarArea(self):
+        """ Get the current tool bar area for the tool bar.
+
+        Returns
+        -------
+        result : QToolBarArea
+            The tool bar area where this tool bar resides.
+
+        """
+        return self._tool_bar_area
+
+    def setToolBarArea(self, area):
+        """ Set the current tool bar area for the tool bar.
+
+        Parameters
+        ----------
+        area : QToolBarArea
+            The tool bar area where this tool bar should reside.
+
+        """
+        self._tool_bar_area = area
+        parent = self.parent()
+        if isinstance(parent, QMainWindow):
+            parent.setToolBarArea(area, self)
+
+    def setFloating(self, floating):
+        """ Set the floating state of the tool bar.
+
+        Parameters
+        ----------
+        floating : bool
+            Whether or not the tool bar should floating.
+
+        """
+        # QToolBar doesn't provide a setFloating() method. This code
+        # is taken mostly from QToolBarPrivate::updateWindowFlags.
+        parent = self.parent()
+        if isinstance(parent, QMainWindow):
+            visible = self.isVisibleTo(parent)
+            flags = Qt.Tool if floating else Qt.Widget
+            flags |= Qt.FramelessWindowHint
+            if sys.platform == 'darwin':
+                flags |= Qt.WindowStaysOnTopHint
+            self.setWindowFlags(flags)
+            if visible:
+                self.resize(self.sizeHint())
+                self.setVisible(True)
 
-        # Compute the effective stretch factors for each window. The
-        # effective stretch factor is the greater of the current or
-        # minimum width of the window, multiplied by the window's
-        # stretch factor.
-        parts = []
-        total_stretch = 0
-        for idx, (sash, window) in enumerate(zip(sashes, windows)):
-            minw = get_min(window)
-            if sash < minw:
-                sash = sashes[idx] = minw
-            stretch = window.GetStretch() * sash
-            parts.append((stretch, idx, minw, window))
-            total_stretch += stretch
-
-        # Add (or remove) the extra space by fairly allocating it to
-        # each window based on their effective stretch factor.
-        diff_space = free_space - sum(sashes)
-        for stretch, idx, minw, window in parts:
-            if stretch > 0:
-                d = diff_space * stretch / total_stretch
-                new = max(sashes[idx] + d, minw)
-                sashes[idx] = new
-
-        # Since the windows are clipped to their minimum width, it's
-        # possible that the current space occupied by the windows will
-        # be too large. In that case, the overage is distributed to the
-        # windows fairly, based on their relative capacity for shrink.
-        curr_space = sum(sashes)
-        if curr_space > free_space:
-            diffs = []
-            total_diff = 0
-            for stretch, idx, minw, window in parts:
-                diff = sashes[idx] - minw
-                if diff > 0:
-                    diffs.append((diff, window, idx, minw))
-                    total_diff += diff
-            remaining = curr_space - free_space
-            diffs.sort()
-            for diff, window, idx, minw in reversed(diffs):
-                delta = remaining * diff / total_diff
-                old = sashes[idx]
-                new = max(old - delta, minw)
-                actual_diff = old - new
-                remaining -= actual_diff
-                total_diff -= actual_diff
-                sashes[idx] = new
 
-        # The superclass handler which will actually perform the layout.
-        super(wxSplitter, self)._OnSize(event)
+# cyclic notification guard flags
+FLOATED_GUARD = 0x1
 
 
-class WxSplitter(WxConstraintsWidget, ProxySplitter):
-    """ A Wx implementation of an Enaml ProxySplitter.
+class QtToolBar(QtConstraintsWidget, ProxyToolBar):
+    """ A Qt implementation of an Enaml ToolBar.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(wxSplitter)
+    widget = Typed(QCustomToolBar)
+
+    #: Cyclic notification guard. This a bitfield of multiple guards.
+    _guard = Int(0)
 
     #--------------------------------------------------------------------------
-    # Setup methods
+    # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Creates the underlying wxSplitter widget.
+        """ Create the QCustomToolBar widget.
 
         """
-        self.widget = wxSplitter(self.parent_widget())
+        self.widget = QCustomToolBar(self.parent_widget())
 
     def init_widget(self):
-        """ Initialize the underlying control.
+        """ Initialize the tool bar widget.
 
         """
-        super(WxSplitter, self).init_widget()
+        super(QtToolBar, self).init_widget()
         d = self.declaration
+        self.set_button_style(d.button_style)
+        self.set_movable(d.movable)
+        self.set_floatable(d.floatable)
+        self.set_floating(d.floating)
+        self.set_dock_area(d.dock_area)
+        self.set_allowed_dock_areas(d.allowed_dock_areas)
         self.set_orientation(d.orientation)
-        self.set_live_drag(d.live_drag)
+        widget = self.widget
+        widget.floated.connect(self.on_floated)
+        widget.docked.connect(self.on_docked)
 
     def init_layout(self):
-        """ Handle the layout initialization for the splitter.
+        """ Initialize the layout for the toolbar.
 
         """
-        super(WxSplitter, self).init_layout()
+        super(QtToolBar, self).init_layout()
         widget = self.widget
-        for item in self.split_items():
-            widget.AppendWindow(item)
+        for child in self.children():
+            if isinstance(child, QtAction):
+                widget.addAction(child.widget)
+            elif isinstance(child, QtActionGroup):
+                widget.addActions(child.actions())
+            elif isinstance(child, QtWidget):
+                widget.addAction(child.get_action(True))
 
     #--------------------------------------------------------------------------
     # Child Events
     #--------------------------------------------------------------------------
+    def find_next_action(self, child):
+        """ Locate the QAction object which logically follows the child.
+
+        Parameters
+        ----------
+        child : QtToolkitObject
+            The child object of interest.
+
+        Returns
+        -------
+        result : QAction or None
+            The QAction which logically follows the position of the
+            child in the list of children. None will be returned if
+            a relevant QAction is not found.
+
+        """
+        found = False
+        for dchild in self.children():
+            if found:
+                if isinstance(dchild, QtAction):
+                    return dchild.widget
+                elif isinstance(dchild, QtActionGroup):
+                    actions = dchild.actions()
+                    if len(actions) > 0:
+                        return actions[0]
+                elif isinstance(dchild, QtWidget):
+                    action = dchild.get_action(False)
+                    if action is not None:
+                        return action
+            else:
+                found = dchild is child
+
     def child_added(self, child):
-        """ Handle the child added event for a WxSplitter.
+        """ Handle the child added event for a QtToolBar.
+
+        This handler will scan the children to find the proper point
+        at which to insert the action.
 
         """
-        super(WxSplitter, self).child_added(child)
-        if isinstance(child, WxSplitItem):
-            for index, dchild in enumerate(self.children()):
-                if child is dchild:
-                    self.widget.InsertWindow(index, child.widget)
-                    self.geometry_updated()
+        super(QtToolBar, self).child_added(child)
+        if isinstance(child, QtAction):
+            before = self.find_next_action(child)
+            self.widget.insertAction(before, child.widget)
+        elif isinstance(child, QtActionGroup):
+            before = self.find_next_action(child)
+            self.widget.insertActions(before, child.actions())
+        elif isinstance(child, QtWidget):
+            before = self.find_next_action(child)
+            self.widget.insertAction(before, child.get_action(True))
 
     def child_removed(self, child):
-        """ Handle the child removed event for a WxSplitter.
+        """  Handle the child removed event for a QtToolBar.
 
         """
-        super(WxSplitter, self).child_removed(child)
-        if isinstance(child, WxSplitItem):
-            widget = child.widget
-            self.widget.DetachWindow(widget)
-            widget.Hide()
-            self.geometry_updated()
+        super(QtToolBar, self).child_removed(child)
+        if isinstance(child, QtAction):
+            self.widget.removeAction(child.widget)
+        elif isinstance(child, QtActionGroup):
+            self.widget.removeActions(child.actions())
+        elif isinstance(child, QtWidget):
+            self.widget.removeAction(child.get_action(False))
 
     #--------------------------------------------------------------------------
-    # Utility Methods
+    # Signal Handlers
     #--------------------------------------------------------------------------
-    def split_items(self):
-        """ Get the split items defined for the widget.
+    def on_floated(self):
+        """ The signal handler for the 'floated' signal.
 
         """
-        for d in self.declaration.split_items():
-            yield d.proxy.widget or None
+        if not self._guard & FLOATED_GUARD:
+            self._guard |= FLOATED_GUARD
+            try:
+                self.declaration.floating = True
+            finally:
+                self._guard &= ~FLOATED_GUARD
+
+    def on_docked(self, area):
+        """ The signal handler for the 'docked' signal.
+
+        """
+        if not self._guard & FLOATED_GUARD:
+            self._guard |= FLOATED_GUARD
+            try:
+                self.declaration.floating = False
+                self.declaration.dock_area = DOCK_AREAS_INV[area]
+            finally:
+                self._guard &= ~FLOATED_GUARD
 
     #--------------------------------------------------------------------------
-    # ProxySplitter API
+    # ProxyToolBar API
     #--------------------------------------------------------------------------
-    def set_orientation(self, orientation):
-        """ Update the orientation of the splitter.
+    def set_button_style(self, style):
+        """ Set the button style for the toolbar.
 
         """
-        wx_orientation = _ORIENTATION_MAP[orientation]
-        widget = self.widget
-        with self.geometry_guard():
-            widget.SetOrientation(wx_orientation)
-            widget.SizeWindows()
+        self.widget.setToolButtonStyle(BUTTON_STYLES[style])
 
-    def set_live_drag(self, live_drag):
-        """ Updates the drag state of the splitter.
+    def set_movable(self, movable):
+        """ Set the movable state on the underlying widget.
 
         """
-        if live_drag:
-            self.widget.WindowStyle |= wx.SP_LIVE_UPDATE
-        else:
-            self.widget.WindowStyle &= ~wx.SP_LIVE_UPDATE
+        self.widget.setMovable(movable)
+
+    def set_floatable(self, floatable):
+        """ Set the floatable state on the underlying widget.
+
+        """
+        self.widget.setFloatable(floatable)
+
+    def set_floating(self, floating):
+        """ Set the floating staet on the underlying widget.
+
+        """
+        if not self._guard & FLOATED_GUARD:
+            self._guard |= FLOATED_GUARD
+            try:
+                self.widget.setFloating(floating)
+            finally:
+                self._guard &= ~FLOATED_GUARD
+
+    def set_dock_area(self, dock_area):
+        """ Set the dock area on the underyling widget.
+
+        """
+        self.widget.setToolBarArea(DOCK_AREAS[dock_area])
+
+    def set_allowed_dock_areas(self, dock_areas):
+        """ Set the allowed dock areas on the underlying widget.
+
+        """
+        qt_areas = Qt.NoToolBarArea
+        for area in dock_areas:
+            qt_areas |= DOCK_AREAS[area]
+        self.widget.setAllowedAreas(qt_areas)
+
+    def set_orientation(self, orientation):
+        """ Set the orientation of the underlying widget.
+
+        """
+        # If the tool bar is a child of a QMainWindow, then that window
+        # will take control of setting its orientation and changes to
+        # the orientation by the user must be ignored.
+        widget = self.widget
+        parent = widget.parent()
+        if not isinstance(parent, QMainWindow):
+            widget.setOrientation(ORIENTATIONS[orientation])
```

### Comparing `enaml-0.9.7/enaml/wx/wx_progress_bar.py` & `enaml-0.9.8/enaml/qt/qt_label.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,97 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-
 from atom.api import Typed
 
-from enaml.widgets.progress_bar import ProxyProgressBar
+from enaml.widgets.label import ProxyLabel
+
+from .QtCore import Qt
+from .QtGui import QLabel
+
+from .qt_control import QtControl
+
+
+ALIGN_MAP = {
+    'left': Qt.AlignLeft,
+    'right': Qt.AlignRight,
+    'center': Qt.AlignHCenter,
+    'justify': Qt.AlignJustify,
+}
+
 
-from .wx_control import WxControl
+VERTICAL_ALIGN_MAP = {
+    'top': Qt.AlignTop,
+    'bottom': Qt.AlignBottom,
+    'center': Qt.AlignVCenter,
+}
 
 
-class WxProgressBar(WxControl, ProxyProgressBar):
-    """ A Wx implementation of an Enaml ProxyProgressBar.
+class QtLabel(QtControl, ProxyLabel):
+    """ A Qt implementation of an Enaml ProxyLabel.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(wx.Gauge)
+    widget = Typed(QLabel)
 
     #--------------------------------------------------------------------------
-    # Setup Methods
+    # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying wx.Gauge widget.
+        """ Create the underlying label widget.
 
         """
-        self.widget = wx.Gauge(self.parent_widget())
+        self.widget = QLabel(self.parent_widget())
 
     def init_widget(self):
-        """ Create and initialize the progress bar control.
+        """ Initialize the underlying widget.
 
         """
-        super(WxProgressBar, self).init_widget()
+        super(QtLabel, self).init_widget()
         d = self.declaration
-        self.set_minimum(d.minimum)
-        self.set_maximum(d.maximum)
-        self.set_value(d.value)
-        self.set_text_visible(d.text_visible)
+        self.set_text(d.text)
+        self.set_align(d.align)
+        self.set_vertical_align(d.vertical_align)
+        self.widget.linkActivated.connect(self.on_link_activated)
 
     #--------------------------------------------------------------------------
-    # ProxyProgressBar API
+    # Signal Handlers
     #--------------------------------------------------------------------------
-    def set_minimum(self, value):
-        """ Set the minimum value of the progress bar
+    def on_link_activated(self, link):
+        """ Handle the link activated signal.
 
         """
-        d = self.declaration
-        self.widget.SetRange(d.maximum - value)
+        self.declaration.link_activated(link)
 
-    def set_maximum(self, value):
-        """ Set the maximum value of the progress bar
+    #--------------------------------------------------------------------------
+    # ProxyLabel API
+    #--------------------------------------------------------------------------
+    def set_text(self, text):
+        """ Set the text in the widget.
 
         """
-        d = self.declaration
-        self.widget.SetRange(value - d.minimum)
+        with self.geometry_guard():
+            self.widget.setText(text)
 
-    def set_value(self, value):
-        """ Set the value of the progress bar
+    def set_align(self, align):
+        """ Set the alignment of the text in the widget.
 
         """
-        d = self.declaration
-        self.widget.SetValue(value - d.minimum)
-
-    def set_text_visible(self, visible):
-        """ Set the text visibility on the widget.
+        widget = self.widget
+        alignment = widget.alignment()
+        alignment &= ~Qt.AlignHorizontal_Mask
+        alignment |= ALIGN_MAP[align]
+        widget.setAlignment(alignment)
 
-        This is not implemented on Wx.
+    def set_vertical_align(self, align):
+        """ Set the vertical alignment of the text in the widget.
 
         """
-        pass
+        widget = self.widget
+        alignment = widget.alignment()
+        alignment &= ~Qt.AlignVertical_Mask
+        alignment |= VERTICAL_ALIGN_MAP[align]
+        widget.setAlignment(alignment)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_resource_helpers.py` & `enaml-0.9.8/enaml/qt/q_resource_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,226 +1,233 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
+from enaml.fontext import FontStyle, FontCaps
 
-from enaml.fontext import FontStyle
+from .QtCore import Qt, QSize
+from .QtGui import QColor, QFont, QImage, QIcon, QPixmap
 
 
-FONT_STYLE = {
-    FontStyle.Normal: wx.FONTSTYLE_NORMAL,
-    FontStyle.Italic: wx.FONTSTYLE_ITALIC,
-    FontStyle.Oblique: wx.FONTSTYLE_SLANT,
-}
-
-
-# ASPECT_RATIO_MODE = {
-#     'ignore': Qt.IgnoreAspectRatio,
-#     'keep': Qt.KeepAspectRatio,
-#     'keep_by_expanding': Qt.KeepAspectRatioByExpanding
-# }
-
-
-# TRANSFORM_MODE = {
-#     'fast': Qt.FastTransformation,
-#     'smooth': Qt.SmoothTransformation
-# }
-
-
-# ICON_MODE = {
-#     'normal': QIcon.Normal,
-#     'disabled': QIcon.Disabled,
-#     'active': QIcon.Active,
-#     'selected': QIcon.Selected,
-# }
-
-
-# ICON_STATE = {
-#     'off': QIcon.Off,
-#     'on': QIcon.On,
-# }
-
-
-# def QImage_from_Image(image):
-#     """ Convert an Enaml Image into a QImage.
-
-#     Parameters
-#     ----------
-#     image : Image
-#         The Enaml Image object.
-
-#     Returns
-#     -------
-#     result : QImage
-#         The QImage instance for the given Enaml image.
-
-#     """
-#     format = image.format
-#     if format == 'auto':
-#         format = ''
-#     qimage = QImage.fromData(image.data, format)
-#     if -1 not in image.size and not qimage.isNull():
-#         qsize = QSize(*image.size)
-#         if qsize != qimage.size():
-#             mode = ASPECT_RATIO_MODE[image.aspect_ratio_mode]
-#             transform = TRANSFORM_MODE[image.transform_mode]
-#             qimage = qimage.scaled(qsize, mode, transform)
-#     return qimage
-
-
-# def get_cached_qimage(image):
-#     """ Get the cached QImage for the Enaml Image.
-
-#     Parameters
-#     ----------
-#     image : Image
-#         The Enaml Image object.
-
-#     Returns
-#     -------
-#     result : QImage
-#         The cached QImage for the image. If no cached image exists, one
-#         will be created.
-
-#     """
-#     qimage = image._tkdata
-#     if not isinstance(qimage, QImage):
-#         qimage = image._tkdata = QImage_from_Image(image)
-#     return qimage
-
-
-# def QIcon_from_Icon(icon):
-#     """ Convert the given Enaml Icon into a QIcon.
-
-#     Parameters
-#     ----------
-#     icon : Icon
-#         The Enaml Icon object.
-
-#     Returns
-#     -------
-#     result : QIcon
-#         The QIcon instance for the given Enaml icon.
-
-#     """
-#     qicon = QIcon()
-#     for icon_image in icon.images:
-#         image = icon_image.image
-#         if not image:
-#             continue
-#         mode = ICON_MODE[icon_image.mode]
-#         state = ICON_STATE[icon_image.state]
-#         qimage = get_cached_qimage(image)
-#         qpixmap = QPixmap.fromImage(qimage)
-#         qicon.addPixmap(qpixmap, mode, state)
-#     return qicon
-
-
-# def get_cached_qicon(icon):
-#     """ Get the cached QIcon for the Enaml Icon.
-
-#     Parameters
-#     ----------
-#     icon : Icon
-#         The Enaml Icon object.
-
-#     Returns
-#     -------
-#     result : QIcon
-#         The cached QIcon for the icon. If no cached icon exists, one
-#         will be created.
-
-#     """
-#     qicon = icon._tkdata
-#     if not isinstance(qicon, QIcon):
-#         qicon = icon._tkdata = QIcon_from_Icon(icon)
-#     return qicon
+FONT_STYLES = {
+    FontStyle.Normal: QFont.StyleNormal,
+    FontStyle.Italic: QFont.StyleItalic,
+    FontStyle.Oblique: QFont.StyleOblique,
+}
+
+
+FONT_CAPS = {
+    FontCaps.MixedCase: QFont.MixedCase,
+    FontCaps.AllUppercase: QFont.AllUppercase,
+    FontCaps.AllLowercase: QFont.AllLowercase,
+    FontCaps.SmallCaps: QFont.SmallCaps,
+    FontCaps.Capitalize: QFont.Capitalize,
+}
+
+
+ASPECT_RATIO_MODE = {
+    'ignore': Qt.IgnoreAspectRatio,
+    'keep': Qt.KeepAspectRatio,
+    'keep_by_expanding': Qt.KeepAspectRatioByExpanding
+}
+
+
+TRANSFORM_MODE = {
+    'fast': Qt.FastTransformation,
+    'smooth': Qt.SmoothTransformation
+}
+
+
+ICON_MODE = {
+    'normal': QIcon.Normal,
+    'disabled': QIcon.Disabled,
+    'active': QIcon.Active,
+    'selected': QIcon.Selected,
+}
+
+
+ICON_STATE = {
+    'off': QIcon.Off,
+    'on': QIcon.On,
+}
 
 
-def wxColor_from_Color(color):
-    """ Convert the given Enaml Color into a wxColor.
+def QImage_from_Image(image):
+    """ Convert an Enaml Image into a QImage.
+
+    Parameters
+    ----------
+    image : Image
+        The Enaml Image object.
+
+    Returns
+    -------
+    result : QImage
+        The QImage instance for the given Enaml image.
+
+    """
+    format = image.format
+    if format == 'argb32':
+        w, h = image.raw_size
+        qimage = QImage(image.data, w, h, QImage.Format_ARGB32)
+    else:
+        if format == 'auto':
+            format = ''
+        qimage = QImage.fromData(image.data, format)
+    if -1 not in image.size and not qimage.isNull():
+        qsize = QSize(*image.size)
+        if qsize != qimage.size():
+            mode = ASPECT_RATIO_MODE[image.aspect_ratio_mode]
+            transform = TRANSFORM_MODE[image.transform_mode]
+            qimage = qimage.scaled(qsize, mode, transform)
+    return qimage
+
+
+def get_cached_qimage(image):
+    """ Get the cached QImage for the Enaml Image.
+
+    Parameters
+    ----------
+    image : Image
+        The Enaml Image object.
+
+    Returns
+    -------
+    result : QImage
+        The cached QImage for the image. If no cached image exists, one
+        will be created.
+
+    """
+    qimage = image._tkdata
+    if not isinstance(qimage, QImage):
+        qimage = image._tkdata = QImage_from_Image(image)
+    return qimage
+
+
+def QIcon_from_Icon(icon):
+    """ Convert the given Enaml Icon into a QIcon.
+
+    Parameters
+    ----------
+    icon : Icon
+        The Enaml Icon object.
+
+    Returns
+    -------
+    result : QIcon
+        The QIcon instance for the given Enaml icon.
+
+    """
+    qicon = QIcon()
+    for icon_image in icon.images:
+        image = icon_image.image
+        if not image:
+            continue
+        mode = ICON_MODE[icon_image.mode]
+        state = ICON_STATE[icon_image.state]
+        qimage = get_cached_qimage(image)
+        qpixmap = QPixmap.fromImage(qimage)
+        qicon.addPixmap(qpixmap, mode, state)
+    return qicon
+
+
+def get_cached_qicon(icon):
+    """ Get the cached QIcon for the Enaml Icon.
+
+    Parameters
+    ----------
+    icon : Icon
+        The Enaml Icon object.
+
+    Returns
+    -------
+    result : QIcon
+        The cached QIcon for the icon. If no cached icon exists, one
+        will be created.
+
+    """
+    qicon = icon._tkdata
+    if not isinstance(qicon, QIcon):
+        qicon = icon._tkdata = QIcon_from_Icon(icon)
+    return qicon
+
+
+def QColor_from_Color(color):
+    """ Convert the given Enaml Color into a QColor.
 
     Parameters
     ----------
     color : Color
         The Enaml Color object.
 
     Returns
     -------
-    result : wxColor
-        The wxColor instance for the given Enaml color.
+    result : QColor
+        The QColor instance for the given Enaml color.
 
     """
-    return wx.Color(color.red, color.green, color.blue, color.alpha)
+    return QColor.fromRgba(color.argb)
 
 
-def get_cached_wxcolor(color):
+def get_cached_qcolor(color):
     """ Get the cached QColor for the Enaml Color.
 
     Parameters
     ----------
     color : Color
         The Enaml Color object.
 
     Returns
     -------
     result : QColor
         The cached QColor for the color. If no cached color exists, one
         will be created.
 
     """
-    wxcolor = color._tkdata
-    if not isinstance(wxcolor, wx.Color):
-        wxcolor = color._tkdata = wxColor_from_Color(color)
-    return wxcolor
+    qcolor = color._tkdata
+    if not isinstance(qcolor, QColor):
+        qcolor = color._tkdata = QColor_from_Color(color)
+    return qcolor
 
 
-def wxFont_from_Font(font):
-    """ Convert the given Enaml Font into a wxFont.
+def QFont_from_Font(font):
+    """ Convert the given Enaml Font into a QFont.
 
     Parameters
     ----------
     font : Font
         The Enaml Font object.
 
     Returns
     -------
-    result : wxFont
-        The wxFont instance for the given Enaml font.
+    result : QFont
+        The QFont instance for the given Enaml font.
 
     """
-    wxstyle = FONT_STYLE[font.style]
-    if font.weight < 50:
-        wxweight = wx.FONTWEIGHT_LIGHT
-    elif font.weight >= 75:
-        wxweight = wx.FONTWEIGHT_BOLD
-    else:
-        wxweight = wx.FONTWEIGHT_NORMAL
-    wxfamily = wx.FONTFAMILY_DEFAULT
-    wxfont = wx.Font(font.pointsize, wxfamily, wxstyle, wxweight)
-    wxfont.SetFaceName(font.family)
-    return wxfont
+    qfont = QFont(font.family, font.pointsize, font.weight)
+    qfont.setStyle(FONT_STYLES[font.style])
+    qfont.setCapitalization(FONT_CAPS[font.caps])
+    return qfont
 
 
-def get_cached_wxfont(font):
-    """ Get the cached wxFont for the Enaml Font.
+def get_cached_qfont(font):
+    """ Get the cached QFont for the Enaml Font.
 
     Parameters
     ----------
     font : Font
         The Enaml Font object.
 
     Returns
     -------
-    result : wxFont
-        The cached wxFont for the font. If no cached font exists, one
+    result : QFont
+        The cached QFont for the font. If no cached font exists, one
         will be created.
 
     """
-    wxfont = font._tkdata
-    if not isinstance(wxfont, wx.Font):
-        wxfont = font._tkdata = wxFont_from_Font(font)
-    return wxfont
+    qfont = font._tkdata
+    if not isinstance(qfont, QFont):
+        qfont = font._tkdata = QFont_from_Font(font)
+    return qfont
```

### Comparing `enaml-0.9.7/enaml/wx/wx_container.py` & `enaml-0.9.8/enaml/qt/qt_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,67 +4,72 @@
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 from collections import deque
 from contextlib import contextmanager
 
-import wx
-
-from atom.api import Atom, Bool, Callable, Float, Typed
+from atom.api import Atom, Callable, Float, Typed
 
 from enaml.layout.layout_manager import LayoutItem, LayoutManager
 from enaml.widgets.constraints_widget import ConstraintsWidget
 from enaml.widgets.container import ProxyContainer
 
-from .wx_constraints_widget import WxConstraintsWidget
-from .wx_frame import WxFrame
+from .QtCore import QRect, QSize, QTimer, Signal
+from .QtGui import QFrame, QWidgetItem, QSizePolicy
+
+from .qt_constraints_widget import QtConstraintsWidget
+from .qt_frame import QtFrame
 
 
 # Commonly used default sizes
-DEFAULT_BEST_SIZE = wx.Size(-1, -1)
-DEFAULT_MIN_SIZE = wx.Size(0, 0)
-DEFAULT_MAX_SIZE = wx.Size(16777215, 16777215)
+DEFAULT_BEST_SIZE = QSize(-1, -1)
+DEFAULT_MIN_SIZE = QSize(0, 0)
+DEFAULT_MAX_SIZE = QSize(16777215, 16777215)
+
+# The size policy to apply to containers. This allows the container
+# to behave properly when added to standard Qt layouts and widgets.
+CONTAINER_POLICY = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
 
 class LayoutPoint(Atom):
     """ A class which represents a point in layout space.
 
     """
     #: The x-coordinate of the point.
     x = Float(0.0)
 
     #: The y-coordinate of the point.
     y = Float(0.0)
 
 
-class WxLayoutItem(LayoutItem):
-    """ A concrete LayoutItem implementation for a WxConstraintsWidget.
+class QtLayoutItem(LayoutItem):
+    """ A concrete LayoutItem implementation for a QtConstraintsWidget.
 
     """
     #: The constraints widget declaration object for the layout item.
     declaration = Typed(ConstraintsWidget)
 
-    #: The underlying widget for the layout item.
-    widget = Typed(wx.Window)
+    #: The widget item used for laying out the underlying widget.
+    widget_item = Typed(QWidgetItem)
 
     #: The layout point which represents the offset of the parent item
     #: from the origin of the root item.
     offset = Typed(LayoutPoint)
 
     #: The layout point which represents the offset of this item from
     #: the offset of the root item.
     origin = Typed(LayoutPoint)
 
     def constrainable(self):
         """ Get a reference to the underlying constrainable object.
 
         Returns
         -------
-        result : Contrainable
+        result : Constrainable
             An object which implements the Constrainable interface.
 
         """
         return self.declaration
 
     def margins(self):
         """ Get the margins for the underlying widget.
@@ -83,47 +88,47 @@
         Returns
         -------
         result : tuple
             A 2-tuple of numbers representing the (width, height)
             size hint of the widget.
 
         """
-        hint = self.widget.GetBestSize()
-        return (hint.width, hint.height)
+        hint = self.widget_item.sizeHint()
+        return (hint.width(), hint.height())
 
     def min_size(self):
         """ Get the minimum size for the underlying widget.
 
         Returns
         -------
         result : tuple
             A 2-tuple of numbers representing the (width, height)
             min size of the widget. If any value is less than zero,
             constraints will not be generated for that dimension.
 
         """
-        min_size = self.widget.GetMinSize()
+        min_size = self.widget_item.widget().minimumSize()
         if min_size != DEFAULT_MIN_SIZE:
-            return (min_size.width, min_size.height)
+            return (min_size.width(), min_size.height())
         return (-1, -1)
 
     def max_size(self):
         """ Get the maximum size for the underlying widget.
 
         Returns
         -------
         result : tuple
             A 2-tuple of numbers representing the (width, height)
             max size of the widget. If any value is less than zero,
             constraints will not be generated for that dimension.
 
         """
-        max_size = self.widget.GetMaxSize()
+        max_size = self.widget_item.widget().maximumSize()
         if max_size != DEFAULT_MAX_SIZE:
-            return (max_size.width, max_size.height)
+            return (max_size.width(), max_size.height())
         return (-1, -1)
 
     def constraints(self):
         """ Get the user-defined constraints for the item.
 
         Returns
         -------
@@ -153,19 +158,19 @@
         """
         origin = self.origin
         origin.x = x
         origin.y = y
         offset = self.offset
         x -= offset.x
         y -= offset.y
-        self.widget.SetDimensions(x, y, width, height)
+        self.widget_item.setGeometry(QRect(x, y, width, height))
 
 
-class WxContainerItem(WxLayoutItem):
-    """ A WxLayoutItem subclass which handles container margins.
+class QtContainerItem(QtLayoutItem):
+    """ A QtLayoutItem subclass which handles container margins.
 
     """
     #: A callable used to get the container widget margins.
     margins_func = Callable()
 
     def margins(self):
         """ Get the margins for the underlying widget.
@@ -173,33 +178,33 @@
         Returns
         -------
         result : tuple
             A 4-tuple of ints representing the container margins.
 
         """
         a, b, c, d = self.declaration.padding
-        e, f, g, h = self.margins_func(self.widget)
+        e, f, g, h = self.margins_func(self.widget_item)
         return (a + e, b + f, c + g, d + h)
 
 
-class WxSharedContainerItem(WxContainerItem):
-    """ A WxContainerItem subclass which works for shared containers.
+class QtSharedContainerItem(QtContainerItem):
+    """ A QtContainerItem subclass which works for shared containers.
 
     """
     def size_hint_constraints(self):
         """ Get the size hint constraints for the item.
 
         A shared container does not generate size hint constraints.
 
         """
         return []
 
 
-class WxChildContainerItem(WxLayoutItem):
-    """ A WxLayoutItem subclass which works for child containers.
+class QtChildContainerItem(QtLayoutItem):
+    """ A QtLayoutItem subclass which works for child containers.
 
     """
     def constraints(self):
         """ Get the user constraints for the item.
 
         A child container does not expose its user defined constraints
         to the parent container.
@@ -207,188 +212,196 @@
         """
         return []
 
     def min_size(self):
         """ Get the minimum size for the underlying widget.
 
         The min size for a child container lives on the proxy object.
-        The widget limits must be bypassed for child container.
+        The QWidgetItem limits must be bypassed for child container.
 
         """
         min_size = self.declaration.proxy.min_size
         if min_size != DEFAULT_MIN_SIZE:
-            return (min_size.width, min_size.height)
+            return (min_size.width(), min_size.height())
         return (-1, -1)
 
     def max_size(self):
         """ Get the maximum size for the underlying widget.
 
         The max size for a child container lives on the proxy object.
-        The widget limits must be bypassed for child container.
+        The QWidgetItem limits must be bypassed for child container.
 
         """
         max_size = self.declaration.proxy.max_size
         if max_size != DEFAULT_MAX_SIZE:
-            return (max_size.width, max_size.height)
+            return (max_size.width(), max_size.height())
         return (-1, -1)
 
 
-class wxContainer(wx.PyPanel):
-    """ A subclass of wx.PyPanel which allows the default best size to
-    be overriden by calling SetBestSize.
-
-    This functionality is used by the WxContainer to override the
-    size hint with a value computed from the constraints layout
-    manager.
+class QContainer(QFrame):
+    """ A subclass of QFrame which behaves as a container.
 
     """
-    #: An invalid wx.Size used as the default value for class instances.
-    _best_size = wx.Size(-1, -1)
+    #: A signal which is emitted on a resize event.
+    resized = Signal()
 
-    def DoGetBestSize(self):
-        """ Reimplemented parent class method.
+    #: The internally cached size hint.
+    _size_hint = QSize()
 
-        This will return the best size as set by a call to SetBestSize.
-        If that is invalid, then the superclass' version will be used.
+    def resizeEvent(self, event):
+        """ Converts a resize event into a signal.
 
         """
-        size = self._best_size
-        if not size.IsFullySpecified():
-            size = super(wxContainer, self).DoGetBestSize()
-        return size
+        super(QContainer, self).resizeEvent(event)
+        self.resized.emit()
 
-    def SetBestSize(self, size):
-        """ Sets the best size to use for this container.
+    def sizeHint(self):
+        """ Returns the previously set size hint. If that size hint is
+        invalid, the superclass' sizeHint will be used.
 
         """
-        self._best_size = size
+        hint = self._size_hint
+        if not hint.isValid():
+            hint = super(QContainer, self).sizeHint()
+        return QSize(hint)
 
+    def setSizeHint(self, hint):
+        """ Sets the size hint to use for this widget.
 
-class wxLayoutTimer(wx.Timer):
-    """ A custom wx Timer which for collapsing layout requests.
+        """
+        self._size_hint = QSize(hint)
 
-    """
-    def __init__(self, owner):
-        super(wxLayoutTimer, self).__init__()
-        self.owner = owner
+    def minimumSizeHint(self):
+        """ Returns the minimum size hint for the widget.
 
-    def Notify(self):
-        self.owner._on_relayout_timer()
+        For a QContainer, the minimum size hint is equivalent to the
+        minimum size as computed by the layout manager.
+
+        """
+        return self.minimumSize()
 
 
-class WxContainer(WxFrame, ProxyContainer):
-    """ A Wx implementation of an Enaml ProxyContainer.
+class QtContainer(QtFrame, ProxyContainer):
+    """ A Qt implementation of an Enaml ProxyContainer.
 
     """
     #: A reference to the toolkit widget created by the proxy.
-    widget = Typed(wxContainer)
+    widget = Typed(QContainer)
 
     #: The minimum size of the container as computed by the layout
     #: manager. This will be updated on every relayout pass and is
-    #: used by the WxChildContainerItem to generate size constraints.
-    min_size = Typed(wx.Size)
+    #: used by the QtChildContainerItem to generate size constraints.
+    min_size = Typed(QSize)
 
     #: The maximum size of the container as computed by the layout
     #: manager. This will be updated on every relayout pass and is
-    #: used by the WxChildContainerItem to generate size constraints.
-    max_size = Typed(wx.Size)
+    #: used by the QtChildContainerItem to generate size constraints.
+    max_size = Typed(QSize)
 
     #: A timer used to collapse relayout requests. The timer is created
     #: on an as needed basis and destroyed when it is no longer needed.
-    _layout_timer = Typed(wxLayoutTimer)
+    _layout_timer = Typed(QTimer)
 
     #: The layout manager which handles the system of constraints.
     _layout_manager = Typed(LayoutManager)
 
-    #: Whether or not the current container is shown. This is toggled
-    #: by the EVT_SHOW handler.
-    _is_shown = Bool(True)
-
     def destroy(self):
         """ A reimplemented destructor.
 
         This destructor clears the layout timer and layout manager
         so that any potential reference cycles are broken.
 
         """
-        timer = self._layout_timer
-        if timer is not None:
-            timer.Stop()
-            del self._layout_timer
+        del self._layout_timer
         del self._layout_manager
-        super(WxContainer, self).destroy()
+        super(QtContainer, self).destroy()
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
         """ Creates the QContainer widget.
 
         """
-        self.widget = wxContainer(self.parent_widget())
+        widget = QContainer(self.parent_widget())
+        widget.setSizePolicy(CONTAINER_POLICY)
+        self.widget = widget
 
     def init_layout(self):
         """ Initialize the layout of the widget.
 
         """
-        super(WxContainer, self).init_layout()
+        super(QtContainer, self).init_layout()
         self._setup_manager()
         self._update_size_bounds()
         self._update_geometries()
-        widget = self.widget
-        widget.Bind(wx.EVT_SIZE, self._on_resized)
-        widget.Bind(wx.EVT_SHOW, self._on_shown)
+        self.widget.resized.connect(self._update_geometries)
+
+    #--------------------------------------------------------------------------
+    # Child Events
+    #--------------------------------------------------------------------------
+    def child_added(self, child):
+        """ Handle the child added event.
+
+        This handler will reparent the child if necessary.
+
+        """
+        super(QtContainer, self).child_added(child)
+        cw = child.widget
+        if cw is not None and cw.parent() != self.widget:
+            cw.setParent(self.widget)
 
     #--------------------------------------------------------------------------
     # Layout API
     #--------------------------------------------------------------------------
     def request_relayout(self):
         """ Request a relayout of the container.
 
         """
         # If this container owns the layout, (re)start the timer. The
-        # list of layout items is reset to prevent an edge case where
+        # list of layout items is cleared to prevent an edge case where
         # a parent container layout occurs before the child container,
         # causing the child to resize potentially deleted widgets which
         # still have strong refs in the layout items list.
         manager = self._layout_manager
         if manager is not None:
             if self._layout_timer is None:
                 manager.clear_items()
-                self.widget.Freeze()
-                self._layout_timer = wxLayoutTimer(self)
-            self._layout_timer.Start(1, oneShot=True)
+                self.widget.setUpdatesEnabled(False)
+                timer = self._layout_timer = QTimer()
+                timer.setSingleShot(True)
+                timer.timeout.connect(self._on_relayout_timer)
+            self._layout_timer.start()
             return
 
         # If an ancestor container owns the layout, proxy the call.
         container = self.layout_container
         if container is not None:
             container.request_relayout()
 
     def geometry_updated(self, item=None):
         """ Notify the layout system that the geometry has changed.
 
         Parameters
         ----------
-        item : WxConstraintsWidget, optional
+        item : QtConstraintsWidget, optional
             The constraints widget with the updated geometry. If this
             is None, it indicates that this container's geometry is
             the one which has changed.
 
         """
         # If this container's geometry has changed and it has an ancestor
         # layout container, notify that container since it cares about
         # this container's geometry. If the layout for this container is
         # shared, the layout item will take care of supplying the proper
         # list geometry constraints.
         container = self.layout_container
         if item is None:
             if container is not None:
                 container.geometry_updated(self)
-            self.post_wx_layout_request()
             return
 
         # If this container owns its layout, update the manager unless
         # a relayout is pending. A pending relayout means the manager
         # has already been reset and the layout indices are invalid.
         manager = self._layout_manager
         if manager is not None:
@@ -407,19 +420,19 @@
     def geometry_guard(self):
         """ A context manager for guarding the geometry of the widget.
 
         This is a reimplementation of the superclass method which uses
         the internally computed min and max size of the container.
 
         """
-        old_hint = self.widget.GetBestSize()
+        old_hint = self.widget.sizeHint()
         old_min = self.min_size
         old_max = self.max_size
         yield
-        if (old_hint != self.widget.GetBestSize() or
+        if (old_hint != self.widget.sizeHint() or
             old_min != self.min_size or
             old_max != self.max_size):
             self.geometry_updated()
 
     @staticmethod
     def margins_func(widget_item):
         """ Get the margins for the given widget item.
@@ -439,15 +452,15 @@
         return (0, 0, 0, 0)
 
     def margins_updated(self, item=None):
         """ Notify the layout system that the margins have changed.
 
         Parameters
         ----------
-        item : WxContainer, optional
+        item : QtContainer, optional
             The container widget with the updated margins. If this is
             None, it indicates that this container's margins are the
             ones which have changed.
 
         """
         # If this container owns its layout, update the manager unless
         # a relayout is pending. A pending relayout means the manager
@@ -464,56 +477,29 @@
 
         # If an ancestor container owns the layout, forward the call.
         container = self.layout_container
         if container is not None:
             container.margins_updated(item or self)
 
     #--------------------------------------------------------------------------
-    # Private Event Handlers
+    # Private Signal Handlers
     #--------------------------------------------------------------------------
-    def _on_resized(self, event):
-        """ The event handler for the EVT_SIZE event.
-
-        This triggers a geometry update for the decendant children.
-
-        """
-        if self._is_shown:
-            self._update_geometries()
-
-    def _on_shown(self, event):
-        """ The event handler for the EVT_SHOW event.
-
-        This handler toggles the value of the _is_shown flag.
-
-        """
-        # The EVT_SHOW event is not reliable. For example, it is not
-        # emitted on the children of widgets that were hidden. So, if
-        # this container is the child of, say, a notebook page, then
-        # the switching of tabs does not emit a show event. So, the
-        # notebook page must cooperatively emit a show event on this
-        # container. Therefore, we can't treat this event as a 'real'
-        # toolkit event, we just use it as a hint.
-        self._is_shown = shown = event.GetShow()
-        if shown:
-            self._update_geometries()
-
     def _on_relayout_timer(self):
         """ Rebuild the layout for the container.
 
         This method is invoked when the relayout timer is triggered. It
         will reset the manager and update the geometries of the children.
 
         """
-        self._layout_timer.Stop()
         del self._layout_timer
         with self.geometry_guard():
             self._setup_manager()
             self._update_size_bounds()
             self._update_geometries()
-        self.widget.Thaw()
+        self.widget.setUpdatesEnabled(True)
 
     #--------------------------------------------------------------------------
     # Private Layout Handling
     #--------------------------------------------------------------------------
     def _setup_manager(self):
         """ Setup the layout manager.
 
@@ -521,78 +507,75 @@
         it with a new layout table.
 
         """
         # Layout ownership can only be transferred *after* the init
         # layout method is called, as layout occurs bottom up. The
         # manager is only created if ownership is unlikely to change.
         share_layout = self.declaration.share_layout
-        if share_layout and isinstance(self.parent(), WxContainer):
-            timer = self._layout_timer
-            if timer is not None:
-                timer.Stop()
+        if share_layout and isinstance(self.parent(), QtContainer):
             del self._layout_timer
             del self._layout_manager
             return
 
         manager = self._layout_manager
         if manager is None:
-            item = WxContainerItem()
+            item = QtContainerItem()
             item.declaration = self.declaration
-            item.widget = self.widget
+            item.widget_item = QWidgetItem(self.widget)
             item.origin = LayoutPoint()
             item.offset = LayoutPoint()
             item.margins_func = self.margins_func
             manager = self._layout_manager = LayoutManager(item)
         manager.set_items(self._create_layout_items())
 
     def _update_geometries(self):
         """ Update the geometries of the layout children.
 
         This method will resize the layout manager to the container size.
 
         """
         manager = self._layout_manager
         if manager is not None:
-            width, height = self.widget.GetSizeTuple()
-            manager.resize(width, height)
+            widget = self.widget
+            manager.resize(widget.width(), widget.height())
 
     def _update_size_bounds(self):
-        """ Update the size bounds of the underlying container.
+        """ Update the sizes of the underlying container.
 
         This method will update the min, max, and best size of the
         container. It will not automatically trigger a geometry
         notification.
 
         """
         widget = self.widget
         manager = self._layout_manager
         if manager is None:
             best_size = DEFAULT_BEST_SIZE
             min_size = DEFAULT_MIN_SIZE
             max_size = DEFAULT_MAX_SIZE
         else:
-            best_size = wx.Size(*manager.best_size())
-            min_size = wx.Size(*manager.min_size())
-            max_size = wx.Size(*manager.max_size())
+            best_size = QSize(*manager.best_size())
+            min_size = QSize(*manager.min_size())
+            max_size = QSize(*manager.max_size())
 
         # Store the computed min and max size, which is used by the
-        # WxChildContainerItem to provide min and max size constraints.
+        # QtChildContainerItem to provide min and max size constraints.
         self.min_size = min_size
         self.max_size = max_size
 
         # If this is a child container, min and max size are not applied
         # to the widget since the ancestor manager must be the ultimate
-        # authority on layout size.
-        widget.SetBestSize(best_size)
-        if isinstance(self.parent(), WxContainer):
-            widget.SetMinSize(DEFAULT_MIN_SIZE)
-            widget.SetMaxSize(DEFAULT_MAX_SIZE)
+        # authority on layout size, not QWidgetItem.
+        widget.setSizeHint(best_size)
+        if isinstance(self.parent(), QtContainer):
+            widget.setMinimumSize(DEFAULT_MIN_SIZE)
+            widget.setMaximumSize(DEFAULT_MAX_SIZE)
         else:
-            widget.SetMinSize(min_size)
-            widget.SetMaxSize(max_size)
+            widget.setMinimumSize(min_size)
+            widget.setMaximumSize(max_size)
 
     def _create_layout_items(self):
         """ Create a layout items for the container decendants.
 
         The layout items are created by traversing the decendants in
         breadth-first order and setting up a LayoutItem object for
         each decendant. The layout item is populated with an offset
@@ -608,27 +591,27 @@
 
         """
         layout_items = []
         offset = LayoutPoint()
         queue = deque((offset, child) for child in self.children())
         while queue:
             offset, child = queue.popleft()
-            if isinstance(child, WxConstraintsWidget):
+            if isinstance(child, QtConstraintsWidget):
                 child.layout_container = self
                 origin = LayoutPoint()
-                if isinstance(child, WxContainer):
+                if isinstance(child, QtContainer):
                     if child.declaration.share_layout:
-                        item = WxSharedContainerItem()
+                        item = QtSharedContainerItem()
                         item.margins_func = child.margins_func
                         for subchild in child.children():
                             queue.append((origin, subchild))
                     else:
-                        item = WxChildContainerItem()
+                        item = QtChildContainerItem()
                 else:
-                    item = WxLayoutItem()
+                    item = QtLayoutItem()
                 item.declaration = child.declaration
-                item.widget = child.widget
+                item.widget_item = QWidgetItem(child.widget)
                 item.offset = offset
                 item.origin = origin
                 child.layout_index = len(layout_items)
                 layout_items.append(item)
         return layout_items
```

### Comparing `enaml-0.9.7/enaml/wx/wx_split_item.py` & `enaml-0.9.8/enaml/qt/qt_popup_view.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,166 +1,182 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-
 from atom.api import Typed
 
-from enaml.widgets.split_item import ProxySplitItem
+from enaml.widgets.popup_view import ProxyPopupView
 
-from .wx_single_widget_sizer import wxSingleWidgetSizer
-from .wx_container import WxContainer
-from .wx_widget import WxWidget
+from .QtCore import Qt, QPointF, QPoint
 
+from .q_popup_view import QPopupView, ArrowEdge, AnchorMode
+from .qt_widget import QtWidget
 
-class wxSplitItem(wx.Panel):
-    """ A wxPanel subclass which acts as an item in a wxSplitter.
 
-    """
-    def __init__(self, parent):
-        """ Initialize a wxSplitItem.
+EDGES = {
+    'left': ArrowEdge.Left,
+    'right': ArrowEdge.Right,
+    'top': ArrowEdge.Top,
+    'bottom': ArrowEdge.Bottom,
+}
 
-        Parameters
-        ----------
-        parent : wx.Window
-            The parent widget of the split item.
-
-        """
-        super(wxSplitItem, self).__init__(parent)
-        self._split_widget = None
-        self._stretch = 0
-        self.SetSizer(wxSingleWidgetSizer())
 
-    def GetSplitWidget(self):
-        """ Get the split widget for this split item.
+WINDOW_TYPES = {
+    'popup': Qt.Popup,
+    'tool_tip': Qt.ToolTip,
+    'window': Qt.Window,
+}
 
-        Returns
-        -------
-        result : wxWindow or None
-            The split widget being managed by this item.
 
-        """
-        return self._split_widget
-
-    def SetSplitWidget(self, widget):
-        """ Set the split widget for this split item.
+ANCHOR_MODE = {
+    'parent': AnchorMode.Parent,
+    'cursor': AnchorMode.Cursor,
+}
 
-        Parameters
-        ----------
-        widget : wxWindow
-            The wxWindow to use as the split widget in this item.
 
-        """
-        self._split_widget = widget
-        self.GetSizer().Add(widget)
-
-    def GetStretch(self):
-        """ Get the stretch factor for the widget.
-
-        Returns
-        -------
-        result : int
-            The stretch factor for the widget.
-
-        """
-        return self._stretch
-
-    def SetStretch(self, stretch):
-        """ Set the stretch factor for the widget.
-
-        Parameters
-        ----------
-        stretch : int
-            The stretch factor for the widget.
-
-        """
-        self._stretch = stretch
-
-
-class WxSplitItem(WxWidget, ProxySplitItem):
-    """ A Wx implementation of an Enaml ProxySplitItem.
+class QtPopupView(QtWidget, ProxyPopupView):
+    """ A Qt implementation of an Enaml ProxyPopupView.
 
     """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(wxSplitItem)
+    #: A reference to the toolkit widget created by the proxy.
+    widget = Typed(QPopupView)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying QStackItem widget.
+        """ Create the QPopupView widget.
 
         """
-        self.widget = wxSplitItem(self.parent_widget())
+        d = self.declaration
+        flags = WINDOW_TYPES[d.window_type]
+        self.widget = QPopupView(self.parent_widget(), flags)
+        if d.translucent_background:
+            self.widget.setAttribute(Qt.WA_TranslucentBackground)
 
     def init_widget(self):
-        """ Initialize the underyling widget.
+        """ Initialize the widget.
 
         """
-        super(WxSplitItem, self).init_widget()
+        super(QtPopupView, self).init_widget()
         d = self.declaration
-        self.set_stretch(d.stretch)
-        self.set_collapsible(d.collapsible)
+        self.set_anchor(d.anchor)
+        self.set_anchor_mode(d.anchor_mode)
+        self.set_parent_anchor(d.parent_anchor)
+        self.set_arrow_size(d.arrow_size)
+        self.set_arrow_edge(d.arrow_edge)
+        self.set_offset(d.offset)
+        self.set_timeout(d.timeout)
+        self.set_fade_in_duration(d.fade_in_duration)
+        self.set_fade_out_duration(d.fade_out_duration)
+        self.set_close_on_click(d.close_on_click)
+        self.widget.closed.connect(self.on_closed)
 
     def init_layout(self):
-        """ Initialize the layout for the underyling widget.
+        """ Initialize the widget layout.
 
         """
-        super(WxSplitItem, self).init_layout()
-        self.widget.SetSplitWidget(self.split_widget())
+        super(QtPopupView, self).init_layout()
+        self.widget.setCentralWidget(self.central_widget())
 
     #--------------------------------------------------------------------------
-    # Utility Methods
+    # Public API
     #--------------------------------------------------------------------------
-    def split_widget(self):
-        """ Find and return the split widget child for this widget.
+    def central_widget(self):
+        """ Find and return the central widget child for this widget.
 
         Returns
         -------
-        result : wxWindow or None
-            The split widget defined for this widget, or None if one is
-            not defined.
+        result : QWidget or None
+            The central widget defined for this widget, or None if one
+            is not defined.
 
         """
-        d = self.declaration.split_widget()
+        d = self.declaration.central_widget()
         if d is not None:
-            return d.proxy.widget or None
+            return d.proxy.widget
 
     #--------------------------------------------------------------------------
-    # Child Events
+    # Signal Handlers
     #--------------------------------------------------------------------------
-    def child_added(self, child):
-        """ Handle the child added event for a WxSplitItem.
-
-        """
-        super(WxSplitItem, self).child_added(child)
-        if isinstance(child, WxContainer):
-            self.widget.SetSplitWidget(self.split_widget())
+    def on_closed(self):
+        """ The signal handler for the 'closed' signal.
 
-    def child_removed(self, child):
-        """ Handle the child removed event for a WxSplitItem.
+        This handler will notify the declaration object that the popup
+        view has closed.
 
         """
-        super(WxSplitItem, self).child_removed(child)
-        if isinstance(child, WxContainer):
-            self.widget.SetSplitWidget(self.split_widget())
+        d = self.declaration
+        if d is not None:
+            d._popup_closed()
 
     #--------------------------------------------------------------------------
-    # ProxySplitItem API
+    # ProxyBubbleView API
     #--------------------------------------------------------------------------
-    def set_stretch(self, stretch):
-        """ Set the stretch factor for the underlying widget.
+    def set_anchor(self, anchor):
+        """ Set the anchor location on the underlying widget.
+
+        """
+        self.widget.setAnchor(QPointF(*anchor))
+
+    def set_anchor_mode(self, mode):
+        """ Set the anchor mode on the underlying widget.
 
         """
-        self.widget.SetStretch(stretch)
+        self.widget.setAnchorMode(ANCHOR_MODE[mode])
 
-    def set_collapsible(self, collapsible):
-        """ Set the collapsible flag for the underlying widget.
+    def set_parent_anchor(self, anchor):
+        """ Set the parent anchor location on the underlying widget.
+
+        """
+        self.widget.setParentAnchor(QPointF(*anchor))
+
+    def set_arrow_size(self, size):
+        """ Set the size of the arrow on the underlying widget.
+
+        """
+        self.widget.setArrowSize(size)
+
+    def set_arrow_edge(self, edge):
+        """ Set the arrow edge on the underlying widget.
+
+        """
+        self.widget.setArrowEdge(EDGES[edge])
+
+    def set_offset(self, offset):
+        """ Set the offset of the underlying widget.
+
+        """
+        self.widget.setOffset(QPoint(*offset))
+
+    def set_timeout(self, timeout):
+        """ Set the timeout for the underlying widget.
+
+        """
+        self.widget.setTimeout(timeout)
+
+    def set_fade_in_duration(self, duration):
+        """ Set the fade in duration for the underlying widget.
+
+        """
+        self.widget.setFadeInDuration(duration)
+
+    def set_fade_out_duration(self, duration):
+        """ Set the fade out duration for the underlying widget.
+
+        """
+        self.widget.setFadeOutDuration(duration)
+
+    def set_close_on_click(self, enable):
+        """ Set the close on click flag for the underlying widget.
+
+        """
+        self.widget.setCloseOnClick(enable)
 
-        This is not supported on wx.
+    def close(self):
+        """ Close the underlying popup widget.
 
         """
-        pass
+        self.widget.close()
```

### Comparing `enaml-0.9.7/enaml/wx/wx_tool_bar.py` & `enaml-0.9.8/enaml/qt/docking/q_dock_area.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,463 +1,459 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
+from enaml.qt.QtCore import QMargins, QSize, QEvent
+from enaml.qt.QtGui import (
+    QFrame, QLayout, QTabWidget, QGridLayout, QStackedLayout, QVBoxLayout,
+    QWidget, QStyle, QStyleOption
+)
 
-from atom.api import Typed
+from .q_dock_bar import QDockBarManager
 
-from enaml.widgets.tool_bar import ProxyToolBar
 
-from .wx_action import WxAction, EVT_ACTION_CHANGED
-from .wx_action_group import WxActionGroup
-from .wx_constraints_widget import WxConstraintsWidget
+class QDockAreaLayout(QStackedLayout):
+    """ A custom stacked layout for the QDockArea.
 
+    This stacked layout reports its size hints according to the widget
+    which is currently visible, as opposed to aggregated hints which is
+    the default.
 
-#: A mapping from Enaml orientation to wx Orientation
-_ORIENTATION_MAP = {
-    'horizontal': wx.HORIZONTAL,
-    'vertical': wx.VERTICAL,
-}
+    """
+    def sizeHint(self):
+        """ Get the size hint for the layout.
+
+        """
+        widget = self.currentWidget()
+        if widget is not None:
+            return widget.sizeHint()
+        return QSize(256, 192)
+
+    def minimumSize(self):
+        """ Get the minimum size for the layout.
+
+        """
+        widget = self.currentWidget()
+        if widget is not None:
+            return widget.minimumSizeHint()
+        return QSize(256, 192)
 
 
-class wxToolBar(wx.ToolBar):
-    """ A wx.ToolBar subclass which handles wxAction instances.
+class QDockArea(QFrame):
+    """ A custom QFrame which provides an area for docking QDockItems.
+
+    A dock area is used by creating QDockItem instances using the dock
+    area as the parent. A DockLayout instance can then be created and
+    applied to the dock area with the 'setDockLayout' method. The names
+    in the DockLayoutItem objects are used to find the matching dock
+    item widget child.
 
     """
-    def __init__(self, *args, **kwargs):
-        """ Initialize a wxToolBar.
+    def __init__(self, parent=None):
+        """ Initialize a QDockArea.
 
         Parameters
         ----------
-        *args, **kwargs
-            The position and keyword arguments needed to initialize
-            an AuiToolBar.
+        parent : QWidget
+            The parent of the dock area.
 
         """
-        super(wxToolBar, self).__init__(*args, **kwargs)
-        self._all_items = []
-        self._actions_map = {}
+        super(QDockArea, self).__init__(parent)
+        self._dock_bar_manager = QDockBarManager(self)
+        self._primary_pane = primary_pane = QWidget(self)
+        self._central_pane = central_pane = QWidget(primary_pane)
+        self._dock_events_enabled = False
+        self._opaque_resize = None
+        self._tab_position = None
+
+        central_layout = QVBoxLayout()
+        central_layout.setContentsMargins(QMargins(0, 0, 0, 0))
+        central_layout.setSizeConstraint(QLayout.SetMinimumSize)
+        central_pane.setLayout(central_layout)
+
+        grid_layout = QGridLayout()
+        grid_layout.setRowStretch(0, 0)
+        grid_layout.setRowStretch(1, 1)
+        grid_layout.setRowStretch(2, 0)
+        grid_layout.setColumnStretch(0, 0)
+        grid_layout.setColumnStretch(1, 1)
+        grid_layout.setColumnStretch(2, 0)
+        grid_layout.setContentsMargins(QMargins(0, 0, 0, 0))
+        grid_layout.setSizeConstraint(QLayout.SetMinimumSize)
+        grid_layout.addWidget(central_pane, 1, 1)
+        primary_pane.setLayout(grid_layout)
+
+        area_layout = QDockAreaLayout()
+        area_layout.setContentsMargins(QMargins(0, 0, 0, 0))
+        area_layout.setSizeConstraint(QLayout.SetMinimumSize)
+        area_layout.insertWidget(0, primary_pane)
+        self.setLayout(area_layout)
+        self.updateSpacing()
 
     #--------------------------------------------------------------------------
-    # Private API
+    # Protected API
     #--------------------------------------------------------------------------
-    def _InsertAction(self, index, action):
-        """ Insert a new tool into the tool bar for the given action.
+    def event(self, event):
+        """ A generic event handler for the dock area.
 
-        Parameters
-        ----------
-        action : wxAction
-            The wxAction instance to add to the tool bar.
-
-        Returns
-        -------
-        result : wxToolBarToolBase
-            The tool base item created when adding the control to the
-            tool bar.
-
-        """
-        if action.IsSeparator():
-            item = self.InsertSeparator(index)
-        else:
-            text = action.GetText()
-            short_help = action.GetToolTip()
-            long_help = action.GetStatusTip()
-            action_id = action.GetId()
-            bmp = wx.EmptyBitmap(0, 0)
-            if action.IsCheckable():
-                item = self.InsertLabelTool(
-                    index, action_id, text, bmp, kind=wx.ITEM_CHECK,
-                    shortHelp=short_help, longHelp=long_help,
-                )
-                if action.IsChecked() != item.IsToggled():
-                    item.Toggle()
-            else:
-                item = self.InsertLabelTool(
-                    index, action_id, text, bmp, kind=wx.ITEM_NORMAL,
-                    shortHelp=short_help, longHelp=long_help,
-                )
-            item.Enable(action.IsEnabled())
-        return item
-
-    def OnActionChanged(self, event):
-        """ The event handler for the EVT_ACTION_CHANGED event.
-
-        This handler will be called when a child action changes. It
-        ensures that the new state of the child action is in sync with
-        the associated tool bar item.
-
-        """
-        event.Skip()
-        action = event.GetEventObject()
-        item = self._actions_map.get(action)
-
-        # Handle a visibility change. The tool must be added/removed.
-        visible = action.IsVisible()
-        if visible != bool(item):
-            if visible:
-                index = self._all_items.index(action)
-                index = min(index, len(self._actions_map))
-                new_item = self._InsertAction(index, action)
-                self._actions_map[action] = new_item
-                self.Realize()
-            else:
-                self.DeleteTool(item.GetId())
-                del self._actions_map[action]
-            return
-
-        # If the item is invisible, there is nothing to update.
-        if not item:
-            return
-
-        # Handle a separator change. The existing tool must be replaced.
-        if action.IsSeparator() != item.IsSeparator():
-            self.DeleteTool(item.GetId())
-            del self._actions_map[action]
-            index = self._all_items.index(action)
-            index = min(index, len(self._actions_map))
-            new_item = self._InsertAction(index, action)
-            self._actions_map[action] = new_item
-            self.Realize()
-            return
-
-        # Handle a checkable change. The existing too must be replaced.
-        if action.IsCheckable() != item.CanBeToggled():
-            self.DeleteTool(item.GetId())
-            del self._actions_map[action]
-            index = self._all_items.index(action)
-            index = min(index, len(self._actions_map))
-            new_item = self._InsertAction(index, action)
-            self._actions_map[action] = new_item
-            self.Realize()
-            return
-
-        # All other state can be updated in-place.
-        item.SetLabel(action.GetText())
-        item.SetShortHelp(action.GetToolTip())
-        item.SetLongHelp(action.GetStatusTip())
-        if action.IsCheckable():
-            if action.IsChecked() != item.IsToggled():
-                item.Toggle()
-        item.Enable(action.IsEnabled())
-        self.Realize()
+        """
+        if event.type() == QEvent.StyleChange:
+            self.updateSpacing()
+        return super(QDockArea, self).event(event)
 
     #--------------------------------------------------------------------------
     # Public API
     #--------------------------------------------------------------------------
-    def AddAction(self, action, realize=True):
-        """ Add an action to the tool bar.
+    def updateSpacing(self):
+        """ Update the primary layout spacing for the dock area.
 
-        If the action already exists in the toolbar, it will be moved
-        to the end.
+        This method will extract spacing value defined in the style
+        sheet for the dock area and apply it to the spacing between
+        the dock bars and the central widget.
+
+        """
+        opt = QStyleOption()
+        opt.initFrom(self)
+        style = self.style()
+        # hack to get the style sheet 'spacing' property.
+        spacing = style.pixelMetric(QStyle.PM_ToolBarItemSpacing, opt, self)
+        grid_layout = self._primary_pane.layout()
+        grid_layout.setVerticalSpacing(spacing)
+        grid_layout.setHorizontalSpacing(spacing)
 
-        Parameters
-        ----------
-        action : wxAction
-            The wxAction instance to add to the tool bar.
+    def centralPane(self):
+        """ Get the central pane for the dock area.
 
-        realize : bool, optional
-            Whether the toolbar should realize the change immediately.
-            If False, Realize() will need to be called manually once
-            all desired changes have been made. The default is True.
+        This method is used the dock bar manager to access the central
+        layout pane. It should not normally be called by user code.
+
+        Returns
+        -------
+        result : QWidget
+            The central pane for the dock area.
 
         """
-        self.InsertAction(None, action, realize)
+        return self._central_pane
 
-    def AddActions(self, actions, realize=True):
-        """ Add multiple wx actions to the tool bar.
+    def primaryPane(self):
+        """ Get the primary pane for the dock area.
 
-        If an action already exists in the tool bar, it will be moved
-        to the end.
+        This method is used the dock bar manager to access the primary
+        layout pane. It should not normally be called by user code.
 
-        Parameters
-        ----------
-        actions : iterable
-            An iterable of wxAction instances to add to the tool bar.
+        Returns
+        -------
+        result : QWidget
+            The primary pane for the dock area.
 
-        realize : bool, optional
-            Whether the toolbar should realize the change immediately.
-            If False, Realize() will need to be called manually once
-            all desired changes have been made. The default is True.
+        """
+        return self._primary_pane
+
+    def centralWidget(self):
+        """ Get the central dock widget for the area.
+
+        This method is called by the dock manager which handles the
+        dock area. It should not normally be called by user code.
+
+        Returns
+        -------
+        result : QWidget or None
+            The central dock widget for the area, or None if no widget
+            is installed.
 
         """
-        insert = self.InsertAction
-        for action in actions:
-            insert(None, action, False)
-        if realize:
-            self.Realize()
+        item = self._central_pane.layout().itemAt(0)
+        if item is not None:
+            return item.widget()
 
-    def InsertAction(self, before, action, realize=True):
-        """ Insert a wx action into the tool bar.
+    def setCentralWidget(self, widget):
+        """ Set the central widget for the dock area.
 
-        If the action already exists in the tool bar, it will be moved
-        to the proper location.
+        This method is called by the dock manager which handles the
+        dock area. It should not normally be called by user code.
 
         Parameters
         ----------
-        before : wxAction or None
-            The action in the tool bar which should come directly after
-            the new action.
+        widget : QWidget
+            The central widget for the dock area.
 
-        action : wxAction
-            The wxAction instance to insert into this tool bar.
+        """
+        layout = self._central_pane.layout()
+        item = layout.itemAt(0)
+        if item is not None:
+            old = item.widget()
+            if old is widget:
+                return
+            old.hide()
+            old.setParent(None)
+        if widget is not None:
+            layout.addWidget(widget)
+            # lower the widget to keep it stacked behind any pinned
+            # containers which are in the slide-out position.
+            widget.lower()
+            widget.show()
 
-        realize : bool, optional
-            Whether the toolbar should realize the change immediately.
-            If False, Realize() will need to be called manually once
-            all desired changes have been made. The default is True.
+    def maximizedWidget(self):
+        """ Get the widget to that is set as the maximized widget.
+
+        Returns
+        -------
+        result : QWidget or None
+            The widget which is maximized over the dock area.
 
         """
-        all_items = self._all_items
-        if action not in all_items:
-            if before in all_items:
-                index = all_items.index(before)
-            else:
-                index = len(all_items)
-            all_items.insert(index, action)
-            if action.IsVisible():
-                max_index = len(self._actions_map)
-                index = min(index, max_index)
-                item = self._InsertAction(index, action)
-                self._actions_map[action] = item
-            action.Bind(EVT_ACTION_CHANGED, self.OnActionChanged)
-            if realize:
-                self.Realize()
-        else:
-            # XXX this is a potentially slow way to do things if the
-            # number of actions being moved around is large. But, the
-            # Wx apis don't appear to offer a better way, so this is
-            # what we get (as usual...).
-            self.RemoveAction(action)
-            self.InsertAction(before, action, realize)
+        return self.layout().widget(1)
 
-    def InsertActions(self, before, actions, realize=True):
-        """ Insert multiple wx actions into the Menu.
+    def setMaximizedWidget(self, widget):
+        """ Set the widget to maximize over the dock area.
 
-        If an action already exists in this menu, it will be moved to
-        the proper location.
+        Returns
+        -------
+        result : QWidget or None
+            The widget to maximize over the dock area.
+
+        """
+        old = self.maximizedWidget()
+        if old is not None:
+            if old is widget:
+                return
+            old.hide()
+            old.setParent(None)
+        if widget is not None:
+            layout = self.layout()
+            layout.insertWidget(1, widget)
+            layout.setCurrentIndex(1)
+            widget.show()
+
+    def addToDockBar(self, container, position, index=-1):
+        """ Add a container to the dock bar at the given position.
 
         Parameters
         ----------
-        before : wxAction, wxMenu, or None
-            The item in the menu which should come directly after the
-            new actions.
+        container : QDockContainer
+            The dock container to add to the dock bar. The container
+            should be unplugged from any other layout before calling
+            this method.
 
-        actions : iterable
-            An iterable of wxAction instances to add to the tool bar.
+        position : QDockBar.Position
+            The enum value specifying the dock bar to which the
+            container should be added.
 
-        realize : bool, optional
-            Whether the toolbar should realize the change immediately.
-            If False, Realize() will need to be called manually once
-            all desired changes have been made. The default is True.
+        index : int, optional
+            The index at which to insert the item. The default is -1
+            and will append the item to the dock bar.
 
         """
-        insert = self.InsertAction
-        for action in actions:
-            insert(before, action, False)
-        if realize:
-            self.Realize()
-
-    def RemoveAction(self, action):
-        """ Remove a wx action from the tool bar.
+        self._dock_bar_manager.addContainer(container, position, index)
 
-        If the action does not exist in the tool bar, this is a no-op.
+    def removeFromDockBar(self, container):
+        """ Remove a container previously added to a dock bar.
 
         Parameters
         ----------
-        action : wxAction
-            The wxAction instance to remove from this tool bar.
+        container : QDockContainer
+            The dock container to remove from the dock bar.
 
         """
-        all_items = self._all_items
-        if action in all_items:
-            all_items.remove(action)
-            action.Unbind(EVT_ACTION_CHANGED, handler=self.OnActionChanged)
-            item = self._actions_map.pop(action, None)
-            if item is not None:
-                self.DeleteTool(item.GetId())
+        self._dock_bar_manager.removeContainer(container)
 
-    def RemoveActions(self, actions):
-        """ Remove multiple actions from the tool bar.
-
-        If an action does not exist in the tool bar, it will be ignored.
+    def dockBarGeometry(self, position):
+        """ Get the geometry of the dock bar at the given position.
 
         Parameters
         ----------
-        actions : iterable
-            An iterable of wxActions to remove from the tool bar.
-
-        """
-        remove = self.RemoveAction
-        for action in actions:
-            remove(action)
+        position : QDockBar.Position
+            The enum value specifying the dock bar of interest.
 
+        Returns
+        -------
+        result : QRect
+            The geometry of the given dock bar expressed in area
+            coordinates. If no dock bar exists at the given position,
+            an invalid QRect will be returned.
 
-class WxToolBar(WxConstraintsWidget, ProxyToolBar):
-    """ A Wx implementation of an Enaml ToolBar.
+        """
+        return self._dock_bar_manager.dockBarGeometry(position)
 
-    """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(wxToolBar)
+    def dockBarContainers(self):
+        """ Get the containers held in the dock bars.
 
-    #--------------------------------------------------------------------------
-    # Initialization API
-    #--------------------------------------------------------------------------
-    def create_widget(self):
-        """ Create the QCustomToolBar widget.
+        Returns
+        -------
+        result : list
+            A list of tuples of the form (container, position).
 
         """
-        # The orientation of a tool bar can only be set at creation time.
-        # Wx does not support changing it dynamically. It is only set if
-        # the tool bar is a child of something other than a wx.Frame.
-        # The style must include TB_FLAT or separators won't be drawn.
-        d = self.declaration
-        parent = self.parent_widget()
-        style =  wx.TB_FLAT | wx.TB_TEXT | wx.NO_BORDER
-        if not isinstance(parent, wx.Frame):
-            style |= _ORIENTATION_MAP[d.orientation]
-        else:
-            style |= wx.HORIZONTAL
-
-        self.widget = wxToolBar(parent, style=style)
-
-        # Setting the tool bar to double buffered avoids a ton of
-        # flickering on Windows during resize events.
-        self.widget.SetDoubleBuffered(True)
-
-        # For now, we set the bitmap size to 0 since we don't yet
-        # support icons or images.
-        self.widget.SetToolBitmapSize(wx.Size(0, 0))
-
-    def init_layout(self):
-        """ Initialize the layout for the toolbar.
-
-        """
-        super(WxToolBar, self).init_layout()
-        widget = self.widget
-        for child in self.children():
-            if isinstance(child, WxAction):
-                widget.AddAction(child.widget, False)
-            elif isinstance(child, WxActionGroup):
-                widget.AddActions(child.actions(), False)
-        widget.Realize()
+        return self._dock_bar_manager.dockBarContainers()
 
-    #--------------------------------------------------------------------------
-    # Child Events
-    #--------------------------------------------------------------------------
-    def find_next_action(self, child):
-        """ Locate the wxAction object which logically follows the child.
+    def dockBarPosition(self, container):
+        """ Get the dock bar position of the given container.
 
         Parameters
         ----------
-        child : WxToolkitObject
-            The child object of interest.
+        container : QDockContainer
+            The dock container of interest.
 
         Returns
         -------
-        result : wxAction or None
-            The wxAction which logically follows the position of the
-            child in the list of children. None will be returned if
-            a relevant wxAction is not found.
+        result : QDockBar.Position or None
+            The position of the container, or None if the container
+            does not exist in the manager.
 
         """
-        found = False
-        for dchild in self.children():
-            if found:
-                if isinstance(dchild, WxAction):
-                    return dchild.widget
-                if isinstance(dchild, WxActionGroup):
-                    acts = dchild.actions()
-                    if len(acts) > 0:
-                        return acts[0]
-            else:
-                found = dchild is child
+        return self._dock_bar_manager.dockBarPosition(container)
 
-    def child_added(self, child):
-        """ Handle the child added event for a WxToolBar.
+    def extendFromDockBar(self, container):
+        """ Extend the given container from its dock bar.
 
-        """
-        super(WxToolBar, self).child_added(child)
-        if isinstance(child, WxAction):
-            before = self.find_next_action(child)
-            self.widget.InsertAction(before, child.widget)
-        elif isinstance(child, WxActionGroup):
-            before = self.find_next_action(child)
-            self.widget.InsertActions(before, child.actions())
+        If the container does not exist in a dock bar, this is a no-op.
 
-    def child_removed(self, child):
-        """  Handle the child removed event for a WxToolBar.
+        Parameters
+        ----------
+        container : QDockContainer
+            The dock container of interest.
 
         """
-        super(WxToolBar, self).child_removed(child)
-        if isinstance(child, WxAction):
-            if child.widget is not None:
-                self.widget.RemoveAction(child.widget)
-        elif isinstance(child, WxActionGroup):
-            self.widget.RemoveActions(child.actions())
+        self._dock_bar_manager.extendContainer(container)
 
-    #--------------------------------------------------------------------------
-    # ProxyToolBar API
-    #--------------------------------------------------------------------------
-    def set_visible(self, visible):
-        """ Overridden parent class visibility setter which properly
-        handles the visibility of the tool bar.
+    def retractToDockBar(self, container):
+        """ Retract the given container into it's dock bar.
 
-        """
-        # XXX implement me!
-        pass
+        If the container does not exist in a dock bar, this is a no-op.
 
-    def set_button_style(self, style):
-        """ This is not supported on wx.
+        Parameters
+        ----------
+        container : QDockContainer
+            The dock container of interest.
 
         """
-        pass
+        self._dock_bar_manager.retractContainer(container)
+
+    def clearDockBars(self):
+        """ Clear the dock bars from the dock area.
 
-    def set_orientation(self, orientation):
-        """ Set the orientation of the underlying widget.
+        This method is called by the dock manager when the dock area
+        is reset. It should not be called directly by user code.
 
         """
-        # Wx does not support dynamically changing the orientation.
-        pass
+        self._dock_bar_manager.clearDockBars()
 
-    def set_movable(self, movable):
-        """ Set the movable state on the underlying widget.
+    def isEmpty(self):
+        """ Get whether or not the dock area is empty.
+
+        Returns
+        -------
+        result : bool
+            True if the dock area is empty, False otherwise.
 
         """
-        # The standard wx toolbar doesn't support docking. The Aui
-        # toolbar sucks, don't use it.
-        pass
+        if self.centralWidget() is not None:
+            return False
+        if self.maximizedWidget() is not None:
+            return False
+        return self._dock_bar_manager.isEmpty()
 
-    def set_floatable(self, floatable):
-        """ Set the floatable state on the underlying widget.
+    def tabPosition(self):
+        """ Get the default position for newly created tab widgets.
+
+        The tab position is inherited from an ancestor dock area unless
+        it is explicitly set by the user.
+
+        Returns
+        -------
+        result : QTabWidget.TabPosition
+            The position for dock area tabs. If the value has not been
+            set by the user and there is no ancestor dock area, the
+            default is QTabWidget.North.
+
+        """
+        pos = self._tab_position
+        if pos is not None:
+            return pos
+        p = self.parent()
+        while p is not None:
+            if isinstance(p, QDockArea):
+                return p.tabPosition()
+            p = p.parent()
+        return QTabWidget.North
+
+    def setTabPosition(self, position):
+        """ Set the default position for newly created tab widget.
+
+        Parameters
+        ----------
+        position : QTabWidget.TabPosition
+            The position for the tabs of newly created tab widgets.
 
         """
-        # The standard wx toolbar doesn't support docking. The Aui
-        # toolbar sucks, don't use it.
-        pass
+        self._tab_position = position
 
-    def set_floating(self, floating):
-        """ Set the floating staet on the underlying widget.
+    def dockEventsEnabled(self):
+        """ Get whether dock events are enabled for the area.
+
+        Returns
+        -------
+        result : bool
+            True if dock events are enabled, False otherwise.
 
         """
-        # The standard wx toolbar doesn't support docking. The Aui
-        # toolbar sucks, don't use it.
-        pass
+        return self._dock_events_enabled
 
-    def set_dock_area(self, dock_area):
-        """ Set the dock area on the underyling widget.
+    def setDockEventsEnabled(self, enabled):
+        """ Set whether dock events are enabled for the area.
+
+        If events are enabled, then the various widgets involved with
+        the dock area will post events to the *root* dock area when the
+        various states have changed. If events are disabled, no such
+        events will be posted.
+
+        Parameters
+        ----------
+        enabled : bool
+            True if dock events should be enabled, False otherwise.
 
         """
-        # The standard wx toolbar doesn't support docking. The Aui
-        # toolbar sucks, don't use it.
-        pass
+        self._dock_events_enabled = enabled
+
+    def opaqueItemResize(self):
+        """ Get whether opaque item resize is enabled.
+
+        The tab position is inherited from an ancestor dock area unless
+        it is explicitly set by the user.
+
+        Returns
+        -------
+        result : bool
+            True if item resizing is opaque, False otherwise. If the
+            value has not been set by the user and there is no ancestor
+            dock area, the default is True.
+
+        """
+        opaque = self._opaque_resize
+        if opaque is not None:
+            return opaque
+        p = self.parent()
+        while p is not None:
+            if isinstance(p, QDockArea):
+                return p.opaqueItemResize()
+            p = p.parent()
+        return True
+
+    def setOpaqueItemResize(self, opaque):
+        """ Set whether opaque item resize is enabled.
 
-    def set_allowed_dock_areas(self, dock_areas):
-        """ Set the allowed dock areas on the underlying widget.
+        Parameters
+        ----------
+        opaque : bool
+            True if item resizing should be opaque, False otherwise.
 
         """
-        # The standard wx toolbar doesn't support docking. The Aui
-        # toolbar sucks, don't use it.
-        pass
+        is_different = opaque != self.opaqueItemResize()
+        self._opaque_resize = opaque
+        if is_different:
+            # Avoid a circular import
+            from .q_dock_splitter import QDockSplitter
+            for sp in self.findChildren(QDockSplitter):
+                sp.inheritOpaqueResize()
```

### Comparing `enaml-0.9.7/enaml/wx/wx_field.py` & `enaml-0.9.8/enaml/qt/qt_dock_pane.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,337 +1,368 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-
 from atom.api import Int, Typed
 
-from enaml.widgets.field import ProxyField
+from enaml.widgets.dock_pane import ProxyDockPane
+
+from .QtCore import Qt, Signal 
+from .QtGui import QDockWidget, QWidget
+
+from .qt_container import QtContainer
+from .qt_widget import QtWidget
+
 
-from .wx_control import WxControl
+#: A mapping from Enaml dock areas to Qt dock areas.
+_DOCK_AREA_MAP = {
+    'top': Qt.TopDockWidgetArea,
+    'right': Qt.RightDockWidgetArea,
+    'bottom': Qt.BottomDockWidgetArea,
+    'left': Qt.LeftDockWidgetArea,
+    'all': Qt.AllDockWidgetAreas,
+}
 
 
-class wxLineEdit(wx.TextCtrl):
-    """ A wx.TextCtrl subclass which is similar to a QLineEdit in terms
-    of features and behavior.
+#: A mapping from Qt dock areas to Enaml dock areas.
+_DOCK_AREA_INV_MAP = {
+    Qt.TopDockWidgetArea: 'top',
+    Qt.RightDockWidgetArea: 'right',
+    Qt.BottomDockWidgetArea: 'bottom',
+    Qt.LeftDockWidgetArea: 'left',
+    Qt.AllDockWidgetAreas: 'all',
+}
+
+
+class QCustomDockWidget(QDockWidget):
+    """ A custom QDockWidget which adds some Enaml specific features.
 
     """
-    def __init__(self, *args, **kwargs):
-        """ Initialize a wxLineEdit.
+    #: A signal emitted when the dock widget is closed by the user.
+    closed = Signal()
 
-        Parameters
-        ----------
-        *args, **kwargs
-            The positional and keyword arguments to initialize a
-            wx.TextCtrl.
+    #: A signal emitted when the dock widget is floated.
+    floated = Signal()
+
+    #: A signal emitted when the dock widget is docked. The payload
+    #: will be the new dock area.
+    docked = Signal(object)
+
+    def __init__(self, parent=None):
+        """ Initialize a QCustomDockWidget.
 
         """
-        super(wxLineEdit, self).__init__(*args, **kwargs)
-        self._placeholder_text = ''
-        self._placeholder_active = False
-        self._user_fgcolor = None
-        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
-        self.Bind(wx.EVT_SET_FOCUS, self.OnSetFocus)
+        super(QCustomDockWidget, self).__init__(parent)
+        self._title_bar_visible = True
+        self._dock_area = Qt.LeftDockWidgetArea
+        self.topLevelChanged.connect(self._onTopLevelChanged)
 
     #--------------------------------------------------------------------------
     # Private API
     #--------------------------------------------------------------------------
-    def _UpdatePlaceholderDisplay(self):
-        """ Updates the display with the placeholder text if no text
-        is currently set for the control.
+    def _onTopLevelChanged(self, top_level):
+        """ The signal handler for the the 'topLevelChanged' signal.
 
         """
-        if not self.GetValue() and self._placeholder_text:
-            self.ChangeValue(self._placeholder_text)
-            color = wx.Color(95, 95, 95)
-            super(wxLineEdit, self).SetForegroundColour(color)
-            self._placeholder_active = True
+        # Hiding the title bar on a floating dock widget causes the
+        # frame to be hidden. We need to make sure its shown when
+        # floating, and hidden again upon docking if needed.
+        if top_level:
+            self._showTitleBar()
+            self.floated.emit()
+        else:
+            if not self._title_bar_visible:
+                self._hideTitleBar()
+            parent = self.parent()
+            if parent is not None:
+                self._dock_area = parent.dockWidgetArea(self)
+            self.docked.emit(self._dock_area)
 
-    def _RemovePlaceholderDisplay(self):
-        """ Removes the placeholder text if it is currently active.
+    def _showTitleBar(self):
+        """ Shows the title bar for the widget.
 
         """
-        if self._placeholder_active:
-            self.ChangeValue('')
-            color = self._user_fgcolor or wx.Color(0, 0, 0)
-            super(wxLineEdit, self).SetForegroundColour(color)
-            self._placeholder_active = False
+        if self.titleBarWidget() is not None:
+            self.setTitleBarWidget(None)
 
-    #--------------------------------------------------------------------------
-    # Event Handlers
-    #--------------------------------------------------------------------------
-    def OnKillFocus(self, event):
-        """ Refreshes the placeholder display when the control loses
-        focus.
+    def _hideTitleBar(self):
+        """ Hides the title bar for the widget.
 
         """
-        self._UpdatePlaceholderDisplay()
-        event.Skip()
+        if self.titleBarWidget() is None:
+            self.setTitleBarWidget(QWidget())
 
-    def OnSetFocus(self, event):
-        """ Removes the placeholder display when the control receives
-        focus.
+    def closeEvent(self, event):
+        """ A close event handler which emits the 'closed' signal.
 
         """
-        self._RemovePlaceholderDisplay()
-        event.Skip()
+        super(QCustomDockWidget, self).closeEvent(event)
+        self.closed.emit()
 
     #--------------------------------------------------------------------------
     # Public API
     #--------------------------------------------------------------------------
-    def GetBestSize(self):
-        """ Overridden best size method to add 44 pixels in width to the
-        field. This makes Wx consistent with Qt.
+    def dockArea(self):
+        """ Get the current dock area for the dock widget.
 
-        """
-        size = super(wxLineEdit, self).GetBestSize()
-        return wx.Size(size.GetWidth() + 44, size.GetHeight())
-
-    def SetPlaceHolderText(self, placeholder_text):
-        """ Sets the placeholder text to the given value. Pass an empty
-        string to turn off the placeholder text functionality.
+        Returns
+        -------
+        result : QDockWidgetArea
+            The dock widget area where this dock widget resides.
 
         """
-        self._placeholder_text = placeholder_text
-        self._UpdatePlaceholderDisplay()
-
-    def GetPlaceHolderText(self):
-        """ Returns the placeholder text for this control.
+        return self._dock_area
 
-        """
-        return self._placeholder_text
+    def setDockArea(self, area):
+        """ Set the current dock area for the dock widget.
 
-    def ChangeValue(self, text):
-        """ Overridden method which moves the insertion point to the end
-        of the field when changing the text value. This causes the field
-        to behave like Qt.
+        Parameters
+        ----------
+        area : QDockWidgetArea
+            The dock widget area where this dock widget should reside.
 
         """
-        super(wxLineEdit, self).ChangeValue(text)
-        self.SetInsertionPoint(len(text))
+        self._dock_area = area
+        parent = self.parent()
+        if parent is not None:
+            parent.setDockWidgetArea(area, self)
 
-    def GetValue(self):
-        """ Returns string value in the control, or an empty string if
-        the placeholder text is active.
+    def titleBarVisible(self):
+        """ Get whether or not the title bar is visible.
+
+        Returns
+        -------
+        result : bool
+            Whether or not the title bar is visible.
 
         """
-        if self._placeholder_active:
-            return ''
-        return super(wxLineEdit, self).GetValue()
+        return self._title_bar_visible
+
+    def setTitleBarVisible(self, visible):
+        """ Set whether or not the title bar is visible.
 
-    def SetForegroundColour(self, wxColor, force=False):
-        """ Sets the foreground color of the field. If the placeholder
-        text is being shown, `force` must be True in order to override
-        the placeholder text color.
+        Parameters
+        ----------
+        visible : bool
+            Whether or not the title bar is visible.
 
         """
-        self._user_fgcolor = wxColor
-        if self._placeholder_active and not force:
-            return
-        super(wxLineEdit, self).SetForegroundColour(wxColor)
+        self._title_bar_visible = visible
+        if visible:
+            self._showTitleBar()
+        else:
+            if not self.isFloating():
+                self._hideTitleBar()
 
 
-# Guard flags
-TEXT_GUARD = 0x1
-ERROR_FLAG = 0x2
+# cyclic notification guard flags
+FLOATED_GUARD = 0x1
 
 
-class WxField(WxControl, ProxyField):
-    """ A Wx implementation of an Enaml ProxyField.
+class QtDockPane(QtWidget, ProxyDockPane):
+    """ A Qt implementation of an Enaml ProxyDockPane.
 
     """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(wxLineEdit)
-
-    #: A collapsing timer for auto sync text.
-    _text_timer = Typed(wx.Timer)
+    #: A reference tot he widget created by the proxy.
+    widget = Typed(QCustomDockWidget)
 
     #: Cyclic notification guard. This a bitfield of multiple guards.
     _guard = Int(0)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Creates the underlying wxLineEdit widget.
+        """ Create the QCustomDockWidget widget.
 
         """
-        # We have to do a bit of initialization in the create method
-        # since wx requires the style of certain things to be set at
-        # the point of instantiation
-        d = self.declaration
-        style = wx.TE_PROCESS_ENTER
-        if d.read_only:
-            style |= wx.TE_READONLY
-        else:
-            style &= ~wx.TE_READONLY
-        if d.echo_mode == 'normal':
-            style &= ~wx.TE_PASSWORD
-        else:
-            style |= wx.TE_PASSWORD
-        self.widget = wxLineEdit(self.parent_widget(), style=style)
+        self.widget = QCustomDockWidget(self.parent_widget())
 
     def init_widget(self):
-        """ Create and initialize the underlying widget.
+        """ Initialize the dock pane control.
 
         """
-        super(WxField, self).init_widget()
+        super(QtDockPane, self).init_widget()
         d = self.declaration
-        if d.text:
-            self.set_text(d.text)
-        if d.mask:
-            self.set_mask(d.mask)
-        if d.placeholder:
-            self.set_placeholder(d.placeholder)
-        self.set_echo_mode(d.echo_mode)
-        self.set_max_length(d.max_length)
-        self.set_read_only(d.read_only)
-        self.set_submit_triggers(d.submit_triggers)
-        self.widget.Bind(wx.EVT_TEXT, self.on_text_edited)
+        self.set_title(d.title)
+        self.set_title_bar_visible(d.title_bar_visible)
+        self.set_title_bar_orientation(d.title_bar_orientation)
+        self.set_closable(d.closable)
+        self.set_movable(d.movable)
+        self.set_floatable(d.floatable)
+        self.set_floating(d.floating)
+        self.set_dock_area(d.dock_area)
+        self.set_allowed_dock_areas(d.allowed_dock_areas)
+        widget = self.widget
+        widget.closed.connect(self.on_closed)
+        widget.floated.connect(self.on_floated)
+        widget.docked.connect(self.on_docked)
+
+    def init_layout(self):
+        """ Handle the layout initialization for the dock pane.
+
+        """
+        super(QtDockPane, self).init_layout()
+        self.widget.setWidget(self.dock_widget())
 
     #--------------------------------------------------------------------------
-    # Private API
+    # Utility Methods
     #--------------------------------------------------------------------------
-    def _validate_and_apply(self):
-        """ Validate and apply the text in the control.
+    def dock_widget(self):
+        """ Find and return the dock widget child for this widget.
+
+        Returns
+        -------
+        result : QWidget or None
+            The dock widget defined for this widget, or None if one is
+            not defined.
 
         """
-        d = self.declaration
-        text = self.widget.GetValue()
-        if d.validator and not d.validator.validate(text):
-            text = d.validator.fixup(text)
-            if not d.validator.validate(text):
-                return
-        self._clear_error_state()
-        d.text = text
+        d = self.declaration.dock_widget()
+        if d is not None:
+            return d.proxy.widget
 
-    def _set_error_state(self):
-        """ Set the error state of the widget.
+    #--------------------------------------------------------------------------
+    # Child Events
+    #--------------------------------------------------------------------------
+    def child_added(self, child):
+        """ Handle the child added event for a QtDockPane.
 
         """
-        # A temporary hack until styles are implemented
-        if not self._guard & ERROR_FLAG:
-            self._guard |= ERROR_FLAG
-            # XXX attempting to change the field style here is futile
+        super(QtDockPane, self).child_added(child)
+        if isinstance(child, QtContainer):
+            self.widget.setWidget(self.dock_widget())
 
-    def _clear_error_state(self):
-        """ Clear the error state of the widget.
+    def child_removed(self, child):
+        """ Handle the child removed event for a QtDockPane.
 
         """
-        # A temporary hack until styles are implemented
-        if self._guard & ERROR_FLAG:
-            self._guard &= ~ERROR_FLAG
-            # XXX attempting to change the field style here is futile
+        super(QtDockPane, self).child_removed(child)
+        if isinstance(child, QtContainer):
+            self.widget.setWidget(self.dock_widget())
 
     #--------------------------------------------------------------------------
-    # Event Handling
+    # Signal Handlers
     #--------------------------------------------------------------------------
-    def on_submit_text(self, event):
-        """ The event handler for the text submit triggers.
+    def on_closed(self):
+        """ The signal handler for the 'closed' signal.
 
         """
-        # Only skip the focus event: wx triggers the system beep if the
-        # enter event is skipped.
-        if isinstance(event, wx.FocusEvent):
-            event.Skip()
-        self._guard |= TEXT_GUARD
-        try:
-            self._validate_and_apply()
-        finally:
-            self._guard &= ~TEXT_GUARD
+        # The closed signal is only emitted when the widget is closed
+        # by the user, so there is no need for a loopback guard.
+        self.declaration.visible = False
+        self.declaration.closed()
 
-    def on_text_edited(self, event):
-        """ The event handler for the text edited event.
+    def on_floated(self):
+        """ The signal handler for the 'floated' signal.
 
         """
-        # Temporary kludge until error style is fully implemented
-        d = self.declaration
-        if d.validator and not d.validator.validate(self.widget.GetValue()):
-            self._set_error_state()
-            self.widget.SetToolTip(wx.ToolTip(d.validator.message))
-        else:
-            self._clear_error_state()
-            self.widget.SetToolTip(wx.ToolTip(''))
-        if self._text_timer is not None:
-            self._text_timer.Start(300, oneShot=True)
+        if not self._guard & FLOATED_GUARD:
+            self._guard |= FLOATED_GUARD
+            try:
+                self.declaration.floating = True
+            finally:
+                self._guard &= ~FLOATED_GUARD
+
+    def on_docked(self, area):
+        """ The signal handler for the 'docked' signal.
+
+        """
+        if not self._guard & FLOATED_GUARD:
+            self._guard |= FLOATED_GUARD
+            try:
+                self.declaration.floating = False
+                self.declaration.dock_area = _DOCK_AREA_INV_MAP[area]
+            finally:
+                self._guard &= ~FLOATED_GUARD
 
     #--------------------------------------------------------------------------
-    # ProxyField API
+    # ProxyDockPane API
     #--------------------------------------------------------------------------
-    def set_text(self, text):
-        """ Updates the text control with the given unicode text.
+    def set_title(self, title):
+        """ Set the title on the underlying widget.
 
         """
-        if not self._guard & TEXT_GUARD:
-            self.widget.ChangeValue(text)
-            self._clear_error_state()
+        self.widget.setWindowTitle(title)
+
+    def set_title_bar_visible(self, visible):
+        """ Set the title bar visibility of the underlying widget.
 
-    def set_mask(self, mask):
-        """ Set the make for the widget.
+        """
+        self.widget.setTitleBarVisible(visible)
 
-        This is not supported in Wx.
+    def set_title_bar_orientation(self, orientation):
+        """ Set the title bar orientation of the underyling widget.
 
         """
-        pass
+        widget = self.widget
+        features = widget.features()
+        if orientation == 'vertical':
+            features |= QDockWidget.DockWidgetVerticalTitleBar
+        else:
+            features &= ~QDockWidget.DockWidgetVerticalTitleBar
+        widget.setFeatures(features)
 
-    def set_submit_triggers(self, triggers):
-        """ Set the submit triggers for the widget.
+    def set_closable(self, closable):
+        """ Set the closable state on the underlying widget.
 
         """
         widget = self.widget
-        handler = self.on_submit_text
-        widget.Unbind(wx.EVT_KILL_FOCUS, handler=handler)
-        widget.Unbind(wx.EVT_TEXT_ENTER, handler=handler)
-        if 'lost_focus' in triggers:
-            widget.Bind(wx.EVT_KILL_FOCUS, handler)
-        if 'return_pressed' in triggers:
-            widget.Bind(wx.EVT_TEXT_ENTER, handler)
-        if 'auto_sync' in triggers:
-            if self._text_timer is None:
-                timer = self._text_timer = wx.Timer()
-                timer.Bind(wx.EVT_TIMER, handler)
+        features = widget.features()
+        if closable:
+            features |= QDockWidget.DockWidgetClosable
         else:
-            if self._text_timer is not None:
-                self._text_timer.Stop()
-                self._text_timer = None
+            features &= ~QDockWidget.DockWidgetClosable
+        widget.setFeatures(features)
 
-    def set_placeholder(self, placeholder):
-        """ Sets the placeholder text in the widget.
+    def set_movable(self, movable):
+        """ Set the movable state on the underlying widget.
 
         """
-        self.widget.SetPlaceHolderText(placeholder)
+        widget = self.widget
+        features = widget.features()
+        if movable:
+            features |= QDockWidget.DockWidgetMovable
+        else:
+            features &= ~QDockWidget.DockWidgetMovable
+        widget.setFeatures(features)
 
-    def set_echo_mode(self, echo_mode):
-        """ Sets the echo mode of the wiget.
+    def set_floatable(self, floatable):
+        """ Set the floatable state on the underlying widget.
 
         """
-        # Wx cannot change the echo mode dynamically. It requires
-        # creating a brand-new control, so we just ignore the change.
-        pass
+        widget = self.widget
+        features = widget.features()
+        if floatable:
+            features |= QDockWidget.DockWidgetFloatable
+        else:
+            features &= ~QDockWidget.DockWidgetFloatable
+        widget.setFeatures(features)
 
-    def set_max_length(self, max_length):
-        """ Set the max length of the control to max_length. If the max
-        length is <= 0 or > 32767 then the control will be set to hold
-        32kb of text.
+    def set_floating(self, floating):
+        """ Set the floating staet on the underlying widget.
 
         """
-        if (max_length <= 0) or (max_length > 32767):
-            max_length = 32767
-        self.widget.SetMaxLength(max_length)
+        if not self._guard & FLOATED_GUARD:
+            self._guard |= FLOATED_GUARD
+            try:
+                self.widget.setFloating(floating)
+            finally:
+                self._guard &= ~FLOATED_GUARD
 
-    def set_read_only(self, read_only):
-        """ Sets the read only state of the widget.
+    def set_dock_area(self, dock_area):
+        """ Set the dock area on the underlying widget.
 
         """
-        # Wx cannot change the read only state dynamically. It requires
-        # creating a brand-new control, so we just ignore the change.
-        pass
+        self.widget.setDockArea(_DOCK_AREA_MAP[dock_area])
 
-    def field_text(self):
-        """ Get the text stored in the widget.
+    def set_allowed_dock_areas(self, dock_areas):
+        """ Set the allowed dock areas on the underlying widget.
 
         """
-        return self.widget.GetValue()
+        qt_areas = Qt.NoDockWidgetArea
+        for area in dock_areas:
+            qt_areas |= _DOCK_AREA_MAP[area]
+        self.widget.setAllowedAreas(qt_areas)
```

### Comparing `enaml-0.9.7/enaml/wx/wx_slider.py` & `enaml-0.9.8/enaml/qt/qt_splitter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,279 +1,223 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import wx
-import wx.lib.newevent
+import sys
 
-from atom.api import Int, Typed
+from atom.api import Typed
 
-from enaml.widgets.slider import ProxySlider
+from enaml.widgets.splitter import ProxySplitter
 
-from .wx_control import WxControl
-
-
-#: Horizontal tick mapping
-_TICK_POSITION_MAP = {
-    'top': wx.SL_TOP | wx.SL_AUTOTICKS,
-    'bottom': wx.SL_BOTTOM | wx.SL_AUTOTICKS,
-    'left': wx.SL_LEFT | wx.SL_AUTOTICKS,
-    'right': wx.SL_RIGHT | wx.SL_AUTOTICKS,
-    'both': wx.SL_BOTH | wx.SL_AUTOTICKS,
-}
-
-
-#: An OR'd combination of all the tick flags.
-_TICK_MASK = (
-    wx.SL_TOP | wx.SL_BOTTOM | wx.SL_LEFT | wx.SL_RIGHT | wx.SL_BOTH |
-    wx.SL_AUTOTICKS
+from .QtCore import Qt, QEvent, Signal
+from .QtGui import (
+    QSplitter, QSplitterHandle, QVBoxLayout, QFrame, QApplication
 )
 
+from .qt_constraints_widget import QtConstraintsWidget
+from .qt_split_item import QtSplitItem
 
-#: A map adapting orientation to tick positions
-_TICK_ADAPT_MAP = {
-    'vertical': {
-        'left': 'left',
-        'right': 'right',
-        'both': 'both',
-        'top': 'left',
-        'bottom': 'right',
-    },
-    'horizontal': {
-        'left': 'top',
-        'right': 'bottom',
-        'both': 'both',
-        'top': 'top',
-        'bottom': 'bottom',
-    },
-}
 
-
-#: A map from string orientation to wx slider orientation
-_ORIENTATION_MAP = {
-    'horizontal': wx.SL_HORIZONTAL,
-    'vertical': wx.SL_VERTICAL,
+ORIENTATION = {
+    'horizontal': Qt.Horizontal,
+    'vertical': Qt.Vertical,
 }
 
 
-#: An OR'd combination of all the orientation flags
-_ORIENTATION_MASK = wx.SL_HORIZONTAL | wx.SL_VERTICAL
-
-
-#: A new event emitted by the custom slider control
-wxSliderEvent, EVT_SLIDER = wx.lib.newevent.NewEvent()
+class QWinSplitterHandle(QSplitterHandle):
+    """ A custom QSplitterHandle which is used on win32 platforms.
 
-
-class wxProperSlider(wx.Slider):
-    """ A wx.Slider subclass which supports tracking.
+    The native Windows style draws the splitter handle the same color as
+    the widget background, which makes it invisible for most cases. This
+    subclass overlays a raised line on the splitter to provide a little
+    bit of visual feedback.
 
     """
-    #: The event types for the frequent thumb track event
-    _tracking_evt = wx.EVT_SCROLL_THUMBTRACK.evtType[0]
-
-    #: The event type for the thumb release event.
-    _release_evt = wx.EVT_SCROLL_THUMBRELEASE.evtType[0]
+    def __init__(self, orientation, parent=None):
+        super(QWinSplitterHandle, self).__init__(orientation, parent)
+        self._frame = frame = QFrame(self)
+        l = QVBoxLayout()
+        l.addWidget(frame)
+        l.setSpacing(0)
+        l.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(l)
+        self.updateFrame()
+
+    def updateFrame(self):
+        """ Update the internal frame style for the current orientation.
+
+        """
+        orientation = self.orientation()
+        s = QFrame.VLine if orientation == Qt.Horizontal else QFrame.HLine
+        self._frame.setFrameStyle(s | QFrame.Raised)
 
-    #: The event type for the scroll end event.
-    _end_evt = wx.EVT_SCROLL_CHANGED.evtType[0]
 
-    def __init__(self, *args, **kwargs):
-        """ Initialize a wxProperSlider.
+class QCustomSplitter(QSplitter):
+    """ A custom QSplitter which handles children of type QSplitItem.
 
-        Parameters
-        ----------
-        *args, **kwargs
-            The positional and keyword arguments for initializing a
-            wx.Slider.
-
-        """
-        super(wxProperSlider, self).__init__(*args, **kwargs)
-        self._tracking = True
-        self.Bind(wx.EVT_SCROLL, self.OnScroll)
+    """
+    #: A signal emitted when a LayoutRequest event is posted to the
+    #: splitter widget. This will typically occur when the size hint
+    #: of the splitter is no longer valid.
+    layoutRequested = Signal()
 
-    def OnScroll(self, event):
-        """ An event handler which handles all scroll events.
+    def createHandle(self):
+        """ A reimplemented virtual method to create splitter handles.
 
-        This handler determines whether or not a slider event sould be
-        emitted for the scroll changed, based on whether tracking is
-        enabled for the slider.
+        On win32 platforms, this will return a custom QSplitterHandle
+        which works around an issue with handle not drawing nicely. On
+        all other platforms, a normal QSplitterHandler widget.
 
         """
-        evt_type = event.EventType
-
-        # We never emit on the _end_event since that is windows-only
-        if evt_type == self._end_evt:
-            return
-
-        if self._tracking:
-            if evt_type != self._release_evt:
-                emit = True
-            else:
-                emit = False
-        else:
-            emit = evt_type != self._tracking_evt
-
-        if emit:
-            evt = wxSliderEvent()
-            wx.PostEvent(self, evt)
+        if sys.platform == 'win32':
+            return QWinSplitterHandle(self.orientation(), self)
+        return QSplitterHandle(self.orientation(), self)
 
-    def GetTracking(self):
-        """ Whether or not tracking is enabled for the slider.
+    def setOrientation(self, orientation):
+        """ Set the orientation of the splitter.
 
-        Returns
-        -------
-        result : bool
-            True if tracking is enabled for the slider, False otherwise.
+        This overriden method will call the `updateFrame` method of the
+        splitter handles when running on win32 platforms. On any other
+        platform, this method simply calls the superclass method.
 
         """
-        return self._tracking
+        old = self.orientation()
+        if old != orientation:
+            super(QCustomSplitter, self).setOrientation(orientation)
+            if sys.platform == 'win32':
+                for idx in xrange(self.count()):
+                    handle = self.handle(idx)
+                    handle.updateFrame()
 
-    def SetTracking(self, tracking):
-        """ Set whether tracking is enabled for the slider.
+    def event(self, event):
+        """ A custom event handler which handles LayoutRequest events.
 
-        Parameters
-        ----------
-        tracking : bool
-            True if tracking should be enabled, False otherwise.
+        When a LayoutRequest event is posted to this widget, it will
+        emit the `layoutRequested` signal. This allows an external
+        consumer of this widget to update their external layout.
 
         """
-        self._tracking = tracking
+        res = super(QCustomSplitter, self).event(event)
+        if event.type() == QEvent.LayoutRequest:
+            self.layoutRequested.emit()
+        return res
 
 
-#: A cyclic guard flag
-VALUE_FLAG = 0x1
-
-
-class WxSlider(WxControl, ProxySlider):
-    """ A Wx implementation of an Enaml ProxySlider.
+class QtSplitter(QtConstraintsWidget, ProxySplitter):
+    """ A Qt implementation of an Enaml ProxySplitter.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(wxProperSlider)
-
-    #: Cyclic notification guard flags.
-    _guard = Int(0)
+    widget = Typed(QCustomSplitter)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying wxProperSlider widget.
+        """ Creates the underlying QSplitter control.
 
         """
-        self.widget = wxProperSlider(self.parent_widget())
+        self.widget = QCustomSplitter(self.parent_widget())
 
     def init_widget(self):
-        """ Initialize the underlying widget.
+        """ Initialize the underlying control.
 
         """
-        # NOTE: The tick interval must be set *after* the tick position
-        # or Wx will ignore the tick interval. grrr...
-        super(WxSlider, self).init_widget()
+        super(QtSplitter, self).init_widget()
         d = self.declaration
-        self.set_minimum(d.minimum)
-        self.set_maximum(d.maximum)
-        self.set_value(d.value)
         self.set_orientation(d.orientation)
-        self.set_page_step(d.page_step)
-        self.set_single_step(d.single_step)
-        self.set_tick_position(d.tick_position)
-        self.set_tick_interval(d.tick_interval)
-        self.set_tracking(d.tracking)
-        self.widget.Bind(EVT_SLIDER, self.on_value_changed)
+        self.set_live_drag(d.live_drag)
 
-    #--------------------------------------------------------------------------
-    # Event Handlers
-    #--------------------------------------------------------------------------
-    def on_value_changed(self, event):
-        """ Send the 'value_changed' action to the Enaml widget when the
-        slider value has changed.
+    def init_layout(self):
+        """ Handle the layout initialization for the splitter.
 
         """
-        if not self._guard & VALUE_FLAG:
-            self._guard |= VALUE_FLAG
-            try:
-                self.declaration.value = self.widget.GetValue()
-            finally:
-                self._guard &= ~VALUE_FLAG
+        super(QtSplitter, self).init_layout()
+        widget = self.widget
+        for item in self.split_items():
+            widget.addWidget(item)
+        widget.layoutRequested.connect(self.on_layout_requested)
+
+        # On Windows, messages are consumed from three different queues,
+        # each with a different priority. The lowest priority is the
+        # queue which holds WM_PAINT messages. Dragging the splitter bar
+        # generates WM_MOUSEMOVE messages which have a higher priority.
+        # These messages (dragging the bar) generate size events in Qt
+        # which are delivered immediately. This means that if handling
+        # the resize event from the drag takes too long (> ~800us) then
+        # another size event will arrive before the paint event, since
+        # the new WM_MOUSEMOVE will be processed before the WM_PAINT.
+        # So on Windows, the `splitterMoved` signal, which is emitted
+        # on every drag, is connected to a handler which will force a
+        # repaint if opaque resize is turned on. Since paint event are
+        # collapsed, the effect of this is to restore the order of event
+        # processing.
+        if sys.platform == 'win32':
+            widget.splitterMoved.connect(self.on_win32_splitter_moved)
 
     #--------------------------------------------------------------------------
-    # ProxySlider API
+    # Child Events
     #--------------------------------------------------------------------------
-    def set_value(self, value):
-        """ Set the value of the underlying widget.
-
-        """
-        if not self._guard & VALUE_FLAG:
-            self._guard |= VALUE_FLAG
-            try:
-                self.widget.SetValue(value)
-            finally:
-                self._guard &= ~VALUE_FLAG
-
-    def set_maximum(self, maximum):
-        """ Set the maximum value of the underlying widget.
+    def child_added(self, child):
+        """ Handle the child added event for a QtSplitter.
 
         """
-        widget = self.widget
-        minimum, _ = widget.GetRange()
-        widget.SetRange(minimum, maximum)
+        super(QtSplitter, self).child_added(child)
+        if isinstance(child, QtSplitItem):
+            for index, dchild in enumerate(self.children()):
+                if child is dchild:
+                    self.widget.insertWidget(index, child.widget)
 
-    def set_minimum(self, minimum):
-        """ Set the minimum value of the underlying widget.
+    # QSplitter automatically removes a widget when it's reparented. The
+    # base child_removed event handler will set the parent to None, and
+    # that is all that is needed.
 
-        """
-        widget = self.widget
-        _, maximum = widget.GetRange()
-        widget.SetRange(minimum, maximum)
-
-    def set_orientation(self, orientation):
-        """ Set the orientation of the underlying widget.
+    #--------------------------------------------------------------------------
+    # Utility Methods
+    #--------------------------------------------------------------------------
+    def split_items(self):
+        """ Get the split items defined for the widget.
 
         """
-        widget = self.widget
-        style = widget.GetWindowStyle()
-        style &= ~_ORIENTATION_MASK
-        style |= _ORIENTATION_MAP[orientation]
-        widget.SetWindowStyle(style)
+        for d in self.declaration.split_items():
+            w = d.proxy.widget
+            if w is not None:
+                yield w
 
-    def set_page_step(self, page_step):
-        """ Set the page step of the underlying widget.
+    #--------------------------------------------------------------------------
+    # Signal Handlers
+    #--------------------------------------------------------------------------
+    def on_layout_requested(self):
+        """ Handle the `layoutRequested` signal from the QSplitter.
 
         """
-        self.widget.SetPageSize(page_step)
-
-    def set_single_step(self, single_step):
-        """ Set the single step of the underlying widget.
+        self.geometry_updated()
 
-        """
-        self.widget.SetLineSize(single_step)
+    def on_win32_splitter_moved(self):
+        """ Handle the 'splitterMoved' signal from the QSplitter.
 
-    def set_tick_interval(self, interval):
-        """ Set the tick interval of the underlying widget.
+        This handler is only connected when running on Windows and it
+        serves to make sure paint events get processed during heavy
+        resize events when opaque resizing is turned on.
 
         """
-        self.widget.SetTickFreq(interval)
+        if self.widget.opaqueResize():
+            QApplication.sendPostedEvents()
 
-    def set_tick_position(self, tick_position):
-        """ Set the tick position of the underlying widget.
+    #--------------------------------------------------------------------------
+    # ProxySplitter API
+    #--------------------------------------------------------------------------
+    def set_orientation(self, orientation):
+        """ Update the orientation of the QSplitter.
 
         """
-        widget = self.widget
-        style = widget.GetWindowStyle()
-        style &= ~_TICK_MASK
-        if tick_position != 'no_ticks':
-            if style & wx.SL_VERTICAL:
-                tick_position = _TICK_ADAPT_MAP['vertical'][tick_position]
-            else:
-                tick_position = _TICK_ADAPT_MAP['horizontal'][tick_position]
-            style |= _TICK_POSITION_MAP[tick_position]
-        widget.SetWindowStyle(style)
+        with self.geometry_guard():
+            self.widget.setOrientation(ORIENTATION[orientation])
 
-    def set_tracking(self, tracking):
-        """ Set the tracking of the underlying widget.
+    def set_live_drag(self, live_drag):
+        """ Update the dragging mode of the QSplitter.
 
         """
-        self.widget.SetTracking(tracking)
+        self.widget.setOpaqueResize(live_drag)
```

### Comparing `enaml-0.9.7/enaml/qt/qt_calendar.py` & `enaml-0.9.8/enaml/qt/docking/q_dock_frame_layout.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,80 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from atom.api import Typed
+from enaml.qt.QtCore import QSize
+from enaml.qt.q_single_widget_layout import QSingleWidgetLayout
 
-from enaml.widgets.calendar import ProxyCalendar
 
-from .QtGui import QCalendarWidget
+class QDockFrameLayout(QSingleWidgetLayout):
+    """ A single widget layout for dock frames.
 
-from .qt_bounded_date import QtBoundedDate, CHANGED_GUARD
-
-
-class QtCalendar(QtBoundedDate, ProxyCalendar):
-    """ A Qt implementation of an Enaml ProxyCalendar.
+    This class is used by the docking framework and is not intended for
+    direct use by user code.
 
     """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(QCalendarWidget)
-
-    #--------------------------------------------------------------------------
-    # Initialization
-    #--------------------------------------------------------------------------
-    def create_widget(self):
-        """ Create the calender widget.
-
-        """
-        self.widget = QCalendarWidget(self.parent_widget())
-
-    def init_widget(self):
-        """ Initialize the widget.
-
-        """
-        super(QtCalendar, self).init_widget()
-        self.widget.activated.connect(self.on_date_changed)
-
-    #--------------------------------------------------------------------------
-    # Abstract API Implementation
-    #--------------------------------------------------------------------------
-    def get_date(self):
-        """ Return the current date in the control.
-
-        Returns
-        -------
-        result : date
-            The current control date as a Python date object.
-
-        """
-        return self.widget.selectedDate().toPython()
-
-    def set_minimum(self, date):
-        """ Set the widget's minimum date.
-
-        Parameters
-        ----------
-        date : date
-            The date object to use for setting the minimum date.
-
-        """
-        self.widget.setMinimumDate(date)
-
-    def set_maximum(self, date):
-        """ Set the widget's maximum date.
+    def __init__(self, parent=None):
+        """ Initialize a QDockFrameLayout.
 
         Parameters
         ----------
-        date : date
-            The date object to use for setting the maximum date.
+        parent : QWidget or None
+            The parent widget owner of the layout.
 
         """
-        self.widget.setMaximumDate(date)
+        super(QDockFrameLayout, self).__init__(parent)
+        self._size_hint = QSize()
+        self._min_size = QSize()
+        self._max_size = QSize()
 
-    def set_date(self, date):
-        """ Set the widget's current date.
-
-        Parameters
-        ----------
-        date : date
-            The date object to use for setting the date.
+    #--------------------------------------------------------------------------
+    # QLayout API
+    #--------------------------------------------------------------------------
+    def invalidate(self):
+        """ Invalidate the cached layout data.
 
         """
-        self._guard |= CHANGED_GUARD
-        try:
-            self.widget.setSelectedDate(date)
-        finally:
-            self._guard &= ~CHANGED_GUARD
+        super(QDockFrameLayout, self).invalidate()
+        self._size_hint = QSize()
+        self._min_size = QSize()
+        self._max_size = QSize()
+
+    def sizeHint(self):
+        """ Get the size hint for the layout.
+
+        """
+        hint = self._size_hint
+        if hint.isValid():
+            return hint
+        hint = super(QDockFrameLayout, self).sizeHint()
+        if not hint.isValid():
+            hint = QSize(256, 192)
+        self._size_hint = hint
+        return hint
+
+    def minimumSize(self):
+        """ Get the minimum size for the layout.
+
+        """
+        size = self._min_size
+        if size.isValid():
+            return size
+        size = super(QDockFrameLayout, self).minimumSize()
+        if not size.isValid():
+            size = QSize(256, 192)
+        self._min_size = size
+        return size
+
+    def maximumSize(self):
+        """ Get the maximum size for the layout.
+
+        """
+        size = self._max_size
+        if size.isValid():
+            return size
+        size = super(QDockFrameLayout, self).maximumSize()
+        self._max_size = size
+        return size
```

### Comparing `enaml-0.9.7/enaml/qt/qt_widget.py` & `enaml-0.9.8/enaml/qt/qt_stack.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,414 +1,422 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from atom.api import Typed, Coerced
+from atom.api import Int, IntEnum, Typed
 
-from enaml.styling import StyleCache
-from enaml.widgets.widget import Feature, ProxyWidget
+from enaml.widgets.stack import ProxyStack
 
-from .QtCore import Qt, QSize
-from .QtGui import QFont, QWidget, QWidgetAction, QApplication
+from .QtCore import QTimer, QEvent, Signal
+from .QtGui import QStackedWidget, QPixmap
 
-from . import focus_registry
-from .q_resource_helpers import get_cached_qcolor, get_cached_qfont
-from .qt_toolkit_object import QtToolkitObject
-from .styleutil import translate_style
-
-
-class QtWidget(QtToolkitObject, ProxyWidget):
-    """ A Qt implementation of an Enaml ProxyWidget.
+from .q_pixmap_painter import QPixmapPainter
+from .q_pixmap_transition import (
+    QDirectedTransition, QSlideTransition, QWipeTransition, QIrisTransition,
+    QFadeTransition, QCrossFadeTransition
+)
+from .qt_constraints_widget import QtConstraintsWidget
+from .qt_stack_item import QtStackItem
+
+
+TRANSITION_TYPE = {
+    'slide': QSlideTransition,
+    'wipe': QWipeTransition,
+    'iris': QIrisTransition,
+    'fade': QFadeTransition,
+    'crossfade': QCrossFadeTransition,
+}
+
+
+TRANSITION_DIRECTION = {
+    'left_to_right': QDirectedTransition.LeftToRight,
+    'right_to_left': QDirectedTransition.RightToLeft,
+    'top_to_bottom': QDirectedTransition.TopToBottom,
+    'bottom_to_top': QDirectedTransition.BottomToTop,
+}
+
+
+def make_transition(transition):
+    """ Make a QPixmapTransition from an Enaml Transition.
+
+    Parameters
+    ----------
+    transition : Transition
+        The Enaml Transition object.
+
+    Returns
+    -------
+    result : QPixmapTransition
+        A QPixmapTransition to use as the transition.
 
     """
-    #: A reference to the toolkit widget created by the proxy.
-    widget = Typed(QWidget)
-
-    #: A private copy of the declaration features. This ensures that
-    #: feature cleanup will proceed correctly in the event that user
-    #: code modifies the declaration features value at runtime.
-    _features = Coerced(Feature.Flags)
-
-    #: Internal storage for the shared widget action.
-    _widget_action = Typed(QWidgetAction)
-
-    #--------------------------------------------------------------------------
-    # Initialization API
-    #--------------------------------------------------------------------------
-    def create_widget(self):
-        """ Create the underlying QWidget object.
-
-        """
-        self.widget = QWidget(self.parent_widget())
+    qtransition = TRANSITION_TYPE[transition.type]()
+    qtransition.setDuration(transition.duration)
+    if isinstance(qtransition, QDirectedTransition):
+        qtransition.setDirection(TRANSITION_DIRECTION[transition.direction])
+    return qtransition
 
-    def init_widget(self):
-        """ Initialize the underlying QWidget object.
 
-        """
-        super(QtWidget, self).init_widget()
-        widget = self.widget
-        focus_registry.register(widget, self)
-        self._setup_features()
-        d = self.declaration
-        if d.background:
-            self.set_background(d.background)
-        if d.foreground:
-            self.set_foreground(d.foreground)
-        if d.font:
-            self.set_font(d.font)
-        if -1 not in d.minimum_size:
-            self.set_minimum_size(d.minimum_size)
-        if -1 not in d.maximum_size:
-            self.set_maximum_size(d.maximum_size)
-        if d.tool_tip:
-            self.set_tool_tip(d.tool_tip)
-        if d.status_tip:
-            self.set_status_tip(d.status_tip)
-        if not d.enabled:
-            self.set_enabled(d.enabled)
-        self.refresh_style_sheet()
-        # Don't make toplevel widgets visible during init or they will
-        # flicker onto the screen. This applies particularly for things
-        # like status bar widgets which are created with no parent and
-        # then reparented by the status bar. Real top-level widgets must
-        # be explicitly shown by calling their .show() method after they
-        # are created.
-        if widget.parent() or not d.visible:
-            self.set_visible(d.visible)
-
-    def destroy(self):
-        """ Destroy the underlying QWidget object.
-
-        """
-        self._teardown_features()
-        focus_registry.unregister(self.widget)
-        super(QtWidget, self).destroy()
-        # If a QWidgetAction was created for this widget, then it has
-        # taken ownership of the widget and the widget will be deleted
-        # when the QWidgetAction is garbage collected. This means the
-        # superclass destroy() method must run before the reference to
-        # the QWidgetAction is dropped.
-        del self._widget_action
+class QStack(QStackedWidget):
+    """ A QStackedWidget subclass which adds support for transitions.
 
-    #--------------------------------------------------------------------------
-    # Private API
-    #--------------------------------------------------------------------------
-    def _setup_features(self):
-        """ Setup the advanced widget feature handlers.
+    """
+    class SizeHintMode(IntEnum):
+        """ An int enum defining the size hint modes of the stack.
 
         """
-        features = self._features = self.declaration.features
-        if not features:
-            return
-        if features & Feature.FocusTraversal:
-            self.hook_focus_traversal()
-        if features & Feature.FocusEvents:
-            self.hook_focus_events()
+        #: The size hint is the union of all stack items.
+        Union = 0
 
-    def _teardown_features(self):
-        """ Teardowns the advanced widget feature handlers.
+        #: The size hint is the size hint of the current stack item.
+        Current = 1
 
-        """
-        features = self._features
-        if not features:
-            return
-        if features & Feature.FocusTraversal:
-            self.unhook_focus_traversal()
-        if features & Feature.FocusEvents:
-            self.unhook_focus_events()
-
-    #--------------------------------------------------------------------------
-    # Protected API
-    #--------------------------------------------------------------------------
-    def refresh_style_sheet(self):
-        """ Refresh the widget style sheet with the current style data.
-
-        """
-        parts = []
-        name = self.widget.objectName()
-        for style in StyleCache.styles(self.declaration):
-            t = translate_style(name, style)
-            if t:
-                parts.append(t)
-        if len(parts) > 0:
-            stylesheet = u'\n\n'.join(parts)
-        else:
-            stylesheet = u''
-        self.widget.setStyleSheet(stylesheet)
+    #: Proxy the SizeHintMode values as if it were an anonymous enum.
+    Union = SizeHintMode.Union
+    Current = SizeHintMode.Current
 
-    def tab_focus_request(self, reason):
-        """ Handle a custom tab focus request.
+    #: A signal emitted when a LayoutRequest event is posted to the
+    #: stack widget. This will typically occur when the size hint of
+    #: the stack is no longer valid.
+    layoutRequested = Signal()
 
-        This method is called when focus is being set on the proxy
-        as a result of a user-implemented focus traversal handler.
-        This can be reimplemented by subclasses as needed.
+    def __init__(self, *args, **kwargs):
+        """ Initialize a QStack.
 
         Parameters
         ----------
-        reason : Qt.FocusReason
-            The reason value for the focus request.
-
-        Returns
-        -------
-        result : bool
-            True if focus was set, False otherwise.
+        *args, **kwargs
+            The positional and keyword arguments needed to initalize
+            a QStackedWidget.
 
         """
-        widget = self.focus_target()
-        if ((widget.focusPolicy() & Qt.TabFocus) and
-            widget.isEnabled() and
-            widget.isVisibleTo(widget.window())):
-            widget.setFocus(reason)
-            return True
-        return False
+        super(QStack, self).__init__(*args, **kwargs)
+        self._painter = None
+        self._transition = None
+        self._transition_index = 0
+        self._size_hint_mode = QStack.Union
 
-    def focus_target(self):
-        """ Return the current focus target for a focus request.
+    #--------------------------------------------------------------------------
+    # Private API
+    #--------------------------------------------------------------------------
+    def _onTransitionFinished(self):
+        """ A signal handler for the `finished` signal of the transition.
 
-        This can be reimplemented by subclasses as needed. The default
-        implementation of this method returns the current proxy widget.
+        This method resets the internal painter and triggers the normal
+        index change for the stacked widget.
 
         """
-        return self.widget
-
-    def hook_focus_traversal(self):
-        """ Install the hooks for focus traversal.
-
-        This method may be overridden by subclasses as needed.
+        painter = self._painter
+        if painter is not None:
+            painter.setTargetWidget(None)
+        self._painter = None
+        self.setCurrentIndex(self._transition_index)
+        # This final show() makes sure the underlyling widget is visible.
+        # If transitions are being fired rapidly, it's possible that the
+        # current index and the transition index will be the same when
+        # the call above is invoked. In such cases, Qt short circuits the
+        # evaluation and the current widget is not shown.
+        self.currentWidget().show()
+
+    def _runTransition(self):
+        """ A private method which runs the transition effect.
+
+        The `_transition_index` attribute should be set before calling
+        this method. If no transition object exists for this widget,
+        then it is equivalent to calling `setCurrentIndex`. If the new
+        index is not different from the current index the transition
+        will not be performed.
 
         """
-        self.widget.focusNextPrevChild = self.focusNextPrevChild
+        from_index = self.currentIndex()
+        to_index = self._transition_index
 
-    def unhook_focus_traversal(self):
-        """ Remove the hooks for the next/prev child focusing.
+        # If the index hasn't changed, there is nothing to update.
+        if from_index == to_index:
+            return
 
-        This method may be overridden by subclasses as needed.
+        # If there is no transition applied, just change the index.
+        transition = self._transition
+        if transition is None:
+            self.setCurrentIndex(to_index)
+            return
 
-        """
-        del self.widget.focusNextPrevChild
+        # Otherwise, grab the pixmaps for the start and ending states
+        # and set them on the transtion. The widgets are resized to the
+        # current size so that the pixmaps are grabbed in a good state.
+        src_widget = self.widget(from_index)
+        dst_widget = self.widget(to_index)
+        size = self.size()
+        src_widget.resize(size)
+        dst_widget.resize(size)
+        src_pixmap = QPixmap.grabWidget(src_widget)
+        dst_pixmap = QPixmap.grabWidget(dst_widget)
+        out_pixmap = QPixmap(size)
+        transition.setPixmaps(src_pixmap, dst_pixmap, out_pixmap)
+
+        # Hide both of the constituent widgets so that the painter has
+        # a clean widget on which to draw.
+        src_widget.setVisible(False)
+        dst_widget.setVisible(False)
+
+        # Hookup the pixmap painter and start the transition.
+        painter = self._painter = QPixmapPainter()
+        painter.setTargetWidget(self)
+        transition.pixmapUpdated.connect(painter.drawPixmap)
+        transition.start()
 
-    def hook_focus_events(self):
-        """ Install the hooks for focus events.
+    #--------------------------------------------------------------------------
+    # Public API
+    #--------------------------------------------------------------------------
+    def event(self, event):
+        """ A custom event handler which handles LayoutRequest events.
 
-        This method may be overridden by subclasses as needed.
+        When a LayoutRequest event is posted to this widget, it will
+        emit the `layoutRequested` signal. This allows an external
+        consumer of this widget to update their external layout.
 
         """
-        widget = self.widget
-        widget.focusInEvent = self.focusInEvent
-        widget.focusOutEvent = self.focusOutEvent
+        res = super(QStack, self).event(event)
+        if event.type() == QEvent.LayoutRequest:
+            self.layoutRequested.emit()
+        return res
 
-    def unhook_focus_events(self):
-        """ Remove the hooks for the focus events.
+    def sizeHint(self):
+        """ A reimplemented size hint handler.
 
-        This method may be overridden by subclasses as needed.
+        This method will compute the size hint based on the size hint
+        of the current tab, instead of the default behavior which is
+        the maximum of all the size hints of the tabs.
 
         """
-        widget = self.widget
-        del widget.focusInEvent
-        del widget.focusOutEvent
+        if self._size_hint_mode == QStack.Current:
+            curr = self.currentWidget()
+            if curr is not None:
+                return curr.sizeHint()
+        return super(QStack, self).sizeHint()
 
-    def focusNextPrevChild(self, next_child):
-        """ The default 'focusNextPrevChild' implementation.
+    def minimumSizeHint(self):
+        """ A reimplemented minimum size hint handler.
 
-        """
-        fd = focus_registry.focused_declaration()
-        if next_child:
-            child = self.declaration.next_focus_child(fd)
-            reason = Qt.TabFocusReason
-        else:
-            child = self.declaration.previous_focus_child(fd)
-            reason = Qt.BacktabFocusReason
-        if child is not None and child.proxy_is_active:
-            return child.proxy.tab_focus_request(reason)
-        widget = self.widget
-        return type(widget).focusNextPrevChild(widget, next_child)
-
-    def focusInEvent(self, event):
-        """ The default 'focusInEvent' implementation.
+        This method will compute the size hint based on the size hint
+        of the current tab, instead of the default behavior which is
+        the maximum of all the minimum size hints of the tabs.
 
         """
-        widget = self.widget
-        type(widget).focusInEvent(widget, event)
-        self.declaration.focus_gained()
+        if self._size_hint_mode == QStack.Current:
+            curr = self.currentWidget()
+            if curr is not None:
+                return curr.minimumSizeHint()
+        return super(QStack, self).minimumSizeHint()
 
-    def focusOutEvent(self, event):
-        """ The default 'focusOutEvent' implementation.
+    def sizeHintMode(self):
+        """ Get the size hint mode of the stack.
 
-        """
-        widget = self.widget
-        type(widget).focusOutEvent(widget, event)
-        self.declaration.focus_lost()
+        Returns
+        -------
+        result : QStack.SizeHintMode
+            The size hint mode enum value for the stack.
 
-    #--------------------------------------------------------------------------
-    # Framework API
-    #--------------------------------------------------------------------------
-    def get_action(self, create=False):
-        """ Get the shared widget action for this widget.
+        """
+        return self._size_hint_mode
 
-        This API is used to support widgets in tool bars and menus.
+    def setSizeHintMode(self, mode):
+        """ Set the size hint mode of the stack.
 
         Parameters
         ----------
-        create : bool, optional
-            Whether to create the action if it doesn't already exist.
-            The default is False.
+        mode : QStack.SizeHintMode
+            The size hint mode for the stack.
+
+        """
+        assert isinstance(mode, QStack.SizeHintMode)
+        self._size_hint_mode = mode
+
+    def transition(self):
+        """ Get the transition installed on this widget.
 
         Returns
         -------
-        result : QWidgetAction or None
-            The cached widget action or None, depending on arguments.
+        result : QPixmapTransition or None
+            The pixmap transition installed on this widget, or None if
+            no transition is being used.
 
         """
-        action = self._widget_action
-        if action is None and create:
-            action = self._widget_action = QWidgetAction(None)
-            action.setDefaultWidget(self.widget)
-        return action
+        return self._transition
 
-    #--------------------------------------------------------------------------
-    # ProxyWidget API
-    #--------------------------------------------------------------------------
-    def set_minimum_size(self, min_size):
-        """ Sets the minimum size of the widget.
+    def setTransition(self, transition):
+        """ Set the transition to be used by this widget.
 
-        """
-        # QWidget uses (0, 0) as the minimum size.
-        if -1 in min_size:
-            min_size = (0, 0)
-        self.widget.setMinimumSize(QSize(*min_size))
+        Parameters
+        ----------
+        transition : QPixmapTransition or None
+            The transition to use when changing between widgets on this
+            stack or None if no transition should be used.
+
+        """
+        old = self._transition
+        if old is not None:
+            old.finished.disconnect(self._onTransitionFinished)
+        self._transition = transition
+        if transition is not None:
+            transition.finished.connect(self._onTransitionFinished)
+
+    def transitionTo(self, index):
+        """ Transition the stack widget to the given index.
+
+        If there is no transition object is installed on the widget
+        this is equivalent to calling `setCurrentIndex`. Otherwise,
+        the change will be animated using the installed transition.
 
-    def set_maximum_size(self, max_size):
-        """ Sets the maximum size of the widget.
+        Parameters
+        ----------
+        index : int
+            The index of the target transition widget.
 
         """
-        # QWidget uses 16777215 as the max size
-        if -1 in max_size:
-            max_size = (16777215, 16777215)
-        self.widget.setMaximumSize(QSize(*max_size))
+        if index < 0 or index >= self.count():
+            return
+        self._transition_index = index
+        if self.transition() is not None:
+            QTimer.singleShot(0, self._runTransition)
+        else:
+            self.setCurrentIndex(index)
 
-    def set_enabled(self, enabled):
-        """ Set the enabled state of the widget.
 
-        """
-        self.widget.setEnabled(enabled)
-        action = self._widget_action
-        if action is not None:
-            action.setEnabled(enabled)
+#: A mapping Enaml -> Qt size hint modes.
+SIZE_HINT_MODE = {
+    'union': QStack.Union,
+    'current': QStack.Current,
+}
 
-    def set_visible(self, visible):
-        """ Set the visibility of the widget.
 
-        """
-        self.widget.setVisible(visible)
-        action = self._widget_action
-        if action is not None:
-            action.setVisible(visible)
+#: Cyclic notification guard
+INDEX_FLAG = 0x1
 
-    def set_background(self, background):
-        """ Set the background color of the widget.
 
-        """
-        widget = self.widget
-        role = widget.backgroundRole()
-        if background is not None:
-            qcolor = get_cached_qcolor(background)
-            widget.setAutoFillBackground(True)
-        else:
-            app_palette = QApplication.instance().palette(widget)
-            qcolor = app_palette.color(role)
-            widget.setAutoFillBackground(False)
-        palette = widget.palette()
-        palette.setColor(role, qcolor)
-        widget.setPalette(palette)
+class QtStack(QtConstraintsWidget, ProxyStack):
+    """ A Qt implementation of an Enaml Stack.
 
-    def set_foreground(self, foreground):
-        """ Set the foreground color of the widget.
+    """
+    #: A reference to the widget created by the proxy.
+    widget = Typed(QStack)
 
-        """
-        widget = self.widget
-        role = widget.foregroundRole()
-        if foreground is not None:
-            qcolor = get_cached_qcolor(foreground)
-        else:
-            app_palette = QApplication.instance().palette(widget)
-            qcolor = app_palette.color(role)
-        palette = widget.palette()
-        palette.setColor(role, qcolor)
-        widget.setPalette(palette)
+    #: Cyclic notification guards
+    _guard = Int(0)
 
-    def set_font(self, font):
-        """ Set the font of the widget.
+    #--------------------------------------------------------------------------
+    # Initialization API
+    #--------------------------------------------------------------------------
+    def create_widget(self):
+        """ Create the underlying QStack widget.
 
         """
-        if font is not None:
-            self.widget.setFont(get_cached_qfont(font))
-        else:
-            self.widget.setFont(QFont())
+        self.widget = QStack(self.parent_widget())
 
-    def set_tool_tip(self, tool_tip):
-        """ Set the tool tip for the widget.
+    def init_widget(self):
+        """ Initialize the underlying control.
 
         """
-        self.widget.setToolTip(tool_tip)
+        super(QtStack, self).init_widget()
+        d = self.declaration
+        self.set_transition(d.transition)
+        self.set_size_hint_mode(d.size_hint_mode, update=False)
 
-    def set_status_tip(self, status_tip):
-        """ Set the status tip for the widget.
+    def init_layout(self):
+        """ Initialize the layout of the underlying control.
 
         """
-        self.widget.setStatusTip(status_tip)
+        super(QtStack, self).init_layout()
+        widget = self.widget
+        for item in self.stack_items():
+            widget.addWidget(item)
+        # Bypass the transition effect during initialization.
+        widget.setCurrentIndex(self.declaration.index)
+        widget.layoutRequested.connect(self.on_layout_requested)
+        widget.currentChanged.connect(self.on_current_changed)
 
-    def ensure_visible(self):
-        """ Ensure the widget is visible.
+    #--------------------------------------------------------------------------
+    # Utility Methods
+    #--------------------------------------------------------------------------
+    def stack_items(self):
+        """ Get the stack items defined on the control.
 
         """
-        self.widget.setVisible(True)
-        action = self._widget_action
-        if action is not None:
-            action.setVisible(True)
+        for d in self.declaration.stack_items():
+            w = d.proxy.widget
+            if w is not None:
+                yield w
 
-    def ensure_hidden(self):
-        """ Ensure the widget is hidden.
+    #--------------------------------------------------------------------------
+    # Child Events
+    #--------------------------------------------------------------------------
+    def child_added(self, child):
+        """ Handle the child added event for a QtStack.
 
         """
-        self.widget.setVisible(False)
-        action = self._widget_action
-        if action is not None:
-            action.setVisible(False)
+        super(QtStack, self).child_added(child)
+        if isinstance(child, QtStackItem):
+            for index, dchild in enumerate(self.children()):
+                if child is dchild:
+                    self.widget.insertWidget(index, child.widget)
 
-    def restyle(self):
-        """ Restyle the widget with the current style data.
+    def child_removed(self, child):
+        """ Handle the child removed event for a QtStack.
 
         """
-        self.refresh_style_sheet()
+        super(QtStack, self).child_removed(child)
+        if isinstance(child, QtStackItem):
+            self.widget.removeWidget(child.widget)
 
-    def set_focus(self):
-        """ Set the keyboard input focus to this widget.
+    #--------------------------------------------------------------------------
+    # Signal Handlers
+    #--------------------------------------------------------------------------
+    def on_layout_requested(self):
+        """ Handle the `layoutRequested` signal from the QStack.
 
         """
-        self.focus_target().setFocus(Qt.OtherFocusReason)
+        self.geometry_updated()
 
-    def clear_focus(self):
-        """ Clear the keyboard input focus from this widget.
+    def on_current_changed(self):
+        """ Handle the `currentChanged` signal from the QStack.
 
         """
-        self.focus_target().clearFocus()
+        if not self._guard & INDEX_FLAG:
+            self._guard |= INDEX_FLAG
+            try:
+                self.declaration.index = self.widget.currentIndex()
+            finally:
+                self._guard &= ~INDEX_FLAG
 
-    def has_focus(self):
-        """ Test whether this widget has input focus.
+    #--------------------------------------------------------------------------
+    # Widget Update Methods
+    #--------------------------------------------------------------------------
+    def set_index(self, index):
+        """ Set the current index of the underlying widget.
 
         """
-        return self.focus_target().hasFocus()
+        if not self._guard & INDEX_FLAG:
+            self._guard |= INDEX_FLAG
+            try:
+                self.widget.transitionTo(index)
+            finally:
+                self._guard &= ~INDEX_FLAG
 
-    def focus_next_child(self):
-        """ Give focus to the next widget in the focus chain.
+    def set_transition(self, transition):
+        """ Set the transition on the underlying widget.
 
         """
-        self.focus_target().focusNextChild()
+        if transition:
+            self.widget.setTransition(make_transition(transition))
+        else:
+            self.widget.setTransition(None)
 
-    def focus_previous_child(self):
-        """ Give focus to the previous widget in the focus chain.
+    def set_size_hint_mode(self, mode, update=True):
+        """ Set the size hint mode for the widget.
 
         """
-        self.focus_target().focusPreviousChild()
+        self.widget.setSizeHintMode(SIZE_HINT_MODE[mode])
+        if update:
+            self.geometry_updated()
```

### Comparing `enaml-0.9.7/enaml/qt/qt_dialog.py` & `enaml-0.9.8/enaml/qt/qt_dialog.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_ipython_console.py` & `enaml-0.9.8/enaml/qt/qt_ipython_console.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_scroll_area.py` & `enaml-0.9.8/enaml/qt/qt_dock_item.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,221 +1,230 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from atom.api import Typed, Value
+from atom.api import Int, Typed
 
-from enaml.widgets.scroll_area import ProxyScrollArea
+from enaml.styling import StyleCache
+from enaml.widgets.dock_item import ProxyDockItem
 
-from .QtCore import Qt, QEvent, QSize, QRect, QPoint, Signal
-from .QtGui import QApplication, QScrollArea, QPainter, QPalette
+from .QtCore import Qt, QSize, Signal
+from .QtGui import QIcon
 
-from .qt_container import QtContainer
-from .qt_frame import QtFrame
+from .docking.q_dock_item import QDockItem
 
+from .q_resource_helpers import get_cached_qicon
+from .qt_widget import QtWidget
+from .styleutil import translate_dock_item_style
 
-POLICIES = {
-    'as_needed': Qt.ScrollBarAsNeeded,
-    'always_off': Qt.ScrollBarAlwaysOff,
-    'always_on': Qt.ScrollBarAlwaysOn
-}
 
+class QCustomDockItem(QDockItem):
+    """ A custom dock item which converts a close event into a signal.
 
-class QCustomScrollArea(QScrollArea):
-    """ A custom QScrollArea for use with the QtScrollArea.
+    """
+    #: A signal emitted if the close event is accepted. It it emitted
+    #: before the close event handler returns.
+    closed = Signal()
 
-    This subclass fixes some bugs related to size hints.
+    def closeEvent(self, event):
+        """ Handle the close event for the dock item.
 
-    """
-    #: A signal emitted when a LayoutRequest event is posted to the
-    #: scroll area. This will typically occur when the size hint of
-    #: the scroll area is no longer valid.
-    layoutRequested = Signal()
-
-    #: A private internally cached size hint.
-    _size_hint = QSize()
-
-    def event(self, event):
-        """ A custom event handler for the scroll area.
-
-        This handler dispatches layout requests and paints the empty
-        corner between the scroll bars.
-
-        """
-        res = super(QCustomScrollArea, self).event(event)
-        event_t = event.type()
-        if event_t == QEvent.Paint:
-            # Fill in the empty corner area with the app window color.
-            color = QApplication.palette().color(QPalette.Window)
-            tl = self.viewport().geometry().bottomRight()
-            fw = self.frameWidth()
-            br = self.rect().bottomRight() - QPoint(fw, fw)
-            QPainter(self).fillRect(QRect(tl, br), color)
-        elif event_t == QEvent.LayoutRequest:
-            self._size_hint = QSize()
-            self.layoutRequested.emit()
-        return res
-
-    def setWidget(self, widget):
-        """ Set the widget for this scroll area.
-
-        This is a reimplemented parent class method which invalidates
-        the cached size hint before setting the widget.
-
-        """
-        self._size_hint = QSize()
-        self.takeWidget()  # Let Python keep ownership of the old widget
-        super(QCustomScrollArea, self).setWidget(widget)
-
-    def sizeHint(self):
-        """ Get the size hint for the scroll area.
-
-        This reimplemented method fixes a Qt bug where the size hint
-        is not updated after the scroll widget is first shown. The
-        bug is documented on the Qt bug tracker:
-        https://bugreports.qt-project.org/browse/QTBUG-10545
-
-        """
-        # This code is ported directly from QScrollArea.cpp but instead
-        # of caching the size hint of the scroll widget, it caches the
-        # size hint for the entire scroll area, and invalidates it when
-        # the widget is changed or it receives a LayoutRequest event.
-        hint = self._size_hint
-        if hint.isValid():
-            return QSize(hint)
-        fw = 2 * self.frameWidth()
-        hint = QSize(fw, fw)
-        font_height = self.fontMetrics().height()
-        widget = self.widget()
-        if widget is not None:
-            if self.widgetResizable():
-                hint += widget.sizeHint()
-            else:
-                hint += widget.size()
-        else:
-            hint += QSize(12 * font_height, 8 * font_height)
-        if self.verticalScrollBarPolicy() == Qt.ScrollBarAlwaysOn:
-            vbar = self.verticalScrollBar()
-            hint.setWidth(hint.width() + vbar.sizeHint().width())
-        if self.horizontalScrollBarPolicy() == Qt.ScrollBarAlwaysOn:
-            hbar = self.horizontalScrollBar()
-            hint.setHeight(hint.height() + hbar.sizeHint().height())
-        hint = hint.boundedTo(QSize(36 * font_height, 24 * font_height))
-        self._size_hint = hint
-        return QSize(hint)
+        """
+        super(QCustomDockItem, self).closeEvent(event)
+        if event.isAccepted():
+            self.closed.emit()
+
+
+# Guard flags
+TITLE_GUARD = 0x1
 
 
-class QtScrollArea(QtFrame, ProxyScrollArea):
-    """ A Qt implementation of an Enaml ProxyScrollArea.
+class QtDockItem(QtWidget, ProxyDockItem):
+    """ A Qt implementation of an Enaml ProxyDockItem.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(QCustomScrollArea)
+    widget = Typed(QCustomDockItem)
 
-    #: A private cache of the old size hint for the scroll area.
-    _old_hint = Value()
+    #: Cyclic notification guard. This a bitfield of multiple guards.
+    _guard = Int(0)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying QScrollArea widget.
+        """ Create the underlying QDockItem widget.
 
         """
-        self.widget = QCustomScrollArea(self.parent_widget())
+        self.widget = QCustomDockItem(self.parent_widget())
 
     def init_widget(self):
-        """ Initialize the underlying widget.
+        """ Initialize the state of the underlying widget.
 
         """
-        super(QtScrollArea, self).init_widget()
+        super(QtDockItem, self).init_widget()
         d = self.declaration
-        self.set_horizontal_policy(d.horizontal_policy)
-        self.set_vertical_policy(d.vertical_policy)
-        self.set_widget_resizable(d.widget_resizable)
+        self.set_title(d.title)
+        self.set_title_editable(d.title_editable)
+        if not d.title_bar_visible:
+            self.set_title_bar_visible(d.title_bar_visible)
+        if d.icon is not None:
+            self.set_icon(d.icon)
+        if -1 not in d.icon_size:
+            self.set_icon_size(d.icon_size)
+        self.set_stretch(d.stretch)
+        self.set_closable(d.closable)
 
     def init_layout(self):
-        """ Initialize the layout of the underlying widget.
+        """ Initialize the layout for the underyling widget.
 
         """
-        super(QtScrollArea, self).init_layout()
+        super(QtDockItem, self).init_layout()
         widget = self.widget
-        widget.setWidget(self.scroll_widget())
-        widget.layoutRequested.connect(self.on_layout_requested)
+        widget.setDockWidget(self.dock_widget())
+        # Use a queued connection so the dock manager can finish
+        # closing the dock item before the signal handler runs.
+        widget.titleEdited.connect(self.on_title_edited)
+        widget.titleBarRightClicked.connect(self.on_title_bar_right_clicked)
+        widget.closed.connect(self.on_closed, Qt.QueuedConnection)
 
     #--------------------------------------------------------------------------
     # Utility Methods
     #--------------------------------------------------------------------------
-    def scroll_widget(self):
-        """ Find and return the scroll widget child for this widget.
+    def dock_widget(self):
+        """ Find and return the dock widget child for this widget.
 
         """
-        w = self.declaration.scroll_widget()
-        if w is not None:
-            return w.proxy.widget
+        d = self.declaration.dock_widget()
+        if d is not None:
+            return d.proxy.widget
 
     #--------------------------------------------------------------------------
-    # Child Events
+    # Reimplementations
     #--------------------------------------------------------------------------
-    def child_added(self, child):
-        """ Handle the child added event for a QtScrollArea.
+    def refresh_style_sheet(self):
+        """ A reimplemented styling method.
 
-        """
-        super(QtScrollArea, self).child_added(child)
-        if isinstance(child, QtContainer):
-            self.widget.setWidget(self.scroll_widget())
-
-    def child_removed(self, child):
-        """ Handle the child removed event for a QtScrollArea.
+        The dock item uses custom stylesheet processing.
 
         """
-        super(QtScrollArea, self).child_removed(child)
-        if isinstance(child, QtContainer):
-            self.widget.setWidget(self.scroll_widget())
+        parts = []
+        name = self.widget.objectName()
+        for style in StyleCache.styles(self.declaration):
+            t = translate_dock_item_style(name, style)
+            if t:
+                parts.append(t)
+        if len(parts) > 0:
+            stylesheet = u'\n\n'.join(parts)
+        else:
+            stylesheet = u''
+        self.widget.setStyleSheet(stylesheet)
 
     #--------------------------------------------------------------------------
     # Signal Handlers
     #--------------------------------------------------------------------------
-    def on_layout_requested(self):
-        """ Handle the `layoutRequested` signal from the QScrollArea.
+    def on_title_edited(self, text):
+        """ Handle the 'titleEdited' signal on the dock item.
+
+        """
+        d = self.declaration
+        if d is not None:
+            self._guard |= TITLE_GUARD
+            try:
+                d.title = text
+            finally:
+                self._guard &= ~TITLE_GUARD
+
+    def on_title_bar_right_clicked(self, pos):
+        """ Handle the 'titleBarRightClicked' signal on the dock item.
 
         """
-        new_hint = self.widget.sizeHint()
-        if new_hint != self._old_hint:
-            self._old_hint = new_hint
-            self.geometry_updated()
+        d = self.declaration
+        if d is not None:
+            d.title_bar_right_clicked()
+
+    def on_closed(self):
+        """ Handle the closed signal from the dock item.
+
+        """
+        d = self.declaration
+        if d is not None:
+            d._item_closed()
 
     #--------------------------------------------------------------------------
-    # Overrides
+    # Child Events
     #--------------------------------------------------------------------------
-    def replace_constraints(self, old_cns, new_cns):
-        """ A reimplemented QtConstraintsWidget layout method.
+    def child_added(self, child):
+        """ Handle the child added event for a QtDockItem.
+
+        """
+        super(QtDockItem, self).child_added(child)
+        self.widget.setDockWidget(self.dock_widget())
 
-        Constraints layout may not cross the boundary of a ScrollArea,
-        so this method is no-op which stops the layout propagation.
+    def child_removed(self, child):
+        """ Handle the child added event for a QtDockItem.
 
         """
-        pass
+        super(QtDockItem, self).child_removed(child)
+        self.widget.setDockWidget(self.dock_widget())
 
     #--------------------------------------------------------------------------
-    # ProxyScrollArea API
+    # ProxyDockItem API
     #--------------------------------------------------------------------------
-    def set_horizontal_policy(self, policy):
-        """ Set the horizontal scrollbar policy of the widget.
+    def set_title(self, title):
+        """ Set the title on the underlying widget.
+
+        """
+        if not self._guard & TITLE_GUARD:
+            self.widget.setTitle(title)
+
+    def set_title_editable(self, editable):
+        """ Set the title editable state on the underlying widget.
+
+        """
+        self.widget.setTitleEditable(editable)
+
+    def set_title_bar_visible(self, visible):
+        """ Set the visibility of the widget's title bar.
+
+        """
+        self.widget.setTitleBarForceHidden(not visible)
+
+    def set_icon(self, icon):
+        """ Set the icon on the underlying widget.
+
+        """
+        if icon:
+            qicon = get_cached_qicon(icon)
+        else:
+            qicon = QIcon()
+        self.widget.setIcon(qicon)
+
+    def set_icon_size(self, size):
+        """ Set the icon size on the underlying widget.
+
+        """
+        self.widget.setIconSize(QSize(*size))
+
+    def set_stretch(self, stretch):
+        """ Set the stretch factor for the underlyling widget.
 
         """
-        self.widget.setHorizontalScrollBarPolicy(POLICIES[policy])
+        sp = self.widget.sizePolicy()
+        sp.setHorizontalStretch(stretch)
+        sp.setVerticalStretch(stretch)
+        self.widget.setSizePolicy(sp)
 
-    def set_vertical_policy(self, policy):
-        """ Set the vertical scrollbar policy of the widget.
+    def set_closable(self, closable):
+        """ Set the closable flag for the underlying widget.
 
         """
-        self.widget.setVerticalScrollBarPolicy(POLICIES[policy])
+        self.widget.setClosable(closable)
 
-    def set_widget_resizable(self, resizable):
-        """ Set whether or not the scroll widget is resizable.
+    def alert(self, level, on, off, repeat, persist):
+        """ Set the alert level on the underlying widget.
 
         """
-        self.widget.setWidgetResizable(resizable)
+        self.widget.alert(level, on, off, repeat, persist)
```

### Comparing `enaml-0.9.7/enaml/qt/qt_html.py` & `enaml-0.9.8/enaml/qt/qt_progress_bar.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,47 +3,67 @@
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 from atom.api import Typed
 
-from enaml.widgets.html import ProxyHtml
+from enaml.widgets.progress_bar import ProxyProgressBar
 
-from .QtGui import QTextEdit
+from .QtGui import QProgressBar
 
 from .qt_control import QtControl
 
 
-class QtHtml(QtControl, ProxyHtml):
-    """ A Qt implementation of an Enaml ProxyHtml widget.
+class QtProgressBar(QtControl, ProxyProgressBar):
+    """ A Qt implementation of an Enaml ProxyProgressBar.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(QTextEdit)
+    widget = Typed(QProgressBar)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying html widget.
+        """ Create the underlying progress bar widget.
 
         """
-        widget = QTextEdit(self.parent_widget())
-        widget.setReadOnly(True)
-        self.widget = widget
+        self.widget = QProgressBar(self.parent_widget())
 
     def init_widget(self):
-        """ Initialize the underlying widget.
+        """ Create and initialize the underlying widget.
 
         """
-        super(QtHtml, self).init_widget()
-        self.set_source(self.declaration.source)
+        super(QtProgressBar, self).init_widget()
+        d = self.declaration
+        self.set_minimum(d.minimum)
+        self.set_maximum(d.maximum)
+        self.set_value(d.value)
+        self.set_text_visible(d.text_visible)
 
     #--------------------------------------------------------------------------
-    # ProxyHtml API
+    # ProxyProgressBar API
     #--------------------------------------------------------------------------
-    def set_source(self, source):
-        """ Set the source of the html widget
+    def set_minimum(self, value):
+        """ Set the minimum value of the widget.
 
         """
-        self.widget.setHtml(source)
+        self.widget.setMinimum(value)
+
+    def set_maximum(self, value):
+        """ Set the maximum value of the widget.
+
+        """
+        self.widget.setMaximum(value)
+
+    def set_value(self, value):
+        """ Set the value of the widget.
+
+        """
+        self.widget.setValue(value)
+
+    def set_text_visible(self, visible):
+        """ Set the text visibility on the widget.
+
+        """
+        self.widget.setTextVisible(visible)
```

### Comparing `enaml-0.9.7/enaml/qt/qt_object_combo.py` & `enaml-0.9.8/enaml/qt/qt_object_combo.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_popup_view.py` & `enaml-0.9.8/enaml/qt/qt_mdi_window.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,180 +3,133 @@
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 from atom.api import Typed
 
-from enaml.widgets.popup_view import ProxyPopupView
+from enaml.widgets.mdi_window import ProxyMdiWindow
 
-from .QtCore import Qt, QPointF, QPoint
+from .QtGui import QMdiSubWindow, QLayout, QIcon
 
-from .q_popup_view import QPopupView, ArrowEdge, AnchorMode
+from .q_resource_helpers import get_cached_qicon
 from .qt_widget import QtWidget
 
 
-EDGES = {
-    'left': ArrowEdge.Left,
-    'right': ArrowEdge.Right,
-    'top': ArrowEdge.Top,
-    'bottom': ArrowEdge.Bottom,
-}
-
-
-WINDOW_TYPES = {
-    'popup': Qt.Popup,
-    'tool_tip': Qt.ToolTip,
-    'window': Qt.Window,
-}
-
-
-ANCHOR_MODE = {
-    'parent': AnchorMode.Parent,
-    'cursor': AnchorMode.Cursor,
-}
-
-
-class QtPopupView(QtWidget, ProxyPopupView):
-    """ A Qt implementation of an Enaml ProxyPopupView.
+class QtMdiWindow(QtWidget, ProxyMdiWindow):
+    """ A Qt implementation of an Enaml ProxyMdiWindow.
 
     """
-    #: A reference to the toolkit widget created by the proxy.
-    widget = Typed(QPopupView)
+    #: A reference to the widget created by the proxy.
+    widget = Typed(QMdiSubWindow)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the QPopupView widget.
+        """ Create the underlying QMdiSubWindow widget.
 
         """
-        d = self.declaration
-        flags = WINDOW_TYPES[d.window_type]
-        self.widget = QPopupView(self.parent_widget(), flags)
-        if d.translucent_background:
-            self.widget.setAttribute(Qt.WA_TranslucentBackground)
+        # We don't parent the subwindow immediately. It will be added
+        # explicitly by the parent QMdiArea during its layout pass.
+        # If we set the parent here, Qt will spit out warnings when
+        # it's set added to the area later on. We *could* parent it
+        # here, and simply not add it explicitly to the mdi area, but
+        # this way is more explicit and consistent with the rest of
+        # the framework.
+        widget = QMdiSubWindow()
+        widget.layout().setSizeConstraint(QLayout.SetMinAndMaxSize)
+        self.widget = widget
 
     def init_widget(self):
         """ Initialize the widget.
 
         """
-        super(QtPopupView, self).init_widget()
+        super(QtMdiWindow, self).init_widget()
         d = self.declaration
-        self.set_anchor(d.anchor)
-        self.set_anchor_mode(d.anchor_mode)
-        self.set_parent_anchor(d.parent_anchor)
-        self.set_arrow_size(d.arrow_size)
-        self.set_arrow_edge(d.arrow_edge)
-        self.set_offset(d.offset)
-        self.set_timeout(d.timeout)
-        self.set_fade_in_duration(d.fade_in_duration)
-        self.set_fade_out_duration(d.fade_out_duration)
-        self.set_close_on_click(d.close_on_click)
-        self.widget.closed.connect(self.on_closed)
+        if d.title:
+            self.set_title(d.title)
+        if d.icon:
+            self.set_icon(d.icon)
 
     def init_layout(self):
-        """ Initialize the widget layout.
-
-        """
-        super(QtPopupView, self).init_layout()
-        self.widget.setCentralWidget(self.central_widget())
-
-    #--------------------------------------------------------------------------
-    # Public API
-    #--------------------------------------------------------------------------
-    def central_widget(self):
-        """ Find and return the central widget child for this widget.
-
-        Returns
-        -------
-        result : QWidget or None
-            The central widget defined for this widget, or None if one
-            is not defined.
+        """ Initialize the layout for the underlying control.
 
         """
-        d = self.declaration.central_widget()
-        if d is not None:
-            return d.proxy.widget
+        super(QtMdiWindow, self).init_layout()
+        self._set_window_widget(self.mdi_widget())
 
     #--------------------------------------------------------------------------
-    # Signal Handlers
+    # Utility Methods
     #--------------------------------------------------------------------------
-    def on_closed(self):
-        """ The signal handler for the 'closed' signal.
-
-        This handler will notify the declaration object that the popup
-        view has closed.
+    def mdi_widget(self):
+        """ Find and return the mdi widget child for this widget.
 
         """
-        d = self.declaration
-        if d is not None:
-            d._popup_closed()
+        w = self.declaration.mdi_widget()
+        if w:
+            return w.proxy.widget
 
     #--------------------------------------------------------------------------
-    # ProxyBubbleView API
+    # Child Events
     #--------------------------------------------------------------------------
-    def set_anchor(self, anchor):
-        """ Set the anchor location on the underlying widget.
-
-        """
-        self.widget.setAnchor(QPointF(*anchor))
-
-    def set_anchor_mode(self, mode):
-        """ Set the anchor mode on the underlying widget.
+    def child_added(self, child):
+        """ Handle the child added event for a QtMdiWindow.
 
         """
-        self.widget.setAnchorMode(ANCHOR_MODE[mode])
+        super(QtMdiWindow, self).child_added(child)
+        if isinstance(child, QtWidget):
+            self._set_window_widget(self.mdi_widget())
 
-    def set_parent_anchor(self, anchor):
-        """ Set the parent anchor location on the underlying widget.
+    def child_removed(self, child):
+        """ Handle the child removed event for a QtMdiWindow.
 
         """
-        self.widget.setParentAnchor(QPointF(*anchor))
+        super(QtMdiWindow, self).child_added(child)
+        if isinstance(child, QtWidget):
+            self._set_window_widget(self.mdi_widget())
 
-    def set_arrow_size(self, size):
-        """ Set the size of the arrow on the underlying widget.
-
-        """
-        self.widget.setArrowSize(size)
-
-    def set_arrow_edge(self, edge):
-        """ Set the arrow edge on the underlying widget.
-
-        """
-        self.widget.setArrowEdge(EDGES[edge])
-
-    def set_offset(self, offset):
-        """ Set the offset of the underlying widget.
-
-        """
-        self.widget.setOffset(QPoint(*offset))
-
-    def set_timeout(self, timeout):
-        """ Set the timeout for the underlying widget.
-
-        """
-        self.widget.setTimeout(timeout)
-
-    def set_fade_in_duration(self, duration):
-        """ Set the fade in duration for the underlying widget.
+    #--------------------------------------------------------------------------
+    # ProxyMdiWindow API
+    #--------------------------------------------------------------------------
+    def set_icon(self, icon):
+        """ Set the mdi window icon.
 
         """
-        self.widget.setFadeInDuration(duration)
+        if icon:
+            qicon = get_cached_qicon(icon)
+        else:
+            qicon = QIcon()
+        self.widget.setWindowIcon(qicon)
 
-    def set_fade_out_duration(self, duration):
-        """ Set the fade out duration for the underlying widget.
+    def set_title(self, title):
+        """ Set the title of the mdi window.
 
         """
-        self.widget.setFadeOutDuration(duration)
+        self.widget.setWindowTitle(title)
 
-    def set_close_on_click(self, enable):
-        """ Set the close on click flag for the underlying widget.
-
-        """
-        self.widget.setCloseOnClick(enable)
+    #--------------------------------------------------------------------------
+    # Private API
+    #--------------------------------------------------------------------------
+    def _set_window_widget(self, mdi_widget):
+        """ A private method which set the child widget on the window.
 
-    def close(self):
-        """ Close the underlying popup widget.
+        Parameters
+        ----------
+        mdi_widget : QWidget
+            The child widget to use in the mdi window.
 
         """
-        self.widget.close()
+        # We need to first set the window widget to None, or Qt will
+        # complain if a widget is already set on the window.
+        widget = self.widget
+        widget.setWidget(None)
+        if mdi_widget is None:
+            return
+        # We need to unparent the underlying widget before adding
+        # it to the subwindow. Otherwise, children like QMainWindow
+        # will persist as top-level non-mdi widgets.
+        mdi_widget.setParent(None)
+        widget.setWidget(mdi_widget)
+        # On OSX, the resize gripper will be obscured unless we
+        # lower the widget in the window's stacking order.
+        mdi_widget.lower()
```

### Comparing `enaml-0.9.7/enaml/qt/qt_window.py` & `enaml-0.9.8/enaml/qt/qt_main_window.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,71 +5,50 @@
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 import sys
 
 from atom.api import Typed, atomref
 
-from enaml.layout.geometry import Pos, Rect, Size
-from enaml.widgets.window import ProxyWindow, CloseEvent
+from enaml.widgets.main_window import ProxyMainWindow
+from enaml.widgets.window import CloseEvent
 
-from .QtCore import Qt, QPoint, QRect, QSize
-from .QtGui import QApplication, QIcon
+from .QtCore import Qt
+from .QtGui import QMainWindow
 
 from .q_deferred_caller import deferredCall
-from .q_resource_helpers import get_cached_qicon
-from .q_window_base import QWindowBase
 from .qt_container import QtContainer
-from .qt_widget import QtWidget
+from .qt_dock_pane import QtDockPane
+from .qt_menu_bar import QtMenuBar
+from .qt_status_bar import QtStatusBar
+from .qt_tool_bar import QtToolBar
+from .qt_window import QtWindow, finalize_close
 
 
-MODALITY = {
-    'non_modal': Qt.NonModal,
-    'application_modal': Qt.ApplicationModal,
-    'window_modal': Qt.WindowModal,
-}
-
-
-def finalize_close(d):
-    """ Finalize the closing of the declaration object.
-
-    This is performed as a deferred call so that the window may fully
-    close before the declaration is potentially destroyed.
-
-    """
-    d.visible = False
-    d.closed()
-    if d.destroy_on_close:
-        d.destroy()
-
-
-class QWindow(QWindowBase):
-    """ A window base subclass which handles the close event.
-
-    The window layout computes the min/max size of the window based
-    on its central widget, unless the user explicitly changes them.
+class QCustomMainWindow(QMainWindow):
+    """ A custom QMainWindow which adds some Enaml specific features.
 
     """
     def __init__(self, proxy, parent=None, flags=Qt.Widget):
-        """ Initialize a QWindow.
+        """ Initialize a QCustomMainWindow.
 
         Parameters
         ----------
-        proxy : QtWindow
+        proxy : QtMainWindow
             The proxy object which owns this window. Only an atomref
             will be maintained to this object.
 
         parent : QWidget, optional
             The parent of the window.
 
         flags : Qt.WindowFlags, optional
             The window flags to pass to the parent constructor.
 
         """
-        super(QWindow, self).__init__(parent, Qt.Window | flags)
+        super(QCustomMainWindow, self).__init__(parent, Qt.Window | flags)
         self._proxy_ref = atomref(proxy)
 
     def closeEvent(self, event):
         """ Handle the close event for the window.
 
         """
         event.accept()
@@ -80,250 +59,198 @@
         d_event = CloseEvent()
         d.closing(d_event)
         if d_event.is_accepted():
             deferredCall(finalize_close, d)
         else:
             event.ignore()
 
-
-class QtWindow(QtWidget, ProxyWindow):
-    """ A Qt implementation of an Enaml ProxyWindow.
-
-    """
-    #: A reference to the toolkit widget created by the proxy.
-    widget = Typed(QWindow)
-
     #--------------------------------------------------------------------------
-    # Initialization API
+    # Public API
     #--------------------------------------------------------------------------
-    def creation_flags(self):
-        """ A convenience function for getting the creation flags.
-
-        """
-        flags = Qt.Widget
-        if self.declaration.always_on_top:
-            flags |= Qt.WindowStaysOnTopHint
-        return flags
+    def setDockWidgetArea(self, area, dock_widget):
+        """ Set the dock area for the given dock widget.
 
-    def create_widget(self):
-        """ Create the QWindow widget.
+        If the dock widget has not been added to the main window, this
+        method is a no-op.
 
-        """
-        flags = self.creation_flags()
-        self.widget = QWindow(self, self.parent_widget(), flags)
+        Parameters
+        ----------
+        area : QDockWidgetArea
+            The dock area to use for the widget.
 
-    def init_widget(self):
-        """ Initialize the widget.
+        dock_widget : QDockWidget
+            The dock widget to move to the given area.
 
         """
-        super(QtWindow, self).init_widget()
-        d = self.declaration
-        if d.title:
-            self.set_title(d.title)
-        if -1 not in d.initial_size:
-            self.widget.resize(*d.initial_size)
-        if -1 not in d.initial_position:
-            self.widget.move(*d.initial_position)
-        if d.modality != 'non_modal':
-            self.set_modality(d.modality)
-        if d.icon:
-            self.set_icon(d.icon)
+        curr = self.dockWidgetArea(dock_widget)
+        if curr != Qt.NoDockWidgetArea:
+            if curr != area:
+                visible = dock_widget.isVisible()
+                self.removeDockWidget(dock_widget)
+                self.addDockWidget(area, dock_widget)
+                dock_widget.setVisible(visible)
 
-    def init_layout(self):
-        """ Initialize the widget layout.
+    def setToolBarArea(self, area, tool_bar):
+        """ Set the tool bar area for the given tool bar.
 
-        """
-        super(QtWindow, self).init_layout()
-        self.widget.setCentralWidget(self.central_widget())
+        If the tool bar has not been added to the main window, this
+        method is a no-op.
 
-    #--------------------------------------------------------------------------
-    # Public API
-    #--------------------------------------------------------------------------
-    def central_widget(self):
-        """ Find and return the central widget child for this widget.
+        Parameters
+        ----------
+        area : QToolBarArea
+            The tool bar area to use for the widget.
 
-        Returns
-        -------
-        result : QWidget or None
-            The central widget defined for this widget, or None if one
-            is not defined.
+        tool_bar : QToolBar
+            The tool bar to move to the given area.
 
         """
-        d = self.declaration.central_widget()
-        if d is not None:
-            return d.proxy.widget
+        curr = self.toolBarArea(tool_bar)
+        if curr != Qt.NoToolBarArea:
+            if curr != area:
+                visible = tool_bar.isVisible()
+                floating = tool_bar.isFloating()
+                tool_bar.setVisible(False)
+                self.removeToolBar(tool_bar)
+                self.addToolBar(area, tool_bar)
+                tool_bar.resize(tool_bar.sizeHint())
+                tool_bar.setFloating(floating)
+                tool_bar.setVisible(visible)
 
-    #--------------------------------------------------------------------------
-    # Child Events
-    #--------------------------------------------------------------------------
-    def child_added(self, child):
-        """ Handle the child added event for a QtWindow.
-
-        """
-        super(QtWindow, self).child_added(child)
-        if isinstance(child, QtContainer):
-            self.widget.setCentralWidget(self.central_widget())
 
-    def child_removed(self, child):
-        """ Handle the child added event for a QtWindow.
+class QtMainWindow(QtWindow, ProxyMainWindow):
+    """ A Qt implementation of an Enaml MainWindow.
 
-        """
-        super(QtWindow, self).child_removed(child)
-        if isinstance(child, QtContainer):
-            self.widget.setCentralWidget(self.central_widget())
+    """
+    #: A reference to the widget created by the proxy.
+    widget = Typed(QCustomMainWindow)
 
     #--------------------------------------------------------------------------
-    # ProxyWindow API
+    # Initialization API
     #--------------------------------------------------------------------------
-    def set_title(self, title):
-        """ Set the title of the window.
-
-        """
-        self.widget.setWindowTitle(title)
-
-    def set_modality(self, modality):
-        """ Set the modality of the window.
-
-        """
-        self.widget.setWindowModality(MODALITY[modality])
-
-    def set_icon(self, icon):
-        """ Set the window icon.
-
-        """
-        if icon:
-            qicon = get_cached_qicon(icon)
-        else:
-            qicon = QIcon()
-        self.widget.setWindowIcon(qicon)
-
-    def position(self):
-        """ Get the position of the of the window.
-
-        """
-        point = self.widget.pos()
-        return Pos(point.x(), point.y())
-
-    def set_position(self, pos):
-        """ Set the position of the window.
-
-        """
-        self.widget.move(*pos)
-
-    def size(self):
-        """ Get the size of the window.
-
-        """
-        size = self.widget.size()
-        return Size(size.width(), size.height())
-
-    def set_size(self, size):
-        """ Set the size of the window.
-
-        """
-        size = QSize(*size)
-        if size.isValid():
-            self.widget.resize(size)
-
-    def geometry(self):
-        """ Get the geometry of the window.
-
-        """
-        rect = self.widget.geometry()
-        return Rect(rect.x(), rect.y(), rect.width(), rect.height())
-
-    def set_geometry(self, rect):
-        """ Set the geometry of the window.
-
-        """
-        rect = QRect(*rect)
-        if rect.isValid():
-            self.widget.setGeometry(rect)
-
-    def frame_geometry(self):
-        """ Get the geometry of the window.
-
-        """
-        rect = self.widget.frameGeometry()
-        return Rect(rect.x(), rect.y(), rect.width(), rect.height())
-
-    def maximize(self):
-        """ Maximize the window.
-
-        """
-        self.widget.showMaximized()
-
-    def is_maximized(self):
-        """ Get whether the window is maximized.
-
-        """
-        return bool(self.widget.windowState() & Qt.WindowMaximized)
-
-    def minimize(self):
-        """ Minimize the window.
-
-        """
-        self.widget.showMinimized()
-
-    def is_minimized(self):
-        """ Get whether the window is minimized.
+    def create_widget(self):
+        """ Create the underlying widget QMainWindow widget.
 
         """
-        return bool(self.widget.windowState() & Qt.WindowMinimized)
+        flags = self.creation_flags()
+        widget = QCustomMainWindow(self, self.parent_widget(), flags)
+        widget.setDocumentMode(True)
+        widget.setDockNestingEnabled(True)
+        self.widget = widget
 
-    def restore(self):
-        """ Restore the window after a minimize or maximize.
+    def init_layout(self):
+        """ Initialize the layout for the underlying widget.
 
         """
-        self.widget.showNormal()
+        # The superclass' init_layout() method is explicitly not called
+        # since the layout initialization for Window is not appropriate
+        # for MainWindow.
+        widget = self.widget
+        widget.setMenuBar(self.menu_bar())
+        widget.setCentralWidget(self.central_widget())
+        widget.setStatusBar(self.status_bar())
+        for d in self.dock_panes():
+            widget.addDockWidget(d.dockArea(), d)
+        for d in self.tool_bars():
+            # XXX slight hack. When adding the toolbar to the main
+            # window, it is forcibly unfloated. In order for the
+            # initial floating state to be maintained, it must be
+            # re-floating after being added. We do the refloating
+            # in the future, so that the main window shows up first.
+            floating = d.isFloating()
+            widget.addToolBar(d.toolBarArea(), d)
+            if floating:
+                deferredCall(d.setFloating, True)
 
-    def send_to_front(self):
-        """ Move the window to the top of the Z order.
+    #--------------------------------------------------------------------------
+    # Utility Methods
+    #--------------------------------------------------------------------------
+    def menu_bar(self):
+        """ Get the QMenuBar widget defined for the main window.
 
         """
-        self.widget.raise_()
+        d = self.declaration.menu_bar()
+        if d is not None:
+            return d.proxy.widget
 
-    def send_to_back(self):
-        """ Move the window to the bottom of the Z order.
+    def dock_panes(self):
+        """ Get the QDockWidget widgets defined for the main window.
 
         """
-        self.widget.lower()
+        for d in self.declaration.dock_panes():
+            w = d.proxy.widget
+            if w is not None:
+                yield w
 
-    def activate_window(self):
-        """ Activate the underlying window widget.
+    def status_bar(self):
+        """ Get the status bar widget defined for the main window.
 
         """
-        self.widget.activateWindow()
-        if sys.platform == 'win32':
-            # For some reason, this needs to be called twice on Windows
-            # in order to get the taskbar entry to flash.
-            self.widget.activateWindow()
+        d = self.declaration.status_bar()
+        if d is not None:
+            return d.proxy.widget
 
-    def center_on_screen(self):
-        """ Center the window on the screen.
+    def tool_bars(self):
+        """ Get the QToolBar widgets defined for the main window.
 
         """
-        widget = self.widget
-        rect = QRect(QPoint(0, 0), widget.frameGeometry().size())
-        geo = QApplication.desktop().screenGeometry(widget)
-        widget.move(geo.center() - rect.center())
+        for d in self.declaration.tool_bars():
+            w = d.proxy.widget
+            if w is not None:
+                yield w
 
-    def center_on_widget(self, other):
-        """ Center the window on another widget.
+    #--------------------------------------------------------------------------
+    # Child Events
+    #--------------------------------------------------------------------------
+    def child_added(self, child):
+        """ Handle the child added event for a QtMainWindow.
 
         """
-        widget = self.widget
-        rect = QRect(QPoint(0, 0), widget.frameGeometry().size())
-        other_widget = other.proxy.widget
-        if other_widget.isWindow():
-            geo = other_widget.frameGeometry()
+        if isinstance(child, QtMenuBar):
+            self.widget.setMenuBar(self.menu_bar())
+        elif isinstance(child, QtContainer):
+            self.widget.setCentralWidget(self.central_widget())
+        elif isinstance(child, QtDockPane):
+            dock_widget = child.widget
+            self.widget.addDockWidget(dock_widget.dockArea(), dock_widget)
+        elif isinstance(child, QtStatusBar):
+            # FIXME Qt will delete the old status bar
+            self.widget.setStatusBar(self.status_bar())
+        elif isinstance(child, QtToolBar):
+            # There are two hacks involved in adding a tool bar. The
+            # first is the same hack that is perfomed in the layout
+            # method for a floating tool bar. The second is specific
+            # to OSX. On that platform, adding a tool bar to main
+            # window which is already visible but does not have any
+            # current tool bars will cause the main window to be hidden.
+            # This will only occur the *first* time a tool bar is added
+            # to the window. The hack below is workaround which should
+            # be sufficient for most use cases. A bug should really be
+            # filed against Qt for this one, since it's reproducible
+            # outside of Enaml.
+            bar_widget = child.widget
+            floating = bar_widget.isFloating()
+            self.widget.addToolBar(bar_widget.toolBarArea(), bar_widget)
+            if floating:
+                deferredCall(bar_widget.setFloating, True)
+            if sys.platform == 'darwin':
+                self.widget.setVisible(True)
         else:
-            size = other_widget.size()
-            point = other_widget.mapToGlobal(QPoint(0, 0))
-            geo = QRect(point, size)
-        widget.move(geo.center() - rect.center())
+            super(QtMainWindow, self).child_added(child)
 
-    def close(self):
-        """ Close the window.
+    def child_removed(self, child):
+        """ Handle the child removed event for a QtMainWindow.
 
         """
-        self.widget.close()
+        if isinstance(child, QtDockPane) and child.widget is not None:
+            self.widget.removeDockWidget(child.widget)
+        elif isinstance(child, QtToolBar) and child.widget is not None:
+            self.widget.removeToolBar(child.widget)
+        elif isinstance(child, QtContainer):
+            self.widget.setCentralWidget(self.central_widget())
+        elif isinstance(child, QtMenuBar):
+            self.widget.setMenuBar(self.menu_bar())
+        elif isinstance(child, QtStatusBar):
+            # FIXME Qt will delete the old status bar
+            self.widget.setStatusBar(self.status_bar())
+        else:
+            super(QtMainWindow, self).child_removed(child)
```

### Comparing `enaml-0.9.7/enaml/qt/qt_multiline_field.py` & `enaml-0.9.8/enaml/qt/qt_multiline_field.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_focus_tracker.py` & `enaml-0.9.8/enaml/qt/qt_focus_tracker.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_web_view.py` & `enaml-0.9.8/enaml/qt/qt_web_view.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_datetime_selector.py` & `enaml-0.9.8/enaml/qt/qt_datetime_selector.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/q_flow_layout.py` & `enaml-0.9.8/enaml/qt/q_flow_layout.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/q_file_dialog_helper.py` & `enaml-0.9.8/enaml/qt/q_file_dialog_helper.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_group_box.py` & `enaml-0.9.8/enaml/qt/qt_group_box.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_main_window.py` & `enaml-0.9.8/enaml/qt/qt_dock_area.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,256 +1,281 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-import sys
+from atom.api import Typed
 
-from atom.api import Typed, atomref
+from enaml.styling import StyleCache
+from enaml.widgets.dock_area import ProxyDockArea
+from enaml.widgets.dock_events import DockItemEvent
+
+from .QtCore import QObject, QEvent, QSize, QTimer
+from .QtGui import QTabWidget
+
+from .docking.dock_manager import DockManager
+from .docking.event_types import (
+    DockItemDocked, DockItemUndocked, DockItemExtended, DockItemRetracted,
+    DockItemShown, DockItemHidden, DockItemClosed, DockTabSelected
+)
+from .docking.q_dock_area import QDockArea
+from .docking.style_sheets import get_style_sheet
+
+from .qt_constraints_widget import QtConstraintsWidget
+from .qt_dock_item import QtDockItem
+from .styleutil import translate_dock_area_style
+
+
+TAB_POSITIONS = {
+    'top': QTabWidget.North,
+    'bottom': QTabWidget.South,
+    'left': QTabWidget.West,
+    'right': QTabWidget.East,
+}
+
+
+EVENT_TYPES = {
+    DockItemDocked: DockItemEvent.Docked,
+    DockItemUndocked: DockItemEvent.Undocked,
+    DockItemExtended: DockItemEvent.Extended,
+    DockItemRetracted: DockItemEvent.Retracted,
+    DockItemShown: DockItemEvent.Shown,
+    DockItemHidden: DockItemEvent.Hidden,
+    DockItemClosed: DockItemEvent.Closed,
+    DockTabSelected: DockItemEvent.TabSelected,
+}
+
+
+class DockLayoutFilter(QObject):
+    """ An event filter used by the QtDockArea.
+
+    This event filter listens for LayoutRequest events on the dock
+    area widget, and will send a geometry_updated notification to
+    the constraints system when the dock area size hint changes. The
+    notifications are collapsed on a single shot timer so that the
+    dock area geometry can fully settle before being snapped by the
+    constraints layout engine.
 
-from enaml.widgets.main_window import ProxyMainWindow
-from enaml.widgets.window import CloseEvent
-
-from .QtCore import Qt
-from .QtGui import QMainWindow
-
-from .q_deferred_caller import deferredCall
-from .qt_container import QtContainer
-from .qt_dock_pane import QtDockPane
-from .qt_menu_bar import QtMenuBar
-from .qt_status_bar import QtStatusBar
-from .qt_tool_bar import QtToolBar
-from .qt_window import QtWindow, finalize_close
-
-
-class QCustomMainWindow(QMainWindow):
-    """ A custom QMainWindow which adds some Enaml specific features.
+    """
+    def __init__(self, owner):
+        super(DockLayoutFilter, self).__init__()
+        self._owner = owner
+        self._size_hint = QSize()
+        self._pending = False
+        self._timer = timer = QTimer()
+        timer.setSingleShot(True)
+        timer.timeout.connect(self.onNotify)
+
+    def onNotify(self):
+        self._owner.geometry_updated()
+        self._pending = False
+
+    def eventFilter(self, obj, event):
+        if not self._pending and event.type() == QEvent.LayoutRequest:
+            hint = obj.sizeHint()
+            if hint != self._size_hint:
+                self._size_hint = hint
+                self._timer.start(0)
+                self._pending = True
+        return False
+
+
+class DockEventFilter(QObject):
+    """ An event filter used by the QtDockArea.
+
+    This event filter listens for dock events on the dock area widget,
+    converts them to front-end events, and posts them to the front-end
+    declaration object.
 
     """
-    def __init__(self, proxy, parent=None, flags=Qt.Widget):
-        """ Initialize a QCustomMainWindow.
+    def __init__(self, owner):
+        super(DockEventFilter, self).__init__()
+        self._owner = owner
+
+    def eventFilter(self, obj, event):
+        e_type = EVENT_TYPES.get(event.type())
+        if e_type is not None:
+            d = self._owner.declaration
+            if d is not None:
+                d.dock_event(DockItemEvent(type=e_type, name=event.name()))
+        return False
 
-        Parameters
-        ----------
-        proxy : QtMainWindow
-            The proxy object which owns this window. Only an atomref
-            will be maintained to this object.
-
-        parent : QWidget, optional
-            The parent of the window.
-
-        flags : Qt.WindowFlags, optional
-            The window flags to pass to the parent constructor.
-
-        """
-        super(QCustomMainWindow, self).__init__(parent, Qt.Window | flags)
-        self._proxy_ref = atomref(proxy)
-
-    def closeEvent(self, event):
-        """ Handle the close event for the window.
-
-        """
-        event.accept()
-        if not self._proxy_ref:
-            return
-        proxy = self._proxy_ref()
-        d = proxy.declaration
-        d_event = CloseEvent()
-        d.closing(d_event)
-        if d_event.is_accepted():
-            deferredCall(finalize_close, d)
-        else:
-            event.ignore()
 
-    #--------------------------------------------------------------------------
-    # Public API
-    #--------------------------------------------------------------------------
-    def setDockWidgetArea(self, area, dock_widget):
-        """ Set the dock area for the given dock widget.
-
-        If the dock widget has not been added to the main window, this
-        method is a no-op.
+class QtDockArea(QtConstraintsWidget, ProxyDockArea):
+    """ A Qt implementation of an Enaml DockArea.
 
-        Parameters
-        ----------
-        area : QDockWidgetArea
-            The dock area to use for the widget.
-
-        dock_widget : QDockWidget
-            The dock widget to move to the given area.
-
-        """
-        curr = self.dockWidgetArea(dock_widget)
-        if curr != Qt.NoDockWidgetArea:
-            if curr != area:
-                visible = dock_widget.isVisible()
-                self.removeDockWidget(dock_widget)
-                self.addDockWidget(area, dock_widget)
-                dock_widget.setVisible(visible)
-
-    def setToolBarArea(self, area, tool_bar):
-        """ Set the tool bar area for the given tool bar.
-
-        If the tool bar has not been added to the main window, this
-        method is a no-op.
-
-        Parameters
-        ----------
-        area : QToolBarArea
-            The tool bar area to use for the widget.
-
-        tool_bar : QToolBar
-            The tool bar to move to the given area.
-
-        """
-        curr = self.toolBarArea(tool_bar)
-        if curr != Qt.NoToolBarArea:
-            if curr != area:
-                visible = tool_bar.isVisible()
-                floating = tool_bar.isFloating()
-                tool_bar.setVisible(False)
-                self.removeToolBar(tool_bar)
-                self.addToolBar(area, tool_bar)
-                tool_bar.resize(tool_bar.sizeHint())
-                tool_bar.setFloating(floating)
-                tool_bar.setVisible(visible)
+    """
+    #: A reference to the widget created by the proxy.
+    widget = Typed(QDockArea)
 
+    #: The docking manager which will drive the dock area.
+    manager = Typed(DockManager)
 
-class QtMainWindow(QtWindow, ProxyMainWindow):
-    """ A Qt implementation of an Enaml MainWindow.
+    #: The event filter which listens for layout requests.
+    dock_layout_filter = Typed(DockLayoutFilter)
 
-    """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(QCustomMainWindow)
+    #: The event filter which listens for dock events.
+    dock_event_filter = Typed(DockEventFilter)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying widget QMainWindow widget.
+        """ Create the underlying QDockArea widget.
 
         """
-        flags = self.creation_flags()
-        widget = QCustomMainWindow(self, self.parent_widget(), flags)
-        widget.setDocumentMode(True)
-        widget.setDockNestingEnabled(True)
-        self.widget = widget
+        self.widget = QDockArea(self.parent_widget())
+        self.manager = DockManager(self.widget)
+        self.dock_event_filter = DockEventFilter(self)
+        self.dock_layout_filter = DockLayoutFilter(self)
+
+    def init_widget(self):
+        """ Initialize the underlying widget.
+
+        """
+        super(QtDockArea, self).init_widget()
+        d = self.declaration
+        self.set_tab_position(d.tab_position)
+        self.set_live_drag(d.live_drag)
+        if d.style:  # TODO remove this in Enaml 1.0
+            self.set_style(d.style)
+        self.set_dock_events_enabled(d.dock_events_enabled)
 
     def init_layout(self):
-        """ Initialize the layout for the underlying widget.
+        """ Initialize the layout of the underlying control.
 
         """
-        # The superclass' init_layout() method is explicitly not called
-        # since the layout initialization for Window is not appropriate
-        # for MainWindow.
-        widget = self.widget
-        widget.setMenuBar(self.menu_bar())
-        widget.setCentralWidget(self.central_widget())
-        widget.setStatusBar(self.status_bar())
-        for d in self.dock_panes():
-            widget.addDockWidget(d.dockArea(), d)
-        for d in self.tool_bars():
-            # XXX slight hack. When adding the toolbar to the main
-            # window, it is forcibly unfloated. In order for the
-            # initial floating state to be maintained, it must be
-            # re-floating after being added. We do the refloating
-            # in the future, so that the main window shows up first.
-            floating = d.isFloating()
-            widget.addToolBar(d.toolBarArea(), d)
-            if floating:
-                deferredCall(d.setFloating, True)
+        super(QtDockArea, self).init_layout()
+        manager = self.manager
+        for item in self.dock_items():
+            manager.add_item(item)
+        d = self.declaration
+        self.apply_layout(d.layout)
+        self.widget.installEventFilter(self.dock_layout_filter)
+
+    def destroy(self):
+        """ A reimplemented destructor.
+
+        This removes the event filter from the dock area and releases
+        the items from the dock manager.
+
+        """
+        self.widget.removeEventFilter(self.dock_layout_filter)
+        self.widget.removeEventFilter(self.dock_event_filter)
+        del self.dock_layout_filter
+        del self.dock_event_filter
+        self.manager.destroy()
+        super(QtDockArea, self).destroy()
 
     #--------------------------------------------------------------------------
-    # Utility Methods
+    # Overrides
     #--------------------------------------------------------------------------
-    def menu_bar(self):
-        """ Get the QMenuBar widget defined for the main window.
+    def refresh_style_sheet(self):
+        """ A reimplemented styling method.
+
+        The dock area uses custom stylesheet processing.
 
         """
-        d = self.declaration.menu_bar()
-        if d is not None:
-            return d.proxy.widget
+        # workaround win-7 sizing bug
+        parts = [u'QDockTabWidget::pane {}']
+        name = self.widget.objectName()
+        for style in StyleCache.styles(self.declaration):
+            t = translate_dock_area_style(name, style)
+            if t:
+                parts.append(t)
+        if len(parts) > 1:
+            stylesheet = u'\n\n'.join(parts)
+        else:
+            stylesheet = u''
+        self.widget.setStyleSheet(stylesheet)
 
-    def dock_panes(self):
-        """ Get the QDockWidget widgets defined for the main window.
+    #--------------------------------------------------------------------------
+    # Utility Methods
+    #--------------------------------------------------------------------------
+    def dock_items(self):
+        """ Get an iterable of QDockItem children for this area.
 
         """
-        for d in self.declaration.dock_panes():
+        for d in self.declaration.dock_items():
             w = d.proxy.widget
             if w is not None:
                 yield w
 
-    def status_bar(self):
-        """ Get the status bar widget defined for the main window.
+    #--------------------------------------------------------------------------
+    # Child Events
+    #--------------------------------------------------------------------------
+    def child_added(self, child):
+        """ Handle the child added event for a QtDockArea.
 
         """
-        d = self.declaration.status_bar()
-        if d is not None:
-            return d.proxy.widget
+        super(QtDockArea, self).child_added(child)
+        if isinstance(child, QtDockItem):
+            w = child.widget
+            if w is not None:
+                self.manager.add_item(w)
 
-    def tool_bars(self):
-        """ Get the QToolBar widgets defined for the main window.
+    def child_removed(self, child):
+        """ Handle the child removed event for a QtDockArea.
 
         """
-        for d in self.declaration.tool_bars():
-            w = d.proxy.widget
+        super(QtDockArea, self).child_removed(child)
+        if isinstance(child, QtDockItem):
+            w = child.widget
             if w is not None:
-                yield w
+                self.manager.remove_item(w)
 
     #--------------------------------------------------------------------------
-    # Child Events
+    # ProxyDockArea API
     #--------------------------------------------------------------------------
-    def child_added(self, child):
-        """ Handle the child added event for a QtMainWindow.
+    def set_tab_position(self, position):
+        """ Set the default tab position on the underyling widget.
 
         """
-        if isinstance(child, QtMenuBar):
-            self.widget.setMenuBar(self.menu_bar())
-        elif isinstance(child, QtContainer):
-            self.widget.setCentralWidget(self.central_widget())
-        elif isinstance(child, QtDockPane):
-            dock_widget = child.widget
-            self.widget.addDockWidget(dock_widget.dockArea(), dock_widget)
-        elif isinstance(child, QtStatusBar):
-            # FIXME Qt will delete the old status bar
-            self.widget.setStatusBar(self.status_bar())
-        elif isinstance(child, QtToolBar):
-            # There are two hacks involved in adding a tool bar. The
-            # first is the same hack that is perfomed in the layout
-            # method for a floating tool bar. The second is specific
-            # to OSX. On that platform, adding a tool bar to main
-            # window which is already visible but does not have any
-            # current tool bars will cause the main window to be hidden.
-            # This will only occur the *first* time a tool bar is added
-            # to the window. The hack below is workaround which should
-            # be sufficient for most use cases. A bug should really be
-            # filed against Qt for this one, since it's reproducible
-            # outside of Enaml.
-            bar_widget = child.widget
-            floating = bar_widget.isFloating()
-            self.widget.addToolBar(bar_widget.toolBarArea(), bar_widget)
-            if floating:
-                deferredCall(bar_widget.setFloating, True)
-            if sys.platform == 'darwin':
-                self.widget.setVisible(True)
-        else:
-            super(QtMainWindow, self).child_added(child)
+        self.widget.setTabPosition(TAB_POSITIONS[position])
 
-    def child_removed(self, child):
-        """ Handle the child removed event for a QtMainWindow.
+    def set_live_drag(self, live_drag):
+        """ Set the live drag state for the underlying widget.
+
+        """
+        self.widget.setOpaqueItemResize(live_drag)
+
+    def set_style(self, style):
+        """ Set the style for the underlying widget.
 
         """
-        if isinstance(child, QtDockPane) and child.widget is not None:
-            self.widget.removeDockWidget(child.widget)
-        elif isinstance(child, QtToolBar) and child.widget is not None:
-            self.widget.removeToolBar(child.widget)
-        elif isinstance(child, QtContainer):
-            self.widget.setCentralWidget(self.central_widget())
-        elif isinstance(child, QtMenuBar):
-            self.widget.setMenuBar(self.menu_bar())
-        elif isinstance(child, QtStatusBar):
-            # FIXME Qt will delete the old status bar
-            self.widget.setStatusBar(self.status_bar())
+        # If get_style_sheet returns something, it means the user will
+        # have already called register_style_sheet, which will raise
+        # a deprecation warning. TODO remove this method in Enaml 1.0.
+        sheet = get_style_sheet(style)
+        if sheet:
+            self.widget.setStyleSheet(sheet)
+
+    def set_dock_events_enabled(self, enabled):
+        """ Set whether or not dock events are enabled for the area.
+
+        """
+        widget = self.widget
+        widget.setDockEventsEnabled(enabled)
+        if enabled:
+            widget.installEventFilter(self.dock_event_filter)
         else:
-            super(QtMainWindow, self).child_removed(child)
+            widget.removeEventFilter(self.dock_event_filter)
+
+    def save_layout(self):
+        """ Save the current layout on the underlying widget.
+
+        """
+        return self.manager.save_layout()
+
+    def apply_layout(self, layout):
+        """ Apply a new layout to the underlying widget.
+
+        """
+        self.manager.apply_layout(layout)
+
+    def update_layout(self, ops):
+        """ Update the layout from a list of layout operations.
+
+        """
+        self.manager.update_layout(ops)
```

### Comparing `enaml-0.9.7/enaml/qt/qt_spin_box.py` & `enaml-0.9.8/enaml/qt/docking/q_text_label.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,133 +1,124 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from atom.api import Int, Typed
+from enaml.qt.QtCore import Qt, QSize, QEvent
+from enaml.qt.QtGui import QFrame, QPainter
 
-from enaml.widgets.spin_box import ProxySpinBox
 
-from .QtGui import QSpinBox
-
-from .qt_control import QtControl
-
-
-#: Cyclic guard flag
-VALUE_FLAG = 0x1
-
-
-class QtSpinBox(QtControl, ProxySpinBox):
-    """ A Qt implementation of an Enaml SpinBox.
+class QTextLabel(QFrame):
+    """ A custom QFrame which draws elided text.
 
     """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(QSpinBox)
-
-    #: Cyclic guard flags
-    _guard = Int(0)
-
-    #--------------------------------------------------------------------------
-    # Initialization API
-    #--------------------------------------------------------------------------
-    def create_widget(self):
-        """ Create the underlying QSpinBox widget.
-
-        """
-        widget = QSpinBox(self.parent_widget())
-        widget.setKeyboardTracking(False)
-        self.widget = widget
+    def __init__(self, parent=None):
+        """ Initialize a QDockTitleBar.
 
-    def init_widget(self):
-        """ Initialize the underlying widget.
+        Parameters
+        ----------
+        parent : QWidget or None
+            The parent of the title bar.
 
         """
-        super(QtSpinBox, self).init_widget()
-        d = self.declaration
-        self.set_maximum(d.maximum)
-        self.set_minimum(d.minimum)
-        self.set_value(d.value)
-        self.set_prefix(d.prefix)
-        self.set_suffix(d.suffix)
-        self.set_special_value_text(d.special_value_text)
-        self.set_single_step(d.single_step)
-        self.set_read_only(d.read_only)
-        self.set_wrapping(d.wrapping)
-        self.widget.valueChanged.connect(self.on_value_changed)
+        super(QTextLabel, self).__init__(parent)
+        self._min_text_size = QSize()
+        self._text_size = QSize()
+        self._text = u''
 
     #--------------------------------------------------------------------------
-    # Signal Handlers
+    # Private API
     #--------------------------------------------------------------------------
-    def on_value_changed(self):
-        """ The signal handler for the 'valueChanged' signal.
+    @staticmethod
+    def _computeElidedText(text):
+        """ Compute the minimum elided text for the tab title.
 
         """
-        if not self._guard & VALUE_FLAG:
-            self._guard |= VALUE_FLAG
-            try:
-                self.declaration.value = self.widget.value()
-            finally:
-                self._guard &= ~VALUE_FLAG
+        # Based on QTabBar::computeElidedText
+        if len(text) > 3:
+            text = text[:2] + '...'
+        return text
 
     #--------------------------------------------------------------------------
-    # ProxySpinBox API
+    # Public API
     #--------------------------------------------------------------------------
-    def set_maximum(self, maximum):
-        """ Set the widget's maximum value.
-
-        """
-        self.widget.setMaximum(maximum)
+    def text(self):
+        """ Get the text string of the text label.
 
-    def set_minimum(self, minimum):
-        """ Set the widget's minimum value.
+        Returns
+        -------
+        result : unicode
+            The unicode text string for the text label.
 
         """
-        self.widget.setMinimum(minimum)
+        return self._text
 
-    def set_value(self, value):
-        """ Set the spin box's value.
-
-        """
-        if not self._guard & VALUE_FLAG:
-            self._guard |= VALUE_FLAG
-            try:
-                self.widget.setValue(value)
-            finally:
-                self._guard &= ~VALUE_FLAG
+    def setText(self, text):
+        """ Set the text string of the text label.
 
-    def set_prefix(self, prefix):
-        """ Set the prefix for the spin box.
+        Parameters
+        ----------
+        text : unicode
+            The unicode string to use for the text label.
 
         """
-        self.widget.setPrefix(prefix)
+        self._min_text_size = QSize()
+        self._text_size = QSize()
+        self._text = text
+        self.updateGeometry()
+        self.update()
 
-    def set_suffix(self, suffix):
-        """ Set the suffix for the spin box.
-
-        """
-        self.widget.setSuffix(suffix)
+    #--------------------------------------------------------------------------
+    # Reimplementations
+    #--------------------------------------------------------------------------
+    def event(self, event):
+        """ The generic event handler for the text label.
 
-    def set_special_value_text(self, text):
-        """ Set the special value text for the spin box.
+        This handler ensures the size hint caches are invalidated when
+        the widget style changes.
 
         """
-        self.widget.setSpecialValueText(text)
+        if event.type() == QEvent.StyleChange:
+            self._min_text_size = QSize()
+            self._text_size = QSize()
+        return super(QTextLabel, self).event(event)
 
-    def set_single_step(self, step):
-        """ Set the widget's single step value.
+    def sizeHint(self):
+        """ Get the size hint for the text label.
 
         """
-        self.widget.setSingleStep(step)
+        base = self._text_size
+        if not base.isValid():
+            metrics = self.fontMetrics()
+            base = QSize(metrics.width(self._text), metrics.height())
+            self._text_size = base
+        left, top, right, bottom = self.getContentsMargins()
+        return base + QSize(left + right, top + bottom)
 
-    def set_read_only(self, read_only):
-        """ Set the widget's read only flag.
+    def minimumSizeHint(self):
+        """ Get the minimum size hint for the text label.
 
         """
-        self.widget.setReadOnly(read_only)
+        base = self._min_text_size
+        if not base.isValid():
+            metrics = self.fontMetrics()
+            text = self._computeElidedText(self._text)
+            base = QSize(metrics.width(text), metrics.height())
+            self._min_text_size = base
+        left, top, right, bottom = self.getContentsMargins()
+        return base + QSize(left + right, top + bottom)
+
+    def paintEvent(self, event):
+        """ Handle the paint event for the title bar.
 
-    def set_wrapping(self, wrapping):
-        """ Set the widget's wrapping flag.
+        This paint handler draws the title bar text and title buttons.
 
         """
-        self.widget.setWrapping(wrapping)
+        super(QTextLabel, self).paintEvent(event)
+        rect = self.contentsRect()
+        metrics = self.fontMetrics()
+        # The +1 is to fix a seeming off-by-one error in elidedText.
+        # https://github.com/nucleic/enaml/issues/38
+        text = metrics.elidedText(self._text, Qt.ElideRight, rect.width() + 1)
+        QPainter(self).drawText(rect, Qt.AlignLeft | Qt.AlignVCenter, text)
```

### Comparing `enaml-0.9.7/enaml/qt/qt_mdi_window.py` & `enaml-0.9.8/enaml/qt/qt_status_bar.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,133 +3,128 @@
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 from atom.api import Typed
 
-from enaml.widgets.mdi_window import ProxyMdiWindow
+from enaml.widgets.status_bar import ProxyStatusBar
 
-from .QtGui import QMdiSubWindow, QLayout, QIcon
+from .QtGui import QStatusBar
 
-from .q_resource_helpers import get_cached_qicon
+from .qt_status_item import QtStatusItem
 from .qt_widget import QtWidget
 
 
-class QtMdiWindow(QtWidget, ProxyMdiWindow):
-    """ A Qt implementation of an Enaml ProxyMdiWindow.
+class QtStatusBar(QtWidget, ProxyStatusBar):
+    """ A Qt implementation of an Enaml ProxyStatusBar.
 
     """
     #: A reference to the widget created by the proxy.
-    widget = Typed(QMdiSubWindow)
+    widget = Typed(QStatusBar)
 
     #--------------------------------------------------------------------------
     # Initialization API
     #--------------------------------------------------------------------------
     def create_widget(self):
-        """ Create the underlying QMdiSubWindow widget.
+        """ Create the QStatusBar widget.
 
         """
-        # We don't parent the subwindow immediately. It will be added
-        # explicitly by the parent QMdiArea during its layout pass.
-        # If we set the parent here, Qt will spit out warnings when
-        # it's set added to the area later on. We *could* parent it
-        # here, and simply not add it explicitly to the mdi area, but
-        # this way is more explicit and consistent with the rest of
-        # the framework.
-        widget = QMdiSubWindow()
-        widget.layout().setSizeConstraint(QLayout.SetMinAndMaxSize)
-        self.widget = widget
+        self.widget = QStatusBar(self.parent_widget())
 
     def init_widget(self):
         """ Initialize the widget.
 
         """
-        super(QtMdiWindow, self).init_widget()
-        d = self.declaration
-        if d.title:
-            self.set_title(d.title)
-        if d.icon:
-            self.set_icon(d.icon)
+        super(QtStatusBar, self).init_widget()
+        self.set_size_grip_enabled(self.declaration.size_grip_enabled)
 
     def init_layout(self):
-        """ Initialize the layout for the underlying control.
+        """ Initialize the layout for the widget.
 
         """
-        super(QtMdiWindow, self).init_layout()
-        self._set_window_widget(self.mdi_widget())
+        super(QtStatusBar, self).init_layout()
+        widget = self.widget
+        for child in self.children():
+            if isinstance(child, QtStatusItem):
+                s_widget = child.status_widget()
+                if s_widget is not None:
+                    stretch = child.stretch()
+                    if child.is_permanent():
+                        widget.addPermanentWidget(s_widget, stretch)
+                    else:
+                        widget.addWidget(s_widget, stretch)
 
     #--------------------------------------------------------------------------
     # Utility Methods
     #--------------------------------------------------------------------------
-    def mdi_widget(self):
-        """ Find and return the mdi widget child for this widget.
+    def refresh_item(self, item):
+        """ A method invoked by a child status item.
+
+        This method can be called when the widget for the item should
+        be refreshed in the status bar.
 
         """
-        w = self.declaration.mdi_widget()
-        if w:
-            return w.proxy.widget
+        w = self.widget
+        s = item.status_widget()
+        if s is not None:
+            w.removeWidget(s)
+            for index, child in enumerate(self.children()):
+                if child is item:
+                    stretch = item.stretch()
+                    if item.is_permanent():
+                        w.insertPermanentWidget(index, s, stretch)
+                    else:
+                        w.insertWidget(index, s, stretch)
+                    s.show()
+                    break
 
     #--------------------------------------------------------------------------
     # Child Events
     #--------------------------------------------------------------------------
     def child_added(self, child):
-        """ Handle the child added event for a QtMdiWindow.
+        """ Handle the child added event for a QtStatusBar.
 
         """
-        super(QtMdiWindow, self).child_added(child)
-        if isinstance(child, QtWidget):
-            self._set_window_widget(self.mdi_widget())
+        super(QtStatusBar, self).child_added(child)
+        if isinstance(child, QtStatusItem):
+            w = self.widget
+            s = child.status_widget()
+            if s is not None:
+                for index, item in enumerate(self.children()):
+                    if child is item:
+                        stretch = item.stretch()
+                        if item.is_permanent():
+                            w.insertPermanentWidget(index, s, stretch)
+                        else:
+                            w.insertWidget(index, s, stretch)
+                        break
 
     def child_removed(self, child):
-        """ Handle the child removed event for a QtMdiWindow.
+        """ Handle the child removed event for a QtStatusBar.
 
         """
-        super(QtMdiWindow, self).child_added(child)
-        if isinstance(child, QtWidget):
-            self._set_window_widget(self.mdi_widget())
+        if isinstance(child, QtStatusItem):
+            s = child.status_widget()
+            if s is not None:
+                self.widget.removeWidget(s)
 
     #--------------------------------------------------------------------------
-    # ProxyMdiWindow API
+    # ProxyStatusBar API
     #--------------------------------------------------------------------------
-    def set_icon(self, icon):
-        """ Set the mdi window icon.
+    def set_size_grip_enabled(self, enabled):
+        """ Set the size grip enabled on the underlying widget.
 
         """
-        if icon:
-            qicon = get_cached_qicon(icon)
-        else:
-            qicon = QIcon()
-        self.widget.setWindowIcon(qicon)
+        self.widget.setSizeGripEnabled(enabled)
 
-    def set_title(self, title):
-        """ Set the title of the mdi window.
+    def show_message(self, message, timeout=0):
+        """ Show a temporary message in the status bar.
 
         """
-        self.widget.setWindowTitle(title)
-
-    #--------------------------------------------------------------------------
-    # Private API
-    #--------------------------------------------------------------------------
-    def _set_window_widget(self, mdi_widget):
-        """ A private method which set the child widget on the window.
+        self.widget.showMessage(message, timeout)
 
-        Parameters
-        ----------
-        mdi_widget : QWidget
-            The child widget to use in the mdi window.
+    def clear_message(self):
+        """ Clear any temporary message shown in the status bar.
 
         """
-        # We need to first set the window widget to None, or Qt will
-        # complain if a widget is already set on the window.
-        widget = self.widget
-        widget.setWidget(None)
-        if mdi_widget is None:
-            return
-        # We need to unparent the underlying widget before adding
-        # it to the subwindow. Otherwise, children like QMainWindow
-        # will persist as top-level non-mdi widgets.
-        mdi_widget.setParent(None)
-        widget.setWidget(mdi_widget)
-        # On OSX, the resize gripper will be obscured unless we
-        # lower the widget in the window's stacking order.
-        mdi_widget.lower()
+        self.widget.clearMessage()
```

### Comparing `enaml-0.9.7/enaml/qt/qt_stack_item.py` & `enaml-0.9.8/enaml/qt/qt_stack_item.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_slider.py` & `enaml-0.9.8/enaml/qt/qt_slider.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/q_pixmap_transition.py` & `enaml-0.9.8/enaml/qt/q_pixmap_transition.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_application.py` & `enaml-0.9.8/enaml/qt/q_deferred_caller.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,73 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from atom.api import Typed
+from .QtCore import QObject, QTimer, QEvent, QThread
+from .QtGui import QApplication
 
-from enaml.application import Application, ProxyResolver
 
-from .QtCore import QThread
-from .QtGui import QApplication
+class DeferredCallEvent(QEvent):
+    """ A custom event type for deferred call events.
 
-from .q_deferred_caller import deferredCall, timedCall
-from .qt_factories import QT_FACTORIES
+    """
+    # Explicitly coerce to QEvent.Type for PySide compatibility.
+    Type = QEvent.Type(QEvent.registerEventType())
 
+    def __init__(self, callback, args, kwargs):
+        super(DeferredCallEvent, self).__init__(self.Type)
+        self.callback = callback
+        self.args = args
+        self.kwargs = kwargs
 
-class QtApplication(Application):
-    """ A Qt implementation of an Enaml application.
 
-    A QtApplication uses the Qt toolkit to implement an Enaml UI that
-    runs in the local process.
+class DeferredCaller(QObject):
+    """ A QObject subclass which handles deferred call events.
 
     """
-    #: The private QApplication instance.
-    _qapp = Typed(QApplication)
-
     def __init__(self):
-        """ Initialize a QtApplication.
+        """ Initialize a DeferredCaller.
 
         """
-        super(QtApplication, self).__init__()
-        self._qapp = QApplication.instance() or QApplication([])
-        self.resolver = ProxyResolver(factories=QT_FACTORIES)
-
-    #--------------------------------------------------------------------------
-    # Abstract API Implementation
-    #--------------------------------------------------------------------------
-    def start(self):
-        """ Start the application's main event loop.
+        super(DeferredCaller, self).__init__()
+        self.moveToThread(QApplication.instance().thread())
+
+    def customEvent(self, event):
+        """ Handle the custom deferred call events.
 
         """
-        app = self._qapp
-        if not getattr(app, '_in_event_loop', False):
-            app._in_event_loop = True
-            app.exec_()
-            app._in_event_loop = False
+        if event.type() == DeferredCallEvent.Type:
+            event.callback(*event.args, **event.kwargs)
 
-    def stop(self):
-        """ Stop the application's main event loop.
 
-        """
-        app = self._qapp
-        app.exit()
-        app._in_event_loop = False
-
-    def deferred_call(self, callback, *args, **kwargs):
-        """ Invoke a callable on the next cycle of the main event loop
-        thread.
-
-        Parameters
-        ----------
-        callback : callable
-            The callable object to execute at some point in the future.
-
-        *args, **kwargs
-            Any additional positional and keyword arguments to pass to
-            the callback.
+#: A globally available caller instance. This will be created on demand
+#: by the globally available caller functions.
+__caller = None
 
-        """
-        deferredCall(callback, *args, **kwargs)
 
-    def timed_call(self, ms, callback, *args, **kwargs):
-        """ Invoke a callable on the main event loop thread at a
-        specified time in the future.
-
-        Parameters
-        ----------
-        ms : int
-            The time to delay, in milliseconds, before executing the
-            callable.
-
-        callback : callable
-            The callable object to execute at some point in the future.
-
-        *args, **kwargs
-            Any additional positional and keyword arguments to pass to
-            the callback.
+def deferredCall(callback, *args, **kwargs):
+    """ Execute the callback on the main gui thread.
 
-        """
-        timedCall(ms, callback, *args, **kwargs)
+    This should only be called after the QApplication is created.
 
-    def is_main_thread(self):
-        """ Indicates whether the caller is on the main gui thread.
+    """
+    global __caller
+    caller = __caller
+    if caller is None:
+        caller = __caller = DeferredCaller()
+    event = DeferredCallEvent(callback, args, kwargs)
+    QApplication.postEvent(caller, event)
 
-        Returns
-        -------
-        result : bool
-            True if called from the main gui thread. False otherwise.
 
-        """
-        return QThread.currentThread() == self._qapp.thread()
+def timedCall(ms, callback, *args, **kwargs):
+    """ Execute a callback on a timer in the main gui thread.
+
+    This should only be called after the QApplication is created.
+
+    """
+    if QThread.currentThread() != QApplication.instance().thread():
+        deferredCall(timedCall, ms, callback, *args, **kwargs)
+    else:
+        QTimer.singleShot(ms, lambda: callback(*args, **kwargs))
```

### Comparing `enaml-0.9.7/enaml/qt/qt_action.py` & `enaml-0.9.8/enaml/qt/qt_action.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_dual_slider.py` & `enaml-0.9.8/enaml/qt/qt_dual_slider.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/q_window_base.py` & `enaml-0.9.8/enaml/qt/q_window_base.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_separator.py` & `enaml-0.9.8/enaml/qt/qt_separator.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_file_dialog_ex.py` & `enaml-0.9.8/enaml/qt/qt_file_dialog_ex.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_push_button.py` & `enaml-0.9.8/enaml/qt/qt_push_button.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_bounded_datetime.py` & `enaml-0.9.8/enaml/qt/qt_bounded_datetime.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_toolkit_dialog.py` & `enaml-0.9.8/enaml/qt/qt_toolkit_dialog.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/QtCore.py` & `enaml-0.9.8/enaml/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_menu_bar.py` & `enaml-0.9.8/enaml/qt/qt_menu_bar.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_scintilla.py` & `enaml-0.9.8/enaml/qt/qt_scintilla.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_split_item.py` & `enaml-0.9.8/enaml/qt/qt_split_item.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_time_selector.py` & `enaml-0.9.8/enaml/qt/docking/q_icon_widget.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,106 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from atom.api import Typed
+from enaml.qt.QtCore import QSize
+from enaml.qt.QtGui import QFrame, QIcon, QPainter
 
-from enaml.widgets.time_selector import ProxyTimeSelector
 
-from .QtGui import QTimeEdit
-
-from .qt_bounded_time import QtBoundedTime, CHANGED_GUARD
-
-
-class QtTimeSelector(QtBoundedTime, ProxyTimeSelector):
-    """ A Qt implementation of an Enaml ProxyTimeSelector.
+class QIconWidget(QFrame):
+    """ A custom QFrame which paints an icon.
 
     """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(QTimeEdit)
-
-    #--------------------------------------------------------------------------
-    # Initialization API
-    #--------------------------------------------------------------------------
-    def create_widget(self):
-        """ Create the QTimeEdit widget.
+    def __init__(self, parent=None):
+        """ Initialize a QIconWidget.
 
-        """
-        self.widget = QTimeEdit(self.parent_widget())
-
-    def init_widget(self):
-        """ Initialize the widget.
+        Parameters
+        ----------
+        parent : QWidget, optional
+            The parent of the icon widget.
 
         """
-        super(QtTimeSelector, self).init_widget()
-        d = self.declaration
-        self.set_time_format(d.time_format)
-        self.widget.timeChanged.connect(self.on_time_changed)
+        super(QIconWidget, self).__init__(parent)
+        self._icon_size = QSize()
+        self._icon = QIcon()
 
     #--------------------------------------------------------------------------
-    # Abstract API Implementation
+    # Public API
     #--------------------------------------------------------------------------
-    def get_time(self):
-        """ Return the current time in the control.
+    def icon(self):
+        """ Get the icon for the widget.
 
         Returns
         -------
-        result : time
-            The current control time as a time object.
+        result : QIcon
+            The icon installed on the widget.
 
         """
-        return self.widget.time().toPython()
+        return self._icon
 
-    def set_minimum(self, time):
-        """ Set the widget's minimum time.
+    def setIcon(self, icon):
+        """ Set the icon for the widget.
 
         Parameters
         ----------
-        time : time
-            The time object to use for setting the minimum time.
+        icon : QIcon
+            The icon to use for the widget.
 
         """
-        self.widget.setMinimumTime(time)
+        self._icon = icon
+        self.update()
 
-    def set_maximum(self, time):
-        """ Set the widget's maximum time.
+    def iconSize(self):
+        """ Get the icon size for the widget.
 
-        Parameters
-        ----------
-        time : time
-            The time object to use for setting the maximum time.
+        Returns
+        -------
+        result : QSize
+            The size to use for displaying the icon.
 
         """
-        self.widget.setMaximumTime(time)
+        return self._icon_size
 
-    def set_time(self, time):
-        """ Set the widget's current time.
+    def setIconSize(self, size):
+        """ Set the icon size for the widget.
 
         Parameters
         ----------
-        time : time
-            The time object to use for setting the date.
+        size : QSize
+            The icon size to use for the widget.
 
         """
-        self._guard |= CHANGED_GUARD
-        try:
-            self.widget.setTime(time)
-        finally:
-            self._guard &= ~CHANGED_GUARD
+        self._icon_size = size
+        self.updateGeometry()
+        self.update()
 
-    def set_time_format(self, format):
-        """ Set the widget's time format.
+    #--------------------------------------------------------------------------
+    # Reimplementations
+    #--------------------------------------------------------------------------
+    def sizeHint(self):
+        """ Get the size hint for the widget.
 
-        Parameters
-        ----------
-        format : string
-            A Python time formatting string.
+        """
+        return self.minimumSizeHint()
+
+    def minimumSizeHint(self):
+        """ Get the minimum size hint for the widget.
+
+        """
+        size = self._icon_size
+        if not size.isValid():
+            size = QSize(16, 16)
+        left, top, right, bottom = self.getContentsMargins()
+        return size + QSize(left + right, top + bottom)
+
+    def paintEvent(self, event):
+        """ Handle the paint event for the widget.
 
         """
-        # XXX make sure Python's and Qt's format strings are the
-        # same, or convert between the two.
-        self.widget.setDisplayFormat(format)
+        super(QIconWidget, self).paintEvent(event)
+        icon = self._icon
+        if icon.isNull():
+            return
+        icon.paint(QPainter(self), self.contentsRect())
```

### Comparing `enaml-0.9.7/enaml/qt/qt_check_box.py` & `enaml-0.9.8/enaml/qt/qt_check_box.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_file_dialog.py` & `enaml-0.9.8/enaml/qt/qt_file_dialog.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_radio_button.py` & `enaml-0.9.8/enaml/qt/qt_radio_button.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_mdi_area.py` & `enaml-0.9.8/enaml/qt/qt_mdi_area.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_dock_area.py` & `enaml-0.9.8/enaml/qt/qt_flow_item.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,279 +3,304 @@
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 from atom.api import Typed
 
-from enaml.styling import StyleCache
-from enaml.widgets.dock_area import ProxyDockArea
-from enaml.widgets.dock_events import DockItemEvent
-
-from .QtCore import QObject, QEvent, QSize, QTimer
-from .QtGui import QTabWidget
-
-from .docking.dock_manager import DockManager
-from .docking.event_types import (
-    DockItemDocked, DockItemUndocked, DockItemExtended, DockItemRetracted,
-    DockItemShown, DockItemHidden, DockItemClosed, DockTabSelected
-)
-from .docking.q_dock_area import QDockArea
-from .docking.style_sheets import get_style_sheet
-
-from .qt_constraints_widget import QtConstraintsWidget
-from .qt_dock_item import QtDockItem
-from .styleutil import translate_dock_area_style
-
-
-TAB_POSITIONS = {
-    'top': QTabWidget.North,
-    'bottom': QTabWidget.South,
-    'left': QTabWidget.West,
-    'right': QTabWidget.East,
-}
+from enaml.widgets.flow_item import ProxyFlowItem
 
+from .QtCore import QSize, QEvent
+from .QtGui import QFrame, QLayout
 
-EVENT_TYPES = {
-    DockItemDocked: DockItemEvent.Docked,
-    DockItemUndocked: DockItemEvent.Undocked,
-    DockItemExtended: DockItemEvent.Extended,
-    DockItemRetracted: DockItemEvent.Retracted,
-    DockItemShown: DockItemEvent.Shown,
-    DockItemHidden: DockItemEvent.Hidden,
-    DockItemClosed: DockItemEvent.Closed,
-    DockTabSelected: DockItemEvent.TabSelected,
-}
+from .q_flow_layout import QFlowLayout, AbstractFlowWidget, FlowLayoutData
+from .q_single_widget_layout import QSingleWidgetLayout
+from .qt_container import QtContainer
+from .qt_widget import QtWidget
 
 
-class DockLayoutFilter(QObject):
-    """ An event filter used by the QtDockArea.
+_ALIGN_MAP = {
+    'leading': QFlowLayout.AlignLeading,
+    'trailing': QFlowLayout.AlignTrailing,
+    'center': QFlowLayout.AlignCenter,
+}
 
-    This event filter listens for LayoutRequest events on the dock
-    area widget, and will send a geometry_updated notification to
-    the constraints system when the dock area size hint changes. The
-    notifications are collapsed on a single shot timer so that the
-    dock area geometry can fully settle before being snapped by the
-    constraints layout engine.
 
-    """
-    def __init__(self, owner):
-        super(DockLayoutFilter, self).__init__()
-        self._owner = owner
-        self._size_hint = QSize()
-        self._pending = False
-        self._timer = timer = QTimer()
-        timer.setSingleShot(True)
-        timer.timeout.connect(self.onNotify)
-
-    def onNotify(self):
-        self._owner.geometry_updated()
-        self._pending = False
-
-    def eventFilter(self, obj, event):
-        if not self._pending and event.type() == QEvent.LayoutRequest:
-            hint = obj.sizeHint()
-            if hint != self._size_hint:
-                self._size_hint = hint
-                self._timer.start(0)
-                self._pending = True
-        return False
-
-
-class DockEventFilter(QObject):
-    """ An event filter used by the QtDockArea.
-
-    This event filter listens for dock events on the dock area widget,
-    converts them to front-end events, and posts them to the front-end
-    declaration object.
+class QFlowItem(QFrame):
+    """ A QFrame subclass which acts as an item in a QFlowArea.
 
     """
-    def __init__(self, owner):
-        super(DockEventFilter, self).__init__()
-        self._owner = owner
-
-    def eventFilter(self, obj, event):
-        e_type = EVENT_TYPES.get(event.type())
-        if e_type is not None:
-            d = self._owner.declaration
-            if d is not None:
-                d.dock_event(DockItemEvent(type=e_type, name=event.name()))
-        return False
+    def __init__(self, parent=None):
+        """ Initialize a QFlowItem.
 
+        Parameters
+        ----------
+        parent : QWidget, optional
+            The parent of the flow item.
 
-class QtDockArea(QtConstraintsWidget, ProxyDockArea):
-    """ A Qt implementation of an Enaml DockArea.
+        """
+        super(QFlowItem, self).__init__(parent)
+        self._flow_widget = None
+        self._layout_data = FlowLayoutData()
+        self.setLayout(QSingleWidgetLayout())
+        self.layout().setSizeConstraint(QLayout.SetMinAndMaxSize)
 
-    """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(QDockArea)
+    def layoutData(self):
+        """ Get the layout data associate with this flow item.
 
-    #: The docking manager which will drive the dock area.
-    manager = Typed(DockManager)
+        This method implements the AbstractFlowWidget interface.
 
-    #: The event filter which listens for layout requests.
-    dock_layout_filter = Typed(DockLayoutFilter)
+        Returns
+        -------
+        result : FlowLayoutData
+            The layout data for this flow item.
 
-    #: The event filter which listens for dock events.
-    dock_event_filter = Typed(DockEventFilter)
+        """
+        return self._layout_data
 
-    #--------------------------------------------------------------------------
-    # Initialization API
-    #--------------------------------------------------------------------------
-    def create_widget(self):
-        """ Create the underlying QDockArea widget.
+    def preferredSize(self):
+        """ Get the preferred size for this widget.
+
+        Returns
+        -------
+        result : QSize
+            The preferred size of this flow item.
 
         """
-        self.widget = QDockArea(self.parent_widget())
-        self.manager = DockManager(self.widget)
-        self.dock_event_filter = DockEventFilter(self)
-        self.dock_layout_filter = DockLayoutFilter(self)
+        return self._layout_data.preferred_size
 
-    def init_widget(self):
-        """ Initialize the underlying widget.
+    def setPreferredSize(self, size):
+        """ Set the preferred size for this flow item.
+
+        This will trigger an invalidation of the layout data.
+
+        Parameters
+        ----------
+        size : QSize
+            The preferred size for the flow item.
 
         """
-        super(QtDockArea, self).init_widget()
-        d = self.declaration
-        self.set_tab_position(d.tab_position)
-        self.set_live_drag(d.live_drag)
-        if d.style:  # TODO remove this in Enaml 1.0
-            self.set_style(d.style)
-        self.set_dock_events_enabled(d.dock_events_enabled)
+        d = self._layout_data
+        d.preferred_size = size
+        d.dirty = True
+        self.updateGeometry()
 
-    def init_layout(self):
-        """ Initialize the layout of the underlying control.
+    def alignment(self):
+        """ Get the alignment for the flow item.
+
+        Returns
+        -------
+        result : QFlowLayout alignment
+            The alignment for the flow item in the layout.
 
         """
-        super(QtDockArea, self).init_layout()
-        manager = self.manager
-        for item in self.dock_items():
-            manager.add_item(item)
-        d = self.declaration
-        self.apply_layout(d.layout)
-        self.widget.installEventFilter(self.dock_layout_filter)
+        return self._layout_data.alignment
+
+    def setAlignment(self, alignment):
+        """ Set the alignment for the flot item.
 
-    def destroy(self):
-        """ A reimplemented destructor.
+        This will trigger an invalidation of the layout data.
 
-        This removes the event filter from the dock area and releases
-        the items from the dock manager.
+        Parameters
+        ----------
+        alignment : QFlowLayout alignment
+            The alignment for the flow item in the layout.
 
         """
-        self.widget.removeEventFilter(self.dock_layout_filter)
-        self.widget.removeEventFilter(self.dock_event_filter)
-        del self.dock_layout_filter
-        del self.dock_event_filter
-        self.manager.destroy()
-        super(QtDockArea, self).destroy()
+        d = self._layout_data
+        d.alignment = alignment
+        d.dirty = True
+        self.updateGeometry()
 
-    #--------------------------------------------------------------------------
-    # Overrides
-    #--------------------------------------------------------------------------
-    def refresh_style_sheet(self):
-        """ A reimplemented styling method.
+    def stretch(self):
+        """ Get the stretch factor for the flow item.
 
-        The dock area uses custom stylesheet processing.
+        Returns
+        -------
+        result : int
+            The stretch factor for the flow item in the direction of
+            the layout flow.
 
         """
-        # workaround win-7 sizing bug
-        parts = [u'QDockTabWidget::pane {}']
-        name = self.widget.objectName()
-        for style in StyleCache.styles(self.declaration):
-            t = translate_dock_area_style(name, style)
-            if t:
-                parts.append(t)
-        if len(parts) > 1:
-            stylesheet = u'\n\n'.join(parts)
-        else:
-            stylesheet = u''
-        self.widget.setStyleSheet(stylesheet)
+        return self._layout_data.stretch
 
-    #--------------------------------------------------------------------------
-    # Utility Methods
-    #--------------------------------------------------------------------------
-    def dock_items(self):
-        """ Get an iterable of QDockItem children for this area.
+    def setStretch(self, stretch):
+        """ Set the stretch factor for the flow item.
+
+        This will trigger an invalidation of the layout data.
+
+        Parameters
+        ----------
+        stretch : int
+            The stretch factor for the flow item in the direction of
+            the layout flow.
+
+        """
+        d = self._layout_data
+        d.stretch = stretch
+        d.dirty = True
+        self.updateGeometry()
+
+    def orthoStretch(self):
+        """ Get the ortho stretch factor for the flow item.
+
+        Returns
+        -------
+        result : int
+            The stretch factor for the flow item in the direction
+            orthogonal to the layout flow.
+
+        """
+        return self._layout_data.stretch
+
+    def setOrthoStretch(self, stretch):
+        """ Set the ortho stretch factor for the flow item.
+
+        This will trigger an invalidation of the layout data.
+
+        Parameters
+        ----------
+        stretch : int
+            The stretch factor for the flow item in the direction
+            orthogonal to the layout flow.
+
+        """
+        d = self._layout_data
+        d.ortho_stretch = stretch
+        d.dirty = True
+        self.updateGeometry()
+
+    def flowWidget(self):
+        """ Get the flow widget for this flow item.
+
+        Returns
+        -------
+        result : QWidget or None
+            The flow widget being managed by this item.
+
+        """
+        return self._flow_widget
+
+    def setFlowWidget(self, widget):
+        """ Set the flow widget for this flow item.
+
+        Parameters
+        ----------
+        widget : QWidget
+            The QWidget to use as the flow widget in this item.
 
         """
-        for d in self.declaration.dock_items():
-            w = d.proxy.widget
-            if w is not None:
-                yield w
+        self._flow_widget = widget
+        self.layout().setWidget(widget)
+
+    def event(self, event):
+        """ A custom event handler which handles LayoutRequest events.
+
+        When a LayoutRequest event is posted to this widget, it will
+        emit the `layoutRequested` signal. This allows an external
+        consumer of this widget to update their external layout.
+
+        """
+        if event.type() == QEvent.LayoutRequest:
+            self._layout_data.dirty = True
+        return super(QFlowItem, self).event(event)
+
+
+AbstractFlowWidget.register(QFlowItem)
+
+
+class QtFlowItem(QtWidget, ProxyFlowItem):
+    """ A Qt implementation of an Enaml ProxyFlowItem.
+
+    """
+    #: A reference to the widget created by the proxy.
+    widget = Typed(QFlowItem)
 
     #--------------------------------------------------------------------------
-    # Child Events
+    # Initialization API
     #--------------------------------------------------------------------------
-    def child_added(self, child):
-        """ Handle the child added event for a QtDockArea.
+    def create_widget(self):
+        """ Create the underlying QFlowItem widget.
 
         """
-        super(QtDockArea, self).child_added(child)
-        if isinstance(child, QtDockItem):
-            w = child.widget
-            if w is not None:
-                self.manager.add_item(w)
+        self.widget = QFlowItem(self.parent_widget())
 
-    def child_removed(self, child):
-        """ Handle the child removed event for a QtDockArea.
+    def init_widget(self):
+        """ Iitialize the underlying control.
+
+        """
+        super(QtFlowItem, self).init_widget()
+        d = self.declaration
+        self.set_preferred_size(d.preferred_size)
+        self.set_align(d.align)
+        self.set_stretch(d.stretch)
+        self.set_ortho_stretch(d.ortho_stretch)
+
+    def init_layout(self):
+        """ Initialize the layout for the underyling widget.
 
         """
-        super(QtDockArea, self).child_removed(child)
-        if isinstance(child, QtDockItem):
-            w = child.widget
-            if w is not None:
-                self.manager.remove_item(w)
+        super(QtFlowItem, self).init_layout()
+        self.widget.setFlowWidget(self.flow_widget())
 
     #--------------------------------------------------------------------------
-    # ProxyDockArea API
+    # Utility Methods
     #--------------------------------------------------------------------------
-    def set_tab_position(self, position):
-        """ Set the default tab position on the underyling widget.
+    def flow_widget(self):
+        """ Find and return the flow widget child for this widget.
+
+        Returns
+        -------
+        result : QWidget or None
+            The flow widget defined for this widget, or None if one is
+            not defined.
 
         """
-        self.widget.setTabPosition(TAB_POSITIONS[position])
+        d = self.declaration.flow_widget()
+        if d is not None:
+            return d.proxy.widget
 
-    def set_live_drag(self, live_drag):
-        """ Set the live drag state for the underlying widget.
+    #--------------------------------------------------------------------------
+    # Child Events
+    #--------------------------------------------------------------------------
+    def child_added(self, child):
+        """ Handle the child added event for a QtFlowItem.
 
         """
-        self.widget.setOpaqueItemResize(live_drag)
+        super(QtFlowItem, self).child_added(child)
+        if isinstance(child, QtContainer):
+            self.widget.setFlowWidget(self.flow_widget())
 
-    def set_style(self, style):
-        """ Set the style for the underlying widget.
+    def child_removed(self, child):
+        """ Handle the child added event for a QtFlowItem.
 
         """
-        # If get_style_sheet returns something, it means the user will
-        # have already called register_style_sheet, which will raise
-        # a deprecation warning. TODO remove this method in Enaml 1.0.
-        sheet = get_style_sheet(style)
-        if sheet:
-            self.widget.setStyleSheet(sheet)
+        super(QtFlowItem, self).child_removed(child)
+        if isinstance(child, QtContainer):
+            self.widget.setFlowWidget(self.flow_widget())
 
-    def set_dock_events_enabled(self, enabled):
-        """ Set whether or not dock events are enabled for the area.
+    #--------------------------------------------------------------------------
+    # ProxyFlowItem API
+    #--------------------------------------------------------------------------
+    def set_preferred_size(self, size):
+        """ Set the preferred size of the underlying widget.
 
         """
-        widget = self.widget
-        widget.setDockEventsEnabled(enabled)
-        if enabled:
-            widget.installEventFilter(self.dock_event_filter)
-        else:
-            widget.removeEventFilter(self.dock_event_filter)
+        self.widget.setPreferredSize(QSize(*size))
 
-    def save_layout(self):
-        """ Save the current layout on the underlying widget.
+    def set_align(self, align):
+        """ Set the alignment of the underlying widget.
 
         """
-        return self.manager.save_layout()
+        self.widget.setAlignment(_ALIGN_MAP[align])
 
-    def apply_layout(self, layout):
-        """ Apply a new layout to the underlying widget.
+    def set_stretch(self, stretch):
+        """ Set the stretch factor of the underlying widget.
 
         """
-        self.manager.apply_layout(layout)
+        self.widget.setStretch(stretch)
 
-    def update_layout(self, ops):
-        """ Update the layout from a list of layout operations.
+    def set_ortho_stretch(self, stretch):
+        """ Set the ortho stretch factor of the underling widget.
 
         """
-        self.manager.update_layout(ops)
+        self.widget.setOrthoStretch(stretch)
```

### Comparing `enaml-0.9.7/enaml/qt/__init__.py` & `enaml-0.9.8/enaml/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_color_dialog.py` & `enaml-0.9.8/enaml/qt/qt_color_dialog.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_progress_bar.py` & `enaml-0.9.8/enaml/qt/qt_status_item.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,94 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from atom.api import Typed
+from atom.api import Constant
 
-from enaml.widgets.progress_bar import ProxyProgressBar
+from enaml.widgets.status_item import ProxyStatusItem
 
-from .QtGui import QProgressBar
+from .qt_toolkit_object import QtToolkitObject
 
-from .qt_control import QtControl
 
-
-class QtProgressBar(QtControl, ProxyProgressBar):
-    """ A Qt implementation of an Enaml ProxyProgressBar.
+class QtStatusItem(QtToolkitObject, ProxyStatusItem):
+    """ A Qt implementation of an Enaml ProxyStatusItem.
 
     """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(QProgressBar)
+    #: The status has no widget representation. All child widgets will
+    #: be reparented by the status bar during the layout pass.
+    widget = Constant(None)
+
+    def create_widget(self):
+        """ A reimplemented parent class method.
+
+        """
+        pass
+
+    def destroy(self):
+        """ A reimplemented parent class destructor.
+
+        """
+        del self.declaration
 
     #--------------------------------------------------------------------------
-    # Initialization API
+    # Utility Methods
     #--------------------------------------------------------------------------
-    def create_widget(self):
-        """ Create the underlying progress bar widget.
+    def status_widget(self):
+        """ Get the status widget defined for this item.
 
         """
-        self.widget = QProgressBar(self.parent_widget())
+        d = self.declaration.status_widget()
+        if d is not None:
+            return d.proxy.widget
 
-    def init_widget(self):
-        """ Create and initialize the underlying widget.
+    def is_permanent(self):
+        """ Get whether this status item should be permanent.
 
         """
-        super(QtProgressBar, self).init_widget()
-        d = self.declaration
-        self.set_minimum(d.minimum)
-        self.set_maximum(d.maximum)
-        self.set_value(d.value)
-        self.set_text_visible(d.text_visible)
+        return self.declaration.mode == 'permanent'
+
+    def stretch(self):
+        """ Get the stretch factor to apply to the item.
+
+        """
+        return self.declaration.stretch
 
     #--------------------------------------------------------------------------
-    # ProxyProgressBar API
+    # Child Events
     #--------------------------------------------------------------------------
-    def set_minimum(self, value):
-        """ Set the minimum value of the widget.
+    def child_added(self, child):
+        """ Handle the child added event for the status item.
 
         """
-        self.widget.setMinimum(value)
+        parent = self.parent()
+        if parent is not None:
+            parent.refresh_item(self)
 
-    def set_maximum(self, value):
-        """ Set the maximum value of the widget.
+    def child_removed(self, child):
+        """ Handle the child removed event for the status item.
 
         """
-        self.widget.setMaximum(value)
+        parent = self.parent()
+        if parent is not None:
+            parent.refresh_item(self)
 
-    def set_value(self, value):
-        """ Set the value of the widget.
+    #--------------------------------------------------------------------------
+    # ProxyStatusItem API
+    #--------------------------------------------------------------------------
+    def set_mode(self, mode):
+        """ Set the mode of the status item.
 
         """
-        self.widget.setValue(value)
+        parent = self.parent()
+        if parent is not None:
+            parent.refresh_item(self)
 
-    def set_text_visible(self, visible):
-        """ Set the text visibility on the widget.
+    def set_stretch(self, stretch):
+        """ Set the stretch factor of the status item.
 
         """
-        self.widget.setTextVisible(visible)
+        parent = self.parent()
+        if parent is not None:
+            parent.refresh_item(self)
```

### Comparing `enaml-0.9.7/enaml/qt/q_single_widget_layout.py` & `enaml-0.9.8/enaml/qt/q_single_widget_layout.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_toolkit_object.py` & `enaml-0.9.8/enaml/qt/qt_toolkit_object.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_raw_widget.py` & `enaml-0.9.8/enaml/qt/qt_raw_widget.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/scintilla_lexers.py` & `enaml-0.9.8/enaml/qt/scintilla_lexers.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/scintilla_tokens.py` & `enaml-0.9.8/enaml/qt/scintilla_tokens.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_action_group.py` & `enaml-0.9.8/enaml/qt/qt_action_group.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/q_popup_view.py` & `enaml-0.9.8/enaml/qt/q_popup_view.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_vtk_canvas.py` & `enaml-0.9.8/enaml/qt/qt_vtk_canvas.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_field.py` & `enaml-0.9.8/enaml/qt/qt_field.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/q_pixmap_painter.py` & `enaml-0.9.8/enaml/qt/q_pixmap_painter.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/focus_registry.py` & `enaml-0.9.8/enaml/qt/focus_registry.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_factories.py` & `enaml-0.9.8/enaml/qt/qt_factories.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/styleutil.py` & `enaml-0.9.8/enaml/qt/styleutil.py`

 * *Files 8% similar despite different names*

```diff
@@ -191,21 +191,26 @@
     else:
         root = u'QDockBarItem QDockBarItemHandle'
     return _basic_pc(root, u':'.join(rest))
 
 
 def _dock_container(name, pc):
     rest = []
+    tabbed = False
     floating = False
     for part in pc.split(u':'):
-        if part == 'floating':
+        if part == 'tabbed':
+            tabbed = True
+        elif part == 'floating':
             floating = True
         else:
             rest.append(part)
-    if floating:
+    if tabbed:
+        root = u'QDockTabWidget QDockContainer'
+    elif floating:
         root = u'QDockContainer[floating="true"]'
     else:
         root = u'QDockContainer'
     return _maybe_alert(root, name, u':'.join(rest))
 
 
 def _dock_window(name, pc):
@@ -275,15 +280,31 @@
             rest.append(part)
     if alert:
         root = u'%s[alert="%s"]' % (root, alert)
     return _basic_pc(root, u':'.join(rest))
 
 
 def _base_dock_item(name, pc):
-    return _maybe_alert(u'QDockItem', name, pc)
+    rest = []
+    tabbed = False
+    floating = False
+    for part in pc.split(u':'):
+        if part == 'tabbed':
+            tabbed = True
+        elif part == 'floating':
+            floating = True
+        else:
+            rest.append(part)
+    if tabbed:
+        root = u'QDockTabWidget QDockItem'
+    elif floating:
+        root = u'QDockContainer[floating="true"] QDockItem'
+    else:
+        root = u'QDockItem'
+    return _maybe_alert(root, name, u':'.join(rest))
 
 
 def _title_bar(name, pc):
     return _maybe_alert(u'QDockTitleBar', name, pc)
 
 
 def _title_bar_label(name, pc):
```

### Comparing `enaml-0.9.7/enaml/qt/docking/layout_saver.py` & `enaml-0.9.8/enaml/qt/docking/layout_saver.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/q_dock_bar.py` & `enaml-0.9.8/enaml/qt/docking/q_dock_bar.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/enaml_dock_resources.qrc` & `enaml-0.9.8/enaml/qt/docking/enaml_dock_resources.qrc`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/q_dock_splitter.py` & `enaml-0.9.8/enaml/qt/docking/q_dock_splitter.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/event_types.py` & `enaml-0.9.8/enaml/qt/docking/event_types.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/q_bitmap_button.py` & `enaml-0.9.8/enaml/qt/docking/q_bitmap_button.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/q_dock_container.py` & `enaml-0.9.8/enaml/qt/docking/q_dock_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,14 +449,15 @@
         self.setParent(self.manager().dock_area(), flags)
         self.layout().setContentsMargins(QMargins(5, 5, 5, 5))
         self.setProperty('floating', True)
         self.setLinked(False)
         self.showLinkButton()
         self.hidePinButton()
         repolish(self)
+        repolish(self.dockItem())
         self.topLevelChanged.emit(True)
 
     def unfloat(self):
         """ Set the window state to be non-floating window.
 
         """
         self.hide()
@@ -465,14 +466,15 @@
         self.layout().setContentsMargins(QMargins(0, 0, 0, 0))
         self.unsetCursor()
         self.setProperty('floating', False)
         self.setLinked(False)
         self.hideLinkButton()
         self.showPinButton()
         repolish(self)
+        repolish(self.dockItem())
         self.topLevelChanged.emit(False)
 
     def parentDockArea(self):
         """ Get the parent dock area of the container.
 
         Returns
         -------
```

### Comparing `enaml-0.9.7/enaml/qt/docking/q_icon_widget.py` & `enaml-0.9.8/enaml/mime_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,88 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2013, Nucleic Development Team.
+# Copyright (c) 2014, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from enaml.qt.QtCore import QSize
-from enaml.qt.QtGui import QFrame, QIcon, QPainter
+from atom.api import Atom
 
 
-class QIconWidget(QFrame):
-    """ A custom QFrame which paints an icon.
+class MimeData(Atom):
+    """ An abstract class for defining mime data.
 
-    """
-    def __init__(self, parent=None):
-        """ Initialize a QIconWidget.
+    Concrete implementations of this class will be created by a
+    toolkit backend and passed to the relevant frontend methods.
 
-        Parameters
-        ----------
-        parent : QWidget, optional
-            The parent of the icon widget.
+    This will never be instantiated directly by user code. A concrete
+    version can be created by calling the `create_mime_data` factory
+    method of an Application instance.
 
-        """
-        super(QIconWidget, self).__init__(parent)
-        self._icon_size = QSize()
-        self._icon = QIcon()
-
-    #--------------------------------------------------------------------------
-    # Public API
-    #--------------------------------------------------------------------------
-    def icon(self):
-        """ Get the icon for the widget.
+    """
+    def formats(self):
+        """ Get a list of the supported mime type formats.
 
         Returns
         -------
-        result : QIcon
-            The icon installed on the widget.
+        result : list
+            A list of mime types supported by the data.
 
         """
-        return self._icon
+        raise NotImplementedError
 
-    def setIcon(self, icon):
-        """ Set the icon for the widget.
+    def has_format(self, mime_type):
+        """ Test whether the data supports the given mime type.
 
         Parameters
         ----------
-        icon : QIcon
-            The icon to use for the widget.
-
-        """
-        self._icon = icon
-        self.update()
-
-    def iconSize(self):
-        """ Get the icon size for the widget.
+        mime_type : unicode
+            The mime type of interest.
 
         Returns
         -------
-        result : QSize
-            The size to use for displaying the icon.
+        result : bool
+            True if there is data for the given type, False otherwise.
 
         """
-        return self._icon_size
+        raise NotImplementedError
 
-    def setIconSize(self, size):
-        """ Set the icon size for the widget.
+    def remove_format(self, mime_type):
+        """ Remove the data entry for the given mime type.
 
         Parameters
         ----------
-        size : QSize
-            The icon size to use for the widget.
+        mime_type : unicode
+            The mime type of interest.
 
         """
-        self._icon_size = size
-        self.updateGeometry()
-        self.update()
-
-    #--------------------------------------------------------------------------
-    # Reimplementations
-    #--------------------------------------------------------------------------
-    def sizeHint(self):
-        """ Get the size hint for the widget.
+        raise NotImplementedError
 
-        """
-        return self.minimumSizeHint()
+    def data(self, mime_type):
+        """ Get the data for the specified mime type.
 
-    def minimumSizeHint(self):
-        """ Get the minimum size hint for the widget.
+        Parameters
+        ----------
+        mime_type : unicode
+            The mime type of interest.
+
+        Returns
+        -------
+        result : str
+            The data for the specified mime type.
 
         """
-        size = self._icon_size
-        if not size.isValid():
-            size = QSize(16, 16)
-        left, top, right, bottom = self.getContentsMargins()
-        return size + QSize(left + right, top + bottom)
+        raise NotImplementedError
+
+    def set_data(self, mime_type, data):
+        """ Set the data for the specified mime type.
+
+        Parameters
+        ----------
+        mime_type : unicode
+            The mime type of interest.
 
-    def paintEvent(self, event):
-        """ Handle the paint event for the widget.
+        data : str
+            The serialized data for the given type.
 
         """
-        super(QIconWidget, self).paintEvent(event)
-        icon = self._icon
-        if icon.isNull():
-            return
-        icon.paint(QPainter(self), self.contentsRect())
+        raise NotImplementedError
```

### Comparing `enaml-0.9.7/enaml/qt/docking/layout_handling.py` & `enaml-0.9.8/enaml/qt/docking/layout_handling.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/layout_builder.py` & `enaml-0.9.8/enaml/qt/docking/layout_builder.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/q_dock_title_bar.py` & `enaml-0.9.8/enaml/qt/docking/q_dock_title_bar.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/dock_manager.py` & `enaml-0.9.8/enaml/qt/docking/dock_manager.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/dock_resources.py` & `enaml-0.9.8/enaml/qt/docking/dock_resources.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/q_dock_window.py` & `enaml-0.9.8/enaml/qt/docking/q_dock_window.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/q_dock_area.py` & `enaml-0.9.8/enaml/qt/docking/q_dock_tab_widget.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,459 +1,430 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from enaml.qt.QtCore import QMargins, QSize, QEvent
+from weakref import ref
+
+from enaml.qt.QtCore import Qt, QPoint, QSize, QMetaObject, QEvent
 from enaml.qt.QtGui import (
-    QFrame, QLayout, QTabWidget, QGridLayout, QStackedLayout, QVBoxLayout,
-    QWidget, QStyle, QStyleOption
+    QApplication, QTabBar, QTabWidget, QMouseEvent, QResizeEvent, QStyle,
+    QCursor, QStylePainter, QStyleOptionTabV3, QPixmap, QPainter
 )
 
-from .q_dock_bar import QDockBarManager
-
-
-class QDockAreaLayout(QStackedLayout):
-    """ A custom stacked layout for the QDockArea.
-
-    This stacked layout reports its size hints according to the widget
-    which is currently visible, as opposed to aggregated hints which is
-    the default.
-
-    """
-    def sizeHint(self):
-        """ Get the size hint for the layout.
-
-        """
-        widget = self.currentWidget()
-        if widget is not None:
-            return widget.sizeHint()
-        return QSize(256, 192)
-
-    def minimumSize(self):
-        """ Get the minimum size for the layout.
-
-        """
-        widget = self.currentWidget()
-        if widget is not None:
-            return widget.minimumSizeHint()
-        return QSize(256, 192)
+from .event_types import QDockItemEvent, DockTabSelected
+from .q_bitmap_button import QBitmapButton
+from .utils import repolish
+from .xbms import CLOSE_BUTTON
 
 
-class QDockArea(QFrame):
-    """ A custom QFrame which provides an area for docking QDockItems.
-
-    A dock area is used by creating QDockItem instances using the dock
-    area as the parent. A DockLayout instance can then be created and
-    applied to the dock area with the 'setDockLayout' method. The names
-    in the DockLayoutItem objects are used to find the matching dock
-    item widget child.
+class QDockTabCloseButton(QBitmapButton):
+    """ A bitmap button subclass used as a dock tab close button.
 
     """
-    def __init__(self, parent=None):
-        """ Initialize a QDockArea.
-
-        Parameters
-        ----------
-        parent : QWidget
-            The parent of the dock area.
-
-        """
-        super(QDockArea, self).__init__(parent)
-        self._dock_bar_manager = QDockBarManager(self)
-        self._primary_pane = primary_pane = QWidget(self)
-        self._central_pane = central_pane = QWidget(primary_pane)
-        self._dock_events_enabled = False
-        self._opaque_resize = None
-        self._tab_position = None
-
-        central_layout = QVBoxLayout()
-        central_layout.setContentsMargins(QMargins(0, 0, 0, 0))
-        central_layout.setSizeConstraint(QLayout.SetMinimumSize)
-        central_pane.setLayout(central_layout)
-
-        grid_layout = QGridLayout()
-        grid_layout.setRowStretch(0, 0)
-        grid_layout.setRowStretch(1, 1)
-        grid_layout.setRowStretch(2, 0)
-        grid_layout.setColumnStretch(0, 0)
-        grid_layout.setColumnStretch(1, 1)
-        grid_layout.setColumnStretch(2, 0)
-        grid_layout.setContentsMargins(QMargins(0, 0, 0, 0))
-        grid_layout.setSizeConstraint(QLayout.SetMinimumSize)
-        grid_layout.addWidget(central_pane, 1, 1)
-        primary_pane.setLayout(grid_layout)
-
-        area_layout = QDockAreaLayout()
-        area_layout.setContentsMargins(QMargins(0, 0, 0, 0))
-        area_layout.setSizeConstraint(QLayout.SetMinimumSize)
-        area_layout.insertWidget(0, primary_pane)
-        self.setLayout(area_layout)
-        self.updateSpacing()
-
-    #--------------------------------------------------------------------------
-    # Protected API
-    #--------------------------------------------------------------------------
-    def event(self, event):
-        """ A generic event handler for the dock area.
-
-        """
-        if event.type() == QEvent.StyleChange:
-            self.updateSpacing()
-        return super(QDockArea, self).event(event)
-
-    #--------------------------------------------------------------------------
-    # Public API
-    #--------------------------------------------------------------------------
-    def updateSpacing(self):
-        """ Update the primary layout spacing for the dock area.
-
-        This method will extract spacing value defined in the style
-        sheet for the dock area and apply it to the spacing between
-        the dock bars and the central widget.
-
-        """
-        opt = QStyleOption()
-        opt.initFrom(self)
-        style = self.style()
-        # hack to get the style sheet 'spacing' property.
-        spacing = style.pixelMetric(QStyle.PM_ToolBarItemSpacing, opt, self)
-        grid_layout = self._primary_pane.layout()
-        grid_layout.setVerticalSpacing(spacing)
-        grid_layout.setHorizontalSpacing(spacing)
-
-    def centralPane(self):
-        """ Get the central pane for the dock area.
-
-        This method is used the dock bar manager to access the central
-        layout pane. It should not normally be called by user code.
+    def styleOption(self):
+        """ Get a filled style option for the button.
 
         Returns
         -------
-        result : QWidget
-            The central pane for the dock area.
+        result : QStyleOption
+            A style option initialized for the current button state.
 
         """
-        return self._central_pane
+        opt = super(QDockTabCloseButton, self).styleOption()
+        parent = self.parent()
+        if isinstance(parent, QDockTabBar):
+            index = parent.currentIndex()
+            if parent.tabButton(index, QTabBar.RightSide) is self:
+                opt.state |= QStyle.State_Selected
+        return opt
 
-    def primaryPane(self):
-        """ Get the primary pane for the dock area.
 
-        This method is used the dock bar manager to access the primary
-        layout pane. It should not normally be called by user code.
+class _TabData(object):
+    """ A private class which holds data about a tab in a tab bar.
 
-        Returns
-        -------
-        result : QWidget
-            The primary pane for the dock area.
-
-        """
-        return self._primary_pane
+    """
+    __slots__ = ('ref', 'normal', 'selected', 'alerted')
 
-    def centralWidget(self):
-        """ Get the central dock widget for the area.
+    def __init__(self, container):
+        self.ref = ref(container)
+        self.normal = None
+        self.selected = None
+        self.alerted = False
 
-        This method is called by the dock manager which handles the
-        dock area. It should not normally be called by user code.
+    @property
+    def container(self):
+        return self.ref()
 
-        Returns
-        -------
-        result : QWidget or None
-            The central dock widget for the area, or None if no widget
-            is installed.
 
-        """
-        item = self._central_pane.layout().itemAt(0)
-        if item is not None:
-            return item.widget()
+class QDockTabBar(QTabBar):
+    """ A custom QTabBar that manages safetly undocking a tab.
 
-    def setCentralWidget(self, widget):
-        """ Set the central widget for the dock area.
+    The user can undock a tab by holding Shift before dragging the tab.
+    This tab bar assumes that its parent is a QTabWidget and that the
+    tabs in the tab widget are QDockItem instances.
 
-        This method is called by the dock manager which handles the
-        dock area. It should not normally be called by user code.
+    """
+    def __init__(self, parent=None):
+        """ Initialize a QDockTabBar.
 
         Parameters
         ----------
-        widget : QWidget
-            The central widget for the dock area.
+        parent : QWidget or None
+            The parent widget for the tab bar.
 
         """
-        layout = self._central_pane.layout()
-        item = layout.itemAt(0)
-        if item is not None:
-            old = item.widget()
-            if old is widget:
-                return
-            old.hide()
-            old.setParent(None)
-        if widget is not None:
-            layout.addWidget(widget)
-            # lower the widget to keep it stacked behind any pinned
-            # containers which are in the slide-out position.
-            widget.lower()
-            widget.show()
-
-    def maximizedWidget(self):
-        """ Get the widget to that is set as the maximized widget.
+        super(QDockTabBar, self).__init__(parent)
+        self.setSelectionBehaviorOnRemove(QTabBar.SelectPreviousTab)
+        self.tabMoved.connect(self._onTabMoved)
+        self._has_alerts = False
+        self._has_mouse = False
+        self._tab_data = []
 
-        Returns
-        -------
-        result : QWidget or None
-            The widget which is maximized over the dock area.
-
-        """
-        return self.layout().widget(1)
-
-    def setMaximizedWidget(self, widget):
-        """ Set the widget to maximize over the dock area.
-
-        Returns
-        -------
-        result : QWidget or None
-            The widget to maximize over the dock area.
-
-        """
-        old = self.maximizedWidget()
-        if old is not None:
-            if old is widget:
-                return
-            old.hide()
-            old.setParent(None)
-        if widget is not None:
-            layout = self.layout()
-            layout.insertWidget(1, widget)
-            layout.setCurrentIndex(1)
-            widget.show()
-
-    def addToDockBar(self, container, position, index=-1):
-        """ Add a container to the dock bar at the given position.
+    #--------------------------------------------------------------------------
+    # Public API
+    #--------------------------------------------------------------------------
+    def setCloseButtonVisible(self, index, visible):
+        """ Set the close button visibility for the given tab index.
 
         Parameters
         ----------
-        container : QDockContainer
-            The dock container to add to the dock bar. The container
-            should be unplugged from any other layout before calling
-            this method.
+        index : int
+            The index of the tab to set the close button visibility.
 
-        position : QDockBar.Position
-            The enum value specifying the dock bar to which the
-            container should be added.
+        visible : bool
+            Whether or not the close button should be visible.
+
+        """
+        if index < 0 or index >= self.count():
+            return
+        button = self.tabButton(index, QTabBar.RightSide)
+        if button is not None:
+            if button.isVisibleTo(self) != visible:
+                # The public QTabBar api does not provide a way to
+                # trigger the 'layoutTabs' method of QTabBarPrivate
+                # and there are certain operations (such as modifying
+                # a tab close button) which need to have that happen.
+                # A workaround is to send a dummy resize event.
+                button.setVisible(visible)
+                if not visible:
+                    button.resize(0, 0)
+                else:
+                    button.resize(button.sizeHint())
+                size = self.size()
+                event = QResizeEvent(size, size)
+                QApplication.sendEvent(self, event)
+                self.update()
 
-        index : int, optional
-            The index at which to insert the item. The default is -1
-            and will append the item to the dock bar.
-
-        """
-        self._dock_bar_manager.addContainer(container, position, index)
-
-    def removeFromDockBar(self, container):
-        """ Remove a container previously added to a dock bar.
+    #--------------------------------------------------------------------------
+    # Private API
+    #--------------------------------------------------------------------------
+    def _onTabMoved(self, from_index, to_index):
+        """ A handler for the 'tabMoved' signal.
 
-        Parameters
-        ----------
-        container : QDockContainer
-            The dock container to remove from the dock bar.
+        This handler synchronizes the internal tab data structures for
+        the new positions of the tabs.
 
         """
-        self._dock_bar_manager.removeContainer(container)
+        data = self._tab_data.pop(from_index)
+        self._tab_data.insert(to_index, data)
 
-    def dockBarGeometry(self, position):
-        """ Get the geometry of the dock bar at the given position.
+    def _onCloseButtonClicked(self):
+        """ Handle the 'clicked' signal on the tab close buttons.
 
-        Parameters
-        ----------
-        position : QDockBar.Position
-            The enum value specifying the dock bar of interest.
-
-        Returns
-        -------
-        result : QRect
-            The geometry of the given dock bar expressed in area
-            coordinates. If no dock bar exists at the given position,
-            an invalid QRect will be returned.
+        This handler will find the tab index for the clicked button
+        and emit the 'tabCloseRequested' signal with that index.
 
         """
-        return self._dock_bar_manager.dockBarGeometry(position)
+        button = self.sender()
+        for index in xrange(self.count()):
+            if self.tabButton(index, QTabBar.RightSide) is button:
+                self.tabCloseRequested.emit(index)
 
-    def dockBarContainers(self):
-        """ Get the containers held in the dock bars.
+    def _onAlerted(self, level):
+        """ A signal handler for the 'alerted' signal on a container.
 
-        Returns
-        -------
-        result : list
-            A list of tuples of the form (container, position).
+        This handler will re-snap the pixmaps for the alerted tab
+        and trigger a repaint of the tab bar.
 
         """
-        return self._dock_bar_manager.dockBarContainers()
+        container = self.sender()
+        index = self.parent().indexOf(container)
+        if index != -1:
+            if level:
+                self._snapAlertPixmaps(index, level)
+            else:
+                self._clearAlertPixmaps(index)
+            self.update()
 
-    def dockBarPosition(self, container):
-        """ Get the dock bar position of the given container.
+    def _snapAlertPixmaps(self, index, level):
+        """ Snap the alert pixmaps for the specified tab.
 
         Parameters
         ----------
-        container : QDockContainer
-            The dock container of interest.
+        index : int
+            The index of the tab of interest.
 
-        Returns
-        -------
-        result : QDockBar.Position or None
-            The position of the container, or None if the container
-            does not exist in the manager.
+        level : unicode
+            The alert level for which to snap the pixmaps.
 
         """
-        return self._dock_bar_manager.dockBarPosition(container)
+        # Force an internal update of the stylesheet rules
+        self.setProperty(u'alert', level)
+        repolish(self)
 
-    def extendFromDockBar(self, container):
-        """ Extend the given container from its dock bar.
+        # Setup the style option for the control
+        opt = QStyleOptionTabV3()
+        self.initStyleOption(opt, index)
+        opt.rect.moveTo(0, 0)
 
-        If the container does not exist in a dock bar, this is a no-op.
+        # Snap the normal pixmap
+        opt.state &= ~QStyle.State_Selected
+        normal = QPixmap(opt.rect.size())
+        normal.fill(Qt.transparent)
+        painter = QStylePainter(normal, self)
+        painter.initFrom(self)
+        painter.drawControl(QStyle.CE_TabBarTab, opt)
 
-        Parameters
-        ----------
-        container : QDockContainer
-            The dock container of interest.
+        # Snap the selected pixmap
+        opt.state |= QStyle.State_Selected
+        selected = QPixmap(opt.rect.size())
+        selected.fill(Qt.transparent)
+        painter = QStylePainter(selected, self)
+        painter.initFrom(self)
+        painter.drawControl(QStyle.CE_TabBarTab, opt)
 
-        """
-        self._dock_bar_manager.extendContainer(container)
+        # Reset the internal stylesheet style
+        self.setProperty(u'alert', None)
+        repolish(self)
+
+        # Update the internal tab data
+        data = self._tab_data[index]
+        data.normal = normal
+        data.selected = selected
+        data.alerted = True
 
-    def retractToDockBar(self, container):
-        """ Retract the given container into it's dock bar.
+        # Flip the alert flag so the pixmaps are painted
+        self._has_alerts = True
 
-        If the container does not exist in a dock bar, this is a no-op.
+    def _clearAlertPixmaps(self, index):
+        """ Clear the alert pixmaps for the specified tab.
 
         Parameters
         ----------
-        container : QDockContainer
-            The dock container of interest.
-
-        """
-        self._dock_bar_manager.retractContainer(container)
-
-    def clearDockBars(self):
-        """ Clear the dock bars from the dock area.
-
-        This method is called by the dock manager when the dock area
-        is reset. It should not be called directly by user code.
+        index : int
+            The index of the tab of interest.
 
         """
-        self._dock_bar_manager.clearDockBars()
+        data = self._tab_data[index]
+        data.normal = None
+        data.selected = None
+        data.alerted = False
 
-    def isEmpty(self):
-        """ Get whether or not the dock area is empty.
+        # Turn off alert painting if there are no more alerts
+        self._has_alerts = any(d.alerted for d in self._tab_data)
 
-        Returns
-        -------
-        result : bool
-            True if the dock area is empty, False otherwise.
-
-        """
-        if self.centralWidget() is not None:
-            return False
-        if self.maximizedWidget() is not None:
-            return False
-        return self._dock_bar_manager.isEmpty()
-
-    def tabPosition(self):
-        """ Get the default position for newly created tab widgets.
+    #--------------------------------------------------------------------------
+    # Reimplementations
+    #--------------------------------------------------------------------------
+    def tabInserted(self, index):
+        """ Handle a tab insertion in the tab bar.
 
-        The tab position is inherited from an ancestor dock area unless
-        it is explicitly set by the user.
+        This handler will create the close button for the tab and then
+        update its visibilty depending on whether or not the dock item
+        is closable. It will also build the internal tab data structure
+        for the new tab. This method assumes that this tab bar is
+        parented by a QDockTabWidget.
+
+        """
+        button = QDockTabCloseButton(self)
+        button.setObjectName('docktab-close-button')
+        button.setBitmap(CLOSE_BUTTON.toBitmap())
+        button.setIconSize(QSize(14, 13))
+        button.clicked.connect(self._onCloseButtonClicked)
+        self.setTabButton(index, QTabBar.LeftSide, None)
+        self.setTabButton(index, QTabBar.RightSide, button)
+        container = self.parent().widget(index)
+        container.alerted.connect(self._onAlerted)
+        self.setCloseButtonVisible(index, container.closable())
+        self._tab_data.insert(index, _TabData(container))
+
+    def tabRemoved(self, index):
+        """ Handle a tab removal from the tab bar.
+
+        This will remove the internal tab data structure and disconnect
+        the relevant signals.
+
+        """
+        data = self._tab_data.pop(index)
+        container = data.container
+        if container is not None:
+            container.alerted.disconnect(self._onAlerted)
+
+    def mousePressEvent(self, event):
+        """ Handle the mouse press event for the tab bar.
+
+        This handler will set the internal '_has_mouse' flag if the
+        left mouse button is pressed on a tab.
+
+        """
+        super(QDockTabBar, self).mousePressEvent(event)
+        self._has_mouse = False
+        if event.button() == Qt.LeftButton:
+            index = self.tabAt(event.pos())
+            if index != -1:
+                self._has_mouse = True
+                data = self._tab_data[index]
+                container = data.container
+                if container is not None:
+                    # likey a no-op, but just in case
+                    container.dockItem().clearAlert()
+        elif event.button() == Qt.RightButton:
+            index = self.tabAt(event.pos())
+            if index != -1:
+                button = self.tabButton(index, QTabBar.RightSide)
+                if button.geometry().contains(event.pos()):
+                    return
+                item = self.parent().widget(index).dockItem()
+                item.titleBarRightClicked.emit(event.globalPos())
+                # Emitting the clicked signal may have caused a popup
+                # menu to open, which will have grabbed the mouse. When
+                # this happens, the hover leave event is not sent and
+                # the tab bar will be stuck in the hovered paint state.
+                # Manual checking as 'underMouse' yields False negatives.
+                p = self.mapFromGlobal(QCursor.pos())
+                if not self.rect().contains(p):
+                    QApplication.sendEvent(self, QEvent(QEvent.HoverLeave))
+
+    def mouseMoveEvent(self, event):
+        """ Handle the mouse move event for the tab bar.
+
+        This handler will undock the tab if the mouse is held and the
+        drag leaves the boundary of the container by the application
+        drag distance amount.
+
+        """
+        super(QDockTabBar, self).mouseMoveEvent(event)
+        if not self._has_mouse:
+            return
+        pos = event.pos()
+        if self.rect().contains(pos):
+            return
+        x = max(0, min(pos.x(), self.width()))
+        y = max(0, min(pos.y(), self.height()))
+        dist = (QPoint(x, y) - pos).manhattanLength()
+        if dist > QApplication.startDragDistance():
+            # Fake a mouse release event so that the tab resets its
+            # internal state and finalizes the animation for the tab.
+            # The button must be Qt.LeftButton, not event.button().
+            btn = Qt.LeftButton
+            mod = event.modifiers()
+            evt = QMouseEvent(QEvent.MouseButtonRelease, pos, btn, btn, mod)
+            QApplication.sendEvent(self, evt)
+            container = self.parent().widget(self.currentIndex())
+            container.untab(event.globalPos())
+            self._has_mouse = False
+
+    def mouseReleaseEvent(self, event):
+        """ Handle the mouse release event for the tab bar.
+
+        This handler will reset the internal '_has_mouse' flag when the
+        left mouse button is released.
+
+        """
+        super(QDockTabBar, self).mouseReleaseEvent(event)
+        if event.button() == Qt.LeftButton:
+            self._has_mouse = False
+
+    def paintEvent(self, event):
+        """ A custom paint event for the tab bar.
+
+        This paint event will blit the pixmaps for the alerted tabs as
+        necessary, after the superclass paint event handler is run.
+
+        """
+        super(QDockTabBar, self).paintEvent(event)
+        if self._has_alerts:
+            painter = QPainter(self)
+            current = self.currentIndex()
+            for index, data in enumerate(self._tab_data):
+                if data.alerted:
+                    rect = self.tabRect(index)
+                    pm = data.selected if index == current else data.normal
+                    painter.drawPixmap(rect, pm)
+
+
+class QDockTabWidget(QTabWidget):
+    """ A custom tab widget for use in the dock area.
+
+    This custom widget ensures that the proper dock tab bar is used. It
+    also allows distinguishing dock tab widgets from standard QTabWidget
+    instances used elsewhere in the application.
 
-        Returns
-        -------
-        result : QTabWidget.TabPosition
-            The position for dock area tabs. If the value has not been
-            set by the user and there is no ancestor dock area, the
-            default is QTabWidget.North.
-
-        """
-        pos = self._tab_position
-        if pos is not None:
-            return pos
-        p = self.parent()
-        while p is not None:
-            if isinstance(p, QDockArea):
-                return p.tabPosition()
-            p = p.parent()
-        return QTabWidget.North
-
-    def setTabPosition(self, position):
-        """ Set the default position for newly created tab widget.
+    """
+    def __init__(self, parent=None):
+        """ Initialize a QDockTabWidget.
 
         Parameters
         ----------
-        position : QTabWidget.TabPosition
-            The position for the tabs of newly created tab widgets.
+        parent : QWidget, optional
+            The parent widget of the tab widget.
 
         """
-        self._tab_position = position
-
-    def dockEventsEnabled(self):
-        """ Get whether dock events are enabled for the area.
+        super(QDockTabWidget, self).__init__(parent)
+        self.setTabBar(QDockTabBar())
+        self.setElideMode(Qt.ElideRight)
+        self.setUsesScrollButtons(True)
+        self.setTabsClosable(True)
+        self.setDocumentMode(True)
+        self.setMovable(True)
+        self.tabBar().setDrawBase(False)
+        self.tabCloseRequested.connect(self._onTabCloseRequested)
+        self.currentChanged.connect(self._onCurrentChanged)
 
-        Returns
-        -------
-        result : bool
-            True if dock events are enabled, False otherwise.
+    #--------------------------------------------------------------------------
+    # Private API
+    #--------------------------------------------------------------------------
+    def _onTabCloseRequested(self, index):
+        """ Handle the close request for the given tab index.
 
         """
-        return self._dock_events_enabled
-
-    def setDockEventsEnabled(self, enabled):
-        """ Set whether dock events are enabled for the area.
+        # Invoke the close slot later to allow the signal to return.
+        container = self.widget(index)
+        QMetaObject.invokeMethod(container, 'close', Qt.QueuedConnection)
+
+    def _onCurrentChanged(self, index):
+        """ Handle the 'currentChanged' signal for the tab widget.
+
+        """
+        # These checks protect against the signal firing during close.
+        container = self.widget(index)
+        if container is None:
+            return
+        manager = container.manager()
+        if manager is None:
+            return
+        area = manager.dock_area()
+        if area is None:
+            return
+        if area.dockEventsEnabled():
+            event = QDockItemEvent(DockTabSelected, container.objectName())
+            QApplication.postEvent(area, event)
 
-        If events are enabled, then the various widgets involved with
-        the dock area will post events to the *root* dock area when the
-        various states have changed. If events are disabled, no such
-        events will be posted.
+    #--------------------------------------------------------------------------
+    # Public API
+    #--------------------------------------------------------------------------
+    def setCloseButtonVisible(self, index, visible):
+        """ Set the close button visibility for the given tab index.
 
         Parameters
         ----------
-        enabled : bool
-            True if dock events should be enabled, False otherwise.
-
-        """
-        self._dock_events_enabled = enabled
-
-    def opaqueItemResize(self):
-        """ Get whether opaque item resize is enabled.
-
-        The tab position is inherited from an ancestor dock area unless
-        it is explicitly set by the user.
+        index : int
+            The index of the tab to set the close button visibility.
 
-        Returns
-        -------
-        result : bool
-            True if item resizing is opaque, False otherwise. If the
-            value has not been set by the user and there is no ancestor
-            dock area, the default is True.
-
-        """
-        opaque = self._opaque_resize
-        if opaque is not None:
-            return opaque
-        p = self.parent()
-        while p is not None:
-            if isinstance(p, QDockArea):
-                return p.opaqueItemResize()
-            p = p.parent()
-        return True
-
-    def setOpaqueItemResize(self, opaque):
-        """ Set whether opaque item resize is enabled.
-
-        Parameters
-        ----------
-        opaque : bool
-            True if item resizing should be opaque, False otherwise.
+        visible : bool
+            Whether or not the close button should be visible.
 
         """
-        is_different = opaque != self.opaqueItemResize()
-        self._opaque_resize = opaque
-        if is_different:
-            # Avoid a circular import
-            from .q_dock_splitter import QDockSplitter
-            for sp in self.findChildren(QDockSplitter):
-                sp.inheritOpaqueResize()
+        self.tabBar().setCloseButtonVisible(index, visible)
```

### Comparing `enaml-0.9.7/enaml/qt/docking/style_sheets.py` & `enaml-0.9.8/enaml/qt/docking/style_sheets.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/q_dock_item.py` & `enaml-0.9.8/enaml/qt/docking/q_dock_item.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/q_dock_frame.py` & `enaml-0.9.8/enaml/qt/docking/q_dock_frame.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/dock_images/cross_ex_box.png` & `enaml-0.9.8/enaml/qt/docking/dock_images/cross_ex_box.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/dock_images/arrow_east.png` & `enaml-0.9.8/enaml/qt/docking/dock_images/arrow_east.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/dock_images/background.png` & `enaml-0.9.8/enaml/qt/docking/dock_images/background.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/dock_images/guide_render.py` & `enaml-0.9.8/enaml/qt/docking/dock_images/guide_render.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/dock_images/split_horizontal.png` & `enaml-0.9.8/enaml/qt/docking/dock_images/split_horizontal.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/dock_images/cross_box.png` & `enaml-0.9.8/enaml/qt/docking/dock_images/cross_box.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/dock_images/arrow_west.png` & `enaml-0.9.8/enaml/qt/docking/dock_images/arrow_west.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/q_guide_rose.py` & `enaml-0.9.8/enaml/qt/docking/q_guide_rose.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/xbms.py` & `enaml-0.9.8/enaml/qt/docking/xbms.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/dock_overlay.py` & `enaml-0.9.8/enaml/qt/docking/dock_overlay.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/utils.py` & `enaml-0.9.8/enaml/qt/docking/utils.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/docking/proximity_handler.py` & `enaml-0.9.8/enaml/qt/docking/proximity_handler.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_combo_box.py` & `enaml-0.9.8/enaml/qt/qt_combo_box.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_tool_button.py` & `enaml-0.9.8/enaml/qt/qt_tool_button.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/enaml/qt/qt_dock_item.py` & `enaml-0.9.8/enaml/qt/qt_flow_area.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,230 +1,199 @@
 #------------------------------------------------------------------------------
 # Copyright (c) 2013, Nucleic Development Team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
-from atom.api import Int, Typed
+from atom.api import Typed
 
-from enaml.styling import StyleCache
-from enaml.widgets.dock_item import ProxyDockItem
+from enaml.widgets.flow_area import ProxyFlowArea
 
-from .QtCore import Qt, QSize, Signal
-from .QtGui import QIcon
+from .QtCore import QEvent, QPoint, QRect
+from .QtGui import QScrollArea, QWidget, QPainter, QPalette, QApplication
 
-from .docking.q_dock_item import QDockItem
+from .qt_frame import QtFrame
+from .qt_flow_item import QtFlowItem
+from .q_flow_layout import QFlowLayout
 
-from .q_resource_helpers import get_cached_qicon
-from .qt_widget import QtWidget
-from .styleutil import translate_dock_item_style
 
+_DIRECTION_MAP = {
+    'left_to_right': QFlowLayout.LeftToRight,
+    'right_to_left': QFlowLayout.RightToLeft,
+    'top_to_bottom': QFlowLayout.TopToBottom,
+    'bottom_to_top': QFlowLayout.BottomToTop,
+}
 
-class QCustomDockItem(QDockItem):
-    """ A custom dock item which converts a close event into a signal.
 
-    """
-    #: A signal emitted if the close event is accepted. It it emitted
-    #: before the close event handler returns.
-    closed = Signal()
-
-    def closeEvent(self, event):
-        """ Handle the close event for the dock item.
+_ALIGN_MAP = {
+    'leading': QFlowLayout.AlignLeading,
+    'trailing': QFlowLayout.AlignTrailing,
+    'center': QFlowLayout.AlignCenter,
+    'justify': QFlowLayout.AlignJustify,
+}
 
-        """
-        super(QCustomDockItem, self).closeEvent(event)
-        if event.isAccepted():
-            self.closed.emit()
 
+class QFlowArea(QScrollArea):
+    """ A custom QScrollArea which implements a flowing layout.
 
-# Guard flags
-TITLE_GUARD = 0x1
-
+    """
+    def __init__(self, parent=None):
+        """ Initialize a QFlowArea.
 
-class QtDockItem(QtWidget, ProxyDockItem):
-    """ A Qt implementation of an Enaml ProxyDockItem.
+        Parameters
+        ----------
+        parent : QWidget, optional
+            The parent widget of this widget.
 
-    """
-    #: A reference to the widget created by the proxy.
-    widget = Typed(QCustomDockItem)
+        """
+        super(QFlowArea, self).__init__(parent)
+        self._widget = QWidget(self)
+        self._layout = QFlowLayout()
+        self._widget.setLayout(self._layout)
+        self.setWidgetResizable(True)
+        self.setWidget(self._widget)
+        # setWidget sets autoFillBackground to True
+        self._widget.setAutoFillBackground(False)
 
-    #: Cyclic notification guard. This a bitfield of multiple guards.
-    _guard = Int(0)
+    def event(self, event):
+        """ A custom event handler for the flow area.
 
-    #--------------------------------------------------------------------------
-    # Initialization API
-    #--------------------------------------------------------------------------
-    def create_widget(self):
-        """ Create the underlying QDockItem widget.
+        This handler paints the empty corner between the scroll bars.
 
         """
-        self.widget = QCustomDockItem(self.parent_widget())
+        res = super(QFlowArea, self).event(event)
+        if event.type() == QEvent.Paint:
+            # Fill in the empty corner area with the app window color.
+            color = QApplication.palette().color(QPalette.Window)
+            tl = self.viewport().geometry().bottomRight()
+            fw = self.frameWidth()
+            br = self.rect().bottomRight() - QPoint(fw, fw)
+            QPainter(self).fillRect(QRect(tl, br), color)
+        return res
 
-    def init_widget(self):
-        """ Initialize the state of the underlying widget.
+    def layout(self):
+        """ Get the layout for this flow area.
 
-        """
-        super(QtDockItem, self).init_widget()
-        d = self.declaration
-        self.set_title(d.title)
-        self.set_title_editable(d.title_editable)
-        if not d.title_bar_visible:
-            self.set_title_bar_visible(d.title_bar_visible)
-        if d.icon is not None:
-            self.set_icon(d.icon)
-        if -1 not in d.icon_size:
-            self.set_icon_size(d.icon_size)
-        self.set_stretch(d.stretch)
-        self.set_closable(d.closable)
+        The majority of interaction for a QFlowArea takes place through
+        its layout, rather than through the widget itself.
 
-    def init_layout(self):
-        """ Initialize the layout for the underyling widget.
+        Returns
+        -------
+        result : QFlowLayout
+            The flow layout for this flow area.
 
         """
-        super(QtDockItem, self).init_layout()
-        widget = self.widget
-        widget.setDockWidget(self.dock_widget())
-        # Use a queued connection so the dock manager can finish
-        # closing the dock item before the signal handler runs.
-        widget.titleEdited.connect(self.on_title_edited)
-        widget.titleBarRightClicked.connect(self.on_title_bar_right_clicked)
-        widget.closed.connect(self.on_closed, Qt.QueuedConnection)
+        return self._layout
 
-    #--------------------------------------------------------------------------
-    # Utility Methods
-    #--------------------------------------------------------------------------
-    def dock_widget(self):
-        """ Find and return the dock widget child for this widget.
+    def setLayout(self, layout):
+        """ A reimplemented method. Setting the layout on a QFlowArea
+        is not supported.
 
         """
-        d = self.declaration.dock_widget()
-        if d is not None:
-            return d.proxy.widget
+        raise TypeError("Cannot set layout on a QFlowArea.")
 
-    #--------------------------------------------------------------------------
-    # Reimplementations
-    #--------------------------------------------------------------------------
-    def refresh_style_sheet(self):
-        """ A reimplemented styling method.
 
-        The dock item uses custom stylesheet processing.
+class QtFlowArea(QtFrame, ProxyFlowArea):
+    """ A Qt implementation of an Enaml ProxyFlowArea.
 
-        """
-        parts = []
-        name = self.widget.objectName()
-        for style in StyleCache.styles(self.declaration):
-            t = translate_dock_item_style(name, style)
-            if t:
-                parts.append(t)
-        if len(parts) > 0:
-            stylesheet = u'\n\n'.join(parts)
-        else:
-            stylesheet = u''
-        self.widget.setStyleSheet(stylesheet)
+    """
+    #: A reference to the widget created by the proxy.
+    widget = Typed(QFlowArea)
 
     #--------------------------------------------------------------------------
-    # Signal Handlers
+    # Initialization API
     #--------------------------------------------------------------------------
-    def on_title_edited(self, text):
-        """ Handle the 'titleEdited' signal on the dock item.
+    def create_widget(self):
+        """ Create the underlying widget.
 
         """
-        d = self.declaration
-        if d is not None:
-            self._guard |= TITLE_GUARD
-            try:
-                d.title = text
-            finally:
-                self._guard &= ~TITLE_GUARD
+        self.widget = QFlowArea(self.parent_widget())
 
-    def on_title_bar_right_clicked(self, pos):
-        """ Handle the 'titleBarRightClicked' signal on the dock item.
+    def init_widget(self):
+        """ Initialize the underlying control.
 
         """
+        super(QtFlowArea, self).init_widget()
         d = self.declaration
-        if d is not None:
-            d.title_bar_right_clicked()
+        self.set_direction(d.direction)
+        self.set_align(d.align)
+        self.set_horizontal_spacing(d.horizontal_spacing)
+        self.set_vertical_spacing(d.vertical_spacing)
+        self.set_margins(d.margins)
 
-    def on_closed(self):
-        """ Handle the closed signal from the dock item.
+    def init_layout(self):
+        """ Initialize the layout for the underlying control.
 
         """
-        d = self.declaration
-        if d is not None:
-            d._item_closed()
+        super(QtFlowArea, self).init_layout()
+        layout = self.widget.layout()
+        for child in self.children():
+            if isinstance(child, QtFlowItem):
+                layout.addWidget(child.widget)
 
     #--------------------------------------------------------------------------
     # Child Events
     #--------------------------------------------------------------------------
     def child_added(self, child):
-        """ Handle the child added event for a QtDockItem.
+        """ Handle the child added event for a QtMdiArea.
 
         """
-        super(QtDockItem, self).child_added(child)
-        self.widget.setDockWidget(self.dock_widget())
+        super(QtFlowArea, self).child_added(child)
+        if isinstance(child, QtFlowItem):
+            for index, dchild in enumerate(self.children()):
+                if dchild is child:
+                    self.widget.layout().insertWidget(index, child.widget)
 
     def child_removed(self, child):
-        """ Handle the child added event for a QtDockItem.
+        """ Handle the child removed event for a QtMdiArea.
 
         """
-        super(QtDockItem, self).child_removed(child)
-        self.widget.setDockWidget(self.dock_widget())
+        super(QtFlowArea, self).child_removed(child)
+        if isinstance(child, QtFlowItem) and child.widget is not None:
+            self.widget.layout().removeWidget(child.widget)
 
     #--------------------------------------------------------------------------
-    # ProxyDockItem API
+    # ProxyFlowArea API
     #--------------------------------------------------------------------------
-    def set_title(self, title):
-        """ Set the title on the underlying widget.
-
-        """
-        if not self._guard & TITLE_GUARD:
-            self.widget.setTitle(title)
-
-    def set_title_editable(self, editable):
-        """ Set the title editable state on the underlying widget.
+    def set_direction(self, direction):
+        """ Set the direction for the underlying control.
 
         """
-        self.widget.setTitleEditable(editable)
+        self.widget.layout().setDirection(_DIRECTION_MAP[direction])
 
-    def set_title_bar_visible(self, visible):
-        """ Set the visibility of the widget's title bar.
+    def set_align(self, align):
+        """ Set the alignment for the underlying control.
 
         """
-        self.widget.setTitleBarForceHidden(not visible)
+        self.widget.layout().setAlignment(_ALIGN_MAP[align])
 
-    def set_icon(self, icon):
-        """ Set the icon on the underlying widget.
+    def set_horizontal_spacing(self, spacing):
+        """ Set the horizontal spacing of the underyling control.
 
         """
-        if icon:
-            qicon = get_cached_qicon(icon)
-        else:
-            qicon = QIcon()
-        self.widget.setIcon(qicon)
+        self.widget.layout().setHorizontalSpacing(spacing)
 
-    def set_icon_size(self, size):
-        """ Set the icon size on the underlying widget.
+    def set_vertical_spacing(self, spacing):
+        """ Set the vertical spacing of the underlying control.
 
         """
-        self.widget.setIconSize(QSize(*size))
+        self.widget.layout().setVerticalSpacing(spacing)
 
-    def set_stretch(self, stretch):
-        """ Set the stretch factor for the underlyling widget.
+    def set_margins(self, margins):
+        """ Set the margins of the underlying control.
 
         """
-        sp = self.widget.sizePolicy()
-        sp.setHorizontalStretch(stretch)
-        sp.setVerticalStretch(stretch)
-        self.widget.setSizePolicy(sp)
+        top, right, bottom, left = margins
+        self.widget.layout().setContentsMargins(left, top, right, bottom)
 
-    def set_closable(self, closable):
-        """ Set the closable flag for the underlying widget.
-
-        """
-        self.widget.setClosable(closable)
+    #--------------------------------------------------------------------------
+    # Overrides
+    #--------------------------------------------------------------------------
+    def replace_constraints(self, old_cns, new_cns):
+        """ A reimplemented QtConstraintsWidget layout method.
 
-    def alert(self, level, on, off, repeat, persist):
-        """ Set the alert level on the underlying widget.
+        Constraints layout may not cross the boundary of a FlowArea,
+        so this method is no-op which stops the layout propagation.
 
         """
-        self.widget.alert(level, on, off, repeat, persist)
+        pass
```

### Comparing `enaml-0.9.7/examples/styling/banner.enaml` & `enaml-0.9.8/examples/styling/banner.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/styling/gradient_push_button.enaml` & `enaml-0.9.8/examples/styling/gradient_push_button.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/styling/dock_item_alerts.enaml` & `enaml-0.9.8/examples/styling/dock_item_alerts.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/dock_pane.enaml` & `enaml-0.9.8/examples/widgets/dock_pane.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/popup_menu.enaml` & `enaml-0.9.8/examples/widgets/popup_menu.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/group_box.enaml` & `enaml-0.9.8/examples/widgets/group_box.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/main_window.enaml` & `enaml-0.9.8/examples/widgets/main_window.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/scroll_area.enaml` & `enaml-0.9.8/examples/widgets/scroll_area.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/flow_area.enaml` & `enaml-0.9.8/examples/widgets/flow_area.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/focus_traversal.enaml` & `enaml-0.9.8/examples/widgets/focus_traversal.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/slider.enaml` & `enaml-0.9.8/examples/widgets/slider.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/v_group.enaml` & `enaml-0.9.8/examples/widgets/v_group.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/dual_slider.enaml` & `enaml-0.9.8/examples/widgets/dual_slider.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/mpl_canvas.enaml` & `enaml-0.9.8/examples/widgets/mpl_canvas.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/form.enaml` & `enaml-0.9.8/examples/widgets/form.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/window.enaml` & `enaml-0.9.8/examples/widgets/window.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/dock_area.enaml` & `enaml-0.9.8/examples/widgets/dock_area.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/buttons.enaml` & `enaml-0.9.8/examples/widgets/buttons.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/spin_box.enaml` & `enaml-0.9.8/examples/widgets/spin_box.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/h_group.enaml` & `enaml-0.9.8/examples/widgets/h_group.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/window_closing.enaml` & `enaml-0.9.8/examples/widgets/window_closing.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/menu_bar.enaml` & `enaml-0.9.8/examples/widgets/menu_bar.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/form_spacing.enaml` & `enaml-0.9.8/examples/widgets/form_spacing.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/notebook.enaml` & `enaml-0.9.8/examples/widgets/notebook.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/progress_bar.enaml` & `enaml-0.9.8/examples/widgets/progress_bar.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/context_menu.enaml` & `enaml-0.9.8/examples/widgets/context_menu.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/tool_bar.enaml` & `enaml-0.9.8/examples/widgets/tool_bar.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/images/document-open.png` & `enaml-0.9.8/examples/widgets/images/document-open.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/images/system-search.png` & `enaml-0.9.8/examples/widgets/images/system-search.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/images/img3.png` & `enaml-0.9.8/docs/source/examples/images/img3.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/images/img2.png` & `enaml-0.9.8/docs/source/examples/images/img2.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/images/document-new.png` & `enaml-0.9.8/examples/widgets/images/document-new.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/images/emblem-system.png` & `enaml-0.9.8/examples/widgets/images/emblem-system.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/images/img1.png` & `enaml-0.9.8/docs/source/examples/images/img1.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/images/go-previous.png` & `enaml-0.9.8/examples/widgets/images/go-previous.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/images/list-add.png` & `enaml-0.9.8/examples/widgets/images/list-add.png`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/splitter.enaml` & `enaml-0.9.8/examples/widgets/splitter.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/popup_view.enaml` & `enaml-0.9.8/examples/widgets/popup_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/window_children.enaml` & `enaml-0.9.8/examples/widgets/window_children.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/tool_buttons.enaml` & `enaml-0.9.8/examples/widgets/tool_buttons.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/file_dialog.enaml` & `enaml-0.9.8/examples/widgets/file_dialog.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/image_view.enaml` & `enaml-0.9.8/examples/widgets/image_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/widgets/vtk_canvas.enaml` & `enaml-0.9.8/examples/widgets/vtk_canvas.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/templates/advanced.enaml` & `enaml-0.9.8/examples/templates/advanced.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/templates/basic.enaml` & `enaml-0.9.8/examples/templates/basic.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/dynamic/notebook_pages.enaml` & `enaml-0.9.8/examples/dynamic/notebook_pages.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/dynamic/looper.enaml` & `enaml-0.9.8/examples/dynamic/looper.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/dynamic/fields.enaml` & `enaml-0.9.8/examples/dynamic/fields.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/dynamic/conditional.enaml` & `enaml-0.9.8/examples/dynamic/conditional.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/aliases/simple_attribute_alias.enaml` & `enaml-0.9.8/examples/aliases/simple_attribute_alias.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/aliases/chained_widget_alias.enaml` & `enaml-0.9.8/examples/aliases/chained_widget_alias.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/aliases/chained_attribute_alias.enaml` & `enaml-0.9.8/examples/aliases/chained_attribute_alias.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/aliases/simple_widget_alias.enaml` & `enaml-0.9.8/examples/aliases/simple_widget_alias.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/tutorial/employee/employee_view.enaml` & `enaml-0.9.8/examples/tutorial/employee/employee_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/tutorial/employee/employee.py` & `enaml-0.9.8/examples/tutorial/employee/employee.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/tutorial/employee/phone_validator.py` & `enaml-0.9.8/examples/tutorial/employee/phone_validator.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/tutorial/hello_world/hello_world.py` & `enaml-0.9.8/examples/tutorial/hello_world/hello_world.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/tutorial/hello_world/hello_world_view.enaml` & `enaml-0.9.8/examples/tutorial/hello_world/hello_world_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/tutorial/person/person.py` & `enaml-0.9.8/examples/tutorial/person/person.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/tutorial/person/person_view.enaml` & `enaml-0.9.8/examples/tutorial/person/person_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/stdlib/task_dialog.enaml` & `enaml-0.9.8/examples/stdlib/task_dialog.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/stdlib/slider_transform.enaml` & `enaml-0.9.8/examples/stdlib/slider_transform.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/stdlib/mapped_view.enaml` & `enaml-0.9.8/examples/stdlib/mapped_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/stdlib/message_box.enaml` & `enaml-0.9.8/examples/stdlib/message_box.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/workbench/persistent_view.enaml` & `enaml-0.9.8/examples/workbench/persistent_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/workbench/crash_course.rst` & `enaml-0.9.8/examples/workbench/crash_course.rst`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/workbench/sample.py` & `enaml-0.9.8/examples/workbench/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #------------------------------------------------------------------------------
 """ A simple example plugin application.
 
-This example serves to demostrates the concepts described the accompanying
+This example serves to demonstrate the concepts described the accompanying
 developer crash source document.
 
 """
 from enaml.workbench.ui.api import UIWorkbench
 
 
 if __name__ == '__main__':
```

### Comparing `enaml-0.9.7/examples/workbench/sample_plugin.enaml` & `enaml-0.9.8/examples/workbench/sample_plugin.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/workbench/first_view.enaml` & `enaml-0.9.8/examples/workbench/first_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/workbench/persistent_workspace.py` & `enaml-0.9.8/examples/workbench/persistent_workspace.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/workbench/second_view.enaml` & `enaml-0.9.8/examples/workbench/second_view.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/workbench/sample_workspace.py` & `enaml-0.9.8/examples/workbench/sample_workspace.py`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/applib/live_editor.enaml` & `enaml-0.9.8/examples/applib/live_editor.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/basic/align.enaml` & `enaml-0.9.8/examples/layout/basic/align.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/basic/hbox_equal_widths.enaml` & `enaml-0.9.8/examples/layout/basic/hbox_equal_widths.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/basic/horizontal.enaml` & `enaml-0.9.8/examples/layout/basic/horizontal.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/basic/grid.enaml` & `enaml-0.9.8/examples/layout/basic/grid.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/basic/vertical.enaml` & `enaml-0.9.8/examples/layout/basic/vertical.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/basic/hbox.enaml` & `enaml-0.9.8/examples/layout/basic/hbox.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/basic/linear_relations.enaml` & `enaml-0.9.8/examples/layout/basic/linear_relations.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/basic/hbox_spacing.enaml` & `enaml-0.9.8/examples/layout/basic/hbox_spacing.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/basic/vbox.enaml` & `enaml-0.9.8/examples/layout/basic/vbox.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/basic/align_offset.enaml` & `enaml-0.9.8/examples/layout/basic/align_offset.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/advanced/nested_containers.enaml` & `enaml-0.9.8/examples/layout/advanced/nested_containers.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/advanced/button_ring.enaml` & `enaml-0.9.8/examples/layout/advanced/button_ring.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/advanced/manual_vbox.enaml` & `enaml-0.9.8/examples/layout/advanced/manual_vbox.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/advanced/factory_func.enaml` & `enaml-0.9.8/examples/layout/advanced/factory_func.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/advanced/fluid.enaml` & `enaml-0.9.8/examples/layout/advanced/fluid.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/advanced/nested_boxes.enaml` & `enaml-0.9.8/examples/layout/advanced/nested_boxes.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/advanced/manual_hbox.enaml` & `enaml-0.9.8/examples/layout/advanced/manual_hbox.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/examples/layout/advanced/find_replace.enaml` & `enaml-0.9.8/examples/layout/advanced/find_replace.enaml`

 * *Files identical despite different names*

### Comparing `enaml-0.9.7/PKG-INFO` & `enaml-0.9.8/enaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: enaml
-Version: 0.9.7
+Version: 0.9.8
 Summary: Declarative DSL for building rich user interfaces in Python
 Home-page: https://github.com/nucleic/enaml
 Author: The Nucleic Development Team
 Author-email: sccolbert@gmail.com
 License: UNKNOWN
 Description: Welcome to Enaml
         ================
```

