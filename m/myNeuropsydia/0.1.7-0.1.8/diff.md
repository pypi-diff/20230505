# Comparing `tmp/myNeuropsydia-0.1.7.tar.gz` & `tmp/myNeuropsydia-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myNeuropsydia-0.1.7.tar", last modified: Thu May  4 18:30:18 2023, max compression
+gzip compressed data, was "myNeuropsydia-0.1.8.tar", last modified: Fri May  5 08:24:06 2023, max compression
```

## Comparing `myNeuropsydia-0.1.7.tar` & `myNeuropsydia-0.1.8.tar`

### file list

```diff
@@ -1,259 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.695376 myNeuropsydia-0.1.7/
--rw-rw-rw-   0        0        0      229 2023-05-04 18:30:18.694377 myNeuropsydia-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      151 2023-05-04 08:12:17.000000 myNeuropsydia-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.103376 myNeuropsydia-0.1.7/myNeuropsydia/
--rw-rw-rw-   0        0        0      330 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.7/myNeuropsydia/__init__.py
--rw-rw-rw-   0        0        0     8399 2023-05-04 09:12:53.000000 myNeuropsydia-0.1.7/myNeuropsydia/ask.py
--rw-rw-rw-   0        0        0    27514 2023-05-04 16:37:28.000000 myNeuropsydia-0.1.7/myNeuropsydia/choice.py
--rw-rw-rw-   0        0        0    27810 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.7/myNeuropsydia/core.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.115378 myNeuropsydia-0.1.7/myNeuropsydia/files/
--rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.157396 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/
--rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/__init__.py
--rw-rw-rw-   0        0        0    51416 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/absorption_desk.png
--rw-rw-rw-   0        0        0    59438 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/absorption_man.png
--rw-rw-rw-   0        0        0   288270 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_absorption.png
--rw-rw-rw-   0        0        0   302887 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_absorption_validated.png
--rw-rw-rw-   0        0        0    47525 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_blue.png
--rw-rw-rw-   0        0        0    49880 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_blue_validated.png
--rw-rw-rw-   0        0        0    43309 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_green.png
--rw-rw-rw-   0        0        0    50122 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_green_validated.png
--rw-rw-rw-   0        0        0    45849 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_orange.png
--rw-rw-rw-   0        0        0    48981 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_orange_validated.png
--rw-rw-rw-   0        0        0    47882 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_purple.png
--rw-rw-rw-   0        0        0    51182 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_purple_validated.png
--rw-rw-rw-   0        0        0    47248 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_red.png
--rw-rw-rw-   0        0        0    44401 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_red_validated.png
--rw-rw-rw-   0        0        0    34927 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_teal.png
--rw-rw-rw-   0        0        0    48362 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_teal_validated.png
--rw-rw-rw-   0        0        0    48420 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_yellow.png
--rw-rw-rw-   0        0        0    47363 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_yellow_validated.png
--rw-rw-rw-   0        0        0    18704 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/scale_point.png
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.175375 myNeuropsydia-0.1.7/myNeuropsydia/files/font/
--rw-rw-rw-   0        0        0   105048 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/LiberationMono-Bold.ttf
--rw-rw-rw-   0        0        0   108168 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/LiberationMono-Regular.ttf
--rw-rw-rw-   0        0        0   164936 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoBlack.ttf
--rw-rw-rw-   0        0        0   163448 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoBold.ttf
--rw-rw-rw-   0        0        0   162636 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoLight.ttf
--rw-rw-rw-   0        0        0   158604 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoRegular.ttf
--rw-rw-rw-   0        0        0    35596 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/Timeless-Bold.ttf
--rw-rw-rw-   0        0        0    61212 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/Timeless.ttf
--rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.198379 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/
--rw-rw-rw-   0        0        0   169046 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/N.png
--rw-rw-rw-   0        0        0   843848 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_HEAD_white.png
--rw-rw-rw-   0        0        0   248442 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_PSY_blue.png
--rw-rw-rw-   0        0        0  4359723 2022-05-03 22:36:13.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_TEXT_white.png
--rw-rw-rw-   0        0        0    70561 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Python.png
--rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/__init__.py
--rw-rw-rw-   0        0        0     1611 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/icon.png
--rw-rw-rw-   0        0        0   827647 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/neuropsydia_banner.png
--rw-rw-rw-   0        0        0     2792 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.7/myNeuropsydia/fill_form.py
--rw-rw-rw-   0        0        0    13763 2023-05-04 17:04:02.000000 myNeuropsydia-0.1.7/myNeuropsydia/image.py
--rw-rw-rw-   0        0        0     3663 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/io.py
--rw-rw-rw-   0        0        0    13500 2023-05-04 18:25:45.000000 myNeuropsydia-0.1.7/myNeuropsydia/meta.py
--rw-rw-rw-   0        0        0    14412 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.7/myNeuropsydia/miscellaneous.py
--rw-rw-rw-   0        0        0      413 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/path.py
--rw-rw-rw-   0        0        0     2801 2023-05-04 09:09:54.000000 myNeuropsydia-0.1.7/myNeuropsydia/procedures.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.238386 myNeuropsydia-0.1.7/myNeuropsydia/pygame/
--rw-rw-rw-   0        0        0    10287 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.242387 myNeuropsydia-0.1.7/myNeuropsydia/pygame/__pyinstaller/
--rw-rw-rw-   0        0        0       72 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0     1367 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/__pyinstaller/hook-pygame.py
--rw-rw-rw-   0        0        0     4386 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/_camera_opencv.py
--rw-rw-rw-   0        0        0     3402 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/_camera_vidcapture.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.244389 myNeuropsydia-0.1.7/myNeuropsydia/pygame/_sdl2/
--rw-rw-rw-   0        0        0      248 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/_sdl2/__init__.py
--rw-rw-rw-   0        0        0     4496 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/camera.py
--rw-rw-rw-   0        0        0    25773 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/colordict.py
--rw-rw-rw-   0        0        0    18203 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/cursors.py
--rw-rw-rw-   0        0        0    18687 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/draw_py.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.320377 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/
--rw-rw-rw-   0        0        0        0 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/__init__.py
--rw-rw-rw-   0        0        0     1034 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/aacircle.py
--rw-rw-rw-   0        0        0    12055 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/aliens.py
--rw-rw-rw-   0        0        0     3633 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/arraydemo.py
--rw-rw-rw-   0        0        0     1563 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/audiocapture.py
--rw-rw-rw-   0        0        0     3425 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/blend_fill.py
--rw-rw-rw-   0        0        0     6345 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/blit_blends.py
--rw-rw-rw-   0        0        0     3028 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/camera.py
--rw-rw-rw-   0        0        0     5910 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/chimp.py
--rw-rw-rw-   0        0        0     2873 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/cursors.py
--rw-rw-rw-   0        0        0     2240 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/dropevent.py
--rw-rw-rw-   0        0        0     5938 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/eventlist.py
--rw-rw-rw-   0        0        0     9841 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/font_viewer.py
--rw-rw-rw-   0        0        0     2080 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/fonty.py
--rw-rw-rw-   0        0        0     3656 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/freetype_misc.py
--rw-rw-rw-   0        0        0    16860 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/glcube.py
--rw-rw-rw-   0        0        0     1301 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/headless_no_windows_needed.py
--rw-rw-rw-   0        0        0     5333 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/joystick.py
--rw-rw-rw-   0        0        0     2541 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/liquid.py
--rw-rw-rw-   0        0        0     5811 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/mask.py
--rw-rw-rw-   0        0        0    29414 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/midi.py
--rw-rw-rw-   0        0        0     1824 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/moveit.py
--rw-rw-rw-   0        0        0     8999 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/music_drop_fade.py
--rw-rw-rw-   0        0        0     3450 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/pixelarray.py
--rw-rw-rw-   0        0        0     5223 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/playmus.py
--rw-rw-rw-   0        0        0     2492 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/prevent_display_stretching.py
--rw-rw-rw-   0        0        0     1046 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/resizing_new.py
--rw-rw-rw-   0        0        0     4866 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/scaletest.py
--rw-rw-rw-   0        0        0     3056 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/scrap_clipboard.py
--rw-rw-rw-   0        0        0     6578 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/scroll.py
--rw-rw-rw-   0        0        0     1801 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/setmodescale.py
--rw-rw-rw-   0        0        0     1172 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/sound.py
--rw-rw-rw-   0        0        0     5797 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/sound_array_demos.py
--rw-rw-rw-   0        0        0     2516 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/sprite_texture.py
--rw-rw-rw-   0        0        0     2762 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/stars.py
--rw-rw-rw-   0        0        0     7001 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/testsprite.py
--rw-rw-rw-   0        0        0     5394 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/textinput.py
--rw-rw-rw-   0        0        0     3277 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/vgrade.py
--rw-rw-rw-   0        0        0     4452 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/video.py
--rw-rw-rw-   0        0        0     1694 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/fastevent.py
--rw-rw-rw-   0        0        0     2216 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/freetype.py
--rw-rw-rw-   0        0        0     6145 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/ftfont.py
--rw-rw-rw-   0        0        0    11638 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/locals.py
--rw-rw-rw-   0        0        0      399 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/macosx.py
--rw-rw-rw-   0        0        0    24398 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/midi.py
--rw-rw-rw-   0        0        0     2445 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/pkgdata.py
--rw-rw-rw-   0        0        0     4083 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/sndarray.py
--rw-rw-rw-   0        0        0    61450 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/sprite.py
--rw-rw-rw-   0        0        0    14424 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/surfarray.py
--rw-rw-rw-   0        0        0    16053 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/sysfont.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.535387 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/
--rw-rw-rw-   0        0        0     1251 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/__init__.py
--rw-rw-rw-   0        0        0     3826 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/__main__.py
--rw-rw-rw-   0        0        0    22634 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/base_test.py
--rw-rw-rw-   0        0        0     4740 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/blit_test.py
--rw-rw-rw-   0        0        0    16511 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/bufferproxy_test.py
--rw-rw-rw-   0        0        0       70 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/camera_test.py
--rw-rw-rw-   0        0        0    47441 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/color_test.py
--rw-rw-rw-   0        0        0     9516 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/constants_test.py
--rw-rw-rw-   0        0        0    10834 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/controller_test.py
--rw-rw-rw-   0        0        0     7700 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/cursors_test.py
--rw-rw-rw-   0        0        0    29009 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/display_test.py
--rw-rw-rw-   0        0        0     1091 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/docs_test.py
--rw-rw-rw-   0        0        0   237007 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/draw_test.py
--rw-rw-rw-   0        0        0    28625 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/event_test.py
--rw-rw-rw-   0        0        0    22605 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/font_test.py
--rw-rw-rw-   0        0        0      182 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/freetype_tags.py
--rw-rw-rw-   0        0        0    64428 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/freetype_test.py
--rw-rw-rw-   0        0        0      180 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/ftfont_tags.py
--rw-rw-rw-   0        0        0      523 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/ftfont_test.py
--rw-rw-rw-   0        0        0    32375 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/gfxdraw_test.py
--rw-rw-rw-   0        0        0     1198 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/image__save_gl_surface_test.py
--rw-rw-rw-   0        0        0      132 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/image_tags.py
--rw-rw-rw-   0        0        0    37989 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/image_test.py
--rw-rw-rw-   0        0        0      135 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/imageext_tags.py
--rw-rw-rw-   0        0        0     2889 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/imageext_test.py
--rw-rw-rw-   0        0        0     6168 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/joystick_test.py
--rw-rw-rw-   0        0        0     4171 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/key_test.py
--rw-rw-rw-   0        0        0   246451 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mask_test.py
--rw-rw-rw-   0        0        0    87928 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/math_test.py
--rw-rw-rw-   0        0        0    16914 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/midi_test.py
--rw-rw-rw-   0        0        0      138 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mixer_music_tags.py
--rw-rw-rw-   0        0        0    13312 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mixer_music_test.py
--rw-rw-rw-   0        0        0      132 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mixer_tags.py
--rw-rw-rw-   0        0        0    43923 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mixer_test.py
--rw-rw-rw-   0        0        0    13149 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mouse_test.py
--rw-rw-rw-   0        0        0    62428 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/pixelarray_test.py
--rw-rw-rw-   0        0        0    25561 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/pixelcopy_test.py
--rw-rw-rw-   0        0        0    75529 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/rect_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.546378 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.590379 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_3_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_4_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_5_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_6_test.py
--rw-rw-rw-   0        0        0      797 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/no_assertions__ret_code_of_1__test.py
--rw-rw-rw-   0        0        0      545 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/zero_tests_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.605378 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/fake_2_test.py
--rw-rw-rw-   0        0        0      909 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/incomplete_todo_test.py
--rw-rw-rw-   0        0        0      859 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/magic_tag_test.py
--rw-rw-rw-   0        0        0      715 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/sleep_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.613378 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/fake_2_test.py
--rw-rw-rw-   0        0        0      925 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/invisible_tag_test.py
--rw-rw-rw-   0        0        0      859 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/magic_tag_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.622377 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_3_test.py
--rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_4_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.628375 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/__init__.py
--rw-rw-rw-   0        0        0      889 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/fake_3_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.633376 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/__init__.py
--rw-rw-rw-   0        0        0      909 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/fake_3_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.641374 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/__init__.py
--rw-rw-rw-   0        0        0      906 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/fake_1_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/fake_2_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.648374 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_2_test.py
--rw-rw-rw-   0        0        0      954 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_3_test.py
--rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_4_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.657376 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_2_test.py
--rw-rw-rw-   0        0        0     1012 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_3_test.py
--rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_4_test.py
--rw-rw-rw-   0        0        0     4342 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/run_tests__test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.664377 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/timeout/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/timeout/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/timeout/fake_2_test.py
--rw-rw-rw-   0        0        0      716 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/timeout/sleep_test.py
--rw-rw-rw-   0        0        0     4323 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/rwobject_test.py
--rw-rw-rw-   0        0        0      671 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/scrap_tags.py
--rw-rw-rw-   0        0        0     9160 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/scrap_test.py
--rw-rw-rw-   0        0        0      190 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sndarray_tags.py
--rw-rw-rw-   0        0        0     6297 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sndarray_test.py
--rw-rw-rw-   0        0        0    46638 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sprite_test.py
--rw-rw-rw-   0        0        0   163734 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surface_test.py
--rw-rw-rw-   0        0        0      260 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surfarray_tags.py
--rw-rw-rw-   0        0        0    25768 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surfarray_test.py
--rw-rw-rw-   0        0        0     4728 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surflock_test.py
--rw-rw-rw-   0        0        0     1463 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sysfont_test.py
--rw-rw-rw-   0        0        0       21 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_test_.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.683378 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/
--rw-rw-rw-   0        0        0     5371 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/__init__.py
--rw-rw-rw-   0        0        0    14843 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/arrinter.py
--rw-rw-rw-   0        0        0     9128 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/async_sub.py
--rw-rw-rw-   0        0        0    23706 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/buftools.py
--rw-rw-rw-   0        0        0      495 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/endian.py
--rw-rw-rw-   0        0        0   152382 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/png.py
--rw-rw-rw-   0        0        0    12049 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/run_tests.py
--rw-rw-rw-   0        0        0     2483 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/test_machinery.py
--rw-rw-rw-   0        0        0     9434 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/test_runner.py
--rw-rw-rw-   0        0        0     7842 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/threads_test.py
--rw-rw-rw-   0        0        0    15336 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/time_test.py
--rw-rw-rw-   0        0        0     3223 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/touch_test.py
--rw-rw-rw-   0        0        0    49044 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/transform_test.py
--rw-rw-rw-   0        0        0     1536 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/version_test.py
--rw-rw-rw-   0        0        0      696 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/video_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.686385 myNeuropsydia-0.1.7/myNeuropsydia/pygame/threads/
--rw-rw-rw-   0        0        0     8074 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/threads/__init__.py
--rw-rw-rw-   0        0        0     2526 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/version.py
--rw-rw-rw-   0        0        0    16381 2023-05-04 09:09:54.000000 myNeuropsydia-0.1.7/myNeuropsydia/scale.py
--rw-rw-rw-   0        0        0     8770 2023-05-04 10:29:19.000000 myNeuropsydia-0.1.7/myNeuropsydia/start.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.691378 myNeuropsydia-0.1.7/myNeuropsydia/tests/
--rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/tests/__init__.py
--rw-rw-rw-   0        0        0      218 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/tests/test_color.py
--rw-rw-rw-   0        0        0     8526 2023-05-04 10:24:43.000000 myNeuropsydia-0.1.7/myNeuropsydia/write.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.113377 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/
--rw-rw-rw-   0        0        0      229 2023-05-04 18:30:17.000000 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10661 2023-05-04 18:30:17.000000 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       62 2023-05-04 18:30:17.000000 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-04 18:30:17.000000 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-04 18:30:17.000000 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 18:30:18.695376 myNeuropsydia-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-05-04 18:30:03.000000 myNeuropsydia-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:24:06.943240 myNeuropsydia-0.1.8/
+-rw-rw-rw-   0        0        0      281 2023-05-05 08:24:06.942243 myNeuropsydia-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2022-04-19 16:08:20.000000 myNeuropsydia-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 08:24:06.908334 myNeuropsydia-0.1.8/myNeuropsydia/
+-rw-rw-rw-   0        0        0      330 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/__init__.py
+-rw-rw-rw-   0        0        0     8399 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/ask.py
+-rw-rw-rw-   0        0        0    27514 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/choice.py
+-rw-rw-rw-   0        0        0    27810 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/core.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:24:06.912322 myNeuropsydia-0.1.8/myNeuropsydia/files/
+-rw-rw-rw-   0        0        0       30 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:24:06.925288 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/
+-rw-rw-rw-   0        0        0       30 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/__init__.py
+-rw-rw-rw-   0        0        0    51416 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/absorption_desk.png
+-rw-rw-rw-   0        0        0    59438 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/absorption_man.png
+-rw-rw-rw-   0        0        0   288270 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_absorption.png
+-rw-rw-rw-   0        0        0   302887 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_absorption_validated.png
+-rw-rw-rw-   0        0        0    47525 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_blue.png
+-rw-rw-rw-   0        0        0    49880 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_blue_validated.png
+-rw-rw-rw-   0        0        0    43309 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_green.png
+-rw-rw-rw-   0        0        0    50122 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_green_validated.png
+-rw-rw-rw-   0        0        0    45849 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_orange.png
+-rw-rw-rw-   0        0        0    48981 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_orange_validated.png
+-rw-rw-rw-   0        0        0    47882 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_purple.png
+-rw-rw-rw-   0        0        0    51182 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_purple_validated.png
+-rw-rw-rw-   0        0        0    47248 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_red.png
+-rw-rw-rw-   0        0        0    44401 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_red_validated.png
+-rw-rw-rw-   0        0        0    34927 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_teal.png
+-rw-rw-rw-   0        0        0    48362 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_teal_validated.png
+-rw-rw-rw-   0        0        0    48420 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_yellow.png
+-rw-rw-rw-   0        0        0    47363 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_yellow_validated.png
+-rw-rw-rw-   0        0        0    18704 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/binary/scale_point.png
+drwxrwxrwx   0        0        0        0 2023-05-05 08:24:06.931272 myNeuropsydia-0.1.8/myNeuropsydia/files/font/
+-rw-rw-rw-   0        0        0   105048 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/font/LiberationMono-Bold.ttf
+-rw-rw-rw-   0        0        0   108168 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/font/LiberationMono-Regular.ttf
+-rw-rw-rw-   0        0        0   164936 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/font/RobotoBlack.ttf
+-rw-rw-rw-   0        0        0   163448 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/font/RobotoBold.ttf
+-rw-rw-rw-   0        0        0   162636 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/font/RobotoLight.ttf
+-rw-rw-rw-   0        0        0   158604 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/font/RobotoRegular.ttf
+-rw-rw-rw-   0        0        0    35596 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/font/Timeless-Bold.ttf
+-rw-rw-rw-   0        0        0    61212 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/font/Timeless.ttf
+-rw-rw-rw-   0        0        0       30 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:24:06.940248 myNeuropsydia-0.1.8/myNeuropsydia/files/logo/
+-rw-rw-rw-   0        0        0   169046 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/logo/N.png
+-rw-rw-rw-   0        0        0   843848 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/logo/Neuropsydia_HEAD_white.png
+-rw-rw-rw-   0        0        0   248442 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/logo/Neuropsydia_PSY_blue.png
+-rw-rw-rw-   0        0        0  4359723 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/logo/Neuropsydia_TEXT_white.png
+-rw-rw-rw-   0        0        0    70561 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/logo/Python.png
+-rw-rw-rw-   0        0        0       30 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/logo/__init__.py
+-rw-rw-rw-   0        0        0     1611 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/logo/icon.png
+-rw-rw-rw-   0        0        0   827647 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/files/logo/neuropsydia_banner.png
+-rw-rw-rw-   0        0        0     2792 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/fill_form.py
+-rw-rw-rw-   0        0        0    13763 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/image.py
+-rw-rw-rw-   0        0        0     3663 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/io.py
+-rw-rw-rw-   0        0        0    13500 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/meta.py
+-rw-rw-rw-   0        0        0    14412 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/miscellaneous.py
+-rw-rw-rw-   0        0        0      413 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/path.py
+-rw-rw-rw-   0        0        0     2801 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/procedures.py
+-rw-rw-rw-   0        0        0    16381 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/scale.py
+-rw-rw-rw-   0        0        0     8770 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/start.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:24:06.942243 myNeuropsydia-0.1.8/myNeuropsydia/tests/
+-rw-rw-rw-   0        0        0       30 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/tests/__init__.py
+-rw-rw-rw-   0        0        0      218 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/tests/test_color.py
+-rw-rw-rw-   0        0        0     8526 2023-05-05 08:21:10.000000 myNeuropsydia-0.1.8/myNeuropsydia/write.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:24:06.911325 myNeuropsydia-0.1.8/myNeuropsydia.egg-info/
+-rw-rw-rw-   0        0        0      281 2023-05-05 08:24:06.000000 myNeuropsydia-0.1.8/myNeuropsydia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2326 2023-05-05 08:24:06.000000 myNeuropsydia-0.1.8/myNeuropsydia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       62 2023-05-05 08:24:06.000000 myNeuropsydia-0.1.8/myNeuropsydia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-05-05 08:24:06.000000 myNeuropsydia-0.1.8/myNeuropsydia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-05 08:24:06.000000 myNeuropsydia-0.1.8/myNeuropsydia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:24:06.943240 myNeuropsydia-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-05-05 08:23:28.000000 myNeuropsydia-0.1.8/setup.py
```

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/ask.py` & `myNeuropsydia-0.1.8/myNeuropsydia/ask.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/choice.py` & `myNeuropsydia-0.1.8/myNeuropsydia/choice.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/core.py` & `myNeuropsydia-0.1.8/myNeuropsydia/core.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/absorption_desk.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/absorption_desk.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/absorption_man.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/absorption_man.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_absorption.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_absorption.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_absorption_validated.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_absorption_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_blue.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_blue.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_blue_validated.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_blue_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_green.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_green.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_green_validated.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_green_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_orange.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_orange.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_orange_validated.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_orange_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_purple.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_purple.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_purple_validated.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_purple_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_red.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_red.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_red_validated.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_red_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_teal.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_teal.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_teal_validated.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_teal_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_yellow.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_yellow.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_yellow_validated.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/cursor_yellow_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/scale_point.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/binary/scale_point.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/font/LiberationMono-Bold.ttf` & `myNeuropsydia-0.1.8/myNeuropsydia/files/font/LiberationMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/font/LiberationMono-Regular.ttf` & `myNeuropsydia-0.1.8/myNeuropsydia/files/font/LiberationMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoBlack.ttf` & `myNeuropsydia-0.1.8/myNeuropsydia/files/font/RobotoBlack.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoBold.ttf` & `myNeuropsydia-0.1.8/myNeuropsydia/files/font/RobotoBold.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoLight.ttf` & `myNeuropsydia-0.1.8/myNeuropsydia/files/font/RobotoLight.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoRegular.ttf` & `myNeuropsydia-0.1.8/myNeuropsydia/files/font/RobotoRegular.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/font/Timeless-Bold.ttf` & `myNeuropsydia-0.1.8/myNeuropsydia/files/font/Timeless-Bold.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/font/Timeless.ttf` & `myNeuropsydia-0.1.8/myNeuropsydia/files/font/Timeless.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/N.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/logo/N.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_HEAD_white.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/logo/Neuropsydia_HEAD_white.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_PSY_blue.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/logo/Neuropsydia_PSY_blue.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_TEXT_white.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/logo/Neuropsydia_TEXT_white.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Python.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/logo/Python.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/icon.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/logo/icon.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/neuropsydia_banner.png` & `myNeuropsydia-0.1.8/myNeuropsydia/files/logo/neuropsydia_banner.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/fill_form.py` & `myNeuropsydia-0.1.8/myNeuropsydia/fill_form.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/image.py` & `myNeuropsydia-0.1.8/myNeuropsydia/image.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/io.py` & `myNeuropsydia-0.1.8/myNeuropsydia/io.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/meta.py` & `myNeuropsydia-0.1.8/myNeuropsydia/meta.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/miscellaneous.py` & `myNeuropsydia-0.1.8/myNeuropsydia/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/procedures.py` & `myNeuropsydia-0.1.8/myNeuropsydia/procedures.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/scale.py` & `myNeuropsydia-0.1.8/myNeuropsydia/scale.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/start.py` & `myNeuropsydia-0.1.8/myNeuropsydia/start.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/myNeuropsydia/write.py` & `myNeuropsydia-0.1.8/myNeuropsydia/write.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.7/setup.py` & `myNeuropsydia-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import find_packages, setup
 
 setup(
     name='myNeuropsydia',
     packages=find_packages(),
-    version='0.1.7',
+    version='0.1.8',
     description='Partially fixed version of Neuropsydia library, a Python module for creating experiments, tasks and questionnaires',
     author='Laborde',
     license='ENS_Paris_Saclay',
     package_data = {
                 	"myNeuropsydia.files.font":["*.ttf", "*.otf"],
                 	"myNeuropsydia.files.binary":["*.png"],
                 	"myNeuropsydia.files.logo":["*.png"]},
     dependency_links=[
 	"https://github.com/neuropsychology/NeuroKit.py/zipball/master"],
     install_requires=['Pillow',
-                      'cryptography', 
+                      'cryptography',
+                      'neurokit',
                       'numpy',
-                      'pandas', 
+                      'pandas',
+                      'pygame',
                       'python-docx',
                       'pyxid',
                       'statsmodels'],
 )
+
+
```

