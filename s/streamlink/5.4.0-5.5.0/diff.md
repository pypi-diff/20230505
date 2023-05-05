# Comparing `tmp/streamlink-5.4.0.tar.gz` & `tmp/streamlink-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlink-5.4.0.tar", last modified: Wed Apr 12 18:44:03 2023, max compression
+gzip compressed data, was "streamlink-5.5.0.tar", last modified: Fri May  5 04:21:56 2023, max compression
```

## Comparing `streamlink-5.4.0.tar` & `streamlink-5.5.0.tar`

### file list

```diff
@@ -1,571 +1,575 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.087135 streamlink-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 18:43:13.000000 streamlink-5.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    74305 2023-04-12 18:43:13.000000 streamlink-5.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-12 18:43:13.000000 streamlink-5.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 18:43:13.000000 streamlink-5.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-12 18:44:03.087135 streamlink-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-12 18:43:13.000000 streamlink-5.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.983133 streamlink-5.4.0/completions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.987133 streamlink-5.4.0/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-12 18:43:49.000000 streamlink-5.4.0/completions/bash/streamlink
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.987133 streamlink-5.4.0/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-04-12 18:43:49.000000 streamlink-5.4.0/completions/zsh/_streamlink
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 18:43:13.000000 streamlink-5.4.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.991133 streamlink-5.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_applications.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.983133 streamlink-5.4.0/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.991133 streamlink-5.4.0/docs/_build/man/
--rw-r--r--   0 runner    (1001) docker     (123)    37413 2023-04-12 18:43:54.000000 streamlink-5.4.0/docs/_build/man/streamlink.1
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_man.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/icon-ffmpeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/icon-python.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/opengraph-image.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/styles/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/_templates/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_templates/sidebar/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_templates/sidebar/github-buttons.html
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/api_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/applications.rst
--rw-r--r--   0 runner    (1001) docker     (123)    74305 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/plugin-sideloading.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/plugins/crunchyroll.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/plugins/twitch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/protocols.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/proxy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/deprecations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/donate.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/ext_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/ext_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/ext_html_template_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/ext_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/ext_releaseref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23921 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/issues.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/players.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/thirdparty.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-04-12 18:43:13.000000 streamlink-5.4.0/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-12 18:43:13.000000 streamlink-5.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-12 18:44:03.091135 streamlink-5.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-12 18:43:13.000000 streamlink-5.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.983133 streamlink-5.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.091135 streamlink-5.4.0/src/streamlink/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-12 18:44:03.091135 streamlink-5.4.0/src/streamlink/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.999133 streamlink-5.4.0/src/streamlink/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/packages/requests_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.003133 streamlink-5.4.0/src/streamlink/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.003133 streamlink-5.4.0/src/streamlink/plugin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/useragents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.003133 streamlink-5.4.0/src/streamlink/plugin/api/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/validate/_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/validate/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/validate/_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/validate/_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.035134 streamlink-5.4.0/src/streamlink/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/abematv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/adultswim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/afreeca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/albavision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/aloula.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/app17.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ard_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/artetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/bigo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/blazetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/booyah.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/brightcove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/btv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/cnews.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/delfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/dlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/dogan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/dogus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/drdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/earthcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/euronews.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/filmon.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/foxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/goodgame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/gulli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/hls.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/htv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/huajiao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/huya.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/idf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/indihometv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/invintus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/kugou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/linelive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mildom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mitele.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/n13tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nicolive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nimotv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nownews.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ntv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/okru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/onetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/openrectv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/pandalive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/picarto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/piczel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/pluto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/pluzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/qq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/radiko.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/radionet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/raiplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/reuters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/rtbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/rtpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/rtve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/rtvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ruv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/showroom.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/sportal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/sportschau.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ssh101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/stadium.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/streann.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/stv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/svtplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/telefe.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/trovo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv360.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv4play.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv999.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tvibo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tvrby.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vidio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vkplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/wasd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/webtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/welt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/yupptv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/zattoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/zeenews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/zengatv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/zhanqi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25641 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.035134 streamlink-5.4.0/src/streamlink/stream/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)    34203 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/dash_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)    31062 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/hls.py
--rw-r--r--   0 runner    (1001) docker     (123)    20608 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/hls_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/segmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.039134 streamlink-5.4.0/src/streamlink/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/l10n.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/processoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.999133 streamlink-5.4.0/src/streamlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16363 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.039134 streamlink-5.4.0/src/streamlink_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43909 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32194 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.043134 streamlink-5.4.0/src/streamlink_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/player.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/versioncheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.047134 streamlink-5.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.047134 streamlink-5.4.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.047134 streamlink-5.4.0/tests/cli/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/output/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/output/test_playeroutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_cmdline_player_fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_cmdline_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    38201 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_main_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_main_setup_config_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    23237 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.047134 streamlink-5.4.0/tests/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/utils/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/utils/test_versioncheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.051134 streamlink-5.4.0/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/mixins/stream_hls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.051134 streamlink-5.4.0/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.051134 streamlink-5.4.0/tests/plugin/override/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugin/override/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugin/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugin/testplugin_invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugin/testplugin_missing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.079135 streamlink-5.4.0/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_abematv.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_adultswim.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_afreeca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_albavision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_aloula.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_app17.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ard_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_artetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_bigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_blazetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_booyah.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_brightcove.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_btv.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_cnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_delfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_dlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_dogan.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_dogus.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_drdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_earthcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_euronews.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_filmon.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_foxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_goodgame.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_gulli.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_htv.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_huajiao.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_huya.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_idf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_indihometv.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_invintus.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_kugou.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_linelive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mildom.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mitele.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_n13tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nicolive.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nimotv.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nos.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nownews.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ntv.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_okru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_onetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_openrectv.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_pandalive.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_picarto.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_piczel.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_pluto.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_pluzz.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_qq.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_radiko.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_radionet.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_raiplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_reuters.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_rtbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_rtpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_rtve.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_rtvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ruv.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_showroom.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_sportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_sportschau.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ssh101.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_stadium.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_streann.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_stv.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_svtplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_telefe.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_trovo.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv360.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv4play.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv8.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv999.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tvibo.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tvp.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tvrby.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vidio.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vk.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vkplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_wasd.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_webtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_welt.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_yupptv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_zattoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_zeenews.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_zengatv.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_zhanqi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.079135 streamlink-5.4.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.983133 streamlink-5.4.0/tests/resources/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.079135 streamlink-5.4.0/tests/resources/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/cli/config/custom
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/cli/config/primary
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/cli/config/primary.testplugin
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/cli/config/secondary
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/cli/config/secondary.testplugin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.083135 streamlink-5.4.0/tests/resources/dash/
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_1.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_10.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_11_static.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_2.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_3.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_8.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_9.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_nested_baseurls.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_no_segment_list_or_template.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_segment_list.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_segments_byterange.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_segments_dynamic_number.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_static_no_publish_time.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_timeline_ids.mpd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.083135 streamlink-5.4.0/tests/resources/hls/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/hls/test_1.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/hls/test_2.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/hls/test_date.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/hls/test_master.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/hls/test_master_twitch_vod.m3u8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.087135 streamlink-5.4.0/tests/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_dash_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    29307 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_hls_filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_hls_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_stream_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_stream_to_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_stream_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_api_http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    48733 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_api_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_api_websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_plugin_userinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_streamlink_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.087135 streamlink-5.4.0/tests/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/testutils/handshake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/testutils/test_handshake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.087135 streamlink-5.4.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_l10n.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_processoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.609623 streamlink-5.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 04:20:47.000000 streamlink-5.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    75451 2023-05-05 04:20:47.000000 streamlink-5.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-05 04:20:47.000000 streamlink-5.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-05 04:20:47.000000 streamlink-5.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-05 04:21:56.609623 streamlink-5.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-05 04:20:47.000000 streamlink-5.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.493620 streamlink-5.5.0/completions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.497620 streamlink-5.5.0/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-05-05 04:21:38.000000 streamlink-5.5.0/completions/bash/streamlink
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.501620 streamlink-5.5.0/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)    33215 2023-05-05 04:21:39.000000 streamlink-5.5.0/completions/zsh/_streamlink
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 04:20:47.000000 streamlink-5.5.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.505620 streamlink-5.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_applications.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.493620 streamlink-5.5.0/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.505620 streamlink-5.5.0/docs/_build/man/
+-rw-r--r--   0 runner    (1001) docker     (123)    37912 2023-05-05 04:21:45.000000 streamlink-5.5.0/docs/_build/man/streamlink.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_man.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.505620 streamlink-5.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/icon-ffmpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/icon-python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/opengraph-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.505620 streamlink-5.5.0/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/styles/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.505620 streamlink-5.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.509620 streamlink-5.5.0/docs/_templates/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_templates/sidebar/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_templates/sidebar/github-buttons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/api_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/applications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    75451 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.509620 streamlink-5.5.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/plugin-sideloading.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.509620 streamlink-5.5.0/docs/cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/plugins/crunchyroll.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/plugins/twitch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/protocols.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/deprecations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/donate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/ext_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/ext_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/ext_html_template_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/ext_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/ext_releaseref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24181 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/players.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/thirdparty.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-05 04:20:47.000000 streamlink-5.5.0/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-05 04:20:47.000000 streamlink-5.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-05 04:21:56.609623 streamlink-5.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-05 04:20:47.000000 streamlink-5.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.493620 streamlink-5.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.613623 streamlink-5.5.0/src/streamlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-05 04:21:56.613623 streamlink-5.5.0/src/streamlink/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.513620 streamlink-5.5.0/src/streamlink/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/packages/requests_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.513620 streamlink-5.5.0/src/streamlink/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.517620 streamlink-5.5.0/src/streamlink/plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/http_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/useragents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.517620 streamlink-5.5.0/src/streamlink/plugin/api/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/validate/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/validate/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/validate/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/validate/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.549621 streamlink-5.5.0/src/streamlink/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/abematv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/albavision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/aloula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/app17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/artetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/bigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/booyah.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/btv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/cnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/delfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/dlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/dogan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/dogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/drdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/euronews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/filmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/foxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/gulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/htv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/idf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/invintus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/kugou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/linelive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mildom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mitele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nownews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ntv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/okru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/onetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/picarto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/piczel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/pluto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/radiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/radionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/reuters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/rtbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/rtve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ruv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/showroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/sportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/stadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/streann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/stv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/telefe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/trovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv360.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv999.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vidio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/wasd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/webtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/welt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/zhanqi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25474 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.549621 streamlink-5.5.0/src/streamlink/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34203 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/dash_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31062 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20611 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/hls_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/segmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.553622 streamlink-5.5.0/src/streamlink/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/l10n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.513620 streamlink-5.5.0/src/streamlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.553622 streamlink-5.5.0/src/streamlink_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44541 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32105 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.557622 streamlink-5.5.0/src/streamlink_cli/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/output/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/output/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/output/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/output/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.557622 streamlink-5.5.0/src/streamlink_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/versioncheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.561622 streamlink-5.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.561622 streamlink-5.5.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.561622 streamlink-5.5.0/tests/cli/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/output/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/output/test_playeroutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_cmdline_player_fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_cmdline_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38283 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_main_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_main_setup_config_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.565622 streamlink-5.5.0/tests/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/utils/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/utils/test_versioncheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.565622 streamlink-5.5.0/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/mixins/stream_hls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.565622 streamlink-5.5.0/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.565622 streamlink-5.5.0/tests/plugin/override/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugin/override/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugin/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugin/testplugin_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugin/testplugin_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.597623 streamlink-5.5.0/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_abematv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_albavision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_aloula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_app17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_artetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_bigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_booyah.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_btv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_cnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_delfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_dlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_dogan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_dogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_drdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_euronews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_filmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_foxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_gulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_htv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_idf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_invintus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_kugou.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_linelive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mildom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mitele.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nownews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ntv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_okru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_onetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_picarto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_piczel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_pluto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_radiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_radionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_reuters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_rtbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_rtve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ruv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_showroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_sportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_stadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_streann.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_stv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_telefe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_trovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv360.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv999.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vidio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_wasd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_webtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_welt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_zhanqi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.597623 streamlink-5.5.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.497620 streamlink-5.5.0/tests/resources/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.601623 streamlink-5.5.0/tests/resources/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/cli/config/custom
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/cli/config/primary
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/cli/config/primary.testplugin
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/cli/config/secondary
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/cli/config/secondary.testplugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.601623 streamlink-5.5.0/tests/resources/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_1.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_10.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_11_static.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_2.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_3.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_8.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_9.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_nested_baseurls.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_no_segment_list_or_template.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_segment_list.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_segments_byterange.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_segments_dynamic_number.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_static_no_publish_time.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_timeline_ids.mpd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.605623 streamlink-5.5.0/tests/resources/hls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/hls/test_1.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/hls/test_2.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/hls/test_date.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/hls/test_master.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/hls/test_master_twitch_vod.m3u8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.605623 streamlink-5.5.0/tests/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_dash_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29307 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_hls_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18847 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_hls_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_stream_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_stream_to_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_stream_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_api_http_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48733 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_api_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_api_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_plugin_userinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_streamlink_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.609623 streamlink-5.5.0/tests/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/testutils/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/testutils/test_handshake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.609623 streamlink-5.5.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_l10n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_url.py
```

### Comparing `streamlink-5.4.0/CHANGELOG.md` & `streamlink-5.5.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## streamlink 5.5.0 (2023-05-05)
+
+Release highlights:
+
+- Added: `--no-config` ([#5314](https://github.com/streamlink/streamlink/pull/5314))
+- Added: `--player-external-http-interface` ([#5295](https://github.com/streamlink/streamlink/pull/5295))
+- Fixed: M3U8 attribute parsing issue ([#5307](https://github.com/streamlink/streamlink/pull/5307))
+- Fixed: various minor plugin issues ([#5291](https://github.com/streamlink/streamlink/pull/5291), [#5299](https://github.com/streamlink/streamlink/pull/5299), [#5306](https://github.com/streamlink/streamlink/pull/5306))
+- Build: bumped urllib3 to `>=1.26.0,<3` and fixed compatibility issues with `urllib3 >=2.0.0` ([#5326](https://github.com/streamlink/streamlink/pull/5326), [#5325](https://github.com/streamlink/streamlink/pull/5325))
+- Docs: bumped furo theme to `2023.03.27` ([#5301](https://github.com/streamlink/streamlink/pull/5301))
+- Docs: bumped build dependencies `sphinx >=5.0.0,<7`, `myst-parser >=1.0.0,<2` and `sphinx-design >=0.4.1,<1` ([#5301](https://github.com/streamlink/streamlink/pull/5301))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/5.4.0...5.5.0)
+
+
 ## streamlink 5.4.0 (2023-04-12)
 
 Release highlights:
 
 - Added: `--progress` CLI argument and [deprecated `--force-progress`](https://streamlink.github.io/deprecations.html#deprecation-of-force-progress) ([#5268](https://github.com/streamlink/streamlink/pull/5268))
 - Added: `--dash-manifest-reload-attempts` and respective session option ([#5208](https://github.com/streamlink/streamlink/pull/5208))
 - Improved: DASH segment availability/download logging ([#5214](https://github.com/streamlink/streamlink/pull/5214), [#5235](https://github.com/streamlink/streamlink/pull/5235))
```

### Comparing `streamlink-5.4.0/LICENSE` & `streamlink-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/PKG-INFO` & `streamlink-5.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 5.4.0
+Version: 5.5.0
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Home-page: https://github.com/streamlink/streamlink
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 5.4.0 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 5.5.0 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Home-page: https://github.com/streamlink/
 streamlink Author: Streamlink Author-email: streamlink@protonmail.com License:
 Simplified BSD Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues Project-
 URL: Source, https://github.com/streamlink/streamlink Project-URL: Funding,
 https://streamlink.github.io/latest/donate.html Classifier: Development Status
```

### Comparing `streamlink-5.4.0/README.md` & `streamlink-5.5.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/completions/bash/streamlink` & `streamlink-5.5.0/completions/bash/streamlink`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # AUTOMATICALLY GENERATED by `shtab`
 
 
 
-_shtab_streamlink_cli_option_strings=('-h' '--help' '-V' '--version' '--plugins' '--plugin-dirs' '--can-handle-url' '--can-handle-url-no-redirect' '--config' '-l' '--loglevel' '--logfile' '-Q' '--quiet' '-j' '--json' '--auto-version-check' '--version-check' '--locale' '--interface' '-4' '--ipv4' '-6' '--ipv6' '-p' '--player' '-a' '--player-args' '-v' '--verbose-player' '-n' '--player-fifo' '--fifo' '--player-http' '--player-continuous-http' '--player-external-http' '--player-external-http-continuous' '--player-external-http-port' '--player-passthrough' '--player-no-close' '-t' '--title' '-o' '--output' '-O' '--stdout' '-r' '--record' '-R' '--record-and-pipe' '--fs-safe-rules' '-f' '--force' '--progress' '--force-progress' '--url' '--default-stream' '--stream-url' '--retry-streams' '--retry-max' '--retry-open' '--stream-types' '--stream-priority' '--stream-sorting-excludes' '--ringbuffer-size' '--stream-segment-attempts' '--stream-segment-threads' '--stream-segment-timeout' '--stream-timeout' '--mux-subtitles' '--hls-live-edge' '--hls-segment-stream-data' '--hls-playlist-reload-attempts' '--hls-playlist-reload-time' '--hls-segment-ignore-names' '--hls-segment-key-uri' '--hls-audio-select' '--hls-start-offset' '--hls-duration' '--hls-live-restart' '--dash-manifest-reload-attempts' '--ffmpeg-ffmpeg' '--ffmpeg-no-validation' '--ffmpeg-verbose' '--ffmpeg-verbose-path' '--ffmpeg-fout' '--ffmpeg-video-transcode' '--ffmpeg-audio-transcode' '--ffmpeg-copyts' '--ffmpeg-start-at-zero' '--http-proxy' '--http-cookie' '--http-header' '--http-query-param' '--http-ignore-env' '--http-no-ssl-verify' '--http-disable-dh' '--http-ssl-cert' '--http-ssl-cert-crt-key' '--http-timeout' '--afreeca-username' '--afreeca-password' '--afreeca-purge-credentials' '--bbciplayer-username' '--bbciplayer-password' '--bbciplayer-hd' '--clubbingtv-username' '--clubbingtv-password' '--crunchyroll-username' '--crunchyroll-password' '--crunchyroll-purge-credentials' '--crunchyroll-session-id' '--niconico-email' '--niconico-password' '--niconico-user-session' '--niconico-purge-credentials' '--niconico-timeshift-offset' '--openrectv-email' '--openrectv-password' '--pixiv-sessionid' '--pixiv-devicetoken' '--pixiv-purge-credentials' '--pixiv-performer' '--steam-email' '--steam-password' '--streann-url' '--twitcasting-password' '--twitch-disable-ads' '--twitch-disable-reruns' '--twitch-low-latency' '--twitch-api-header' '--twitch-access-token-param' '--ustream-password' '--ustvnow-username' '--ustvnow-password' '--wwenetwork-email' '--wwenetwork-password' '--yupptv-boxid' '--yupptv-yuppflixtoken' '--yupptv-purge-credentials' '--zattoo-email' '--zattoo-password' '--zattoo-purge-credentials' '--zattoo-stream-types')
+_shtab_streamlink_cli_option_strings=('-h' '--help' '-V' '--version' '--plugins' '--plugin-dirs' '--can-handle-url' '--can-handle-url-no-redirect' '--config' '--no-config' '-l' '--loglevel' '--logfile' '-Q' '--quiet' '-j' '--json' '--auto-version-check' '--version-check' '--locale' '--interface' '-4' '--ipv4' '-6' '--ipv6' '-p' '--player' '-a' '--player-args' '-v' '--verbose-player' '-n' '--player-fifo' '--fifo' '--player-http' '--player-continuous-http' '--player-external-http' '--player-external-http-continuous' '--player-external-http-interface' '--player-external-http-port' '--player-passthrough' '--player-no-close' '-t' '--title' '-o' '--output' '-O' '--stdout' '-r' '--record' '-R' '--record-and-pipe' '--fs-safe-rules' '-f' '--force' '--progress' '--force-progress' '--url' '--default-stream' '--stream-url' '--retry-streams' '--retry-max' '--retry-open' '--stream-types' '--stream-priority' '--stream-sorting-excludes' '--ringbuffer-size' '--stream-segment-attempts' '--stream-segment-threads' '--stream-segment-timeout' '--stream-timeout' '--mux-subtitles' '--hls-live-edge' '--hls-segment-stream-data' '--hls-playlist-reload-attempts' '--hls-playlist-reload-time' '--hls-segment-ignore-names' '--hls-segment-key-uri' '--hls-audio-select' '--hls-start-offset' '--hls-duration' '--hls-live-restart' '--dash-manifest-reload-attempts' '--ffmpeg-ffmpeg' '--ffmpeg-no-validation' '--ffmpeg-verbose' '--ffmpeg-verbose-path' '--ffmpeg-fout' '--ffmpeg-video-transcode' '--ffmpeg-audio-transcode' '--ffmpeg-copyts' '--ffmpeg-start-at-zero' '--http-proxy' '--http-cookie' '--http-header' '--http-query-param' '--http-ignore-env' '--http-no-ssl-verify' '--http-disable-dh' '--http-ssl-cert' '--http-ssl-cert-crt-key' '--http-timeout' '--afreeca-username' '--afreeca-password' '--afreeca-purge-credentials' '--bbciplayer-username' '--bbciplayer-password' '--bbciplayer-hd' '--clubbingtv-username' '--clubbingtv-password' '--crunchyroll-username' '--crunchyroll-password' '--crunchyroll-purge-credentials' '--crunchyroll-session-id' '--niconico-email' '--niconico-password' '--niconico-user-session' '--niconico-purge-credentials' '--niconico-timeshift-offset' '--openrectv-email' '--openrectv-password' '--pixiv-sessionid' '--pixiv-devicetoken' '--pixiv-purge-credentials' '--pixiv-performer' '--steam-email' '--steam-password' '--streann-url' '--twitcasting-password' '--twitch-disable-ads' '--twitch-disable-reruns' '--twitch-low-latency' '--twitch-api-header' '--twitch-access-token-param' '--ustream-password' '--ustvnow-username' '--ustvnow-password' '--wwenetwork-email' '--wwenetwork-password' '--yupptv-boxid' '--yupptv-yuppflixtoken' '--yupptv-purge-credentials' '--zattoo-email' '--zattoo-password' '--zattoo-purge-credentials' '--zattoo-stream-types')
 
 
 
 _shtab_streamlink_cli__l_choices=('none' 'critical' 'error' 'warning' 'info' 'debug' 'trace' 'all')
 _shtab_streamlink_cli___loglevel_choices=('none' 'critical' 'error' 'warning' 'info' 'debug' 'trace' 'all')
 _shtab_streamlink_cli___fs_safe_rules_choices=('POSIX' 'Windows')
 _shtab_streamlink_cli___progress_choices=('yes' 'force' 'no')
 
 _shtab_streamlink_cli__h_nargs=0
 _shtab_streamlink_cli___help_nargs=0
 _shtab_streamlink_cli__V_nargs=0
 _shtab_streamlink_cli___version_nargs=0
 _shtab_streamlink_cli___plugins_nargs=0
+_shtab_streamlink_cli___no_config_nargs=0
 _shtab_streamlink_cli__Q_nargs=0
 _shtab_streamlink_cli___quiet_nargs=0
 _shtab_streamlink_cli__j_nargs=0
 _shtab_streamlink_cli___json_nargs=0
 _shtab_streamlink_cli___version_check_nargs=0
 _shtab_streamlink_cli__4_nargs=0
 _shtab_streamlink_cli___ipv4_nargs=0
```

### Comparing `streamlink-5.4.0/completions/zsh/_streamlink` & `streamlink-5.5.0/completions/zsh/_streamlink`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,17 @@
         ]:can_handle_url_no_redirect:"
   "*--config[
         Load options from this config file.
 
         Can be repeated to load multiple files, in which case the options are
         merged on top of each other where the last config has highest priority.
         ]:config:"
+  "--no-config[
+        Disable loading any default or custom config files.
+        ]"
   {-l,--loglevel}"[
         Set the log message threshold.
 
         Valid levels are, in order of increasing verbosity\:
 
         \`none\`, \`critical\`, \`error\`, \`warning\`, \`info\`, \`debug\`, \`trace\`, \`all\`
 
@@ -186,14 +189,17 @@
         useful to allow external devices like smartphones or streaming boxes to
         watch streams they wouldn\'t be able to otherwise.
 
         The default behavior is similar to the --player-continuous-http option,
         but no player program will be started, and the server will listen on all available
         connections instead of just in the local (loopback) interface.
 
+        See --player-external-http-interface for choosing a specific network interface, and
+        see --player-external-http-port for choosing a non-randomized port.
+
         Optionally, the --player-external-http-continuous option allows for disabling
         the continuous run-mode, so that Streamlink will stop when the stream ends.
 
         The URLs that can be used to access the stream will be printed to the
         console, and the server can be interrupted using CTRL-C.
         ]"
   "--player-external-http-continuous[
@@ -202,14 +208,18 @@
         In the continuous run-mode, Streamlink will keep running after the stream has ended
         and will wait for the next HTTP request being made unless it gets shut down via CTRL-C.
 
         If set to non-continuous, Streamlink will stop once the stream has ended.
 
         Default is true.
         ]:player_external_http_continuous:"
+  "--player-external-http-interface[
+        The network interface on which the HTTP server will be listening on.
+        If unset or set to \`0.0.0.0\`, all available interfaces will be bound.
+        ]:player_external_http_interface:"
   "--player-external-http-port[
         A fixed port to use for the external HTTP server if that mode is
         enabled. Omit or set to \`0\` to use a random high ( \>1024) port.
         ]:player_external_http_port:"
   "--player-passthrough[
         A comma-delimited list of stream types to pass to the player as a URL to
         let it handle the transport of the stream instead.
```

### Comparing `streamlink-5.4.0/docs/Makefile` & `streamlink-5.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_build/man/streamlink.1` & `streamlink-5.5.0/docs/_build/man/streamlink.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "STREAMLINK" "1" "Apr 12, 2023" "5.4.0" "Streamlink"
+.TH "STREAMLINK" "1" "May 05, 2023" "5.5.0" "Streamlink"
 .SH NAME
 streamlink \- extracts streams from various services and pipes them into a video player of choice
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -142,14 +142,19 @@
 Load options from this config file.
 .sp
 Can be repeated to load multiple files, in which case the options are
 merged on top of each other where the last config has highest priority.
 .UNINDENT
 .INDENT 0.0
 .TP
+.B \-\-no\-config
+Disable loading any default or custom config files.
+.UNINDENT
+.INDENT 0.0
+.TP
 .B \-l LEVEL
 .TP
 .B \-\-loglevel LEVEL
 Set the log message threshold.
 .sp
 Valid levels are, in order of increasing verbosity:
 .sp
@@ -414,14 +419,17 @@
 useful to allow external devices like smartphones or streaming boxes to
 watch streams they wouldn\(aqt be able to otherwise.
 .sp
 The default behavior is similar to the \fI\%\-\-player\-continuous\-http\fP option,
 but no player program will be started, and the server will listen on all available
 connections instead of just in the local (loopback) interface.
 .sp
+See \fI\%\-\-player\-external\-http\-interface\fP for choosing a specific network interface, and
+see \fI\%\-\-player\-external\-http\-port\fP for choosing a non\-randomized port.
+.sp
 Optionally, the \fI\%\-\-player\-external\-http\-continuous\fP option allows for disabling
 the continuous run\-mode, so that Streamlink will stop when the stream ends.
 .sp
 The URLs that can be used to access the stream will be printed to the
 console, and the server can be interrupted using CTRL\-C.
 .UNINDENT
 .INDENT 0.0
@@ -434,14 +442,20 @@
 .sp
 If set to non\-continuous, Streamlink will stop once the stream has ended.
 .sp
 Default is: \fBtrue\fP\&.
 .UNINDENT
 .INDENT 0.0
 .TP
+.B \-\-player\-external\-http\-interface INTERFACE
+The network interface on which the HTTP server will be listening on.
+If unset or set to \fB0.0.0.0\fP, all available interfaces will be bound.
+.UNINDENT
+.INDENT 0.0
+.TP
 .B \-\-player\-external\-http\-port PORT
 A fixed port to use for the external HTTP server if that mode is
 enabled. Omit or set to \fB0\fP to use a random high ( >1024) port.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-player\-passthrough TYPES
```

### Comparing `streamlink-5.4.0/docs/_man.rst` & `streamlink-5.5.0/docs/_man.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_static/apple-touch-icon.png` & `streamlink-5.5.0/docs/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_static/favicon-16x16.png` & `streamlink-5.5.0/docs/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_static/favicon-32x32.png` & `streamlink-5.5.0/docs/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_static/favicon.ico` & `streamlink-5.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_static/icon-ffmpeg.svg` & `streamlink-5.5.0/docs/_static/icon-ffmpeg.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_static/icon-python.svg` & `streamlink-5.5.0/docs/_static/icon-python.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_static/icon.svg` & `streamlink-5.5.0/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_static/opengraph-image.png` & `streamlink-5.5.0/docs/_static/opengraph-image.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_static/styles/custom.css` & `streamlink-5.5.0/docs/_static/styles/custom.css`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_templates/base.html` & `streamlink-5.5.0/docs/_templates/base.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/_templates/sidebar/brand.html` & `streamlink-5.5.0/docs/_templates/sidebar/brand.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 <a class="sidebar-brand centered" href="{{ pathto(master_doc) }}">
   <div class="sidebar-logo-container">
-    <img class="sidebar-logo" src="{{ pathto('_static/' + logo, 1) }}" alt="{{ project }}"/>
+    <img class="sidebar-logo only-light" src="{{ pathto('_static/' + theme_light_logo, 1) }}" alt="{{ project }}"/>
+    <img class="sidebar-logo only-dark" src="{{ pathto('_static/' + theme_dark_logo, 1) }}" alt="{{ project }}"/>
   </div>
   <p class="sidebar-brand-text">{{ project }}</p>
   <p class="sidebar-brand-oneliner">{{ oneliner }}</p>
 </a>
 <div class="sidebar-versions centered" role="note" aria-label="versions">
   <pre class="sidebar-versions-current">{{ release }}</pre>
   <dl class="sidebar-versions-others">
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-[{{_project_}}]
+[{{_project_}}]_[{{_project_}}]
 {{_project_}}
 {{_oneliner_}}
 {{ release }}
       Stable
       Latest
```

### Comparing `streamlink-5.4.0/docs/_templates/sidebar/github-buttons.html` & `streamlink-5.5.0/docs/_templates/sidebar/github-buttons.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/api.rst` & `streamlink-5.5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/api_guide.rst` & `streamlink-5.5.0/docs/api_guide.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/applications.rst` & `streamlink-5.5.0/docs/applications.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/changelog.md` & `streamlink-5.5.0/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## streamlink 5.5.0 (2023-05-05)
+
+Release highlights:
+
+- Added: `--no-config` ([#5314](https://github.com/streamlink/streamlink/pull/5314))
+- Added: `--player-external-http-interface` ([#5295](https://github.com/streamlink/streamlink/pull/5295))
+- Fixed: M3U8 attribute parsing issue ([#5307](https://github.com/streamlink/streamlink/pull/5307))
+- Fixed: various minor plugin issues ([#5291](https://github.com/streamlink/streamlink/pull/5291), [#5299](https://github.com/streamlink/streamlink/pull/5299), [#5306](https://github.com/streamlink/streamlink/pull/5306))
+- Build: bumped urllib3 to `>=1.26.0,<3` and fixed compatibility issues with `urllib3 >=2.0.0` ([#5326](https://github.com/streamlink/streamlink/pull/5326), [#5325](https://github.com/streamlink/streamlink/pull/5325))
+- Docs: bumped furo theme to `2023.03.27` ([#5301](https://github.com/streamlink/streamlink/pull/5301))
+- Docs: bumped build dependencies `sphinx >=5.0.0,<7`, `myst-parser >=1.0.0,<2` and `sphinx-design >=0.4.1,<1` ([#5301](https://github.com/streamlink/streamlink/pull/5301))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/5.4.0...5.5.0)
+
+
 ## streamlink 5.4.0 (2023-04-12)
 
 Release highlights:
 
 - Added: `--progress` CLI argument and [deprecated `--force-progress`](https://streamlink.github.io/deprecations.html#deprecation-of-force-progress) ([#5268](https://github.com/streamlink/streamlink/pull/5268))
 - Added: `--dash-manifest-reload-attempts` and respective session option ([#5208](https://github.com/streamlink/streamlink/pull/5208))
 - Improved: DASH segment availability/download logging ([#5214](https://github.com/streamlink/streamlink/pull/5214), [#5235](https://github.com/streamlink/streamlink/pull/5235))
```

### Comparing `streamlink-5.4.0/docs/cli/config.rst` & `streamlink-5.5.0/docs/cli/config.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/cli/metadata.rst` & `streamlink-5.5.0/docs/cli/metadata.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/cli/plugin-sideloading.rst` & `streamlink-5.5.0/docs/cli/plugin-sideloading.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/cli/plugins/crunchyroll.rst` & `streamlink-5.5.0/docs/cli/plugins/crunchyroll.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/cli/plugins/twitch.rst` & `streamlink-5.5.0/docs/cli/plugins/twitch.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/cli/protocols.rst` & `streamlink-5.5.0/docs/cli/protocols.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/cli/proxy.rst` & `streamlink-5.5.0/docs/cli/proxy.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/cli/tutorial.rst` & `streamlink-5.5.0/docs/cli/tutorial.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/cli.rst` & `streamlink-5.5.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/conf.py` & `streamlink-5.5.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,16 @@
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     "source_repository": "https://github.com/streamlink/streamlink/",
     "source_branch": "master",
     "source_directory": "docs/",
+    "light_logo": "icon.svg",
+    "dark_logo": "icon.svg",
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 #html_theme_path = []
 
 # HTML template variables via the custom ext_html_template_vars extension
 html_template_vars = {
```

### Comparing `streamlink-5.4.0/docs/deprecations.rst` & `streamlink-5.5.0/docs/deprecations.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/developing.rst` & `streamlink-5.5.0/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/donate.rst` & `streamlink-5.5.0/docs/donate.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/ext_argparse.py` & `streamlink-5.5.0/docs/ext_argparse.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/ext_github.py` & `streamlink-5.5.0/docs/ext_github.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/ext_plugins.py` & `streamlink-5.5.0/docs/ext_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/ext_releaseref.py` & `streamlink-5.5.0/docs/ext_releaseref.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/index.rst` & `streamlink-5.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/install.rst` & `streamlink-5.5.0/docs/install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -179,28 +179,33 @@
 
                                      `NixOS channel`_
 
 `openSUSE`_                          .. code-block:: bash
 
                                         sudo zypper install streamlink
 
+`Solus`_                             .. code-block:: bash
+
+                                        sudo eopkg install streamlink
+
 `Void`_                              .. code-block:: bash
 
                                         sudo xbps-install streamlink
 ==================================== ===========================================
 
 .. _Arch Linux: https://www.archlinux.org/packages/community/any/streamlink/
 .. _Arch Linux (aur, git): https://aur.archlinux.org/packages/streamlink-git/
 .. _Debian (sid, testing): https://packages.debian.org/unstable/streamlink
 .. _Debian (stable): https://packages.debian.org/unstable/streamlink
 .. _Fedora: https://src.fedoraproject.org/rpms/python-streamlink
 .. _Gentoo Linux: https://packages.gentoo.org/package/net-misc/streamlink
 .. _NetBSD (pkgsrc): https://pkgsrc.se/multimedia/streamlink
 .. _NixOS: https://github.com/NixOS/nixpkgs/tree/master/pkgs/applications/video/streamlink
 .. _openSUSE: https://build.opensuse.org/package/show/multimedia:apps/streamlink
+.. _Solus: https://dev.getsol.us/source/streamlink/
 .. _Void: https://github.com/void-linux/void-packages/tree/master/srcpkgs/streamlink
 
 .. _Installing AUR packages: https://wiki.archlinux.org/index.php/Arch_User_Repository#Installing_packages
 .. _Installing Debian backported packages: https://wiki.debian.org/Backports#Using_the_command_line
 .. _NixOS channel: https://search.nixos.org/packages?show=streamlink&query=streamlink
 
 
@@ -217,14 +222,15 @@
 Chocolatey                           Scott Walters <me at scowalt.com>
 Debian                               Alexis Murzeau <amubtdx at gmail.com>
 Fedora                               Mohamed El Morabity <melmorabity at fedoraproject.org>
 Gentoo                               soredake <fdsfgs at krutt.org>
 NetBSD                               Maya Rashish <maya at netbsd.org>
 NixOS                                Tuomas Tynkkynen <tuomas.tynkkynen at iki.fi>
 openSUSE                             Simon Puchert <simonpuchert at alice.de>
+Solus                                Joey Riches <josephriches at gmail.com>
 Void                                 Michal Vasilek <michal at vasilek.cz>
 Windows binaries                     Sebastian Meyer <mail at bastimeyer.de>
 Linux AppImages                      Sebastian Meyer <mail at bastimeyer.de>
 ==================================== ===========================================
 
 
 Package availability
@@ -235,15 +241,15 @@
 the `Windows installers + portable builds <Windows binaries_>`_,
 and the `Linux AppImages <Linux AppImages_>`_.
 
 If a packaged release of Streamlink is not available for your operating system / distro or your system's architecture,
 or if it's out of date or broken, then please contact the respective package maintainers or package-repository maintainers
 of your operating system / distro, as it's up to them to add, update, or fix those packages.
 
-Users of glibc-based Linux distros can find up-to-date Streamlink releases via the available `AppImages <Linux AppImages>`_.
+Users of glibc-based Linux distros can find up-to-date Streamlink releases via the available `AppImages <Linux AppImages_>`_.
 
 Please open an issue or pull request on GitHub if an **available**, **maintained** and **up-to-date** package is missing
 from the install docs.
 
 
 .. _pypi-package-and-source-code:
```

### Comparing `streamlink-5.4.0/docs/issues.rst` & `streamlink-5.5.0/docs/issues.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/players.rst` & `streamlink-5.5.0/docs/players.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/docs/thirdparty.rst` & `streamlink-5.5.0/docs/thirdparty.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/icon.svg` & `streamlink-5.5.0/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/pyproject.toml` & `streamlink-5.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/setup.cfg` & `streamlink-5.5.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 	importlib-metadata ; python_version<"3.8"
 	isodate
 	lxml >=4.6.4,<5.0
 	pycountry
 	pycryptodome >=3.4.3,<4
 	PySocks !=1.5.7,>=1.5.6
 	requests >=2.26.0,<3.0
-	urllib3 >=1.26.0
+	urllib3 >=1.26.0,<3
 	websocket-client >=1.2.1,<2.0
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 streamlink =
```

### Comparing `streamlink-5.4.0/setup.py` & `streamlink-5.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/__init__.py` & `streamlink-5.5.0/src/streamlink/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/_version.py` & `streamlink-5.5.0/src/streamlink/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
     return get_version(
         project_dir=Path(streamlink.__file__).parents[2],
     )
 
 
 # The following _get_version() call will get replaced by versioningit with a static version string when building streamlink
 # `pip install .` / `pip wheel .` / `python setup.py build` / `python setup.py bdist_wheel` / etc.
-__version__ = "5.4.0"
+__version__ = "5.5.0"
```

### Comparing `streamlink-5.4.0/src/streamlink/api.py` & `streamlink-5.5.0/src/streamlink/api.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/buffers.py` & `streamlink-5.5.0/src/streamlink/buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/cache.py` & `streamlink-5.5.0/src/streamlink/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/exceptions.py` & `streamlink-5.5.0/src/streamlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/logger.py` & `streamlink-5.5.0/src/streamlink/logger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/options.py` & `streamlink-5.5.0/src/streamlink/options.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/packages/requests_file.py` & `streamlink-5.5.0/src/streamlink/packages/requests_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugin/__init__.py` & `streamlink-5.5.0/src/streamlink/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugin/api/http_session.py` & `streamlink-5.5.0/src/streamlink/plugin/api/http_session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-import ssl
+import re
 import time
 from typing import Any, Dict, Pattern, Tuple
 
 import requests.adapters
 import urllib3
 from requests import PreparedRequest, Request, Session
+from requests.adapters import HTTPAdapter
 
 from streamlink.exceptions import PluginError
 from streamlink.packages.requests_file import FileAdapter
 from streamlink.plugin.api import useragents
 from streamlink.utils.parse import parse_json, parse_xml
 
 
+# urllib3>=2.0.0: enforce_content_length now defaults to True (keep the override for backwards compatibility)
 class _HTTPResponse(urllib3.response.HTTPResponse):
     def __init__(self, *args, **kwargs):
         # Always enforce content length validation!
         # This fixes a bug in requests which doesn't raise errors on HTTP responses where
         # the "Content-Length" header doesn't match the response's body length.
         # https://github.com/psf/requests/issues/4956#issuecomment-573325001
         #
@@ -46,24 +48,27 @@
 # > The uppercase hexadecimal digits 'A' through 'F' are equivalent to
 # > the lowercase digits 'a' through 'f', respectively.  If two URIs
 # > differ only in the case of hexadecimal digits used in percent-encoded
 # > octets, they are equivalent.  For consistency, URI producers and
 # > normalizers should use uppercase hexadecimal digits for all percent-
 # > encodings.
 class Urllib3UtilUrlPercentReOverride:
-    _re_percent_encoding: Pattern = urllib3.util.url.PERCENT_RE  # type: ignore[attr-defined]
+    # urllib3>=2.0.0: _PERCENT_RE, urllib3<2.0.0: PERCENT_RE
+    _re_percent_encoding: Pattern \
+        = getattr(urllib3.util.url, "_PERCENT_RE", getattr(urllib3.util.url, "PERCENT_RE", re.compile(r"%[a-fA-F0-9]{2}")))
 
     # urllib3>=1.25.8
     # https://github.com/urllib3/urllib3/blame/1.25.8/src/urllib3/util/url.py#L219-L227
     @classmethod
     def subn(cls, repl: Any, string: str, count: Any = None) -> Tuple[str, int]:
         return string, len(cls._re_percent_encoding.findall(string))
 
 
-urllib3.util.url.PERCENT_RE = Urllib3UtilUrlPercentReOverride  # type: ignore[attr-defined]
+# urllib3>=2.0.0: _PERCENT_RE, urllib3<2.0.0: PERCENT_RE
+urllib3.util.url._PERCENT_RE = urllib3.util.url.PERCENT_RE = Urllib3UtilUrlPercentReOverride  # type: ignore[attr-defined]
 
 
 # requests.Request.__init__ keywords, except for "hooks"
 _VALID_REQUEST_ARGS = "method", "url", "headers", "files", "data", "params", "auth", "cookies", "json"
 
 
 class HTTPSession(Session):
@@ -177,16 +182,28 @@
 
         if schema:
             res = schema.validate(res.text, name="response text", exception=PluginError)
 
         return res
 
 
-class TLSSecLevel1Adapter(requests.adapters.HTTPAdapter):
+class TLSNoDHAdapter(HTTPAdapter):
     def init_poolmanager(self, *args, **kwargs):
-        ctx = ssl.create_default_context()
+        ctx = urllib3.util.create_urllib3_context()
+        ctx.load_default_certs()
+        ciphers = ":".join(cipher.get("name") for cipher in ctx.get_ciphers())
+        ciphers += ":!DH"
+        ctx.set_ciphers(ciphers)
+        kwargs["ssl_context"] = ctx
+        return super().init_poolmanager(*args, **kwargs)
+
+
+class TLSSecLevel1Adapter(HTTPAdapter):
+    def init_poolmanager(self, *args, **kwargs):
+        ctx = urllib3.util.create_urllib3_context()
+        ctx.load_default_certs()
         ctx.set_ciphers("DEFAULT:@SECLEVEL=1")
         kwargs["ssl_context"] = ctx
         return super().init_poolmanager(*args, **kwargs)
 
 
-__all__ = ["HTTPSession", "TLSSecLevel1Adapter"]
+__all__ = ["HTTPSession", "TLSNoDHAdapter", "TLSSecLevel1Adapter"]
```

### Comparing `streamlink-5.4.0/src/streamlink/plugin/api/useragents.py` & `streamlink-5.5.0/src/streamlink/plugin/api/useragents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-ANDROID = "Mozilla/5.0 (Linux; Android 13) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.5563.116 Mobile Safari/537.36"
-CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"
-CHROME_OS = "Mozilla/5.0 (X11; CrOS x86_64 15236.80.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.5414.125 Safari/537.36"
-FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:111.0) Gecko/20100101 Firefox/111.0"
+ANDROID = "Mozilla/5.0 (Linux; Android 13) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.5615.135 Mobile Safari/537.36"
+CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36"
+CHROME_OS = "Mozilla/5.0 (X11; CrOS x86_64 15359.58.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.5615.134 Safari/537.36"
+FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109) Gecko/20100101 Firefox/112.0"
 IE_11 = "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko"
-IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 16_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.4 Mobile/15E148 Safari/604.1"
-OPERA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 OPR/97.0.4719.17"
-SAFARI = "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_3) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.4 Safari/605.1.15"
+IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 16_4_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.4 Mobile/15E148 Safari/604.1"
+OPERA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 OPR/98.0.4759.3"
+SAFARI = "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_3_1) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.4 Safari/605.1.15"
 
 # Backwards compatibility
 EDGE = CHROME
 FIREFOX_MAC = FIREFOX
 IE_6 = IE_7 = IE_8 = IE_9 = IE_11
 IPHONE_6 = IPAD = IPHONE
 SAFARI_7 = SAFARI_8 = SAFARI
```

### Comparing `streamlink-5.4.0/src/streamlink/plugin/api/validate/__init__.py` & `streamlink-5.5.0/src/streamlink/plugin/api/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugin/api/validate/_exception.py` & `streamlink-5.5.0/src/streamlink/plugin/api/validate/_exception.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugin/api/validate/_schemas.py` & `streamlink-5.5.0/src/streamlink/plugin/api/validate/_schemas.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugin/api/validate/_validate.py` & `streamlink-5.5.0/src/streamlink/plugin/api/validate/_validate.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugin/api/validate/_validators.py` & `streamlink-5.5.0/src/streamlink/plugin/api/validate/_validators.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugin/api/websocket.py` & `streamlink-5.5.0/src/streamlink/plugin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugin/plugin.py` & `streamlink-5.5.0/src/streamlink/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/abematv.py` & `streamlink-5.5.0/src/streamlink/plugins/abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/adultswim.py` & `streamlink-5.5.0/src/streamlink/plugins/adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/afreeca.py` & `streamlink-5.5.0/src/streamlink/plugins/afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/albavision.py` & `streamlink-5.5.0/src/streamlink/plugins/albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/aloula.py` & `streamlink-5.5.0/src/streamlink/plugins/aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/app17.py` & `streamlink-5.5.0/src/streamlink/plugins/app17.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/ard_live.py` & `streamlink-5.5.0/src/streamlink/plugins/ard_live.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/ard_mediathek.py` & `streamlink-5.5.0/src/streamlink/plugins/ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/artetv.py` & `streamlink-5.5.0/src/streamlink/plugins/artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/atpchallenger.py` & `streamlink-5.5.0/src/streamlink/plugins/atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/atresplayer.py` & `streamlink-5.5.0/src/streamlink/plugins/atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/bbciplayer.py` & `streamlink-5.5.0/src/streamlink/plugins/bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/bfmtv.py` & `streamlink-5.5.0/src/streamlink/plugins/bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/bigo.py` & `streamlink-5.5.0/src/streamlink/plugins/bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/bilibili.py` & `streamlink-5.5.0/src/streamlink/plugins/bilibili.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/blazetv.py` & `streamlink-5.5.0/src/streamlink/plugins/blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/bloomberg.py` & `streamlink-5.5.0/src/streamlink/plugins/bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/booyah.py` & `streamlink-5.5.0/src/streamlink/plugins/booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/brightcove.py` & `streamlink-5.5.0/src/streamlink/plugins/brightcove.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/btv.py` & `streamlink-5.5.0/src/streamlink/plugins/btv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/cbsnews.py` & `streamlink-5.5.0/src/streamlink/plugins/cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/cdnbg.py` & `streamlink-5.5.0/src/streamlink/plugins/cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/ceskatelevize.py` & `streamlink-5.5.0/src/streamlink/plugins/ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/cinergroup.py` & `streamlink-5.5.0/src/streamlink/plugins/cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/clubbingtv.py` & `streamlink-5.5.0/src/streamlink/plugins/clubbingtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/cmmedia.py` & `streamlink-5.5.0/src/streamlink/plugins/cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/cnews.py` & `streamlink-5.5.0/src/streamlink/plugins/cnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/crunchyroll.py` & `streamlink-5.5.0/src/streamlink/plugins/crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/dailymotion.py` & `streamlink-5.5.0/src/streamlink/plugins/dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/dash.py` & `streamlink-5.5.0/src/streamlink/plugins/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/delfi.py` & `streamlink-5.5.0/src/streamlink/plugins/delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/deutschewelle.py` & `streamlink-5.5.0/src/streamlink/plugins/deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/dlive.py` & `streamlink-5.5.0/src/streamlink/plugins/dlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/dogan.py` & `streamlink-5.5.0/src/streamlink/plugins/dogan.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,42 +29,49 @@
     API_URLS = [
         "/api/media?id={id}",
         "/actions/content/media/{id}",
         "/action/media/{id}",
     ]
     API_URL_OLD = "/actions/media?id={id}"
 
-    def _get_content_id(self):
-        return self.session.http.get(
-            self.url,
-            schema=validate.Schema(
-                validate.parse_html(),
-                validate.any(
-                    validate.all(
-                        validate.xml_xpath_string("""
-                            .//div[@data-id][
-                                @data-live
-                                or @id='video-element'
-                                or @id='player-container'
-                                or contains(@class, 'player-container')
-                            ][1]/@data-id
-                        """),
-                        str,
-                    ),
-                    # xpath query needs to have a lower priority
-                    validate.all(
-                        validate.xml_xpath_string(
-                            ".//body[@data-content-id][1]/@data-content-id",
-                        ),
-                        str,
+    @staticmethod
+    def _get_hls_url(root):
+        schema = validate.Schema(
+            validate.xml_xpath_string(".//*[@data-live][contains(@data-url,'.m3u8')]/@data-url"),
+        )
+
+        return schema.validate(root)
+
+    @staticmethod
+    def _get_content_id(root):
+        schema=validate.Schema(
+            validate.any(
+                validate.all(
+                    validate.xml_xpath_string("""
+                        .//div[@data-id][
+                            @data-live
+                            or @id='video-element'
+                            or @id='player-container'
+                            or contains(@class, 'player-container')
+                        ][1]/@data-id
+                    """),
+                    str,
+                ),
+                # xpath query needs to have a lower priority
+                validate.all(
+                    validate.xml_xpath_string(
+                        ".//body[@data-content-id][1]/@data-content-id",
                     ),
+                    str,
                 ),
             ),
         )
 
+        return schema.validate(root)
+
     def _api_query_new(self, content_id, api_url):
         url = urljoin(self.url, api_url.format(id=content_id))
         data = self.session.http.get(
             url,
             schema=validate.Schema(
                 validate.parse_json(),
                 validate.any(
@@ -127,30 +134,33 @@
                 validate.get(("data", "media", "link")),
                 validate.union_get("serviceUrl", "defaultServiceUrl", "securePath"),
             ),
         )
 
         return urljoin(service_url or default_service_url, secure_path)
 
-    def _get_hls_url(self, content_id):
+    def _query_hls_url(self, content_id):
         for idx, match in enumerate(self.matches[:len(self.API_URLS)]):
             if match:
                 return self._api_query_new(content_id, self.API_URLS[idx])
 
         return self._api_query_old(content_id)
 
     def _get_streams(self):
-        try:
-            content_id = self._get_content_id()
-        except PluginError:
-            log.error("Could not find the content ID for this stream")
-            return
+        root = self.session.http.get(self.url, schema=validate.Schema(validate.parse_html()))
 
-        log.debug(f"Loading content: {content_id}")
-        hls_url = self._get_hls_url(content_id)
+        hls_url = self._get_hls_url(root)
         if not hls_url:
-            return
+            try:
+                content_id = self._get_content_id(root)
+            except PluginError:
+                log.error("Could not find the content ID for this stream")
+                return
+
+            log.debug(f"Loading content: {content_id}")
+            hls_url = self._query_hls_url(content_id)
 
-        return HLSStream.parse_variant_playlist(self.session, hls_url)
+        if hls_url:
+            return HLSStream.parse_variant_playlist(self.session, hls_url)
 
 
 __plugin__ = Dogan
```

### Comparing `streamlink-5.4.0/src/streamlink/plugins/dogus.py` & `streamlink-5.5.0/src/streamlink/plugins/dogus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/drdk.py` & `streamlink-5.5.0/src/streamlink/plugins/drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/earthcam.py` & `streamlink-5.5.0/src/streamlink/plugins/earthcam.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/euronews.py` & `streamlink-5.5.0/src/streamlink/plugins/euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/facebook.py` & `streamlink-5.5.0/src/streamlink/plugins/facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/filmon.py` & `streamlink-5.5.0/src/streamlink/plugins/filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/foxtr.py` & `streamlink-5.5.0/src/streamlink/plugins/foxtr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/galatasaraytv.py` & `streamlink-5.5.0/src/streamlink/plugins/galatasaraytv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/goltelevision.py` & `streamlink-5.5.0/src/streamlink/plugins/goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/goodgame.py` & `streamlink-5.5.0/src/streamlink/plugins/goodgame.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/googledrive.py` & `streamlink-5.5.0/src/streamlink/plugins/googledrive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/gulli.py` & `streamlink-5.5.0/src/streamlink/plugins/gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/hiplayer.py` & `streamlink-5.5.0/src/streamlink/plugins/hiplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/hls.py` & `streamlink-5.5.0/src/streamlink/plugins/hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/http.py` & `streamlink-5.5.0/src/streamlink/plugins/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/htv.py` & `streamlink-5.5.0/src/streamlink/plugins/htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/huajiao.py` & `streamlink-5.5.0/src/streamlink/plugins/huajiao.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/huya.py` & `streamlink-5.5.0/src/streamlink/plugins/huya.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/idf1.py` & `streamlink-5.5.0/src/streamlink/plugins/idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/indihometv.py` & `streamlink-5.5.0/src/streamlink/plugins/indihometv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/invintus.py` & `streamlink-5.5.0/src/streamlink/plugins/invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/kugou.py` & `streamlink-5.5.0/src/streamlink/plugins/kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/linelive.py` & `streamlink-5.5.0/src/streamlink/plugins/linelive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/livestream.py` & `streamlink-5.5.0/src/streamlink/plugins/livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/lnk.py` & `streamlink-5.5.0/src/streamlink/plugins/lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/lrt.py` & `streamlink-5.5.0/src/streamlink/plugins/lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/ltv_lsm_lv.py` & `streamlink-5.5.0/src/streamlink/plugins/ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/mdstrm.py` & `streamlink-5.5.0/src/streamlink/plugins/mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/mediaklikk.py` & `streamlink-5.5.0/src/streamlink/plugins/mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/mediavitrina.py` & `streamlink-5.5.0/src/streamlink/plugins/mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/mildom.py` & `streamlink-5.5.0/src/streamlink/plugins/mildom.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/mitele.py` & `streamlink-5.5.0/src/streamlink/plugins/mitele.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,11 +109,16 @@
                 log.warning("Stream may be protected by DRM")
                 continue
             cdn_token = tokens.get(stream["lid"], {}).get("cdn", "")
             qsd = parse_qsd(cdn_token)
             urls.add(update_qsd(stream["stream"], qsd, quote_via=lambda string, *_, **__: string))
 
         for url in urls:
-            yield from HLSStream.parse_variant_playlist(self.session, url, name_fmt="{pixels}_{bitrate}").items()
+            yield from HLSStream.parse_variant_playlist(
+                self.session,
+                url,
+                headers={"Origin": "https://www.mitele.es"},
+                name_fmt="{pixels}_{bitrate}",
+            ).items()
 
 
 __plugin__ = Mitele
```

### Comparing `streamlink-5.4.0/src/streamlink/plugins/mixcloud.py` & `streamlink-5.5.0/src/streamlink/plugins/mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/mjunoon.py` & `streamlink-5.5.0/src/streamlink/plugins/mjunoon.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/mrtmk.py` & `streamlink-5.5.0/src/streamlink/plugins/mrtmk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/n13tv.py` & `streamlink-5.5.0/src/streamlink/plugins/n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/nhkworld.py` & `streamlink-5.5.0/src/streamlink/plugins/nhkworld.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/nicolive.py` & `streamlink-5.5.0/src/streamlink/plugins/nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/nimotv.py` & `streamlink-5.5.0/src/streamlink/plugins/nimotv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/nos.py` & `streamlink-5.5.0/src/streamlink/plugins/nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/nownews.py` & `streamlink-5.5.0/src/streamlink/plugins/nownews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/nrk.py` & `streamlink-5.5.0/src/streamlink/plugins/nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/ntv.py` & `streamlink-5.5.0/src/streamlink/plugins/ntv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/okru.py` & `streamlink-5.5.0/src/streamlink/plugins/okru.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/olympicchannel.py` & `streamlink-5.5.0/src/streamlink/plugins/olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/oneplusone.py` & `streamlink-5.5.0/src/streamlink/plugins/oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/onetv.py` & `streamlink-5.5.0/src/streamlink/plugins/onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/openrectv.py` & `streamlink-5.5.0/src/streamlink/plugins/openrectv.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
             else:
                 log.error("There is no video file.")
 
             if m3u8_file is not None:
                 yield from HLSStream.parse_variant_playlist(
                     self.session,
                     m3u8_file,
+                    headers={"Referer": self.url},
                 ).items()
 
         else:
             log.error("You don't have the authority or no video file.")
 
 
 __plugin__ = OPENRECtv
```

### Comparing `streamlink-5.4.0/src/streamlink/plugins/pandalive.py` & `streamlink-5.5.0/src/streamlink/plugins/pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/picarto.py` & `streamlink-5.5.0/src/streamlink/plugins/picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/piczel.py` & `streamlink-5.5.0/src/streamlink/plugins/piczel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/pixiv.py` & `streamlink-5.5.0/src/streamlink/plugins/pixiv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/pluto.py` & `streamlink-5.5.0/src/streamlink/plugins/pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/pluzz.py` & `streamlink-5.5.0/src/streamlink/plugins/pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/qq.py` & `streamlink-5.5.0/src/streamlink/plugins/qq.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/radiko.py` & `streamlink-5.5.0/src/streamlink/plugins/radiko.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/radionet.py` & `streamlink-5.5.0/src/streamlink/plugins/radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/raiplay.py` & `streamlink-5.5.0/src/streamlink/plugins/raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/reuters.py` & `streamlink-5.5.0/src/streamlink/plugins/reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/rtbf.py` & `streamlink-5.5.0/src/streamlink/plugins/rtbf.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/rtpa.py` & `streamlink-5.5.0/src/streamlink/plugins/rtpa.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/rtpplay.py` & `streamlink-5.5.0/src/streamlink/plugins/rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/rtve.py` & `streamlink-5.5.0/src/streamlink/plugins/rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/rtvs.py` & `streamlink-5.5.0/src/streamlink/plugins/rtvs.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/ruv.py` & `streamlink-5.5.0/src/streamlink/plugins/ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/sbscokr.py` & `streamlink-5.5.0/src/streamlink/plugins/sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/showroom.py` & `streamlink-5.5.0/src/streamlink/plugins/showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/sportal.py` & `streamlink-5.5.0/src/streamlink/plugins/sportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/sportschau.py` & `streamlink-5.5.0/src/streamlink/plugins/sportschau.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/ssh101.py` & `streamlink-5.5.0/src/streamlink/plugins/ssh101.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/stadium.py` & `streamlink-5.5.0/src/streamlink/plugins/stadium.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/steam.py` & `streamlink-5.5.0/src/streamlink/plugins/steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/streamable.py` & `streamlink-5.5.0/src/streamlink/plugins/streamable.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/streann.py` & `streamlink-5.5.0/src/streamlink/plugins/streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/stv.py` & `streamlink-5.5.0/src/streamlink/plugins/stv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/svtplay.py` & `streamlink-5.5.0/src/streamlink/plugins/svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/swisstxt.py` & `streamlink-5.5.0/src/streamlink/plugins/swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/telefe.py` & `streamlink-5.5.0/src/streamlink/plugins/telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/telemadrid.py` & `streamlink-5.5.0/src/streamlink/plugins/telemadrid.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tf1.py` & `streamlink-5.5.0/src/streamlink/plugins/tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/trovo.py` & `streamlink-5.5.0/src/streamlink/plugins/trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/turkuvaz.py` & `streamlink-5.5.0/src/streamlink/plugins/turkuvaz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tv360.py` & `streamlink-5.5.0/src/streamlink/plugins/tv360.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tv3cat.py` & `streamlink-5.5.0/src/streamlink/plugins/tv3cat.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tv4play.py` & `streamlink-5.5.0/src/streamlink/plugins/tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tv5monde.py` & `streamlink-5.5.0/src/streamlink/plugins/tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tv8.py` & `streamlink-5.5.0/src/streamlink/plugins/tv8.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tv999.py` & `streamlink-5.5.0/src/streamlink/plugins/tv999.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tvibo.py` & `streamlink-5.5.0/src/streamlink/plugins/tvibo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tviplayer.py` & `streamlink-5.5.0/src/streamlink/plugins/tviplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tvp.py` & `streamlink-5.5.0/src/streamlink/plugins/tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tvrby.py` & `streamlink-5.5.0/src/streamlink/plugins/tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tvrplus.py` & `streamlink-5.5.0/src/streamlink/plugins/tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/tvtoya.py` & `streamlink-5.5.0/src/streamlink/plugins/tvtoya.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/twitcasting.py` & `streamlink-5.5.0/src/streamlink/plugins/twitcasting.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/twitch.py` & `streamlink-5.5.0/src/streamlink/plugins/twitch.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/ustreamtv.py` & `streamlink-5.5.0/src/streamlink/plugins/ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/ustvnow.py` & `streamlink-5.5.0/src/streamlink/plugins/ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/vidio.py` & `streamlink-5.5.0/src/streamlink/plugins/vidio.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/vimeo.py` & `streamlink-5.5.0/src/streamlink/plugins/vimeo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/vinhlongtv.py` & `streamlink-5.5.0/src/streamlink/plugins/vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/vk.py` & `streamlink-5.5.0/src/streamlink/plugins/vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/vkplay.py` & `streamlink-5.5.0/src/streamlink/plugins/vkplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/vlive.py` & `streamlink-5.5.0/src/streamlink/plugins/vlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/vtvgo.py` & `streamlink-5.5.0/src/streamlink/plugins/vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/wasd.py` & `streamlink-5.5.0/src/streamlink/plugins/wasd.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/webtv.py` & `streamlink-5.5.0/src/streamlink/plugins/webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/welt.py` & `streamlink-5.5.0/src/streamlink/plugins/welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/wwenetwork.py` & `streamlink-5.5.0/src/streamlink/plugins/wwenetwork.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/youtube.py` & `streamlink-5.5.0/src/streamlink/plugins/youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/yupptv.py` & `streamlink-5.5.0/src/streamlink/plugins/yupptv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/zattoo.py` & `streamlink-5.5.0/src/streamlink/plugins/zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/zdf_mediathek.py` & `streamlink-5.5.0/src/streamlink/plugins/zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/zeenews.py` & `streamlink-5.5.0/src/streamlink/plugins/zeenews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/zengatv.py` & `streamlink-5.5.0/src/streamlink/plugins/zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/plugins/zhanqi.py` & `streamlink-5.5.0/src/streamlink/plugins/zhanqi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/session.py` & `streamlink-5.5.0/src/streamlink/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import pkgutil
 import warnings
 from functools import lru_cache
 from socket import AF_INET, AF_INET6
 from typing import Any, Callable, ClassVar, Dict, Iterator, Mapping, Optional, Tuple, Type
 
 import urllib3.util.connection as urllib3_util_connection
-import urllib3.util.ssl_ as urllib3_util_ssl
+from requests.adapters import HTTPAdapter
 
 from streamlink import __version__, plugins
 from streamlink.exceptions import NoPluginError, PluginError, StreamlinkDeprecationWarning
 from streamlink.logger import StreamlinkLogger
 from streamlink.options import Options
-from streamlink.plugin.api.http_session import HTTPSession
+from streamlink.plugin.api.http_session import HTTPSession, TLSNoDHAdapter
 from streamlink.plugin.plugin import NO_PRIORITY, NORMAL_PRIORITY, Matcher, Plugin
 from streamlink.utils.l10n import Localization
 from streamlink.utils.module import load_module
 from streamlink.utils.url import update_scheme
 
 
 # Ensure that the Logger class returned is Streamslink's for using the API (for backwards compatibility)
@@ -111,22 +111,20 @@
         self._deprecate_https_proxy(key)
 
     def _set_http_attr(self, key, value):
         setattr(self.session.http, self._OPTIONS_HTTP_ATTRS[key], value)
 
     def _set_http_disable_dh(self, key, value):
         self.set_explicit(key, value)
-        default_ciphers = [
-            item
-            for item in urllib3_util_ssl.DEFAULT_CIPHERS.split(":")  # type: ignore[attr-defined]
-            if item != "!DH"
-        ]
         if value:
-            default_ciphers.append("!DH")
-        urllib3_util_ssl.DEFAULT_CIPHERS = ":".join(default_ciphers)  # type: ignore[attr-defined]
+            adapter = TLSNoDHAdapter()
+        else:
+            adapter = HTTPAdapter()
+
+        self.session.http.mount("https://", adapter)
 
     @staticmethod
     def _factory_set_http_attr_key_equals_value(delimiter: str) -> Callable[["StreamlinkOptions", str, Any], None]:
         def inner(self: "StreamlinkOptions", key: str, value: Any) -> None:
             getattr(self.session.http, self._OPTIONS_HTTP_ATTRS[key]).update(
                 value if isinstance(value, dict) else dict(self._parse_key_equals_value_string(delimiter, value)),
             )
```

### Comparing `streamlink-5.4.0/src/streamlink/stream/dash.py` & `streamlink-5.5.0/src/streamlink/stream/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/stream/dash_manifest.py` & `streamlink-5.5.0/src/streamlink/stream/dash_manifest.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/stream/ffmpegmux.py` & `streamlink-5.5.0/src/streamlink/stream/ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/stream/file.py` & `streamlink-5.5.0/src/streamlink/stream/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/stream/filtered.py` & `streamlink-5.5.0/src/streamlink/stream/filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/stream/hls.py` & `streamlink-5.5.0/src/streamlink/stream/hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/stream/hls_playlist.py` & `streamlink-5.5.0/src/streamlink/stream/hls_playlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
 
 class M3U8Parser:
     _TAGS: ClassVar[Mapping[str, Callable[["M3U8Parser", str], None]]]
 
     _extinf_re = re.compile(r"(?P<duration>\d+(\.\d+)?)(,(?P<title>.+))?")
     _attr_re = re.compile(r"""
-        (?P<key>[A-Z\-]+)
+        (?P<key>[A-Z0-9\-]+)
         =
         (?P<value>
             (?# decimal-integer)
             \d+
             (?# hexadecimal-sequence)
             |0[xX][0-9A-Fa-f]+
             (?# decimal-floating-point and signed-decimal-floating-point)
```

### Comparing `streamlink-5.4.0/src/streamlink/stream/http.py` & `streamlink-5.5.0/src/streamlink/stream/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/stream/segmented.py` & `streamlink-5.5.0/src/streamlink/stream/segmented.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/stream/stream.py` & `streamlink-5.5.0/src/streamlink/stream/stream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/stream/wrappers.py` & `streamlink-5.5.0/src/streamlink/stream/wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/user_input.py` & `streamlink-5.5.0/src/streamlink/user_input.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/__init__.py` & `streamlink-5.5.0/src/streamlink/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/args.py` & `streamlink-5.5.0/src/streamlink/utils/args.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/cache.py` & `streamlink-5.5.0/src/streamlink/utils/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/crypto.py` & `streamlink-5.5.0/src/streamlink/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/data.py` & `streamlink-5.5.0/src/streamlink/utils/data.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/formatter.py` & `streamlink-5.5.0/src/streamlink/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/l10n.py` & `streamlink-5.5.0/src/streamlink/utils/l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/named_pipe.py` & `streamlink-5.5.0/src/streamlink/utils/named_pipe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/parse.py` & `streamlink-5.5.0/src/streamlink/utils/parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/processoutput.py` & `streamlink-5.5.0/src/streamlink/utils/processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/times.py` & `streamlink-5.5.0/src/streamlink/utils/times.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink/utils/url.py` & `streamlink-5.5.0/src/streamlink/utils/url.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink.egg-info/PKG-INFO` & `streamlink-5.5.0/src/streamlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 5.4.0
+Version: 5.5.0
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Home-page: https://github.com/streamlink/streamlink
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 5.4.0 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 5.5.0 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Home-page: https://github.com/streamlink/
 streamlink Author: Streamlink Author-email: streamlink@protonmail.com License:
 Simplified BSD Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues Project-
 URL: Source, https://github.com/streamlink/streamlink Project-URL: Funding,
 https://streamlink.github.io/latest/donate.html Classifier: Development Status
```

### Comparing `streamlink-5.4.0/src/streamlink.egg-info/SOURCES.txt` & `streamlink-5.5.0/src/streamlink.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -270,19 +270,22 @@
 src/streamlink_cli/__init__.py
 src/streamlink_cli/__main__.py
 src/streamlink_cli/argparser.py
 src/streamlink_cli/compat.py
 src/streamlink_cli/console.py
 src/streamlink_cli/constants.py
 src/streamlink_cli/main.py
-src/streamlink_cli/output.py
 src/streamlink_cli/streamrunner.py
+src/streamlink_cli/output/__init__.py
+src/streamlink_cli/output/abc.py
+src/streamlink_cli/output/file.py
+src/streamlink_cli/output/http.py
+src/streamlink_cli/output/player.py
 src/streamlink_cli/utils/__init__.py
 src/streamlink_cli/utils/formatter.py
-src/streamlink_cli/utils/http_server.py
 src/streamlink_cli/utils/path.py
 src/streamlink_cli/utils/player.py
 src/streamlink_cli/utils/progress.py
 src/streamlink_cli/utils/versioncheck.py
 tests/__init__.py
 tests/conftest.py
 tests/test_api_http_session.py
```

### Comparing `streamlink-5.4.0/src/streamlink_cli/argparser.py` & `streamlink-5.5.0/src/streamlink_cli/argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,14 +265,21 @@
         Load options from this config file.
 
         Can be repeated to load multiple files, in which case the options are
         merged on top of each other where the last config has highest priority.
         """,
     )
     general.add_argument(
+        "--no-config",
+        action="store_true",
+        help="""
+        Disable loading any default or custom config files.
+        """,
+    )
+    general.add_argument(
         "-l", "--loglevel",
         metavar="LEVEL",
         choices=logger.levels,
         default="info",
         help=f"""
         Set the log message threshold.
 
@@ -489,14 +496,17 @@
         useful to allow external devices like smartphones or streaming boxes to
         watch streams they wouldn't be able to otherwise.
 
         The default behavior is similar to the --player-continuous-http option,
         but no player program will be started, and the server will listen on all available
         connections instead of just in the local (loopback) interface.
 
+        See --player-external-http-interface for choosing a specific network interface, and
+        see --player-external-http-port for choosing a non-randomized port.
+
         Optionally, the --player-external-http-continuous option allows for disabling
         the continuous run-mode, so that Streamlink will stop when the stream ends.
 
         The URLs that can be used to access the stream will be printed to the
         console, and the server can be interrupted using CTRL-C.
         """,
     )
@@ -513,14 +523,22 @@
 
         If set to non-continuous, Streamlink will stop once the stream has ended.
 
         Default is true.
         """,
     )
     player.add_argument(
+        "--player-external-http-interface",
+        metavar="INTERFACE",
+        help="""
+        The network interface on which the HTTP server will be listening on.
+        If unset or set to `0.0.0.0`, all available interfaces will be bound.
+        """,
+    )
+    player.add_argument(
         "--player-external-http-port",
         metavar="PORT",
         type=num(int, ge=0, le=65535),
         default=0,
         help="""
         A fixed port to use for the external HTTP server if that mode is
         enabled. Omit or set to `0` to use a random high ( >1024) port.
```

### Comparing `streamlink-5.4.0/src/streamlink_cli/compat.py` & `streamlink-5.5.0/src/streamlink_cli/compat.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink_cli/console.py` & `streamlink-5.5.0/src/streamlink_cli/console.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink_cli/constants.py` & `streamlink-5.5.0/src/streamlink_cli/constants.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink_cli/main.py` & `streamlink-5.5.0/src/streamlink_cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from streamlink.stream.stream import Stream, StreamIO
 from streamlink.utils.named_pipe import NamedPipe
 from streamlink.utils.times import LOCAL as LOCALTIMEZONE
 from streamlink_cli.argparser import ArgumentParser, build_parser, setup_session_options
 from streamlink_cli.compat import DeprecatedPath, importlib_metadata, stdout
 from streamlink_cli.console import ConsoleOutput, ConsoleUserInputRequester
 from streamlink_cli.constants import CONFIG_FILES, DEFAULT_STREAM_METADATA, LOG_DIR, PLUGIN_DIRS, STREAM_SYNONYMS
-from streamlink_cli.output import FileOutput, PlayerOutput
+from streamlink_cli.output import FileOutput, HTTPOutput, PlayerOutput
 from streamlink_cli.streamrunner import StreamRunner
-from streamlink_cli.utils import Formatter, HTTPServer, datetime
+from streamlink_cli.utils import Formatter, datetime
 from streamlink_cli.utils.versioncheck import check_version
 
 
 QUIET_OPTIONS = ("json", "stream_url", "quiet")
 
 
 args: Any = None  # type: ignore[assignment]
@@ -144,43 +144,28 @@
             namedpipe=namedpipe,
             http=http,
             record=record,
             title=formatter.title(args.title, defaults=DEFAULT_STREAM_METADATA) if args.title else args.url,
         )
 
 
-def create_http_server(*_args, **_kwargs):
-    """Creates an HTTP server listening on a given host and port.
-
-    If host is empty, listen on all available interfaces, and if port is 0,
-    listen on a random high port.
+def create_http_server(host: Optional[str] = None, port: int = 0) -> HTTPOutput:
+    """
+    Create an HTTP server listening on a given host and port.
+    If host is None, listen on all available interfaces.
+    If port is 0, listen on a random high port.
     """
 
     try:
-        http = HTTPServer()
-        http.bind(*_args, **_kwargs)
+        httpoutput = HTTPOutput(host, port)
+        httpoutput.start_server()
+        return httpoutput
     except OSError as err:
         console.exit(f"Failed to create HTTP server: {err}")
-        return
-
-    return http
-
-
-def iter_http_requests(server, player):
-    """Repeatedly accept HTTP connections on a server.
-
-    Forever if the serving externally, or while a player is running if it is not
-    empty.
-    """
-
-    while not player or player.running:
-        try:
-            yield server.open(timeout=2.5)
-        except OSError:
-            continue
+        raise
 
 
 def output_stream_http(
     plugin: Plugin,
     initial_streams: Dict[str, Stream],
     formatter: Formatter,
     external: bool = False,
@@ -209,24 +194,30 @@
         try:
             log.info(f"Starting player: {args.player}")
             if player:
                 player.open()
         except OSError as err:
             console.exit(f"Failed to start player: {args.player} ({err})")
     else:
-        server = create_http_server(host=None, port=port)
+        server = create_http_server(args.player_external_http_interface, port)
         player = None
 
         log.info("Starting server, access with one of:")
         for url in server.urls:
             log.info(f" {url}")
 
     initial_streams_used = False
-    for req in iter_http_requests(server, player):
-        user_agent = req.headers.get("User-Agent") or "unknown player"
+    while not player or player.running:
+        try:
+            server.accept_connection(timeout=2.5)
+            server.open()
+        except OSError:
+            continue
+
+        user_agent = server.request.headers.get("User-Agent") or "unknown player"
         log.info(f"Got HTTP request from {user_agent}")
 
         stream_fd = prebuffer = None
         while not stream_fd and (not player or player.running):
             try:
                 if not initial_streams_used:
                     streams = initial_streams
@@ -260,19 +251,19 @@
             except OSError as err:
                 # TODO: refactor all console.exit() calls
                 console.exit(str(err))
 
         if not continuous:
             break
 
-        server.close(True)
+        server.close()
 
     if player:
         player.close()
-    server.close()
+    server.shutdown()
 
 
 def output_stream_passthrough(stream, formatter: Formatter):
     """Prepares a filename to be passed to the player."""
     global output
 
     try:
@@ -646,14 +637,17 @@
         args.stream = [stream.lower() for stream in args.stream]
 
     if not args.url and args.url_param:
         args.url = args.url_param
 
 
 def setup_config_args(parser, ignore_unknown=False):
+    if args.no_config:
+        return
+
     config_files = []
 
     if args.config:
         # We want the config specified last to get the highest priority
         config_files.extend(
             config_file
             for config_file in [Path(path).expanduser() for path in reversed(args.config)]
```

### Comparing `streamlink-5.4.0/src/streamlink_cli/output.py` & `streamlink-5.5.0/src/streamlink_cli/output/player.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,25 @@
 import logging
 import os
 import re
 import shlex
 import subprocess
 import sys
 from contextlib import suppress
-from pathlib import Path
 from time import sleep
-from typing import BinaryIO, Optional
 
 from streamlink.compat import is_win32
-from streamlink_cli.compat import stdout
 from streamlink_cli.constants import PLAYER_ARGS_INPUT_DEFAULT, PLAYER_ARGS_INPUT_FALLBACK, SUPPORTED_PLAYERS
+from streamlink_cli.output.abc import Output
 from streamlink_cli.utils import Formatter
 
 
-if is_win32:
-    import msvcrt
-
 log = logging.getLogger("streamlink.cli.output")
 
 
-class Output:
-    def __init__(self):
-        self.opened = False
-
-    def open(self):
-        self._open()
-        self.opened = True
-
-    def close(self):
-        if self.opened:
-            self._close()
-
-        self.opened = False
-
-    def write(self, data):
-        if not self.opened:
-            raise OSError("Output is not opened")
-
-        return self._write(data)
-
-    def _open(self):
-        pass
-
-    def _close(self):
-        pass
-
-    def _write(self, data):
-        pass
-
-
-class FileOutput(Output):
-    def __init__(
-        self,
-        filename: Optional[Path] = None,
-        fd: Optional[BinaryIO] = None,
-        record: Optional["FileOutput"] = None,
-    ):
-        super().__init__()
-        self.filename = filename
-        self.fd = fd
-        self.record = record
-
-    def _open(self):
-        if self.filename:
-            self.filename.parent.mkdir(parents=True, exist_ok=True)
-            self.fd = open(self.filename, "wb")
-
-        if self.record:
-            self.record.open()
-
-        if is_win32:
-            msvcrt.setmode(self.fd.fileno(), os.O_BINARY)
-
-    def _close(self):
-        if self.fd is not stdout:
-            self.fd.close()
-        if self.record:
-            self.record.close()
-
-    def _write(self, data):
-        self.fd.write(data)
-        if self.record:
-            self.record.write(data)
-
-
 class PlayerOutput(Output):
     PLAYER_TERMINATE_TIMEOUT = 10.0
 
     _re_player_args_input = re.compile("|".join(
         re.escape(f"{{{const}}}")
         for const in [PLAYER_ARGS_INPUT_DEFAULT, PLAYER_ARGS_INPUT_FALLBACK]
     ))
@@ -239,23 +169,24 @@
         # Wait 0.5 seconds to see if program exited prematurely
         if not self.running:
             raise OSError("Process exited prematurely")
 
         if self.namedpipe:
             self.namedpipe.open()
         elif self.http:
+            self.http.accept_connection()
             self.http.open()
 
     def _close(self):
         # Close input to the player first to signal the end of the
         # stream and allow the player to terminate of its own accord
         if self.namedpipe:
             self.namedpipe.close()
         elif self.http:
-            self.http.close()
+            self.http.shutdown()
         elif not self.filename:
             self.player.stdin.close()
 
         if self.record:
             self.record.close()
 
         if self.kill:
@@ -277,10 +208,7 @@
 
         if self.namedpipe:
             self.namedpipe.write(data)
         elif self.http:
             self.http.write(data)
         else:
             self.player.stdin.write(data)
-
-
-__all__ = ["PlayerOutput", "FileOutput"]
```

### Comparing `streamlink-5.4.0/src/streamlink_cli/streamrunner.py` & `streamlink-5.5.0/src/streamlink_cli/streamrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import errno
 import logging
 import sys
 from contextlib import suppress
 from pathlib import Path
 from threading import Event, Lock, Thread
-from typing import Optional, Union
+from typing import Optional
 
 from streamlink.stream.stream import StreamIO
-from streamlink_cli.output import FileOutput, PlayerOutput
-from streamlink_cli.utils.http_server import HTTPServer
+from streamlink_cli.output import FileOutput, HTTPOutput, Output, PlayerOutput
 from streamlink_cli.utils.progress import Progress
 
 
 # Use the main Streamlink CLI module as logger
 log = logging.getLogger("streamlink.cli")
 
 
@@ -71,24 +70,23 @@
 
 class StreamRunner:
     """Read data from a stream and write it to the output."""
 
     playerpoller: Optional[PlayerPollThread] = None
     progress: Optional[Progress] = None
 
-    # TODO: refactor all output implementations
     def __init__(
         self,
         stream: StreamIO,
-        output: Union[PlayerOutput, FileOutput, HTTPServer],
+        output: Output,
         show_progress: bool = False,
     ):
         self.stream = stream
         self.output = output
-        self.is_http = isinstance(output, HTTPServer)
+        self.is_http = isinstance(output, HTTPOutput)
 
         filename: Optional[Path] = None
 
         if isinstance(output, PlayerOutput):
             self.playerpoller = PlayerPollThread(stream, output)
             if output.record:
                 filename = output.record.filename
```

### Comparing `streamlink-5.4.0/src/streamlink_cli/utils/__init__.py` & `streamlink-5.5.0/src/streamlink_cli/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 from datetime import datetime as _datetime
 
 from streamlink_cli.utils.formatter import Formatter
-from streamlink_cli.utils.http_server import HTTPServer
 from streamlink_cli.utils.player import find_default_player
 
 
 __all__ = [
-    "Formatter", "HTTPServer", "JSONEncoder",
+    "Formatter", "JSONEncoder",
     "datetime",
     "find_default_player",
 ]
 
 
 class JSONEncoder(json.JSONEncoder):
     def default(self, obj):
```

### Comparing `streamlink-5.4.0/src/streamlink_cli/utils/formatter.py` & `streamlink-5.5.0/src/streamlink_cli/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink_cli/utils/http_server.py` & `streamlink-5.5.0/src/streamlink_cli/output/http.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,84 @@
 import socket
+from contextlib import suppress
 from http.server import BaseHTTPRequestHandler
 from io import BytesIO
+from typing import Optional
+
+from streamlink_cli.output.abc import Output
 
 
 class HTTPRequest(BaseHTTPRequestHandler):
+    # noinspection PyMissingConstructor
     def __init__(self, request_text):
         self.rfile = BytesIO(request_text)
         self.raw_requestline = self.rfile.readline()
         self.error_code = self.error_message = None
         self.parse_request()
 
-    def send_error(self, code, message):
+    def send_error(self, code, message=None, explain=None):
         self.error_code = code
         self.error_message = message
 
 
-class HTTPServer:
-    def __init__(self):
-        self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self.conn = self.host = self.port = None
-        self.bound = False
+class HTTPOutput(Output):
+    socket: socket.socket
+
+    def __init__(self, host: Optional[str] = "127.0.0.1", port: int = 0) -> None:
+        super().__init__()
+        self.host = host
+        self.port = port
+        self.conn: Optional[socket.socket] = None
 
     @property
     def addresses(self):
         if self.host:
             return [self.host]
 
-        addrs = set()
-        try:
-            for info in socket.getaddrinfo(socket.gethostname(), self.port,
-                                           socket.AF_INET):
+        addrs = {"127.0.0.1"}
+        with suppress(socket.gaierror):
+            for info in socket.getaddrinfo(socket.gethostname(), self.port, socket.AF_INET):
                 addrs.add(info[4][0])
-        except socket.gaierror:
-            pass
 
-        addrs.add("127.0.0.1")
         return sorted(addrs)
 
     @property
     def urls(self):
         for addr in self.addresses:
-            yield "http://{0}:{1}/".format(addr, self.port)
+            yield f"http://{addr}:{self.port}/"
 
     @property
     def url(self):
         return next(self.urls, None)
 
-    def bind(self, host="127.0.0.1", port=0):
-        try:
-            self.socket.bind((host or "", port))
-        except OSError:
-            raise
-
+    def start_server(self):
+        self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self.socket.bind((self.host or "", self.port))
         self.socket.listen(1)
-        self.bound = True
         self.host, self.port = self.socket.getsockname()
         if self.host == "0.0.0.0":
             self.host = None
 
-    def open(self, timeout=30):
+    def accept_connection(self, timeout=30) -> None:
         self.socket.settimeout(timeout)
 
         try:
             conn, addr = self.socket.accept()
             conn.settimeout(None)
+            self.conn = conn
         except socket.timeout as err:
+            self.conn = None
             raise OSError("Socket accept timed out") from err
 
+    def _open(self):
+        conn = self.conn
+        if not conn:
+            raise OSError("No client connection")
+
         try:
             req_data = conn.recv(1024)
         except OSError as err:
             raise OSError("Failed to read data from socket") from err
 
         req = HTTPRequest(req_data)
         if req.command not in ("GET", "HEAD"):
@@ -88,27 +95,24 @@
             raise OSError("Failed to write data to socket") from err
 
         # We don't want to send any data on HEAD requests.
         if req.command == "HEAD":
             conn.close()
             raise OSError
 
-        self.conn = conn
-
-        return req
-
-    def write(self, data):
-        if not self.conn:
-            raise OSError("No connection")
+        self.request = req
 
+    def _write(self, data):
         self.conn.sendall(data)
 
-    def close(self, client_only=False):
+    def _close(self):
         if self.conn:
-            self.conn.close()
-
-        if not client_only:
-            try:
-                self.socket.shutdown(2)
-            except OSError:
-                pass
+            with suppress(OSError):
+                self.conn.close()
+            self.conn = None
+
+    def shutdown(self) -> None:
+        self.close()
+        with suppress(OSError):
+            self.socket.shutdown(socket.SHUT_RDWR)
+        with suppress(OSError):
             self.socket.close()
```

### Comparing `streamlink-5.4.0/src/streamlink_cli/utils/path.py` & `streamlink-5.5.0/src/streamlink_cli/utils/path.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink_cli/utils/player.py` & `streamlink-5.5.0/src/streamlink_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink_cli/utils/progress.py` & `streamlink-5.5.0/src/streamlink_cli/utils/progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/src/streamlink_cli/utils/versioncheck.py` & `streamlink-5.5.0/src/streamlink_cli/utils/versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/__init__.py` & `streamlink-5.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/cli/output/test_output.py` & `streamlink-5.5.0/tests/cli/output/test_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from unittest.mock import Mock, call, patch
 
 import pytest
 
 from streamlink_cli.output import FileOutput, PlayerOutput
 
 
-@patch("streamlink_cli.output.stdout")
+@patch("streamlink_cli.output.file.stdout")
 class TestFileOutput(unittest.TestCase):
     @staticmethod
     def subject(filename, fd):
         fo_record = FileOutput(fd=fd)
         fo_main = FileOutput(filename=filename, record=fo_record)
 
         return fo_main, fo_record
@@ -71,15 +71,15 @@
 
     @pytest.mark.posix_only()
     @patch("builtins.open")
     def test_open_posix(self, mock_open: Mock, mock_stdout: Mock):
         self._test_open(mock_open, mock_stdout)
 
     @pytest.mark.windows_only()
-    @patch("streamlink_cli.output.msvcrt")
+    @patch("streamlink_cli.output.file.msvcrt")
     @patch("builtins.open")
     def test_open_windows(self, mock_open: Mock, mock_msvcrt: Mock, mock_stdout: Mock):
         mock_path = self._test_open(mock_open, mock_stdout)
         assert mock_msvcrt.setmode.call_args_list == [
             call(mock_stdout.fileno(), os.O_BINARY),
             call(mock_open(mock_path, "wb").fileno(), os.O_BINARY),
         ]
@@ -87,39 +87,39 @@
 
 class TestPlayerOutput(unittest.TestCase):
     def test_supported_player_generic(self):
         assert PlayerOutput.supported_player("vlc") == "vlc"
         assert PlayerOutput.supported_player("mpv") == "mpv"
         assert PlayerOutput.supported_player("potplayermini.exe") == "potplayer"
 
-    @patch("streamlink_cli.output.os.path.basename", new=ntpath.basename)
+    @patch("streamlink_cli.output.player.os.path.basename", new=ntpath.basename)
     def test_supported_player_win32(self):
         assert PlayerOutput.supported_player("C:\\MPV\\mpv.exe") == "mpv"
         assert PlayerOutput.supported_player("C:\\VLC\\vlc.exe") == "vlc"
         assert PlayerOutput.supported_player("C:\\PotPlayer\\PotPlayerMini64.exe") == "potplayer"
 
-    @patch("streamlink_cli.output.os.path.basename", new=posixpath.basename)
+    @patch("streamlink_cli.output.player.os.path.basename", new=posixpath.basename)
     def test_supported_player_posix(self):
         assert PlayerOutput.supported_player("/usr/bin/mpv") == "mpv"
         assert PlayerOutput.supported_player("/usr/bin/vlc") == "vlc"
 
-    @patch("streamlink_cli.output.os.path.basename", new=ntpath.basename)
+    @patch("streamlink_cli.output.player.os.path.basename", new=ntpath.basename)
     def test_supported_player_args_win32(self):
         assert PlayerOutput.supported_player("C:\\MPV\\mpv.exe --argh") == "mpv"
         assert PlayerOutput.supported_player("C:\\VLC\\vlc.exe --argh") == "vlc"
         assert PlayerOutput.supported_player("C:\\PotPlayer\\PotPlayerMini64.exe --argh") == "potplayer"
 
-    @patch("streamlink_cli.output.os.path.basename", new=posixpath.basename)
+    @patch("streamlink_cli.output.player.os.path.basename", new=posixpath.basename)
     def test_supported_player_args_posix(self):
         assert PlayerOutput.supported_player("/usr/bin/mpv --argh") == "mpv"
         assert PlayerOutput.supported_player("/usr/bin/vlc --argh") == "vlc"
 
-    @patch("streamlink_cli.output.os.path.basename", new=posixpath.basename)
+    @patch("streamlink_cli.output.player.os.path.basename", new=posixpath.basename)
     def test_supported_player_negative_posix(self):
         assert PlayerOutput.supported_player("/usr/bin/xmpvideo") is None
         assert PlayerOutput.supported_player("/usr/bin/echo") is None
 
-    @patch("streamlink_cli.output.os.path.basename", new=ntpath.basename)
+    @patch("streamlink_cli.output.player.os.path.basename", new=ntpath.basename)
     def test_supported_player_negative_win32(self):
         assert PlayerOutput.supported_player("C:\\mpc\\mpc-hd.exe") is None
         assert PlayerOutput.supported_player("C:\\mplayer\\not-vlc.exe") is None
         assert PlayerOutput.supported_player("C:\\NotPlayer\\NotPlayerMini64.exe") is None
```

### Comparing `streamlink-5.4.0/tests/cli/output/test_playeroutput.py` & `streamlink-5.5.0/tests/cli/output/test_playeroutput.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import pytest
 
 from streamlink_cli.output import PlayerOutput
 
 
 @pytest.fixture()
 def playeroutput(request: pytest.FixtureRequest):
-    with patch("streamlink_cli.output.sleep"):
+    with patch("streamlink_cli.output.player.sleep"):
         playeroutput = PlayerOutput(**getattr(request, "param", {}))
         yield playeroutput
         playeroutput.close()
 
 
 @pytest.fixture()
 def mock_popen(playeroutput: PlayerOutput):
     mock_popen = Mock(return_value=Mock(poll=Mock(side_effect=Mock(return_value=None))))
-    with patch("streamlink_cli.output.sleep"), \
+    with patch("streamlink_cli.output.player.sleep"), \
          patch("subprocess.Popen", mock_popen):
         yield mock_popen
 
 
 @pytest.mark.parametrize(("playeroutput", "expected"), [
     pytest.param(
         dict(cmd="mpv", title="foo bar"),
```

### Comparing `streamlink-5.4.0/tests/cli/test_argparser.py` & `streamlink-5.5.0/tests/cli/test_argparser.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/cli/test_cmdline.py` & `streamlink-5.5.0/tests/cli/test_cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
         actual_exit_code = 0
         with patch("sys.argv") as mock_argv, \
              patch("streamlink_cli.main.CONFIG_FILES", []), \
              patch("streamlink_cli.main.setup_logger_and_console"), \
              patch("streamlink_cli.main.setup_plugins"), \
              patch("streamlink_cli.main.setup_streamlink") as mock_setup_streamlink, \
              patch("streamlink_cli.main.streamlink", session), \
-             patch("streamlink_cli.output.subprocess.Popen") as mock_popen, \
-             patch("streamlink_cli.output.subprocess.call") as mock_call, \
-             patch("streamlink_cli.output.sleep"):
+             patch("streamlink_cli.output.player.subprocess.Popen") as mock_popen, \
+             patch("streamlink_cli.output.player.subprocess.call") as mock_call, \
+             patch("streamlink_cli.output.player.sleep"):
             mock_argv.__getitem__.side_effect = lambda x: args[x]
             mock_popen.return_value = Mock(poll=Mock(side_effect=poll_factory([None, 0])))
             try:
                 streamlink_cli.main.main()
             except SystemExit as exc:
                 actual_exit_code = exc.code
```

### Comparing `streamlink-5.4.0/tests/cli/test_cmdline_player_fifo.py` & `streamlink-5.5.0/tests/cli/test_cmdline_player_fifo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/cli/test_cmdline_title.py` & `streamlink-5.5.0/tests/cli/test_cmdline_title.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/cli/test_console.py` & `streamlink-5.5.0/tests/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/cli/test_main.py` & `streamlink-5.5.0/tests/cli/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -916,14 +916,17 @@
                  patch("streamlink_cli.main.setup_signals"):
                 with pytest.raises(SystemExit) as cm:
                     streamlink_cli.main.main()
                 assert cm.value.code == 0
                 mock_resolve_url.assert_not_called()
                 mock_resolve_url_no_redirect.assert_not_called()
 
+    def tearDown(self):
+        streamlink_cli.main.logger.root.handlers.clear()
+
     @staticmethod
     def get_stdout(mock_stdout):
         return "".join([call_arg[0][0] for call_arg in mock_stdout.write.call_args_list])
 
     @patch("sys.stdout")
     @patch("sys.argv", ["streamlink"])
     def test_print_usage(self, mock_stdout):
```

### Comparing `streamlink-5.4.0/tests/cli/test_main_formatter.py` & `streamlink-5.5.0/tests/cli/test_main_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/cli/test_main_setup_config_args.py` & `streamlink-5.5.0/tests/cli/test_main_setup_config_args.py`

 * *Files 21% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
 
 # noinspection PyTestParametrized
 @pytest.mark.usefixtures("_args", "_config_files")
 @pytest.mark.parametrize(("_args", "_config_files", "expected", "deprecations"), [
     pytest.param(
         {
+            "no_config": False,
             "config": None,
             "url": None,
         },
         [
             configdir / "primary",
             DeprecatedPath(configdir / "secondary"),
         ],
@@ -59,14 +60,15 @@
             configdir / "primary",
         ],
         [],
         id="No URL, default config",
     ),
     pytest.param(
         {
+            "no_config": False,
             "config": [
                 str(configdir / "non-existent"),
             ],
             "url": None,
         },
         [
             configdir / "primary",
@@ -74,14 +76,15 @@
         ],
         [],
         [],
         id="No URL, non-existent custom config",
     ),
     pytest.param(
         {
+            "no_config": False,
             "config": None,
             "url": "noplugin",
         },
         [
             configdir / "primary",
             DeprecatedPath(configdir / "secondary"),
         ],
@@ -89,14 +92,15 @@
             configdir / "primary",
         ],
         [],
         id="No plugin, default config",
     ),
     pytest.param(
         {
+            "no_config": False,
             "config": [
                 str(configdir / "non-existent"),
             ],
             "url": "noplugin",
         },
         [
             configdir / "primary",
@@ -104,14 +108,15 @@
         ],
         [],
         [],
         id="No plugin, non-existent custom config",
     ),
     pytest.param(
         {
+            "no_config": False,
             "config": None,
             "url": "testplugin",
         },
         [
             configdir / "primary",
             DeprecatedPath(configdir / "secondary"),
         ],
@@ -120,14 +125,15 @@
             configdir / "primary.testplugin",
         ],
         [],
         id="Default primary config",
     ),
     pytest.param(
         {
+            "no_config": False,
             "config": None,
             "url": "testplugin",
         },
         [
             configdir / "non-existent",
             DeprecatedPath(configdir / "secondary"),
         ],
@@ -147,14 +153,15 @@
                 + f"{configdir / 'secondary.testplugin'}",
             ),
         ],
         id="Default secondary config",
     ),
     pytest.param(
         {
+            "no_config": False,
             "config": [
                 str(configdir / "custom"),
             ],
             "url": "testplugin",
         },
         [
             configdir / "primary",
@@ -165,14 +172,15 @@
             configdir / "primary.testplugin",
         ],
         [],
         id="Custom config with primary plugin",
     ),
     pytest.param(
         {
+            "no_config": False,
             "config": [
                 str(configdir / "custom"),
             ],
             "url": "testplugin",
         },
         [
             configdir / "non-existent",
@@ -189,14 +197,15 @@
                 + f"{configdir / 'secondary.testplugin'}",
             ),
         ],
         id="Custom config with deprecated plugin",
     ),
     pytest.param(
         {
+            "no_config": False,
             "config": [
                 str(configdir / "non-existent"),
                 str(configdir / "primary"),
                 str(configdir / "secondary"),
             ],
             "url": "testplugin",
         },
@@ -208,14 +217,53 @@
             configdir / "secondary",
             configdir / "primary",
             configdir / "primary.testplugin",
         ],
         [],
         id="Multiple custom configs",
     ),
+    pytest.param(
+        {
+            "no_config": True,
+            "config": [],
+            "url": "testplugin",
+        },
+        [],
+        [],
+        [],
+        id="No config",
+    ),
+    pytest.param(
+        {
+            "no_config": True,
+            "config": [
+                str(configdir / "primary"),
+                str(configdir / "secondary"),
+            ],
+            "url": "testplugin",
+        },
+        [],
+        [],
+        [],
+        id="No config with multiple custom configs",
+    ),
+    pytest.param(
+        {
+            "no_config": True,
+            "config": [],
+            "url": "testplugin",
+        },
+        [
+            configdir / "primary",
+            DeprecatedPath(configdir / "secondary"),
+        ],
+        [],
+        [],
+        id="No config with multiple default configs",
+    ),
 ], indirect=["_args", "_config_files"])
 def test_setup_config_args(
     recwarn: pytest.WarningsRecorder,
     setup_args: Mock,
     expected: list,
     deprecations: list,
 ):
```

### Comparing `streamlink-5.4.0/tests/cli/test_streamrunner.py` & `streamlink-5.5.0/tests/cli/test_streamrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 from threading import Thread
 from typing import Callable, Deque, List, Union
 from unittest.mock import Mock, patch
 
 import pytest
 
 from streamlink.stream.stream import StreamIO
-from streamlink_cli.output import FileOutput, PlayerOutput
+from streamlink_cli.output import FileOutput, HTTPOutput, PlayerOutput
 from streamlink_cli.streamrunner import PlayerPollThread, StreamRunner, log as streamrunnerlogger
-from streamlink_cli.utils.http_server import HTTPServer
 from streamlink_cli.utils.progress import Progress
 from tests.testutils.handshake import Handshake
 
 
 TIMEOUT_AWAIT_HANDSHAKE = 1
 TIMEOUT_AWAIT_THREADJOIN = 1
 
@@ -75,18 +74,16 @@
     pass
 
 
 class FakeFileOutput(FakeOutput, FileOutput):
     pass
 
 
-class FakeHTTPServer(FakeOutput, HTTPServer):
-    def __init__(self, *args, **kwargs):
-        with patch("streamlink_cli.utils.http_server.socket"):
-            super().__init__(*args, **kwargs)
+class FakeHTTPOutput(FakeOutput, HTTPOutput):
+    pass
 
 
 class FakeProgress(FakeOutput, Progress):
     # we're not interested in any application logic of the Progress class
     update = print_end = lambda *_, **__: None
 
 
@@ -160,15 +157,15 @@
         player_process.poll = Mock(return_value=None)
 
         return player_process
 
     @pytest.fixture()
     def output(self, player_process: Mock):
         with patch("subprocess.Popen") as mock_popen, \
-             patch("streamlink_cli.output.sleep"):
+             patch("streamlink_cli.output.player.sleep"):
             mock_popen.return_value = player_process
             output = FakePlayerOutput("mocked")
             output.open()
             yield output
             output.close()
 
     @pytest.fixture()
@@ -450,32 +447,32 @@
             ("streamrunner", "info", "Stream ended"),
         ]
 
 
 class TestHTTPServer:
     @pytest.fixture()
     def output(self):
-        return FakeHTTPServer()
+        return FakeHTTPOutput()
 
     @pytest.fixture()
-    def stream_runner(self, stream: FakeStream, output: FakeHTTPServer):
+    def stream_runner(self, stream: FakeStream, output: FakeHTTPOutput):
         stream_runner = StreamRunner(stream, output)
         assert not stream_runner.playerpoller
         assert not stream_runner.progress
         assert stream_runner.is_http
         return stream_runner
 
     @pytest.mark.asyncio()
     async def test_read_write(
         self,
         caplog: pytest.LogCaptureFixture,
         runnerthread: Thread,
         stream_runner: FakeStreamRunner,
         stream: FakeStream,
-        output: FakeHTTPServer,
+        output: FakeHTTPOutput,
     ):
         stream.data.extend((b"foo", b"bar"))
 
         runnerthread.start()
         assert output.data == []
 
         # write prebuffer
@@ -566,22 +563,22 @@
                 id="Player output without record",
             ),
             pytest.param(
                 FakeFileOutput(fd=Mock()),
                 id="FileOutput with file descriptor",
             ),
             pytest.param(
-                FakeHTTPServer(),
+                FakeHTTPOutput(),
                 id="HTTPServer",
             ),
         ],
     )
     def test_no_progress(
         self,
-        output: Union[FakePlayerOutput, FakeFileOutput, FakeHTTPServer],
+        output: Union[FakePlayerOutput, FakeFileOutput, FakeHTTPOutput],
     ):
         stream_runner = FakeStreamRunner(StreamIO(), output, show_progress=True)
         assert not stream_runner.progress
 
     @pytest.mark.parametrize(
         ("output", "expected"),
         [
```

### Comparing `streamlink-5.4.0/tests/cli/utils/test_formatter.py` & `streamlink-5.5.0/tests/cli/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/cli/utils/test_path.py` & `streamlink-5.5.0/tests/cli/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/cli/utils/test_progress.py` & `streamlink-5.5.0/tests/cli/utils/test_progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/cli/utils/test_versioncheck.py` & `streamlink-5.5.0/tests/cli/utils/test_versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/conftest.py` & `streamlink-5.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/mixins/stream_hls.py` & `streamlink-5.5.0/tests/mixins/stream_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugin/testplugin.py` & `streamlink-5.5.0/tests/plugin/testplugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/__init__.py` & `streamlink-5.5.0/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/conftest.py` & `streamlink-5.5.0/tests/plugins/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_abematv.py` & `streamlink-5.5.0/tests/plugins/test_abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_adultswim.py` & `streamlink-5.5.0/tests/plugins/test_adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_afreeca.py` & `streamlink-5.5.0/tests/plugins/test_afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_albavision.py` & `streamlink-5.5.0/tests/plugins/test_albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_aloula.py` & `streamlink-5.5.0/tests/plugins/test_aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_ard_mediathek.py` & `streamlink-5.5.0/tests/plugins/test_ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_artetv.py` & `streamlink-5.5.0/tests/plugins/test_artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_atpchallenger.py` & `streamlink-5.5.0/tests/plugins/test_atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_atresplayer.py` & `streamlink-5.5.0/tests/plugins/test_atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_bbciplayer.py` & `streamlink-5.5.0/tests/plugins/test_bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_bfmtv.py` & `streamlink-5.5.0/tests/plugins/test_bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_bigo.py` & `streamlink-5.5.0/tests/plugins/test_bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_blazetv.py` & `streamlink-5.5.0/tests/plugins/test_blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_bloomberg.py` & `streamlink-5.5.0/tests/plugins/test_bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_booyah.py` & `streamlink-5.5.0/tests/plugins/test_booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_cbsnews.py` & `streamlink-5.5.0/tests/plugins/test_cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_cdnbg.py` & `streamlink-5.5.0/tests/plugins/test_cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_ceskatelevize.py` & `streamlink-5.5.0/tests/plugins/test_ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_cinergroup.py` & `streamlink-5.5.0/tests/plugins/test_cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_cmmedia.py` & `streamlink-5.5.0/tests/plugins/test_cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_crunchyroll.py` & `streamlink-5.5.0/tests/plugins/test_crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_dailymotion.py` & `streamlink-5.5.0/tests/plugins/test_dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_dash.py` & `streamlink-5.5.0/tests/plugins/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_delfi.py` & `streamlink-5.5.0/tests/plugins/test_delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_deutschewelle.py` & `streamlink-5.5.0/tests/plugins/test_deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_dogan.py` & `streamlink-5.5.0/tests/plugins/test_dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_drdk.py` & `streamlink-5.5.0/tests/plugins/test_drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_euronews.py` & `streamlink-5.5.0/tests/plugins/test_euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_facebook.py` & `streamlink-5.5.0/tests/plugins/test_facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_filmon.py` & `streamlink-5.5.0/tests/plugins/test_filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_goltelevision.py` & `streamlink-5.5.0/tests/plugins/test_goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_gulli.py` & `streamlink-5.5.0/tests/plugins/test_gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_htv.py` & `streamlink-5.5.0/tests/plugins/test_htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_idf1.py` & `streamlink-5.5.0/tests/plugins/test_idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_invintus.py` & `streamlink-5.5.0/tests/plugins/test_invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_kugou.py` & `streamlink-5.5.0/tests/plugins/test_kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_livestream.py` & `streamlink-5.5.0/tests/plugins/test_livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_lnk.py` & `streamlink-5.5.0/tests/plugins/test_lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_lrt.py` & `streamlink-5.5.0/tests/plugins/test_lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_ltv_lsm_lv.py` & `streamlink-5.5.0/tests/plugins/test_ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_mdstrm.py` & `streamlink-5.5.0/tests/plugins/test_mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_mediaklikk.py` & `streamlink-5.5.0/tests/plugins/test_mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_mediavitrina.py` & `streamlink-5.5.0/tests/plugins/test_mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_mitele.py` & `streamlink-5.5.0/tests/plugins/test_mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_mixcloud.py` & `streamlink-5.5.0/tests/plugins/test_mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_n13tv.py` & `streamlink-5.5.0/tests/plugins/test_n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_nicolive.py` & `streamlink-5.5.0/tests/plugins/test_nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_nos.py` & `streamlink-5.5.0/tests/plugins/test_nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_nrk.py` & `streamlink-5.5.0/tests/plugins/test_nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_olympicchannel.py` & `streamlink-5.5.0/tests/plugins/test_olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_oneplusone.py` & `streamlink-5.5.0/tests/plugins/test_oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_onetv.py` & `streamlink-5.5.0/tests/plugins/test_onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_pandalive.py` & `streamlink-5.5.0/tests/plugins/test_pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_picarto.py` & `streamlink-5.5.0/tests/plugins/test_picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_pluto.py` & `streamlink-5.5.0/tests/plugins/test_pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_pluzz.py` & `streamlink-5.5.0/tests/plugins/test_pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_radionet.py` & `streamlink-5.5.0/tests/plugins/test_radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_raiplay.py` & `streamlink-5.5.0/tests/plugins/test_raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_reuters.py` & `streamlink-5.5.0/tests/plugins/test_reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_rtbf.py` & `streamlink-5.5.0/tests/plugins/test_rtbf.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_rtpplay.py` & `streamlink-5.5.0/tests/plugins/test_rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_rtve.py` & `streamlink-5.5.0/tests/plugins/test_rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_ruv.py` & `streamlink-5.5.0/tests/plugins/test_ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_sbscokr.py` & `streamlink-5.5.0/tests/plugins/test_sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_showroom.py` & `streamlink-5.5.0/tests/plugins/test_showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_steam.py` & `streamlink-5.5.0/tests/plugins/test_steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_stream.py` & `streamlink-5.5.0/tests/plugins/test_stream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_streann.py` & `streamlink-5.5.0/tests/plugins/test_streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_svtplay.py` & `streamlink-5.5.0/tests/plugins/test_svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_swisstxt.py` & `streamlink-5.5.0/tests/plugins/test_swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_telefe.py` & `streamlink-5.5.0/tests/plugins/test_telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_tf1.py` & `streamlink-5.5.0/tests/plugins/test_tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_trovo.py` & `streamlink-5.5.0/tests/plugins/test_trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_turkuvaz.py` & `streamlink-5.5.0/tests/plugins/test_turkuvaz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_tv4play.py` & `streamlink-5.5.0/tests/plugins/test_tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_tv5monde.py` & `streamlink-5.5.0/tests/plugins/test_tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_tvp.py` & `streamlink-5.5.0/tests/plugins/test_tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_tvrby.py` & `streamlink-5.5.0/tests/plugins/test_tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_tvrplus.py` & `streamlink-5.5.0/tests/plugins/test_tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_twitch.py` & `streamlink-5.5.0/tests/plugins/test_twitch.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_ustreamtv.py` & `streamlink-5.5.0/tests/plugins/test_ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_ustvnow.py` & `streamlink-5.5.0/tests/plugins/test_ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_vimeo.py` & `streamlink-5.5.0/tests/plugins/test_vimeo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_vinhlongtv.py` & `streamlink-5.5.0/tests/plugins/test_vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_vk.py` & `streamlink-5.5.0/tests/plugins/test_vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_vtvgo.py` & `streamlink-5.5.0/tests/plugins/test_vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_webtv.py` & `streamlink-5.5.0/tests/plugins/test_webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_welt.py` & `streamlink-5.5.0/tests/plugins/test_welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_youtube.py` & `streamlink-5.5.0/tests/plugins/test_youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_zattoo.py` & `streamlink-5.5.0/tests/plugins/test_zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_zdf_mediathek.py` & `streamlink-5.5.0/tests/plugins/test_zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/plugins/test_zengatv.py` & `streamlink-5.5.0/tests/plugins/test_zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/__init__.py` & `streamlink-5.5.0/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_1.mpd` & `streamlink-5.5.0/tests/resources/dash/test_1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_10.mpd` & `streamlink-5.5.0/tests/resources/dash/test_10.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_11_static.mpd` & `streamlink-5.5.0/tests/resources/dash/test_11_static.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_2.mpd` & `streamlink-5.5.0/tests/resources/dash/test_2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_3.mpd` & `streamlink-5.5.0/tests/resources/dash/test_3.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_8.mpd` & `streamlink-5.5.0/tests/resources/dash/test_8.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_9.mpd` & `streamlink-5.5.0/tests/resources/dash/test_9.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd` & `streamlink-5.5.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd` & `streamlink-5.5.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_nested_baseurls.mpd` & `streamlink-5.5.0/tests/resources/dash/test_nested_baseurls.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_no_segment_list_or_template.mpd` & `streamlink-5.5.0/tests/resources/dash/test_no_segment_list_or_template.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_segment_list.mpd` & `streamlink-5.5.0/tests/resources/dash/test_segment_list.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_segments_byterange.mpd` & `streamlink-5.5.0/tests/resources/dash/test_segments_byterange.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_segments_dynamic_number.mpd` & `streamlink-5.5.0/tests/resources/dash/test_segments_dynamic_number.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_static_no_publish_time.mpd` & `streamlink-5.5.0/tests/resources/dash/test_static_no_publish_time.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/dash/test_timeline_ids.mpd` & `streamlink-5.5.0/tests/resources/dash/test_timeline_ids.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/hls/test_1.m3u8` & `streamlink-5.5.0/tests/resources/hls/test_1.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/hls/test_2.m3u8` & `streamlink-5.5.0/tests/resources/hls/test_2.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/hls/test_date.m3u8` & `streamlink-5.5.0/tests/resources/hls/test_date.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/hls/test_master.m3u8` & `streamlink-5.5.0/tests/resources/hls/test_master.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/resources/hls/test_master_twitch_vod.m3u8` & `streamlink-5.5.0/tests/resources/hls/test_master_twitch_vod.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/stream/test_dash.py` & `streamlink-5.5.0/tests/stream/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/stream/test_dash_parser.py` & `streamlink-5.5.0/tests/stream/test_dash_parser.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/stream/test_ffmpegmux.py` & `streamlink-5.5.0/tests/stream/test_ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/stream/test_file.py` & `streamlink-5.5.0/tests/stream/test_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/stream/test_hls.py` & `streamlink-5.5.0/tests/stream/test_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/stream/test_hls_filtered.py` & `streamlink-5.5.0/tests/stream/test_hls_filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/stream/test_hls_playlist.py` & `streamlink-5.5.0/tests/stream/test_hls_playlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 def test_split_tag(string: str, expected: Union[Tuple[str, str], Tuple[None, None]]):
     assert M3U8Parser.split_tag(string) == expected
 
 
 @pytest.mark.parametrize(("attributes", "log", "expected"), [
     pytest.param("", False, {}, id="empty attribute list"),
     pytest.param("invalid", True, {}, id="invalid attribute list"),
+    pytest.param("?=VALUE", True, {}, id="invalid attribute name"),
     pytest.param("key=VALUE", True, {}, id="lowercase attribute name"),
-    pytest.param("123=VALUE", True, {}, id="non-alpha attribute name"),
     pytest.param("KEY = VALUE", True, {}, id="invalid attribute format"),
     pytest.param("KEY=", True, {}, id="missing attribute value"),
     pytest.param("KEY=\"", True, {}, id="invalid attribute value"),
     pytest.param("KEY=123", False, {"KEY": "123"}, id="decimal integer"),
     pytest.param("KEY=0xdeadbeef", False, {"KEY": "0xdeadbeef"}, id="hexadecimal sequence, lowercase"),
     pytest.param("KEY=0XDEADBEEF", False, {"KEY": "0XDEADBEEF"}, id="hexadecimal sequence, uppercase"),
     pytest.param("KEY=123.456", False, {"KEY": "123.456"}, id="decimal floating point number"),
@@ -70,14 +70,15 @@
     pytest.param("KEY=\"foobar\"", False, {"KEY": "foobar"}, id="quoted string"),
     pytest.param("KEY=\"foo\"bar\"", True, {}, id="invalid quoted string (quote)"),
     pytest.param("KEY=\"foo\rbar\"", True, {}, id="invalid quoted string (carriage return)"),
     pytest.param("KEY=\"foo\nbar\"", True, {}, id="invalid quoted string (new line)"),
     pytest.param("KEY=VALUE", False, {"KEY": "VALUE"}, id="enumerated string"),
     pytest.param("KEY=<@_@>", False, {"KEY": "<@_@>"}, id="enumerated string with special characters"),
     pytest.param("KEY=1920x1080", False, {"KEY": "1920x1080"}, id="decimal resolution"),
+    pytest.param("KEY-123=VALUE", False, {"KEY-123": "VALUE"}, id="attribute name with alphanumerical chars and dashes"),
     pytest.param(
         "A=123,B=0xdeadbeef,C=123.456,D=-123.456,E=\"value, value, value\",F=VALUE,G=1920x1080",
         False,
         {
             "A": "123",
             "B": "0xdeadbeef",
             "C": "123.456",
```

### Comparing `streamlink-5.4.0/tests/stream/test_stream_json.py` & `streamlink-5.5.0/tests/stream/test_stream_json.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/stream/test_stream_to_url.py` & `streamlink-5.5.0/tests/stream/test_stream_to_url.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/stream/test_stream_wrappers.py` & `streamlink-5.5.0/tests/stream/test_stream_wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/test_api_http_session.py` & `streamlink-5.5.0/tests/test_api_http_session.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/test_api_validate.py` & `streamlink-5.5.0/tests/test_api_validate.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/test_api_websocket.py` & `streamlink-5.5.0/tests/test_api_websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/test_buffers.py` & `streamlink-5.5.0/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/test_cache.py` & `streamlink-5.5.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/test_logger.py` & `streamlink-5.5.0/tests/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,20 @@
 def log(request, output: StringIO):
     params = getattr(request, "param", {})
     params.setdefault("format", "[{name}][{levelname}] {message}")
     params.setdefault("style", "{")
     fakeroot = logging.getLogger("streamlink.test")
     with patch("streamlink.logger.root", fakeroot), \
          patch("streamlink.utils.times.LOCAL", timezone.utc):
-        logger.basicConfig(stream=output, **params)
+        handler = logger.basicConfig(stream=output, **params)
+        assert isinstance(handler, logging.Handler)
         yield fakeroot
         logger.capturewarnings(False)
+        fakeroot.removeHandler(handler)
+        assert not fakeroot.handlers
 
 
 class TestLogging:
     @pytest.fixture()
     def log_failure(self, request, log: logging.Logger, output: StringIO):
         params = getattr(request, "param", {})
         root = logging.getLogger("streamlink")
```

### Comparing `streamlink-5.4.0/tests/test_options.py` & `streamlink-5.5.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/test_plugin.py` & `streamlink-5.5.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/test_plugin_userinput.py` & `streamlink-5.5.0/tests/test_plugin_userinput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/test_plugins.py` & `streamlink-5.5.0/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/test_session.py` & `streamlink-5.5.0/tests/test_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from pathlib import Path
 from socket import AF_INET, AF_INET6
 from unittest.mock import Mock, call, patch
 
 import pytest
 import requests_mock
 import urllib3
+from requests.adapters import HTTPAdapter
 
 import tests.plugin
 from streamlink.exceptions import NoPluginError, StreamlinkDeprecationWarning
 from streamlink.plugin import HIGH_PRIORITY, LOW_PRIORITY, NO_PRIORITY, NORMAL_PRIORITY, Plugin, pluginmatcher
+from streamlink.plugin.api.http_session import TLSNoDHAdapter
 from streamlink.session import Streamlink
 from streamlink.stream.hls import HLSStream
 from streamlink.stream.http import HTTPStream
 
 
 PATH_TESTPLUGINS = Path(tests.plugin.__path__[0])
 PATH_TESTPLUGINS_OVERRIDE = PATH_TESTPLUGINS / "override"
@@ -390,27 +392,25 @@
 
         session.set_option("ipv4", True)
         session.set_option("ipv6", False)
         assert session.get_option("ipv4") is True
         assert session.get_option("ipv6") is False
         assert mock_urllib3_util_connection.allowed_gai_family is _original_allowed_gai_family
 
-    @patch("streamlink.session.urllib3_util_ssl", DEFAULT_CIPHERS="foo:!bar:baz")
-    def test_http_disable_dh(self, mock_urllib3_util_ssl):
+    def test_http_disable_dh(self):
         session = self.subject(load_plugins=False)
-        assert mock_urllib3_util_ssl.DEFAULT_CIPHERS == "foo:!bar:baz"
+        assert isinstance(session.http.adapters["https://"], HTTPAdapter)
+        assert not isinstance(session.http.adapters["https://"], TLSNoDHAdapter)
 
         session.set_option("http-disable-dh", True)
-        assert mock_urllib3_util_ssl.DEFAULT_CIPHERS == "foo:!bar:baz:!DH"
-
-        session.set_option("http-disable-dh", True)
-        assert mock_urllib3_util_ssl.DEFAULT_CIPHERS == "foo:!bar:baz:!DH"
+        assert isinstance(session.http.adapters["https://"], TLSNoDHAdapter)
 
         session.set_option("http-disable-dh", False)
-        assert mock_urllib3_util_ssl.DEFAULT_CIPHERS == "foo:!bar:baz"
+        assert isinstance(session.http.adapters["https://"], HTTPAdapter)
+        assert not isinstance(session.http.adapters["https://"], TLSNoDHAdapter)
 
 
 class TestSessionOptionHttpProxy:
     @pytest.fixture()
     def _no_deprecation(self, recwarn: pytest.WarningsRecorder):
         yield
         assert recwarn.list == []
```

### Comparing `streamlink-5.4.0/tests/test_streamlink_api.py` & `streamlink-5.5.0/tests/test_streamlink_api.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/testutils/handshake.py` & `streamlink-5.5.0/tests/testutils/handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/testutils/test_handshake.py` & `streamlink-5.5.0/tests/testutils/test_handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_args.py` & `streamlink-5.5.0/tests/utils/test_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_cache.py` & `streamlink-5.5.0/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_crypto.py` & `streamlink-5.5.0/tests/utils/test_crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_data.py` & `streamlink-5.5.0/tests/utils/test_data.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_formatter.py` & `streamlink-5.5.0/tests/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_l10n.py` & `streamlink-5.5.0/tests/utils/test_l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_module.py` & `streamlink-5.5.0/tests/utils/test_module.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_named_pipe.py` & `streamlink-5.5.0/tests/utils/test_named_pipe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_parse.py` & `streamlink-5.5.0/tests/utils/test_parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_processoutput.py` & `streamlink-5.5.0/tests/utils/test_processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_times.py` & `streamlink-5.5.0/tests/utils/test_times.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.4.0/tests/utils/test_url.py` & `streamlink-5.5.0/tests/utils/test_url.py`

 * *Files identical despite different names*

